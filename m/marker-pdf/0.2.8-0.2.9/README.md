# Comparing `tmp/marker_pdf-0.2.8.tar.gz` & `tmp/marker_pdf-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marker_pdf-0.2.8.tar", max compression
+gzip compressed data, was "marker_pdf-0.2.9.tar", max compression
```

## Comparing `marker_pdf-0.2.8.tar` & `marker_pdf-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35101 2024-05-18 04:28:38.027526 marker_pdf-0.2.8/LICENSE
--rw-r--r--   0        0        0    12609 2024-05-18 04:28:38.027526 marker_pdf-0.2.8/README.md
--rwxr-xr-x   0        0        0      638 2024-05-18 04:28:38.027526 marker_pdf-0.2.8/chunk_convert.py
--rwxr-xr-x   0        0        0     1151 2024-05-18 04:28:38.027526 marker_pdf-0.2.8/chunk_convert.sh
--rwxr-xr-x   0        0        0     4853 2024-05-18 04:28:38.027526 marker_pdf-0.2.8/convert.py
--rwxr-xr-x   0        0        0     1246 2024-05-18 04:28:38.031525 marker_pdf-0.2.8/convert_single.py
--rw-r--r--   0        0        0     1376 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/benchmark/scoring.py
--rw-r--r--   0        0        0      231 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/cleaners/bullets.py
--rw-r--r--   0        0        0     4457 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/cleaners/code.py
--rw-r--r--   0        0        0      950 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/cleaners/fontstyle.py
--rw-r--r--   0        0        0     2766 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/cleaners/headers.py
--rw-r--r--   0        0        0     2456 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/cleaners/headings.py
--rw-r--r--   0        0        0      248 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/cleaners/text.py
--rw-r--r--   0        0        0     5172 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/convert.py
--rw-r--r--   0        0        0     2450 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/debug/data.py
--rw-r--r--   0        0        0     7884 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/equations/equations.py
--rw-r--r--   0        0        0     1549 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/equations/inference.py
--rw-r--r--   0        0        0     2594 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/images/extract.py
--rw-r--r--   0        0        0      473 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/images/save.py
--rw-r--r--   0        0        0     1928 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/layout/layout.py
--rw-r--r--   0        0        0     2516 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/layout/order.py
--rw-r--r--   0        0        0      396 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/logger.py
--rw-r--r--   0        0        0     3121 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/models.py
--rw-r--r--   0        0        0      888 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/ocr/detection.py
--rw-r--r--   0        0        0     2468 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/ocr/heuristics.py
--rw-r--r--   0        0        0     1223 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/ocr/lang.py
--rw-r--r--   0        0        0     5742 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/ocr/recognition.py
--rw-r--r--   0        0        0     2180 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/ocr/tesseract.py
--rw-r--r--   0        0        0      258 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/ocr/utils.py
--rw-r--r--   0        0        0     1266 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/output.py
--rw-r--r--   0        0        0     3932 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/pdf/extract_text.py
--rw-r--r--   0        0        0      817 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/pdf/images.py
--rw-r--r--   0        0        0     2442 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/pdf/utils.py
--rw-r--r--   0        0        0     4134 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/postprocessors/editor.py
--rw-r--r--   0        0        0     7226 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/postprocessors/markdown.py
--rw-r--r--   0        0        0     4977 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/postprocessors/t5.py
--rw-r--r--   0        0        0     2849 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/schema/bbox.py
--rw-r--r--   0        0        0     3259 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/schema/block.py
--rw-r--r--   0        0        0      502 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/schema/merged.py
--rw-r--r--   0        0        0     1618 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/schema/page.py
--rw-r--r--   0        0        0     4238 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/settings.py
--rw-r--r--   0        0        0     3384 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/tables/cells.py
--rw-r--r--   0        0        0     7178 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/tables/table.py
--rw-r--r--   0        0        0     1128 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/tables/utils.py
--rw-r--r--   0        0        0      156 2024-05-18 04:28:38.039525 marker_pdf-0.2.8/marker/utils.py
--rw-r--r--   0        0        0     1270 2024-05-18 04:28:38.043525 marker_pdf-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    14231 1970-01-01 00:00:00.000000 marker_pdf-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35101 2024-05-23 23:24:42.138038 marker_pdf-0.2.9/LICENSE
+-rw-r--r--   0        0        0    12609 2024-05-23 23:24:42.138038 marker_pdf-0.2.9/README.md
+-rwxr-xr-x   0        0        0      638 2024-05-23 23:24:42.138038 marker_pdf-0.2.9/chunk_convert.py
+-rwxr-xr-x   0        0        0     1151 2024-05-23 23:24:42.138038 marker_pdf-0.2.9/chunk_convert.sh
+-rwxr-xr-x   0        0        0     4853 2024-05-23 23:24:42.138038 marker_pdf-0.2.9/convert.py
+-rwxr-xr-x   0        0        0     1246 2024-05-23 23:24:42.138038 marker_pdf-0.2.9/convert_single.py
+-rw-r--r--   0        0        0     1376 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/benchmark/scoring.py
+-rw-r--r--   0        0        0      231 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/cleaners/bullets.py
+-rw-r--r--   0        0        0     4457 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/cleaners/code.py
+-rw-r--r--   0        0        0      950 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/cleaners/fontstyle.py
+-rw-r--r--   0        0        0     2766 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/cleaners/headers.py
+-rw-r--r--   0        0        0     2456 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/cleaners/headings.py
+-rw-r--r--   0        0        0      248 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/cleaners/text.py
+-rw-r--r--   0        0        0     5187 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/convert.py
+-rw-r--r--   0        0        0     2450 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/debug/data.py
+-rw-r--r--   0        0        0     7884 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/equations/equations.py
+-rw-r--r--   0        0        0     1549 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/equations/inference.py
+-rw-r--r--   0        0        0     2594 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/images/extract.py
+-rw-r--r--   0        0        0      473 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/images/save.py
+-rw-r--r--   0        0        0     1928 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/layout/layout.py
+-rw-r--r--   0        0        0     2516 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/layout/order.py
+-rw-r--r--   0        0        0      396 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/logger.py
+-rw-r--r--   0        0        0     3121 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/models.py
+-rw-r--r--   0        0        0      888 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/ocr/detection.py
+-rw-r--r--   0        0        0     2468 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/ocr/heuristics.py
+-rw-r--r--   0        0        0     1223 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/ocr/lang.py
+-rw-r--r--   0        0        0     5861 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/ocr/recognition.py
+-rw-r--r--   0        0        0     2180 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/ocr/tesseract.py
+-rw-r--r--   0        0        0      258 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/ocr/utils.py
+-rw-r--r--   0        0        0     1266 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/output.py
+-rw-r--r--   0        0        0     3979 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/pdf/extract_text.py
+-rw-r--r--   0        0        0      817 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/pdf/images.py
+-rw-r--r--   0        0        0     2442 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/pdf/utils.py
+-rw-r--r--   0        0        0     4134 2024-05-23 23:24:42.146038 marker_pdf-0.2.9/marker/postprocessors/editor.py
+-rw-r--r--   0        0        0     7226 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/postprocessors/markdown.py
+-rw-r--r--   0        0        0     4977 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/postprocessors/t5.py
+-rw-r--r--   0        0        0     2849 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/schema/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/schema/block.py
+-rw-r--r--   0        0        0      502 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/schema/merged.py
+-rw-r--r--   0        0        0     1618 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/schema/page.py
+-rw-r--r--   0        0        0     4348 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/settings.py
+-rw-r--r--   0        0        0     3384 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/tables/cells.py
+-rw-r--r--   0        0        0     7178 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/tables/table.py
+-rw-r--r--   0        0        0     1128 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/tables/utils.py
+-rw-r--r--   0        0        0      156 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/marker/utils.py
+-rw-r--r--   0        0        0     1270 2024-05-23 23:24:42.150038 marker_pdf-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    14231 1970-01-01 00:00:00.000000 marker_pdf-0.2.9/PKG-INFO
```

### Comparing `marker_pdf-0.2.8/LICENSE` & `marker_pdf-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/README.md` & `marker_pdf-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/chunk_convert.py` & `marker_pdf-0.2.9/chunk_convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/chunk_convert.sh` & `marker_pdf-0.2.9/chunk_convert.sh`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/convert.py` & `marker_pdf-0.2.9/convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/convert_single.py` & `marker_pdf-0.2.9/convert_single.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/benchmark/scoring.py` & `marker_pdf-0.2.9/marker/benchmark/scoring.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/cleaners/code.py` & `marker_pdf-0.2.9/marker/cleaners/code.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/cleaners/fontstyle.py` & `marker_pdf-0.2.9/marker/cleaners/fontstyle.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/cleaners/headers.py` & `marker_pdf-0.2.9/marker/cleaners/headers.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/cleaners/headings.py` & `marker_pdf-0.2.9/marker/cleaners/headings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/convert.py` & `marker_pdf-0.2.9/marker/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     if filetype == "other": # We can't process this file
         return "", {}, out_meta
 
     # Get initial text blocks from the pdf
     doc = pdfium.PdfDocument(fname)
     pages, toc = get_text_blocks(
         doc,
+        fname,
         max_pages=max_pages,
     )
     out_meta.update({
         "toc": toc,
         "pages": len(pages),
     })
```

