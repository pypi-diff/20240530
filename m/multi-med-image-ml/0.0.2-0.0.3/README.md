# Comparing `tmp/multi_med_image_ml-0.0.2.tar.gz` & `tmp/multi_med_image_ml-0.0.3.tar.gz`

## Comparing `multi_med_image_ml-0.0.2.tar` & `multi_med_image_ml-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.images/logo.png
--rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.images/model_diagram.png
--rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/.images/regress_figure.png
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/example_train.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/options/base_options.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/options/test_options.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/example/options/train_options.py
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10799 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTester.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    17623 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/tests/unit_tests.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/tests/weights.json
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/README.md
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/.images/logo.png
+-rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/.images/model_diagram.png
+-rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/.images/regress_figure.png
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/example/example_train.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/example/options/base_options.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/example/options/test_options.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/example/options/train_options.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10799 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    17623 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/tests/weights.json
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/README.md
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.3/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.2/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/.images/logo.png` & `multi_med_image_ml-0.0.3/.images/logo.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/.images/model_diagram.png` & `multi_med_image_ml-0.0.3/.images/model_diagram.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/.images/regress_figure.png` & `multi_med_image_ml-0.0.3/.images/regress_figure.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/example/example_train.py` & `multi_med_image_ml-0.0.3/example/example_train.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/example/options/base_options.py` & `multi_med_image_ml-0.0.3/example/options/base_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/example/options/test_options.py` & `multi_med_image_ml-0.0.3/example/options/test_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/example/options/train_options.py` & `multi_med_image_ml-0.0.3/example/options/train_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/MedImageLoader.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTester.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/MultiInputTester.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/MultiInputTrainer.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/MultiInputTrainer.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/Records.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/models.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.3/src/multi_med_image_ml/utils.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/tests/unit_tests.py` & `multi_med_image_ml-0.0.3/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/README.md` & `multi_med_image_ml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.2/pyproject.toml` & `multi_med_image_ml-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.2"
+version = "0.0.3"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `multi_med_image_ml-0.0.2/PKG-INFO` & `multi_med_image_ml-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multi_med_image_ml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deep learning library to encode multiple brain images and other electronic health record data in disease detection.
 Project-URL: Homepage, https://github.com/mleming/MultiMedImageML
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,deep learning,ehr,machine learning,mri,pytorch
 Requires-Python: >=3.8
```

