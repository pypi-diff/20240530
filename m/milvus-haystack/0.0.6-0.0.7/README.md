# Comparing `tmp/milvus_haystack-0.0.6.tar.gz` & `tmp/milvus_haystack-0.0.7.tar.gz`

## Comparing `milvus_haystack-0.0.6.tar` & `milvus_haystack-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/OWNERS
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.github/mergify.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.github/workflows/main.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/__about__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/__init__.py
--rw-r--r--   0        0        0    25495 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/document_store.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/filters.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/milvus_embedding_retriever.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/test_document_store.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/test_filters.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.gitignore
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/README.md
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/OWNERS
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/.github/mergify.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/src/milvus_haystack/__about__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/src/milvus_haystack/__init__.py
+-rw-r--r--   0        0        0    25761 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/src/milvus_haystack/document_store.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/src/milvus_haystack/filters.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/src/milvus_haystack/milvus_embedding_retriever.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/tests/test_document_store.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/tests/test_filters.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/.gitignore
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/README.md
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 milvus_haystack-0.0.7/PKG-INFO
```

### Comparing `milvus_haystack-0.0.6/.github/mergify.yml` & `milvus_haystack-0.0.7/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/.github/workflows/test.yml` & `milvus_haystack-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/src/milvus_haystack/document_store.py` & `milvus_haystack-0.0.7/src/milvus_haystack/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
             from pymilvus import Collection, utility
         except ImportError as err:
             err_msg = "Could not import pymilvus python package. Please install it with `pip install pymilvus`."
             raise ValueError(err_msg) from err
 
         # Default search params when one is not provided.
         self.default_search_params = {
+            "GPU_IVF_FLAT": {"metric_type": "L2", "params": {"nprobe": 10}},
+            "GPU_IVF_PQ": {"metric_type": "L2", "params": {"nprobe": 10}},
+            "GPU_CAGRA": {"metric_type": "L2", "params": {"itopk_size": 128}},
             "IVF_FLAT": {"metric_type": "L2", "params": {"nprobe": 10}},
             "IVF_SQ8": {"metric_type": "L2", "params": {"nprobe": 10}},
             "IVF_PQ": {"metric_type": "L2", "params": {"nprobe": 10}},
             "HNSW": {"metric_type": "L2", "params": {"ef": 10}},
             "RHNSW_FLAT": {"metric_type": "L2", "params": {"ef": 10}},
             "RHNSW_SQ": {"metric_type": "L2", "params": {"ef": 10}},
             "RHNSW_PQ": {"metric_type": "L2", "params": {"ef": 10}},
@@ -319,31 +322,32 @@
                         insert_dict.setdefault(key, []).append(value)
 
         # Total insert count
         vectors: list = insert_dict[self._vector_field]
         total_count = len(vectors)
 
         batch_size = 1000
+        wrote_ids = []
         if not isinstance(self.col, Collection):
             raise MilvusException(message="Collection is not initialized")
         for i in range(0, total_count, batch_size):
             # Grab end index
             end = min(i + batch_size, total_count)
             # Convert dict to list of lists batch for insertion
             insert_list = [insert_dict[x][i:end] for x in self.fields]
             # Insert into the collection.
             try:
                 # res: Collection
                 res = self.col.insert(insert_list, timeout=None, **kwargs)
-                ids.extend(res.primary_keys)
+                wrote_ids.extend(res.primary_keys)
             except MilvusException as err:
                 logger.error("Failed to insert batch starting at entity: %s/%s", i, total_count)
                 raise err
         self.col.flush()
-        return len(ids)
+        return len(wrote_ids)
 
     def delete_documents(self, document_ids: List[str]) -> None:
         """
         Deletes all documents with a matching document_ids from the document store.
 
         :param document_ids: The object_ids to delete
         """
```

### Comparing `milvus_haystack-0.0.6/src/milvus_haystack/filters.py` & `milvus_haystack-0.0.7/src/milvus_haystack/filters.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/src/milvus_haystack/milvus_embedding_retriever.py` & `milvus_haystack-0.0.7/src/milvus_haystack/milvus_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/tests/test_document_store.py` & `milvus_haystack-0.0.7/tests/test_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,19 @@
                 "password": "",
                 "secure": False,
             },
             drop_old=True,
         )
 
     def test_write_documents(self, document_store: DocumentStore):
-        document_store.write_documents(
+        return_value = document_store.write_documents(
             [Document(content="test doc 1"), Document(content="test doc 2"), Document(content="test doc 3")]
         )
         assert document_store.count_documents() == 3
+        assert return_value == 3
 
     def test_delete_documents(self, document_store: DocumentStore):
         """
         Test delete_documents() normal behaviour.
         """
         doc = Document(content="test doc")
         document_store.write_documents([doc])
```

### Comparing `milvus_haystack-0.0.6/tests/test_embedding_retriever.py` & `milvus_haystack-0.0.7/tests/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/tests/test_filters.py` & `milvus_haystack-0.0.7/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/.gitignore` & `milvus_haystack-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/LICENSE.txt` & `milvus_haystack-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/README.md` & `milvus_haystack-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/pyproject.toml` & `milvus_haystack-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.6/PKG-INFO` & `milvus_haystack-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: milvus-haystack
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: Documentation, https://github.com/milvus-io/milvus-haystack#readme
 Project-URL: Issues, https://github.com/milvus-io/milvus-haystack/issues
 Project-URL: Source, https://github.com/milvus-io/milvus-haystack
 Author-email: Zilliz <support@zilliz.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

