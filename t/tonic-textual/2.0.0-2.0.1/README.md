# Comparing `tmp/tonic_textual-2.0.0.tar.gz` & `tmp/tonic_textual-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_textual-2.0.0.tar", max compression
+gzip compressed data, was "tonic_textual-2.0.1.tar", max compression
```

## Comparing `tonic_textual-2.0.0.tar` & `tonic_textual-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-2.0.0/LICENSE
--rw-r--r--   0        0        0      979 2024-05-24 21:03:00.487683 tonic_textual-2.0.0/README.md
--rw-r--r--   0        0        0      598 2024-05-24 21:03:00.489256 tonic_textual-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-24 21:03:00.490079 tonic_textual-2.0.0/tonic_textual/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 21:40:23.410925 tonic_textual-2.0.0/tonic_textual/classes/__init__.py
--rw-r--r--   0        0        0      268 2024-05-24 21:03:00.490219 tonic_textual-2.0.0/tonic_textual/classes/api_responses/PaginationResponseModel
--rw-r--r--   0        0        0     1817 2024-05-24 21:03:00.490506 tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/base_file.py
--rw-r--r--   0        0        0     1224 2024-05-24 21:03:00.490739 tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/single_detection_result.py
--rw-r--r--   0        0        0      405 2024-05-24 21:03:00.491133 tonic_textual-2.0.0/tonic_textual/classes/custom_model.py
--rw-r--r--   0        0        0     9366 2024-05-24 21:03:00.491484 tonic_textual-2.0.0/tonic_textual/classes/dataset.py
--rw-r--r--   0        0        0     1836 2024-05-24 21:03:00.491817 tonic_textual-2.0.0/tonic_textual/classes/datasetfile.py
--rw-r--r--   0        0        0      130 2024-05-24 21:03:00.492019 tonic_textual-2.0.0/tonic_textual/classes/enums/docx_header_footer_type.py
--rw-r--r--   0        0        0      211 2024-05-24 21:03:00.492357 tonic_textual-2.0.0/tonic_textual/classes/enums/file_type.py
--rw-r--r--   0        0        0      263 2024-05-24 21:03:00.492503 tonic_textual-2.0.0/tonic_textual/classes/enums/pdf_content_type.py
--rw-r--r--   0        0        0      225 2024-05-24 21:03:00.492644 tonic_textual-2.0.0/tonic_textual/classes/enums/pdf_table_cell_type.py
--rw-r--r--   0        0        0      800 2024-05-24 21:03:00.492802 tonic_textual-2.0.0/tonic_textual/classes/file_content/base_document.py
--rw-r--r--   0        0        0     2014 2024-05-24 21:03:00.493027 tonic_textual-2.0.0/tonic_textual/classes/file_content/content.py
--rw-r--r--   0        0        0      587 2024-05-24 21:03:00.493272 tonic_textual-2.0.0/tonic_textual/classes/file_content/csv_document.py
--rw-r--r--   0        0        0     1037 2024-05-24 21:03:00.493457 tonic_textual-2.0.0/tonic_textual/classes/file_content/docx_document.py
--rw-r--r--   0        0        0     1489 2024-05-24 21:03:00.493714 tonic_textual-2.0.0/tonic_textual/classes/file_content/pdf_document.py
--rw-r--r--   0        0        0      385 2024-05-24 21:03:00.493923 tonic_textual-2.0.0/tonic_textual/classes/file_content/raw_document.py
--rw-r--r--   0        0        0      790 2024-05-24 21:03:00.494112 tonic_textual-2.0.0/tonic_textual/classes/file_content/xlsx_document.py
--rw-r--r--   0        0        0     2148 2024-05-24 23:05:01.047399 tonic_textual-2.0.0/tonic_textual/classes/file_parse_result_diff_enumerator.py
--rw-r--r--   0        0        0     5112 2024-05-24 22:11:30.124934 tonic_textual-2.0.0/tonic_textual/classes/httpclient.py
--rw-r--r--   0        0        0    10406 2024-05-24 23:05:01.047617 tonic_textual-2.0.0/tonic_textual/classes/parse_api_responses/file_parse_result.py
--rw-r--r--   0        0        0      514 2024-05-24 21:03:00.495403 tonic_textual-2.0.0/tonic_textual/classes/parse_api_responses/file_parse_results_diff.py
--rw-r--r--   0        0        0     2148 2024-05-24 21:03:00.495592 tonic_textual-2.0.0/tonic_textual/classes/pipeline.py
--rw-r--r--   0        0        0     1970 2024-05-24 21:03:00.495892 tonic_textual-2.0.0/tonic_textual/classes/pipeline_file_enumerator.py
--rw-r--r--   0        0        0      873 2024-05-24 21:03:00.496090 tonic_textual-2.0.0/tonic_textual/classes/pipeline_run.py
--rw-r--r--   0        0        0      947 2024-05-24 21:03:00.496385 tonic_textual-2.0.0/tonic_textual/classes/redact_api_responses/redaction_response.py
--rw-r--r--   0        0        0     2373 2024-05-24 23:05:01.047866 tonic_textual-2.0.0/tonic_textual/classes/tonic_exception.py
--rw-r--r--   0        0        0      123 2024-05-24 21:03:00.496930 tonic_textual-2.0.0/tonic_textual/enums/pii_state.py
--rw-r--r--   0        0        0      711 2024-05-24 21:03:00.497143 tonic_textual-2.0.0/tonic_textual/generator_utils.py
--rw-r--r--   0        0        0     2907 2024-05-24 21:03:00.497319 tonic_textual-2.0.0/tonic_textual/markdown_utils.py
--rw-r--r--   0        0        0     2234 2024-05-24 21:03:00.497439 tonic_textual-2.0.0/tonic_textual/parse_api.py
--rw-r--r--   0        0        0    19135 2024-05-24 21:03:00.497758 tonic_textual-2.0.0/tonic_textual/redact_api.py
--rw-r--r--   0        0        0        0 2024-05-20 21:40:23.412740 tonic_textual-2.0.0/tonic_textual/services/__init__.py
--rw-r--r--   0        0        0      639 2024-05-24 21:03:00.498153 tonic_textual-2.0.0/tonic_textual/services/dataset.py
--rw-r--r--   0        0        0      771 2024-05-24 21:03:00.498415 tonic_textual-2.0.0/tonic_textual/services/datasetfile.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 tonic_textual-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-2.0.1/LICENSE
+-rw-r--r--   0        0        0      979 2024-05-24 21:03:00.487683 tonic_textual-2.0.1/README.md
+-rw-r--r--   0        0        0      598 2024-05-29 04:05:49.410813 tonic_textual-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-29 04:05:49.411206 tonic_textual-2.0.1/tonic_textual/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:40:23.410925 tonic_textual-2.0.1/tonic_textual/classes/__init__.py
+-rw-r--r--   0        0        0      268 2024-05-24 21:03:00.490219 tonic_textual-2.0.1/tonic_textual/classes/api_responses/PaginationResponseModel
+-rw-r--r--   0        0        0     1817 2024-05-24 21:03:00.490506 tonic_textual-2.0.1/tonic_textual/classes/common_api_responses/base_file.py
+-rw-r--r--   0        0        0     1224 2024-05-24 21:03:00.490739 tonic_textual-2.0.1/tonic_textual/classes/common_api_responses/single_detection_result.py
+-rw-r--r--   0        0        0      405 2024-05-24 21:03:00.491133 tonic_textual-2.0.1/tonic_textual/classes/custom_model.py
+-rw-r--r--   0        0        0     9366 2024-05-24 21:03:00.491484 tonic_textual-2.0.1/tonic_textual/classes/dataset.py
+-rw-r--r--   0        0        0     1836 2024-05-24 21:03:00.491817 tonic_textual-2.0.1/tonic_textual/classes/datasetfile.py
+-rw-r--r--   0        0        0      130 2024-05-24 21:03:00.492019 tonic_textual-2.0.1/tonic_textual/classes/enums/docx_header_footer_type.py
+-rw-r--r--   0        0        0      211 2024-05-24 21:03:00.492357 tonic_textual-2.0.1/tonic_textual/classes/enums/file_type.py
+-rw-r--r--   0        0        0      263 2024-05-24 21:03:00.492503 tonic_textual-2.0.1/tonic_textual/classes/enums/pdf_content_type.py
+-rw-r--r--   0        0        0      225 2024-05-24 21:03:00.492644 tonic_textual-2.0.1/tonic_textual/classes/enums/pdf_table_cell_type.py
+-rw-r--r--   0        0        0      800 2024-05-29 04:05:49.411802 tonic_textual-2.0.1/tonic_textual/classes/file_content/base_document.py
+-rw-r--r--   0        0        0     2150 2024-05-29 04:05:49.412196 tonic_textual-2.0.1/tonic_textual/classes/file_content/content.py
+-rw-r--r--   0        0        0      587 2024-05-24 21:03:00.493272 tonic_textual-2.0.1/tonic_textual/classes/file_content/csv_document.py
+-rw-r--r--   0        0        0     1037 2024-05-24 21:03:00.493457 tonic_textual-2.0.1/tonic_textual/classes/file_content/docx_document.py
+-rw-r--r--   0        0        0     1489 2024-05-24 21:03:00.493714 tonic_textual-2.0.1/tonic_textual/classes/file_content/pdf_document.py
+-rw-r--r--   0        0        0      385 2024-05-24 21:03:00.493923 tonic_textual-2.0.1/tonic_textual/classes/file_content/raw_document.py
+-rw-r--r--   0        0        0      790 2024-05-24 21:03:00.494112 tonic_textual-2.0.1/tonic_textual/classes/file_content/xlsx_document.py
+-rw-r--r--   0        0        0     2148 2024-05-24 23:05:01.047399 tonic_textual-2.0.1/tonic_textual/classes/file_parse_result_diff_enumerator.py
+-rw-r--r--   0        0        0     5112 2024-05-24 22:11:30.124934 tonic_textual-2.0.1/tonic_textual/classes/httpclient.py
+-rw-r--r--   0        0        0    10882 2024-05-29 04:05:49.412749 tonic_textual-2.0.1/tonic_textual/classes/parse_api_responses/file_parse_result.py
+-rw-r--r--   0        0        0      514 2024-05-24 21:03:00.495403 tonic_textual-2.0.1/tonic_textual/classes/parse_api_responses/file_parse_results_diff.py
+-rw-r--r--   0        0        0     2148 2024-05-24 21:03:00.495592 tonic_textual-2.0.1/tonic_textual/classes/pipeline.py
+-rw-r--r--   0        0        0     1970 2024-05-24 21:03:00.495892 tonic_textual-2.0.1/tonic_textual/classes/pipeline_file_enumerator.py
+-rw-r--r--   0        0        0      873 2024-05-24 21:03:00.496090 tonic_textual-2.0.1/tonic_textual/classes/pipeline_run.py
+-rw-r--r--   0        0        0      947 2024-05-24 21:03:00.496385 tonic_textual-2.0.1/tonic_textual/classes/redact_api_responses/redaction_response.py
+-rw-r--r--   0        0        0     2373 2024-05-24 23:05:01.047866 tonic_textual-2.0.1/tonic_textual/classes/tonic_exception.py
+-rw-r--r--   0        0        0      123 2024-05-24 21:03:00.496930 tonic_textual-2.0.1/tonic_textual/enums/pii_state.py
+-rw-r--r--   0        0        0     1538 2024-05-29 04:07:05.456011 tonic_textual-2.0.1/tonic_textual/generator_utils.py
+-rw-r--r--   0        0        0     2907 2024-05-24 21:03:00.497319 tonic_textual-2.0.1/tonic_textual/markdown_utils.py
+-rw-r--r--   0        0        0     2234 2024-05-24 21:03:00.497439 tonic_textual-2.0.1/tonic_textual/parse_api.py
+-rw-r--r--   0        0        0    19135 2024-05-24 21:03:00.497758 tonic_textual-2.0.1/tonic_textual/redact_api.py
+-rw-r--r--   0        0        0        0 2024-05-20 21:40:23.412740 tonic_textual-2.0.1/tonic_textual/services/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-24 21:03:00.498153 tonic_textual-2.0.1/tonic_textual/services/dataset.py
+-rw-r--r--   0        0        0      771 2024-05-24 21:03:00.498415 tonic_textual-2.0.1/tonic_textual/services/datasetfile.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 tonic_textual-2.0.1/PKG-INFO
```

### Comparing `tonic_textual-2.0.0/LICENSE` & `tonic_textual-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/README.md` & `tonic_textual-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/pyproject.toml` & `tonic_textual-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-textual"
-version = "2.0.0"
+version = "2.0.1"
 description = "Wrappers around the Tonic Textual API"
 authors = ["Adam Kamor <adam@tonic.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.tonic.ai/"
 keywords = ["tonic.ai", "tonic", "tonic textual"]
```

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/base_file.py` & `tonic_textual-2.0.1/tonic_textual/classes/common_api_responses/base_file.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/common_api_responses/single_detection_result.py` & `tonic_textual-2.0.1/tonic_textual/classes/common_api_responses/single_detection_result.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/dataset.py` & `tonic_textual-2.0.1/tonic_textual/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/datasetfile.py` & `tonic_textual-2.0.1/tonic_textual/classes/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_content/base_document.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_content/base_document.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_content/content.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_content/content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List, Dict
 from tonic_textual.enums.pii_state import PiiState
 from tonic_textual.classes.httpclient import HttpClient
 from tonic_textual.classes.common_api_responses.single_detection_result import (
     SingleDetectionResult,
 )
-from tonic_textual.generator_utils import filter_entities_by_config
+from tonic_textual.generator_utils import (
+    filter_entities_by_config, make_utf_compatible_entities
+)
 
 
 class Content:
     def __init__(self, client: HttpClient, json_def: Dict):
         self.ner_results: List[SingleDetectionResult] = [
             SingleDetectionResult(
                 s["pythonStart"], s["pythonEnd"], s["label"], s["text"], s["score"]
@@ -41,15 +43,16 @@
         generator_default: PiiState = PiiState.Off,
     ) -> str:
         markdown = self.get_markdown()
         all_entities = self.get_all_entities()
         entities = filter_entities_by_config(
             all_entities, generator_config, generator_default
         )
+        utf_compatible_entities = make_utf_compatible_entities(markdown, entities)
         response = self.client.http_post(
             "/api/redact/known_entities",
-            data={"knownEntities": entities, "text": markdown},
+            data={"knownEntities": utf_compatible_entities, "text": markdown},
         )
         return response["redactedText"]
 
     def is_sensitive(self, sensitive_entity_types: List[str]):
         return len(self.get_entities(sensitive_entity_types)) > 0
```

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_content/csv_document.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_content/csv_document.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_content/docx_document.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_content/docx_document.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_content/pdf_document.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_content/pdf_document.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_content/xlsx_document.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_content/xlsx_document.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/file_parse_result_diff_enumerator.py` & `tonic_textual-2.0.1/tonic_textual/classes/file_parse_result_diff_enumerator.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/httpclient.py` & `tonic_textual-2.0.1/tonic_textual/classes/httpclient.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/parse_api_responses/file_parse_result.py` & `tonic_textual-2.0.1/tonic_textual/classes/parse_api_responses/file_parse_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from tonic_textual.classes.file_content.docx_document import DocxDocument
 from tonic_textual.classes.file_content.pdf_document import PdfDocument
 from tonic_textual.classes.file_content.raw_document import RawDocument
 from tonic_textual.classes.file_content.xlsx_document import XlsxDocument
 from tonic_textual.classes.httpclient import HttpClient
 from tonic_textual.enums.pii_state import PiiState
 from tonic_textual.markdown_utils import split_markdown
-from tonic_textual.generator_utils import filter_entities_by_config
+from tonic_textual.generator_utils import (
+    filter_entities_by_config, make_utf_compatible_entities
+)
 
 
 class FileParseResult(object):
     def __init__(self, response: Dict, client: HttpClient, lazy_load_content=False):
         self.id: str = response["id"]
         self.file: BaseFile = BaseFile(response["file"])
         self.file_parse_job_id: str = response["fileParseJobId"]
@@ -30,15 +32,16 @@
         self.__is_content_retrieved = False
         self.content: Union[
             RawDocument, CsvDocument, DocxDocument, XlsxDocument, PdfDocument
         ]
         self.client = client
         if not lazy_load_content:
             self.__get_content()
-        self.metadata = {} 
+        self.metadata = {}
+
     def __get_content(self):
         if not self.__is_content_retrieved:
             with requests.Session() as session:
                 response = self.client.http_get(
                     f"/api/parsejob/files/{self.id}/content", session=session
                 )
 
@@ -46,37 +49,47 @@
                     self.content = CsvDocument(self.client, response)
                 elif self.file.fileType == FileTypeEnum.raw:
                     self.content = RawDocument(self.client, response)
                 elif self.file.fileType == FileTypeEnum.xlsx:
                     self.content = XlsxDocument(self.client, response)
                 elif self.file.fileType == FileTypeEnum.docX:
                     self.content = DocxDocument(self.client, response)
-                elif self.file.fileType == FileTypeEnum.pdf or self.file.fileType == FileTypeEnum.png or self.file.fileType == FileTypeEnum.jpg or self.file.fileType == FileTypeEnum.tif:
+                elif (
+                    self.file.fileType == FileTypeEnum.pdf
+                    or self.file.fileType == FileTypeEnum.png
+                    or self.file.fileType == FileTypeEnum.jpg
+                    or self.file.fileType == FileTypeEnum.tif
+                ):
                     self.content = PdfDocument(self.client, response)
                 else:
                     raise Exception("Unknown file type " + self.file.fileType)
 
             self.__is_content_retrieved = True
 
     def get_markdown(
         self,
         generator_config: Dict[str, PiiState] = dict(),
         generator_default: PiiState = PiiState.Off,
-    ):
+    ) -> str:
         self.__get_content()
         rawtext = self.content.get_markdown()
         filtered_entities = filter_entities_by_config(
-            self.content.get_all_entities(), generator_config, generator_default
+            self.content.get_all_entities(),
+            generator_config,
+            generator_default,
         )
         if len(filtered_entities) == 0:
             return rawtext
