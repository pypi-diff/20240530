# Comparing `tmp/danila-lib-1.8.3.tar.gz` & `tmp/danila-lib-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.8.3.tar", last modified: Tue May 28 13:59:57 2024, max compression
+gzip compressed data, was "danila-lib-1.8.4.tar", last modified: Thu May 30 06:42:37 2024, max compression
```

## Comparing `danila-lib-1.8.3.tar` & `danila-lib-1.8.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:59:57.756676 danila-lib-1.8.3/
--rw-rw-rw-   0        0        0     9615 2024-05-28 13:59:57.756676 danila-lib-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 13:59:57.598383 danila-lib-1.8.3/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.3/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.8.3/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.3/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.3/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.3/danila/danila_v3.py
--rw-rw-rw-   0        0        0    24356 2024-05-28 10:23:30.000000 danila-lib-1.8.3/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:59:57.630241 danila-lib-1.8.3/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-28 13:59:57.000000 danila-lib-1.8.3/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-28 13:59:57.000000 danila-lib-1.8.3/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:59:57.000000 danila-lib-1.8.3/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-28 13:59:57.000000 danila-lib-1.8.3/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-28 13:59:57.000000 danila-lib-1.8.3/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 13:59:57.631236 danila-lib-1.8.3/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:59:57.682010 danila-lib-1.8.3/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.3/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.3/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.3/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.3/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.3/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.3/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.3/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.8.3/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.3/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.3/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:59:57.755680 danila-lib-1.8.3/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.3/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.3/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.3/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.3/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.3/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.3/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.3/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.3/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.3/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.3/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.3/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-28 13:59:57.765634 danila-lib-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-28 13:59:54.000000 danila-lib-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.439840 danila-lib-1.8.4/
+-rw-rw-rw-   0        0        0     9615 2024-05-30 06:42:37.439840 danila-lib-1.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.320376 danila-lib-1.8.4/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.4/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.8.4/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.4/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.4/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.4/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    24356 2024-05-28 10:23:30.000000 danila-lib-1.8.4/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.338295 danila-lib-1.8.4/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.338295 danila-lib-1.8.4/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.4/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.386081 danila-lib-1.8.4/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.4/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.4/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.4/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.4/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.4/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.4/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.4/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      880 2024-05-30 06:42:19.000000 danila-lib-1.8.4/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.4/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.4/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.438845 danila-lib-1.8.4/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.4/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.4/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.4/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.4/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.4/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.4/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.4/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.4/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.4/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.4/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.4/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:42:37.444818 danila-lib-1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-30 06:42:26.000000 danila-lib-1.8.4/setup.py
```

### Comparing `danila-lib-1.8.3/PKG-INFO` & `danila-lib-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.3
+Version: 1.8.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.3/README.md` & `danila-lib-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila/danila.py` & `danila-lib-1.8.4/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila/danila_v1.py` & `danila-lib-1.8.4/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila/danila_v2.py` & `danila-lib-1.8.4/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila/danila_v3.py` & `danila-lib-1.8.4/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila/danila_v4.py` & `danila-lib-1.8.4/danila/danila_v4.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.4/danila_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.3
+Version: 1.8.4
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.3/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.4/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.4/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/Letters_recognize.py` & `danila-lib-1.8.4/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.4/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.4/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.4/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/Text_detect_class.py` & `danila-lib-1.8.4/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/letters_in_image.py` & `danila-lib-1.8.4/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/models.py` & `danila-lib-1.8.4/data/neuro/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 RAMA_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/4xtNt0zftHFFVg'
 RAMA_BEGICKAYA_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/sE5iSXYWL3xEkQ'
 RAMA_RUZHIMMASH_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/zAEw0_ALgtBg9Q'
 RAMA_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/rgthm-mMrbhOmw'
 RAMA_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/QhicLdm2-PT6oA'
-TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS = 'https://disk.yandex.ru/d/C2hDMsbTZMnL8Q'
-TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS = 'https://disk.yandex.ru/d/C2hDMsbTZMnL8Q'
+# TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS = 'https://disk.yandex.ru/d/C2hDMsbTZMnL8Q' -7500_b7500_r
+# TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS = 'https://disk.yandex.ru/d/C2hDMsbTZMnL8Q'
+TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS = 'https://disk.yandex.ru/d/GcI-mAtwpb2I-g' # 11000_b_11000_r
+TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS = 'https://disk.yandex.ru/d/GcI-mAtwpb2I-g'  # 11000_b_11000_r
+
 RAMA_PROD_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/8FI8TaTwaCfbSA'
```

### Comparing `danila-lib-1.8.3/data/neuro/objs_in_image.py` & `danila-lib-1.8.4/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.4/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/result/Image_text_areas.py` & `danila-lib-1.8.4/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/result/Rect.py` & `danila-lib-1.8.4/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/result/Text_area.py` & `danila-lib-1.8.4/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/data/result/Yolo_label_rect.py` & `danila-lib-1.8.4/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.3/setup.py` & `danila-lib-1.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.8.3',
+  version='1.8.4',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

