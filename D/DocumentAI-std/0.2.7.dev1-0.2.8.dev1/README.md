# Comparing `tmp/DocumentAI_std-0.2.7.dev1.tar.gz` & `tmp/documentai_std-0.2.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DocumentAI_std-0.2.7.dev1.tar", last modified: Sat Apr 27 15:04:41 2024, max compression
+gzip compressed data, was "documentai_std-0.2.8.dev1.tar", last modified: Thu May 30 15:59:01 2024, max compression
```

## Comparing `DocumentAI_std-0.2.7.dev1.tar` & `documentai_std-0.2.8.dev1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/DocumentAI_std/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/__init__.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/__init__.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4851 2024-03-12 10:10:29.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/doc_element.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3296 2024-03-12 09:46:38.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/doc_element_classification.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3723 2024-03-05 18:02:12.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/doc_enum.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     5867 2024-03-12 09:44:24.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/document.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2694 2024-03-12 10:36:03.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/document_entity_classification.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/__init__.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4242 2024-04-26 14:57:10.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/cord.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2622 2024-04-26 14:58:56.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/funsd.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2814 2024-04-26 11:41:52.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/wildreceipt.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2678 2024-04-26 16:29:42.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/xfund.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7774 2024-04-26 10:47:09.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/OCR_adapter.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 10:23:11.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/__init__.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4515 2024-04-26 14:57:10.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/base_utils.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4855 2024-03-26 08:47:18.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/image_utils.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     6919 2024-03-09 14:06:30.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/layout_utils.py
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7406 2024-03-05 17:11:24.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/text_utils.py
-drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1534 2024-04-27 15:04:41.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/PKG-INFO
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      891 2024-04-27 15:04:41.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/SOURCES.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        1 2024-04-27 15:04:41.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/dependency_links.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      143 2024-04-27 15:04:41.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/requires.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       15 2024-04-27 15:04:41.000000 DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/top_level.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-01-24 16:32:43.000000 DocumentAI_std-0.2.7.dev1/LICENSE
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       24 2024-04-07 11:51:59.000000 DocumentAI_std-0.2.7.dev1/MANIFEST.in
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1534 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/PKG-INFO
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1302 2024-04-27 15:00:52.000000 DocumentAI_std-0.2.7.dev1/README.md
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      143 2024-04-08 16:31:54.000000 DocumentAI_std-0.2.7.dev1/requirements.txt
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       38 2024-04-27 15:04:41.124715 DocumentAI_std-0.2.7.dev1/setup.cfg
--rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      805 2024-04-27 15:03:25.000000 DocumentAI_std-0.2.7.dev1/setup.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-05-30 15:59:01.426057 documentai_std-0.2.8.dev1/
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-05-30 15:59:01.422724 documentai_std-0.2.8.dev1/DocumentAI_std/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 documentai_std-0.2.8.dev1/DocumentAI_std/__init__.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-05-30 15:59:01.422724 documentai_std-0.2.8.dev1/DocumentAI_std/base/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 documentai_std-0.2.8.dev1/DocumentAI_std/base/__init__.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4851 2024-03-12 10:10:29.000000 documentai_std-0.2.8.dev1/DocumentAI_std/base/doc_element.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3296 2024-03-12 09:46:38.000000 documentai_std-0.2.8.dev1/DocumentAI_std/base/doc_element_classification.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     3723 2024-03-05 18:02:12.000000 documentai_std-0.2.8.dev1/DocumentAI_std/base/doc_enum.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     5859 2024-04-30 16:20:38.000000 documentai_std-0.2.8.dev1/DocumentAI_std/base/document.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2694 2024-03-12 10:36:03.000000 documentai_std-0.2.8.dev1/DocumentAI_std/base/document_entity_classification.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-05-30 15:59:01.422724 documentai_std-0.2.8.dev1/DocumentAI_std/datasets/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 09:46:28.000000 documentai_std-0.2.8.dev1/DocumentAI_std/datasets/__init__.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4242 2024-04-26 14:57:10.000000 documentai_std-0.2.8.dev1/DocumentAI_std/datasets/cord.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2622 2024-04-26 14:58:56.000000 documentai_std-0.2.8.dev1/DocumentAI_std/datasets/funsd.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2792 2024-04-30 16:19:37.000000 documentai_std-0.2.8.dev1/DocumentAI_std/datasets/wildreceipt.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2678 2024-04-26 16:29:42.000000 documentai_std-0.2.8.dev1/DocumentAI_std/datasets/xfund.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-05-30 15:59:01.426057 documentai_std-0.2.8.dev1/DocumentAI_std/utils/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7774 2024-04-26 10:47:09.000000 documentai_std-0.2.8.dev1/DocumentAI_std/utils/OCR_adapter.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        0 2024-02-13 10:23:11.000000 documentai_std-0.2.8.dev1/DocumentAI_std/utils/__init__.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4521 2024-05-01 16:26:51.000000 documentai_std-0.2.8.dev1/DocumentAI_std/utils/base_utils.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     4829 2024-04-30 16:16:14.000000 documentai_std-0.2.8.dev1/DocumentAI_std/utils/image_utils.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     6911 2024-04-30 16:15:11.000000 documentai_std-0.2.8.dev1/DocumentAI_std/utils/layout_utils.py
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     7406 2024-03-05 17:11:24.000000 documentai_std-0.2.8.dev1/DocumentAI_std/utils/text_utils.py
+drwxr-xr-x   0 bobmarley  (1000) bobmarley  (1000)        0 2024-05-30 15:59:01.426057 documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2146 2024-05-30 15:59:01.000000 documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/PKG-INFO
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      891 2024-05-30 15:59:01.000000 documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/SOURCES.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)        1 2024-05-30 15:59:01.000000 documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/dependency_links.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      141 2024-05-30 15:59:01.000000 documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/requires.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       15 2024-05-30 15:59:01.000000 documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/top_level.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1062 2024-04-27 15:07:45.000000 documentai_std-0.2.8.dev1/LICENSE
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       24 2024-04-07 11:51:59.000000 documentai_std-0.2.8.dev1/MANIFEST.in
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     2146 2024-05-30 15:59:01.426057 documentai_std-0.2.8.dev1/PKG-INFO
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)     1302 2024-04-27 15:00:52.000000 documentai_std-0.2.8.dev1/README.md
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      141 2024-05-30 15:36:26.000000 documentai_std-0.2.8.dev1/requirements.txt
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)       38 2024-05-30 15:59:01.426057 documentai_std-0.2.8.dev1/setup.cfg
+-rw-r--r--   0 bobmarley  (1000) bobmarley  (1000)      972 2024-05-30 15:57:30.000000 documentai_std-0.2.8.dev1/setup.py
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/doc_element.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/base/doc_element.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/doc_element_classification.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/base/doc_element_classification.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/doc_enum.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/base/doc_enum.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/document.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/base/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
-from typing import Any, List, Tuple
+from typing import Any, List
 
 from PIL import Image
 
