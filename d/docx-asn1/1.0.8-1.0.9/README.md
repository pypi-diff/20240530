# Comparing `tmp/docx_asn1-1.0.8.tar.gz` & `tmp/docx_asn1-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_asn1-1.0.8.tar", last modified: Fri Apr 26 15:15:01 2024, max compression
+gzip compressed data, was "docx_asn1-1.0.9.tar", last modified: Thu May 30 19:11:52 2024, max compression
```

## Comparing `docx_asn1-1.0.8.tar` & `docx_asn1-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-04-26 15:15:01.210613 docx_asn1-1.0.8/
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1061 2024-04-26 15:03:12.000000 docx_asn1-1.0.8/LICENSE
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-04-26 15:15:01.210613 docx_asn1-1.0.8/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      388 2024-03-13 17:24:22.000000 docx_asn1-1.0.8/README.md
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-04-26 15:15:01.210613 docx_asn1-1.0.8/docx_asn1/
--rwxrwxr-x   0 n4n5      (1000) n4n5      (1000)       90 2024-03-13 17:10:15.000000 docx_asn1-1.0.8/docx_asn1/__init__.py
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      111 2024-03-13 16:55:43.000000 docx_asn1-1.0.8/docx_asn1/__main__.py
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1453 2024-04-26 15:13:56.000000 docx_asn1-1.0.8/docx_asn1/utils.py
-drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-04-26 15:15:01.210613 docx_asn1-1.0.8/docx_asn1.egg-info/
--rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-04-26 15:15:01.000000 docx_asn1-1.0.8/docx_asn1.egg-info/PKG-INFO
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      227 2024-04-26 15:15:01.000000 docx_asn1-1.0.8/docx_asn1.egg-info/SOURCES.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-04-26 15:15:01.000000 docx_asn1-1.0.8/docx_asn1.egg-info/dependency_links.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       10 2024-04-26 15:15:01.000000 docx_asn1-1.0.8/docx_asn1.egg-info/top_level.txt
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      698 2024-04-26 15:14:42.000000 docx_asn1-1.0.8/pyproject.toml
--rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-04-26 15:15:01.210613 docx_asn1-1.0.8/setup.cfg
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-30 19:11:52.587146 docx_asn1-1.0.9/
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1061 2024-04-26 15:03:12.000000 docx_asn1-1.0.9/LICENSE
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-05-30 19:11:52.587146 docx_asn1-1.0.9/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      388 2024-05-30 16:42:26.000000 docx_asn1-1.0.9/README.md
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-30 19:11:52.583146 docx_asn1-1.0.9/docx_asn1/
+-rwxrwxr-x   0 n4n5      (1000) n4n5      (1000)       90 2024-03-13 17:10:15.000000 docx_asn1-1.0.9/docx_asn1/__init__.py
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      111 2024-03-13 16:55:43.000000 docx_asn1-1.0.9/docx_asn1/__main__.py
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)     1883 2024-05-30 17:59:17.000000 docx_asn1-1.0.9/docx_asn1/utils.py
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-30 19:11:52.583146 docx_asn1-1.0.9/docx_asn1.egg-info/
+-rw-r--r--   0 n4n5      (1000) n4n5      (1000)     2177 2024-05-30 19:11:52.000000 docx_asn1-1.0.9/docx_asn1.egg-info/PKG-INFO
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      245 2024-05-30 19:11:52.000000 docx_asn1-1.0.9/docx_asn1.egg-info/SOURCES.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)        1 2024-05-30 19:11:52.000000 docx_asn1-1.0.9/docx_asn1.egg-info/dependency_links.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       10 2024-05-30 19:11:52.000000 docx_asn1-1.0.9/docx_asn1.egg-info/top_level.txt
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      698 2024-05-30 19:11:34.000000 docx_asn1-1.0.9/pyproject.toml
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)       38 2024-05-30 19:11:52.587146 docx_asn1-1.0.9/setup.cfg
+drwxrwxr-x   0 n4n5      (1000) n4n5      (1000)        0 2024-05-30 19:11:52.583146 docx_asn1-1.0.9/tests/
+-rw-rw-r--   0 n4n5      (1000) n4n5      (1000)      992 2024-05-30 17:10:04.000000 docx_asn1-1.0.9/tests/test_lib.py
```

### Comparing `docx_asn1-1.0.8/LICENSE` & `docx_asn1-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_asn1-1.0.8/PKG-INFO` & `docx_asn1-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-asn1
-Version: 1.0.8
+Version: 1.0.9
 Summary: Extract ASN.1 from DOCX files
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 n4n5
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `docx_asn1-1.0.8/docx_asn1/utils.py` & `docx_asn1-1.0.9/docx_asn1/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 from docx import Document
+from docx.oxml.ns import qn
+from docx.text.run import Run
 from sys import argv, stderr
 from os.path import isfile
 
+tab = qn("w:tab")
+
+
+def extract_paragraph(paragraph):
+    p = paragraph._element
+    # ---use XPath to get all the w:r descendents, wherever they may be---
+    rs = p.xpath(".//w:r")
+    # ---generate a Run object for each w:r element, in document order---
+    # for r in rs:
+    txt = "".join(["\t" if r.tag == tab else r.text for r in rs])
+    return txt
+
 
 def extract_text_from_docx(
     filename, start_text="-- ASN1START", stop_text="-- ASN1STOP", add=False
 ):
     """extract asn1 from a docx file"""
     if not isfile(filename):
         print(f"File {filename} not found", file=stderr)
         return None
     doc = Document(filename)
     full_text = []
     inside_range = False
     for para in doc.paragraphs:
-        if para.text.startswith(start_text):
+        text = extract_paragraph(para)
+        if text.startswith(start_text):
             if add:
-                full_text.append(para.text)
+                full_text.append(text)
             inside_range = True
             continue
-        elif para.text.startswith(stop_text):
+        elif text.startswith(stop_text):
             if add:
-                full_text.append(para.text)
+                full_text.append(text)
             inside_range = False
             continue
 
         # Add the paragraph text if inside the desired range
         if inside_range:
-            full_text.append(para.text)
+            full_text.append(text)
     return "\n".join(full_text)
 
 
 def main():
     """main function"""
     if len(argv) < 2:
         print("Usage: python decode_asn1.py <filename>", file=stderr)
```

### Comparing `docx_asn1-1.0.8/docx_asn1.egg-info/PKG-INFO` & `docx_asn1-1.0.9/docx_asn1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-asn1
-Version: 1.0.8
+Version: 1.0.9
 Summary: Extract ASN.1 from DOCX files
 Author-email: n4n5 <its.just.n4n5@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 n4n5
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `docx_asn1-1.0.8/pyproject.toml` & `docx_asn1-1.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docx-asn1"
-version = "1.0.8"
+version = "1.0.9"
 description = "Extract ASN.1 from DOCX files"
 readme = "README.md"
 authors = [{ name = "n4n5", email = "its.just.n4n5@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

