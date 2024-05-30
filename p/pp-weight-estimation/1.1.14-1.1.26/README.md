# Comparing `tmp/pp_weight_estimation-1.1.14.tar.gz` & `tmp/pp_weight_estimation-1.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.14.tar", last modified: Tue May 28 14:06:03 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.26.tar", last modified: Wed May 29 19:51:12 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.14.tar` & `pp_weight_estimation-1.1.26.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.14/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7871 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6680 2024-05-26 03:01:35.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-28 14:05:49.000000 pp_weight_estimation-1.1.14/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-28 14:06:03.000000 pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.14/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.094194 pp_weight_estimation-1.1.14/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.14/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.14/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 14:06:03.098194 pp_weight_estimation-1.1.14/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.14/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.26/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.287520 pp_weight_estimation-1.1.26/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     9537 2024-05-29 19:11:15.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6712 2024-05-29 12:30:55.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-29 19:51:00.000000 pp_weight_estimation-1.1.26/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-29 19:51:12.000000 pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.26/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.287520 pp_weight_estimation-1.1.26/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.26/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.26/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-29 19:51:12.291520 pp_weight_estimation-1.1.26/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.26/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.14/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.26/pp_weight_estimation/core/function_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 import transformers as t
 from PIL import Image
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from mb_utils.src import logging
-from .get_weight import get_seg, get_final_mask, get_final_img, get_histogram, get_val
+from pp_weight_estimation.core.get_weight import get_seg, get_final_mask, get_final_img, get_histogram, get_val
+from pp_weight_estimation.core.s3_io import get_client, download_image
 from urllib.parse import urlparse
 from typing import List,Dict,Union
+import cv2
+import yaml
+import boto3
 
 logger = logging.logger 
 model_checkpoint = '/Users/test/test1/mit-segformer-s' 
 model = t.TFSegformerForSemanticSegmentation.from_pretrained(model_checkpoint)
 
 __all__ = ["load_color_values", "process_pipeline"]
 
+def load_config(yaml_path: str) -> dict:
+    """
+    Function to load configurations from a YAML file
+    Args:
+        yaml_path (str): Path to the YAML file
+    Returns:
+        dict: Dictionary containing configurations
+    """
+    with open(yaml_path, 'r') as file:
+        config = yaml.safe_load(file)
+    return config
+
 def load_color_values(csv_path : str, logger: logging.Logger = None) -> Dict:
     """
     Function to load color values from a CSV file
     Args:
         csv_path (str): Path to the CSV file
         logger (Logger): Logger object
     Returns:
@@ -34,114 +50,142 @@
         color = row['colors']
         if taxcode and site and color:
             composed_key = f"{site}_{taxcode}"
             color_list = eval(color)
             color_dict[composed_key] = color_list
     return color_dict
 
-def process_pipeline(input_csv_path : str,gt_csv_path: str  ,val_color_csv_path : str,logger: logging.logger = None, **kwargs) -> Union[pd.DataFrame,List]:
+def process_pipeline(config_path: str, logger: logging.Logger = None, **kwargs) -> Union[pd.DataFrame, List]:
     """
-    Function to process the pipeline of Production Planning
+    Function to process the pipeline of Production Planning.
+    
+    This function automates the process of downloading images from an S3 bucket, applying segmentation and masking,
+    calculating histograms, and saving the results to an output CSV file. The function uses configurations provided
+    in a YAML file for flexibility.
+
     Args:
-        input_csv_path (str): Path to the input CSV file
-        gt_csv_path (str): Path to the groundtruth CSV file
-        val_color_csv_path (str): Path to the color values CSV file
-        logger (Logger): Logger object
+        config_path (str): Path to the YAML configuration file.
+        logger (logging.Logger): Logger object for logging messages (optional).
+        **kwargs: Additional keyword arguments (optional).
+        
     Returns:
