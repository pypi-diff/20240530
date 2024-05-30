# Comparing `tmp/epubcrush-2.0.3.tar.gz` & `tmp/epubcrush-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubcrush-2.0.3.tar", last modified: Mon Apr 10 02:18:42 2023, max compression
+gzip compressed data, was "epubcrush-2.0.4.tar", last modified: Thu May 30 01:10:40 2024, max compression
```

## Comparing `epubcrush-2.0.3.tar` & `epubcrush-2.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-10 02:18:42.682225 epubcrush-2.0.3/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-10 02:18:42.682225 epubcrush-2.0.3/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-10 02:18:42.682225 epubcrush-2.0.3/epubcrush/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       59 2022-11-20 10:14:49.000000 epubcrush-2.0.3/epubcrush/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9445 2023-04-10 02:16:55.000000 epubcrush-2.0.3/epubcrush/epubcrush.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-04-10 02:18:42.682225 epubcrush-2.0.3/epubcrush.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2827 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      221 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       46 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/entry_points.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       10 2023-04-10 02:18:42.000000 epubcrush-2.0.3/epubcrush.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-04-10 02:18:42.686225 epubcrush-2.0.3/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      761 2023-04-10 02:17:28.000000 epubcrush-2.0.3/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2024-05-30 01:10:40.445893 epubcrush-2.0.4/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2890 2024-05-30 01:10:40.445893 epubcrush-2.0.4/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2024-05-30 01:10:40.445893 epubcrush-2.0.4/epubcrush/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       59 2022-11-20 10:14:49.000000 epubcrush-2.0.4/epubcrush/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    11901 2023-05-04 17:54:07.000000 epubcrush-2.0.4/epubcrush/epubcrush.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2024-05-30 01:10:40.445893 epubcrush-2.0.4/epubcrush.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2890 2024-05-30 01:10:40.000000 epubcrush-2.0.4/epubcrush.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      221 2024-05-30 01:10:40.000000 epubcrush-2.0.4/epubcrush.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2024-05-30 01:10:40.000000 epubcrush-2.0.4/epubcrush.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       46 2024-05-30 01:10:40.000000 epubcrush-2.0.4/epubcrush.egg-info/entry_points.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       10 2024-05-30 01:10:40.000000 epubcrush-2.0.4/epubcrush.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2024-05-30 01:10:40.445893 epubcrush-2.0.4/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      761 2024-05-30 01:10:09.000000 epubcrush-2.0.4/setup.py
```

### Comparing `epubcrush-2.0.3/PKG-INFO` & `epubcrush-2.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubcrush
-Version: 2.0.3
+Version: 2.0.4
 Summary: Compress EPUB files
 Home-page: https://github.com/jncraton/epubcrush
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: EPUB Crush
         ==========
