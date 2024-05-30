# Comparing `tmp/openwebmath_text_extract-0.1.0.tar.gz` & `tmp/openwebmath_text_extract-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwebmath_text_extract-0.1.0.tar", last modified: Thu May 30 03:45:49 2024, max compression
+gzip compressed data, was "openwebmath_text_extract-0.1.1.tar", last modified: Thu May 30 04:03:11 2024, max compression
```

## Comparing `openwebmath_text_extract-0.1.0.tar` & `openwebmath_text_extract-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 03:45:49.449358 openwebmath_text_extract-0.1.0/
--rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 03:45:49.449160 openwebmath_text_extract-0.1.0/PKG-INFO
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 03:45:49.448557 openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 03:45:49.000000 openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)      761 2024-05-30 03:45:49.000000 openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2024-05-30 03:45:49.000000 openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      218 2024-05-30 03:45:49.000000 openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       13 2024-05-30 03:45:49.000000 openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/top_level.txt
--rwxr-xr-x   0 lucas      (502) staff       (20)     2210 2024-05-30 03:44:15.000000 openwebmath_text_extract-0.1.0/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2024-05-30 03:45:49.449410 openwebmath_text_extract-0.1.0/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 03:45:49.443257 openwebmath_text_extract-0.1.0/text_extract/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1807 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/banned_selectors.txt
--rw-r--r--   0 lucas      (502) staff       (20)     1851 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/boilerplate_words.txt
--rw-r--r--   0 lucas      (502) staff       (20)     4763 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/extract.py
--rw-r--r--   0 lucas      (502) staff       (20)    27327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/latex_processing.py
--rw-r--r--   0 lucas      (502) staff       (20)     3141 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/line_processing.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 03:45:49.447746 openwebmath_text_extract-0.1.0/text_extract/mmltex/
--rw-r--r--   0 lucas      (502) staff       (20)     3189 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/README
--rw-r--r--   0 lucas      (502) staff       (20)    36723 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/cmarkup.xsl
--rw-r--r--   0 lucas      (502) staff       (20)    71528 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/entities.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     6333 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/glayout.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     1643 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/mmltex.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     9901 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/scripts.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     4327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/tables.xsl
--rw-r--r--   0 lucas      (502) staff       (20)    10654 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/mmltex/tokens.xsl
--rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:27:48.000000 openwebmath_text_extract-0.1.0/text_extract/py.typed
--rw-r--r--   0 lucas      (502) staff       (20)    14725 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/tree_processing.py
--rw-r--r--   0 lucas      (502) staff       (20)     3293 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.0/text_extract/utils.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.866155 openwebmath_text_extract-0.1.1/
+-rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 04:03:11.865968 openwebmath_text_extract-0.1.1/PKG-INFO
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.865381 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)      802 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      218 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       13 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/top_level.txt
+-rwxr-xr-x   0 lucas      (502) staff       (20)     2223 2024-05-30 04:02:51.000000 openwebmath_text_extract-0.1.1/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2024-05-30 04:03:11.866204 openwebmath_text_extract-0.1.1/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.861771 openwebmath_text_extract-0.1.1/text_extract/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1807 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/banned_selectors.txt
+-rw-r--r--   0 lucas      (502) staff       (20)     1851 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/boilerplate_words.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.861924 openwebmath_text_extract-0.1.1/text_extract/configs/
+-rw-r--r--   0 lucas      (502) staff       (20)      563 2024-05-30 04:01:08.000000 openwebmath_text_extract-0.1.1/text_extract/configs/randomized_all.yaml
+-rw-r--r--   0 lucas      (502) staff       (20)     4763 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/extract.py
+-rw-r--r--   0 lucas      (502) staff       (20)    27327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/latex_processing.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3141 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/line_processing.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.864699 openwebmath_text_extract-0.1.1/text_extract/mmltex/
+-rw-r--r--   0 lucas      (502) staff       (20)     3189 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/README
+-rw-r--r--   0 lucas      (502) staff       (20)    36723 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/cmarkup.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)    71528 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/entities.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     6333 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/glayout.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     1643 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/mmltex.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     9901 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/scripts.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     4327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/tables.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)    10654 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/tokens.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:27:48.000000 openwebmath_text_extract-0.1.1/text_extract/py.typed
+-rw-r--r--   0 lucas      (502) staff       (20)    14725 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/tree_processing.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3400 2024-05-30 04:02:36.000000 openwebmath_text_extract-0.1.1/text_extract/utils.py
```

### Comparing `openwebmath_text_extract-0.1.0/PKG-INFO` & `openwebmath_text_extract-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwebmath-text-extract
-Version: 0.1.0
+Version: 0.1.1
 Summary: Text Extractor from OpenWebMath
 Author-email: Keiran Paster <keirp@cs.toronto.edu>
 Maintainer-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/soldni/OpenWebMath
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/PKG-INFO` & `openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwebmath-text-extract
-Version: 0.1.0
+Version: 0.1.1
 Summary: Text Extractor from OpenWebMath
 Author-email: Keiran Paster <keirp@cs.toronto.edu>
 Maintainer-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/soldni/OpenWebMath
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openwebmath_text_extract-0.1.0/openwebmath_text_extract.egg-info/SOURCES.txt` & `openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 text_extract/boilerplate_words.txt
 text_extract/extract.py
 text_extract/latex_processing.py
 text_extract/line_processing.py
 text_extract/py.typed
 text_extract/tree_processing.py
 text_extract/utils.py
