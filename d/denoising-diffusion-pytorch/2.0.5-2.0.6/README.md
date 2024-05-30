# Comparing `tmp/denoising_diffusion_pytorch-2.0.5.tar.gz` & `tmp/denoising_diffusion_pytorch-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising_diffusion_pytorch-2.0.5.tar", last modified: Thu May 23 21:17:42 2024, max compression
+gzip compressed data, was "denoising_diffusion_pytorch-2.0.6.tar", last modified: Thu May 30 16:21:38 2024, max compression
```

## Comparing `denoising_diffusion_pytorch-2.0.5.tar` & `denoising_diffusion_pytorch-2.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:42.374117 denoising_diffusion_pytorch-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 21:17:42.370117 denoising_diffusion_pytorch-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:42.370117 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35670 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/karras_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/karras_unet_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/karras_unet_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    40507 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/repaint.py
--rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:42.370117 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 21:17:42.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 21:17:42.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:17:42.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 21:17:42.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 21:17:42.000000 denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:42.374117 denoising_diffusion_pytorch-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 21:17:38.000000 denoising_diffusion_pytorch-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:38.171583 denoising_diffusion_pytorch-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 16:21:38.171583 denoising_diffusion_pytorch-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:38.171583 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38426 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35670 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/karras_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/karras_unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23187 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/karras_unet_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/repaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21071 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:38.171583 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 16:21:38.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-30 16:21:38.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:21:38.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 16:21:38.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 16:21:38.000000 denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:21:38.171583 denoising_diffusion_pytorch-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 16:21:31.000000 denoising_diffusion_pytorch-2.0.6/setup.py
```

### Comparing `denoising_diffusion_pytorch-2.0.5/LICENSE` & `denoising_diffusion_pytorch-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/PKG-INFO` & `denoising_diffusion_pytorch-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.5
+Version: 2.0.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.5/README.md` & `denoising_diffusion_pytorch-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/__init__.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/attend.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/karras_unet.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/karras_unet.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/karras_unet_1d.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/karras_unet_1d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/karras_unet_3d.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/karras_unet_3d.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/repaint.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/repaint.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,15 +710,15 @@
 
         for t in tqdm(reversed(range(0, self.num_timesteps)), desc = 'sampling loop time step', total = self.num_timesteps):
             self_cond = x_start if self.self_condition else None
             img, x_start = self.p_sample(x=img, t=t, x_self_cond=self_cond, gt=gt, mask=mask)
             imgs.append(img)
 
             # Resampling loop: line 9 of Algorithm 1 in https://arxiv.org/pdf/2201.09865
-            if resample is True and (t > 0) and (t % resample_every == 0 or t == 1):
+            if resample is True and (t > 0) and (t % resample_every == 0 or t == 1) and mask is not None:
                 # Jump back for resample_jump timesteps and resample_iter times
                 for iter in tqdm(range(resample_iter), desc = 'resample loop', total = resample_iter):
                     t = resample_jump
                     beta = self.betas[t]
                     img = torch.sqrt(1 - beta) * img + torch.sqrt(beta) * torch.randn_like(img)
                     for j in reversed(range(0, resample_jump)):
                         img, x_start = self.p_sample(x=img, t=t, gt=gt, mask=mask)
```

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 2.0.5
+Version: 2.0.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising_diffusion_pytorch-2.0.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising_diffusion_pytorch-2.0.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising_diffusion_pytorch-2.0.5/setup.py` & `denoising_diffusion_pytorch-2.0.6/setup.py`

 * *Files identical despite different names*

