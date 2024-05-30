# Comparing `tmp/napari_cosmos_ts-0.1.3.tar.gz` & `tmp/napari_cosmos_ts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_cosmos_ts-0.1.3.tar", last modified: Mon May  6 21:03:44 2024, max compression
+gzip compressed data, was "napari_cosmos_ts-0.1.4.tar", last modified: Thu May 30 15:08:38 2024, max compression
```

## Comparing `napari_cosmos_ts-0.1.3.tar` & `napari_cosmos_ts-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2024-04-04 20:40:34.143863 napari_cosmos_ts-0.1.3/LICENSE
--rw-r--r--   0        0        0     1852 2024-04-22 14:05:21.046015 napari_cosmos_ts-0.1.3/README.md
--rw-r--r--   0        0        0     1177 2024-05-06 21:03:44.087463 napari_cosmos_ts-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 15:49:27.422300 napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/__init__.py
--rw-r--r--   0        0        0    87724 2024-05-06 20:49:23.297635 napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/main_widget.py
--rw-r--r--   0        0        0      311 2024-04-11 15:00:04.753800 napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/napari.yaml
--rw-r--r--   0        0        0        0 2024-04-09 15:49:27.423781 napari_cosmos_ts-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2751 1970-01-01 00:00:00.000000 napari_cosmos_ts-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-04 20:40:34.143863 napari_cosmos_ts-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1852 2024-04-22 14:05:21.046015 napari_cosmos_ts-0.1.4/README.md
+-rw-r--r--   0        0        0     1216 2024-05-30 15:08:38.552846 napari_cosmos_ts-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 15:49:27.422300 napari_cosmos_ts-0.1.4/src/napari_cosmos_ts/__init__.py
+-rw-r--r--   0        0        0    87724 2024-05-06 20:49:23.297635 napari_cosmos_ts-0.1.4/src/napari_cosmos_ts/main_widget.py
+-rw-r--r--   0        0        0      311 2024-04-11 15:00:04.753800 napari_cosmos_ts-0.1.4/src/napari_cosmos_ts/napari.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 15:49:27.423781 napari_cosmos_ts-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 napari_cosmos_ts-0.1.4/PKG-INFO
```

### Comparing `napari_cosmos_ts-0.1.3/LICENSE` & `napari_cosmos_ts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_cosmos_ts-0.1.3/README.md` & `napari_cosmos_ts-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `napari_cosmos_ts-0.1.3/pyproject.toml` & `napari_cosmos_ts-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "napari-cosmos-ts"
 description = "napari plugin for colocalization single-molecule spectroscopy (CoSMoS) time series (TS) analysis"
 authors = [
+    { name = "Marcel Goldschen-Ohm" },
     { name = "Marcel Goldschen-Ohm", email = "goldschen-ohm@utexas.edu" },
 ]
 dependencies = [
     "napari>=0.4.19.post1",
     "pyqtgraph>=0.13.4",
     "pystackreg>=0.2.7",
     "pycpd>=2.0.0",
@@ -16,15 +17,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Framework :: napari",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.1.3"
+version = "0.1.4"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."napari.manifest"]
 napari-cosmos-ts = "napari_cosmos_ts:napari.yaml"
```

### Comparing `napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/main_widget.py` & `napari_cosmos_ts-0.1.4/src/napari_cosmos_ts/main_widget.py`

 * *Files identical despite different names*

### Comparing `napari_cosmos_ts-0.1.3/PKG-INFO` & `napari_cosmos_ts-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: napari-cosmos-ts
-Version: 0.1.3
+Version: 0.1.4
 Summary: napari plugin for colocalization single-molecule spectroscopy (CoSMoS) time series (TS) analysis
 Home-page: https://github.com/marcel-goldschen-ohm/napari-cosmos-ts
+Author: Marcel Goldschen-Ohm
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: napari
 Classifier: Programming Language :: Python :: 3 :: Only
```

