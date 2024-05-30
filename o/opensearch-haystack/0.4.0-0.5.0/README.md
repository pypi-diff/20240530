# Comparing `tmp/opensearch_haystack-0.4.0.tar.gz` & `tmp/opensearch_haystack-0.5.0.tar.gz`

## Comparing `opensearch_haystack-0.4.0.tar` & `opensearch_haystack-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/docker-compose.yml
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/pydoc/config.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/__init__.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/__init__.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/document_store.py
--rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_bm25_retriever.py
--rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_filters.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/LICENSE
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/README.md
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/docker-compose.yml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/pydoc/config.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/opensearch/__init__.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/src/haystack_integrations/document_stores/opensearch/__init__.py
+-rw-r--r--   0        0        0    16002 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/src/haystack_integrations/document_stores/opensearch/document_store.py
+-rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/src/haystack_integrations/document_stores/opensearch/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/tests/test_bm25_retriever.py
+-rw-r--r--   0        0        0    18197 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/LICENSE
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/README.md
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 opensearch_haystack-0.5.0/PKG-INFO
```

### Comparing `opensearch_haystack-0.4.0/pydoc/config.yml` & `opensearch_haystack-0.5.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py` & `opensearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py` & `opensearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/document_store.py` & `opensearch_haystack-0.5.0/src/haystack_integrations/document_stores/opensearch/document_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,76 +23,101 @@
 # (e.g., BM25_SCALING_FACTOR for the bm25_retrieval method).
 # Larger scaling factor decreases scaled scores. For example, an input of 10 is scaled to 0.99 with
 # BM25_SCALING_FACTOR=2 but to 0.78 with BM25_SCALING_FACTOR=8 (default). The defaults were chosen empirically.
 # Increase the default if most unscaled scores are larger than expected (>30) and otherwise would incorrectly
 # all be mapped to scores ~1.
 BM25_SCALING_FACTOR = 8
 
+DEFAULT_SETTINGS = {"index.knn": True}
+DEFAULT_MAX_CHUNK_BYTES = 100 * 1024 * 1024
+
 
 class OpenSearchDocumentStore:
     def __init__(
         self,
         *,
         hosts: Optional[Hosts] = None,
         index: str = "default",
+        max_chunk_bytes: int = DEFAULT_MAX_CHUNK_BYTES,
+        embedding_dim: int = 768,
+        method: Optional[Dict[str, Any]] = None,
+        mappings: Optional[Dict[str, Any]] = None,
+        settings: Optional[Dict[str, Any]] = DEFAULT_SETTINGS,
         **kwargs,
     ):
         """
         Creates a new OpenSearchDocumentStore instance.
 
-        For more information on connection parameters, see the [official OpenSearch documentation](https://opensearch.org/docs/latest/clients/python-low-level/#connecting-to-opensearch)
+        The ``embeddings_dim``, ``method``, ``mappings``, and ``settings`` arguments are only used if the index does not
+        exists and needs to be created. If the index already exists, its current configurations will be used.
 
-        For the full list of supported kwargs, see the [official OpenSearch reference](https://opensearch-project.github.io/opensearch-py/api-ref/clients/opensearch_client.html)
+        For more information on connection parameters, see the [official OpenSearch documentation](https://opensearch.org/docs/latest/clients/python-low-level/#connecting-to-opensearch)
 
         :param hosts: List of hosts running the OpenSearch client. Defaults to None
         :param index: Name of index in OpenSearch, if it doesn't exist it will be created. Defaults to "default"
-        :param **kwargs: Optional arguments that ``OpenSearch`` takes.
+        :param max_chunk_bytes: Maximum size of the requests in bytes. Defaults to 100MB
+        :param embedding_dim: Dimension of the embeddings. Defaults to 768
+        :param method: The method definition of the underlying configuration of the approximate k-NN algorithm. Please
+            see the [official OpenSearch docs](https://opensearch.org/docs/latest/search-plugins/knn/knn-index/#method-definitions)
+            for more information. Defaults to None
+        :param mappings: The mapping of how the documents are stored and indexed. Please see the [official OpenSearch docs](https://opensearch.org/docs/latest/field-types/)
+            for more information. If None, it uses the embedding_dim and method arguments to create default mappings.
+            Defaults to None
+        :param settings: The settings of the index to be created. Please see the [official OpenSearch docs](https://opensearch.org/docs/latest/search-plugins/knn/knn-index/#index-settings)
+            for more information. Defaults to {"index.knn": True}
+        :param **kwargs: Optional arguments that ``OpenSearch`` takes. For the full list of supported kwargs,
+            see the [official OpenSearch reference](https://opensearch-project.github.io/opensearch-py/api-ref/clients/opensearch_client.html)
         """
         self._client = None
         self._hosts = hosts
         self._index = index
