# Comparing `tmp/multi_med_image_ml-0.0.5.tar.gz` & `tmp/multi_med_image_ml-0.0.6.tar.gz`

## Comparing `multi_med_image_ml-0.0.5.tar` & `multi_med_image_ml-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/.images/logo.png
--rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/.images/model_diagram.png
--rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/.images/regress_figure.png
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/example/example_train.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/example/options/base_options.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/example/options/test_options.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/example/options/train_options.py
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10799 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/MultiInputTester.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    17623 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/tests/unit_tests.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/tests/weights.json
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/README.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.images/logo.png
+-rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.images/model_diagram.png
+-rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.images/regress_figure.png
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/example_train.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/options/base_options.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/options/test_options.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/options/train_options.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10801 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/tests/weights.json
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.5/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/.images/logo.png` & `multi_med_image_ml-0.0.6/.images/logo.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/.images/model_diagram.png` & `multi_med_image_ml-0.0.6/.images/model_diagram.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/.images/regress_figure.png` & `multi_med_image_ml-0.0.6/.images/regress_figure.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/example/example_train.py` & `multi_med_image_ml-0.0.6/example/example_train.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/example/options/base_options.py` & `multi_med_image_ml-0.0.6/example/options/base_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/example/options/test_options.py` & `multi_med_image_ml-0.0.6/example/options/test_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/example/options/train_options.py` & `multi_med_image_ml-0.0.6/example/options/train_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import os
 import numpy as np
-from utils import *
+from .utils import *
 import dateutil
 
 class DataBaseWrapper():
 	"""
 	Wrapper for Pandas table to cache some common and repeated functions
 	"""
 	def __init__(self,
```

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/MedImageLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import torch.multiprocessing
 from utils import *
 torch.multiprocessing.set_sharing_strategy('file_system')
 import shutil
 import nibabel as nb
 from nibabel.filebasedimages import *
 
-from Records import BatchRecord,ImageRecord
-from DataBaseWrapper import DataBaseWrapper
+from .Records import BatchRecord,ImageRecord
+from .DataBaseWrapper import DataBaseWrapper
 
 # Translates a filename to a key and back, for storing files as keys in the
 # pandas dataframe. By default, the keys are the full filepaths. This function
 # may need to be changed when switching to different systems
 def path_func_default(fkey,reverse=False):
 	return fkey
```

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/MultiInputTester.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTester.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch,os
 from torch import nn
 import numpy as np
-from Records import BatchRecord
+from .Records import BatchRecord
 import matplotlib.pyplot as plt
 import matplotlib
 matplotlib.use('Agg')
 from pytorch_grad_cam import GradCAMPlusPlus,GradCAM 
 
 # Tests either the model directly or the output files
 class MultiInputTester():
```

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/MultiInputTrainer.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTrainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch,os
 from torch import nn
 import numpy as np
-from Records import BatchRecord
+from .Records import BatchRecord
 import matplotlib.pyplot as plt
 import matplotlib
 matplotlib.use('Agg')
 
 """
 Used to apply training updates to the Multi Input Model. May also output graphs
 of the training loss
```

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/Records.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools,os
 import numpy as np
 from monai.transforms import *
-from utils import *
+from .utils import *
 
 generate_transforms = Compose([
 		RandAffine(prob=0.5, translate_range=10), 
 		RandRotate(prob=0.5, range_x=10.0),
 		RandGaussianNoise(prob=0.5),
 		RandBiasField(prob=0.5)])
 #,
```

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import random
 import itertools
 import numpy as np
 from datetime import datetime
 import hashlib
 import os,sys
 from copy import deepcopy as copy
-from Records import ImageRecord,BatchRecord
-from utils import download_weights
+from .Records import ImageRecord,BatchRecord
+from .utils import download_weights
 
 # Three functions that are used to get the age encoding functions
 def time_index(i,pos,d=512,c=10000):
 	if i % 2 == 0:
 		v = math.sin(pos/(c**(2*i/d)))
 	else:
 		v = math.cos(pos/(c**(2*i/d)))
```

### Comparing `multi_med_image_ml-0.0.5/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.6/src/multi_med_image_ml/utils.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/tests/unit_tests.py` & `multi_med_image_ml-0.0.6/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/README.md` & `multi_med_image_ml-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.5/pyproject.toml` & `multi_med_image_ml-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.5"
+version = "0.0.6"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `multi_med_image_ml-0.0.5/PKG-INFO` & `multi_med_image_ml-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multi_med_image_ml
-Version: 0.0.5
+Version: 0.0.6
 Summary: Deep learning library to encode multiple brain images and other electronic health record data in disease detection.
 Project-URL: Homepage, https://github.com/mleming/MultiMedImageML
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,deep learning,ehr,machine learning,mri,pytorch
 Requires-Python: >=3.8
```