@@ -26,17 +26,17 @@
         ```
         
         Performance
         -----------
         
         | File | Original |  txt  | txtz  | Images q=100 | Images q=50  |  No Images   |
         | ---- | -------- | ----- | ----- | ------------ | ------------ | ------------ |
-        |    1 |    589kB |  27kB |  12kB |  584kB (99%) |  257kB (44%) |   27kB ( 5%) |
-        |    2 |    589kB |  88kB |  30kB |  584kB (99%) |  285kB (48%) |   47kB ( 8%) |
-        |    3 |     87kB |  89kB |  34kB |   75kB (86%) |   49kB (56%) |   39kB (45%) |
+        |    1 |    589kB |  27kB |  11kB |  583kB (99%) |  256kB (43%) |   26kB ( 4%) |
+        |    2 |    589kB |  91kB |  31kB |  583kB (99%) |  284kB (48%) |   46kB ( 8%) |
+        |    3 |     87kB |  89kB |  34kB |   76kB (87%) |   50kB (57%) |   39kB (45%) |
         
         Why?
         -----
         
         EPUBs may include features that may not be desirable from a privacy or efficiency standpoint. Publishers may choose to include high-res images, custom fonts, styles, scripts, and other features that bloat the size of EPUBs beyond what is needed for the text content of a book. This application strips away everything but the plain text content.
         
         Why not use plain text?
@@ -50,19 +50,21 @@
         - Iterate files in container
         - Remove all files that are not part of the document text or part of the EPUB structure
         - Parse XML files
           - Remove the following tags
             - link
             - meta
             - style
+            - img
             - picture
             - audio
             - video
             - script
-          - Replace `img` tags with their alt text in a `p` tag
+        - Parse opf file removing references to files that no longer exist
+        - Remove print page lists
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `epubcrush-2.0.3/epubcrush/epubcrush.py` & `epubcrush-2.0.4/epubcrush/epubcrush.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from xml.etree import ElementTree
 import argparse
 import os
 
 
 def modernize_childrens(text):
     """
+    >>> modernize_childrens("I asked the policeman for help.")
+    'I asked the police officer for help.'
+    >>> modernize_childrens("The mailmen arrived.")
+    'The mail carriers arrived.'
     >>> modernize_childrens("You are queer.")
     'You are strange.'
     >>> modernize_childrens("I am a queer boy.")
     'I am a strange boy.'
     >>> modernize_childrens("She was feeling gay.")
     'She was feeling happy.'
     >>> modernize_childrens("Gay children played.")
@@ -112,15 +116,27 @@
                             flags=re.I,
                         )
 
                         if not images:
                             xml = re.sub('properties="svg"', "", xml)
 
                         newepub.writestr(file, xml)
+                    elif file.endswith("ncx"):
+                        xml = epub.open(file).read().decode("utf8")
+
+                        xml = ElementTree.canonicalize(xml)
+
+                        xml = re.sub(
+                            "<pageList>.*?</pageList>",
+                            "",
+                            xml,
+                            flags=re.I | re.M | re.DOTALL,
+                        )
 
+                        newepub.writestr(file, xml)
                     elif quality < 100 and re.match(r".*(jpeg|jpg)", file, flags=re.I):
                         jpeg = epub.extract(file, "/tmp")
                         compressed_jpeg = f"{jpeg}.comp.jpeg"
                         try:
                             run(
                                 [
                                     "/opt/mozjpeg/bin/cjpeg",
@@ -168,14 +184,34 @@
                         newepub.writestr(
                             file, epub.read(file), compress_type=ZIP_STORED
                         )
                     else:
                         newepub.writestr(file, epub.read(file))
 
 
+def get_nonanchor_text(xml: str):
+    """Return just plain text context not in <a> tags
+
+    >>> get_nonanchor_text("hello <a>world</a>")
+    'hello '
+    >>> get_nonanchor_text("<a id=1>hello world</a>")
+    ''
+    >>> get_nonanchor_text("<a id=1><span>hello</span> world</a>")
+    ''
+    >>> get_nonanchor_text("<a id=1>hello</a><p>world</p>")
+    'world'
+    """
+
+    xml = re.sub("<a.*?>.*?</a>", "", xml, flags=re.I | re.M | re.DOTALL)
+    xml = re.sub("<.*?>", "", xml, flags=re.I | re.M | re.DOTALL)
+    xml = re.sub("[\n\r\t ]+", " ", xml, flags=re.M)
+
+    return xml
+
+
 def clean_xml(xml: str, images=False, styles=False) -> str:
     """Cleans unwanted XML tags
 
     >>> clean_xml('<html></html>')
     '<html xmlns="http://www.w3.org/1999/xhtml"></html>'
 
     >>> clean_xml('<html><link></link></html>')
@@ -209,19 +245,57 @@
     exclude_tags = [
         "script",
         "audio",
         "video",
         "meta",
     ]
 
+    exclude_pages = [
+        "cover",
+        "titlepage",
+        "copyright-page",
+        "dedication",
+        "index",
+        "imprint",
+    ]
+
+    text_tags = [
+        "p",
+        "span",
+        "a",
+        "ol",
+        "ul",
+        "table",
+        "h1",
+        "h2",
+        "h3",
+        "h4",
+        "h5",
+        "h6",
+    ]
+
     if not images:
-        exclude_tags += ["picture", "svg", "{http://www.w3.org/2000/svg}svg"]
+        exclude_tags += ["img", "picture", "svg", "{http://www.w3.org/2000/svg}svg"]
 
     exclude_attrs = []
 
