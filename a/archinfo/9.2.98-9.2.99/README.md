# Comparing `tmp/archinfo-9.2.98.tar.gz` & `tmp/archinfo-9.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archinfo-9.2.98.tar", last modified: Tue Apr  9 17:02:02 2024, max compression
+gzip compressed data, was "archinfo-9.2.99.tar", last modified: Tue Apr 16 17:01:59 2024, max compression
```

## Comparing `archinfo-9.2.98.tar` & `archinfo-9.2.99.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:02.680538 archinfo-9.2.98/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-09 17:01:24.000000 archinfo-9.2.98/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-04-09 17:01:24.000000 archinfo-9.2.98/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1875 2024-04-09 17:02:02.680538 archinfo-9.2.98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-04-09 17:01:24.000000 archinfo-9.2.98/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:02.676538 archinfo-9.2.98/archinfo/
--rw-r--r--   0 vsts      (1001) docker     (127)     1520 2024-04-09 17:01:43.000000 archinfo-9.2.98/archinfo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35350 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16843 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_aarch64.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17691 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_amd64.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28764 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_arm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5696 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_avr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12496 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_mips32.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9623 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_mips64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5662 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_pcode.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15734 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_ppc32.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17938 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_ppc64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7625 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_riscv64.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9367 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_s390x.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11449 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_soot.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12490 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/arch_x86.py
--rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/archerror.py
--rw-r--r--   0 vsts      (1001) docker     (127)    62561 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/defines.py
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1010 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/tls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1334 2024-04-09 17:01:24.000000 archinfo-9.2.98/archinfo/types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:02.676538 archinfo-9.2.98/archinfo.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1875 2024-04-09 17:02:02.000000 archinfo-9.2.98/archinfo.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-09 17:02:02.000000 archinfo-9.2.98/archinfo.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 17:02:02.000000 archinfo-9.2.98/archinfo.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-09 17:02:02.000000 archinfo-9.2.98/archinfo.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-09 17:02:02.000000 archinfo-9.2.98/archinfo.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-04-09 17:01:43.000000 archinfo-9.2.98/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      999 2024-04-09 17:02:02.680538 archinfo-9.2.98/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:02.676538 archinfo-9.2.98/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     2945 2024-04-09 17:01:24.000000 archinfo-9.2.98/tests/test_amd64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      762 2024-04-09 17:01:24.000000 archinfo-9.2.98/tests/test_pcode.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-09 17:01:24.000000 archinfo-9.2.98/tests/test_register.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:58.993562 archinfo-9.2.99/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-16 17:01:25.000000 archinfo-9.2.99/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       34 2024-04-16 17:01:25.000000 archinfo-9.2.99/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1875 2024-04-16 17:01:58.993562 archinfo-9.2.99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      735 2024-04-16 17:01:25.000000 archinfo-9.2.99/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:58.985562 archinfo-9.2.99/archinfo/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1520 2024-04-16 17:01:35.000000 archinfo-9.2.99/archinfo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35350 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16843 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_aarch64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17691 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28764 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_arm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5696 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_avr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12496 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_mips32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9623 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_mips64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5662 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_pcode.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15734 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_ppc32.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17938 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_ppc64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7625 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_riscv64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9367 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_s390x.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11449 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_soot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12490 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/arch_x86.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/archerror.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    62561 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/defines.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1010 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/tls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1334 2024-04-16 17:01:25.000000 archinfo-9.2.99/archinfo/types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:58.989562 archinfo-9.2.99/archinfo.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1875 2024-04-16 17:01:58.000000 archinfo-9.2.99/archinfo.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-16 17:01:58.000000 archinfo-9.2.99/archinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 17:01:58.000000 archinfo-9.2.99/archinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-16 17:01:58.000000 archinfo-9.2.99/archinfo.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-16 17:01:58.000000 archinfo-9.2.99/archinfo.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-04-16 17:01:35.000000 archinfo-9.2.99/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      999 2024-04-16 17:01:58.993562 archinfo-9.2.99/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:01:58.989562 archinfo-9.2.99/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2945 2024-04-16 17:01:25.000000 archinfo-9.2.99/tests/test_amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      762 2024-04-16 17:01:25.000000 archinfo-9.2.99/tests/test_pcode.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-16 17:01:25.000000 archinfo-9.2.99/tests/test_register.py
```

### Comparing `archinfo-9.2.98/LICENSE` & `archinfo-9.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/PKG-INFO` & `archinfo-9.2.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archinfo
-Version: 9.2.98
+Version: 9.2.99
 Summary: Classes with architecture-specific information useful to other projects.
 Home-page: https://github.com/angr/archinfo
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `archinfo-9.2.98/README.md` & `archinfo-9.2.99/README.md`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/__init__.py` & `archinfo-9.2.99/archinfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=wrong-import-position
 """
 archinfo is a collection of classes that contain architecture-specific information.
 It is useful for cross-architecture tools (such as pyvex).
 """
 
-__version__ = "9.2.98"
+__version__ = "9.2.99"
 
 
 from .arch import (
     Arch,
     ArchNotFound,
     Register,
     all_arches,
```

### Comparing `archinfo-9.2.98/archinfo/arch.py` & `archinfo-9.2.99/archinfo/arch.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_aarch64.py` & `archinfo-9.2.99/archinfo/arch_aarch64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_amd64.py` & `archinfo-9.2.99/archinfo/arch_amd64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_arm.py` & `archinfo-9.2.99/archinfo/arch_arm.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_avr.py` & `archinfo-9.2.99/archinfo/arch_avr.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_mips32.py` & `archinfo-9.2.99/archinfo/arch_mips32.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_mips64.py` & `archinfo-9.2.99/archinfo/arch_mips64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_pcode.py` & `archinfo-9.2.99/archinfo/arch_pcode.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_ppc32.py` & `archinfo-9.2.99/archinfo/arch_ppc32.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_ppc64.py` & `archinfo-9.2.99/archinfo/arch_ppc64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_riscv64.py` & `archinfo-9.2.99/archinfo/arch_riscv64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_s390x.py` & `archinfo-9.2.99/archinfo/arch_s390x.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_soot.py` & `archinfo-9.2.99/archinfo/arch_soot.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/arch_x86.py` & `archinfo-9.2.99/archinfo/arch_x86.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/defines.py` & `archinfo-9.2.99/archinfo/defines.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/tls.py` & `archinfo-9.2.99/archinfo/tls.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo/types.py` & `archinfo-9.2.99/archinfo/types.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/archinfo.egg-info/PKG-INFO` & `archinfo-9.2.99/archinfo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archinfo
-Version: 9.2.98
+Version: 9.2.99
 Summary: Classes with architecture-specific information useful to other projects.
 Home-page: https://github.com/angr/archinfo
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `archinfo-9.2.98/archinfo.egg-info/SOURCES.txt` & `archinfo-9.2.99/archinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/setup.cfg` & `archinfo-9.2.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/tests/test_amd64.py` & `archinfo-9.2.99/tests/test_amd64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/tests/test_pcode.py` & `archinfo-9.2.99/tests/test_pcode.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.98/tests/test_register.py` & `archinfo-9.2.99/tests/test_register.py`

 * *Files identical despite different names*

