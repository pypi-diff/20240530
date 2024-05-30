# Comparing `tmp/elasticsearch_haystack-0.5.0.tar.gz` & `tmp/elasticsearch_haystack-0.6.0.tar.gz`

## Comparing `elasticsearch_haystack-0.5.0.tar` & `elasticsearch_haystack-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/docker-compose.yml
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/pydoc/config.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/__init__.py
--rw-r--r--   0        0        0    18304 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_bm25_retriever.py
--rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_document_store.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_filters.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/LICENSE
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/README.md
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/docker-compose.yml
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/pydoc/config.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/src/haystack_integrations/components/retrievers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/src/haystack_integrations/document_stores/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    18719 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/src/haystack_integrations/document_stores/elasticsearch/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/tests/test_bm25_retriever.py
+-rw-r--r--   0        0        0    14683 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/LICENSE
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/README.md
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.6.0/PKG-INFO
```

### Comparing `elasticsearch_haystack-0.5.0/pydoc/config.yml` & `elasticsearch_haystack-0.6.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py` & `elasticsearch_haystack-0.6.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py` & `elasticsearch_haystack-0.6.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py` & `elasticsearch_haystack-0.6.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,56 +89,68 @@
             This parameter only takes effect if the index does not yet exist and is created.
             To choose the most appropriate function, look for information about your embedding model.
             To understand how document scores are computed, see the Elasticsearch
             [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/dense-vector.html#dense-vector-params)
         :param **kwargs: Optional arguments that `Elasticsearch` takes.
         """
         self._hosts = hosts
-        self._client = Elasticsearch(
-            hosts,
-            headers={"user-agent": f"haystack-py-ds/{haystack_version}"},
-            **kwargs,
-        )
+        self._client = None
         self._index = index
         self._embedding_similarity_function = embedding_similarity_function
         self._custom_mapping = custom_mapping
         self._kwargs = kwargs
 
-        # Check client connection, this will raise if not connected
-        self._client.info()
-
         if self._custom_mapping and not isinstance(self._custom_mapping, Dict):
             msg = "custom_mapping must be a dictionary"
             raise ValueError(msg)
 
-        if self._custom_mapping:
-            mappings = self._custom_mapping
-        else:
-            # Configure mapping for the embedding field if none is provided
-            mappings = {
-                "properties": {
-                    "embedding": {"type": "dense_vector", "index": True, "similarity": embedding_similarity_function},
-                    "content": {"type": "text"},
-                },
-                "dynamic_templates": [
-                    {
-                        "strings": {
-                            "path_match": "*",
-                            "match_mapping_type": "string",
-                            "mapping": {
-                                "type": "keyword",
-                            },
+    @property
+    def client(self) -> Elasticsearch:
+        if self._client is None:
+            client = Elasticsearch(
+                self._hosts,
+                headers={"user-agent": f"haystack-py-ds/{haystack_version}"},
+                **self._kwargs,
+            )
+            # Check client connection, this will raise if not connected
+            client.info()
+
+            if self._custom_mapping:
+                mappings = self._custom_mapping
+            else:
+                # Configure mapping for the embedding field if none is provided
+                mappings = {
+                    "properties": {
+                        "embedding": {
+                            "type": "dense_vector",
+                            "index": True,
+                            "similarity": self._embedding_similarity_function,
+                        },
+                        "content": {"type": "text"},
+                    },
+                    "dynamic_templates": [
+                        {
+                            "strings": {
+                                "path_match": "*",
+                                "match_mapping_type": "string",
+                                "mapping": {
+                                    "type": "keyword",
+                                },
+                            }
                         }
-                    }
-                ],
-            }
-
-        # Create the index if it doesn't exist
-        if not self._client.indices.exists(index=index):
-            self._client.indices.create(index=index, mappings=mappings)
+                    ],
+                }
+
+            # Create the index if it doesn't exist
+            if not client.indices.exists(index=self._index):
+                client.indices.create(index=self._index, mappings=mappings)
+
+            self._client = client
+
+        return self._client
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
@@ -168,30 +180,30 @@
         return default_from_dict(cls, data)
 
     def count_documents(self) -> int:
         """
         Returns how many documents are present in the document store.
         :returns: Number of documents in the document store.
         """
-        return self._client.count(index=self._index)["count"]
+        return self.client.count(index=self._index)["count"]
 
     def _search_documents(self, **kwargs) -> List[Document]:
         """
         Calls the Elasticsearch client's search method and handles pagination.
         """
 
         top_k = kwargs.get("size")
         if top_k is None and "knn" in kwargs and "k" in kwargs["knn"]:
             top_k = kwargs["knn"]["k"]
 
         documents: List[Document] = []
         from_ = 0
         # Handle pagination
         while True:
-            res = self._client.search(
+            res = self.client.search(
                 index=self._index,
                 from_=from_,
                 **kwargs,
             )
 
             documents.extend(self._deserialize_document(hit) for hit in res["hits"]["hits"])
             from_ = len(documents)
@@ -257,15 +269,15 @@
                     "_op_type": action,
                     "_id": doc.id,
                     "_source": doc_dict,
                 }
             )
 
         documents_written, errors = helpers.bulk(
-            client=self._client,
+            client=self.client,
             actions=elasticsearch_actions,
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
         )
 
         if errors:
@@ -313,15 +325,15 @@
         """
         Deletes all `Document`s with a matching `document_ids` from the document store.
 
         :param document_ids: the object IDs to delete
         """
 
         helpers.bulk(
-            client=self._client,
+            client=self.client,
             actions=({"_op_type": "delete", "_id": id_} for id_ in document_ids),
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
         )
 
     def _bm25_retrieval(
```

### Comparing `elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/filters.py` & `elasticsearch_haystack-0.6.0/src/haystack_integrations/document_stores/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/tests/test_bm25_retriever.py` & `elasticsearch_haystack-0.6.0/tests/test_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/tests/test_document_store.py` & `elasticsearch_haystack-0.6.0/tests/test_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 from haystack_integrations.document_stores.elasticsearch import ElasticsearchDocumentStore
 
 
 @patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
+def test_init_is_lazy(_mock_es_client):
+    ElasticsearchDocumentStore(hosts="testhost")
+    _mock_es_client.assert_not_called()
+
+
+@patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
 def test_to_dict(_mock_elasticsearch_client):
     document_store = ElasticsearchDocumentStore(hosts="some hosts")
     res = document_store.to_dict()
     assert res == {
         "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
         "init_parameters": {
             "hosts": "some hosts",
@@ -69,15 +75,15 @@
         # in fact, it works fine with vectors like [0.0] * 768, while cosine similarity would raise an exception
         embedding_similarity_function = "max_inner_product"
 
         store = ElasticsearchDocumentStore(
             hosts=hosts, index=index, embedding_similarity_function=embedding_similarity_function
         )
         yield store
-        store._client.options(ignore_status=[400, 404]).indices.delete(index=index)
+        store.client.options(ignore_status=[400, 404]).indices.delete(index=index)
 
     def assert_documents_are_equal(self, received: List[Document], expected: List[Document]):
         """
         The ElasticSearchDocumentStore.filter_documents() method returns a Documents with their score set.
         We don't want to compare the score, so we set it to None before comparing the documents.
         """
         received_meta = []
@@ -97,15 +103,15 @@
             expected_meta.append(r)
         for doc in received:
             doc.score = None
 
         super().assert_documents_are_equal(received, expected)
 
     def test_user_agent_header(self, document_store: ElasticsearchDocumentStore):
-        assert document_store._client._headers["user-agent"].startswith("haystack-py-ds/")
+        assert document_store.client._headers["user-agent"].startswith("haystack-py-ds/")
 
     def test_write_documents(self, document_store: ElasticsearchDocumentStore):
         docs = [Document(id="1")]
         assert document_store.write_documents(docs) == 1
         with pytest.raises(DuplicateDocumentError):
             document_store.write_documents(docs, DuplicatePolicy.FAIL)
 
@@ -304,12 +310,12 @@
             ],
         }
         mock_client = Mock(
             indices=Mock(create=Mock(), exists=Mock(return_value=False)),
         )
         mock_elasticsearch.return_value = mock_client
 
-        ElasticsearchDocumentStore(hosts="some hosts", custom_mapping=custom_mapping)
+        _ = ElasticsearchDocumentStore(hosts="some hosts", custom_mapping=custom_mapping).client
         mock_client.indices.create.assert_called_once_with(
             index="default",
             mappings=custom_mapping,
         )
```

### Comparing `elasticsearch_haystack-0.5.0/tests/test_embedding_retriever.py` & `elasticsearch_haystack-0.6.0/tests/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/tests/test_filters.py` & `elasticsearch_haystack-0.6.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/.gitignore` & `elasticsearch_haystack-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/LICENSE` & `elasticsearch_haystack-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/README.md` & `elasticsearch_haystack-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/pyproject.toml` & `elasticsearch_haystack-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.5.0/PKG-INFO` & `elasticsearch_haystack-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elasticsearch-haystack
-Version: 0.5.0
+Version: 0.6.0
 Summary: Haystack 2.x Document Store for ElasticSearch
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/elasticsearch#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/elasticsearch
 Author-email: Silvano Cerza <silvanocerza@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