### Comparing `marker_pdf-0.2.8/marker/debug/data.py` & `marker_pdf-0.2.9/marker/debug/data.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/equations/equations.py` & `marker_pdf-0.2.9/marker/equations/equations.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/equations/inference.py` & `marker_pdf-0.2.9/marker/equations/inference.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/images/extract.py` & `marker_pdf-0.2.9/marker/images/extract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/layout/layout.py` & `marker_pdf-0.2.9/marker/layout/layout.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/layout/order.py` & `marker_pdf-0.2.9/marker/layout/order.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/models.py` & `marker_pdf-0.2.9/marker/models.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/ocr/detection.py` & `marker_pdf-0.2.9/marker/ocr/detection.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/ocr/heuristics.py` & `marker_pdf-0.2.9/marker/ocr/heuristics.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/ocr/lang.py` & `marker_pdf-0.2.9/marker/ocr/lang.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/ocr/recognition.py` & `marker_pdf-0.2.9/marker/ocr/recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import tempfile
 from itertools import repeat
 from typing import List, Optional, Dict
 
 import pypdfium2 as pdfium
 import io
 from concurrent.futures import ThreadPoolExecutor
 
@@ -156,13 +157,16 @@
         optimize=False,
         fast_web_view=1e6,
         skip_big=15,  # skip images larger than 15 megapixels
         tesseract_timeout=settings.TESSERACT_TIMEOUT,
         tesseract_non_ocr_timeout=settings.TESSERACT_TIMEOUT,
     )
 
