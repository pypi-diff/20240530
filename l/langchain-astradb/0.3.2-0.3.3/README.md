# Comparing `tmp/langchain_astradb-0.3.2.tar.gz` & `tmp/langchain_astradb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_astradb-0.3.2.tar", max compression
+gzip compressed data, was "langchain_astradb-0.3.3.tar", max compression
```

## Comparing `langchain_astradb-0.3.2.tar` & `langchain_astradb-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/LICENSE
--rw-r--r--   0        0        0     2058 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/README.md
--rw-r--r--   0        0        0      624 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/__init__.py
--rw-r--r--   0        0        0    21179 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/cache.py
--rw-r--r--   0        0        0     5627 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/chat_message_histories.py
--rw-r--r--   0        0        0     4837 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/document_loaders.py
--rw-r--r--   0        0        0        0 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/py.typed
--rw-r--r--   0        0        0     9399 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/storage.py
--rw-r--r--   0        0        0    15826 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/utils/astradb.py
--rw-r--r--   0        0        0     3165 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/utils/mmr.py
--rw-r--r--   0        0        0    62443 2024-05-20 19:31:29.275205 langchain_astradb-0.3.2/langchain_astradb/vectorstores.py
--rw-r--r--   0        0        0     2888 2024-05-20 19:31:29.279205 langchain_astradb-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 langchain_astradb-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2058 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/README.md
+-rw-r--r--   0        0        0      624 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/langchain_astradb/__init__.py
+-rw-r--r--   0        0        0    21179 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/langchain_astradb/cache.py
+-rw-r--r--   0        0        0     5627 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/langchain_astradb/chat_message_histories.py
+-rw-r--r--   0        0        0     4837 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/langchain_astradb/document_loaders.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:50:51.866660 langchain_astradb-0.3.3/langchain_astradb/py.typed
+-rw-r--r--   0        0        0     9399 2024-05-30 10:50:51.870660 langchain_astradb-0.3.3/langchain_astradb/storage.py
+-rw-r--r--   0        0        0    16265 2024-05-30 10:50:51.870660 langchain_astradb-0.3.3/langchain_astradb/utils/astradb.py
+-rw-r--r--   0        0        0     3165 2024-05-30 10:50:51.870660 langchain_astradb-0.3.3/langchain_astradb/utils/mmr.py
+-rw-r--r--   0        0        0    63485 2024-05-30 10:50:51.870660 langchain_astradb-0.3.3/langchain_astradb/vectorstores.py
+-rw-r--r--   0        0        0     2890 2024-05-30 10:50:51.870660 langchain_astradb-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 langchain_astradb-0.3.3/PKG-INFO
```

### Comparing `langchain_astradb-0.3.2/LICENSE` & `langchain_astradb-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/README.md` & `langchain_astradb-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/__init__.py` & `langchain_astradb-0.3.3/langchain_astradb/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/cache.py` & `langchain_astradb-0.3.3/langchain_astradb/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/chat_message_histories.py` & `langchain_astradb-0.3.3/langchain_astradb/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/document_loaders.py` & `langchain_astradb-0.3.3/langchain_astradb/document_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/storage.py` & `langchain_astradb-0.3.3/langchain_astradb/storage.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/utils/astradb.py` & `langchain_astradb-0.3.3/langchain_astradb/utils/astradb.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from astrapy.db import AstraDB, AstraDBCollection, AsyncAstraDB, AsyncAstraDBCollection
 from astrapy.info import CollectionVectorServiceOptions
 
 TOKEN_ENV_VAR = "ASTRA_DB_APPLICATION_TOKEN"
 API_ENDPOINT_ENV_VAR = "ASTRA_DB_API_ENDPOINT"
 NAMESPACE_ENV_VAR = "ASTRA_DB_KEYSPACE"
 
+DEFAULT_VECTORIZE_SECRET_HEADER = "x-embedding-api-key"
+
 logger = logging.getLogger()
 
 
 class SetupMode(Enum):
     SYNC = 1
     ASYNC = 2
     OFF = 3