+        self._max_chunk_bytes = max_chunk_bytes
+        self._embedding_dim = embedding_dim
+        self._method = method
+        self._mappings = mappings or self._get_default_mappings()
+        self._settings = settings
         self._kwargs = kwargs
 
+    def _get_default_mappings(self) -> Dict[str, Any]:
+        default_mappings: Dict[str, Any] = {
+            "properties": {
+                "embedding": {"type": "knn_vector", "index": True, "dimension": self._embedding_dim},
+                "content": {"type": "text"},
+            },
+            "dynamic_templates": [
+                {
+                    "strings": {
+                        "match_mapping_type": "string",
+                        "mapping": {"type": "keyword"},
+                    }
+                }
+            ],
+        }
+        if self._method:
+            default_mappings["properties"]["embedding"]["method"] = self._method
+        return default_mappings
+
     @property
     def client(self) -> OpenSearch:
         if not self._client:
             self._client = OpenSearch(self._hosts, **self._kwargs)
             # Check client connection, this will raise if not connected
             self._client.info()  # type:ignore
 
+        if self._client.indices.exists(index=self._index):  # type:ignore
+            logger.debug(
+                "The index '%s' already exists. The `embedding_dim`, `method`, `mappings`, and "
+                "`settings` values will be ignored.",
+                self._index,
+            )
+        else:
             # Create the index if it doesn't exist
-            if not self._client.indices.exists(index=self._index):  # type:ignore
-                # configure fallback mapping for the embedding field
-                method = self._kwargs.get("method", None)
-                embedding_dim = self._kwargs.get("embedding_dim", 768)
-                default_mappings: Dict[str, Any] = {
-                    "properties": {
-                        "embedding": {"type": "knn_vector", "index": True, "dimension": embedding_dim},
-                        "content": {"type": "text"},
-                    },
-                    "dynamic_templates": [
-                        {
-                            "strings": {
-                                "match_mapping_type": "string",
-                                "mapping": {
-                                    "type": "keyword",
-                                },
-                            }
-                        }
-                    ],
-                }
-                if method:
-                    default_mappings["properties"]["embedding"]["method"] = method
-
-                body = {
-                    "mappings": self._kwargs.get("mappings", default_mappings),
-                    "settings": self._kwargs.get("settings", {"index.knn": True}),
-                }
-                self._client.indices.create(index=self._index, body=body)  # type:ignore
+            body = {"mappings": self._mappings, "settings": self._settings}
 
+            self._client.indices.create(index=self._index, body=body)  # type:ignore
         return self._client
 
     def to_dict(self) -> Dict[str, Any]:
         # This is not the best solution to serialise this class but is the fastest to implement.
         # Not all kwargs types can be serialised to text so this can fail. We must serialise each
         # type explicitly to handle this properly.
         """
@@ -101,14 +126,19 @@
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             hosts=self._hosts,
             index=self._index,
+            max_chunk_bytes=self._max_chunk_bytes,
+            embedding_dim=self._embedding_dim,
+            method=self._method,
+            mappings=self._mappings,
+            settings=self._settings,
             **self._kwargs,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "OpenSearchDocumentStore":
         """
         Deserializes the component from a dictionary.
@@ -174,14 +204,15 @@
                     "_source": doc.to_dict(),
                 }
                 for doc in documents
             ),
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
+            max_chunk_bytes=self._max_chunk_bytes,
         )
 
         if errors:
             duplicate_errors_ids = []
             other_errors = []
             for e in errors:
                 # OpenSearch might not return a correctly formatted error, in that case we
