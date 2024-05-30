# Comparing `tmp/multi_med_image_ml-0.0.6.tar.gz` & `tmp/multi_med_image_ml-0.0.7.tar.gz`

## Comparing `multi_med_image_ml-0.0.6.tar` & `multi_med_image_ml-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/setup.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.images/logo.png
--rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.images/model_diagram.png
--rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/.images/regress_figure.png
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/example_train.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/options/base_options.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/options/test_options.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/example/options/train_options.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/DataBaseWrapper.py
--rwxr-xr-x   0        0        0    10801 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/MedImageLoader.py
--rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTester.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTrainer.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/Records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/__init__.py
--rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/models.py
--rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/src/multi_med_image_ml/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/tests/unit_tests.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/tests/weights.json
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/README.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/setup.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0   506885 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.images/logo.png
+-rw-r--r--   0        0        0  2674703 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.images/model_diagram.png
+-rw-r--r--   0        0        0   289892 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/.images/regress_figure.png
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/example_train.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/options/base_options.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/options/test_options.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/example/options/train_options.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/DataBaseWrapper.py
+-rwxr-xr-x   0        0        0    10802 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/MedImageLoader.py
+-rw-r--r--   0        0        0    19875 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTester.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTrainer.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/Records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/__init__.py
+-rw-r--r--   0        0        0    17625 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/models.py
+-rw-r--r--   0        0        0    46062 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/src/multi_med_image_ml/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/tests/unit_tests.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/tests/weights.json
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/README.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 multi_med_image_ml-0.0.7/PKG-INFO
```

### Comparing `multi_med_image_ml-0.0.6/.github/workflows/publish-to-pypi.yml` & `multi_med_image_ml-0.0.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/.images/logo.png` & `multi_med_image_ml-0.0.7/.images/logo.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/.images/model_diagram.png` & `multi_med_image_ml-0.0.7/.images/model_diagram.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/.images/regress_figure.png` & `multi_med_image_ml-0.0.7/.images/regress_figure.png`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/example/example_train.py` & `multi_med_image_ml-0.0.7/example/example_train.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/example/options/base_options.py` & `multi_med_image_ml-0.0.7/example/options/base_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/example/options/test_options.py` & `multi_med_image_ml-0.0.7/example/options/test_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/example/options/train_options.py` & `multi_med_image_ml-0.0.7/example/options/train_options.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/DataBaseWrapper.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/DataBaseWrapper.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/MedImageLoader.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/MedImageLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torchvision.transforms as transforms
 from pdb import set_trace as st
 import random
 import numpy as np
 import torch
 import pandas as pd
 import torch.multiprocessing
-from utils import *
+from .utils import *
 torch.multiprocessing.set_sharing_strategy('file_system')
 import shutil
 import nibabel as nb
 from nibabel.filebasedimages import *
 
 from .Records import BatchRecord,ImageRecord
 from .DataBaseWrapper import DataBaseWrapper
```

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTester.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTester.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/MultiInputTrainer.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/MultiInputTrainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 				self.optimizer.step()
 				self.optimizer.zero_grad()
 				self.model.classifier_freeze()
 				if dataloader is not None:
 					dataloader.switch_stack()
 			else:
 				self.optimizer_reg.step()
-				self.optimizer_reg.zero_step()
+				self.optimizer_reg.zero_grad()
 				self.model.regressor_freeze()
 				if dataloader is not None:
 					dataloader.switch_stack()
 			self.one_step = not self.one_step
 		if self.index % self.save_latest_freq == 0 and self.index != 0:
 			if self.checkpoint_dir is not None:
 				torch.save(
```

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/Records.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/Records.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/models.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/models.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/src/multi_med_image_ml/utils.py` & `multi_med_image_ml-0.0.7/src/multi_med_image_ml/utils.py`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/tests/unit_tests.py` & `multi_med_image_ml-0.0.7/tests/unit_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 					cache = True,
 					channels_first=False)
 		for image,label in medim_loader:
 			self.assertTrue(medim_loader.cache)
 			self.assertTrue(isinstance(image,np.ndarray))
 			self.assertTrue(isinstance(label,np.ndarray))
 			imsize = image.shape
