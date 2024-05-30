# Comparing `tmp/openwebmath_text_extract-0.1.1.tar.gz` & `tmp/openwebmath_text_extract-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwebmath_text_extract-0.1.1.tar", last modified: Thu May 30 04:03:11 2024, max compression
+gzip compressed data, was "openwebmath_text_extract-0.1.2.tar", last modified: Thu May 30 04:10:48 2024, max compression
```

## Comparing `openwebmath_text_extract-0.1.1.tar` & `openwebmath_text_extract-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.866155 openwebmath_text_extract-0.1.1/
--rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 04:03:11.865968 openwebmath_text_extract-0.1.1/PKG-INFO
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.865381 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)      802 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      218 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       13 2024-05-30 04:03:11.000000 openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/top_level.txt
--rwxr-xr-x   0 lucas      (502) staff       (20)     2223 2024-05-30 04:02:51.000000 openwebmath_text_extract-0.1.1/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2024-05-30 04:03:11.866204 openwebmath_text_extract-0.1.1/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.861771 openwebmath_text_extract-0.1.1/text_extract/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1807 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/banned_selectors.txt
--rw-r--r--   0 lucas      (502) staff       (20)     1851 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/boilerplate_words.txt
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.861924 openwebmath_text_extract-0.1.1/text_extract/configs/
--rw-r--r--   0 lucas      (502) staff       (20)      563 2024-05-30 04:01:08.000000 openwebmath_text_extract-0.1.1/text_extract/configs/randomized_all.yaml
--rw-r--r--   0 lucas      (502) staff       (20)     4763 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/extract.py
--rw-r--r--   0 lucas      (502) staff       (20)    27327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/latex_processing.py
--rw-r--r--   0 lucas      (502) staff       (20)     3141 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/line_processing.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:03:11.864699 openwebmath_text_extract-0.1.1/text_extract/mmltex/
--rw-r--r--   0 lucas      (502) staff       (20)     3189 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/README
--rw-r--r--   0 lucas      (502) staff       (20)    36723 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/cmarkup.xsl
--rw-r--r--   0 lucas      (502) staff       (20)    71528 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/entities.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     6333 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/glayout.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     1643 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/mmltex.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     9901 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/scripts.xsl
--rw-r--r--   0 lucas      (502) staff       (20)     4327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/tables.xsl
--rw-r--r--   0 lucas      (502) staff       (20)    10654 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/mmltex/tokens.xsl
--rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:27:48.000000 openwebmath_text_extract-0.1.1/text_extract/py.typed
--rw-r--r--   0 lucas      (502) staff       (20)    14725 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.1/text_extract/tree_processing.py
--rw-r--r--   0 lucas      (502) staff       (20)     3400 2024-05-30 04:02:36.000000 openwebmath_text_extract-0.1.1/text_extract/utils.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:10:48.359866 openwebmath_text_extract-0.1.2/
+-rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 04:10:48.359515 openwebmath_text_extract-0.1.2/PKG-INFO
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:10:48.358706 openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     1002 2024-05-30 04:10:48.000000 openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)      802 2024-05-30 04:10:48.000000 openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2024-05-30 04:10:48.000000 openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      218 2024-05-30 04:10:48.000000 openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       13 2024-05-30 04:10:48.000000 openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/top_level.txt
+-rwxr-xr-x   0 lucas      (502) staff       (20)     2223 2024-05-30 04:10:35.000000 openwebmath_text_extract-0.1.2/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2024-05-30 04:10:48.359926 openwebmath_text_extract-0.1.2/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:10:48.353137 openwebmath_text_extract-0.1.2/text_extract/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1807 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/banned_selectors.txt
+-rw-r--r--   0 lucas      (502) staff       (20)     1851 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/boilerplate_words.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:10:48.353313 openwebmath_text_extract-0.1.2/text_extract/configs/
+-rw-r--r--   0 lucas      (502) staff       (20)      563 2024-05-30 04:01:08.000000 openwebmath_text_extract-0.1.2/text_extract/configs/randomized_all.yaml
+-rw-r--r--   0 lucas      (502) staff       (20)     4763 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/extract.py
+-rw-r--r--   0 lucas      (502) staff       (20)    27327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/latex_processing.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3141 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/line_processing.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2024-05-30 04:10:48.358100 openwebmath_text_extract-0.1.2/text_extract/mmltex/
+-rw-r--r--   0 lucas      (502) staff       (20)     3189 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/README
+-rw-r--r--   0 lucas      (502) staff       (20)    36723 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/cmarkup.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)    71528 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/entities.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     6333 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/glayout.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     1643 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/mmltex.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     9901 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/scripts.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)     4327 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/tables.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)    10654 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/mmltex/tokens.xsl
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2024-05-30 03:27:48.000000 openwebmath_text_extract-0.1.2/text_extract/py.typed
+-rw-r--r--   0 lucas      (502) staff       (20)    14725 2024-05-30 03:16:50.000000 openwebmath_text_extract-0.1.2/text_extract/tree_processing.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3401 2024-05-30 04:10:15.000000 openwebmath_text_extract-0.1.2/text_extract/utils.py
```

### Comparing `openwebmath_text_extract-0.1.1/PKG-INFO` & `openwebmath_text_extract-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwebmath-text-extract
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text Extractor from OpenWebMath
 Author-email: Keiran Paster <keirp@cs.toronto.edu>
 Maintainer-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/soldni/OpenWebMath
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/PKG-INFO` & `openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwebmath-text-extract
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text Extractor from OpenWebMath
 Author-email: Keiran Paster <keirp@cs.toronto.edu>
 Maintainer-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/soldni/OpenWebMath
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openwebmath_text_extract-0.1.1/openwebmath_text_extract.egg-info/SOURCES.txt` & `openwebmath_text_extract-0.1.2/openwebmath_text_extract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/pyproject.toml` & `openwebmath_text_extract-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openwebmath-text-extract"
-version = "0.1.1"
+version = "0.1.2"
 description = "Text Extractor from OpenWebMath"
 authors = [
     {name = "Keiran Paster", email = "keirp@cs.toronto.edu" }
 ]
 maintainers = [
     {name = "Luca Soldaini", email = "luca@soldaini.net" }
 ]
