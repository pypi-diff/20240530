# Comparing `tmp/pp_weight_estimation-1.1.27.tar.gz` & `tmp/pp_weight_estimation-1.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.27.tar", last modified: Thu May 30 01:40:58 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.39.tar", last modified: Thu May 30 11:54:49 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.27.tar` & `pp_weight_estimation-1.1.39.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.324910 pp_weight_estimation-1.1.27/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.27/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     9537 2024-05-30 01:40:37.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6712 2024-05-29 12:30:55.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-30 01:40:49.000000 pp_weight_estimation-1.1.27/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-30 01:40:58.000000 pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.27/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.27/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-30 01:40:58.324910 pp_weight_estimation-1.1.27/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.27/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 01:40:58.320910 pp_weight_estimation-1.1.27/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.27/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.39/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    11113 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6734 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-30 11:54:37.000000 pp_weight_estimation-1.1.39/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 11:54:49.000000 pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-30 11:54:49.000000 pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-30 11:54:49.000000 pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-30 11:54:49.000000 pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-30 11:54:49.000000 pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.39/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.39/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.39/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 11:54:49.555596 pp_weight_estimation-1.1.39/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.39/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.27/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.39/pp_weight_estimation/core/function_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from mb_utils.src import logging
 from pp_weight_estimation.core.get_weight import get_seg, get_final_mask, get_final_img, get_histogram, get_val
 from pp_weight_estimation.core.s3_io import get_client, download_image
+from pp_weight_estimation.core.gpt_support import get_count
 from urllib.parse import urlparse
 from typing import List,Dict,Union
 import cv2
 import yaml
 import boto3
 
 logger = logging.logger 
-model_checkpoint = '/Users/test/test1/mit-segformer-s' 
-model = t.TFSegformerForSemanticSegmentation.from_pretrained(model_checkpoint)
+#model_checkpoint = '/Users/test/test1/mit-segformer-s' 
+#model = t.TFSegformerForSemanticSegmentation.from_pretrained(model_checkpoint)
 
 __all__ = ["load_color_values", "process_pipeline"]
 
 def load_config(yaml_path: str) -> dict:
     """
     Function to load configurations from a YAML file
     Args:
@@ -70,24 +71,43 @@
     Returns:
         tuple: A tuple containing:
             - str: The path to the output CSV file.
             - list: A list of results for each processed image.
     """
     config = load_config(config_path)
 
-    input_csv_path = config['input_csv_path']
-    gt_csv_path = config['gt_csv_path']
-    val_color_csv_path = config['val_color_csv_path']
-    save_plots = config.get('save_plots', False)
-    final_mask_vals = config.get('final_mask_vals', 50)
-    #dummy bucket, needs to be changed
-    s3_bucket = 'pp-image-capture-processed-useast1-prod'
+    input_csv_path = config['data']['input_csv_path']
+    gt_csv_path = config['data']['gt_csv_path']
+    val_color_csv_path = config['data']['val_color_csv_path']
+    path_to_save_images = config['data']['path_to_save_images']
+    
+    save_plots = config['results'].get('save_plots', False)
+    final_mask_vals = config['results'].get('final_mask_vals', 50)
+    mask_val = config['results'].get('model_val', 0.08)
+    new_bg_removal = config['results'].get('background_removal', True)
+    equalizer_items = config['results'].get('equalizer_items')
+
+    model_path = config['model']['model_path']
+    model_name = config['model']['model_name']
+    model_version = config['model']['model_version']
+
+    bucket = config['aws_data']['bucket_name']
+    profile = config['aws_data']['profile']
+
+    gpt_response = config['gpt_res'].get('gpt_response', False)
+    gpt_token = config['gpt_res'].get('gpt_token', None)
+    gpt_model = config['gpt_res'].get('gpt_model', None)
+    gpt_prompt = config['gpt_res'].get('gpt_prompt', None)
+    gpt_file_path = config['gpt_res'].get('gpt_file_path', None)
+    gpt_api_key = config['gpt_res']['gpt_api_key']
+
+    model = t.TFSegformerForSemanticSegmentation.from_pretrained(model_path)  
 
     #might have to be change this
