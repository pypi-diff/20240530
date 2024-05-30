# Comparing `tmp/libschrodinger-1.0.1.tar.gz` & `tmp/libschrodinger-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libschrodinger-1.0.1.tar", last modified: Thu May 30 19:48:06 2024, max compression
+gzip compressed data, was "libschrodinger-1.0.2.tar", last modified: Thu May 30 20:06:59 2024, max compression
```

## Comparing `libschrodinger-1.0.1.tar` & `libschrodinger-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 19:48:06.360918 libschrodinger-1.0.1/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.0.1/LICENSE
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 19:48:06.360594 libschrodinger-1.0.1/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.0.1/README.md
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 19:48:06.358529 libschrodinger-1.0.1/lib/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      236 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/__init__.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/config.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      651 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/constants.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4899 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/electron.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/figlocation.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2728 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/gauss.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4515 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/graphs.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      812 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/interaction.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1954 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/particle.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2987 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/potential.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      866 2024-05-30 09:54:56.000000 libschrodinger-1.0.1/lib/waveutils.py
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 19:48:06.360164 libschrodinger-1.0.1/libschrodinger.egg-info/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 19:48:06.000000 libschrodinger-1.0.1/libschrodinger.egg-info/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      362 2024-05-30 19:48:06.000000 libschrodinger-1.0.1/libschrodinger.egg-info/SOURCES.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 19:48:06.000000 libschrodinger-1.0.1/libschrodinger.egg-info/dependency_links.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        4 2024-05-30 19:48:06.000000 libschrodinger-1.0.1/libschrodinger.egg-info/top_level.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      622 2024-05-30 19:47:12.000000 libschrodinger-1.0.1/pyproject.toml
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 19:48:06.360987 libschrodinger-1.0.1/setup.cfg
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:06:59.749455 libschrodinger-1.0.2/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.0.2/LICENSE
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 20:06:59.749029 libschrodinger-1.0.2/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.0.2/README.md
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:06:59.746284 libschrodinger-1.0.2/libschrodinger/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      236 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/config.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      651 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/constants.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4899 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/electron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/figlocation.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2728 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/gauss.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4515 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/graphs.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      812 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/interaction.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1954 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/particle.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2987 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/potential.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      866 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/waveutils.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:06:59.748536 libschrodinger-1.0.2/libschrodinger.egg-info/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      483 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/SOURCES.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/dependency_links.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/top_level.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      633 2024-05-30 20:06:52.000000 libschrodinger-1.0.2/pyproject.toml
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 20:06:59.749555 libschrodinger-1.0.2/setup.cfg
```

### Comparing `libschrodinger-1.0.1/LICENSE` & `libschrodinger-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/PKG-INFO` & `libschrodinger-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.0.1/README.md` & `libschrodinger-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/config.py` & `libschrodinger-1.0.2/libschrodinger/config.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/constants.py` & `libschrodinger-1.0.2/libschrodinger/constants.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/electron.py` & `libschrodinger-1.0.2/libschrodinger/electron.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/figlocation.py` & `libschrodinger-1.0.2/libschrodinger/figlocation.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/gauss.py` & `libschrodinger-1.0.2/libschrodinger/gauss.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/graphs.py` & `libschrodinger-1.0.2/libschrodinger/graphs.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/interaction.py` & `libschrodinger-1.0.2/libschrodinger/interaction.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/particle.py` & `libschrodinger-1.0.2/libschrodinger/particle.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/potential.py` & `libschrodinger-1.0.2/libschrodinger/potential.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/lib/waveutils.py` & `libschrodinger-1.0.2/libschrodinger/waveutils.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.1/libschrodinger.egg-info/PKG-INFO` & `libschrodinger-1.0.2/libschrodinger.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.0.1
+Version: 1.0.2
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.0.1/pyproject.toml` & `libschrodinger-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libschrodinger"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="1p22geo", email="1p22geodecki@gmail.com" },
   { name="KacperTZSTI", email="kacper.m.trzop@gmail.com" },
 ]
 description = "A small package for simulating quantum-scale physics."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -15,8 +15,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/1p22geo/schrodinger"
 Issues = "https://github.com/1p22geo/schrodinger/issues"
 
 [tool.setuptools.packages.find]
-include = ["lib"]
+include = ["libschrodinger"]
```

