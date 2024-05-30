# Comparing `tmp/megaparse-0.0.2.tar.gz` & `tmp/megaparse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaparse-0.0.2.tar", last modified: Thu May 30 15:53:13 2024, max compression
+gzip compressed data, was "megaparse-0.0.3.tar", last modified: Thu May 30 16:23:17 2024, max compression
```

## Comparing `megaparse-0.0.2.tar` & `megaparse-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:13.748304 megaparse-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 15:53:09.000000 megaparse-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 15:53:13.748304 megaparse-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-30 15:53:09.000000 megaparse-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:13.748304 megaparse-0.0.2/megaparse/
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-30 15:53:09.000000 megaparse-0.0.2/megaparse/Converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:09.000000 megaparse-0.0.2/megaparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-30 15:53:09.000000 megaparse-0.0.2/megaparse/markdown_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 15:53:09.000000 megaparse-0.0.2/megaparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:53:13.748304 megaparse-0.0.2/megaparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 15:53:13.000000 megaparse-0.0.2/megaparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-30 15:53:13.000000 megaparse-0.0.2/megaparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:53:13.000000 megaparse-0.0.2/megaparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 15:53:13.000000 megaparse-0.0.2/megaparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:53:13.000000 megaparse-0.0.2/megaparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:53:13.748304 megaparse-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 15:53:09.000000 megaparse-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:17.538246 megaparse-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 16:23:08.000000 megaparse-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-30 16:23:17.538246 megaparse-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-30 16:23:08.000000 megaparse-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:17.534246 megaparse-0.0.3/megaparse/
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/markdown_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:17.538246 megaparse-0.0.3/megaparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:23:17.538246 megaparse-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 16:23:08.000000 megaparse-0.0.3/setup.py
```

### Comparing `megaparse-0.0.2/LICENSE` & `megaparse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.2/PKG-INFO` & `megaparse-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: megaparse
-Version: 0.0.2
-Summary: Parse complex files (PDF,Docx,PPTX) for LLM consumption
-Author: Quivr
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-docx
-Requires-Dist: mammoth
-Requires-Dist: python-pptx
-Requires-Dist: nest-asyncio
-Requires-Dist: llama-parse
-Requires-Dist: pdf2docx
-
 # MegaParse - Your Mega Parser for every type of documents
 
 <div align="center">
     <img src="https://raw.githubusercontent.com/QuivrHQ/MegaParse/main/logo.png" alt="Quivr-logo" width="30%"  style="border-radius: 50%; padding-bottom: 20px"/>
 </div>
 
 MegaParse is a powerful and versatile parser that can handle various types of documents with ease. Whether you're dealing with text, PDFs, Powerpoint presentations, Word documents MegaParse has got you covered. Focus on having no information loss during parsing.
@@ -23,14 +9,23 @@
 ## Key Features 🎯
 - **Versatile Parser**: MegaParse is a powerful and versatile parser that can handle various types of documents with ease.
 - **No Information Loss**: Focus on having no information loss during parsing.
 - **Fast and Efficient**: Designed with speed and efficiency at its core.
 - **Wide File Compatibility**: Supports Text, PDF, Powerpoint presentations, Excel, CSV, Word documents.
 - **Open Source**: Freedom is beautiful, and so is MegaParse. Open source and free to use.
 
+## Support
+- Files: ✅ PDF ✅ Powerpoint ✅ Word
+- Content: ✅ Tables ✅ TOC ✅ Headers ✅ Footers ✅ Images
+
+### Example
+
+<div align="center">
+    <img src="https://raw.githubusercontent.com/QuivrHQ/MegaParse/main/images/tables.png" alt="Quivr-logo" width="50%"  style="padding-bottom: 20px"/>
+</div>
 
 ## Installation
 
 ```bash
 pip install megaparse
 ```
 
@@ -52,7 +47,16 @@
 from megaparse import MegaParse
 
 megaparse = MegaParse(file_path="./test.pdf")
 content = megaparse.convert()
 print(content)
 megaparse.save_md(content, "./test.md")
 ```
+
+## Next Steps
+
+- [ ] Add Unstructured Parser Support
+- [ ] Improve Table Parsing
+- [ ] Improve Image Parsing and description
+- [ ] Add TOC for Docx
+- [ ] Add Hyperlinks for Docx
+- [ ] Order Headers for Docx to Markdown
```

### Comparing `megaparse-0.0.2/megaparse/Converter.py` & `megaparse-0.0.3/megaparse/Converter.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.2/megaparse/markdown_processor.py` & `megaparse-0.0.3/megaparse/markdown_processor.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.2/megaparse/utils.py` & `megaparse-0.0.3/megaparse/utils.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.2/megaparse.egg-info/PKG-INFO` & `megaparse-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaparse
-Version: 0.0.2
+Version: 0.0.3
 Summary: Parse complex files (PDF,Docx,PPTX) for LLM consumption
 Author: Quivr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-docx
 Requires-Dist: mammoth
 Requires-Dist: python-pptx
@@ -23,14 +23,23 @@
 ## Key Features 🎯
 - **Versatile Parser**: MegaParse is a powerful and versatile parser that can handle various types of documents with ease.
 - **No Information Loss**: Focus on having no information loss during parsing.
 - **Fast and Efficient**: Designed with speed and efficiency at its core.
 - **Wide File Compatibility**: Supports Text, PDF, Powerpoint presentations, Excel, CSV, Word documents.
 - **Open Source**: Freedom is beautiful, and so is MegaParse. Open source and free to use.
 
+## Support
+- Files: ✅ PDF ✅ Powerpoint ✅ Word
+- Content: ✅ Tables ✅ TOC ✅ Headers ✅ Footers ✅ Images
+
+### Example
+
+<div align="center">
+    <img src="https://raw.githubusercontent.com/QuivrHQ/MegaParse/main/images/tables.png" alt="Quivr-logo" width="50%"  style="padding-bottom: 20px"/>
+</div>
 
 ## Installation
 
 ```bash
 pip install megaparse
 ```
 
@@ -52,7 +61,16 @@
 from megaparse import MegaParse
 
 megaparse = MegaParse(file_path="./test.pdf")
 content = megaparse.convert()
 print(content)
 megaparse.save_md(content, "./test.md")
 ```
+
+## Next Steps
+
+- [ ] Add Unstructured Parser Support
+- [ ] Improve Table Parsing
+- [ ] Improve Image Parsing and description
+- [ ] Add TOC for Docx
+- [ ] Add Hyperlinks for Docx
+- [ ] Order Headers for Docx to Markdown
```

