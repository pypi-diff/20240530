# Comparing `tmp/dashvector-1.0.8.tar.gz` & `tmp/dashvector-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashvector-1.0.8.tar", max compression
+gzip compressed data, was "dashvector-1.0.9.tar", max compression
```

## Comparing `dashvector-1.0.8.tar` & `dashvector-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    12090 2023-07-12 09:23:56.995297 dashvector-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0    18480 2023-12-05 11:16:14.250198 dashvector-1.0.8/README.md
--rw-r--r--   0        0        0     1268 2023-12-05 11:16:14.252482 dashvector-1.0.8/dashvector/__init__.py
--rw-r--r--   0        0        0      671 2023-08-10 02:25:04.035974 dashvector-1.0.8/dashvector/common/__init__.py
--rw-r--r--   0        0        0     1320 2023-12-05 11:16:14.254397 dashvector-1.0.8/dashvector/common/constants.py
--rw-r--r--   0        0        0     3926 2023-12-05 11:16:14.255162 dashvector-1.0.8/dashvector/common/error.py
--rw-r--r--   0        0        0     6057 2023-12-05 11:16:14.255896 dashvector-1.0.8/dashvector/common/handler.py
--rw-r--r--   0        0        0     1671 2023-12-05 11:16:14.257151 dashvector-1.0.8/dashvector/common/logging.py
--rw-r--r--   0        0        0     2007 2023-12-05 11:16:14.258605 dashvector-1.0.8/dashvector/common/status.py
--rw-r--r--   0        0        0    14733 2023-12-05 11:16:14.260528 dashvector-1.0.8/dashvector/common/types.py
--rw-r--r--   0        0        0      671 2023-08-10 02:25:04.041375 dashvector-1.0.8/dashvector/core/__init__.py
--rw-r--r--   0        0        0    14940 2023-12-05 11:16:14.261731 dashvector-1.0.8/dashvector/core/client.py
--rw-r--r--   0        0        0    28311 2023-12-05 11:16:14.263944 dashvector-1.0.8/dashvector/core/collection.py
--rw-r--r--   0        0        0     7083 2023-12-05 11:16:14.265127 dashvector-1.0.8/dashvector/core/doc.py
--rw-r--r--   0        0        0      671 2023-08-10 02:25:04.044202 dashvector-1.0.8/dashvector/core/handler/__init__.py
--rw-r--r--   0        0        0    15940 2023-12-05 11:16:14.265979 dashvector-1.0.8/dashvector/core/handler/grpc_handler.py
--rw-r--r--   0        0        0    17306 2023-12-05 11:16:14.266835 dashvector-1.0.8/dashvector/core/handler/http_handler.py
--rw-r--r--   0        0        0      671 2023-08-10 02:25:04.046685 dashvector-1.0.8/dashvector/core/models/__init__.py
--rw-r--r--   0        0        0     6619 2023-12-05 11:16:14.267649 dashvector-1.0.8/dashvector/core/models/collection_meta_status.py
--rw-r--r--   0        0        0     7450 2023-12-05 11:16:14.269150 dashvector-1.0.8/dashvector/core/models/create_collection_request.py
--rw-r--r--   0        0        0     2339 2023-12-05 11:16:14.270126 dashvector-1.0.8/dashvector/core/models/create_partition_request.py
--rw-r--r--   0        0        0     1951 2023-12-05 11:16:14.270768 dashvector-1.0.8/dashvector/core/models/delete_collection_request.py
--rw-r--r--   0        0        0     5058 2023-12-05 11:16:14.271873 dashvector-1.0.8/dashvector/core/models/delete_doc_request.py
--rw-r--r--   0        0        0     2275 2023-12-05 11:16:14.272634 dashvector-1.0.8/dashvector/core/models/delete_partition_request.py
--rw-r--r--   0        0        0     1965 2023-12-05 11:16:14.273373 dashvector-1.0.8/dashvector/core/models/describe_collection_request.py
--rw-r--r--   0        0        0     2287 2023-12-05 11:16:14.274437 dashvector-1.0.8/dashvector/core/models/describe_partition_request.py
--rw-r--r--   0        0        0     4692 2023-12-05 11:16:14.275137 dashvector-1.0.8/dashvector/core/models/fetch_doc_request.py
--rw-r--r--   0        0        0     1020 2023-08-10 02:25:04.052985 dashvector-1.0.8/dashvector/core/models/get_version_request.py
--rw-r--r--   0        0        0     1029 2023-08-10 02:25:04.053587 dashvector-1.0.8/dashvector/core/models/list_collections_request.py
--rw-r--r--   0        0        0     2131 2023-12-05 11:16:14.275739 dashvector-1.0.8/dashvector/core/models/list_partitions_request.py
--rw-r--r--   0        0        0     1662 2023-12-05 11:16:14.276655 dashvector-1.0.8/dashvector/core/models/partition_meta_status.py
--rw-r--r--   0        0        0    12803 2023-12-05 11:16:14.277884 dashvector-1.0.8/dashvector/core/models/query_doc_request.py
--rw-r--r--   0        0        0     1929 2023-12-05 11:16:14.278918 dashvector-1.0.8/dashvector/core/models/stats_collection_request.py
--rw-r--r--   0        0        0     2271 2023-12-05 11:16:14.280401 dashvector-1.0.8/dashvector/core/models/stats_partition_request.py
--rw-r--r--   0        0        0    16547 2023-12-05 11:16:14.281141 dashvector-1.0.8/dashvector/core/models/upsert_doc_request.py
--rw-r--r--   0        0        0      671 2023-08-10 02:25:04.057160 dashvector-1.0.8/dashvector/core/proto/__init__.py
--rw-r--r--   0        0        0    42212 2023-12-05 11:16:14.282398 dashvector-1.0.8/dashvector/core/proto/dashvector_pb2.py
--rw-r--r--   0        0        0    28800 2023-12-05 11:16:14.283223 dashvector-1.0.8/dashvector/core/proto/dashvector_pb2_grpc.py
--rw-r--r--   0        0        0      671 2023-12-05 11:16:14.283934 dashvector-1.0.8/dashvector/util/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-05 11:16:14.284502 dashvector-1.0.8/dashvector/util/validator.py
--rw-r--r--   0        0        0      760 2023-12-05 11:16:14.285476 dashvector-1.0.8/dashvector/version.py
--rw-r--r--   0        0        0     1999 2023-12-06 12:05:03.544867 dashvector-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    19970 1970-01-01 00:00:00.000000 dashvector-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    12090 2023-07-12 09:23:56.995297 dashvector-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0    18480 2023-12-05 11:16:14.250198 dashvector-1.0.9/README.md
+-rw-r--r--   0        0        0     1268 2023-12-05 11:16:14.252482 dashvector-1.0.9/dashvector/__init__.py
+-rw-r--r--   0        0        0      671 2023-08-10 02:25:04.035974 dashvector-1.0.9/dashvector/common/__init__.py
+-rw-r--r--   0        0        0     1320 2023-12-05 11:16:14.254397 dashvector-1.0.9/dashvector/common/constants.py
+-rw-r--r--   0        0        0     3959 2023-12-15 06:56:50.858122 dashvector-1.0.9/dashvector/common/error.py
+-rw-r--r--   0        0        0     6057 2023-12-14 08:15:04.885729 dashvector-1.0.9/dashvector/common/handler.py
+-rw-r--r--   0        0        0     1671 2023-12-05 11:16:14.257151 dashvector-1.0.9/dashvector/common/logging.py
+-rw-r--r--   0        0        0     2007 2023-12-05 11:16:14.258605 dashvector-1.0.9/dashvector/common/status.py
+-rw-r--r--   0        0        0    14733 2023-12-05 11:16:14.260528 dashvector-1.0.9/dashvector/common/types.py
+-rw-r--r--   0        0        0      671 2023-08-10 02:25:04.041375 dashvector-1.0.9/dashvector/core/__init__.py
+-rw-r--r--   0        0        0    14940 2023-12-05 11:16:14.261731 dashvector-1.0.9/dashvector/core/client.py
+-rw-r--r--   0        0        0    28311 2023-12-07 03:24:27.810621 dashvector-1.0.9/dashvector/core/collection.py
+-rw-r--r--   0        0        0     7083 2023-12-05 11:16:14.265127 dashvector-1.0.9/dashvector/core/doc.py
+-rw-r--r--   0        0        0      671 2023-08-10 02:25:04.044202 dashvector-1.0.9/dashvector/core/handler/__init__.py
+-rw-r--r--   0        0        0    15940 2023-12-05 11:16:14.265979 dashvector-1.0.9/dashvector/core/handler/grpc_handler.py
+-rw-r--r--   0        0        0    17306 2023-12-05 11:16:14.266835 dashvector-1.0.9/dashvector/core/handler/http_handler.py
+-rw-r--r--   0        0        0      671 2023-08-10 02:25:04.046685 dashvector-1.0.9/dashvector/core/models/__init__.py
+-rw-r--r--   0        0        0     6619 2023-12-05 11:16:14.267649 dashvector-1.0.9/dashvector/core/models/collection_meta_status.py
+-rw-r--r--   0        0        0     7450 2023-12-05 11:16:14.269150 dashvector-1.0.9/dashvector/core/models/create_collection_request.py
+-rw-r--r--   0        0        0     2339 2023-12-05 11:16:14.270126 dashvector-1.0.9/dashvector/core/models/create_partition_request.py
+-rw-r--r--   0        0        0     1951 2023-12-05 11:16:14.270768 dashvector-1.0.9/dashvector/core/models/delete_collection_request.py
+-rw-r--r--   0        0        0     5058 2023-12-05 11:16:14.271873 dashvector-1.0.9/dashvector/core/models/delete_doc_request.py
+-rw-r--r--   0        0        0     2275 2023-12-05 11:16:14.272634 dashvector-1.0.9/dashvector/core/models/delete_partition_request.py
+-rw-r--r--   0        0        0     1965 2023-12-05 11:16:14.273373 dashvector-1.0.9/dashvector/core/models/describe_collection_request.py
+-rw-r--r--   0        0        0     2287 2023-12-05 11:16:14.274437 dashvector-1.0.9/dashvector/core/models/describe_partition_request.py
+-rw-r--r--   0        0        0     4692 2023-12-05 11:16:14.275137 dashvector-1.0.9/dashvector/core/models/fetch_doc_request.py
+-rw-r--r--   0        0        0     1020 2023-08-10 02:25:04.052985 dashvector-1.0.9/dashvector/core/models/get_version_request.py
+-rw-r--r--   0        0        0     1029 2023-08-10 02:25:04.053587 dashvector-1.0.9/dashvector/core/models/list_collections_request.py
+-rw-r--r--   0        0        0     2131 2023-12-05 11:16:14.275739 dashvector-1.0.9/dashvector/core/models/list_partitions_request.py
+-rw-r--r--   0        0        0     1662 2023-12-05 11:16:14.276655 dashvector-1.0.9/dashvector/core/models/partition_meta_status.py
+-rw-r--r--   0        0        0    12209 2023-12-15 06:56:50.859086 dashvector-1.0.9/dashvector/core/models/query_doc_request.py
+-rw-r--r--   0        0        0     1929 2023-12-05 11:16:14.278918 dashvector-1.0.9/dashvector/core/models/stats_collection_request.py
+-rw-r--r--   0        0        0     2271 2023-12-05 11:16:14.280401 dashvector-1.0.9/dashvector/core/models/stats_partition_request.py
+-rw-r--r--   0        0        0    16000 2023-12-15 06:56:50.860001 dashvector-1.0.9/dashvector/core/models/upsert_doc_request.py
+-rw-r--r--   0        0        0      671 2023-08-10 02:25:04.057160 dashvector-1.0.9/dashvector/core/proto/__init__.py
+-rw-r--r--   0        0        0    42212 2023-12-05 11:16:14.282398 dashvector-1.0.9/dashvector/core/proto/dashvector_pb2.py
+-rw-r--r--   0        0        0    28800 2023-12-05 11:16:14.283223 dashvector-1.0.9/dashvector/core/proto/dashvector_pb2_grpc.py
+-rw-r--r--   0        0        0      671 2023-12-05 11:16:14.283934 dashvector-1.0.9/dashvector/util/__init__.py
+-rw-r--r--   0        0        0     1017 2023-12-15 06:56:50.860818 dashvector-1.0.9/dashvector/util/convertor.py
+-rw-r--r--   0        0        0     2475 2023-12-15 06:56:50.861702 dashvector-1.0.9/dashvector/util/validator.py
+-rw-r--r--   0        0        0      760 2023-12-05 11:16:14.285476 dashvector-1.0.9/dashvector/version.py
+-rw-r--r--   0        0        0     1999 2023-12-15 07:03:45.569540 dashvector-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    19970 1970-01-01 00:00:00.000000 dashvector-1.0.9/PKG-INFO
```

### Comparing `dashvector-1.0.8/LICENSE.txt` & `dashvector-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/README.md` & `dashvector-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/__init__.py` & `dashvector-1.0.9/dashvector/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/common/__init__.py` & `dashvector-1.0.9/dashvector/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/common/constants.py` & `dashvector-1.0.9/dashvector/common/constants.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/common/error.py` & `dashvector-1.0.9/dashvector/common/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     InvalidTopk = -2041
     InvalidCollectionName = -2042
     InvalidPartitionName = -2043
     InvalidFieldName = -2044
     InvalidChannelCount = -2045
     InvalidReplicaCount = -2046
     InvalidJson = -2047
