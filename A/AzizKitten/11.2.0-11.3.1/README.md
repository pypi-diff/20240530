# Comparing `tmp/azizkitten-11.2.0.tar.gz` & `tmp/azizkitten-11.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azizkitten-11.2.0.tar", last modified: Sat May 25 15:42:04 2024, max compression
+gzip compressed data, was "azizkitten-11.3.1.tar", last modified: Thu May 30 15:51:29 2024, max compression
```

## Comparing `azizkitten-11.2.0.tar` & `azizkitten-11.3.1.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 15:42:04.808017 azizkitten-11.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-25 15:42:04.798017 azizkitten-11.2.0/AzizKitten/
--rw-rw-rw-   0        0        0      986 2024-05-25 15:34:10.000000 azizkitten-11.2.0/AzizKitten/__init__.py
--rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.2.0/AzizKitten/acos.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.2.0/AzizKitten/acot.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.2.0/AzizKitten/acsc.py
--rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.2.0/AzizKitten/among_us.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.2.0/AzizKitten/asec.py
--rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.2.0/AzizKitten/asin.py
--rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.2.0/AzizKitten/atan.py
--rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.2.0/AzizKitten/bin_rep.py
--rw-rw-rw-   0        0        0     2226 2024-05-20 18:59:59.000000 azizkitten-11.2.0/AzizKitten/cbrt.py
--rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.2.0/AzizKitten/constants.py
--rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.2.0/AzizKitten/cos.py
--rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.2.0/AzizKitten/cosh.py
--rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.2.0/AzizKitten/cot.py
--rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.2.0/AzizKitten/coth.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.2.0/AzizKitten/csc.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.2.0/AzizKitten/csch.py
--rw-rw-rw-   0        0        0     2799 2024-05-25 15:33:55.000000 azizkitten-11.2.0/AzizKitten/cubic.py
--rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.2.0/AzizKitten/degrees.py
--rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.2.0/AzizKitten/exp.py
--rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.2.0/AzizKitten/factorial.py
--rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.2.0/AzizKitten/floor.py
--rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.2.0/AzizKitten/gcd.py
--rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.2.0/AzizKitten/integrate.py
--rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.2.0/AzizKitten/lcm.py
--rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.2.0/AzizKitten/limit.py
--rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.2.0/AzizKitten/ln.py
--rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.2.0/AzizKitten/log.py
--rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.2.0/AzizKitten/ment_calc.py
--rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.2.0/AzizKitten/mystery.py
--rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.2.0/AzizKitten/quad.py
--rw-rw-rw-   0        0        0     1461 2024-05-25 15:33:42.000000 azizkitten-11.2.0/AzizKitten/quartic.py
--rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.2.0/AzizKitten/radians.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.2.0/AzizKitten/sec.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.2.0/AzizKitten/sech.py
--rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.2.0/AzizKitten/sin.py
--rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.2.0/AzizKitten/sinh.py
--rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.2.0/AzizKitten/sqrt.py
--rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.2.0/AzizKitten/tan.py
--rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.2.0/AzizKitten/tanh.py
-drwxrwxrwx   0        0        0        0 2024-05-25 15:42:04.805017 azizkitten-11.2.0/AzizKitten.egg-info/
--rw-rw-rw-   0        0        0      785 2024-05-25 15:42:04.000000 azizkitten-11.2.0/AzizKitten.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2024-05-25 15:42:04.000000 azizkitten-11.2.0/AzizKitten.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 15:42:04.000000 azizkitten-11.2.0/AzizKitten.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-25 15:42:04.000000 azizkitten-11.2.0/AzizKitten.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.2.0/LICENSE
--rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      785 2024-05-25 15:42:04.805995 azizkitten-11.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.2.0/README.md
--rw-rw-rw-   0        0        0      673 2024-05-25 15:39:32.000000 azizkitten-11.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 15:42:04.808017 azizkitten-11.2.0/setup.cfg
--rw-rw-rw-   0        0        0      708 2024-05-25 15:39:38.000000 azizkitten-11.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:51:29.459638 azizkitten-11.3.1/
+drwxrwxrwx   0        0        0        0 2024-05-30 15:51:29.445505 azizkitten-11.3.1/AzizKitten/
+-rw-rw-rw-   0        0        0      960 2024-05-30 15:46:47.000000 azizkitten-11.3.1/AzizKitten/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.3.1/AzizKitten/acos.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.3.1/AzizKitten/acot.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.3.1/AzizKitten/acsc.py
+-rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.3.1/AzizKitten/among_us.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.3.1/AzizKitten/asec.py
+-rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.3.1/AzizKitten/asin.py
+-rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.3.1/AzizKitten/atan.py
+-rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.3.1/AzizKitten/bin_rep.py
+-rw-rw-rw-   0        0        0     2226 2024-05-20 18:59:59.000000 azizkitten-11.3.1/AzizKitten/cbrt.py
+-rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.3.1/AzizKitten/constants.py
+-rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.3.1/AzizKitten/cos.py
+-rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.3.1/AzizKitten/cosh.py
+-rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.3.1/AzizKitten/cot.py
+-rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.3.1/AzizKitten/coth.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.3.1/AzizKitten/csc.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.3.1/AzizKitten/csch.py
+-rw-rw-rw-   0        0        0     2799 2024-05-25 15:33:55.000000 azizkitten-11.3.1/AzizKitten/cubic.py
+-rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.3.1/AzizKitten/degrees.py
+-rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.3.1/AzizKitten/exp.py
+-rw-rw-rw-   0        0        0      481 2024-05-30 15:43:10.000000 azizkitten-11.3.1/AzizKitten/factorial.py
+-rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.3.1/AzizKitten/floor.py
+-rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.3.1/AzizKitten/gcd.py
+-rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.3.1/AzizKitten/integrate.py
+-rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.3.1/AzizKitten/lcm.py
+-rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.3.1/AzizKitten/ln.py
+-rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.3.1/AzizKitten/log.py
+-rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.3.1/AzizKitten/ment_calc.py
+-rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.3.1/AzizKitten/mystery.py
+-rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.3.1/AzizKitten/quad.py
+-rw-rw-rw-   0        0        0     1461 2024-05-25 15:33:42.000000 azizkitten-11.3.1/AzizKitten/quartic.py
+-rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.3.1/AzizKitten/radians.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.3.1/AzizKitten/sec.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.3.1/AzizKitten/sech.py
+-rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.3.1/AzizKitten/sin.py
+-rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.3.1/AzizKitten/sinh.py
+-rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.3.1/AzizKitten/sqrt.py
+-rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.3.1/AzizKitten/tan.py
+-rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.3.1/AzizKitten/tanh.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:51:29.456637 azizkitten-11.3.1/AzizKitten.egg-info/
+-rw-rw-rw-   0        0        0      785 2024-05-30 15:51:29.000000 azizkitten-11.3.1/AzizKitten.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      963 2024-05-30 15:51:29.000000 azizkitten-11.3.1/AzizKitten.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:51:29.000000 azizkitten-11.3.1/AzizKitten.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-30 15:51:29.000000 azizkitten-11.3.1/AzizKitten.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.3.1/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      785 2024-05-30 15:51:29.457639 azizkitten-11.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.3.1/README.md
+-rw-rw-rw-   0        0        0      673 2024-05-30 15:50:51.000000 azizkitten-11.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 15:51:29.459638 azizkitten-11.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-30 15:50:48.000000 azizkitten-11.3.1/setup.py
```

### Comparing `azizkitten-11.2.0/AzizKitten/__init__.py` & `azizkitten-11.3.1/AzizKitten/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from .coth import coth
 from .sech import sech
 from .csch import csch
 from .floor import floor
 from .exp import exp
 from .factorial import factorial
 from .integrate import integrate
