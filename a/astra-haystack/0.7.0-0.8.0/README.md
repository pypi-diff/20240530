# Comparing `tmp/astra_haystack-0.7.0.tar.gz` & `tmp/astra_haystack-0.8.0.tar.gz`

## Comparing `astra_haystack-0.7.0.tar` & `astra_haystack-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/__init__.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/example.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/pipeline_example.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/requirements.txt
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/data/usr_01.txt
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/pydoc/config.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/components/retrievers/astra/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/components/retrievers/astra/retriever.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/__init__.py
--rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/astra_client.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/document_store.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/errors.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/filters.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/tests/test_document_store.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/LICENSE
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/README.md
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/__init__.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/examples/example.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/examples/pipeline_example.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/examples/requirements.txt
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/examples/data/usr_01.txt
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/pydoc/config.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/components/retrievers/astra/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/components/retrievers/astra/retriever.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/__init__.py
+-rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/astra_client.py
+-rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/document_store.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/errors.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/filters.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/README.md
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 astra_haystack-0.8.0/PKG-INFO
```

### Comparing `astra_haystack-0.7.0/examples/example.py` & `astra_haystack-0.8.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/examples/pipeline_example.py` & `astra_haystack-0.8.0/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/examples/data/usr_01.txt` & `astra_haystack-0.8.0/examples/data/usr_01.txt`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/pydoc/config.yml` & `astra_haystack-0.8.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/src/haystack_integrations/components/retrievers/astra/retriever.py` & `astra_haystack-0.8.0/src/haystack_integrations/components/retrievers/astra/retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/astra_client.py` & `astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/astra_client.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/document_store.py` & `astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/document_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,39 +81,46 @@
         resolved_api_endpoint = api_endpoint.resolve_value()
         if resolved_api_endpoint is None:
             msg = (
                 "AstraDocumentStore expects the API endpoint. "
                 "Set the ASTRA_DB_API_ENDPOINT environment variable (recommended) or pass it explicitly."
             )
             raise ValueError(msg)
+        self.resolved_api_endpoint = resolved_api_endpoint
 
         resolved_token = token.resolve_value()
         if resolved_token is None:
             msg = (
                 "AstraDocumentStore expects an authentication token. "
                 "Set the ASTRA_DB_APPLICATION_TOKEN environment variable (recommended) or pass it explicitly."
             )
             raise ValueError(msg)
+        self.resolved_token = resolved_token
 
         self.api_endpoint = api_endpoint
         self.token = token
         self.collection_name = collection_name
         self.embedding_dimension = embedding_dimension
         self.duplicates_policy = duplicates_policy
         self.similarity = similarity
         self.namespace = namespace
+        self._index: Optional[AstraClient] = None
 
-        self.index = AstraClient(
-            resolved_api_endpoint,
-            resolved_token,
-            self.collection_name,
-            self.embedding_dimension,
-            self.similarity,
-            namespace,
-        )
+    @property
+    def index(self) -> AstraClient:
+        if self._index is None:
+            self._index = AstraClient(
+                self.resolved_api_endpoint,
+                self.resolved_token,
+                self.collection_name,
+                self.embedding_dimension,
+                self.similarity,
+                self.namespace,
+            )
+        return self._index
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "AstraDocumentStore":
         """
         Deserializes the component from a dictionary.
 
         :param data:
```

### Comparing `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/errors.py` & `astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/errors.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/filters.py` & `astra_haystack-0.8.0/src/haystack_integrations/document_stores/astra/filters.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/tests/test_document_store.py` & `astra_haystack-0.8.0/tests/test_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,27 @@
 
 @pytest.fixture
 def mock_auth(monkeypatch):
     monkeypatch.setenv("ASTRA_DB_API_ENDPOINT", "http://example.com")
     monkeypatch.setenv("ASTRA_DB_APPLICATION_TOKEN", "test_token")
 
 
+@mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB")
+def test_init_is_lazy(_mock_client, mock_auth):
+    _ = AstraDocumentStore()
+    _mock_client.assert_not_called()
+
+
 def test_namespace_init(mock_auth):  # noqa
     with mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB") as client:
-        AstraDocumentStore()
+        _ = AstraDocumentStore().index
         assert "namespace" in client.call_args.kwargs
         assert client.call_args.kwargs["namespace"] is None
 
-        AstraDocumentStore(namespace="foo")
+        _ = AstraDocumentStore(namespace="foo").index
         assert "namespace" in client.call_args.kwargs
         assert client.call_args.kwargs["namespace"] == "foo"
 
 
 def test_to_dict(mock_auth):  # noqa
     with mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB"):
         ds = AstraDocumentStore()
```

### Comparing `astra_haystack-0.7.0/tests/test_retriever.py` & `astra_haystack-0.8.0/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/.gitignore` & `astra_haystack-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/LICENSE` & `astra_haystack-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/README.md` & `astra_haystack-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/pyproject.toml` & `astra_haystack-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.7.0/PKG-INFO` & `astra_haystack-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astra-haystack
-Version: 0.7.0
+Version: 0.8.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra
 Author-email: Anant Corporation <support@anant.us>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