```

### Comparing `openwebmath_text_extract-0.1.1/text_extract/banned_selectors.txt` & `openwebmath_text_extract-0.1.2/text_extract/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/boilerplate_words.txt` & `openwebmath_text_extract-0.1.2/text_extract/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/configs/randomized_all.yaml` & `openwebmath_text_extract-0.1.2/text_extract/configs/randomized_all.yaml`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/extract.py` & `openwebmath_text_extract-0.1.2/text_extract/extract.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/latex_processing.py` & `openwebmath_text_extract-0.1.2/text_extract/latex_processing.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/line_processing.py` & `openwebmath_text_extract-0.1.2/text_extract/line_processing.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/README` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/README`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/cmarkup.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/entities.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/glayout.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/mmltex.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/scripts.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/tables.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/mmltex/tokens.xsl` & `openwebmath_text_extract-0.1.2/text_extract/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/tree_processing.py` & `openwebmath_text_extract-0.1.2/text_extract/tree_processing.py`

 * *Files identical despite different names*

### Comparing `openwebmath_text_extract-0.1.1/text_extract/utils.py` & `openwebmath_text_extract-0.1.2/text_extract/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import re
 import yaml
 import numpy as np
 
-CONFIG_PATH = str((Path(__file__).parent / "configs/randomize_all.yaml").absolute())
+CONFIG_PATH = str((Path(__file__).parent / "configs/randomized_all.yaml").absolute())
 
 
 def has_style(style, styles):
     """Does the style string contain any of the styles?
     This function is robust to variations in the spaces between the styles.
     """
     # Remove any spaces.
```