+        utf_compatible_filtered_entities = make_utf_compatible_entities(
+            rawtext, filtered_entities
+        )
         response = self.client.http_post(
             "/api/redact/known_entities",
-            data={"knownEntities": filtered_entities, "text": rawtext},
-        )  # TODO: need to implement this
+            data={"knownEntities": utf_compatible_filtered_entities, "text": rawtext},
+        )
         return response["redactedText"]
 
     def describe(self):
         return f"{self.parsed_file_path}"
 
     def get_all_entities(self) -> List[SingleDetectionResult]:
         self.__get_content()
@@ -105,21 +118,26 @@
         Returns:
             List[Dict]
                 A list of dictionaries containing the entity type, source start index,
                 source end index, the entity text, and replacement text.
         """
         self.__get_content()
         all_entities = self.content.get_all_entities()
+        rawtext = self.content.get_markdown()
         filtered_entities = filter_entities_by_config(
             all_entities, generator_config, generator_default
         )
         if allow_overlap:
             return filtered_entities
+        utf_compatible_filtered_entities = make_utf_compatible_entities(
+            rawtext, filtered_entities
+        )
         response = self.client.http_post(
-            "/api/redact/known_entities", data={"knownEntities": filtered_entities}
+            "/api/redact/known_entities",
+            data={"knownEntities": utf_compatible_filtered_entities}
         )
         return [
             SingleDetectionResult(
                 x["start"], x["end"], x["label"], x["text"], x["score"]
             )
             for x in list(response["deIdentifyResults"])
         ]
@@ -158,17 +176,15 @@
                 entity_list.append(entity_text)
             entity_dict[entity_type] = entity_list
         return entity_dict
 
     @staticmethod
     def _find_intersecting_entites(
         start: int, end: int, entities: List[SingleDetectionResult]
-    ) -> List[
-        Dict
-    ]:
+    ) -> List[Dict]:
         """Finds entities that intersect with the given start and end gindices
         Args:
             start: int
                 The start index to check for intersecting entities.
             end: int
                 The end index to check for intersecting entities. If -1, will return all
                 entities that occur after start