@@ -134,27 +136,37 @@
         embedding_dimension: Union[int, Awaitable[int], None] = None,
         metric: Optional[str] = None,
         requested_indexing_policy: Optional[Dict[str, Any]] = None,
         default_indexing_policy: Optional[Dict[str, Any]] = None,
         collection_vector_service_options: Optional[
             CollectionVectorServiceOptions
         ] = None,
+        collection_embedding_api_key: Optional[str] = None,
     ) -> None:
         super().__init__(
             token, api_endpoint, astra_db_client, async_astra_db_client, namespace
         )
+        embedding_key_header = {
+            k: v
+            for k, v in {
+                DEFAULT_VECTORIZE_SECRET_HEADER: collection_embedding_api_key,
+            }.items()
+            if v is not None
+        }
         self.collection_name = collection_name
         self.collection = AstraDBCollection(
             collection_name=collection_name,
             astra_db=self.astra_db,
+            additional_headers=embedding_key_header,
         )
 
         self.async_collection = AsyncAstraDBCollection(
             collection_name=collection_name,
             astra_db=self.async_astra_db,
+            additional_headers=embedding_key_header,
         )
 
         if requested_indexing_policy is not None:
             _options = {"indexing": requested_indexing_policy}
         else:
             _options = None
```

### Comparing `langchain_astradb-0.3.2/langchain_astradb/utils/mmr.py` & `langchain_astradb-0.3.3/langchain_astradb/utils/mmr.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.2/langchain_astradb/vectorstores.py` & `langchain_astradb-0.3.3/langchain_astradb/vectorstores.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         pre_delete_collection: bool = False,
         metadata_indexing_include: Optional[Iterable[str]] = None,
         metadata_indexing_exclude: Optional[Iterable[str]] = None,
         collection_indexing_policy: Optional[Dict[str, Any]] = None,
         collection_vector_service_options: Optional[
             CollectionVectorServiceOptions
         ] = None,
+        collection_embedding_api_key: Optional[str] = None,
     ) -> None:
         """Wrapper around DataStax Astra DB for vector-store workloads.
 
         For quickstart and details, visit
         https://docs.datastax.com/en/astra/astra-db-vector/
 
         Example:
@@ -177,16 +178,17 @@
 
                 vectorstore.add_texts(["Giraffes", "All good here"])
                 results = vectorstore.similarity_search("Everything's ok", k=1)
 
         Args:
             embedding: the embeddings function or service to use.
                 This enables client-side embedding functions or calls to external
-                embedding providers. Only one of `embedding` or
-                `collection_vector_service_options` can be provided.
+                embedding providers. If `embedding` is provided, arguments
+                `collection_vector_service_options` and
+                `collection_embedding_api_key` cannot be provided.
             collection_name: name of the Astra DB collection to create/use.
             token: API token for Astra DB usage. If not provided, the environment
                 variable ASTRA_DB_APPLICATION_TOKEN is inspected.
             api_endpoint: full URL to the API endpoint, such as
                 `https://<DB-ID>-us-east1.apps.astra.datastax.com`. If not provided,
                 the environment variable ASTRA_DB_API_ENDPOINT is inspected.
             astra_db_client: *alternative to token+api_endpoint*,
@@ -216,18 +218,24 @@
                 that should not be indexed for later filtering in searches.
             collection_indexing_policy: a full "indexing" specification for
                 what fields should be indexed for later filtering in searches.
                 This dict must conform to to the API specifications
                 (see docs.datastax.com/en/astra/astra-db-vector/api-reference/
                 data-api-commands.html#advanced-feature-indexing-clause-on-createcollection)
             collection_vector_service_options: specifies the use of server-side
-                embeddings within Astra DB. Only one of `embedding` or
-                `collection_vector_service_options` can be provided.
-                NOTE: This feature is under current development.
-
+                embeddings within Astra DB. If passing this parameter, `embedding`
+                cannot be provided.
+            collection_embedding_api_key: for usage of server-side embeddings
+                within Astra DB, with this parameter one can supply an API Key
+                that will be passed to Astra DB with each data request.
+                This is useful when the service is configured for the collection,
+                but no corresponding secret is stored within
+                Astra's key management system.
+                This parameter cannot be provided without
+                specifying `collection_vector_service_options`.
 
         Note:
             For concurrency in synchronous :meth:`~add_texts`:, as a rule of thumb, on a
             typical client machine it is suggested to keep the quantity
             bulk_insert_batch_concurrency * bulk_insert_overwrite_concurrency
             much below 1000 to avoid exhausting the client multithreading/networking
             resources. The hardcoded defaults are somewhat conservative to meet
@@ -238,35 +246,45 @@
 
             A bit of experimentation is required to nail the best results here,
             depending on both the machine/network specs and the expected workload
             (specifically, how often a write is an update of an existing id).
             Remember you can pass concurrency settings to individual calls to
             :meth:`~add_texts` and :meth:`~add_documents` as well.
         """