-    new_doc = pdfium.PdfDocument(out_pdf.getvalue())
+    with tempfile.NamedTemporaryFile() as f:
+        f.write(out_pdf.getvalue())
+        f.seek(0)
+        new_doc = pdfium.PdfDocument(f.name)
+        blocks, _ = get_text_blocks(new_doc, f.name, max_pages=1)
 
-    blocks, _ = get_text_blocks(new_doc, max_pages=1)
     page = blocks[0]
     page.ocr_method = "tesseract"
     return page
```

### Comparing `marker_pdf-0.2.8/marker/ocr/tesseract.py` & `marker_pdf-0.2.9/marker/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/output.py` & `marker_pdf-0.2.9/marker/output.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/pdf/extract_text.py` & `marker_pdf-0.2.9/marker/pdf/extract_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,23 +70,23 @@
         bbox=page_bbox,
         rotation=rotation,
         char_blocks=char_blocks
     )
     return out_page
 
 
-def get_text_blocks(doc, max_pages: Optional[int] = None) -> (List[Page], Dict):
+def get_text_blocks(doc, fname, max_pages: Optional[int] = None) -> (List[Page], Dict):
     toc = get_toc(doc)
 
     page_range = range(len(doc))
     if max_pages:
         range_end = min(max_pages, len(doc))
         page_range = range(range_end)
 
-    char_blocks = dictionary_output(doc, page_range=page_range, keep_chars=True)
+    char_blocks = dictionary_output(fname, page_range=page_range, keep_chars=True, workers=settings.PDFTEXT_CPU_WORKERS)
     marker_blocks = [pdftext_format_to_blocks(page, pnum) for pnum, page in enumerate(char_blocks)]
 
     return marker_blocks, toc
 
 
 def naive_get_text(doc):
     full_text = ""