-        pd.DataFrame: Output dataframe
-        List: List of results
+        tuple: A tuple containing:
+            - str: The path to the output CSV file.
+            - list: A list of results for each processed image.
     """
+    config = load_config(config_path)
+
+    input_csv_path = config['input_csv_path']
+    gt_csv_path = config['gt_csv_path']
+    val_color_csv_path = config['val_color_csv_path']
+    save_plots = config.get('save_plots', False)
+    final_mask_vals = config.get('final_mask_vals', 50)
+    #dummy bucket, needs to be changed
+    s3_bucket = 'pp-image-capture-processed-useast1-prod'
+
+    #might have to be change this
+    session = boto3.Session(profile_name='winnow')
+    client = session.client('s3')
 
     color_dict = load_color_values(val_color_csv_path)
     groundtruth_df = pd.read_csv(gt_csv_path)
-    
     input_df = pd.read_csv(input_csv_path)
     input_df['mask'] = ''
     input_df['final_image'] = ''
     input_df['pixel_count'] = 0
     input_df['histogram'] = ''
     input_df['pred_w2'] = 0.0
     input_df['error'] = 0.0
     input_df['success'] = False
 
     use_input_groundtruth = 'input_groundtruth' in input_df.columns
 
     entries = []
     for _, row in input_df.iterrows():
-        s3_image_path = row['s3_image_path']
+        local_image_path = row['s3_image_path']
         site_id = row['site_id']
         taxonomy_code = row['taxonomy_code']
         input_groundtruth = row['input_groundtruth'] if use_input_groundtruth else 0
-        if s3_image_path and site_id and taxonomy_code:
+        if local_image_path and site_id and taxonomy_code:
             composed_key = f"{site_id}_{taxonomy_code}"
-            entries.append((site_id, s3_image_path, composed_key, taxonomy_code))
+            entries.append((site_id, local_image_path, composed_key, taxonomy_code))
     
     if not entries:
         if logger:
             logger.error("No valid entries found in the CSV file")
         raise ValueError("No valid entries found in the CSV file")
     
     results = []
-    for index, (site_id, s3_image_path, composed_key, taxonomy_code) in enumerate(entries):
+    for index, (site_id, local_image_path, composed_key, taxonomy_code) in enumerate(entries):
         try:
             if composed_key not in color_dict:
                 if logger:
-                    logger.error(f"No color found for key {composed_key}. Skipping image {s3_image_path}.")
+                    logger.error(f"No color found for key {composed_key}. Skipping image {local_image_path}.")
                 input_df.at[index, 'success'] = False
                 continue
-            color = color_dict[composed_key]
+            colors = color_dict[composed_key]
         
-            site_dir = os.path.join('/pp_images/images', site_id)
+            site_dir = os.path.join('data/pp_images/images', site_id)
             os.makedirs(site_dir, exist_ok=True)
         
-            parsed_url = urlparse(s3_image_path)
-            original_filename = os.path.basename(parsed_url.path)
+            original_filename = os.path.basename(local_image_path)
+            save_filename, _ = os.path.splitext(os.path.basename(local_image_path))
             download_path = os.path.join(site_dir, original_filename)
         
             if logger:
                 logger.info(f"Processing image: {local_image_path}")
-            local_image_path = download_image_from_s3(s3_image_path, download_path)
-        
-            a, b, c, d, e = get_seg(local_image_path, mask_val=0.08, resize=True, new_bg_removal=True, equalize=True)
-        
-            mask_vals = 50
-            new_mask = get_final_mask(a, d, color=color, val=mask_vals)
+
+            image = download_image(s3_bucket, local_image_path, client)
+            image.save(download_path)
+            ori_img = cv2.imread(download_path)
+
+            masked_img = get_seg(local_image_path, model, mask_val=0.08, resize=True, new_bg_removal=True, equalize=True)
+
+            final_mask = None
+            for color in colors:
+                mask = get_final_mask(ori_img, masked_img, color=color, val=final_mask_vals, logger=logger)
+                if final_mask is None:
+                    final_mask = mask
+                else:
+                    final_mask = cv2.bitwise_or(final_mask, mask)
 
             masks_dir = os.path.join('data/pp_images/masks')
             os.makedirs(masks_dir, exist_ok=True)
-            mask_save_path = os.path.join(masks_dir, f"{original_filename}_mask_{mask_vals}.png")
-            mask_image = Image.fromarray(new_mask.astype(np.uint8))
+            mask_save_path = os.path.join(masks_dir, f"{original_filename}_mask_{final_mask_vals}.png")
+            mask_image = Image.fromarray(final_mask.astype(np.uint8))
             mask_image.save(mask_save_path)
             input_df.at[index, 'mask'] = mask_save_path
 
-            new_final_img = get_final_img(a, new_mask, mask_val=0.2)
+            new_final_img = get_final_img(masked_img, final_mask, mask_val=0.2)
 
             final_images_dir = os.path.join('data/pp_images/final_image')
             os.makedirs(final_images_dir, exist_ok=True)
-            final_img_save_path = os.path.join(final_images_dir, f"{os.path.basename(local_image_path)}_final.png")
+            final_img_save_path = os.path.join(final_images_dir, f"{original_filename}_final.png")
             final_image = Image.fromarray(new_final_img.astype(np.uint8))
             final_image.save(final_img_save_path)
             input_df.at[index, 'final_image'] = final_img_save_path
-        
-            new_histogram, bin_edges = get_histogram(new_final_img)
+
+            final_image_np = np.array(final_image)
+
+            new_histogram, bin_edges = get_histogram(final_image_np)
 
             pixel_count = new_histogram[-1]
-            histograms_dir = os.path.join('data/pp_images/histograms')
-            os.makedirs(histograms_dir, exist_ok=True)
-            histogram_save_path = os.path.join(histograms_dir, f"{os.path.basename(local_image_path)}_{pixel_count}_hist.png")
             input_df.at[index, 'pixel_count'] = pixel_count
             input_df.at[index, 'histogram'] = histogram_save_path
-        
-            plt.figure()
-            plt.hist(new_final_img.ravel(), bins=bin_edges)
-            plt.title('Histogram')
-            plt.xlabel('Pixel Value')
-            plt.ylabel('Frequency')
-            plt.savefig(histogram_save_path)
-            plt.close()       
+
+            if save_plots:
+                plots_dir = os.path.join('data/pp_images/image_plots')
+                os.makedirs(plots_dir, exist_ok=True)
+                
+                hist_plot_path = os.path.join(plots_dir, f"{original_filename}_hist_plot.png")
+                
+                plt.savefig(hist_plot_path)
+                plt.close()
+            else:
+                plt.close()
 
             reference_row = groundtruth_df[groundtruth_df['taxonomy_code'] == taxonomy_code]
             if not reference_row.empty:
                 reference_pixel_count = reference_row.iloc[0]['reference_pixel_count']
                 groundtruth_weight = reference_row.iloc[0]['groundtruth']
 
                 weight2 = input_groundtruth if input_groundtruth else 0
@@ -150,37 +194,38 @@
                 if logger:
                     logger.error(f"No groundtruth data found for taxonomy_code {taxonomy_code}.")
 
             input_df.at[index, 'pred_w2'] = pred_w2
             input_df.at[index, 'error'] = error
             input_df.at[index, 'success'] = True if pred_w2 is not None else False
 
-            results.append((a, b, c, d, e, new_mask, new_final_img, new_histogram, pred_w2, error))
+            results.append((masked_img, final_mask, new_final_img, new_histogram, pred_w2, error))
         except Exception as e:
             if logger:
-                logger.error(f"Error processing image {s3_image_path}: {e}")
+                logger.error(f"Error processing image {local_image_path}: {e}")
             input_df.at[index, 'success'] = False
             continue
     
-    output_csv_path = "data/pp_images/csv/output_csv/output.csv"
+    output_csv_dir = os.path.join('data/pp_images/csv/output_csv')
+    os.makedirs(output_csv_dir, exist_ok=True)
+    output_csv_path = os.path.join(output_csv_dir, "output.csv")
     input_df.to_csv(output_csv_path, index=False)
 
     if logger:
         logger.info(f"Processing complete. Output saved to {output_csv_path}")
         
     return output_csv_path, results
 
 
-
-# add logger
+# add logger - done
 # error if there is not taxcode and skip that image - done
 # column to output with failure or success -done
 # new csv with refrence image and groundtruth, and histogram pixel inside segmentation, model-checkpoint - done
 # download to GH2  particular location - done
 # save everything mask(save the 50 val in the name of file as _50) histogram and final image - done 
 # save everything locally - done
-# save the plots locally only when input is given add plot boolean input to process_pipeline at images_plot folder 
-# yaml file for inputs
-# write the _mask after the name
+# save the plots locally only when input is given add plot boolean input to process_pipeline at images_plot folder - done
+# yaml file for inputs -done
+# write the _mask after the name - done
 # s3cmd ls s3://pp-image-capture-processed-useast1-prod/siteId=33263/mealService=b514a5da-2bcf-4330-8a3c-f17e7f85a922/
 # get-repsonse -> get-image -> download image -> 
 # aslo csv files
```

### Comparing `pp_weight_estimation-1.1.14/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.26/pp_weight_estimation/core/get_weight.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
     if logger:
         logger.info('histogram :  {}'.format(histogram))
         logger.info('bin edges : {}'.format(bin_edges))
     if show:
         plt.figure()
         plt.plot(bin_edges[:-1], histogram)
         plt.show()
+    return histogram, bin_edges
 
 def get_weight(img,model,**kwargs):
     """
     Function to get the weight of the object in the image
     """
     mask = get_seg(img,model,**kwargs)
     get_histogram(mask,)
```

### Comparing `pp_weight_estimation-1.1.14/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.26/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.14/pp_weight_estimation/core/s3_io.py` & `pp_weight_estimation-1.1.26/pp_weight_estimation/core/s3_io.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.14/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.26/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.14/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.26/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.14/setup.py` & `pp_weight_estimation-1.1.26/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.14/tests/test_function_test.py` & `pp_weight_estimation-1.1.26/tests/test_function_test.py`

 * *Files identical despite different names*

