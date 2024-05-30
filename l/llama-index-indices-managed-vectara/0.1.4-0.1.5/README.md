# Comparing `tmp/llama_index_indices_managed_vectara-0.1.4.tar.gz` & `tmp/llama_index_indices_managed_vectara-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_indices_managed_vectara-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_indices_managed_vectara-0.1.5.tar", max compression
```

## Comparing `llama_index_indices_managed_vectara-0.1.4.tar` & `llama_index_indices_managed_vectara-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       42 2024-03-13 20:45:49.665223 llama_index_indices_managed_vectara-0.1.4/README.md
--rw-r--r--   0        0        0      248 2024-03-13 20:45:49.665628 llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/__init__.py
--rw-r--r--   0        0        0    14037 2024-03-13 20:45:49.665736 llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/base.py
--rw-r--r--   0        0        0     4034 2024-03-13 20:45:49.665820 llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/prompts.py
--rw-r--r--   0        0        0     5450 2024-03-13 20:45:49.665884 llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/query.py
--rw-r--r--   0        0        0    11485 2024-03-13 20:45:49.665968 llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/retriever.py
--rw-r--r--   0        0        0     1566 2024-03-18 00:30:20.758727 llama_index_indices_managed_vectara-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 llama_index_indices_managed_vectara-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       42 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/README.md
+-rw-r--r--   0        0        0      248 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/__init__.py
+-rw-r--r--   0        0        0    15341 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/base.py
+-rw-r--r--   0        0        0     4034 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/prompts.py
+-rw-r--r--   0        0        0     9067 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/query.py
+-rw-r--r--   0        0        0    17939 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/retriever.py
+-rw-r--r--   0        0        0     1566 2024-05-30 03:13:05.917119 llama_index_indices_managed_vectara-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 llama_index_indices_managed_vectara-0.1.5/PKG-INFO
```

### Comparing `llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/base.py` & `llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Managed index.
+"""
+Managed index.
 
 A managed Index - where the index is accessible via some API that
 interfaces a managed service.
 
 """
 
 import json
@@ -10,47 +11,47 @@
 import os
 from concurrent.futures import ThreadPoolExecutor
 from hashlib import blake2b
 from typing import Any, Dict, List, Optional, Sequence, Type
 
 import requests
 from llama_index.core.base.base_query_engine import BaseQueryEngine
+from llama_index.core.chat_engine.types import BaseChatEngine
 from llama_index.core.base.base_retriever import BaseRetriever
 from llama_index.core.callbacks.base import CallbackManager
 from llama_index.core.data_structs.data_structs import IndexDict, IndexStructType
 from llama_index.core.indices.managed.base import BaseManagedIndex, IndexType
 from llama_index.core.llms.utils import LLMType, resolve_llm
 from llama_index.core.schema import (
     BaseNode,
     Document,
     MetadataMode,
     TextNode,
     TransformComponent,
 )
-from llama_index.core.service_context import ServiceContext
 from llama_index.core.settings import Settings
-from llama_index.core.storage.storage_context import StorageContext
-
 from llama_index.core.response_synthesizers import ResponseMode
 from llama_index.core import get_response_synthesizer
 
+
 _logger = logging.getLogger(__name__)
 
 
 class VectaraIndexStruct(IndexDict):
     """Vectara Index Struct."""
 
     @classmethod
     def get_type(cls) -> IndexStructType:
         """Get index struct type."""
         return IndexStructType.VECTARA
 
 
 class VectaraIndex(BaseManagedIndex):
-    """Vectara Index.
+    """
+    Vectara Index.
 
     The Vectara index implements a managed index that uses Vectara as the backend.
     Vectara performs a lot of the functions in traditional indexes in the backend:
     - breaks down a document into chunks (nodes)
     - Creates the embedding for each chunk (node)
     - Performs the search for the top k most similar nodes to a query
     - Optionally can perform summarization of the top k nodes
@@ -77,24 +78,21 @@
             index_id=str(vectara_corpus_id),
             summary="Vectara Index",
         )
 
         super().__init__(
             show_progress=show_progress,
             index_struct=index_struct,
-            service_context=ServiceContext.from_defaults(
-                llm=None, llm_predictor=None, embed_model=None
-            ),
             **kwargs,
         )
         self._vectara_customer_id = vectara_customer_id or os.environ.get(
             "VECTARA_CUSTOMER_ID"
         )
-        self._vectara_corpus_id = vectara_corpus_id or os.environ.get(
-            "VECTARA_CORPUS_ID"
+        self._vectara_corpus_id = vectara_corpus_id or str(
+            os.environ.get("VECTARA_CORPUS_ID")
         )
         self._vectara_api_key = vectara_api_key or os.environ.get("VECTARA_API_KEY")
         if (
             self._vectara_customer_id is None
             or self._vectara_corpus_id is None
             or self._vectara_api_key is None
         ):
@@ -130,37 +128,50 @@
                 id_=node.id_,  # type: ignore
             )
             for node in nodes
         ]
         self.add_documents(docs, use_core_api)
         return self.index_struct
 