-from DocumentAI_std.base.doc_enum import ContentType
-
 from DocumentAI_std.base.doc_element import DocElement
+from DocumentAI_std.base.doc_enum import ContentType
 
 
 class Document:
     """
     Represents a document consisting of content elements defined by bounding boxes.
 
     A document is characterized by its content, where each content element is represented by a bounding box
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/base/document_entity_classification.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/base/document_entity_classification.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/cord.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/datasets/cord.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/funsd.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/datasets/funsd.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/wildreceipt.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/datasets/wildreceipt.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         self.train = train
         self.data: List[Document] = []
 
         with open(label_path, "r") as file:
             data = file.read()
         # Split the text file into separate JSON strings
         json_strings = data.strip().split("\n")
-        _targets = []
         for json_string in json_strings:
             json_data = json.loads(json_string)
             img_path = json_data["file_name"]
             annotations = json_data["annotations"]
 
             box_targets, text_targets, label_targets = zip(
                 *[
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/datasets/xfund.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/datasets/xfund.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/OCR_adapter.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/utils/OCR_adapter.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/base_utils.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/utils/base_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,16 @@
     def assign_line_label(line: str, entities: pd.DataFrame):
         line_set = line.replace(",", "").strip().split()
         for i, column in enumerate(entities):
             entity_values = entities.iloc[0, i].replace(",", "").strip()
             entity_set = entity_values.split()
 
             matches_count = 0
-            for l in line_set:
-                if any(SequenceMatcher(a=l, b=b).ratio() > 0.8 for b in entity_set):
+            for line in line_set:
+                if any(SequenceMatcher(a=line, b=b).ratio() > 0.8 for b in entity_set):
                     matches_count += 1
 
                 if (
                     (
                         column.upper() == "ADDRESS"
                         and (matches_count / len(line_set)) >= 0.5
                     )
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/image_utils.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/utils/image_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # TODO: Add a library for Embedding (Visaul, Text, and combined)
 import math
 
 import torch
-from scipy import ndimage
 from skimage.filters import gabor
 
 from DocumentAI_std.base.doc_element import DocElement
 
 
 class ImageUtils:
     @staticmethod
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/layout_utils.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/utils/layout_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,16 @@
         Args:
             a (DocElement): The first bounding box.
             b (DocElement): The second bounding box.
 
         Returns:
             HorizontalAlignment: Horizontal alignment ('left', 'center', 'right').
         """