```

### Comparing `marker_pdf-0.2.8/marker/pdf/images.py` & `marker_pdf-0.2.9/marker/pdf/images.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/pdf/utils.py` & `marker_pdf-0.2.9/marker/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/postprocessors/editor.py` & `marker_pdf-0.2.9/marker/postprocessors/editor.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/postprocessors/markdown.py` & `marker_pdf-0.2.9/marker/postprocessors/markdown.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/postprocessors/t5.py` & `marker_pdf-0.2.9/marker/postprocessors/t5.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/schema/bbox.py` & `marker_pdf-0.2.9/marker/schema/bbox.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/schema/block.py` & `marker_pdf-0.2.9/marker/schema/block.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/schema/page.py` & `marker_pdf-0.2.9/marker/schema/page.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/settings.py` & `marker_pdf-0.2.9/marker/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     VRAM_PER_TASK: float = 4.5 # How much VRAM to allocate per task (in GB).  Peak marker VRAM usage is around 5GB, but avg across workers is lower.
     DEFAULT_LANG: str = "English" # Default language we assume files to be in, should be one of the keys in TESSERACT_LANGUAGES
 
     SUPPORTED_FILETYPES: Dict = {
         "application/pdf": "pdf",
     }
 
+    # Text extraction
+    PDFTEXT_CPU_WORKERS: int = 4 # How many CPU workers to use for pdf text extraction
+
     # Text line Detection
     DETECTOR_BATCH_SIZE: Optional[int] = None # Defaults to 6 for CPU, 12 otherwise
     SURYA_DETECTOR_DPI: int = 96
     DETECTOR_POSTPROCESSING_CPU_WORKERS: int = 4
 
     # OCR
     INVALID_CHARS: List[str] = [chr(0xfffd), "�"]
```

### Comparing `marker_pdf-0.2.8/marker/tables/cells.py` & `marker_pdf-0.2.9/marker/tables/cells.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/tables/table.py` & `marker_pdf-0.2.9/marker/tables/table.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/marker/tables/utils.py` & `marker_pdf-0.2.9/marker/tables/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.8/pyproject.toml` & `marker_pdf-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marker-pdf"
-version = "0.2.8"
+version = "0.2.9"
 description = "Convert PDF to markdown with high speed and accuracy."
 authors = ["Vik Paruchuri <github@vikas.sh>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/marker"
 keywords = ["pdf", "markdown", "ocr", "nlp"]
 packages = [
@@ -29,18 +29,18 @@
 torch = "^2.2.2" # Issue with torch 2.3.0 and vision models - https://github.com/pytorch/pytorch/issues/121834
 ray = "^2.20.0"
 tqdm = "^4.66.1"
 tabulate = "^0.9.0"
 ftfy = "^6.1.1"
 texify = "^0.1.9"
 rapidfuzz = "^3.8.1"
-surya-ocr = "^0.4.7"
+surya-ocr = "^0.4.8"
 filetype = "^1.2.0"
 regex = "^2024.4.28"
-pdftext = "^0.3.7"
+pdftext = "^0.3.8"
 grpcio = "^1.63.0"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [tool.poetry.scripts]
 marker = "convert:main"
```

### Comparing `marker_pdf-0.2.8/PKG-INFO` & `marker_pdf-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marker-pdf
-Version: 0.2.8
+Version: 0.2.9
 Summary: Convert PDF to markdown with high speed and accuracy.
 Home-page: https://github.com/VikParuchuri/marker
 License: GPL-3.0-or-later
 Keywords: pdf,markdown,ocr,nlp
 Author: Vik Paruchuri
 Author-email: github@vikas.sh
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -15,23 +15,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=10.1.0,<11.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
 Requires-Dist: grpcio (>=1.63.0,<2.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
-Requires-Dist: pdftext (>=0.3.7,<0.4.0)
+Requires-Dist: pdftext (>=0.3.8,<0.4.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
 Requires-Dist: ray (>=2.20.0,<3.0.0)
 Requires-Dist: regex (>=2024.4.28,<2025.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
-Requires-Dist: surya-ocr (>=0.4.7,<0.5.0)
+Requires-Dist: surya-ocr (>=0.4.8,<0.5.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: texify (>=0.1.9,<0.2.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: transformers (>=4.36.2,<5.0.0)
 Project-URL: Repository, https://github.com/VikParuchuri/marker
 Description-Content-Type: text/markdown
```