+    # Remove text from pages that are mostly links
+    anchors = re.findall("<a", xml, flags=re.I)
+    text = get_nonanchor_text(xml)
+    anchors_per_char = len(anchors) / max(1, len(text))
+    is_epub_toc = re.search('type="toc"', xml, flags=re.I)
+    if anchors_per_char > 0.02 and not is_epub_toc:
+        exclude_tags += text_tags
+
+    # Blank excluded pages (titlepage, dedication, etc)
+    if re.search(
+        '<(nav|body|div).*?epub:type="(' + "|".join(exclude_pages) + ')".*?>', xml
+    ):
+        exclude_tags += text_tags
+
     if not styles:
         exclude_tags += ["style", "link"]
         exclude_attrs += ["style", "class"]
 
     # Remove the default namespace definition
     xml = re.sub(r'\sxmlns="[^"]+"', "", xml, count=1)
     xml = xml.replace("&nbsp;", " ")
@@ -229,16 +303,29 @@
         xml,
         exclude_tags=exclude_tags,
         exclude_attrs=exclude_attrs,
     )
     # Ensure correct namespace definition
     xml = re.sub(r"<html", '<html xmlns="http://www.w3.org/1999/xhtml"', xml)
 
-    if not images:
-        xml = re.sub(r"<img.*>.*?</img>", "", xml)
+    # Remove page list used for printing
+    xml = re.sub(
+        '<nav epub:type="page-list">.*?</nav>', "", xml, flags=re.I | re.M | re.DOTALL
+    )
+
+    # Remove page breaks
+    xml = re.sub(
+        '<span[^>]+?type="pagebreak"[^>]*></span>',
+        "",
+        xml,
+        flags=re.M | re.I | re.DOTALL,
+    )
+
+    # Strip whitespace
+    xml = re.sub("[\r\n\t]+", "\n", xml, flags=re.M)
 
     return xml
 
 
 def repack(filename: str) -> None:
     run(["advzip", "-z", "-4", filename])
```

### Comparing `epubcrush-2.0.3/epubcrush.egg-info/PKG-INFO` & `epubcrush-2.0.4/epubcrush.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubcrush
-Version: 2.0.3
+Version: 2.0.4
 Summary: Compress EPUB files
 Home-page: https://github.com/jncraton/epubcrush
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: EPUB Crush
         ==========
@@ -26,17 +26,17 @@
         ```
         
         Performance
         -----------
         
         | File | Original |  txt  | txtz  | Images q=100 | Images q=50  |  No Images   |
         | ---- | -------- | ----- | ----- | ------------ | ------------ | ------------ |
-        |    1 |    589kB |  27kB |  12kB |  584kB (99%) |  257kB (44%) |   27kB ( 5%) |
-        |    2 |    589kB |  88kB |  30kB |  584kB (99%) |  285kB (48%) |   47kB ( 8%) |
-        |    3 |     87kB |  89kB |  34kB |   75kB (86%) |   49kB (56%) |   39kB (45%) |
+        |    1 |    589kB |  27kB |  11kB |  583kB (99%) |  256kB (43%) |   26kB ( 4%) |
+        |    2 |    589kB |  91kB |  31kB |  583kB (99%) |  284kB (48%) |   46kB ( 8%) |
+        |    3 |     87kB |  89kB |  34kB |   76kB (87%) |   50kB (57%) |   39kB (45%) |
         
         Why?
         -----
         
         EPUBs may include features that may not be desirable from a privacy or efficiency standpoint. Publishers may choose to include high-res images, custom fonts, styles, scripts, and other features that bloat the size of EPUBs beyond what is needed for the text content of a book. This application strips away everything but the plain text content.
         
         Why not use plain text?
@@ -50,19 +50,21 @@
         - Iterate files in container
         - Remove all files that are not part of the document text or part of the EPUB structure
         - Parse XML files
           - Remove the following tags
             - link
             - meta
             - style
+            - img
             - picture
             - audio
             - video
             - script
-          - Replace `img` tags with their alt text in a `p` tag
+        - Parse opf file removing references to files that no longer exist
+        - Remove print page lists
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `epubcrush-2.0.3/setup.py` & `epubcrush-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="epubcrush",
-    version="2.0.3",
+    version="2.0.4",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Compress EPUB files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/epubcrush",
     packages=setuptools.find_packages(),
```