@@ -230,14 +261,15 @@
 
         bulk(
             client=self.client,
             actions=({"_op_type": "delete", "_id": id_} for id_ in document_ids),
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
+            max_chunk_bytes=self._max_chunk_bytes,
         )
 
     def _bm25_retrieval(
         self,
         query: str,
         *,
         filters: Optional[Dict[str, Any]] = None,
```

### Comparing `opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/filters.py` & `opensearch_haystack-0.5.0/src/haystack_integrations/document_stores/opensearch/filters.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/tests/test_bm25_retriever.py` & `opensearch_haystack-0.5.0/tests/test_bm25_retriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 from unittest.mock import Mock, patch
 
 from haystack.dataclasses import Document
 from haystack_integrations.components.retrievers.opensearch import OpenSearchBM25Retriever
 from haystack_integrations.document_stores.opensearch import OpenSearchDocumentStore
+from haystack_integrations.document_stores.opensearch.document_store import DEFAULT_MAX_CHUNK_BYTES
 
 
 def test_init_default():
     mock_store = Mock(spec=OpenSearchDocumentStore)
     retriever = OpenSearchBM25Retriever(document_store=mock_store)
     assert retriever._document_store == mock_store
     assert retriever._filters == {}
@@ -23,16 +24,29 @@
     retriever = OpenSearchBM25Retriever(document_store=document_store)
     res = retriever.to_dict()
     assert res == {
         "type": "haystack_integrations.components.retrievers.opensearch.bm25_retriever.OpenSearchBM25Retriever",
         "init_parameters": {
             "document_store": {
                 "init_parameters": {
+                    "embedding_dim": 768,
                     "hosts": "some fake host",
                     "index": "default",
+                    "mappings": {
+                        "dynamic_templates": [
+                            {"strings": {"mapping": {"type": "keyword"}, "match_mapping_type": "string"}}
+                        ],
+                        "properties": {
+                            "content": {"type": "text"},
+                            "embedding": {"dimension": 768, "index": True, "type": "knn_vector"},
+                        },
+                    },
+                    "max_chunk_bytes": DEFAULT_MAX_CHUNK_BYTES,
+                    "method": None,
+                    "settings": {"index.knn": True},
                 },
                 "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
             },
             "filters": {},
             "fuzziness": "AUTO",
             "top_k": 10,
             "scale_score": False,
```

### Comparing `opensearch_haystack-0.4.0/tests/test_document_store.py` & `opensearch_haystack-0.5.0/tests/test_document_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,50 +7,88 @@
 
 import pytest
 from haystack.dataclasses.document import Document
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 from haystack_integrations.document_stores.opensearch import OpenSearchDocumentStore
+from haystack_integrations.document_stores.opensearch.document_store import DEFAULT_MAX_CHUNK_BYTES
 from opensearchpy.exceptions import RequestError
 
 
 @patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
 def test_to_dict(_mock_opensearch_client):
     document_store = OpenSearchDocumentStore(hosts="some hosts")
     res = document_store.to_dict()
     assert res == {
         "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
         "init_parameters": {
+            "embedding_dim": 768,
             "hosts": "some hosts",
             "index": "default",
+            "mappings": {
+                "dynamic_templates": [{"strings": {"mapping": {"type": "keyword"}, "match_mapping_type": "string"}}],
+                "properties": {
+                    "content": {"type": "text"},
+                    "embedding": {"dimension": 768, "index": True, "type": "knn_vector"},
+                },
+            },
+            "max_chunk_bytes": DEFAULT_MAX_CHUNK_BYTES,
+            "method": None,
+            "settings": {"index.knn": True},
         },
     }
 
 
 @patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
 def test_from_dict(_mock_opensearch_client):
     data = {
         "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
-        "init_parameters": {
-            "hosts": "some hosts",
-            "index": "default",
-        },
+        "init_parameters": {"hosts": "some hosts", "index": "default", "max_chunk_bytes": 1000, "embedding_dim": 1536},
     }
     document_store = OpenSearchDocumentStore.from_dict(data)
     assert document_store._hosts == "some hosts"
     assert document_store._index == "default"
+    assert document_store._max_chunk_bytes == 1000
+    assert document_store._embedding_dim == 1536
+    assert document_store._method is None
+    assert document_store._mappings == {
+        "properties": {
+            "embedding": {"type": "knn_vector", "index": True, "dimension": 1536},
+            "content": {"type": "text"},
+        },
+        "dynamic_templates": [
+            {
+                "strings": {
+                    "match_mapping_type": "string",
+                    "mapping": {"type": "keyword"},
+                }
+            }
+        ],
+    }
+    assert document_store._settings == {"index.knn": True}
 
 
 @patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
 def test_init_is_lazy(_mock_opensearch_client):
     OpenSearchDocumentStore(hosts="testhost")
     _mock_opensearch_client.assert_not_called()
 
 
+@patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
+def test_get_default_mappings(_mock_opensearch_client):
+    store = OpenSearchDocumentStore(hosts="testhost", embedding_dim=1536, method={"name": "hnsw"})
+    assert store._mappings["properties"]["embedding"] == {
+        "type": "knn_vector",
+        "index": True,
+        "dimension": 1536,
+        "method": {"name": "hnsw"},
+    }
+
+
 @pytest.mark.integration
 class TestDocumentStore(DocumentStoreBaseTests):
     """
     Common test cases will be provided by `DocumentStoreBaseTests` but
     you can add more to this class.
     """
 
@@ -335,7 +373,14 @@
     def test_write_documents_with_badly_formatted_bulk_errors(self, mock_bulk, document_store):
         error = {"some_key": "some_value"}
         mock_bulk.return_value = ([], [error])
 
         with pytest.raises(DocumentStoreError) as e:
             document_store.write_documents([Document(content="Hello world")])
             e.match(f"{error}")
+
+    @patch("haystack_integrations.document_stores.opensearch.document_store.bulk")
+    def test_write_documents_max_chunk_bytes(self, mock_bulk, document_store):
+        mock_bulk.return_value = (1, [])
+        document_store.write_documents([Document(content="Hello world")])
+
+        assert mock_bulk.call_args.kwargs["max_chunk_bytes"] == DEFAULT_MAX_CHUNK_BYTES
```

### Comparing `opensearch_haystack-0.4.0/tests/test_embedding_retriever.py` & `opensearch_haystack-0.5.0/tests/test_embedding_retriever.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 from unittest.mock import Mock, patch
 
 from haystack.dataclasses import Document
 from haystack_integrations.components.retrievers.opensearch import OpenSearchEmbeddingRetriever
 from haystack_integrations.document_stores.opensearch import OpenSearchDocumentStore
+from haystack_integrations.document_stores.opensearch.document_store import DEFAULT_MAX_CHUNK_BYTES
 
 
 def test_init_default():
     mock_store = Mock(spec=OpenSearchDocumentStore)
     retriever = OpenSearchEmbeddingRetriever(document_store=mock_store)
     assert retriever._document_store == mock_store
     assert retriever._filters == {}
@@ -23,16 +24,44 @@
     res = retriever.to_dict()
     type_s = "haystack_integrations.components.retrievers.opensearch.embedding_retriever.OpenSearchEmbeddingRetriever"
     assert res == {
         "type": type_s,
         "init_parameters": {
             "document_store": {
                 "init_parameters": {
+                    "embedding_dim": 768,
                     "hosts": "some fake host",
                     "index": "default",
+                    "mappings": {
+                        "dynamic_templates": [
+                            {
+                                "strings": {
+                                    "mapping": {
+                                        "type": "keyword",
+                                    },
+                                    "match_mapping_type": "string",
+                                },
+                            },
+                        ],
+                        "properties": {
+                            "content": {
+                                "type": "text",
+                            },
+                            "embedding": {
+                                "dimension": 768,
+                                "index": True,
+                                "type": "knn_vector",
+                            },
+                        },
+                    },
+                    "max_chunk_bytes": DEFAULT_MAX_CHUNK_BYTES,
+                    "method": None,
+                    "settings": {
+                        "index.knn": True,
+                    },
                 },
                 "type": "haystack_integrations.document_stores.opensearch.document_store.OpenSearchDocumentStore",
             },
             "filters": {},
             "top_k": 10,
         },
     }
```

### Comparing `opensearch_haystack-0.4.0/tests/test_filters.py` & `opensearch_haystack-0.5.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/.gitignore` & `opensearch_haystack-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/LICENSE` & `opensearch_haystack-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/README.md` & `opensearch_haystack-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/pyproject.toml` & `opensearch_haystack-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.4.0/PKG-INFO` & `opensearch_haystack-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opensearch-haystack
-Version: 0.4.0
+Version: 0.5.0
 Summary: Haystack 2.x Document Store for OpenSearch
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/opensearch#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/opensearch
 Author-email: deepset <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