@@ -205,37 +221,40 @@
                 Values must be one of "Redaction", "Synthesis", or "Off".
 
             generator_default: PiiState = PiiState.Redaction
                 The default redaction used for all types not specified in
                 generator_config.
                 Values must be one of "Redaction", "Synthesis", or "Off".
 
+
             include_metadata: bool = True
                 If True, the metadata will be included in the chunk.
         Returns:
             List[str]
                 A list of strings containing the chunks of text.
         """
         text = self.get_markdown(generator_config, generator_default)
         all_entities = self.get_all_entities()
         entities = [ent for ent in all_entities if ent["label"] in metadata_entities]
         output = []
         for chunk in split_markdown(text, max_chars):
             start, end = chunk["indices"]
             headers = chunk["headers"]
-            sensitive_entity_types = [label for label, key in generator_config.items() if key != PiiState.Off]
-            
+            sensitive_entity_types = [
+                label for label, key in generator_config.items() if key != PiiState.Off
+            ]
+
             chunk_text = text[start:end]
-            is_sensitive = self.is_sensitive(sensitive_entity_types, start, end) # type: ignore
+            is_sensitive = self.is_sensitive(sensitive_entity_types, start, end)  # type: ignore
             chunk_dict = {"text": chunk_text, "is_sensitive": is_sensitive}
             if include_metadata:
                 entity_metdata = self._make_entity_metadata(  # type: ignore
                     self._find_intersecting_entites(
                         start, end, entities  # type: ignore
                     )
                 )
 
                 metadata = {"headers": headers, "entities": entity_metdata}
                 metadata.update(self.metadata)
-                chunk_dict['metadata'] = metadata
+                chunk_dict["metadata"] = metadata
             output.append(chunk_dict)
         return output
```

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/parse_api_responses/file_parse_results_diff.py` & `tonic_textual-2.0.1/tonic_textual/classes/parse_api_responses/file_parse_results_diff.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/pipeline.py` & `tonic_textual-2.0.1/tonic_textual/classes/pipeline.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/pipeline_file_enumerator.py` & `tonic_textual-2.0.1/tonic_textual/classes/pipeline_file_enumerator.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/pipeline_run.py` & `tonic_textual-2.0.1/tonic_textual/classes/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/redact_api_responses/redaction_response.py` & `tonic_textual-2.0.1/tonic_textual/classes/redact_api_responses/redaction_response.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/classes/tonic_exception.py` & `tonic_textual-2.0.1/tonic_textual/classes/tonic_exception.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/markdown_utils.py` & `tonic_textual-2.0.1/tonic_textual/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/parse_api.py` & `tonic_textual-2.0.1/tonic_textual/parse_api.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/redact_api.py` & `tonic_textual-2.0.1/tonic_textual/redact_api.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/services/dataset.py` & `tonic_textual-2.0.1/tonic_textual/services/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/tonic_textual/services/datasetfile.py` & `tonic_textual-2.0.1/tonic_textual/services/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-2.0.0/PKG-INFO` & `tonic_textual-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-textual
-Version: 2.0.0
+Version: 2.0.1
 Summary: Wrappers around the Tonic Textual API
 Home-page: https://www.tonic.ai/
 License: MIT
 Keywords: tonic.ai,tonic,tonic textual
 Author: Adam Kamor
 Author-email: adam@tonic.ai
 Requires-Python: >=3.7,<4.0
```