-        # Embedding and collection_vector_service_options are mutually exclusive,
+        # Embedding and the server-side embeddings are mutually exclusive,
         # as both specify how to produce embeddings
         if embedding is None and collection_vector_service_options is None:
             raise ValueError(
                 "Either an `embedding` or a `collection_vector_service_options`\
                     must be provided."
             )
 
         if embedding is not None and collection_vector_service_options is not None:
             raise ValueError(
                 "Only one of `embedding` or `collection_vector_service_options`\
                     can be provided."
             )
 
+        if (
+            collection_vector_service_options is None
+            and collection_embedding_api_key is not None
+        ):
+            raise ValueError(
+                "`collection_embedding_api_key` cannot be provided unless"
+                " `collection_vector_service_options` is also passed."
+            )
+
         self.embedding_dimension: Optional[int] = None
         self.embedding = embedding
         self.collection_name = collection_name
         self.token = token
         self.api_endpoint = api_endpoint
         self.namespace = namespace
         self.collection_vector_service_options = collection_vector_service_options
+        self.collection_embedding_api_key = collection_embedding_api_key
         # Concurrency settings
         self.batch_size: int = batch_size or DEFAULT_BATCH_SIZE
         self.bulk_insert_batch_concurrency: int = (
             bulk_insert_batch_concurrency or DEFAULT_BULK_INSERT_BATCH_CONCURRENCY
         )
         self.bulk_insert_overwrite_concurrency: int = (
             bulk_insert_overwrite_concurrency
@@ -301,14 +319,15 @@
             setup_mode=setup_mode,
             pre_delete_collection=pre_delete_collection,
             embedding_dimension=embedding_dimension,
             metric=metric,
             requested_indexing_policy=self.indexing_policy,
             default_indexing_policy=DEFAULT_INDEXING_OPTIONS,
             collection_vector_service_options=collection_vector_service_options,
+            collection_embedding_api_key=collection_embedding_api_key,
         )
         self.astra_db = self.astra_env.astra_db
         self.async_astra_db = self.astra_env.async_astra_db
         self.collection = self.astra_env.collection
         self.async_collection = self.astra_env.async_collection
 
     def _get_embedding_dimension(self) -> int:
```

### Comparing `langchain_astradb-0.3.2/pyproject.toml` & `langchain_astradb-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-astradb"
-version = "0.3.2"
+version = "0.3.3"
 description = "An integration package connecting Astra DB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-datastax"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-datastax/tree/main/libs/astradb"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = ">=0.1.31,<0.3"
-astrapy = "^1"
+astrapy = "^1.2"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_astradb-0.3.2/PKG-INFO` & `langchain_astradb-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-astradb
-Version: 0.3.2
+Version: 0.3.3
 Summary: An integration package connecting Astra DB and LangChain
 Home-page: https://github.com/langchain-ai/langchain-datastax
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: astrapy (>=1,<2)
+Requires-Dist: astrapy (>=1.2,<2.0)
 Requires-Dist: langchain-core (>=0.1.31,<0.3)
 Requires-Dist: numpy (>=1,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-datastax
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-datastax/tree/main/libs/astradb
 Description-Content-Type: text/markdown
 
 # langchain-astradb
```

