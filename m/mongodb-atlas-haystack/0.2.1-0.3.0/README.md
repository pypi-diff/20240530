# Comparing `tmp/mongodb_atlas_haystack-0.2.1.tar.gz` & `tmp/mongodb_atlas_haystack-0.3.0.tar.gz`

## Comparing `mongodb_atlas_haystack-0.2.1.tar` & `mongodb_atlas_haystack-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/examples/example.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/pydoc/config.yml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/components/retrievers/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    12792 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/test_document_store.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/test_embedding_retrieval.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/README.md
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/examples/example.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/pydoc/config.yml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/src/haystack_integrations/components/retrievers/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/src/haystack_integrations/document_stores/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/src/haystack_integrations/document_stores/mongodb_atlas/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/tests/test_embedding_retrieval.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/README.md
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 mongodb_atlas_haystack-0.3.0/PKG-INFO
```

### Comparing `mongodb_atlas_haystack-0.2.1/examples/example.py` & `mongodb_atlas_haystack-0.3.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/pydoc/config.yml` & `mongodb_atlas_haystack-0.3.0/pydoc/config.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: MongoDB Atlas integration for Haystack
   category_slug: integrations-api
   title: MongoDB Atlas
   slug: integrations-mongodb-atlas
   order: 160
   markdown:
     descriptive_class_title: false
```

### Comparing `mongodb_atlas_haystack-0.2.1/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py` & `mongodb_atlas_haystack-0.3.0/src/haystack_integrations/components/retrievers/mongodb_atlas/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py` & `mongodb_atlas_haystack-0.3.0/src/haystack_integrations/document_stores/mongodb_atlas/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from haystack import default_from_dict, default_to_dict
 from haystack.dataclasses.document import Document
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.utils import Secret, deserialize_secrets_inplace
 from haystack_integrations.document_stores.mongodb_atlas.filters import _normalize_filters
 from pymongo import InsertOne, MongoClient, ReplaceOne, UpdateOne
+from pymongo.collection import Collection
 from pymongo.driver_info import DriverInfo
 from pymongo.errors import BulkWriteError
 
 logger = logging.getLogger(__name__)
 
 
 class MongoDBAtlasDocumentStore:
@@ -77,30 +78,42 @@
 
         :raises ValueError: If the collection name contains invalid characters.
         """
         if collection_name and not bool(re.match(r"^[a-zA-Z0-9\-_]+$", collection_name)):
             msg = f'Invalid collection name: "{collection_name}". It can only contain letters, numbers, -, or _.'
             raise ValueError(msg)
 
-        resolved_connection_string = mongo_connection_string.resolve_value()
+        self.resolved_connection_string = mongo_connection_string.resolve_value()
         self.mongo_connection_string = mongo_connection_string
 
         self.database_name = database_name
         self.collection_name = collection_name
         self.vector_search_index = vector_search_index
+        self._connection: Optional[MongoClient] = None
+        self._collection: Optional[Collection] = None
 
-        self.connection: MongoClient = MongoClient(
-            resolved_connection_string, driver=DriverInfo(name="MongoDBAtlasHaystackIntegration")
-        )
-        database = self.connection[self.database_name]
+    @property
+    def connection(self) -> MongoClient:
+        if self._connection is None:
+            self._connection = MongoClient(
+                self.resolved_connection_string, driver=DriverInfo(name="MongoDBAtlasHaystackIntegration")
+            )
+
+        return self._connection
+
+    @property
+    def collection(self) -> Collection:
+        if self._collection is None:
+            database = self.connection[self.database_name]
 
-        if collection_name not in database.list_collection_names():
-            msg = f"Collection '{collection_name}' does not exist in database '{database_name}'."
-            raise ValueError(msg)
-        self.collection = database[self.collection_name]
+            if self.collection_name not in database.list_collection_names():
+                msg = f"Collection '{self.collection_name}' does not exist in database '{self.database_name}'."
+                raise ValueError(msg)
+            self._collection = database[self.collection_name]
+        return self._collection
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
@@ -229,15 +242,15 @@
         :raises ValueError: If `query_embedding` is empty.
         :raises DocumentStoreError: If the retrieval of documents from MongoDB Atlas fails.
         """
         if not query_embedding:
             msg = "Query embedding must not be empty"
             raise ValueError(msg)
 
-        filters = _normalize_filters(filters) if filters else None
+        filters = _normalize_filters(filters) if filters else {}
 
         pipeline = [
             {
                 "$vectorSearch": {
                     "index": self.vector_search_index,
                     "path": "embedding",
                     "queryVector": query_embedding,
```

### Comparing `mongodb_atlas_haystack-0.2.1/src/haystack_integrations/document_stores/mongodb_atlas/filters.py` & `mongodb_atlas_haystack-0.3.0/src/haystack_integrations/document_stores/mongodb_atlas/filters.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/tests/test_document_store.py` & `mongodb_atlas_haystack-0.3.0/tests/test_document_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
+from unittest.mock import patch
 from uuid import uuid4
 
 import pytest
 from haystack.dataclasses.document import ByteStream, Document
 from haystack.document_stores.errors import DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 from haystack.utils import Secret
 from haystack_integrations.document_stores.mongodb_atlas import MongoDBAtlasDocumentStore
 from pandas import DataFrame
 from pymongo import MongoClient
 from pymongo.driver_info import DriverInfo
 
 
+@patch("haystack_integrations.document_stores.mongodb_atlas.document_store.MongoClient")
+def test_init_is_lazy(_mock_client):
+    MongoDBAtlasDocumentStore(
+        mongo_connection_string=Secret.from_token("test"),
+        database_name="database_name",
+        collection_name="collection_name",
+        vector_search_index="cosine_index",
+    )
+    _mock_client.assert_not_called()
+
+
 @pytest.mark.skipif(
     "MONGO_CONNECTION_STRING" not in os.environ,
     reason="No MongoDB Atlas connection string provided",
 )
 @pytest.mark.integration
 class TestDocumentStore(DocumentStoreBaseTests):
-
     @pytest.fixture
     def document_store(self):
         database_name = "haystack_integration_test"
         collection_name = "test_collection_" + str(uuid4())
 
         connection: MongoClient = MongoClient(
             os.environ["MONGO_CONNECTION_STRING"], driver=DriverInfo(name="MongoDBAtlasHaystackIntegration")
```

### Comparing `mongodb_atlas_haystack-0.2.1/tests/test_embedding_retrieval.py` & `mongodb_atlas_haystack-0.3.0/tests/test_embedding_retrieval.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/tests/test_retriever.py` & `mongodb_atlas_haystack-0.3.0/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/.gitignore` & `mongodb_atlas_haystack-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/LICENSE.txt` & `mongodb_atlas_haystack-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/README.md` & `mongodb_atlas_haystack-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_atlas_haystack-0.2.1/pyproject.toml` & `mongodb_atlas_haystack-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "deepset GmbH", email = "info@deepset.ai" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
@@ -46,15 +47,15 @@
 git_describe_command = 'git describe --tags --match="integrations/mongodb_atlas-v[0-9]*"'
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "ipython",
-  "haystack-pydoc-tools",  
+  "haystack-pydoc-tools",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `mongodb_atlas_haystack-0.2.1/PKG-INFO` & `mongodb_atlas_haystack-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: mongodb-atlas-haystack
-Version: 0.2.1
+Version: 0.3.0
 Summary: An integration of MongoDB Atlas with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/mongodb_atlas/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

