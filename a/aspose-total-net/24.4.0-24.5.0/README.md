# Comparing `tmp/aspose_total_net-24.4.0.tar.gz` & `tmp/aspose_total_net-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspose_total_net-24.4.0.tar", last modified: Tue Apr 30 15:31:22 2024, max compression
+gzip compressed data, was "aspose_total_net-24.5.0.tar", last modified: Thu May 30 19:36:14 2024, max compression
```

## Comparing `aspose_total_net-24.4.0.tar` & `aspose_total_net-24.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 15:31:22.352939 aspose_total_net-24.4.0/
--rw-rw-rw-   0        0        0       38 2023-07-11 21:08:19.000000 aspose_total_net-24.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    14642 2024-04-30 15:31:22.346296 aspose_total_net-24.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    12341 2024-04-30 15:28:19.000000 aspose_total_net-24.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 15:31:22.292327 aspose_total_net-24.4.0/aspose-total-net/
--rw-rw-rw-   0        0        0        0 2022-05-30 04:52:54.000000 aspose_total_net-24.4.0/aspose-total-net/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 15:31:22.341437 aspose_total_net-24.4.0/aspose_total_net.egg-info/
--rw-rw-rw-   0        0        0    14642 2024-04-30 15:31:22.000000 aspose_total_net-24.4.0/aspose_total_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-04-30 15:31:22.000000 aspose_total_net-24.4.0/aspose_total_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 15:31:22.000000 aspose_total_net-24.4.0/aspose_total_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-06-06 08:16:12.000000 aspose_total_net-24.4.0/aspose_total_net.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      420 2024-04-30 15:31:22.000000 aspose_total_net-24.4.0/aspose_total_net.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-30 15:31:22.000000 aspose_total_net-24.4.0/aspose_total_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      213 2023-07-11 21:07:56.000000 aspose_total_net-24.4.0/license.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 15:31:22.354949 aspose_total_net-24.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2984 2024-04-30 15:24:43.000000 aspose_total_net-24.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 19:36:14.218988 aspose_total_net-24.5.0/
+-rw-rw-rw-   0        0        0       38 2023-07-11 21:08:19.000000 aspose_total_net-24.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15563 2024-05-30 19:36:14.204980 aspose_total_net-24.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13225 2024-05-30 19:22:20.000000 aspose_total_net-24.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 19:36:14.119415 aspose_total_net-24.5.0/aspose-total-net/
+-rw-rw-rw-   0        0        0        0 2022-05-30 04:52:54.000000 aspose_total_net-24.5.0/aspose-total-net/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 19:36:14.191982 aspose_total_net-24.5.0/aspose_total_net.egg-info/
+-rw-rw-rw-   0        0        0    15563 2024-05-30 19:36:13.000000 aspose_total_net-24.5.0/aspose_total_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-30 19:36:13.000000 aspose_total_net-24.5.0/aspose_total_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 19:36:13.000000 aspose_total_net-24.5.0/aspose_total_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-06-06 08:16:12.000000 aspose_total_net-24.5.0/aspose_total_net.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      441 2024-05-30 19:36:13.000000 aspose_total_net-24.5.0/aspose_total_net.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 19:36:13.000000 aspose_total_net-24.5.0/aspose_total_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      213 2023-07-11 21:07:56.000000 aspose_total_net-24.5.0/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 19:36:14.221982 aspose_total_net-24.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3020 2024-05-30 19:27:29.000000 aspose_total_net-24.5.0/setup.py
```

### Comparing `aspose_total_net-24.4.0/PKG-INFO` & `aspose_total_net-24.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,178 +1,187 @@
 Metadata-Version: 2.1
 Name: aspose-total-net
-Version: 24.4.0
+Version: 24.5.0
 Summary: Aspose.Total for Python via .NET is a Document Processing python class library that allows developers to work with Microsoft Word®, Microsoft PowerPoint®, Microsoft Outlook®, OpenOffice®, & 3D file formats without needing Office Automation.
 Home-page: https://products.aspose.com/total/python-net
 Author: Aspose
 Author-email: total@aspose.com
 Keywords: DOC,DOCX,RTF,DOT,DOTX,DOTM,DOCM FlatOPC,FlatOpcMacroEnabled,FlatOpcTemplate,FlatOpcTemplateMacroEnabled,ODT,OTT,WordML,HTML,MHTML,PDF,MOBI,TXT,PDF/A,XPS,OpenXPS,PostScript (PS),TIFF,JPEG,PNG,BMP,SVG,EMF,GIF,HtmlFixed,PCL,EPUB,XamlFixed,XamlFlow,XamlFlowPack,MSG,PST,OST,OFT,EML,EMLX,MBOX,ICS,VCF,OLM,PPT,PPTX,PPS,POT,PPSX,PPTM,PPSM,POTX,POTM,ODP,FBX,STL,OBJ,3DS,U3D,DAE,glTF,ASCII,Binary,DRC,RVM,AMF,PLY,A3DW,X,DirectX,JT,DXF,3MF,ASE,VRML,Create,Clone,Render,Compare,Join,Split,Encrypt,Digital Signature,Mail Merge,Reporting,Watermark,LINQ,Reporting Engine,Editor,Merger,Viewer,Conversion,Splitter,OCR,Translator,Compress,SSL,TLS,TNEF,Email Attachment,Email,POP3,IMAP,iCalendar,OleObject,Chart,3D,Scene,Triangulate,Vulkan,Geometry,Camera,Mesh,Shape
 Platform: Operating System :: MacOS :: MacOS X
 Platform: Operating System :: Microsoft :: Windows :: Windows 7
 Platform: Operating System :: Microsoft :: Windows :: Windows Vista
 Platform: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: license.txt
-Requires-Dist: aspose-3d==24.4.0
-Requires-Dist: aspose-barcode-for-python-via-net==24.4
-Requires-Dist: aspose-cad==24.3.0
-Requires-Dist: aspose-cells-python==24.4.0
-Requires-Dist: aspose-diagram-python==24.4
-Requires-Dist: Aspose.Email-for-Python-via-NET==24.4
-Requires-Dist: aspose-finance==24.3
-Requires-Dist: aspose-imaging-python-net==24.4.0
-Requires-Dist: aspose-ocr-python-net==24.3.0
+Requires-Dist: aspose-3d==24.5.0
+Requires-Dist: aspose-barcode-for-python-via-net==24.5
+Requires-Dist: aspose-cad==24.4
+Requires-Dist: aspose-cells-python==24.5.0
+Requires-Dist: aspose-diagram-python==24.5
+Requires-Dist: Aspose.Email-for-Python-via-NET==24.5
+Requires-Dist: aspose-finance==24.4
+Requires-Dist: aspose-imaging-python-net==24.5.0
+Requires-Dist: aspose-ocr-python-net==24.5.0
 Requires-Dist: aspose-page==24.2.0
-Requires-Dist: aspose-pdf==24.4.0
-Requires-Dist: aspose-psd==24.2.0
-Requires-Dist: Aspose.Slides==24.4.0
-Requires-Dist: aspose-tasks==24.4.0
+Requires-Dist: aspose-pdf==24.5.0
+Requires-Dist: aspose-psd==24.4.0
+Requires-Dist: Aspose.Slides==24.5.0
+Requires-Dist: aspose-svg-net==24.5.0
+Requires-Dist: aspose-tasks==24.5.0
 Requires-Dist: aspose-tex-net==24.3.0