-			self.assertEqual(imsize[0], 16)
+			self.assertEqual(imsize[0], 14)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 		pandas_file = medim_loader.all_vars_file
 		self.assertTrue(os.path.isfile(pandas_file))
 		df = pd.read_pickle(pandas_file)
 		self.assertTrue(len(df) > 10)
@@ -183,15 +183,15 @@
 		self.assertTrue(os.path.isfile(pandas_file))
 		medim_loader = MedImageLoader(pandas_file,
 			dim=(48,32,24),dtype="numpy",channels_first=False)
 		self.assertEqual(medim_loader.mode,"iterate")
 		for image in medim_loader:
 			imsize = image.shape
 			self.assertEqual(len(imsize),5)
-			self.assertEqual(imsize[0], 16)
+			self.assertEqual(imsize[0], 14)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 	
 	def test_match_label_confounds(self):
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			dim=(48,32,24),
@@ -206,15 +206,15 @@
 			label=["MRAcquisitionType"],
 			confounds=["PercentSampling"],
 			channels_first=False)
 		self.assertEqual(medim_loader.mode,"match")
 		for image,label in medim_loader:
 			imsize = image.shape
 			self.assertEqual(len(imsize),5)
-			self.assertEqual(imsize[0], 16)
+			self.assertEqual(imsize[0], 14)
 			self.assertEqual(imsize[1], 48)
 			self.assertEqual(imsize[2], 32)
 			self.assertEqual(imsize[3], 24)
 	def test_grouping(self):
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			dim=(48,32,24),
 			cache=True,
@@ -270,23 +270,23 @@
 			optimizer.zero_grad()
 			y_pred,y_reg = model(p)
 			loss = loss_function(p.get_Y(),y_pred)
 			loss.backward()
 			optimizer.step()
 			break
 	def test_trainer(self):
-		model = MultiInputModule(Y_dim = (17,2),C_dim=(13,11))
+		model = MultiInputModule(Y_dim = (17,4),C_dim=(13,11))
 		medim_loader = MedImageLoader(imfolder1,imfolder2,
 			cache=True,
 			label=["MRAcquisitionType",
 					"ImageOrientationPatientDICOM"],
 			confounds=["Slice Thickness","Repetition Time"],
 			return_obj = True,
 			dtype="torch",
-			batch_size=14,Y_dim=(17,2),C_dim=(13,11))
+			batch_size=14,Y_dim=(17,4),C_dim=(13,11))
 		trainer = MultiInputTrainer(model,batch_size=2)
 		for i in range(3):
 			#print(f"Epoch {i}")
 			for p in medim_loader:
 				trainer.loop(p,dataloader=medim_loader)
 		
 	def test_cache2(self):
```

### Comparing `multi_med_image_ml-0.0.6/README.md` & `multi_med_image_ml-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `multi_med_image_ml-0.0.6/pyproject.toml` & `multi_med_image_ml-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "multi_med_image_ml"
 
-version = "0.0.6"
+version = "0.0.7"
 
 dependencies = [
   "numpy",
   "scipy",
   "torch",
   "torchvision",
   "opencv-python>=4.5.4",
```

### Comparing `multi_med_image_ml-0.0.6/PKG-INFO` & `multi_med_image_ml-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multi_med_image_ml
-Version: 0.0.6
+Version: 0.0.7
 Summary: Deep learning library to encode multiple brain images and other electronic health record data in disease detection.
 Project-URL: Homepage, https://github.com/mleming/MultiMedImageML
 Author-email: Matt Leming <mleming@mgh.harvard.edu>
 Maintainer-email: Matt Leming <mleming@mgh.harvard.edu>
 License: MIT License
 Keywords: biomedical,deep learning,ehr,machine learning,mri,pytorch
 Requires-Python: >=3.8
```

