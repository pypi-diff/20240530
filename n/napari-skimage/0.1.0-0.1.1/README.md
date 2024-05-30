# Comparing `tmp/napari_skimage-0.1.0.tar.gz` & `tmp/napari_skimage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_skimage-0.1.0.tar", last modified: Wed May 29 21:11:20 2024, max compression
+gzip compressed data, was "napari_skimage-0.1.1.tar", last modified: Wed May 29 21:24:09 2024, max compression
```

## Comparing `napari_skimage-0.1.0.tar` & `napari_skimage-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.558924 napari_skimage-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.546923 napari_skimage-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.550924 napari_skimage-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.550924 napari_skimage-0.1.0/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-29 21:11:20.558924 napari_skimage-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.554924 napari_skimage-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/Docs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   156351 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/binary_morphology.png
--rw-r--r--   0 runner    (1001) docker     (127)   325762 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/denoise_nl.png
--rw-r--r--   0 runner    (1001) docker     (127)   293208 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/gaussian.png
--rw-r--r--   0 runner    (1001) docker     (127)   298737 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/morphology.png
--rw-r--r--   0 runner    (1001) docker     (127)   357944 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/simple_maths.png
--rw-r--r--   0 runner    (1001) docker     (127)   254360 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/docs/thresholding.png
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:11:20.558924 napari_skimage-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.546923 napari_skimage-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.554924 napari_skimage-0.1.0/src/napari_skimage/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.554924 napari_skimage-0.1.0/src/napari_skimage/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/_tests/test_basic_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/mathsops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/skimage_filter_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/skimage_morphology_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/skimage_restoration_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/src/napari_skimage/skimage_threshold_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:11:20.554924 napari_skimage-0.1.0/src/napari_skimage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 21:11:20.000000 napari_skimage-0.1.0/src/napari_skimage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 21:11:08.000000 napari_skimage-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.975954 napari_skimage-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.967954 napari_skimage-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.967954 napari_skimage-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.967954 napari_skimage-0.1.1/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-29 21:24:09.975954 napari_skimage-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.971954 napari_skimage-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/Docs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   156351 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/binary_morphology.png
+-rw-r--r--   0 runner    (1001) docker     (127)   325762 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/denoise_nl.png
+-rw-r--r--   0 runner    (1001) docker     (127)   293208 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/gaussian.png
+-rw-r--r--   0 runner    (1001) docker     (127)   298737 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/morphology.png
+-rw-r--r--   0 runner    (1001) docker     (127)   357944 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/simple_maths.png
+-rw-r--r--   0 runner    (1001) docker     (127)   254360 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/docs/thresholding.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:24:09.975954 napari_skimage-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.967954 napari_skimage-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.975954 napari_skimage-0.1.1/src/napari_skimage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.975954 napari_skimage-0.1.1/src/napari_skimage/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/_tests/test_basic_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/mathsops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/skimage_filter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/skimage_morphology_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/skimage_restoration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/src/napari_skimage/skimage_threshold_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:24:09.975954 napari_skimage-0.1.1/src/napari_skimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 21:24:09.000000 napari_skimage-0.1.1/src/napari_skimage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 21:23:59.000000 napari_skimage-0.1.1/tox.ini
```

### Comparing `napari_skimage-0.1.0/.github/workflows/test_and_deploy.yml` & `napari_skimage-0.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/.gitignore` & `napari_skimage-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/.pre-commit-config.yaml` & `napari_skimage-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/LICENSE` & `napari_skimage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/PKG-INFO` & `napari_skimage-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-skimage
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin to apply scikit-image operations
 Author: Guillaume Witz
 Author-email: guillaume.witz@unibe.ch
 License: 
         Copyright (c) 2024, Guillaume Witz, Data Science Lab, University of Bern
         All rights reserved.
```

### Comparing `napari_skimage-0.1.0/README.md` & `napari_skimage-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/Docs.ipynb` & `napari_skimage-0.1.1/docs/Docs.ipynb`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/binary_morphology.png` & `napari_skimage-0.1.1/docs/binary_morphology.png`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/denoise_nl.png` & `napari_skimage-0.1.1/docs/denoise_nl.png`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/gaussian.png` & `napari_skimage-0.1.1/docs/gaussian.png`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/morphology.png` & `napari_skimage-0.1.1/docs/morphology.png`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/simple_maths.png` & `napari_skimage-0.1.1/docs/simple_maths.png`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/docs/thresholding.png` & `napari_skimage-0.1.1/docs/thresholding.png`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/pyproject.toml` & `napari_skimage-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/__init__.py` & `napari_skimage-0.1.1/src/napari_skimage/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/_tests/test_basic_widgets.py` & `napari_skimage-0.1.1/src/napari_skimage/_tests/test_basic_widgets.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/mathsops.py` & `napari_skimage-0.1.1/src/napari_skimage/mathsops.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/napari.yaml` & `napari_skimage-0.1.1/src/napari_skimage/napari.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,22 @@
       title: Make Butterworth filter widget
     - id: napari-skimage.make_threshold_widget
       python_name: napari_skimage.skimage_threshold_widget:threshold_widget
       title: Make threshold widget
     - id: napari-skimage.make_binary_morphology_widget
       python_name: napari_skimage.skimage_morphology_widget:binary_morphology_widget
       title: Make binary morphology widget
-    - id: napari-skimage.make__morphology_widget
+    - id: napari-skimage.make_morphology_widget
       python_name: napari_skimage.skimage_morphology_widget:morphology_widget
       title: Make morphology widget
     - id: napari-skimage.make_connected_components_widget
       python_name: napari_skimage.skimage_morphology_widget:connected_components_widget
       title: Make connected components widget
     - id: napari-skimage.make_maths_image_pairs_widget
-      python_name: napari_skimage.mathsops:maths_image_pairs
+      python_name: napari_skimage.mathsops:maths_image_pairs_widget
       title: Make image pairs maths widget
     - id: napari-skimage.make_simple_maths_widget
       python_name: napari_skimage.mathsops:simple_maths_widget
       title: Make simple maths widget
     - id: napari-skimage.make_conversion_widget
       python_name: napari_skimage.mathsops:conversion_widget
       title: Make conversion widget
```

### Comparing `napari_skimage-0.1.0/src/napari_skimage/skimage_filter_widget.py` & `napari_skimage-0.1.1/src/napari_skimage/skimage_filter_widget.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/skimage_morphology_widget.py` & `napari_skimage-0.1.1/src/napari_skimage/skimage_morphology_widget.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/skimage_restoration_widget.py` & `napari_skimage-0.1.1/src/napari_skimage/skimage_restoration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage/skimage_threshold_widget.py` & `napari_skimage-0.1.1/src/napari_skimage/skimage_threshold_widget.py`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/src/napari_skimage.egg-info/PKG-INFO` & `napari_skimage-0.1.1/src/napari_skimage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-skimage
-Version: 0.1.0
+Version: 0.1.1
 Summary: A plugin to apply scikit-image operations
 Author: Guillaume Witz
 Author-email: guillaume.witz@unibe.ch
 License: 
         Copyright (c) 2024, Guillaume Witz, Data Science Lab, University of Bern
         All rights reserved.
```

### Comparing `napari_skimage-0.1.0/src/napari_skimage.egg-info/SOURCES.txt` & `napari_skimage-0.1.1/src/napari_skimage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_skimage-0.1.0/tox.ini` & `napari_skimage-0.1.1/tox.ini`

 * *Files identical despite different names*