-        x1, y1, w1, h1 = a.x, a.y, a.w, a.h
-        x2, y2, w2, h2 = b.x, b.y, b.w, b.h
+        x1, _, w1, _ = a.x, a.y, a.w, a.h
+        x2, _, w2, _ = b.x, b.y, b.w, b.h
 
         if x1 == x2:
             return HorizontalAlignment.CENTER
         elif x1 < x2:
             if x1 + w1 == x2:
                 return HorizontalAlignment.RIGHT
             else:
@@ -197,16 +197,16 @@
         Args:
             a (DocElement): The first bounding box.
             b (DocElement): The second bounding box.
 
         Returns:
             VerticalAlignment: Vertical alignment ('top', 'middle', 'bottom').
         """
-        x1, y1, w1, h1 = a.x, a.y, a.w, a.h
-        x2, y2, w2, h2 = b.x, b.y, b.w, b.h
+        _, y1, _, h1 = a.x, a.y, a.w, a.h
+        _, y2, _, h2 = b.x, b.y, b.w, b.h
 
         if y1 == y2:
             return VerticalAlignment.MIDDLE
         elif y1 < y2:
             if y1 + h1 == y2:
                 return VerticalAlignment.BOTTOM
             else:
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std/utils/text_utils.py` & `documentai_std-0.2.8.dev1/DocumentAI_std/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/PKG-INFO` & `documentai_std-0.2.8.dev1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: DocumentAI-std
-Version: 0.2.7.dev1
-Summary: The main standards for Latis Document AI project
-Home-page: 
-Author: Hamza Gbada
-Author-email: 
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DocumentAI-std
 
 **DocumentAI-std** is a Python library designed to facilitate and standardize document analysis and processing tasks. It offers functionality for handling document elements, performing optical character recognition (OCR), and managing document datasets.
 
 ## Installation
 
 To install **DocumentAI-std**, you can follow these steps:
@@ -46,8 +36,8 @@
 assert len(train_set.data) == 1267
 assert len(test_set.data) == 472
 ```
 
 In the above example:
 - We import the `Wildreceipt` dataset from the DocumentAI_std library.
 - We create train and test dataset instances, specifying the paths to image folders and annotation files.
-- We assert that the number of data samples in the train and test sets matches the expected counts.
+- We assert that the number of data samples in the train and test sets matches the expected counts.
```

### Comparing `DocumentAI_std-0.2.7.dev1/DocumentAI_std.egg-info/SOURCES.txt` & `documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DocumentAI_std-0.2.7.dev1/PKG-INFO` & `documentai_std-0.2.8.dev1/DocumentAI_std.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 Metadata-Version: 2.1
 Name: DocumentAI_std
-Version: 0.2.7.dev1
+Version: 0.2.8.dev1
 Summary: The main standards for Latis Document AI project
-Home-page: 
+Home-page: https://github.com/LATIS-DocumentAI-Group/DocumentAI-std
 Author: Hamza Gbada
-Author-email: 
+Author-email: hamza.gbada@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.11, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest==7.4.4
+Requires-Dist: easyocr==1.7.1
+Requires-Dist: pytesseract==0.3.10
+Requires-Dist: numpy>=1.26.3
+Requires-Dist: paddleocr==2.7.3
+Requires-Dist: Pillow==10.3.0
+Requires-Dist: PyMuPDF>=1.21.1
+Requires-Dist: setuptools
+Requires-Dist: paddlepaddle
+Requires-Dist: black
 
 # DocumentAI-std
 
 **DocumentAI-std** is a Python library designed to facilitate and standardize document analysis and processing tasks. It offers functionality for handling document elements, performing optical character recognition (OCR), and managing document datasets.
 
 ## Installation
```

### Comparing `DocumentAI_std-0.2.7.dev1/setup.py` & `documentai_std-0.2.8.dev1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from pathlib import Path
-
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
+
 setup(
     name="DocumentAI_std",
-    version="0.2.7.dev1",
-    # packages=find_packages(where='DocumentAI_std'),  # Include all packages within this directory
+    version="0.2.8.dev1",
     packages=find_packages(exclude=["DocumentAI_std.tests"]),
-    # package_dir={'': 'DocumentAI_std'},  # Set root package directory
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=required,
-    url="",
-    license="",
+    url="https://github.com/LATIS-DocumentAI-Group/DocumentAI-std",
+    license="MIT",
     author="Hamza Gbada",
-    author_email="",
+    author_email="hamza.gbada@gmail.com",
+    python_requires=">=3.11, <3.13",
     description="The main standards for Latis Document AI project",
+    classifiers=[
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: POSIX :: Linux",
+    ],
 )
```