-    session = boto3.Session(profile_name='winnow')
+    session = boto3.Session(profile_name=profile)
     client = session.client('s3')
 
     color_dict = load_color_values(val_color_csv_path)
     groundtruth_df = pd.read_csv(gt_csv_path)
     input_df = pd.read_csv(input_csv_path)
     input_df['mask'] = ''
     input_df['final_image'] = ''
@@ -100,14 +120,15 @@
     use_input_groundtruth = 'input_groundtruth' in input_df.columns
 
     entries = []
     for _, row in input_df.iterrows():
         local_image_path = row['s3_image_path']
         site_id = row['site_id']
         taxonomy_code = row['taxonomy_code']
+        food_item = row['food_item']
         input_groundtruth = row['input_groundtruth'] if use_input_groundtruth else 0
         if local_image_path and site_id and taxonomy_code:
             composed_key = f"{site_id}_{taxonomy_code}"
             entries.append((site_id, local_image_path, composed_key, taxonomy_code))
     
     if not entries:
         if logger:
@@ -120,68 +141,68 @@
             if composed_key not in color_dict:
                 if logger:
                     logger.error(f"No color found for key {composed_key}. Skipping image {local_image_path}.")
                 input_df.at[index, 'success'] = False
                 continue
             colors = color_dict[composed_key]
         
-            site_dir = os.path.join('data/pp_images/images', site_id)
+            site_dir = os.path.join(path_to_save_images, 'images' , site_id)
             os.makedirs(site_dir, exist_ok=True)
         
             original_filename = os.path.basename(local_image_path)
             save_filename, _ = os.path.splitext(os.path.basename(local_image_path))
             download_path = os.path.join(site_dir, original_filename)
         
             if logger:
                 logger.info(f"Processing image: {local_image_path}")
 
-            image = download_image(s3_bucket, local_image_path, client)
+            image = download_image(bucket, local_image_path, client)
             image.save(download_path)
             ori_img = cv2.imread(download_path)
 
-            masked_img = get_seg(local_image_path, model, mask_val=0.08, resize=True, new_bg_removal=True, equalize=True)
+            masked_img = get_seg(local_image_path, model, mask_val=mask_val, resize=True, new_bg_removal=new_bg_removal, equalize=True)
 
             final_mask = None
             for color in colors:
                 mask = get_final_mask(ori_img, masked_img, color=color, val=final_mask_vals, logger=logger)
                 if final_mask is None:
                     final_mask = mask
                 else:
                     final_mask = cv2.bitwise_or(final_mask, mask)
 
-            masks_dir = os.path.join('data/pp_images/masks')
+            masks_dir = os.path.join(path_to_save_images, 'masks')
             os.makedirs(masks_dir, exist_ok=True)
-            mask_save_path = os.path.join(masks_dir, f"{original_filename}_mask_{final_mask_vals}.png")
+            mask_save_path = os.path.join(masks_dir, f"{save_filename}_mask_{final_mask_vals}.png")
             mask_image = Image.fromarray(final_mask.astype(np.uint8))
             mask_image.save(mask_save_path)
             input_df.at[index, 'mask'] = mask_save_path
 
-            new_final_img = get_final_img(masked_img, final_mask, mask_val=0.2)
+            new_final_img = get_final_img(masked_img, final_mask, mask_val=mask_val)
 
-            final_images_dir = os.path.join('data/pp_images/final_image')
+            final_images_dir = os.path.join(path_to_save_images, 'final_image')
             os.makedirs(final_images_dir, exist_ok=True)
-            final_img_save_path = os.path.join(final_images_dir, f"{original_filename}_final.png")
+            final_img_save_path = os.path.join(final_images_dir, f"{save_filename}_final.png")
             final_image = Image.fromarray(new_final_img.astype(np.uint8))
             final_image.save(final_img_save_path)
             input_df.at[index, 'final_image'] = final_img_save_path
 
             final_image_np = np.array(final_image)
 
             new_histogram, bin_edges = get_histogram(final_image_np)
 
             pixel_count = new_histogram[-1]