+    def _get_corpus_id(self, corpus_id: str) -> str:
+        """
+        Get the corpus id to use for the index.
+        If corpus_id is provided, check if it is one of the valid corpus ids.
+        If not, use the first corpus id in the list.
+        """
+        if corpus_id is not None:
+            if corpus_id in self._vectara_corpus_id.split(","):
+                return corpus_id
+        return self._vectara_corpus_id.split(",")[0]
+
     def _get_post_headers(self) -> dict:
         """Returns headers that should be attached to each post request."""
         return {
             "x-api-key": self._vectara_api_key,
             "customer-id": self._vectara_customer_id,
             "Content-Type": "application/json",
             "X-Source": "llama_index",
         }
 
-    def _delete_doc(self, doc_id: str) -> bool:
+    def _delete_doc(self, doc_id: str, corpus_id: Optional[str] = None) -> bool:
         """
         Delete a document from the Vectara corpus.
 
         Args:
             url (str): URL of the page to delete.
             doc_id (str): ID of the document to delete.
+            corpus_id (str): corpus ID to delete the document from.
 
         Returns:
             bool: True if deletion was successful, False otherwise.
         """
+        valid_corpus_id = self._get_corpus_id(corpus_id)
         body = {
             "customerId": self._vectara_customer_id,
-            "corpusId": self._vectara_corpus_id,
+            "corpusId": valid_corpus_id,
             "documentId": doc_id,
         }
         response = self._session.post(
             "https://api.vectara.io/v1/delete-doc",
             data=json.dumps(body),
             verify=True,
             headers=self._get_post_headers(),
@@ -172,18 +183,18 @@
                 f"Delete request failed for doc_id = {doc_id} with status code "
                 f"{response.status_code}, reason {response.reason}, text "
                 f"{response.text}"
             )
             return False
         return True
 
-    def _index_doc(self, doc: dict) -> str:
+    def _index_doc(self, doc: dict, corpus_id) -> str:
         request: Dict[str, Any] = {}
         request["customerId"] = self._vectara_customer_id
-        request["corpusId"] = self._vectara_corpus_id
+        request["corpusId"] = corpus_id
         request["document"] = doc
 
         if "parts" in doc:
             api_url = "https://api.vectara.io/v1/core/index"
         else:
             api_url = "https://api.vectara.io/v1/index"
 
@@ -207,14 +218,15 @@
             return "E_NO_PERMISSIONS"
         else:
             return "E_SUCCEEDED"
 
     def _insert(
         self,
         nodes: Sequence[BaseNode],
+        corpus_id: Optional[str] = None,
         use_core_api: bool = False,
         **insert_kwargs: Any,
     ) -> None:
         """Insert a set of documents (each a node)."""
 
         def gen_hash(s: str) -> str:
             hash_object = blake2b(digest_size=32)
@@ -231,50 +243,58 @@
             doc = {
                 "documentId": doc_id,
                 "metadataJson": json.dumps(node.metadata),
                 section_key: [{"text": text}],
             }
             docs.append(doc)
 
+        valid_corpus_id = self._get_corpus_id(corpus_id)
         if self.parallelize_ingest:
             with ThreadPoolExecutor() as executor:
-                futures = [executor.submit(self._index_doc, doc) for doc in docs]
+                futures = [
+                    executor.submit(self._index_doc, doc, valid_corpus_id)
+                    for doc in docs
+                ]
                 for future in futures:
                     ecode = future.result()
                     if ecode != "E_SUCCEEDED":
                         _logger.error(
                             f"Error indexing document in Vectara with error code {ecode}"
                         )
+            self.doc_ids.extend([doc["documentId"] for doc in docs])
         else:
             for doc in docs:
-                ecode = self._index_doc(doc)
+                ecode = self._index_doc(doc, valid_corpus_id)
                 if ecode != "E_SUCCEEDED":
                     _logger.error(
                         f"Error indexing document in Vectara with error code {ecode}"
                     )
-                self.doc_ids.append(doc_id)
+                self.doc_ids.append(doc["documentId"])
 
     def add_documents(
         self,
         docs: Sequence[Document],
+        corpus_id: Optional[str],
         use_core_api: bool = False,
         allow_update: bool = True,
     ) -> None:
         nodes = [
             TextNode(text=doc.get_content(), metadata=doc.metadata) for doc in docs  # type: ignore
         ]
-        self._insert(nodes, use_core_api)
+        self._insert(nodes, corpus_id, use_core_api)
 
     def insert_file(
         self,
         file_path: str,
         metadata: Optional[dict] = None,
+        corpus_id: Optional[str] = None,
         **insert_kwargs: Any,
     ) -> Optional[str]:
-        """Vectara provides a way to add files (binary or text) directly via our API
+        """
+        Vectara provides a way to add files (binary or text) directly via our API
         where pre-processing and chunking occurs internally in an optimal way
         This method provides a way to use that API in Llama_index.
 
         # ruff: noqa: E501
         Full API Docs: https://docs.vectara.com/docs/api-reference/indexing-apis/
         file-upload/file-upload-filetypes
 
@@ -295,33 +315,40 @@
         metadata["framework"] = "llama_index"
         files: dict = {
             "file": (file_path, open(file_path, "rb")),
             "doc_metadata": json.dumps(metadata),
         }
         headers = self._get_post_headers()
         headers.pop("Content-Type")
+        valid_corpus_id = self._get_corpus_id(corpus_id)
         response = self._session.post(
-            f"https://api.vectara.io/upload?c={self._vectara_customer_id}&o={self._vectara_corpus_id}&d=True",
+            f"https://api.vectara.io/upload?c={self._vectara_customer_id}&o={valid_corpus_id}&d=True",
             files=files,
             verify=True,
             headers=headers,
             timeout=self.vectara_api_timeout,
         )
 
+        res = response.json()
         if response.status_code == 409:
-            doc_id = response.json()["document"]["documentId"]
             _logger.info(
-                f"File {file_path} already exists on Vectara "
-                f"(doc_id={doc_id}), skipping"
+                f"File {file_path} already exists on Vectara, skipping indexing"
             )
             return None
         elif response.status_code == 200:
-            return response.json()["document"]["documentId"]
+            quota = res["response"]["quotaConsumed"]["numChars"]
+            if quota == 0:
+                _logger.warning(
+                    f"File Upload for {file_path} returned 0 quota consumed, please check your Vectara account quota"
+                )
+            doc_id = res["document"]["documentId"]
+            self.doc_ids.append(doc_id)
+            return doc_id
         else:
-            _logger.info(f"Error indexing file {file_path}: {response.json()}")
+            _logger.info(f"Error indexing file {file_path}: {res}")
             return None
 
     def delete_ref_doc(
         self, ref_doc_id: str, delete_from_docstore: bool = False, **delete_kwargs: Any
     ) -> None:
         raise NotImplementedError(
             "Vectara does not support deleting a reference document"
@@ -336,25 +363,35 @@
         """Return a Retriever for this managed index."""
         from llama_index.indices.managed.vectara.retriever import (
             VectaraRetriever,
         )
 
         return VectaraRetriever(self, **kwargs)
 
+    def as_chat_engine(self, **kwargs: Any) -> BaseChatEngine:
+        kwargs["summary_enabled"] = True
+        retriever = self.as_retriever(**kwargs)
+        kwargs.pop("summary_enabled")
+        from llama_index.indices.managed.vectara.query import (
+            VectaraChatEngine,
+        )
+
+        return VectaraChatEngine.from_args(retriever, **kwargs)  # type: ignore
+
     def as_query_engine(
         self, llm: Optional[LLMType] = None, **kwargs: Any
     ) -> BaseQueryEngine:
         if kwargs.get("summary_enabled", True):
             from llama_index.indices.managed.vectara.query import (
                 VectaraQueryEngine,
             )
 
             kwargs["summary_enabled"] = True
             retriever = self.as_retriever(**kwargs)
-            return VectaraQueryEngine.from_args(retriever, **kwargs)  # type: ignore
+            return VectaraQueryEngine.from_args(retriever=retriever, **kwargs)  # type: ignore
         else:
             from llama_index.core.query_engine.retriever_query_engine import (
                 RetrieverQueryEngine,
             )
 
             llm = (
                 resolve_llm(llm, callback_manager=self._callback_manager)
@@ -372,20 +409,17 @@
                 **kwargs,
             )
 
     @classmethod
     def from_documents(
         cls: Type[IndexType],
         documents: Sequence[Document],
-        storage_context: Optional[StorageContext] = None,
         show_progress: bool = False,
         callback_manager: Optional[CallbackManager] = None,
         transformations: Optional[List[TransformComponent]] = None,
-        # deprecated
-        service_context: Optional[ServiceContext] = None,
         **kwargs: Any,
     ) -> IndexType:
         """Build a Vectara index from a sequence of documents."""
         nodes = [
             TextNode(text=document.get_content(), metadata=document.metadata)  # type: ignore
             for document in documents
         ]
```

### Comparing `llama_index_indices_managed_vectara-0.1.4/llama_index/indices/managed/vectara/prompts.py` & `llama_index_indices_managed_vectara-0.1.5/llama_index/indices/managed/vectara/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_indices_managed_vectara-0.1.4/pyproject.toml` & `llama_index_indices_managed_vectara-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index managed vectara integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-indices-managed-vectara"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_indices_managed_vectara-0.1.4/PKG-INFO` & `llama_index_indices_managed_vectara-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-indices-managed-vectara
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index managed vectara integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

