# Comparing `tmp/libschrodinger-1.0.4rc1.tar.gz` & `tmp/libschrodinger-1.0.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libschrodinger-1.0.4rc1.tar", last modified: Thu May 30 20:35:35 2024, max compression
+gzip compressed data, was "libschrodinger-1.0.4rc2.tar", last modified: Thu May 30 20:42:00 2024, max compression
```

## Comparing `libschrodinger-1.0.4rc1.tar` & `libschrodinger-1.0.4rc2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:35:35.394228 libschrodinger-1.0.4rc1/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.0.4rc1/LICENSE
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1448 2024-05-30 20:35:35.393598 libschrodinger-1.0.4rc1/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.0.4rc1/README.md
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:35:35.390998 libschrodinger-1.0.4rc1/libschrodinger/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      247 2024-05-30 20:13:20.000000 libschrodinger-1.0.4rc1/libschrodinger/__init__.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/config.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.0.4rc1/libschrodinger/constants.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5031 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/electron.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/figlocation.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2816 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/gauss.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4636 2024-05-30 20:14:06.000000 libschrodinger-1.0.4rc1/libschrodinger/graphs.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      922 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/interaction.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2053 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/particle.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/potential.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      899 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc1/libschrodinger/waveutils.py
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:35:35.393073 libschrodinger-1.0.4rc1/libschrodinger.egg-info/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1448 2024-05-30 20:35:35.000000 libschrodinger-1.0.4rc1/libschrodinger.egg-info/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      483 2024-05-30 20:35:35.000000 libschrodinger-1.0.4rc1/libschrodinger.egg-info/SOURCES.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 20:35:35.000000 libschrodinger-1.0.4rc1/libschrodinger.egg-info/dependency_links.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-30 20:35:35.000000 libschrodinger-1.0.4rc1/libschrodinger.egg-info/top_level.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:35:31.000000 libschrodinger-1.0.4rc1/pyproject.toml
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 20:35:35.394351 libschrodinger-1.0.4rc1/setup.cfg
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:42:00.175303 libschrodinger-1.0.4rc2/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.0.4rc2/LICENSE
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1516 2024-05-30 20:42:00.174882 libschrodinger-1.0.4rc2/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.0.4rc2/README.md
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:42:00.172088 libschrodinger-1.0.4rc2/libschrodinger/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      247 2024-05-30 20:13:20.000000 libschrodinger-1.0.4rc2/libschrodinger/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/config.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.0.4rc2/libschrodinger/constants.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5031 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/electron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/figlocation.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2816 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/gauss.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4636 2024-05-30 20:14:06.000000 libschrodinger-1.0.4rc2/libschrodinger/graphs.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      922 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/interaction.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2053 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/particle.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/potential.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      899 2024-05-30 20:12:35.000000 libschrodinger-1.0.4rc2/libschrodinger/waveutils.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:42:00.174355 libschrodinger-1.0.4rc2/libschrodinger.egg-info/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1516 2024-05-30 20:42:00.000000 libschrodinger-1.0.4rc2/libschrodinger.egg-info/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      520 2024-05-30 20:42:00.000000 libschrodinger-1.0.4rc2/libschrodinger.egg-info/SOURCES.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 20:42:00.000000 libschrodinger-1.0.4rc2/libschrodinger.egg-info/dependency_links.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-05-30 20:42:00.000000 libschrodinger-1.0.4rc2/libschrodinger.egg-info/requires.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-30 20:42:00.000000 libschrodinger-1.0.4rc2/libschrodinger.egg-info/top_level.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      854 2024-05-30 20:41:23.000000 libschrodinger-1.0.4rc2/pyproject.toml
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 20:42:00.175381 libschrodinger-1.0.4rc2/setup.cfg
```

### Comparing `libschrodinger-1.0.4rc1/LICENSE` & `libschrodinger-1.0.4rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/PKG-INFO` & `libschrodinger-1.0.4rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.0.4rc1
+Version: 1.0.4rc2
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
 
 # A Python script to solve the Schrodinger's equation in a 2D domain.
 
 ![schreenshot showing app UI where people can create and edit particles](https://github.com/1p22geo/schrodinger/raw/master/static/media/png/screenshot.png)
 
 ## Static deployment
```

### Comparing `libschrodinger-1.0.4rc1/README.md` & `libschrodinger-1.0.4rc2/README.md`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/config.py` & `libschrodinger-1.0.4rc2/libschrodinger/config.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/constants.py` & `libschrodinger-1.0.4rc2/libschrodinger/constants.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/electron.py` & `libschrodinger-1.0.4rc2/libschrodinger/electron.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/figlocation.py` & `libschrodinger-1.0.4rc2/libschrodinger/figlocation.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/gauss.py` & `libschrodinger-1.0.4rc2/libschrodinger/gauss.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/graphs.py` & `libschrodinger-1.0.4rc2/libschrodinger/graphs.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/interaction.py` & `libschrodinger-1.0.4rc2/libschrodinger/interaction.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/particle.py` & `libschrodinger-1.0.4rc2/libschrodinger/particle.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/potential.py` & `libschrodinger-1.0.4rc2/libschrodinger/potential.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger/waveutils.py` & `libschrodinger-1.0.4rc2/libschrodinger/waveutils.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.4rc1/libschrodinger.egg-info/PKG-INFO` & `libschrodinger-1.0.4rc2/libschrodinger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.0.4rc1
+Version: 1.0.4rc2
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3) 
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
 
 # A Python script to solve the Schrodinger's equation in a 2D domain.
 
 ![schreenshot showing app UI where people can create and edit particles](https://github.com/1p22geo/schrodinger/raw/master/static/media/png/screenshot.png)
 
 ## Static deployment
```