+    InvalidSparseIndices = -2951
     InvalidEndpoint = -2952
     ExceedIdsLimit = -2967
     InvalidVectorType = -2968
     ExceedRequestSize = -2970
     ExistVectorAndId = -2973
     InvalidArgument = -2999
```

### Comparing `dashvector-1.0.8/dashvector/common/handler.py` & `dashvector-1.0.9/dashvector/common/handler.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/common/logging.py` & `dashvector-1.0.9/dashvector/common/logging.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/common/status.py` & `dashvector-1.0.9/dashvector/common/status.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/common/types.py` & `dashvector-1.0.9/dashvector/common/types.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/__init__.py` & `dashvector-1.0.9/dashvector/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/client.py` & `dashvector-1.0.9/dashvector/core/client.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/collection.py` & `dashvector-1.0.9/dashvector/core/collection.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/doc.py` & `dashvector-1.0.9/dashvector/core/doc.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/handler/__init__.py` & `dashvector-1.0.9/dashvector/core/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/handler/grpc_handler.py` & `dashvector-1.0.9/dashvector/core/handler/grpc_handler.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/handler/http_handler.py` & `dashvector-1.0.9/dashvector/core/handler/http_handler.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/__init__.py` & `dashvector-1.0.9/dashvector/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/collection_meta_status.py` & `dashvector-1.0.9/dashvector/core/models/collection_meta_status.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/create_collection_request.py` & `dashvector-1.0.9/dashvector/core/models/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/create_partition_request.py` & `dashvector-1.0.9/dashvector/core/models/create_partition_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/delete_collection_request.py` & `dashvector-1.0.9/dashvector/core/models/delete_collection_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/delete_doc_request.py` & `dashvector-1.0.9/dashvector/core/models/delete_doc_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/delete_partition_request.py` & `dashvector-1.0.9/dashvector/core/models/delete_partition_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/describe_collection_request.py` & `dashvector-1.0.9/dashvector/core/models/describe_collection_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/describe_partition_request.py` & `dashvector-1.0.9/dashvector/core/models/describe_partition_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/fetch_doc_request.py` & `dashvector-1.0.9/dashvector/core/models/fetch_doc_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/get_version_request.py` & `dashvector-1.0.9/dashvector/core/models/get_version_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/list_collections_request.py` & `dashvector-1.0.9/dashvector/core/models/list_collections_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/list_partitions_request.py` & `dashvector-1.0.9/dashvector/core/models/list_partitions_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/partition_meta_status.py` & `dashvector-1.0.9/dashvector/core/models/partition_meta_status.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/query_doc_request.py` & `dashvector-1.0.9/dashvector/core/models/query_doc_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import re
 
 from dashvector.common.constants import *
 from dashvector.common.handler import RPCRequest
 from dashvector.common.types import *
 from dashvector.core.models.collection_meta_status import CollectionMeta
 from dashvector.core.proto import dashvector_pb2