-Requires-Dist: aspose-words==24.4.0
-Requires-Dist: aspose-zip==24.4.0
+Requires-Dist: aspose-words==24.5.0
+Requires-Dist: aspose-zip==24.5.0
 
 [Product Page](https://products.aspose.com/total/python-net) | [Docs](https://docs.aspose.com/total/pythonnet/) | [Demos](https://products.aspose.app/total/family) | [Examples](https://aspose.github.io/) | [Download](https://downloads.aspose.com/total/pythonnet) | [Blog](https://blog.aspose.com/category/total/) | [Releases](https://releases.aspose.com/) | [Free Support](https://forum.aspose.com/c/total/7) | [Temporary License](https://purchase.aspose.com/temporary-license)
 
 Aspose.Total for Python via .NET is a collection of powerful yet easy-to-use document processing libraries for Python developers. Create, edit, convert DOC, DOCX, XLSX, XLS, CSV, PPT, PPTX, EML, MSG, 3D, and more formats within Python apps. Render PDF and images with high fidelity, compare documents, protect or encrypt, mail merge, clone slides, work with PowerPoint tables, generate presentations from the database, create custom charts, handle email formats, TNEF attachments, and send/receive emails. Plus, manipulate 3D and CAD files. Aspose.Total for Python via .NET handles a multitude of file formats, including Microsoft Word, PowerPoint, Outlook, OpenOffice, Web, Fixed Layout, Images, and 3D & CAD files. Make Next Generation document processing Apps now!
 
 This release includes the following:
 
-# [Aspose.3D for Python via .NET](https://releases.aspose.com/3d/python-net/) (v24.4.0)
+# [Aspose.3D for Python via .NET](https://releases.aspose.com/3d/python-net/) (v24.5.0)
 
 Unleash the power of Aspose.3D for Python via .NET, the ultimate Python 3D manipulation high code API. Effortlessly create, process, manipulate, and convert 3D scenes, meshes, and entities - no need for 3rd party software. Enjoy scene creation, animation, geometry, scene hierarchy, triangulate mesh, target camera, 3D plane, shadows, cylinders, conversion, import, and export capabilities. Grow your 3D projects with seamless integration and exceptional 3D control!
 
 ```python
-pip install aspose-3d==24.4.0
+pip install aspose-3d==24.5.0
 ```
 
-# [Aspose.BarCode for Python via .NET](https://releases.aspose.com/barcode/python-net/) (v24.4.0)
+# [Aspose.BarCode for Python via .NET](https://releases.aspose.com/barcode/python-net/) (v24.5.0)
 
 Aspose.BarCode for Python via .NET is a barcode generation and scanning library for .NET and Python developers. Create barcode images with precise control over size, captions, colors, and font. Generate QR, MicroQR, and Datamatrix barcodes with custom error correction and encoding. Support error correction and checksum for various symbologies. Adjust 2D barcode size and aspect ratio. Customize image border and style. Detect Unicode encoding, hide long codetext, or reduce font size. Colorize barcode, code text, background, border, and caption. Specify size unit in document, inch, millimeter, pixel, or point.
 
 ```python
-pip install aspose-barcode-for-python-via-net==24.4
+pip install aspose-barcode-for-python-via-net==24.5
 ```
 
-# [Aspose.CAD for Python via .NET](https://releases.aspose.com/cad/python-net/) (v24.3.0)
+# [Aspose.CAD for Python via .NET](https://releases.aspose.com/cad/python-net/) (v24.4.0)
 
 Aspose.CAD for Python via .NET is ultimate CAD and BIM drawing processing API for .NET and Python developers. Enhance your apps with high-quality conversion and rendering of DWG, DWF, DWFX, DGN, STL, OBJ, CF2, IGES, IFC, DXF, and more formats to PDF and images. No need for AutoCAD&reg; or rendering workflows. Manipulate drawing entities and blocks, select specific layouts and layers, and adjust drawing size before rendering. Exciting new features in Version 23.6 include support for OBJ file format export, HoloLens 2, and AutoCAD Plotter Configuration (PC3) files.
 
 ```python
-pip install aspose-cad==24.3.0
+pip install aspose-cad==24.4
 ```
 
-# [Aspose.Cells for Python via .NET](https://releases.aspose.com/cells/python-net/) (v24.4.0)
+# [Aspose.Cells for Python via .NET](https://releases.aspose.com/cells/python-net/) (v24.5.0)
 
 Experience the full potential of Aspose.Cells for Python via .NET, our Excel&reg; file handling solution for .NET and Python developers. Create, manipulate, and save Excel&reg; files with ease. Benefit from high-quality format conversion, rendering, and printing capabilities. Effortlessly customize charts, Pivot Tables, and apply advanced formatting. Protect, merge, and parse Excel&reg; sheets seamlessly. Convert charts to images and PDFs while supporting various file formats. Take advantage of the formula calculation engine with support for all Excel functions.
 
 ```python
-pip install aspose-cells-python==24.4.0
+pip install aspose-cells-python==24.5.0
 ```
 
-# [Aspose.Diagram for Python via .NET](https://releases.aspose.com/diagram/python-net/) (v24.4.0)
+# [Aspose.Diagram for Python via .NET](https://releases.aspose.com/diagram/python-net/) (v24.5.0)
 
 Improve Visio&reg; file processing with Aspose.Diagram for Python via .NET. Seamlessly create, manipulate, and convert Visio&reg; files, all without Microsoft Office&reg; dependencies. Enjoy features like shape conversion, comment management, and versatile format inter-conversion. Elevate your Python development workflow now!
 
 ```python
-pip install aspose-diagram-python==24.4
+pip install aspose-diagram-python==24.5
 ```
 
-# [Aspose.Email for Python via .NET](https://releases.aspose.com/email/pythonnet/) (v24.4.0)
+# [Aspose.Email for Python via .NET](https://releases.aspose.com/email/pythonnet/) (v24.5.0)
 
 Boost your Python applications with Aspose.Email for Python via .NET, an on-premise API designed to streamline email handling. Send & receive emails with attachments, perform email rendering and format conversions, and download messages from POP3 and IMAP servers. Seamlessly send iCalendar compliant appointments or meetings and work with message storage files. SSL & TLS support included. Uplift your email capabilities now!
 
 ```python
-pip install Aspose.Email-for-Python-via-NET==24.4
+pip install Aspose.Email-for-Python-via-NET==24.5
 ```
 
-# [Aspose.Finance for Python via .NET](https://releases.aspose.com/finance/python-net/) (v24.3.0)
+# [Aspose.Finance for Python via .NET](https://releases.aspose.com/finance/python-net/) (v24.4.0)
 
 Aspose.Finance for Python via .NET is a powerful API for processing finance-related formats like XBRL, iXBRL, and OFX using Python. It allows creation, manipulation, and conversion of XBRL, iXBRL, and OFX files, providing a comprehensive solution for developers. With features like XBRL and iXBRL creation, format conversion, validation, and more, Aspose.Finance streamlines financial data handling with ease and efficiency.
 
 ```python
-pip install aspose-finance==24.3
+pip install aspose-finance==24.4
 ```
 
-# [Aspose.Imaging for Python via .NET](https://releases.aspose.com/imaging/python-net/) (v24.4.0)
+# [Aspose.Imaging for Python via .NET](https://releases.aspose.com/imaging/python-net/) (v24.5.0)
 
 Aspose.Imaging for Python via .NET is an advanced image processing library. Easily create, load, manipulate, convert, compress images. Supports drawing and graphic primitives. Core features include; image export & conversion, transformations (resize, crop, flip &rotate, etc.), filtering, memory optimization. Handles popular formats like DjVu, DICOM, WebP & DNG, and extends .NET & .NET Core support. Cross-platform; Windows & Linux compatible. Explore powerful features now: create, read, write, draw, process & convert images effortlessly with Aspose.Imaging!
 
 ```python
-pip install aspose-imaging-python-net==24.4.0
+pip install aspose-imaging-python-net==24.5.0
 ```
 
-# [Aspose.OCR for Python via .NET](https://releases.aspose.com/ocr/python-net/) (v24.3.0)
+# [Aspose.OCR for Python via .NET](https://releases.aspose.com/ocr/python-net/) (v24.5.0)
 
 Aspose.OCR for Python via .NET is an easy-to-use OCR engine for Python Apps. Recognize text in 28 languages, Latin, Cyrillic & Asian scripts. Extract text from scans, photos, PDFs. Handle blurry, distorted, rotated, noisy images. Preserve original layout, detect paragraphs, lines, single words. Bulk process multipage docs, folders, archives. Identify misspelled words, compare image texts. Simplify OCR tasks with Aspose.OCR!
 
 ```python
-pip install aspose-ocr-python-net==24.3.0
+pip install aspose-ocr-python-net==24.5.0
 ```
 
 # [Aspose.Page for Python via .NET](https://releases.aspose.com/page/python-net/) (v24.2.0)
 
 Aspose.Page for Python via .NET empowers developers to work with PS, EPS, and XPS formats seamlessly, eliminating the need for Microsoft Office or Adobe products entirely. Streamline your document processing workflows today! Effortlessly integrate this lightweight library into your Python projects using pip.
 
 ```python
 pip install aspose-page==24.2.0
 ```
 
-# [Aspose.PDF for Python via .NET](https://releases.aspose.com/pdf/pythonnet/) (v24.4.0)
+# [Aspose.PDF for Python via .NET](https://releases.aspose.com/pdf/pythonnet/) (v24.5.0)
 
 Aspose.PDF for Python via .NET is a powerful native library for PDF processing in your applications. Generate, read, convert, and manipulate PDF files without Adobe Acrobat&reg;. Perform form processing, metadata handling, text and page manipulation, annotations management, bookmarks and watermarks, attachments, custom font handling, and more. Supercharge your PDF capabilities via API!
 
 ```python
-pip install aspose-pdf==24.4.0
+pip install aspose-pdf==24.5.0
 ```
 
-# [Aspose.PSD for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.2.0)
+# [Aspose.PSD for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.4.0)
 
 Aspose.PSD for Python simplifies handling of PSD, PSB, and AI files. It allows creation, editing, conversion, and export to various formats while supporting advanced features like layer manipulation, effects, and drawing tools. This cross-platform library caters to diverse use cases with robust functionality.
 
 ```python
-pip install aspose-psd==24.2.0
+pip install aspose-psd==24.4.0
 ```
 
-# [Aspose.Slides for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.4.0)
+# [Aspose.Slides for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.5.0)
 
 Level up your Python programs with Aspose.Slides for Python via .NET - the ultimate Python class library for PowerPoint&reg; & OpenOffice&reg; presentations. No need to install Microsoft PowerPoint&reg; or any 3rd party software. Effortlessly create, clone, and manipulate slides from templates. Master slides, animations, charts, shapes, OLE, VBA Macros, video frames, picture frames, audio frames, encryption, and decryption - all at your fingertips. Elevate your presentation game now!
 
 ```python
-pip install Aspose.Slides==24.4.0
+pip install Aspose.Slides==24.5.0
 ```
 
-# [Aspose.Tasks for Python via .NET](https://releases.aspose.com/tasks/python-net/) (v24.4.0)
+# [Aspose.SVG for Python via .NET](https://releases.aspose.com/svg/python-net/) (v24.5.0)
+
+Aspose.SVG for Python via .NET is a versatile on-premise class library designed to handle a variety of tasks involving SVG files without the need for additional SVG tools. It enables you to create, edit, optimize, and convert SVG files. The Python API allows for document and element manipulation, providing advanced navigation and inspection features such as XPath queries and CSS selectors. Developers can also vectorize images and texts, apply SVG transformations, filters, gradients, and patterns, and specify colors in various formats. Aspose.SVG for Python via .NET is ideal for creating applications like SVG editors, converters, mergers, and image vectorizers, offering comprehensive SVG processing capabilities for developers.
+
+```python
+pip install aspose-svg-net==24.5.0
+```
+
+# [Aspose.Tasks for Python via .NET](https://releases.aspose.com/tasks/python-net/) (v24.5.0)
 
 Aspose.Tasks for Python via .NET, a powerful native library for adding MS-Project file processing capabilities to your applications. Easily create, read, convert, and manipulate MS-Project files without Microsoft Project&reg; itself. Perform calculations, manage tasks, resources, and calendars, manipulate views, and handle attachments effortlessly. Enjoy features like export to various image formats, XLSX, HTML, CSV, and PDF, along with support for Oracle Primavera&reg; and Project Server. Supported MS-Project versions include 2003 to 2021. Convert MPP to images, Excel, HTML, CSV, and PDF with ease. Manage tasks, resources, assignments, and customize Gantt Chart view styles.
 
 ```python
-pip install aspose-tasks==24.4.0
+pip install aspose-tasks==24.5.0
 ```
 
 # [Aspose.TeX for Python via .NET](https://releases.aspose.com/tex/python-net/) (v24.3.0)
 
 Streamline your document creation process with Aspose.TeX for Python via .NET, the powerful TeX/LaTeX processing library for developers Effortlessly typeset complex documents in various TeX and LaTeX formats, without relying on external software. Get started quickly by integrating Aspose.TeX into your Python projects using pip.
 
 ```python
 pip install aspose-tex-net==24.3.0
 ```
 
-# [Aspose.Words for Python via .NET](https://releases.aspose.com/words/python/) (v24.4.0)
+# [Aspose.Words for Python via .NET](https://releases.aspose.com/words/python/) (v24.5.0)
 
 Empower your Python applications with Aspose.Words for Python via .NET, an on-premise API for seamless Microsoft Word&reg; document handling. Create, edit, render, and convert Word&reg; files to various formats (PDF, XPS, Raster Image, PCL, EPUB, etc.) effortlessly. Enjoy report generation, data visualization, and a range of document tasks like viewing, merging, splitting, translating, watermarking, and comparison. Level up your document processing now!
 
 ```python
-pip install aspose-words==24.4.0
+pip install aspose-words==24.5.0
 ```
 
-# [Aspose.ZIP for Python via .NET](https://releases.aspose.com/zip/python-net/) (v24.4.0)
+# [Aspose.ZIP for Python via .NET](https://releases.aspose.com/zip/python-net/) (v24.5.0)
 
 Aspose.ZIP for Python via .NET is a powerful Python API to create, manipulate, extract & protect archive formats - ZIP, BZIP, BZ2 & TAR. Simplify compression/decompression in your Python apps without complex coding. Offers a wide range of features, including archive creation, extraction, encryption (password, AES), and compressing single/multiple files and directories. Secure your files with password or AES encryption. Explore advanced options like appending files to existing archives, Gzip/Bzip2 packing into TAR archives, and creating self-extracting compressed archives.
 
 ```python
-pip install aspose-zip==24.4.0
+pip install aspose-zip==24.5.0
 ```
 
 [Product Page](https://products.aspose.com/total/python-net) | [Docs](https://docs.aspose.com/total/pythonnet/) | [Demos](https://products.aspose.app/total/family) | [Examples](https://aspose.github.io/) | [Download](https://downloads.aspose.com/total/pythonnet) | [Blog](https://blog.aspose.com/category/total/) | [Releases](https://releases.aspose.com/) | [Free Support](https://forum.aspose.com/c/total/7) | [Temporary License](https://purchase.aspose.com/temporary-license)
```

### Comparing `aspose_total_net-24.4.0/README.md` & `aspose_total_net-24.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,143 +1,151 @@
 [Product Page](https://products.aspose.com/total/python-net) | [Docs](https://docs.aspose.com/total/pythonnet/) | [Demos](https://products.aspose.app/total/family) | [Examples](https://aspose.github.io/) | [Download](https://downloads.aspose.com/total/pythonnet) | [Blog](https://blog.aspose.com/category/total/) | [Releases](https://releases.aspose.com/) | [Free Support](https://forum.aspose.com/c/total/7) | [Temporary License](https://purchase.aspose.com/temporary-license)
 
 Aspose.Total for Python via .NET is a collection of powerful yet easy-to-use document processing libraries for Python developers. Create, edit, convert DOC, DOCX, XLSX, XLS, CSV, PPT, PPTX, EML, MSG, 3D, and more formats within Python apps. Render PDF and images with high fidelity, compare documents, protect or encrypt, mail merge, clone slides, work with PowerPoint tables, generate presentations from the database, create custom charts, handle email formats, TNEF attachments, and send/receive emails. Plus, manipulate 3D and CAD files. Aspose.Total for Python via .NET handles a multitude of file formats, including Microsoft Word, PowerPoint, Outlook, OpenOffice, Web, Fixed Layout, Images, and 3D & CAD files. Make Next Generation document processing Apps now!
 
 This release includes the following:
 
-# [Aspose.3D for Python via .NET](https://releases.aspose.com/3d/python-net/) (v24.4.0)
+# [Aspose.3D for Python via .NET](https://releases.aspose.com/3d/python-net/) (v24.5.0)
 
 Unleash the power of Aspose.3D for Python via .NET, the ultimate Python 3D manipulation high code API. Effortlessly create, process, manipulate, and convert 3D scenes, meshes, and entities - no need for 3rd party software. Enjoy scene creation, animation, geometry, scene hierarchy, triangulate mesh, target camera, 3D plane, shadows, cylinders, conversion, import, and export capabilities. Grow your 3D projects with seamless integration and exceptional 3D control!
 
 ```python
-pip install aspose-3d==24.4.0
+pip install aspose-3d==24.5.0
 ```
 
-# [Aspose.BarCode for Python via .NET](https://releases.aspose.com/barcode/python-net/) (v24.4.0)
+# [Aspose.BarCode for Python via .NET](https://releases.aspose.com/barcode/python-net/) (v24.5.0)
 
 Aspose.BarCode for Python via .NET is a barcode generation and scanning library for .NET and Python developers. Create barcode images with precise control over size, captions, colors, and font. Generate QR, MicroQR, and Datamatrix barcodes with custom error correction and encoding. Support error correction and checksum for various symbologies. Adjust 2D barcode size and aspect ratio. Customize image border and style. Detect Unicode encoding, hide long codetext, or reduce font size. Colorize barcode, code text, background, border, and caption. Specify size unit in document, inch, millimeter, pixel, or point.
 
 ```python
-pip install aspose-barcode-for-python-via-net==24.4
+pip install aspose-barcode-for-python-via-net==24.5
 ```
 
-# [Aspose.CAD for Python via .NET](https://releases.aspose.com/cad/python-net/) (v24.3.0)
+# [Aspose.CAD for Python via .NET](https://releases.aspose.com/cad/python-net/) (v24.4.0)
 
 Aspose.CAD for Python via .NET is ultimate CAD and BIM drawing processing API for .NET and Python developers. Enhance your apps with high-quality conversion and rendering of DWG, DWF, DWFX, DGN, STL, OBJ, CF2, IGES, IFC, DXF, and more formats to PDF and images. No need for AutoCAD&reg; or rendering workflows. Manipulate drawing entities and blocks, select specific layouts and layers, and adjust drawing size before rendering. Exciting new features in Version 23.6 include support for OBJ file format export, HoloLens 2, and AutoCAD Plotter Configuration (PC3) files.
 
 ```python
-pip install aspose-cad==24.3.0
+pip install aspose-cad==24.4
 ```
 
-# [Aspose.Cells for Python via .NET](https://releases.aspose.com/cells/python-net/) (v24.4.0)
+# [Aspose.Cells for Python via .NET](https://releases.aspose.com/cells/python-net/) (v24.5.0)
 
 Experience the full potential of Aspose.Cells for Python via .NET, our Excel&reg; file handling solution for .NET and Python developers. Create, manipulate, and save Excel&reg; files with ease. Benefit from high-quality format conversion, rendering, and printing capabilities. Effortlessly customize charts, Pivot Tables, and apply advanced formatting. Protect, merge, and parse Excel&reg; sheets seamlessly. Convert charts to images and PDFs while supporting various file formats. Take advantage of the formula calculation engine with support for all Excel functions.
 
 ```python
-pip install aspose-cells-python==24.4.0
+pip install aspose-cells-python==24.5.0
 ```
 
-# [Aspose.Diagram for Python via .NET](https://releases.aspose.com/diagram/python-net/) (v24.4.0)
+# [Aspose.Diagram for Python via .NET](https://releases.aspose.com/diagram/python-net/) (v24.5.0)
 
 Improve Visio&reg; file processing with Aspose.Diagram for Python via .NET. Seamlessly create, manipulate, and convert Visio&reg; files, all without Microsoft Office&reg; dependencies. Enjoy features like shape conversion, comment management, and versatile format inter-conversion. Elevate your Python development workflow now!
 
 ```python
-pip install aspose-diagram-python==24.4
+pip install aspose-diagram-python==24.5
 ```
 
-# [Aspose.Email for Python via .NET](https://releases.aspose.com/email/pythonnet/) (v24.4.0)
+# [Aspose.Email for Python via .NET](https://releases.aspose.com/email/pythonnet/) (v24.5.0)
 
 Boost your Python applications with Aspose.Email for Python via .NET, an on-premise API designed to streamline email handling. Send & receive emails with attachments, perform email rendering and format conversions, and download messages from POP3 and IMAP servers. Seamlessly send iCalendar compliant appointments or meetings and work with message storage files. SSL & TLS support included. Uplift your email capabilities now!
 
 ```python
-pip install Aspose.Email-for-Python-via-NET==24.4
+pip install Aspose.Email-for-Python-via-NET==24.5
 ```
 
-# [Aspose.Finance for Python via .NET](https://releases.aspose.com/finance/python-net/) (v24.3.0)
+# [Aspose.Finance for Python via .NET](https://releases.aspose.com/finance/python-net/) (v24.4.0)
 
 Aspose.Finance for Python via .NET is a powerful API for processing finance-related formats like XBRL, iXBRL, and OFX using Python. It allows creation, manipulation, and conversion of XBRL, iXBRL, and OFX files, providing a comprehensive solution for developers. With features like XBRL and iXBRL creation, format conversion, validation, and more, Aspose.Finance streamlines financial data handling with ease and efficiency.
 
 ```python
-pip install aspose-finance==24.3
+pip install aspose-finance==24.4
 ```
 
-# [Aspose.Imaging for Python via .NET](https://releases.aspose.com/imaging/python-net/) (v24.4.0)
+# [Aspose.Imaging for Python via .NET](https://releases.aspose.com/imaging/python-net/) (v24.5.0)
 
 Aspose.Imaging for Python via .NET is an advanced image processing library. Easily create, load, manipulate, convert, compress images. Supports drawing and graphic primitives. Core features include; image export & conversion, transformations (resize, crop, flip &rotate, etc.), filtering, memory optimization. Handles popular formats like DjVu, DICOM, WebP & DNG, and extends .NET & .NET Core support. Cross-platform; Windows & Linux compatible. Explore powerful features now: create, read, write, draw, process & convert images effortlessly with Aspose.Imaging!
 
 ```python
-pip install aspose-imaging-python-net==24.4.0
+pip install aspose-imaging-python-net==24.5.0
 ```
 
-# [Aspose.OCR for Python via .NET](https://releases.aspose.com/ocr/python-net/) (v24.3.0)
+# [Aspose.OCR for Python via .NET](https://releases.aspose.com/ocr/python-net/) (v24.5.0)
 
 Aspose.OCR for Python via .NET is an easy-to-use OCR engine for Python Apps. Recognize text in 28 languages, Latin, Cyrillic & Asian scripts. Extract text from scans, photos, PDFs. Handle blurry, distorted, rotated, noisy images. Preserve original layout, detect paragraphs, lines, single words. Bulk process multipage docs, folders, archives. Identify misspelled words, compare image texts. Simplify OCR tasks with Aspose.OCR!
 
 ```python
-pip install aspose-ocr-python-net==24.3.0
+pip install aspose-ocr-python-net==24.5.0
 ```
 
 # [Aspose.Page for Python via .NET](https://releases.aspose.com/page/python-net/) (v24.2.0)
 
 Aspose.Page for Python via .NET empowers developers to work with PS, EPS, and XPS formats seamlessly, eliminating the need for Microsoft Office or Adobe products entirely. Streamline your document processing workflows today! Effortlessly integrate this lightweight library into your Python projects using pip.
 
 ```python
 pip install aspose-page==24.2.0
 ```
 
-# [Aspose.PDF for Python via .NET](https://releases.aspose.com/pdf/pythonnet/) (v24.4.0)
+# [Aspose.PDF for Python via .NET](https://releases.aspose.com/pdf/pythonnet/) (v24.5.0)
 
 Aspose.PDF for Python via .NET is a powerful native library for PDF processing in your applications. Generate, read, convert, and manipulate PDF files without Adobe Acrobat&reg;. Perform form processing, metadata handling, text and page manipulation, annotations management, bookmarks and watermarks, attachments, custom font handling, and more. Supercharge your PDF capabilities via API!
 
 ```python
-pip install aspose-pdf==24.4.0
+pip install aspose-pdf==24.5.0
 ```
 
-# [Aspose.PSD for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.2.0)
+# [Aspose.PSD for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.4.0)
 
 Aspose.PSD for Python simplifies handling of PSD, PSB, and AI files. It allows creation, editing, conversion, and export to various formats while supporting advanced features like layer manipulation, effects, and drawing tools. This cross-platform library caters to diverse use cases with robust functionality.
 
 ```python
-pip install aspose-psd==24.2.0
+pip install aspose-psd==24.4.0
 ```
 
-# [Aspose.Slides for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.4.0)
+# [Aspose.Slides for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.5.0)
 
 Level up your Python programs with Aspose.Slides for Python via .NET - the ultimate Python class library for PowerPoint&reg; & OpenOffice&reg; presentations. No need to install Microsoft PowerPoint&reg; or any 3rd party software. Effortlessly create, clone, and manipulate slides from templates. Master slides, animations, charts, shapes, OLE, VBA Macros, video frames, picture frames, audio frames, encryption, and decryption - all at your fingertips. Elevate your presentation game now!
 
 ```python
-pip install Aspose.Slides==24.4.0
+pip install Aspose.Slides==24.5.0
 ```
 
-# [Aspose.Tasks for Python via .NET](https://releases.aspose.com/tasks/python-net/) (v24.4.0)
+# [Aspose.SVG for Python via .NET](https://releases.aspose.com/svg/python-net/) (v24.5.0)
+
+Aspose.SVG for Python via .NET is a versatile on-premise class library designed to handle a variety of tasks involving SVG files without the need for additional SVG tools. It enables you to create, edit, optimize, and convert SVG files. The Python API allows for document and element manipulation, providing advanced navigation and inspection features such as XPath queries and CSS selectors. Developers can also vectorize images and texts, apply SVG transformations, filters, gradients, and patterns, and specify colors in various formats. Aspose.SVG for Python via .NET is ideal for creating applications like SVG editors, converters, mergers, and image vectorizers, offering comprehensive SVG processing capabilities for developers.
+
+```python
+pip install aspose-svg-net==24.5.0
+```
+
+# [Aspose.Tasks for Python via .NET](https://releases.aspose.com/tasks/python-net/) (v24.5.0)
 
 Aspose.Tasks for Python via .NET, a powerful native library for adding MS-Project file processing capabilities to your applications. Easily create, read, convert, and manipulate MS-Project files without Microsoft Project&reg; itself. Perform calculations, manage tasks, resources, and calendars, manipulate views, and handle attachments effortlessly. Enjoy features like export to various image formats, XLSX, HTML, CSV, and PDF, along with support for Oracle Primavera&reg; and Project Server. Supported MS-Project versions include 2003 to 2021. Convert MPP to images, Excel, HTML, CSV, and PDF with ease. Manage tasks, resources, assignments, and customize Gantt Chart view styles.
 
 ```python
-pip install aspose-tasks==24.4.0
+pip install aspose-tasks==24.5.0
 ```
 
 # [Aspose.TeX for Python via .NET](https://releases.aspose.com/tex/python-net/) (v24.3.0)
 
 Streamline your document creation process with Aspose.TeX for Python via .NET, the powerful TeX/LaTeX processing library for developers Effortlessly typeset complex documents in various TeX and LaTeX formats, without relying on external software. Get started quickly by integrating Aspose.TeX into your Python projects using pip.
 
 ```python
 pip install aspose-tex-net==24.3.0
 ```
 
-# [Aspose.Words for Python via .NET](https://releases.aspose.com/words/python/) (v24.4.0)
+# [Aspose.Words for Python via .NET](https://releases.aspose.com/words/python/) (v24.5.0)
 
 Empower your Python applications with Aspose.Words for Python via .NET, an on-premise API for seamless Microsoft Word&reg; document handling. Create, edit, render, and convert Word&reg; files to various formats (PDF, XPS, Raster Image, PCL, EPUB, etc.) effortlessly. Enjoy report generation, data visualization, and a range of document tasks like viewing, merging, splitting, translating, watermarking, and comparison. Level up your document processing now!
 
 ```python
-pip install aspose-words==24.4.0
+pip install aspose-words==24.5.0
 ```
 
-# [Aspose.ZIP for Python via .NET](https://releases.aspose.com/zip/python-net/) (v24.4.0)
+# [Aspose.ZIP for Python via .NET](https://releases.aspose.com/zip/python-net/) (v24.5.0)
 
 Aspose.ZIP for Python via .NET is a powerful Python API to create, manipulate, extract & protect archive formats - ZIP, BZIP, BZ2 & TAR. Simplify compression/decompression in your Python apps without complex coding. Offers a wide range of features, including archive creation, extraction, encryption (password, AES), and compressing single/multiple files and directories. Secure your files with password or AES encryption. Explore advanced options like appending files to existing archives, Gzip/Bzip2 packing into TAR archives, and creating self-extracting compressed archives.
 
 ```python
-pip install aspose-zip==24.4.0
+pip install aspose-zip==24.5.0
 ```
 
 [Product Page](https://products.aspose.com/total/python-net) | [Docs](https://docs.aspose.com/total/pythonnet/) | [Demos](https://products.aspose.app/total/family) | [Examples](https://aspose.github.io/) | [Download](https://downloads.aspose.com/total/pythonnet) | [Blog](https://blog.aspose.com/category/total/) | [Releases](https://releases.aspose.com/) | [Free Support](https://forum.aspose.com/c/total/7) | [Temporary License](https://purchase.aspose.com/temporary-license)
```

### Comparing `aspose_total_net-24.4.0/aspose_total_net.egg-info/PKG-INFO` & `aspose_total_net-24.5.0/aspose_total_net.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,178 +1,187 @@
 Metadata-Version: 2.1
 Name: aspose-total-net
-Version: 24.4.0
+Version: 24.5.0
 Summary: Aspose.Total for Python via .NET is a Document Processing python class library that allows developers to work with Microsoft Word®, Microsoft PowerPoint®, Microsoft Outlook®, OpenOffice®, & 3D file formats without needing Office Automation.
 Home-page: https://products.aspose.com/total/python-net
 Author: Aspose
 Author-email: total@aspose.com
 Keywords: DOC,DOCX,RTF,DOT,DOTX,DOTM,DOCM FlatOPC,FlatOpcMacroEnabled,FlatOpcTemplate,FlatOpcTemplateMacroEnabled,ODT,OTT,WordML,HTML,MHTML,PDF,MOBI,TXT,PDF/A,XPS,OpenXPS,PostScript (PS),TIFF,JPEG,PNG,BMP,SVG,EMF,GIF,HtmlFixed,PCL,EPUB,XamlFixed,XamlFlow,XamlFlowPack,MSG,PST,OST,OFT,EML,EMLX,MBOX,ICS,VCF,OLM,PPT,PPTX,PPS,POT,PPSX,PPTM,PPSM,POTX,POTM,ODP,FBX,STL,OBJ,3DS,U3D,DAE,glTF,ASCII,Binary,DRC,RVM,AMF,PLY,A3DW,X,DirectX,JT,DXF,3MF,ASE,VRML,Create,Clone,Render,Compare,Join,Split,Encrypt,Digital Signature,Mail Merge,Reporting,Watermark,LINQ,Reporting Engine,Editor,Merger,Viewer,Conversion,Splitter,OCR,Translator,Compress,SSL,TLS,TNEF,Email Attachment,Email,POP3,IMAP,iCalendar,OleObject,Chart,3D,Scene,Triangulate,Vulkan,Geometry,Camera,Mesh,Shape
 Platform: Operating System :: MacOS :: MacOS X
 Platform: Operating System :: Microsoft :: Windows :: Windows 7
 Platform: Operating System :: Microsoft :: Windows :: Windows Vista
 Platform: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: license.txt
-Requires-Dist: aspose-3d==24.4.0
-Requires-Dist: aspose-barcode-for-python-via-net==24.4
-Requires-Dist: aspose-cad==24.3.0
-Requires-Dist: aspose-cells-python==24.4.0
-Requires-Dist: aspose-diagram-python==24.4
-Requires-Dist: Aspose.Email-for-Python-via-NET==24.4
-Requires-Dist: aspose-finance==24.3
-Requires-Dist: aspose-imaging-python-net==24.4.0
-Requires-Dist: aspose-ocr-python-net==24.3.0
+Requires-Dist: aspose-3d==24.5.0
+Requires-Dist: aspose-barcode-for-python-via-net==24.5
+Requires-Dist: aspose-cad==24.4
+Requires-Dist: aspose-cells-python==24.5.0
+Requires-Dist: aspose-diagram-python==24.5
+Requires-Dist: Aspose.Email-for-Python-via-NET==24.5
+Requires-Dist: aspose-finance==24.4
+Requires-Dist: aspose-imaging-python-net==24.5.0
+Requires-Dist: aspose-ocr-python-net==24.5.0
 Requires-Dist: aspose-page==24.2.0
-Requires-Dist: aspose-pdf==24.4.0
-Requires-Dist: aspose-psd==24.2.0
-Requires-Dist: Aspose.Slides==24.4.0
-Requires-Dist: aspose-tasks==24.4.0
+Requires-Dist: aspose-pdf==24.5.0
+Requires-Dist: aspose-psd==24.4.0
+Requires-Dist: Aspose.Slides==24.5.0
+Requires-Dist: aspose-svg-net==24.5.0
+Requires-Dist: aspose-tasks==24.5.0
 Requires-Dist: aspose-tex-net==24.3.0
-Requires-Dist: aspose-words==24.4.0
-Requires-Dist: aspose-zip==24.4.0
+Requires-Dist: aspose-words==24.5.0
+Requires-Dist: aspose-zip==24.5.0
 
 [Product Page](https://products.aspose.com/total/python-net) | [Docs](https://docs.aspose.com/total/pythonnet/) | [Demos](https://products.aspose.app/total/family) | [Examples](https://aspose.github.io/) | [Download](https://downloads.aspose.com/total/pythonnet) | [Blog](https://blog.aspose.com/category/total/) | [Releases](https://releases.aspose.com/) | [Free Support](https://forum.aspose.com/c/total/7) | [Temporary License](https://purchase.aspose.com/temporary-license)
 
 Aspose.Total for Python via .NET is a collection of powerful yet easy-to-use document processing libraries for Python developers. Create, edit, convert DOC, DOCX, XLSX, XLS, CSV, PPT, PPTX, EML, MSG, 3D, and more formats within Python apps. Render PDF and images with high fidelity, compare documents, protect or encrypt, mail merge, clone slides, work with PowerPoint tables, generate presentations from the database, create custom charts, handle email formats, TNEF attachments, and send/receive emails. Plus, manipulate 3D and CAD files. Aspose.Total for Python via .NET handles a multitude of file formats, including Microsoft Word, PowerPoint, Outlook, OpenOffice, Web, Fixed Layout, Images, and 3D & CAD files. Make Next Generation document processing Apps now!
 
 This release includes the following:
 
-# [Aspose.3D for Python via .NET](https://releases.aspose.com/3d/python-net/) (v24.4.0)
+# [Aspose.3D for Python via .NET](https://releases.aspose.com/3d/python-net/) (v24.5.0)
 
 Unleash the power of Aspose.3D for Python via .NET, the ultimate Python 3D manipulation high code API. Effortlessly create, process, manipulate, and convert 3D scenes, meshes, and entities - no need for 3rd party software. Enjoy scene creation, animation, geometry, scene hierarchy, triangulate mesh, target camera, 3D plane, shadows, cylinders, conversion, import, and export capabilities. Grow your 3D projects with seamless integration and exceptional 3D control!
 
 ```python
-pip install aspose-3d==24.4.0
+pip install aspose-3d==24.5.0
 ```
 
-# [Aspose.BarCode for Python via .NET](https://releases.aspose.com/barcode/python-net/) (v24.4.0)
+# [Aspose.BarCode for Python via .NET](https://releases.aspose.com/barcode/python-net/) (v24.5.0)
 
 Aspose.BarCode for Python via .NET is a barcode generation and scanning library for .NET and Python developers. Create barcode images with precise control over size, captions, colors, and font. Generate QR, MicroQR, and Datamatrix barcodes with custom error correction and encoding. Support error correction and checksum for various symbologies. Adjust 2D barcode size and aspect ratio. Customize image border and style. Detect Unicode encoding, hide long codetext, or reduce font size. Colorize barcode, code text, background, border, and caption. Specify size unit in document, inch, millimeter, pixel, or point.
 
 ```python
-pip install aspose-barcode-for-python-via-net==24.4
+pip install aspose-barcode-for-python-via-net==24.5
 ```
 
-# [Aspose.CAD for Python via .NET](https://releases.aspose.com/cad/python-net/) (v24.3.0)
+# [Aspose.CAD for Python via .NET](https://releases.aspose.com/cad/python-net/) (v24.4.0)
 
 Aspose.CAD for Python via .NET is ultimate CAD and BIM drawing processing API for .NET and Python developers. Enhance your apps with high-quality conversion and rendering of DWG, DWF, DWFX, DGN, STL, OBJ, CF2, IGES, IFC, DXF, and more formats to PDF and images. No need for AutoCAD&reg; or rendering workflows. Manipulate drawing entities and blocks, select specific layouts and layers, and adjust drawing size before rendering. Exciting new features in Version 23.6 include support for OBJ file format export, HoloLens 2, and AutoCAD Plotter Configuration (PC3) files.
 
 ```python
-pip install aspose-cad==24.3.0
+pip install aspose-cad==24.4
 ```
 
-# [Aspose.Cells for Python via .NET](https://releases.aspose.com/cells/python-net/) (v24.4.0)
+# [Aspose.Cells for Python via .NET](https://releases.aspose.com/cells/python-net/) (v24.5.0)
 
 Experience the full potential of Aspose.Cells for Python via .NET, our Excel&reg; file handling solution for .NET and Python developers. Create, manipulate, and save Excel&reg; files with ease. Benefit from high-quality format conversion, rendering, and printing capabilities. Effortlessly customize charts, Pivot Tables, and apply advanced formatting. Protect, merge, and parse Excel&reg; sheets seamlessly. Convert charts to images and PDFs while supporting various file formats. Take advantage of the formula calculation engine with support for all Excel functions.
 
 ```python
-pip install aspose-cells-python==24.4.0
+pip install aspose-cells-python==24.5.0
 ```
 
-# [Aspose.Diagram for Python via .NET](https://releases.aspose.com/diagram/python-net/) (v24.4.0)
+# [Aspose.Diagram for Python via .NET](https://releases.aspose.com/diagram/python-net/) (v24.5.0)
 
 Improve Visio&reg; file processing with Aspose.Diagram for Python via .NET. Seamlessly create, manipulate, and convert Visio&reg; files, all without Microsoft Office&reg; dependencies. Enjoy features like shape conversion, comment management, and versatile format inter-conversion. Elevate your Python development workflow now!
 
 ```python
-pip install aspose-diagram-python==24.4
+pip install aspose-diagram-python==24.5
 ```
 
-# [Aspose.Email for Python via .NET](https://releases.aspose.com/email/pythonnet/) (v24.4.0)
+# [Aspose.Email for Python via .NET](https://releases.aspose.com/email/pythonnet/) (v24.5.0)
 
 Boost your Python applications with Aspose.Email for Python via .NET, an on-premise API designed to streamline email handling. Send & receive emails with attachments, perform email rendering and format conversions, and download messages from POP3 and IMAP servers. Seamlessly send iCalendar compliant appointments or meetings and work with message storage files. SSL & TLS support included. Uplift your email capabilities now!
 
 ```python
-pip install Aspose.Email-for-Python-via-NET==24.4
+pip install Aspose.Email-for-Python-via-NET==24.5
 ```
 
-# [Aspose.Finance for Python via .NET](https://releases.aspose.com/finance/python-net/) (v24.3.0)
+# [Aspose.Finance for Python via .NET](https://releases.aspose.com/finance/python-net/) (v24.4.0)
 
 Aspose.Finance for Python via .NET is a powerful API for processing finance-related formats like XBRL, iXBRL, and OFX using Python. It allows creation, manipulation, and conversion of XBRL, iXBRL, and OFX files, providing a comprehensive solution for developers. With features like XBRL and iXBRL creation, format conversion, validation, and more, Aspose.Finance streamlines financial data handling with ease and efficiency.
 
 ```python
-pip install aspose-finance==24.3
+pip install aspose-finance==24.4
 ```
 
-# [Aspose.Imaging for Python via .NET](https://releases.aspose.com/imaging/python-net/) (v24.4.0)
+# [Aspose.Imaging for Python via .NET](https://releases.aspose.com/imaging/python-net/) (v24.5.0)
 
 Aspose.Imaging for Python via .NET is an advanced image processing library. Easily create, load, manipulate, convert, compress images. Supports drawing and graphic primitives. Core features include; image export & conversion, transformations (resize, crop, flip &rotate, etc.), filtering, memory optimization. Handles popular formats like DjVu, DICOM, WebP & DNG, and extends .NET & .NET Core support. Cross-platform; Windows & Linux compatible. Explore powerful features now: create, read, write, draw, process & convert images effortlessly with Aspose.Imaging!
 
 ```python
-pip install aspose-imaging-python-net==24.4.0
+pip install aspose-imaging-python-net==24.5.0
 ```
 
-# [Aspose.OCR for Python via .NET](https://releases.aspose.com/ocr/python-net/) (v24.3.0)
+# [Aspose.OCR for Python via .NET](https://releases.aspose.com/ocr/python-net/) (v24.5.0)
 
 Aspose.OCR for Python via .NET is an easy-to-use OCR engine for Python Apps. Recognize text in 28 languages, Latin, Cyrillic & Asian scripts. Extract text from scans, photos, PDFs. Handle blurry, distorted, rotated, noisy images. Preserve original layout, detect paragraphs, lines, single words. Bulk process multipage docs, folders, archives. Identify misspelled words, compare image texts. Simplify OCR tasks with Aspose.OCR!
 
 ```python
-pip install aspose-ocr-python-net==24.3.0
+pip install aspose-ocr-python-net==24.5.0
 ```
 
 # [Aspose.Page for Python via .NET](https://releases.aspose.com/page/python-net/) (v24.2.0)
 
 Aspose.Page for Python via .NET empowers developers to work with PS, EPS, and XPS formats seamlessly, eliminating the need for Microsoft Office or Adobe products entirely. Streamline your document processing workflows today! Effortlessly integrate this lightweight library into your Python projects using pip.
 
 ```python
 pip install aspose-page==24.2.0
 ```
 
-# [Aspose.PDF for Python via .NET](https://releases.aspose.com/pdf/pythonnet/) (v24.4.0)
+# [Aspose.PDF for Python via .NET](https://releases.aspose.com/pdf/pythonnet/) (v24.5.0)
 
 Aspose.PDF for Python via .NET is a powerful native library for PDF processing in your applications. Generate, read, convert, and manipulate PDF files without Adobe Acrobat&reg;. Perform form processing, metadata handling, text and page manipulation, annotations management, bookmarks and watermarks, attachments, custom font handling, and more. Supercharge your PDF capabilities via API!
 
 ```python
-pip install aspose-pdf==24.4.0
+pip install aspose-pdf==24.5.0
 ```
 
-# [Aspose.PSD for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.2.0)
+# [Aspose.PSD for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.4.0)
 
 Aspose.PSD for Python simplifies handling of PSD, PSB, and AI files. It allows creation, editing, conversion, and export to various formats while supporting advanced features like layer manipulation, effects, and drawing tools. This cross-platform library caters to diverse use cases with robust functionality.
 
 ```python
-pip install aspose-psd==24.2.0
+pip install aspose-psd==24.4.0
 ```
 
-# [Aspose.Slides for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.4.0)
+# [Aspose.Slides for Python via .NET](https://releases.aspose.com/slides/python-net/) (v24.5.0)
 
 Level up your Python programs with Aspose.Slides for Python via .NET - the ultimate Python class library for PowerPoint&reg; & OpenOffice&reg; presentations. No need to install Microsoft PowerPoint&reg; or any 3rd party software. Effortlessly create, clone, and manipulate slides from templates. Master slides, animations, charts, shapes, OLE, VBA Macros, video frames, picture frames, audio frames, encryption, and decryption - all at your fingertips. Elevate your presentation game now!
 
 ```python
-pip install Aspose.Slides==24.4.0
+pip install Aspose.Slides==24.5.0
 ```
 
-# [Aspose.Tasks for Python via .NET](https://releases.aspose.com/tasks/python-net/) (v24.4.0)
+# [Aspose.SVG for Python via .NET](https://releases.aspose.com/svg/python-net/) (v24.5.0)
+
+Aspose.SVG for Python via .NET is a versatile on-premise class library designed to handle a variety of tasks involving SVG files without the need for additional SVG tools. It enables you to create, edit, optimize, and convert SVG files. The Python API allows for document and element manipulation, providing advanced navigation and inspection features such as XPath queries and CSS selectors. Developers can also vectorize images and texts, apply SVG transformations, filters, gradients, and patterns, and specify colors in various formats. Aspose.SVG for Python via .NET is ideal for creating applications like SVG editors, converters, mergers, and image vectorizers, offering comprehensive SVG processing capabilities for developers.
+
+```python
+pip install aspose-svg-net==24.5.0
+```
+
+# [Aspose.Tasks for Python via .NET](https://releases.aspose.com/tasks/python-net/) (v24.5.0)
 
 Aspose.Tasks for Python via .NET, a powerful native library for adding MS-Project file processing capabilities to your applications. Easily create, read, convert, and manipulate MS-Project files without Microsoft Project&reg; itself. Perform calculations, manage tasks, resources, and calendars, manipulate views, and handle attachments effortlessly. Enjoy features like export to various image formats, XLSX, HTML, CSV, and PDF, along with support for Oracle Primavera&reg; and Project Server. Supported MS-Project versions include 2003 to 2021. Convert MPP to images, Excel, HTML, CSV, and PDF with ease. Manage tasks, resources, assignments, and customize Gantt Chart view styles.
 
 ```python
-pip install aspose-tasks==24.4.0
+pip install aspose-tasks==24.5.0
 ```
 
 # [Aspose.TeX for Python via .NET](https://releases.aspose.com/tex/python-net/) (v24.3.0)
 
 Streamline your document creation process with Aspose.TeX for Python via .NET, the powerful TeX/LaTeX processing library for developers Effortlessly typeset complex documents in various TeX and LaTeX formats, without relying on external software. Get started quickly by integrating Aspose.TeX into your Python projects using pip.
 
 ```python
 pip install aspose-tex-net==24.3.0
 ```
 
-# [Aspose.Words for Python via .NET](https://releases.aspose.com/words/python/) (v24.4.0)
+# [Aspose.Words for Python via .NET](https://releases.aspose.com/words/python/) (v24.5.0)
 
 Empower your Python applications with Aspose.Words for Python via .NET, an on-premise API for seamless Microsoft Word&reg; document handling. Create, edit, render, and convert Word&reg; files to various formats (PDF, XPS, Raster Image, PCL, EPUB, etc.) effortlessly. Enjoy report generation, data visualization, and a range of document tasks like viewing, merging, splitting, translating, watermarking, and comparison. Level up your document processing now!
 
 ```python
-pip install aspose-words==24.4.0
+pip install aspose-words==24.5.0
 ```
 
-# [Aspose.ZIP for Python via .NET](https://releases.aspose.com/zip/python-net/) (v24.4.0)
+# [Aspose.ZIP for Python via .NET](https://releases.aspose.com/zip/python-net/) (v24.5.0)
 
 Aspose.ZIP for Python via .NET is a powerful Python API to create, manipulate, extract & protect archive formats - ZIP, BZIP, BZ2 & TAR. Simplify compression/decompression in your Python apps without complex coding. Offers a wide range of features, including archive creation, extraction, encryption (password, AES), and compressing single/multiple files and directories. Secure your files with password or AES encryption. Explore advanced options like appending files to existing archives, Gzip/Bzip2 packing into TAR archives, and creating self-extracting compressed archives.
 
 ```python
-pip install aspose-zip==24.4.0
+pip install aspose-zip==24.5.0
 ```
 
 [Product Page](https://products.aspose.com/total/python-net) | [Docs](https://docs.aspose.com/total/pythonnet/) | [Demos](https://products.aspose.app/total/family) | [Examples](https://aspose.github.io/) | [Download](https://downloads.aspose.com/total/pythonnet) | [Blog](https://blog.aspose.com/category/total/) | [Releases](https://releases.aspose.com/) | [Free Support](https://forum.aspose.com/c/total/7) | [Temporary License](https://purchase.aspose.com/temporary-license)
```

### Comparing `aspose_total_net-24.4.0/setup.py` & `aspose_total_net-24.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup
 
 NAME = "aspose-total-net"
-VERSION = "24.4.0"
+VERSION = "24.5.0"
 
-REQUIRES = ["aspose-3d==24.4.0",
-            "aspose-barcode-for-python-via-net==24.4",
-            "aspose-cad==24.3.0",
-            "aspose-cells-python==24.4.0",
-            "aspose-diagram-python==24.4",
-            "Aspose.Email-for-Python-via-NET==24.4",
-            "aspose-finance==24.3",
-            "aspose-imaging-python-net==24.4.0",
-            "aspose-ocr-python-net==24.3.0",
+REQUIRES = ["aspose-3d==24.5.0",
+            "aspose-barcode-for-python-via-net==24.5",
+            "aspose-cad==24.4",
+            "aspose-cells-python==24.5.0",
+            "aspose-diagram-python==24.5",
+            "Aspose.Email-for-Python-via-NET==24.5",
+            "aspose-finance==24.4",
+            "aspose-imaging-python-net==24.5.0",
+            "aspose-ocr-python-net==24.5.0",
             "aspose-page==24.2.0",
-            "aspose-pdf==24.4.0",
-            "aspose-psd==24.2.0",
-            "Aspose.Slides==24.4.0",
-            "aspose-tasks==24.4.0",
+            "aspose-pdf==24.5.0",
+            "aspose-psd==24.4.0",
+            "Aspose.Slides==24.5.0",
+            "aspose-svg-net==24.5.0",
+            "aspose-tasks==24.5.0",
             "aspose-tex-net==24.3.0",
-            "aspose-words==24.4.0",
-            "aspose-zip==24.4.0"]
+            "aspose-words==24.5.0",
+            "aspose-zip==24.5.0"]
 
 """
 REQUIRES = [
             "aspose-finance"]
 """
 
 setup(
```