+text_extract/configs/randomized_all.yaml
 text_extract/mmltex/README
 text_extract/mmltex/cmarkup.xsl
 text_extract/mmltex/entities.xsl
 text_extract/mmltex/glayout.xsl
 text_extract/mmltex/mmltex.xsl
 text_extract/mmltex/scripts.xsl
 text_extract/mmltex/tables.xsl
```

### Comparing `openwebmath_text_extract-0.1.0/pyproject.toml` & `openwebmath_text_extract-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openwebmath-text-extract"
-version = "0.1.0"
+version = "0.1.1"
 description = "Text Extractor from OpenWebMath"
 authors = [
     {name = "Keiran Paster", email = "keirp@cs.toronto.edu" }
 ]
 maintainers = [
     {name = "Luca Soldaini", email = "luca@soldaini.net" }
 ]
@@ -25,15 +25,15 @@
 homepage = "https://github.com/soldni/OpenWebMath"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["text_extract*"]
 
 [tool.setuptools.package-data]
-"*" = ["py.typed", "*.pyi", "mmltex/*", "*txt", "*.py"]
+"*" = ["py.typed", "*.pyi", "mmltex/*", "*txt", "*.py", "configs/*"]
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
     "setuptools >= 61.0.0",
     "wheel"
 ]
```

### Comparing `openwebmath_text_extract-0.1.0/text_extract/banned_selectors.txt` & `openwebmath_text_extract-0.1.1/text_extract/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/boilerplate_words.txt` & `openwebmath_text_extract-0.1.1/text_extract/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/extract.py` & `openwebmath_text_extract-0.1.1/text_extract/extract.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/latex_processing.py` & `openwebmath_text_extract-0.1.1/text_extract/latex_processing.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/line_processing.py` & `openwebmath_text_extract-0.1.1/text_extract/line_processing.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/README` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/README`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/cmarkup.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/entities.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/glayout.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/mmltex.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/scripts.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/tables.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/mmltex/tokens.xsl` & `openwebmath_text_extract-0.1.1/text_extract/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/tree_processing.py` & `openwebmath_text_extract-0.1.1/text_extract/tree_processing.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.0/text_extract/utils.py` & `openwebmath_text_extract-0.1.1/text_extract/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from pathlib import Path
 import re
 import yaml
 import numpy as np
 
+CONFIG_PATH = str((Path(__file__).parent / "configs/randomize_all.yaml").absolute())
+
+
 def has_style(style, styles):
     """Does the style string contain any of the styles?
     This function is robust to variations in the spaces between the styles.
     """
     # Remove any spaces.
     style = style.replace(' ', '')
     styles = [s.replace(' ', '') for s in styles]
@@ -38,47 +42,47 @@
 
     if current_line:
         lines.append(" ".join(current_line))
 
     return "\n".join(lines)
 
 class ReplacementManager:
-    """This replacement manager simply adds tags next to the instances of the text. 
+    """This replacement manager simply adds tags next to the instances of the text.
     It contains a method to remove these tags."""
 
     def __init__(self):
         self.tags = []
 
     def add_replacement(self, text, tag='default'):
         self.tags.append(tag)
         return f'§§{tag}§§' + text
-    
+
     def remove_tags(self, text):
         tag_regex = "|".join(f'§§{tag}§§' for tag in self.tags)
         return re.sub(tag_regex, '', text)
-    
+
     def has_tag(self, text, tag):
         return f'§§{tag}§§' in text
 
 class Config:
     """A simple config object that loads a config from a YAML file and
     presents as a dictionary"""
 
-    def __init__(self, config_file):
+    def __init__(self, config_file: str = CONFIG_PATH):
         with open(config_file, 'r') as f:
             self.config = yaml.safe_load(f)
-        
+
     def sample_from_list(self, list):
         """Sample from a list of (probability, value) tuples."""
         probabilities = [p for p, _ in list]
         values = [v for _, v in list]
         probabilities = np.array(probabilities)
         probabilities /= probabilities.sum()
         return np.random.choice(values, p=probabilities)
-    
+
     def _sample(self, config):
         # For every value that has a type of list, first check it is in the format of:
         # - (probability, value)
         # - (probability, value)
         # - ...
         # And the probabilities sum to 1.
         # Then sample from the list.
@@ -91,10 +95,10 @@
                 # Sample from the list.
                 sampled_config[key] = self.sample_from_list(value)
             elif isinstance(value, dict):
                 sampled_config[key] = self._sample(value)
             else:
                 sampled_config[key] = value
         return sampled_config
-    
+
     def sample(self):
-        return self._sample(self.config)
+        return self._sample(self.config)
```