+from dashvector.util.convertor import to_sorted_sparse_vector
 
 
 class QueryDocRequest(RPCRequest):
     def __init__(
         self,
         *,
         collection_meta: CollectionMeta,
@@ -232,25 +233,15 @@
         self._sparse_vector = sparse_vector
         if self._sparse_vector is not None:
             if self._metric != MetricStrType.DOTPRODUCT:
                 raise DashVectorException(
                     code=DashVectorCode.InvalidSparseValues,
                     reason=f"DashVectorSDK supports query with sparse_vector only collection metric is dotproduct",
                 )
-            if not isinstance(self._sparse_vector, dict):
-                raise DashVectorException(
-                    code=DashVectorCode.InvalidArgument,
-                    reason=f"DashVectorSDK QueryDocRequest sparse_vector type({type(sparse_vector)}) is invalid and must be Dict[int, float]",
-                )
-            for key, value in sorted(self._sparse_vector.items()):
-                if not isinstance(key, int) or not isinstance(value, float):
-                    raise DashVectorException(
-                        code=DashVectorCode.InvalidArgument,
-                        reason=f"DashVectorSDK QueryDocRequest sparse_vector type({type(sparse_vector)}) is invalid and must be Dict[int, float]",
-                    )
+            for key, value in to_sorted_sparse_vector(self._sparse_vector).items():
                 query_request.sparse_vector[key] = value
         super().__init__(request=query_request)
 
     @property
     def collection_meta(self):
         return self._collection_meta
```

### Comparing `dashvector-1.0.8/dashvector/core/models/stats_collection_request.py` & `dashvector-1.0.9/dashvector/core/models/stats_collection_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/stats_partition_request.py` & `dashvector-1.0.9/dashvector/core/models/stats_partition_request.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/models/upsert_doc_request.py` & `dashvector-1.0.9/dashvector/core/models/upsert_doc_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from dashvector.common.constants import *
 from dashvector.common.handler import RPCRequest
 from dashvector.common.types import *
 from dashvector.core.doc import Doc, DocBuilder
 from dashvector.core.models.collection_meta_status import CollectionMeta
 from dashvector.core.proto import dashvector_pb2
+from dashvector.util.convertor import to_sorted_sparse_vector
 
 
 class UpsertDocRequest(RPCRequest):
     def __init__(
         self,
         *,
         collection_meta: CollectionMeta,
@@ -200,35 +201,23 @@
                         fvalue.bool_value = filed_value
                     elif ftype == FieldType.FLOAT:
                         fvalue.float_value = filed_value
                     elif ftype == FieldType.INT:
                         fvalue.int_value = filed_value
                     elif ftype == FieldType.STRING:
                         fvalue.string_value = filed_value
-
             # doc sparse_vector
             if sparse_vector is not None:
                 if self._metric != MetricStrType.DOTPRODUCT:
                     raise DashVectorException(
                         code=DashVectorCode.InvalidSparseValues,
                         reason=f"DashVectorSDK supports doc with sparse_vector only collection metric is dotproduct",
                     )
-                if not isinstance(sparse_vector, dict):
-                    raise DashVectorException(
-                        code=DashVectorCode.InvalidSparseValues,
-                        reason=f"DashVectorSDK UpsertDocRequest sparse_vector ({sparse_vector}) in invalid and must be Dict[int, float]",
-                    )
-                for key, value in sorted(sparse_vector.items()):
-                    if not isinstance(key, int) or not isinstance(value, float):
-                        raise DashVectorException(
-                            code=DashVectorCode.InvalidSparseValues,
-                            reason=f"DashVectorSDK QueryDocRequest sparse_vector Type({type(sparse_vector)}) is Invalid and must be Dict[int, float]",
-                        )
+                for key, value in sparse_vector.items():
                     new_doc.sparse_vector[key] = value
-
             self._docs.append(DocBuilder.from_pb(new_doc, collection_meta=collection_meta).__dict__())
 
         super().__init__(request=upsert_request)
 
     def _format_input(self, *, doc: Optional[Doc] = None, tup: Optional[Tuple] = None):
         if doc is not None:
             return doc.id, doc.vector, doc.fields, doc.sparse_vector
@@ -308,16 +297,16 @@
 
         # check sparse_vector
         if batch_size != len(sparse_vector_list):
             raise DashVectorException(
                 code=DashVectorCode.InvalidBatchSize,
                 reason=f"DashVectorSDK UpsertDocRequest batch size({batch_size}) is different between id and sparse_vector",
             )
-
-        return id_list, vector_list, fields_list, sparse_vector_list
+        sort_sparse_lists = [to_sorted_sparse_vector(sparse_vector) for sparse_vector in sparse_vector_list]
+        return id_list, vector_list, fields_list, sort_sparse_lists
 
     def _vector_to_pb(self, vector: VectorValueType):
         if isinstance(vector, list):
             if len(vector) != self._dimension:
                 raise DashVectorException(
                     code=DashVectorCode.MismatchedDimension,
                     reason=f"DashVectorSDK UpsertDocRequest vector length({len(vector)}) is invalid and must be same with collection dimension({self._dimension})",
```

### Comparing `dashvector-1.0.8/dashvector/core/proto/__init__.py` & `dashvector-1.0.9/dashvector/core/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/proto/dashvector_pb2.py` & `dashvector-1.0.9/dashvector/core/proto/dashvector_pb2.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/core/proto/dashvector_pb2_grpc.py` & `dashvector-1.0.9/dashvector/core/proto/dashvector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/util/__init__.py` & `dashvector-1.0.9/dashvector/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/dashvector/util/validator.py` & `dashvector-1.0.9/dashvector/util/convertor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-##
 #   Copyright 2021 Alibaba, Inc. and its affiliates. All Rights Reserved.
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
@@ -10,22 +9,20 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 ##
+import collections
 
 # -*- coding: utf-8 -*-
+from typing import Dict, Optional
 
-import re
-from typing import Optional
-
-ENDPOINT_PATTERN = "^([a-zA-Z0-9-.]+)\.([a-z\.]{2,6})\/?$"
-
+from dashvector.util.validator import verify_sparse_vector
 
-def verify_endpoint(endpoint: Optional[str]) -> bool:
-    """Verify endpoint is valid
 
-    verify_endpoint("dashvector.cn-hangzhou.aliyuncs.com") -> True
-    """
-    return endpoint and re.search(ENDPOINT_PATTERN, endpoint) is not None
+def to_sorted_sparse_vector(sparse_vector: Optional[Dict[int, float]]) -> Optional[Dict[int, float]]:
+    if sparse_vector is None:
+        return
+    verify_sparse_vector(sparse_vector)
+    return dict(sorted(sparse_vector.items()))
```

### Comparing `dashvector-1.0.8/dashvector/version.py` & `dashvector-1.0.9/dashvector/version.py`

 * *Files identical despite different names*

### Comparing `dashvector-1.0.8/pyproject.toml` & `dashvector-1.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                      # the root of the project
 )
 '''
 
 [tool.poetry]
 name = "dashvector"
 description = "DashVector Client Python Sdk Library"
-version = "1.0.8"
+version = "1.0.9"
 authors = ["Alibaba"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://help.aliyun.com/document_detail/2510225.html"
 homepage = "https://github.com/alibaba/proxima"
 keywords = ["DashVector", "vector", "database", "cloud"]
 classifiers = [
```

### Comparing `dashvector-1.0.8/PKG-INFO` & `dashvector-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashvector
-Version: 1.0.8
+Version: 1.0.9
 Summary: DashVector Client Python Sdk Library
 Home-page: https://github.com/alibaba/proxima
 License: Apache-2.0
 Keywords: DashVector,vector,database,cloud
 Author: Alibaba
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

