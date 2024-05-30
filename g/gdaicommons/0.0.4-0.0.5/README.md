# Comparing `tmp/gdaicommons-0.0.4.tar.gz` & `tmp/gdaicommons-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdaicommons-0.0.4.tar", last modified: Thu May 30 06:17:15 2024, max compression
+gzip compressed data, was "gdaicommons-0.0.5.tar", last modified: Thu May 30 20:50:03 2024, max compression
```

## Comparing `gdaicommons-0.0.4.tar` & `gdaicommons-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.4/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.4/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-30 06:14:44.000000 gdaicommons-0.0.4/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/gdaicommons/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:22:49.000000 gdaicommons-0.0.4/src/gdaicommons/__init__.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/gdaicommons/nlp/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-30 05:04:54.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2765 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/fill_mask.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2830 2024-05-30 06:08:30.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text2text_generation.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1839 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_classification.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2930 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_generation.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1831 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_labelling.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2817 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_summarization.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     7807 2024-05-30 05:47:59.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/transformations.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      262 2024-05-30 06:15:40.000000 gdaicommons-0.0.4/src/gdaicommons/utils.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/gdaicommons.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      571 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      833 2024-05-30 06:03:21.000000 gdaicommons-0.0.4/tests/test_suite.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 20:50:03.191905 gdaicommons-0.0.5/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.5/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 20:50:03.191905 gdaicommons-0.0.5/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.5/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-30 20:21:04.000000 gdaicommons-0.0.5/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-30 20:50:03.191905 gdaicommons-0.0.5/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 20:50:03.187905 gdaicommons-0.0.5/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 20:50:03.187905 gdaicommons-0.0.5/src/gdaicommons/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:22:49.000000 gdaicommons-0.0.5/src/gdaicommons/__init__.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 20:50:03.191905 gdaicommons-0.0.5/src/gdaicommons/nlp/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-30 05:04:54.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2765 2024-05-30 06:01:23.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/fill_mask.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2830 2024-05-30 06:08:30.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/text2text_generation.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1839 2024-05-30 06:01:23.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/text_classification.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2930 2024-05-30 06:01:23.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/text_generation.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1831 2024-05-30 06:01:23.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/text_labelling.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2817 2024-05-30 06:01:23.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/text_summarization.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     7860 2024-05-30 20:22:41.000000 gdaicommons-0.0.5/src/gdaicommons/nlp/transformations.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      262 2024-05-30 06:15:40.000000 gdaicommons-0.0.5/src/gdaicommons/utils.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 20:50:03.191905 gdaicommons-0.0.5/src/gdaicommons.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 20:50:03.000000 gdaicommons-0.0.5/src/gdaicommons.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      571 2024-05-30 20:50:03.000000 gdaicommons-0.0.5/src/gdaicommons.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-30 20:50:03.000000 gdaicommons-0.0.5/src/gdaicommons.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-30 20:50:03.000000 gdaicommons-0.0.5/src/gdaicommons.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 20:50:03.191905 gdaicommons-0.0.5/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      833 2024-05-30 06:03:21.000000 gdaicommons-0.0.5/tests/test_suite.py
```

### Comparing `gdaicommons-0.0.4/LICENSE` & `gdaicommons-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/PKG-INFO` & `gdaicommons-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdaicommons-0.0.4/pyproject.toml` & `gdaicommons-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdaicommons"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "AI transformation libraries and utilities to run on Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/fill_mask.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/fill_mask.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/text2text_generation.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/text_classification.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/text_classification.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/text_generation.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/text_generation.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/text_labelling.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/text_labelling.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/text_summarization.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/text_summarization.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/src/gdaicommons/nlp/transformations.py` & `gdaicommons-0.0.5/src/gdaicommons/nlp/transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .fill_mask import FillMaskTransformation
 from .text2text_generation import Text2TextGenerationTransformation
 from .text_classification import TextClassificationTransformation
 from .text_generation import TextGenerationTransformation
 from .text_labelling import TextLabellingTransformation
 from .text_summarization import TextSummarizationTransformation
 
+VALUE_SEPARATOR = "__sep__"
+
 
 @transformation_builder(name='text-classification-builder', is_batch=True)
 def text_classification(*args, **kwargs):
     model = kwargs['model']
     input_field = kwargs['input_field']
     output_field = kwargs['output_field']
     gpu_device = int(kwargs.get('gpu_device')) if 'gpu_device' in kwargs and kwargs['gpu_device'] else None
@@ -23,15 +25,15 @@
 
 @transformation_builder(name='text-labelling-builder', is_batch=True)
 def text_labelling(*args, **kwargs):
     model = kwargs['model']
     input_field = kwargs['input_field']
     output_field = kwargs['output_field']
     labels = kwargs['labels']
-    labels = str(labels).split(sep=",")
+    labels = str(labels).split(sep=VALUE_SEPARATOR)
     labels = [l.strip() for l in labels]
     gpu_device = int(kwargs.get('gpu_device')) if 'gpu_device' in kwargs and kwargs['gpu_device'] else None
 
     text_labeller = TextLabellingTransformation(model, input_field, output_field, labels,
                                                 gpu_device=gpu_device)
     return text_labeller.transform
 
@@ -40,15 +42,15 @@
 def fill_mask(*args, **kwargs):
     model = kwargs['model']
     input_field = kwargs['input_field']
     output_field = kwargs['output_field']
     mask_placeholder = kwargs.get('mask_placeholder', '[MASK]')
     mask_targets = kwargs.get('mask_targets', None)
     if mask_targets:
-        mask_targets = str(mask_targets).split(sep=",")
+        mask_targets = str(mask_targets).split(sep=VALUE_SEPARATOR)
         mask_targets = [t.strip() for t in mask_targets]
     gpu_device = int(kwargs.get('gpu_device')) if 'gpu_device' in kwargs and kwargs['gpu_device'] else None
 
     fill_mask_transformation = FillMaskTransformation(model, input_field, output_field,
                                                       mask_placeholder=mask_placeholder,
                                                       mask_targets=mask_targets,
                                                       top_k_scores=5,
```

### Comparing `gdaicommons-0.0.4/src/gdaicommons.egg-info/PKG-INFO` & `gdaicommons-0.0.5/src/gdaicommons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdaicommons-0.0.4/src/gdaicommons.egg-info/SOURCES.txt` & `gdaicommons-0.0.5/src/gdaicommons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.4/tests/test_suite.py` & `gdaicommons-0.0.5/tests/test_suite.py`

 * *Files identical despite different names*

