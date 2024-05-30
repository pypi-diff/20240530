# Comparing `tmp/onediffx-1.1.0.dev202405280128.tar.gz` & `tmp/onediffx-1.1.0.dev202405290129.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-1.1.0.dev202405280128.tar", last modified: Tue May 28 01:28:45 2024, max compression
+gzip compressed data, was "onediffx-1.1.0.dev202405290129.tar", last modified: Wed May 29 01:30:13 2024, max compression
```

## Comparing `onediffx-1.1.0.dev202405280128.tar` & `onediffx-1.1.0.dev202405290129.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/
--rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21267 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.673739 onediffx-1.1.0.dev202405280128/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.677739 onediffx-1.1.0.dev202405280128/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.677739 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.677739 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-05-28 01:28:45.000000 onediffx-1.1.0.dev202405280128/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-28 01:28:45.000000 onediffx-1.1.0.dev202405280128/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:28:45.000000 onediffx-1.1.0.dev202405280128/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 01:28:45.000000 onediffx-1.1.0.dev202405280128/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 01:28:45.000000 onediffx-1.1.0.dev202405280128/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:28:45.681739 onediffx-1.1.0.dev202405280128/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-28 01:28:21.000000 onediffx-1.1.0.dev202405280128/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/
+-rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21267 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.144261 onediffx-1.1.0.dev202405290129/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.144261 onediffx-1.1.0.dev202405290129/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.144261 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.144261 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22324 2024-05-29 01:30:13.000000 onediffx-1.1.0.dev202405290129/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 01:30:13.000000 onediffx-1.1.0.dev202405290129/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:30:13.000000 onediffx-1.1.0.dev202405290129/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 01:30:13.000000 onediffx-1.1.0.dev202405290129/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 01:30:13.000000 onediffx-1.1.0.dev202405290129/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:30:13.148261 onediffx-1.1.0.dev202405290129/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-29 01:29:48.000000 onediffx-1.1.0.dev202405290129/tests/test_lora.py
```

### Comparing `onediffx-1.1.0.dev202405280128/PKG-INFO` & `onediffx-1.1.0.dev202405290129/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.1.0.dev202405280128
+Version: 1.1.0.dev202405290129
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-1.1.0.dev202405280128/README.md` & `onediffx-1.1.0.dev202405290129/README.md`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-1.1.0.dev202405290129/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/__init__.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-1.1.0.dev202405290129/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/lora/lora.py` & `onediffx-1.1.0.dev202405290129/onediffx/lora/lora.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/lora/state_dict_utils.py` & `onediffx-1.1.0.dev202405290129/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/lora/text_encoder.py` & `onediffx-1.1.0.dev202405290129/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/lora/unet.py` & `onediffx-1.1.0.dev202405290129/onediffx/lora/unet.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/lora/utils.py` & `onediffx-1.1.0.dev202405290129/onediffx/lora/utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx/utils/patch_image_processor.py` & `onediffx-1.1.0.dev202405290129/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/onediffx.egg-info/PKG-INFO` & `onediffx-1.1.0.dev202405290129/onediffx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.1.0.dev202405280128
+Version: 1.1.0.dev202405290129
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `onediffx-1.1.0.dev202405280128/onediffx.egg-info/SOURCES.txt` & `onediffx-1.1.0.dev202405290129/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/setup.py` & `onediffx-1.1.0.dev202405290129/setup.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.1.0.dev202405280128/tests/test_lora.py` & `onediffx-1.1.0.dev202405290129/tests/test_lora.py`

 * *Files identical despite different names*