+            pixel_count = pixel_count.astype(int)
             input_df.at[index, 'pixel_count'] = pixel_count
-            input_df.at[index, 'histogram'] = histogram_save_path
 
             if save_plots:
-                plots_dir = os.path.join('data/pp_images/image_plots')
+                plots_dir = os.path.join(path_to_save_images, 'image_plots')
                 os.makedirs(plots_dir, exist_ok=True)
                 
-                hist_plot_path = os.path.join(plots_dir, f"{original_filename}_hist_plot.png")
-                
+                hist_plot_path = os.path.join(plots_dir, f"{save_filename}_hist_plot.png")
+                input_df.at[index, 'histogram'] = hist_plot_path             
                 plt.savefig(hist_plot_path)
                 plt.close()
             else:
                 plt.close()
 
             reference_row = groundtruth_df[groundtruth_df['taxonomy_code'] == taxonomy_code]
             if not reference_row.empty:
@@ -192,24 +213,32 @@
                 pred_w2, error = get_val(reference_pixel_count, pixel_count, groundtruth_weight, weight2)
             else:
                 if logger:
                     logger.error(f"No groundtruth data found for taxonomy_code {taxonomy_code}.")
 
             input_df.at[index, 'pred_w2'] = pred_w2
             input_df.at[index, 'error'] = error
-            input_df.at[index, 'success'] = True if pred_w2 is not None else False
 
-            results.append((masked_img, final_mask, new_final_img, new_histogram, pred_w2, error))
+            if gpt_response:
+                gpt_result = get_count(image_path = local_image_path, item = food_item, api_key = gpt_api_key, df_loc = gpt_file_path, prompt = gpt_prompt)
+                gpt_error = (weight2-gpt_result)/weight2
+                input_df.at[index, 'gpt_result'] = gpt_result
+                input_df.at[index, 'gpt_error'] = gpt_error
+                input_df.at[index, 'success'] = True if gpt_result is not None else False
+            else:    
+                input_df.at[index, 'success'] = True if pred_w2 is not None else False
+
+            results.append((masked_img, final_mask, new_final_img, new_histogram, pred_w2, error, gpt_result, gpt_error))
         except Exception as e:
             if logger:
                 logger.error(f"Error processing image {local_image_path}: {e}")
             input_df.at[index, 'success'] = False
             continue
     
-    output_csv_dir = os.path.join('data/pp_images/csv/output_csv')
+    output_csv_dir = os.path.join(path_to_save_images, 'csv', site_id, 'output_csv')
     os.makedirs(output_csv_dir, exist_ok=True)
     output_csv_path = os.path.join(output_csv_dir, "output.csv")
     input_df.to_csv(output_csv_path, index=False)
 
     if logger:
         logger.info(f"Processing complete. Output saved to {output_csv_path}")
```

### Comparing `pp_weight_estimation-1.1.27/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.39/pp_weight_estimation/core/get_weight.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     return np.sum(mask)
 
 def get_val(pix1,pix2,weight1,weight2,logger=None):
     """
     Function to get the histogram error
     """
     pred_w2 = weight1*(pix2/pix1)
-    error = (weight2-pred_w2)/weight2
+    error = (weight2-pred_w2)/weight2 if weight2 !=0 else 0
     if logger:
         logger.info(pred_w2)
         logger.info(error)
     return pred_w2,error
 
 def split_filename(file: str,logger=None) -> dict :
     """
```

### Comparing `pp_weight_estimation-1.1.27/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.39/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.27/pp_weight_estimation/core/s3_io.py` & `pp_weight_estimation-1.1.39/pp_weight_estimation/core/s3_io.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.27/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.39/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.27/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.39/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.27/setup.py` & `pp_weight_estimation-1.1.39/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.27/tests/test_function_test.py` & `pp_weight_estimation-1.1.39/tests/test_function_test.py`

 * *Files identical despite different names*