-from .limit import limit
 from .ln import ln
 from .log import log
 from .radians import radians
 from .degrees import degrees
 from .cbrt import cbrt
 from .cubic import cubic
 from .quartic import quartic
```

### Comparing `azizkitten-11.2.0/AzizKitten/among_us.py` & `azizkitten-11.3.1/AzizKitten/among_us.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/cbrt.py` & `azizkitten-11.3.1/AzizKitten/cbrt.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/cubic.py` & `azizkitten-11.3.1/AzizKitten/cubic.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/integrate.py` & `azizkitten-11.3.1/AzizKitten/integrate.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/ln.py` & `azizkitten-11.3.1/AzizKitten/ln.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/ment_calc.py` & `azizkitten-11.3.1/AzizKitten/ment_calc.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/mystery.py` & `azizkitten-11.3.1/AzizKitten/mystery.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/quad.py` & `azizkitten-11.3.1/AzizKitten/quad.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten/quartic.py` & `azizkitten-11.3.1/AzizKitten/quartic.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/AzizKitten.egg-info/SOURCES.txt` & `azizkitten-11.3.1/AzizKitten.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 AzizKitten/degrees.py
 AzizKitten/exp.py
 AzizKitten/factorial.py
 AzizKitten/floor.py
 AzizKitten/gcd.py
 AzizKitten/integrate.py
 AzizKitten/lcm.py
-AzizKitten/limit.py
 AzizKitten/ln.py
 AzizKitten/log.py
 AzizKitten/ment_calc.py
 AzizKitten/mystery.py
 AzizKitten/quad.py
 AzizKitten/quartic.py
 AzizKitten/radians.py
```

### Comparing `azizkitten-11.2.0/LICENSE` & `azizkitten-11.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azizkitten-11.2.0/pyproject.toml` & `azizkitten-11.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AzizKitten"
-version = "11.2.0"
+version = "11.3.1"
 authors = [
   { name="AzizKitten", email="azizprv43@gmail.com" },
 ]
 description = "AzizOmrane's own Python package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `azizkitten-11.2.0/setup.py` & `azizkitten-11.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AzizKitten",
-    version="11.2.0",
+    version="11.3.1",
     packages=find_packages(),
     include_package_data=True,
     author="AzizKitten",
     author_email="azizprv43@gmail.com",
     description="AzizOmrane's own python library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

