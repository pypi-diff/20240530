# Comparing `tmp/infinity_sdk-0.2.0.dev2-py3-none-any.whl.zip` & `tmp/infinity_sdk-0.2.0.dev3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,28 @@
-Zip file size: 50816 bytes, number of entries: 26
+Zip file size: 52918 bytes, number of entries: 26
 -rw-rw-r--  2.0 unx     1190 b- defN 24-May-26 15:19 infinity/__init__.py
 -rw-rw-r--  2.0 unx     1341 b- defN 24-May-26 15:06 infinity/common.py
 -rw-rw-r--  2.0 unx     1791 b- defN 24-May-16 06:36 infinity/connection_pool.py
 -rw-rw-r--  2.0 unx     1387 b- defN 24-May-16 06:36 infinity/db.py
 -rw-rw-r--  2.0 unx     4527 b- defN 24-May-27 01:59 infinity/errors.py
 -rw-rw-r--  2.0 unx     2481 b- defN 24-May-27 01:52 infinity/index.py
 -rw-rw-r--  2.0 unx     1237 b- defN 24-May-17 02:48 infinity/infinity.py
 -rw-rw-r--  2.0 unx     2487 b- defN 24-May-26 15:31 infinity/table.py
 -rw-rw-r--  2.0 unx     1515 b- defN 24-May-27 01:56 infinity/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Mar-27 16:25 infinity/remote_thrift/__init__.py
--rw-rw-r--  2.0 unx    13794 b- defN 24-May-26 09:28 infinity/remote_thrift/client.py
+-rw-rw-r--  2.0 unx    13987 b- defN 24-May-30 08:56 infinity/remote_thrift/client.py
 -rw-rw-r--  2.0 unx      680 b- defN 24-Mar-17 04:21 infinity/remote_thrift/common.py
--rw-rw-r--  2.0 unx    12826 b- defN 24-May-27 01:51 infinity/remote_thrift/db.py
+-rw-rw-r--  2.0 unx    13148 b- defN 24-May-30 06:59 infinity/remote_thrift/db.py
 -rw-rw-r--  2.0 unx     4167 b- defN 24-May-26 15:22 infinity/remote_thrift/infinity.py
--rw-rw-r--  2.0 unx    10027 b- defN 24-May-26 15:25 infinity/remote_thrift/query_builder.py
--rw-rw-r--  2.0 unx    18214 b- defN 24-May-26 15:29 infinity/remote_thrift/table.py
--rw-rw-r--  2.0 unx    10201 b- defN 24-May-25 12:23 infinity/remote_thrift/types.py
+-rw-rw-r--  2.0 unx    11523 b- defN 24-May-30 06:59 infinity/remote_thrift/query_builder.py
+-rw-rw-r--  2.0 unx    19944 b- defN 24-May-30 06:59 infinity/remote_thrift/table.py
+-rw-rw-r--  2.0 unx    16026 b- defN 24-May-30 06:59 infinity/remote_thrift/types.py
 -rw-rw-r--  2.0 unx     7763 b- defN 24-May-27 02:01 infinity/remote_thrift/utils.py
 -rw-rw-r--  2.0 unx   178466 b- defN 24-May-26 09:16 infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py
 -rw-rw-r--  2.0 unx       53 b- defN 24-Mar-27 16:25 infinity/remote_thrift/infinity_thrift_rpc/__init__.py
 -rw-rw-r--  2.0 unx      366 b- defN 24-May-16 06:36 infinity/remote_thrift/infinity_thrift_rpc/constants.py
--rw-rw-r--  2.0 unx   274464 b- defN 24-May-26 09:16 infinity/remote_thrift/infinity_thrift_rpc/ttypes.py
--rw-rw-r--  2.0 unx     2241 b- defN 24-May-28 10:07 infinity_sdk-0.2.0.dev2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-28 10:07 infinity_sdk-0.2.0.dev2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-May-28 10:07 infinity_sdk-0.2.0.dev2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2275 b- defN 24-May-28 10:07 infinity_sdk-0.2.0.dev2.dist-info/RECORD
-26 files, 553594 bytes uncompressed, 47118 bytes compressed:  91.5%
+-rw-rw-r--  2.0 unx   285540 b- defN 24-May-30 06:59 infinity/remote_thrift/infinity_thrift_rpc/ttypes.py
+-rw-rw-r--  2.0 unx     2241 b- defN 24-May-30 09:44 infinity_sdk-0.2.0.dev3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-30 09:44 infinity_sdk-0.2.0.dev3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-30 09:44 infinity_sdk-0.2.0.dev3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2275 b- defN 24-May-30 09:44 infinity_sdk-0.2.0.dev3.dist-info/RECORD
+26 files, 574236 bytes uncompressed, 49220 bytes compressed:  91.4%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: infinity/remote_thrift/infinity_thrift_rpc/constants.py
 Comment: 
 
 Filename: infinity/remote_thrift/infinity_thrift_rpc/ttypes.py
 Comment: 
 
-Filename: infinity_sdk-0.2.0.dev2.dist-info/METADATA
+Filename: infinity_sdk-0.2.0.dev3.dist-info/METADATA
 Comment: 
 
-Filename: infinity_sdk-0.2.0.dev2.dist-info/WHEEL
+Filename: infinity_sdk-0.2.0.dev3.dist-info/WHEEL
 Comment: 
 
-Filename: infinity_sdk-0.2.0.dev2.dist-info/top_level.txt
+Filename: infinity_sdk-0.2.0.dev3.dist-info/top_level.txt
 Comment: 
 
-Filename: infinity_sdk-0.2.0.dev2.dist-info/RECORD
+Filename: infinity_sdk-0.2.0.dev3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## infinity/remote_thrift/client.py

```diff
@@ -17,15 +17,15 @@
 from thrift.transport import TSocket
 from thrift.transport.TTransport import TTransportException
 
 from infinity import URI
 from infinity.remote_thrift.infinity_thrift_rpc import *
 from infinity.remote_thrift.infinity_thrift_rpc.ttypes import *
 from infinity.errors import ErrorCode
-
+from infinity.common import InfinityException
 
 class ThriftInfinityClient:
     def __init__(self, uri: URI):
         self.uri = uri
         self.transport = None
         self.reconnect()
 
@@ -39,15 +39,18 @@
         self.protocol = TBinaryProtocol.TBinaryProtocol(self.transport)
         # self.protocol = TCompactProtocol.TCompactProtocol(self.transport)
         self.client = InfinityService.Client(self.protocol)
         self.transport.open()
 
         # version: 0.2.0.dev2, client_version: 1
         # version: 0.2.0.dev3, client_version: 2
-        res = self.client.Connect(ConnectRequest(client_version=1))
+        # version: 0.2.0.dev4, client_version: 3
+        res = self.client.Connect(ConnectRequest(client_version=2))
+        if res.error_code != 0:
+            raise InfinityException(res.error_code, res.error_msg)
         self.session_id = res.session_id
 
     def create_database(self, db_name: str, conflict_type: CreateConflict = CreateConflict.Error):
         return self.client.CreateDatabase(CreateDatabaseRequest(session_id=self.session_id,
                                                                 db_name=db_name,
                                                                 create_option=CreateOption(
                                                                     conflict_type=conflict_type)))
```

## infinity/remote_thrift/db.py

```diff
@@ -112,15 +112,20 @@
     length = column_big_info[1]
     element_type = column_big_info[2]
 
     proto_column_def = ttypes.ColumnDef()
     proto_column_def.id = index
     proto_column_def.name = column_name
     column_type = ttypes.DataType()
-    column_type.logic_type = ttypes.LogicType.Embedding
+    if column_big_info[0] == "vector":
+        column_type.logic_type = ttypes.LogicType.Embedding
+    elif column_big_info[0] == "tensor":
+        column_type.logic_type = ttypes.LogicType.Tensor
+    elif column_big_info[0] == "tensorarray":
+        column_type.logic_type = ttypes.LogicType.TensorArray
     embedding_type = ttypes.EmbeddingType()
     if element_type == "bit":
         embedding_type.element_type = ttypes.ElementType.ElementBit
     elif element_type == "float32" or element_type == "float":
         embedding_type.element_type = ttypes.ElementType.ElementFloat32
     elif element_type == "float64" or element_type == "double":
         embedding_type.element_type = ttypes.ElementType.ElementFloat64
@@ -201,15 +206,15 @@
             }, None)
         """
         # to column_defs
         column_defs = []
         for index, (column_name, column_info) in enumerate(columns_definition.items()):
             check_valid_name(column_name, "Column")
             column_big_info = [item.strip() for item in column_info["type"].split(",")]
-            if column_big_info[0] == "vector":
+            if column_big_info[0] == "vector" or column_big_info[0] == "tensor" or column_big_info[0] == "tensorarray":
                 get_embedding_info(column_info, column_defs, column_name, index)
 
             else:  # numeric or varchar
                 get_ordinary_info(column_info, column_defs, column_name, index)
 
         create_table_conflict: ttypes.CreateConflict
         if conflict_type == ConflictType.Error:
```

## infinity/remote_thrift/query_builder.py

```diff
@@ -22,15 +22,15 @@
 import polars as pl
 import pyarrow as pa
 from pyarrow import Table
 from sqlglot import condition, maybe_parse
 
 from infinity.common import VEC, InfinityException
 from infinity.remote_thrift.infinity_thrift_rpc.ttypes import *
-from infinity.remote_thrift.types import logic_type_to_dtype
+from infinity.remote_thrift.types import logic_type_to_dtype, make_match_tensor_expr
 from infinity.remote_thrift.utils import traverse_conditions, parse_expr
 
 '''FIXME: How to disable validation of only the search field?'''
 
 
 class Query(ABC):
     def __init__(self, columns: Optional[List[ParsedExpr]], search: Optional[SearchExpr], filter: Optional[ParsedExpr],
@@ -150,21 +150,37 @@
         match_expr = MatchExpr()
         match_expr.fields = fields
         match_expr.matching_text = matching_text
         match_expr.options_text = options_text
         self._search.match_exprs.append(match_expr)
         return self
 
-    def fusion(self, method: str, options_text: str = '') -> InfinityThriftQueryBuilder:
+    def match_tensor(self, vector_column_name: str, embedding_data: VEC, embedding_data_type: str, method_type: str,
+                     extra_option: str) -> InfinityThriftQueryBuilder:
         if self._search is None:
             self._search = SearchExpr()
+        if self._search.match_tensor_exprs is None:
+            self._search.match_tensor_exprs = list()
+        match_tensor_expr = make_match_tensor_expr(vector_column_name, embedding_data, embedding_data_type,
+                                                   method_type, extra_option)
+        self._search.match_tensor_exprs.append(match_tensor_expr)
+        return self
+
+    def fusion(self, method: str, options_text: str = '',
+               match_tensor_expr: MatchTensorExpr = None) -> InfinityThriftQueryBuilder:
+        if self._search is None:
+            self._search = SearchExpr()
+        if self._search.fusion_exprs is None:
+            self._search.fusion_exprs = list()
         fusion_expr = FusionExpr()
         fusion_expr.method = method
         fusion_expr.options_text = options_text
-        self._search.fusion_expr = fusion_expr
+        if match_tensor_expr is not None:
+            fusion_expr.optional_match_tensor_expr = match_tensor_expr
+        self._search.fusion_exprs.append(fusion_expr)
         return self
 
     def filter(self, where: Optional[str]) -> InfinityThriftQueryBuilder:
         where_expr = traverse_conditions(condition(where))
         self._filter = where_expr
         return self
 
@@ -194,22 +210,30 @@
             match column:
                 case "*":
                     column_expr = ColumnExpr(star=True, column_name=[])
                     expr_type = ParsedExprType(column_expr=column_expr)
                     parsed_expr = ParsedExpr(type=expr_type)
                     select_list.append(parsed_expr)
                 case "_row_id":
-                    func_expr = FunctionExpr(
-                        function_name="row_id", arguments=[])
+                    func_expr = FunctionExpr(function_name="row_id", arguments=[])
                     expr_type = ParsedExprType(function_expr=func_expr)
                     parsed_expr = ParsedExpr(type=expr_type)
                     select_list.append(parsed_expr)
                 case "_score":
-                    func_expr = FunctionExpr(
-                        function_name="score", arguments=[])
+                    func_expr = FunctionExpr(function_name="score", arguments=[])
+                    expr_type = ParsedExprType(function_expr=func_expr)
+                    parsed_expr = ParsedExpr(type=expr_type)
+                    select_list.append(parsed_expr)
+                case "_similarity":
+                    func_expr = FunctionExpr(function_name="similarity", arguments=[])
+                    expr_type = ParsedExprType(function_expr=func_expr)
+                    parsed_expr = ParsedExpr(type=expr_type)
+                    select_list.append(parsed_expr)
+                case "_distance":
+                    func_expr = FunctionExpr(function_name="distance", arguments=[])
                     expr_type = ParsedExprType(function_expr=func_expr)
                     parsed_expr = ParsedExpr(type=expr_type)
                     select_list.append(parsed_expr)
                 case _:
                     select_list.append(parse_expr(maybe_parse(column)))
 
         self._columns = select_list
```

## infinity/remote_thrift/table.py

```diff
@@ -190,16 +190,34 @@
                 elif isinstance(value, list):
                     if isinstance(value[0], int):
                         constant_expression = ttypes.ConstantExpr(literal_type=ttypes.LiteralType.IntegerArray,
                                                                   i64_array_value=value)
                     elif isinstance(value[0], float):
                         constant_expression = ttypes.ConstantExpr(literal_type=ttypes.LiteralType.DoubleArray,
                                                                   f64_array_value=value)
+                    elif isinstance(value[0], list):
+                        if isinstance(value[0][0], int):
+                            constant_expression = ttypes.ConstantExpr(
+                                literal_type=ttypes.LiteralType.IntegerArray,
+                                i64_array_value=[x for xs in value for x in xs])
+                        elif isinstance(value[0][0], float):
+                            constant_expression = ttypes.ConstantExpr(
+                                literal_type=ttypes.LiteralType.DoubleArray,
+                                f64_array_value=[x for xs in value for x in xs])
+                        elif isinstance(value[0][0], list):
+                            if isinstance(value[0][0][0], int):
+                                constant_expression = ttypes.ConstantExpr(
+                                    literal_type=ttypes.LiteralType.IntegerTensorArray,
+                                    i64_tensor_array_value=value)
+                            elif isinstance(value[0][0][0], float):
+                                constant_expression = ttypes.ConstantExpr(
+                                    literal_type=ttypes.LiteralType.DoubleTensorArray,
+                                    f64_tensor_array_value=value)
                 else:
-                    raise InfinityException(3069, "Invalid constant expression")
+                    raise InfinityException(3069, f"Invalid constant expression: {type(value)}")
 
                 expr_type = ttypes.ParsedExprType(
                     constant_expr=constant_expression)
                 paser_expr = ttypes.ParsedExpr(type=expr_type)
 
                 parse_exprs.append(paser_expr)
 
@@ -326,16 +344,23 @@
 
     @params_type_check
     def match(self, fields: str, matching_text: str, options_text: str = ''):
         self.query_builder.match(fields, matching_text, options_text)
         return self
 
     @params_type_check
-    def fusion(self, method: str, options_text: str = ''):
-        self.query_builder.fusion(method, options_text)
+    def match_tensor(self, vector_column_name: str, embedding_data: VEC, embedding_data_type: str, method_type: str,
+                     extra_option: str):
+        self.query_builder.match_tensor(vector_column_name, embedding_data, embedding_data_type, method_type,
+                                        extra_option)
+        return self
+
+    @params_type_check
+    def fusion(self, method: str, options_text: str = '', match_tensor_expr: ttypes.MatchTensorExpr = None):
+        self.query_builder.fusion(method, options_text, match_tensor_expr)
         return self
 
     def output(self, columns: Optional[List[str]]):
         self.query_builder.output(columns)
         return self
 
     def filter(self, filter: Optional[str]):
```

## infinity/remote_thrift/types.py

```diff
@@ -9,14 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import struct
+import numpy as np
+from infinity.common import VEC, InfinityException
+from infinity.remote_thrift.infinity_thrift_rpc.ttypes import *
 from collections import defaultdict
 from typing import Any, Tuple, Dict, List
 
 import polars as pl
 from numpy import dtype
 
 import infinity.remote_thrift.infinity_thrift_rpc.ttypes as ttypes
@@ -75,14 +78,18 @@
                         return object
                     case ttypes.ElementType.ElementFloat64:
                         return object
                     case ttypes.ElementType.ElementBit:
                         return object
                     case _:
                         raise NotImplementedError(f"Unsupported type {ttype}")
+        case ttypes.LogicType.Tensor:
+            return object
+        case ttypes.LogicType.TensorArray:
+            return object
         case _:
             raise NotImplementedError(f"Unsupported type {ttype}")
 
 
 def logic_type_to_pl_type(ttype: ttypes.DataType):
     match ttype.logic_type:
         case ttypes.LogicType.Boolean:
@@ -170,14 +177,18 @@
             elif column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementBit:
                 all_list = list(struct.unpack(
                     '<{}?'.format(len(column_vector)), column_vector))
                 return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
             else:
                 raise NotImplementedError(
                     f"Unsupported type {column_data_type.physical_type.embedding_type.element_type}")
+        case ttypes.ColumnType.ColumnTensor:
+            return parse_tensor_bytes(column_data_type, column_vector)
+        case ttypes.ColumnType.ColumnTensorArray:
+            return parse_tensorarray_bytes(column_data_type, column_vector)
         case _:
             raise NotImplementedError(f"Unsupported type {column_type}")
 
 
 def parse_bytes(bytes_data):
     results = []
     offset = 0
@@ -186,14 +197,74 @@
         offset += 4
         string_data = bytes_data[offset:offset + length].decode('utf-8')
         results.append(string_data)
         offset += length
     return results
 
 
+def parse_tensor_bytes(column_data_type: ttypes.DataType, bytes_data):
+    results = []
+    offset = 0
+    while offset < len(bytes_data):
+        length = struct.unpack('I', bytes_data[offset:offset + 4])[0]
+        offset += 4
+        tensor_data = tensor_to_list(column_data_type, bytes_data[offset:offset + length])
+        results.append(tensor_data)
+        offset += length
+    return results
+
+
+def parse_tensorarray_bytes(column_data_type: ttypes.DataType, bytes_data):
+    results = []
+    offset = 0
+    while offset < len(bytes_data):
+        tensor_n = struct.unpack('I', bytes_data[offset:offset + 4])[0]
+        offset += 4
+        tensorarray_data = []
+        for _ in range(tensor_n):
+            length = struct.unpack('I', bytes_data[offset:offset + 4])[0]
+            offset += 4
+            tensor_data = tensor_to_list(column_data_type, bytes_data[offset:offset + length])
+            offset += length
+            tensorarray_data.append(tensor_data)
+        results.append(tensorarray_data)
+    return results
+
+
+def tensor_to_list(column_data_type: ttypes.DataType, binary_data) -> list[list[Any]]:
+    dimension = column_data_type.physical_type.embedding_type.dimension
+    if column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementInt8:
+        all_list = list(struct.unpack(
+            '<{}b'.format(len(binary_data)), binary_data))
+        return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
+    elif column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementInt16:
+        all_list = list(struct.unpack('<{}h'.format(
+            len(binary_data) // 2), binary_data))
+        return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
+    elif column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementInt32:
+        all_list = list(struct.unpack('<{}i'.format(
+            len(binary_data) // 4), binary_data))
+        return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
+    elif column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementFloat32:
+        all_list = list(struct.unpack('<{}f'.format(
+            len(binary_data) // 4), binary_data))
+        return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
+    elif column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementFloat64:
+        all_list = list(struct.unpack('<{}d'.format(
+            len(binary_data) // 8), binary_data))
+        return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
+    elif column_data_type.physical_type.embedding_type.element_type == ttypes.ElementType.ElementBit:
+        all_list = list(struct.unpack(
+            '<{}?'.format(len(binary_data)), binary_data))
+        return [all_list[i:i + dimension] for i in range(0, len(all_list), dimension)]
+    else:
+        raise NotImplementedError(
+            f"Unsupported type {column_data_type.physical_type.embedding_type.element_type}")
+
+
 def find_data_type(column_name: str, column_defs: list[ttypes.ColumnDef]) -> ttypes.DataType:
     for column_def in column_defs:
         if column_def.name == column_name:
             return column_def.data_type
     raise KeyError(f"column name {column_name} not found in column defs")
 
 
@@ -214,7 +285,42 @@
 
         data_list = column_vector_to_list(column_type, column_data_type, column_vectors)
         # data_series = pd.Series(data_list, dtype=logic_type_to_dtype(column_data_type))
         data_dict[column_name] = data_list
         data_type_dict[column_name] = column_data_type
 
     return data_dict, data_type_dict
+
+
+def make_match_tensor_expr(vector_column_name: str, embedding_data: VEC, embedding_data_type: str,
+                           method_type: str, extra_option: str = None) -> MatchTensorExpr:
+    match_tensor_expr = MatchTensorExpr()
+    match_tensor_expr.column_expr = ColumnExpr(column_name=[vector_column_name], star=False)
+    match_tensor_expr.search_method = method_type
+    match_tensor_expr.extra_options = extra_option
+    data = EmbeddingData()
+    if embedding_data_type == 'bit':
+        raise InfinityException(3057, f"Invalid embedding {embedding_data[0]} type")
+    elif embedding_data_type == 'tinyint' or embedding_data_type == 'int8' or embedding_data_type == 'i8':
+        elem_type = ElementType.ElementInt8
+        data.i8_array_value = np.asarray(embedding_data, dtype=np.int8).flatten()
+    elif embedding_data_type == 'smallint' or embedding_data_type == 'int16' or embedding_data_type == 'i16':
+        elem_type = ElementType.ElementInt16
+        data.i16_array_value = np.asarray(embedding_data, dtype=np.int16).flatten()
+    elif embedding_data_type == 'int' or embedding_data_type == 'int32' or embedding_data_type == 'i32':
+        elem_type = ElementType.ElementInt32
+        data.i32_array_value = np.asarray(embedding_data, dtype=np.int32).flatten()
+    elif embedding_data_type == 'bigint' or embedding_data_type == 'int64' or embedding_data_type == 'i64':
+        elem_type = ElementType.ElementInt64
+        data.i64_array_value = np.asarray(embedding_data, dtype=np.int64).flatten()
+    elif embedding_data_type == 'float' or embedding_data_type == 'float32' or embedding_data_type == 'f32':
+        elem_type = ElementType.ElementFloat32
+        data.f32_array_value = np.asarray(embedding_data, dtype=np.float32).flatten()
+    elif embedding_data_type == 'double' or embedding_data_type == 'float64' or embedding_data_type == 'f64':
+        elem_type = ElementType.ElementFloat64
+        data.f64_array_value = np.asarray(embedding_data, dtype=np.float64).flatten()
+    else:
+        raise InfinityException(3057, f"Invalid embedding {embedding_data[0]} type")
+
+    match_tensor_expr.embedding_data_type = elem_type
+    match_tensor_expr.embedding_data = data
+    return match_tensor_expr
```

## infinity/remote_thrift/infinity_thrift_rpc/ttypes.py

```diff
@@ -24,44 +24,50 @@
     BigInt = 4
     HugeInt = 5
     Decimal = 6
     Float = 7
     Double = 8
     Varchar = 9
     Embedding = 10
-    Invalid = 11
+    Tensor = 11
+    TensorArray = 12
+    Invalid = 13
 
     _VALUES_TO_NAMES = {
         0: "Boolean",
         1: "TinyInt",
         2: "SmallInt",
         3: "Integer",
         4: "BigInt",
         5: "HugeInt",
         6: "Decimal",
         7: "Float",
         8: "Double",
         9: "Varchar",
         10: "Embedding",
-        11: "Invalid",
+        11: "Tensor",
+        12: "TensorArray",
+        13: "Invalid",
     }
 
     _NAMES_TO_VALUES = {
         "Boolean": 0,
         "TinyInt": 1,
         "SmallInt": 2,
         "Integer": 3,
         "BigInt": 4,
         "HugeInt": 5,
         "Decimal": 6,
         "Float": 7,
         "Double": 8,
         "Varchar": 9,
         "Embedding": 10,
-        "Invalid": 11,
+        "Tensor": 11,
+        "TensorArray": 12,
+        "Invalid": 13,
     }
 
 
 class CreateConflict(object):
     Ignore = 0
     Error = 1
     Replace = 2
@@ -149,33 +155,39 @@
     Boolean = 0
     Double = 1
     String = 2
     Int64 = 3
     Null = 4
     IntegerArray = 5
     DoubleArray = 6
+    IntegerTensorArray = 7
+    DoubleTensorArray = 8
 
     _VALUES_TO_NAMES = {
         0: "Boolean",
         1: "Double",
         2: "String",
         3: "Int64",
         4: "Null",
         5: "IntegerArray",
         6: "DoubleArray",
+        7: "IntegerTensorArray",
+        8: "DoubleTensorArray",
     }
 
     _NAMES_TO_VALUES = {
         "Boolean": 0,
         "Double": 1,
         "String": 2,
         "Int64": 3,
         "Null": 4,
         "IntegerArray": 5,
         "DoubleArray": 6,
+        "IntegerTensorArray": 7,
+        "DoubleTensorArray": 8,
     }
 
 
 class KnnDistanceType(object):
     L2 = 0
     Cosine = 1
     InnerProduct = 2
@@ -223,43 +235,49 @@
     ColumnInt16 = 2
     ColumnInt32 = 3
     ColumnInt64 = 4
     ColumnFloat32 = 5
     ColumnFloat64 = 6
     ColumnVarchar = 7
     ColumnEmbedding = 8
-    ColumnRowID = 9
-    ColumnInvalid = 10
+    ColumnTensor = 9
+    ColumnTensorArray = 10
+    ColumnRowID = 11
+    ColumnInvalid = 12
 
     _VALUES_TO_NAMES = {
         0: "ColumnBool",
         1: "ColumnInt8",
         2: "ColumnInt16",
         3: "ColumnInt32",
         4: "ColumnInt64",
         5: "ColumnFloat32",
         6: "ColumnFloat64",
         7: "ColumnVarchar",
         8: "ColumnEmbedding",
-        9: "ColumnRowID",
-        10: "ColumnInvalid",
+        9: "ColumnTensor",
+        10: "ColumnTensorArray",
+        11: "ColumnRowID",
+        12: "ColumnInvalid",
     }
 
     _NAMES_TO_VALUES = {
         "ColumnBool": 0,
         "ColumnInt8": 1,
         "ColumnInt16": 2,
         "ColumnInt32": 3,
         "ColumnInt64": 4,
         "ColumnFloat32": 5,
         "ColumnFloat64": 6,
         "ColumnVarchar": 7,
         "ColumnEmbedding": 8,
-        "ColumnRowID": 9,
-        "ColumnInvalid": 10,
+        "ColumnTensor": 9,
+        "ColumnTensorArray": 10,
+        "ColumnRowID": 11,
+        "ColumnInvalid": 12,
     }
 
 
 class IndexType(object):
     IVFFlat = 0
     HnswLVQ = 1
     Hnsw = 2
@@ -1349,14 +1367,223 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class ConstantExpr(object):
+    """
+    Attributes:
+     - literal_type
+     - bool_value
+     - i64_value
+     - f64_value
+     - str_value
+     - i64_array_value
+     - f64_array_value
+     - i64_tensor_array_value
+     - f64_tensor_array_value
+
+    """
+
+
+    def __init__(self, literal_type=None, bool_value=None, i64_value=None, f64_value=None, str_value=None, i64_array_value=None, f64_array_value=None, i64_tensor_array_value=None, f64_tensor_array_value=None,):
+        self.literal_type = literal_type
+        self.bool_value = bool_value
+        self.i64_value = i64_value
+        self.f64_value = f64_value
+        self.str_value = str_value
+        self.i64_array_value = i64_array_value
+        self.f64_array_value = f64_array_value
+        self.i64_tensor_array_value = i64_tensor_array_value
+        self.f64_tensor_array_value = f64_tensor_array_value
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.literal_type = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.BOOL:
+                    self.bool_value = iprot.readBool()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I64:
+                    self.i64_value = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.DOUBLE:
+                    self.f64_value = iprot.readDouble()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRING:
+                    self.str_value = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.LIST:
+                    self.i64_array_value = []
+                    (_etype66, _size63) = iprot.readListBegin()
+                    for _i67 in range(_size63):
+                        _elem68 = iprot.readI64()
+                        self.i64_array_value.append(_elem68)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 7:
+                if ftype == TType.LIST:
+                    self.f64_array_value = []
+                    (_etype72, _size69) = iprot.readListBegin()
+                    for _i73 in range(_size69):
+                        _elem74 = iprot.readDouble()
+                        self.f64_array_value.append(_elem74)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 8:
+                if ftype == TType.LIST:
+                    self.i64_tensor_array_value = []
+                    (_etype78, _size75) = iprot.readListBegin()
+                    for _i79 in range(_size75):
+                        _elem80 = []
+                        (_etype84, _size81) = iprot.readListBegin()
+                        for _i85 in range(_size81):
+                            _elem86 = []
+                            (_etype90, _size87) = iprot.readListBegin()
+                            for _i91 in range(_size87):
+                                _elem92 = iprot.readI64()
+                                _elem86.append(_elem92)
+                            iprot.readListEnd()
+                            _elem80.append(_elem86)
+                        iprot.readListEnd()
+                        self.i64_tensor_array_value.append(_elem80)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 9:
+                if ftype == TType.LIST:
+                    self.f64_tensor_array_value = []
+                    (_etype96, _size93) = iprot.readListBegin()
+                    for _i97 in range(_size93):
+                        _elem98 = []
+                        (_etype102, _size99) = iprot.readListBegin()
+                        for _i103 in range(_size99):
+                            _elem104 = []
+                            (_etype108, _size105) = iprot.readListBegin()
+                            for _i109 in range(_size105):
+                                _elem110 = iprot.readDouble()
+                                _elem104.append(_elem110)
+                            iprot.readListEnd()
+                            _elem98.append(_elem104)
+                        iprot.readListEnd()
+                        self.f64_tensor_array_value.append(_elem98)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('ConstantExpr')
+        if self.literal_type is not None:
+            oprot.writeFieldBegin('literal_type', TType.I32, 1)
+            oprot.writeI32(self.literal_type)
+            oprot.writeFieldEnd()
+        if self.bool_value is not None:
+            oprot.writeFieldBegin('bool_value', TType.BOOL, 2)
+            oprot.writeBool(self.bool_value)
+            oprot.writeFieldEnd()
+        if self.i64_value is not None:
+            oprot.writeFieldBegin('i64_value', TType.I64, 3)
+            oprot.writeI64(self.i64_value)
+            oprot.writeFieldEnd()
+        if self.f64_value is not None:
+            oprot.writeFieldBegin('f64_value', TType.DOUBLE, 4)
+            oprot.writeDouble(self.f64_value)
+            oprot.writeFieldEnd()
+        if self.str_value is not None:
+            oprot.writeFieldBegin('str_value', TType.STRING, 5)
+            oprot.writeString(self.str_value.encode('utf-8') if sys.version_info[0] == 2 else self.str_value)
+            oprot.writeFieldEnd()
+        if self.i64_array_value is not None:
+            oprot.writeFieldBegin('i64_array_value', TType.LIST, 6)
+            oprot.writeListBegin(TType.I64, len(self.i64_array_value))
+            for iter111 in self.i64_array_value:
+                oprot.writeI64(iter111)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.f64_array_value is not None:
+            oprot.writeFieldBegin('f64_array_value', TType.LIST, 7)
+            oprot.writeListBegin(TType.DOUBLE, len(self.f64_array_value))
+            for iter112 in self.f64_array_value:
+                oprot.writeDouble(iter112)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.i64_tensor_array_value is not None:
+            oprot.writeFieldBegin('i64_tensor_array_value', TType.LIST, 8)
+            oprot.writeListBegin(TType.LIST, len(self.i64_tensor_array_value))
+            for iter113 in self.i64_tensor_array_value:
+                oprot.writeListBegin(TType.LIST, len(iter113))
+                for iter114 in iter113:
+                    oprot.writeListBegin(TType.I64, len(iter114))
+                    for iter115 in iter114:
+                        oprot.writeI64(iter115)
+                    oprot.writeListEnd()
+                oprot.writeListEnd()
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.f64_tensor_array_value is not None:
+            oprot.writeFieldBegin('f64_tensor_array_value', TType.LIST, 9)
+            oprot.writeListBegin(TType.LIST, len(self.f64_tensor_array_value))
+            for iter116 in self.f64_tensor_array_value:
+                oprot.writeListBegin(TType.LIST, len(iter116))
+                for iter117 in iter116:
+                    oprot.writeListBegin(TType.DOUBLE, len(iter117))
+                    for iter118 in iter117:
+                        oprot.writeDouble(iter118)
+                    oprot.writeListEnd()
+                oprot.writeListEnd()
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class KnnExpr(object):
     """
     Attributes:
      - column_expr
      - embedding_data
      - embedding_data_type
      - distance_type
@@ -1413,19 +1640,19 @@
                 if ftype == TType.I64:
                     self.topn = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.opt_params = []
-                    (_etype66, _size63) = iprot.readListBegin()
-                    for _i67 in range(_size63):
-                        _elem68 = InitParameter()
-                        _elem68.read(iprot)
-                        self.opt_params.append(_elem68)
+                    (_etype122, _size119) = iprot.readListBegin()
+                    for _i123 in range(_size119):
+                        _elem124 = InitParameter()
+                        _elem124.read(iprot)
+                        self.opt_params.append(_elem124)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -1454,16 +1681,16 @@
         if self.topn is not None:
             oprot.writeFieldBegin('topn', TType.I64, 5)
             oprot.writeI64(self.topn)
             oprot.writeFieldEnd()
         if self.opt_params is not None:
             oprot.writeFieldBegin('opt_params', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.opt_params))
-            for iter69 in self.opt_params:
-                iter69.write(oprot)
+            for iter125 in self.opt_params:
+                iter125.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -1476,74 +1703,98 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class MatchExpr(object):
+class MatchTensorExpr(object):
     """
     Attributes:
-     - fields
-     - matching_text
-     - options_text
+     - search_method
+     - column_expr
+     - embedding_data_type
+     - embedding_data
+     - extra_options
 
     """
 
 
-    def __init__(self, fields=None, matching_text=None, options_text=None,):
-        self.fields = fields
-        self.matching_text = matching_text
-        self.options_text = options_text
+    def __init__(self, search_method=None, column_expr=None, embedding_data_type=None, embedding_data=None, extra_options=None,):
+        self.search_method = search_method
+        self.column_expr = column_expr
+        self.embedding_data_type = embedding_data_type
+        self.embedding_data = embedding_data
+        self.extra_options = extra_options
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.STRING:
-                    self.fields = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                    self.search_method = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
-                if ftype == TType.STRING:
-                    self.matching_text = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                if ftype == TType.STRUCT:
+                    self.column_expr = ColumnExpr()
+                    self.column_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
+                if ftype == TType.I32:
+                    self.embedding_data_type = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.embedding_data = EmbeddingData()
+                    self.embedding_data.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
                 if ftype == TType.STRING:
-                    self.options_text = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                    self.extra_options = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('MatchExpr')
-        if self.fields is not None:
-            oprot.writeFieldBegin('fields', TType.STRING, 1)
-            oprot.writeString(self.fields.encode('utf-8') if sys.version_info[0] == 2 else self.fields)
+        oprot.writeStructBegin('MatchTensorExpr')
+        if self.search_method is not None:
+            oprot.writeFieldBegin('search_method', TType.STRING, 1)
+            oprot.writeString(self.search_method.encode('utf-8') if sys.version_info[0] == 2 else self.search_method)
             oprot.writeFieldEnd()
-        if self.matching_text is not None:
-            oprot.writeFieldBegin('matching_text', TType.STRING, 2)
-            oprot.writeString(self.matching_text.encode('utf-8') if sys.version_info[0] == 2 else self.matching_text)
+        if self.column_expr is not None:
+            oprot.writeFieldBegin('column_expr', TType.STRUCT, 2)
+            self.column_expr.write(oprot)
             oprot.writeFieldEnd()
-        if self.options_text is not None:
-            oprot.writeFieldBegin('options_text', TType.STRING, 3)
-            oprot.writeString(self.options_text.encode('utf-8') if sys.version_info[0] == 2 else self.options_text)
+        if self.embedding_data_type is not None:
+            oprot.writeFieldBegin('embedding_data_type', TType.I32, 3)
+            oprot.writeI32(self.embedding_data_type)
+            oprot.writeFieldEnd()
+        if self.embedding_data is not None:
+            oprot.writeFieldBegin('embedding_data', TType.STRUCT, 4)
+            self.embedding_data.write(oprot)
+            oprot.writeFieldEnd()
+        if self.extra_options is not None:
+            oprot.writeFieldBegin('extra_options', TType.STRING, 5)
+            oprot.writeString(self.extra_options.encode('utf-8') if sys.version_info[0] == 2 else self.extra_options)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
@@ -1555,62 +1806,73 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class FusionExpr(object):
+class MatchExpr(object):
     """
     Attributes:
-     - method
+     - fields
+     - matching_text
      - options_text
 
     """
 
 
-    def __init__(self, method=None, options_text=None,):
-        self.method = method
+    def __init__(self, fields=None, matching_text=None, options_text=None,):
+        self.fields = fields
+        self.matching_text = matching_text
         self.options_text = options_text
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.STRING:
-                    self.method = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                    self.fields = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
+                    self.matching_text = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
                     self.options_text = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('FusionExpr')
-        if self.method is not None:
-            oprot.writeFieldBegin('method', TType.STRING, 1)
-            oprot.writeString(self.method.encode('utf-8') if sys.version_info[0] == 2 else self.method)
+        oprot.writeStructBegin('MatchExpr')
+        if self.fields is not None:
+            oprot.writeFieldBegin('fields', TType.STRING, 1)
+            oprot.writeString(self.fields.encode('utf-8') if sys.version_info[0] == 2 else self.fields)
+            oprot.writeFieldEnd()
+        if self.matching_text is not None:
+            oprot.writeFieldBegin('matching_text', TType.STRING, 2)
+            oprot.writeString(self.matching_text.encode('utf-8') if sys.version_info[0] == 2 else self.matching_text)
             oprot.writeFieldEnd()
         if self.options_text is not None:
-            oprot.writeFieldBegin('options_text', TType.STRING, 2)
+            oprot.writeFieldBegin('options_text', TType.STRING, 3)
             oprot.writeString(self.options_text.encode('utf-8') if sys.version_info[0] == 2 else self.options_text)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -1623,93 +1885,75 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class SearchExpr(object):
+class FusionExpr(object):
     """
     Attributes:
-     - match_exprs
-     - knn_exprs
-     - fusion_expr
+     - method
+     - options_text
+     - optional_match_tensor_expr
 
     """
 
 
-    def __init__(self, match_exprs=None, knn_exprs=None, fusion_expr=None,):
-        self.match_exprs = match_exprs
-        self.knn_exprs = knn_exprs
-        self.fusion_expr = fusion_expr
+    def __init__(self, method=None, options_text=None, optional_match_tensor_expr=None,):
+        self.method = method
+        self.options_text = options_text
+        self.optional_match_tensor_expr = optional_match_tensor_expr
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
-                if ftype == TType.LIST:
-                    self.match_exprs = []
-                    (_etype73, _size70) = iprot.readListBegin()
-                    for _i74 in range(_size70):
-                        _elem75 = MatchExpr()
-                        _elem75.read(iprot)
-                        self.match_exprs.append(_elem75)
-                    iprot.readListEnd()
+                if ftype == TType.STRING:
+                    self.method = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
-                if ftype == TType.LIST:
-                    self.knn_exprs = []
-                    (_etype79, _size76) = iprot.readListBegin()
-                    for _i80 in range(_size76):
-                        _elem81 = KnnExpr()
-                        _elem81.read(iprot)
-                        self.knn_exprs.append(_elem81)
-                    iprot.readListEnd()
+                if ftype == TType.STRING:
+                    self.options_text = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRUCT:
-                    self.fusion_expr = FusionExpr()
-                    self.fusion_expr.read(iprot)
+                    self.optional_match_tensor_expr = MatchTensorExpr()
+                    self.optional_match_tensor_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('SearchExpr')
-        if self.match_exprs is not None:
-            oprot.writeFieldBegin('match_exprs', TType.LIST, 1)
-            oprot.writeListBegin(TType.STRUCT, len(self.match_exprs))
-            for iter82 in self.match_exprs:
-                iter82.write(oprot)
-            oprot.writeListEnd()
+        oprot.writeStructBegin('FusionExpr')
+        if self.method is not None:
+            oprot.writeFieldBegin('method', TType.STRING, 1)
+            oprot.writeString(self.method.encode('utf-8') if sys.version_info[0] == 2 else self.method)
             oprot.writeFieldEnd()
-        if self.knn_exprs is not None:
-            oprot.writeFieldBegin('knn_exprs', TType.LIST, 2)
-            oprot.writeListBegin(TType.STRUCT, len(self.knn_exprs))
-            for iter83 in self.knn_exprs:
-                iter83.write(oprot)
-            oprot.writeListEnd()
+        if self.options_text is not None:
+            oprot.writeFieldBegin('options_text', TType.STRING, 2)
+            oprot.writeString(self.options_text.encode('utf-8') if sys.version_info[0] == 2 else self.options_text)
             oprot.writeFieldEnd()
-        if self.fusion_expr is not None:
-            oprot.writeFieldBegin('fusion_expr', TType.STRUCT, 3)
-            self.fusion_expr.write(oprot)
+        if self.optional_match_tensor_expr is not None:
+            oprot.writeFieldBegin('optional_match_tensor_expr', TType.STRUCT, 3)
+            self.optional_match_tensor_expr.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
@@ -1721,133 +1965,120 @@
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         return not (self == other)
 
 
-class ConstantExpr(object):
+class SearchExpr(object):
     """
     Attributes:
-     - literal_type
-     - bool_value
-     - i64_value
-     - f64_value
-     - str_value
-     - i64_array_value
-     - f64_array_value
+     - match_exprs
+     - knn_exprs
+     - match_tensor_exprs
+     - fusion_exprs
 
     """
 
 
-    def __init__(self, literal_type=None, bool_value=None, i64_value=None, f64_value=None, str_value=None, i64_array_value=None, f64_array_value=None,):
-        self.literal_type = literal_type
-        self.bool_value = bool_value
-        self.i64_value = i64_value
-        self.f64_value = f64_value
-        self.str_value = str_value
-        self.i64_array_value = i64_array_value
-        self.f64_array_value = f64_array_value
+    def __init__(self, match_exprs=None, knn_exprs=None, match_tensor_exprs=None, fusion_exprs=None,):
+        self.match_exprs = match_exprs
+        self.knn_exprs = knn_exprs
+        self.match_tensor_exprs = match_tensor_exprs
+        self.fusion_exprs = fusion_exprs
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
-                if ftype == TType.I32:
-                    self.literal_type = iprot.readI32()
+                if ftype == TType.LIST:
+                    self.match_exprs = []
+                    (_etype129, _size126) = iprot.readListBegin()
+                    for _i130 in range(_size126):
+                        _elem131 = MatchExpr()
+                        _elem131.read(iprot)
+                        self.match_exprs.append(_elem131)
+                    iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
-                if ftype == TType.BOOL:
-                    self.bool_value = iprot.readBool()
+                if ftype == TType.LIST:
+                    self.knn_exprs = []
+                    (_etype135, _size132) = iprot.readListBegin()
+                    for _i136 in range(_size132):
+                        _elem137 = KnnExpr()
+                        _elem137.read(iprot)
+                        self.knn_exprs.append(_elem137)
+                    iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
-                if ftype == TType.I64:
-                    self.i64_value = iprot.readI64()
-                else:
-                    iprot.skip(ftype)
-            elif fid == 4:
-                if ftype == TType.DOUBLE:
-                    self.f64_value = iprot.readDouble()
-                else:
-                    iprot.skip(ftype)
-            elif fid == 5:
-                if ftype == TType.STRING:
-                    self.str_value = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                else:
-                    iprot.skip(ftype)
-            elif fid == 6:
                 if ftype == TType.LIST:
-                    self.i64_array_value = []
-                    (_etype87, _size84) = iprot.readListBegin()
-                    for _i88 in range(_size84):
-                        _elem89 = iprot.readI64()
-                        self.i64_array_value.append(_elem89)
+                    self.match_tensor_exprs = []
+                    (_etype141, _size138) = iprot.readListBegin()
+                    for _i142 in range(_size138):
+                        _elem143 = MatchTensorExpr()
+                        _elem143.read(iprot)
+                        self.match_tensor_exprs.append(_elem143)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
-            elif fid == 7:
+            elif fid == 4:
                 if ftype == TType.LIST:
-                    self.f64_array_value = []
-                    (_etype93, _size90) = iprot.readListBegin()
-                    for _i94 in range(_size90):
-                        _elem95 = iprot.readDouble()
-                        self.f64_array_value.append(_elem95)
+                    self.fusion_exprs = []
+                    (_etype147, _size144) = iprot.readListBegin()
+                    for _i148 in range(_size144):
+                        _elem149 = FusionExpr()
+                        _elem149.read(iprot)
+                        self.fusion_exprs.append(_elem149)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
-        oprot.writeStructBegin('ConstantExpr')
-        if self.literal_type is not None:
-            oprot.writeFieldBegin('literal_type', TType.I32, 1)
-            oprot.writeI32(self.literal_type)
-            oprot.writeFieldEnd()
-        if self.bool_value is not None:
-            oprot.writeFieldBegin('bool_value', TType.BOOL, 2)
-            oprot.writeBool(self.bool_value)
-            oprot.writeFieldEnd()
-        if self.i64_value is not None:
-            oprot.writeFieldBegin('i64_value', TType.I64, 3)
-            oprot.writeI64(self.i64_value)
-            oprot.writeFieldEnd()
-        if self.f64_value is not None:
-            oprot.writeFieldBegin('f64_value', TType.DOUBLE, 4)
-            oprot.writeDouble(self.f64_value)
+        oprot.writeStructBegin('SearchExpr')
+        if self.match_exprs is not None:
+            oprot.writeFieldBegin('match_exprs', TType.LIST, 1)
+            oprot.writeListBegin(TType.STRUCT, len(self.match_exprs))
+            for iter150 in self.match_exprs:
+                iter150.write(oprot)
+            oprot.writeListEnd()
             oprot.writeFieldEnd()
-        if self.str_value is not None:
-            oprot.writeFieldBegin('str_value', TType.STRING, 5)
-            oprot.writeString(self.str_value.encode('utf-8') if sys.version_info[0] == 2 else self.str_value)
+        if self.knn_exprs is not None:
+            oprot.writeFieldBegin('knn_exprs', TType.LIST, 2)
+            oprot.writeListBegin(TType.STRUCT, len(self.knn_exprs))
+            for iter151 in self.knn_exprs:
+                iter151.write(oprot)
+            oprot.writeListEnd()
             oprot.writeFieldEnd()
-        if self.i64_array_value is not None:
-            oprot.writeFieldBegin('i64_array_value', TType.LIST, 6)
-            oprot.writeListBegin(TType.I64, len(self.i64_array_value))
-            for iter96 in self.i64_array_value:
-                oprot.writeI64(iter96)
+        if self.match_tensor_exprs is not None:
+            oprot.writeFieldBegin('match_tensor_exprs', TType.LIST, 3)
+            oprot.writeListBegin(TType.STRUCT, len(self.match_tensor_exprs))
+            for iter152 in self.match_tensor_exprs:
+                iter152.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
-        if self.f64_array_value is not None:
-            oprot.writeFieldBegin('f64_array_value', TType.LIST, 7)
-            oprot.writeListBegin(TType.DOUBLE, len(self.f64_array_value))
-            for iter97 in self.f64_array_value:
-                oprot.writeDouble(iter97)
+        if self.fusion_exprs is not None:
+            oprot.writeFieldBegin('fusion_exprs', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.fusion_exprs))
+            for iter153 in self.fusion_exprs:
+                iter153.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -1890,19 +2121,19 @@
                 if ftype == TType.STRING:
                     self.function_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.arguments = []
-                    (_etype101, _size98) = iprot.readListBegin()
-                    for _i102 in range(_size98):
-                        _elem103 = ParsedExpr()
-                        _elem103.read(iprot)
-                        self.arguments.append(_elem103)
+                    (_etype157, _size154) = iprot.readListBegin()
+                    for _i158 in range(_size154):
+                        _elem159 = ParsedExpr()
+                        _elem159.read(iprot)
+                        self.arguments.append(_elem159)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -1915,16 +2146,16 @@
         if self.function_name is not None:
             oprot.writeFieldBegin('function_name', TType.STRING, 1)
             oprot.writeString(self.function_name.encode('utf-8') if sys.version_info[0] == 2 else self.function_name)
             oprot.writeFieldEnd()
         if self.arguments is not None:
             oprot.writeFieldBegin('arguments', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.arguments))
-            for iter104 in self.arguments:
-                iter104.write(oprot)
+            for iter160 in self.arguments:
+                iter160.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2208,18 +2439,18 @@
                     self.data_type = DataType()
                     self.data_type.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.constraints = []
-                    (_etype108, _size105) = iprot.readListBegin()
-                    for _i109 in range(_size105):
-                        _elem110 = iprot.readI32()
-                        self.constraints.append(_elem110)
+                    (_etype164, _size161) = iprot.readListBegin()
+                    for _i165 in range(_size161):
+                        _elem166 = iprot.readI32()
+                        self.constraints.append(_elem166)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.constant_expr = ConstantExpr()
                     self.constant_expr.read(iprot)
@@ -2246,16 +2477,16 @@
         if self.data_type is not None:
             oprot.writeFieldBegin('data_type', TType.STRUCT, 3)
             self.data_type.write(oprot)
             oprot.writeFieldEnd()
         if self.constraints is not None:
             oprot.writeFieldBegin('constraints', TType.LIST, 4)
             oprot.writeListBegin(TType.I32, len(self.constraints))
-            for iter111 in self.constraints:
-                oprot.writeI32(iter111)
+            for iter167 in self.constraints:
+                oprot.writeI32(iter167)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.constant_expr is not None:
             oprot.writeFieldBegin('constant_expr', TType.STRUCT, 5)
             self.constant_expr.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2299,19 +2530,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.parse_exprs = []
-                    (_etype115, _size112) = iprot.readListBegin()
-                    for _i116 in range(_size112):
-                        _elem117 = ParsedExpr()
-                        _elem117.read(iprot)
-                        self.parse_exprs.append(_elem117)
+                    (_etype171, _size168) = iprot.readListBegin()
+                    for _i172 in range(_size168):
+                        _elem173 = ParsedExpr()
+                        _elem173.read(iprot)
+                        self.parse_exprs.append(_elem173)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2320,16 +2551,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Field')
         if self.parse_exprs is not None:
             oprot.writeFieldBegin('parse_exprs', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.parse_exprs))
-            for iter118 in self.parse_exprs:
-                iter118.write(oprot)
+            for iter174 in self.parse_exprs:
+                iter174.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2378,18 +2609,18 @@
                 if ftype == TType.I32:
                     self.column_type = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.column_vectors = []
-                    (_etype122, _size119) = iprot.readListBegin()
-                    for _i123 in range(_size119):
-                        _elem124 = iprot.readBinary()
-                        self.column_vectors.append(_elem124)
+                    (_etype178, _size175) = iprot.readListBegin()
+                    for _i179 in range(_size175):
+                        _elem180 = iprot.readBinary()
+                        self.column_vectors.append(_elem180)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRING:
                     self.column_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
@@ -2407,16 +2638,16 @@
         if self.column_type is not None:
             oprot.writeFieldBegin('column_type', TType.I32, 1)
             oprot.writeI32(self.column_type)
             oprot.writeFieldEnd()
         if self.column_vectors is not None:
             oprot.writeFieldBegin('column_vectors', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.column_vectors))
-            for iter125 in self.column_vectors:
-                oprot.writeBinary(iter125)
+            for iter181 in self.column_vectors:
+                oprot.writeBinary(iter181)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.column_name is not None:
             oprot.writeFieldBegin('column_name', TType.STRING, 3)
             oprot.writeString(self.column_name.encode('utf-8') if sys.version_info[0] == 2 else self.column_name)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2814,18 +3045,18 @@
                 if ftype == TType.STRING:
                     self.error_msg = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.db_names = []
-                    (_etype129, _size126) = iprot.readListBegin()
-                    for _i130 in range(_size126):
-                        _elem131 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.db_names.append(_elem131)
+                    (_etype185, _size182) = iprot.readListBegin()
+                    for _i186 in range(_size182):
+                        _elem187 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.db_names.append(_elem187)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2842,16 +3073,16 @@
         if self.error_msg is not None:
             oprot.writeFieldBegin('error_msg', TType.STRING, 2)
             oprot.writeString(self.error_msg.encode('utf-8') if sys.version_info[0] == 2 else self.error_msg)
             oprot.writeFieldEnd()
         if self.db_names is not None:
             oprot.writeFieldBegin('db_names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.db_names))
-            for iter132 in self.db_names:
-                oprot.writeString(iter132.encode('utf-8') if sys.version_info[0] == 2 else iter132)
+            for iter188 in self.db_names:
+                oprot.writeString(iter188.encode('utf-8') if sys.version_info[0] == 2 else iter188)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2973,18 +3204,18 @@
                 if ftype == TType.STRING:
                     self.error_msg = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.table_names = []
-                    (_etype136, _size133) = iprot.readListBegin()
-                    for _i137 in range(_size133):
-                        _elem138 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.table_names.append(_elem138)
+                    (_etype192, _size189) = iprot.readListBegin()
+                    for _i193 in range(_size189):
+                        _elem194 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.table_names.append(_elem194)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3001,16 +3232,16 @@
         if self.error_msg is not None:
             oprot.writeFieldBegin('error_msg', TType.STRING, 2)
             oprot.writeString(self.error_msg.encode('utf-8') if sys.version_info[0] == 2 else self.error_msg)
             oprot.writeFieldEnd()
         if self.table_names is not None:
             oprot.writeFieldBegin('table_names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.table_names))
-            for iter139 in self.table_names:
-                oprot.writeString(iter139.encode('utf-8') if sys.version_info[0] == 2 else iter139)
+            for iter195 in self.table_names:
+                oprot.writeString(iter195.encode('utf-8') if sys.version_info[0] == 2 else iter195)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3143,18 +3374,18 @@
                 if ftype == TType.STRING:
                     self.error_msg = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.index_names = []
-                    (_etype143, _size140) = iprot.readListBegin()
-                    for _i144 in range(_size140):
-                        _elem145 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.index_names.append(_elem145)
+                    (_etype199, _size196) = iprot.readListBegin()
+                    for _i200 in range(_size196):
+                        _elem201 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.index_names.append(_elem201)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3171,16 +3402,16 @@
         if self.error_msg is not None:
             oprot.writeFieldBegin('error_msg', TType.STRING, 2)
             oprot.writeString(self.error_msg.encode('utf-8') if sys.version_info[0] == 2 else self.error_msg)
             oprot.writeFieldEnd()
         if self.index_names is not None:
             oprot.writeFieldBegin('index_names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.index_names))
-            for iter146 in self.index_names:
-                oprot.writeString(iter146.encode('utf-8') if sys.version_info[0] == 2 else iter146)
+            for iter202 in self.index_names:
+                oprot.writeString(iter202.encode('utf-8') if sys.version_info[0] == 2 else iter202)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3774,19 +4005,19 @@
                 if ftype == TType.I32:
                     self.index_type = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.index_param_list = []
-                    (_etype150, _size147) = iprot.readListBegin()
-                    for _i151 in range(_size147):
-                        _elem152 = InitParameter()
-                        _elem152.read(iprot)
-                        self.index_param_list.append(_elem152)
+                    (_etype206, _size203) = iprot.readListBegin()
+                    for _i207 in range(_size203):
+                        _elem208 = InitParameter()
+                        _elem208.read(iprot)
+                        self.index_param_list.append(_elem208)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3803,16 +4034,16 @@
         if self.index_type is not None:
             oprot.writeFieldBegin('index_type', TType.I32, 2)
             oprot.writeI32(self.index_type)
             oprot.writeFieldEnd()
         if self.index_param_list is not None:
             oprot.writeFieldBegin('index_param_list', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.index_param_list))
-            for iter153 in self.index_param_list:
-                iter153.write(oprot)
+            for iter209 in self.index_param_list:
+                iter209.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3877,19 +4108,19 @@
                 if ftype == TType.STRING:
                     self.index_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.index_info_list = []
-                    (_etype157, _size154) = iprot.readListBegin()
-                    for _i158 in range(_size154):
-                        _elem159 = IndexInfo()
-                        _elem159.read(iprot)
-                        self.index_info_list.append(_elem159)
+                    (_etype213, _size210) = iprot.readListBegin()
+                    for _i214 in range(_size210):
+                        _elem215 = IndexInfo()
+                        _elem215.read(iprot)
+                        self.index_info_list.append(_elem215)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.I64:
                     self.session_id = iprot.readI64()
                 else:
@@ -3921,16 +4152,16 @@
         if self.index_name is not None:
             oprot.writeFieldBegin('index_name', TType.STRING, 3)
             oprot.writeString(self.index_name.encode('utf-8') if sys.version_info[0] == 2 else self.index_name)
             oprot.writeFieldEnd()
         if self.index_info_list is not None:
             oprot.writeFieldBegin('index_info_list', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.index_info_list))
-            for iter160 in self.index_info_list:
-                iter160.write(oprot)
+            for iter216 in self.index_info_list:
+                iter216.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.session_id is not None:
             oprot.writeFieldBegin('session_id', TType.I64, 6)
             oprot.writeI64(self.session_id)
             oprot.writeFieldEnd()
         if self.create_option is not None:
@@ -4594,19 +4825,19 @@
                 if ftype == TType.STRING:
                     self.table_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.column_defs = []
-                    (_etype164, _size161) = iprot.readListBegin()
-                    for _i165 in range(_size161):
-                        _elem166 = ColumnDef()
-                        _elem166.read(iprot)
-                        self.column_defs.append(_elem166)
+                    (_etype220, _size217) = iprot.readListBegin()
+                    for _i221 in range(_size217):
+                        _elem222 = ColumnDef()
+                        _elem222.read(iprot)
+                        self.column_defs.append(_elem222)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.I64:
                     self.session_id = iprot.readI64()
                 else:
@@ -4634,16 +4865,16 @@
         if self.table_name is not None:
             oprot.writeFieldBegin('table_name', TType.STRING, 2)
             oprot.writeString(self.table_name.encode('utf-8') if sys.version_info[0] == 2 else self.table_name)
             oprot.writeFieldEnd()
         if self.column_defs is not None:
             oprot.writeFieldBegin('column_defs', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.column_defs))
-            for iter167 in self.column_defs:
-                iter167.write(oprot)
+            for iter223 in self.column_defs:
+                iter223.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.session_id is not None:
             oprot.writeFieldBegin('session_id', TType.I64, 6)
             oprot.writeI64(self.session_id)
             oprot.writeFieldEnd()
         if self.create_option is not None:
@@ -4804,29 +5035,29 @@
                 if ftype == TType.STRING:
                     self.table_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.column_names = []
-                    (_etype171, _size168) = iprot.readListBegin()
-                    for _i172 in range(_size168):
-                        _elem173 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.column_names.append(_elem173)
+                    (_etype227, _size224) = iprot.readListBegin()
+                    for _i228 in range(_size224):
+                        _elem229 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.column_names.append(_elem229)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype177, _size174) = iprot.readListBegin()
-                    for _i178 in range(_size174):
-                        _elem179 = Field()
-                        _elem179.read(iprot)
-                        self.fields.append(_elem179)
+                    (_etype233, _size230) = iprot.readListBegin()
+                    for _i234 in range(_size230):
+                        _elem235 = Field()
+                        _elem235.read(iprot)
+                        self.fields.append(_elem235)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.I64:
                     self.session_id = iprot.readI64()
                 else:
@@ -4848,23 +5079,23 @@
         if self.table_name is not None:
             oprot.writeFieldBegin('table_name', TType.STRING, 2)
             oprot.writeString(self.table_name.encode('utf-8') if sys.version_info[0] == 2 else self.table_name)
             oprot.writeFieldEnd()
         if self.column_names is not None:
             oprot.writeFieldBegin('column_names', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.column_names))
-            for iter180 in self.column_names:
-                oprot.writeString(iter180.encode('utf-8') if sys.version_info[0] == 2 else iter180)
+            for iter236 in self.column_names:
+                oprot.writeString(iter236.encode('utf-8') if sys.version_info[0] == 2 else iter236)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter181 in self.fields:
-                iter181.write(oprot)
+            for iter237 in self.fields:
+                iter237.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.session_id is not None:
             oprot.writeFieldBegin('session_id', TType.I64, 5)
             oprot.writeI64(self.session_id)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5066,19 +5297,19 @@
                 if ftype == TType.STRING:
                     self.table_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.select_list = []
-                    (_etype185, _size182) = iprot.readListBegin()
-                    for _i186 in range(_size182):
-                        _elem187 = ParsedExpr()
-                        _elem187.read(iprot)
-                        self.select_list.append(_elem187)
+                    (_etype241, _size238) = iprot.readListBegin()
+                    for _i242 in range(_size238):
+                        _elem243 = ParsedExpr()
+                        _elem243.read(iprot)
+                        self.select_list.append(_elem243)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.search_expr = SearchExpr()
                     self.search_expr.read(iprot)
@@ -5089,19 +5320,19 @@
                     self.where_expr = ParsedExpr()
                     self.where_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.group_by_list = []
-                    (_etype191, _size188) = iprot.readListBegin()
-                    for _i192 in range(_size188):
-                        _elem193 = ParsedExpr()
-                        _elem193.read(iprot)
-                        self.group_by_list.append(_elem193)
+                    (_etype247, _size244) = iprot.readListBegin()
+                    for _i248 in range(_size244):
+                        _elem249 = ParsedExpr()
+                        _elem249.read(iprot)
+                        self.group_by_list.append(_elem249)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.STRUCT:
                     self.having_expr = ParsedExpr()
                     self.having_expr.read(iprot)
@@ -5118,19 +5349,19 @@
                     self.offset_expr = ParsedExpr()
                     self.offset_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 11:
                 if ftype == TType.LIST:
                     self.order_by_list = []
-                    (_etype197, _size194) = iprot.readListBegin()
-                    for _i198 in range(_size194):
-                        _elem199 = OrderByExpr()
-                        _elem199.read(iprot)
-                        self.order_by_list.append(_elem199)
+                    (_etype253, _size250) = iprot.readListBegin()
+                    for _i254 in range(_size250):
+                        _elem255 = OrderByExpr()
+                        _elem255.read(iprot)
+                        self.order_by_list.append(_elem255)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 12:
                 if ftype == TType.I32:
                     self.explain_type = iprot.readI32()
                 else:
@@ -5156,31 +5387,31 @@
         if self.table_name is not None:
             oprot.writeFieldBegin('table_name', TType.STRING, 3)
             oprot.writeString(self.table_name.encode('utf-8') if sys.version_info[0] == 2 else self.table_name)
             oprot.writeFieldEnd()
         if self.select_list is not None:
             oprot.writeFieldBegin('select_list', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.select_list))
-            for iter200 in self.select_list:
-                iter200.write(oprot)
+            for iter256 in self.select_list:
+                iter256.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.search_expr is not None:
             oprot.writeFieldBegin('search_expr', TType.STRUCT, 5)
             self.search_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.where_expr is not None:
             oprot.writeFieldBegin('where_expr', TType.STRUCT, 6)
             self.where_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.group_by_list is not None:
             oprot.writeFieldBegin('group_by_list', TType.LIST, 7)
             oprot.writeListBegin(TType.STRUCT, len(self.group_by_list))
-            for iter201 in self.group_by_list:
-                iter201.write(oprot)
+            for iter257 in self.group_by_list:
+                iter257.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.having_expr is not None:
             oprot.writeFieldBegin('having_expr', TType.STRUCT, 8)
             self.having_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.limit_expr is not None:
@@ -5190,16 +5421,16 @@
         if self.offset_expr is not None:
             oprot.writeFieldBegin('offset_expr', TType.STRUCT, 10)
             self.offset_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.order_by_list is not None:
             oprot.writeFieldBegin('order_by_list', TType.LIST, 11)
             oprot.writeListBegin(TType.STRUCT, len(self.order_by_list))
-            for iter202 in self.order_by_list:
-                iter202.write(oprot)
+            for iter258 in self.order_by_list:
+                iter258.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.explain_type is not None:
             oprot.writeFieldBegin('explain_type', TType.I32, 12)
             oprot.writeI32(self.explain_type)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5263,30 +5494,30 @@
                 if ftype == TType.STRING:
                     self.error_msg = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.column_defs = []
-                    (_etype206, _size203) = iprot.readListBegin()
-                    for _i207 in range(_size203):
-                        _elem208 = ColumnDef()
-                        _elem208.read(iprot)
-                        self.column_defs.append(_elem208)
+                    (_etype262, _size259) = iprot.readListBegin()
+                    for _i263 in range(_size259):
+                        _elem264 = ColumnDef()
+                        _elem264.read(iprot)
+                        self.column_defs.append(_elem264)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.column_fields = []
-                    (_etype212, _size209) = iprot.readListBegin()
-                    for _i213 in range(_size209):
-                        _elem214 = ColumnField()
-                        _elem214.read(iprot)
-                        self.column_fields.append(_elem214)
+                    (_etype268, _size265) = iprot.readListBegin()
+                    for _i269 in range(_size265):
+                        _elem270 = ColumnField()
+                        _elem270.read(iprot)
+                        self.column_fields.append(_elem270)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5303,23 +5534,23 @@
         if self.error_msg is not None:
             oprot.writeFieldBegin('error_msg', TType.STRING, 2)
             oprot.writeString(self.error_msg.encode('utf-8') if sys.version_info[0] == 2 else self.error_msg)
             oprot.writeFieldEnd()
         if self.column_defs is not None:
             oprot.writeFieldBegin('column_defs', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.column_defs))
-            for iter215 in self.column_defs:
-                iter215.write(oprot)
+            for iter271 in self.column_defs:
+                iter271.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.column_fields is not None:
             oprot.writeFieldBegin('column_fields', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.column_fields))
-            for iter216 in self.column_fields:
-                iter216.write(oprot)
+            for iter272 in self.column_fields:
+                iter272.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5402,19 +5633,19 @@
                 if ftype == TType.STRING:
                     self.table_name = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.select_list = []
-                    (_etype220, _size217) = iprot.readListBegin()
-                    for _i221 in range(_size217):
-                        _elem222 = ParsedExpr()
-                        _elem222.read(iprot)
-                        self.select_list.append(_elem222)
+                    (_etype276, _size273) = iprot.readListBegin()
+                    for _i277 in range(_size273):
+                        _elem278 = ParsedExpr()
+                        _elem278.read(iprot)
+                        self.select_list.append(_elem278)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.STRUCT:
                     self.search_expr = SearchExpr()
                     self.search_expr.read(iprot)
@@ -5425,19 +5656,19 @@
                     self.where_expr = ParsedExpr()
                     self.where_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.group_by_list = []
-                    (_etype226, _size223) = iprot.readListBegin()
-                    for _i227 in range(_size223):
-                        _elem228 = ParsedExpr()
-                        _elem228.read(iprot)
-                        self.group_by_list.append(_elem228)
+                    (_etype282, _size279) = iprot.readListBegin()
+                    for _i283 in range(_size279):
+                        _elem284 = ParsedExpr()
+                        _elem284.read(iprot)
+                        self.group_by_list.append(_elem284)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 8:
                 if ftype == TType.STRUCT:
                     self.having_expr = ParsedExpr()
                     self.having_expr.read(iprot)
@@ -5454,19 +5685,19 @@
                     self.offset_expr = ParsedExpr()
                     self.offset_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 11:
                 if ftype == TType.LIST:
                     self.order_by_list = []
-                    (_etype232, _size229) = iprot.readListBegin()
-                    for _i233 in range(_size229):
-                        _elem234 = OrderByExpr()
-                        _elem234.read(iprot)
-                        self.order_by_list.append(_elem234)
+                    (_etype288, _size285) = iprot.readListBegin()
+                    for _i289 in range(_size285):
+                        _elem290 = OrderByExpr()
+                        _elem290.read(iprot)
+                        self.order_by_list.append(_elem290)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5487,31 +5718,31 @@
         if self.table_name is not None:
             oprot.writeFieldBegin('table_name', TType.STRING, 3)
             oprot.writeString(self.table_name.encode('utf-8') if sys.version_info[0] == 2 else self.table_name)
             oprot.writeFieldEnd()
         if self.select_list is not None:
             oprot.writeFieldBegin('select_list', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.select_list))
-            for iter235 in self.select_list:
-                iter235.write(oprot)
+            for iter291 in self.select_list:
+                iter291.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.search_expr is not None:
             oprot.writeFieldBegin('search_expr', TType.STRUCT, 5)
             self.search_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.where_expr is not None:
             oprot.writeFieldBegin('where_expr', TType.STRUCT, 6)
             self.where_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.group_by_list is not None:
             oprot.writeFieldBegin('group_by_list', TType.LIST, 7)
             oprot.writeListBegin(TType.STRUCT, len(self.group_by_list))
-            for iter236 in self.group_by_list:
-                iter236.write(oprot)
+            for iter292 in self.group_by_list:
+                iter292.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.having_expr is not None:
             oprot.writeFieldBegin('having_expr', TType.STRUCT, 8)
             self.having_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.limit_expr is not None:
@@ -5521,16 +5752,16 @@
         if self.offset_expr is not None:
             oprot.writeFieldBegin('offset_expr', TType.STRUCT, 10)
             self.offset_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.order_by_list is not None:
             oprot.writeFieldBegin('order_by_list', TType.LIST, 11)
             oprot.writeListBegin(TType.STRUCT, len(self.order_by_list))
-            for iter237 in self.order_by_list:
-                iter237.write(oprot)
+            for iter293 in self.order_by_list:
+                iter293.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5590,30 +5821,30 @@
                 if ftype == TType.STRING:
                     self.error_msg = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.column_defs = []
-                    (_etype241, _size238) = iprot.readListBegin()
-                    for _i242 in range(_size238):
-                        _elem243 = ColumnDef()
-                        _elem243.read(iprot)
-                        self.column_defs.append(_elem243)
+                    (_etype297, _size294) = iprot.readListBegin()
+                    for _i298 in range(_size294):
+                        _elem299 = ColumnDef()
+                        _elem299.read(iprot)
+                        self.column_defs.append(_elem299)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.column_fields = []
-                    (_etype247, _size244) = iprot.readListBegin()
-                    for _i248 in range(_size244):
-                        _elem249 = ColumnField()
-                        _elem249.read(iprot)
-                        self.column_fields.append(_elem249)
+                    (_etype303, _size300) = iprot.readListBegin()
+                    for _i304 in range(_size300):
+                        _elem305 = ColumnField()
+                        _elem305.read(iprot)
+                        self.column_fields.append(_elem305)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5630,23 +5861,23 @@
         if self.error_msg is not None:
             oprot.writeFieldBegin('error_msg', TType.STRING, 2)
             oprot.writeString(self.error_msg.encode('utf-8') if sys.version_info[0] == 2 else self.error_msg)
             oprot.writeFieldEnd()
         if self.column_defs is not None:
             oprot.writeFieldBegin('column_defs', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.column_defs))
-            for iter250 in self.column_defs:
-                iter250.write(oprot)
+            for iter306 in self.column_defs:
+                iter306.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.column_fields is not None:
             oprot.writeFieldBegin('column_fields', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.column_fields))
-            for iter251 in self.column_fields:
-                iter251.write(oprot)
+            for iter307 in self.column_fields:
+                iter307.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5801,19 +6032,19 @@
                     self.where_expr = ParsedExpr()
                     self.where_expr.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.update_expr_array = []
-                    (_etype255, _size252) = iprot.readListBegin()
-                    for _i256 in range(_size252):
-                        _elem257 = UpdateExpr()
-                        _elem257.read(iprot)
-                        self.update_expr_array.append(_elem257)
+                    (_etype311, _size308) = iprot.readListBegin()
+                    for _i312 in range(_size308):
+                        _elem313 = UpdateExpr()
+                        _elem313.read(iprot)
+                        self.update_expr_array.append(_elem313)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.I64:
                     self.session_id = iprot.readI64()
                 else:
@@ -5839,16 +6070,16 @@
         if self.where_expr is not None:
             oprot.writeFieldBegin('where_expr', TType.STRUCT, 3)
             self.where_expr.write(oprot)
             oprot.writeFieldEnd()
         if self.update_expr_array is not None:
             oprot.writeFieldBegin('update_expr_array', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.update_expr_array))
-            for iter258 in self.update_expr_array:
-                iter258.write(oprot)
+            for iter314 in self.update_expr_array:
+                iter314.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.session_id is not None:
             oprot.writeFieldBegin('session_id', TType.I64, 5)
             oprot.writeI64(self.session_id)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -6923,55 +7154,68 @@
 )
 all_structs.append(InitParameter)
 InitParameter.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'param_name', 'UTF8', None, ),  # 1
     (2, TType.STRING, 'param_value', 'UTF8', None, ),  # 2
 )
+all_structs.append(ConstantExpr)
+ConstantExpr.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'literal_type', None, None, ),  # 1
+    (2, TType.BOOL, 'bool_value', None, None, ),  # 2
+    (3, TType.I64, 'i64_value', None, None, ),  # 3
+    (4, TType.DOUBLE, 'f64_value', None, None, ),  # 4
+    (5, TType.STRING, 'str_value', 'UTF8', None, ),  # 5
+    (6, TType.LIST, 'i64_array_value', (TType.I64, None, False), None, ),  # 6
+    (7, TType.LIST, 'f64_array_value', (TType.DOUBLE, None, False), None, ),  # 7
+    (8, TType.LIST, 'i64_tensor_array_value', (TType.LIST, (TType.LIST, (TType.I64, None, False), False), False), None, ),  # 8
+    (9, TType.LIST, 'f64_tensor_array_value', (TType.LIST, (TType.LIST, (TType.DOUBLE, None, False), False), False), None, ),  # 9
+)
 all_structs.append(KnnExpr)
 KnnExpr.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'column_expr', [ColumnExpr, None], None, ),  # 1
     (2, TType.STRUCT, 'embedding_data', [EmbeddingData, None], None, ),  # 2
     (3, TType.I32, 'embedding_data_type', None, None, ),  # 3
     (4, TType.I32, 'distance_type', None, None, ),  # 4
     (5, TType.I64, 'topn', None, None, ),  # 5
     (6, TType.LIST, 'opt_params', (TType.STRUCT, [InitParameter, None], False), [
     ], ),  # 6
 )
+all_structs.append(MatchTensorExpr)
+MatchTensorExpr.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'search_method', 'UTF8', None, ),  # 1
+    (2, TType.STRUCT, 'column_expr', [ColumnExpr, None], None, ),  # 2
+    (3, TType.I32, 'embedding_data_type', None, None, ),  # 3
+    (4, TType.STRUCT, 'embedding_data', [EmbeddingData, None], None, ),  # 4
+    (5, TType.STRING, 'extra_options', 'UTF8', None, ),  # 5
+)
 all_structs.append(MatchExpr)
 MatchExpr.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'fields', 'UTF8', None, ),  # 1
     (2, TType.STRING, 'matching_text', 'UTF8', None, ),  # 2
     (3, TType.STRING, 'options_text', 'UTF8', None, ),  # 3
 )
 all_structs.append(FusionExpr)
 FusionExpr.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'method', 'UTF8', None, ),  # 1
     (2, TType.STRING, 'options_text', 'UTF8', None, ),  # 2
+    (3, TType.STRUCT, 'optional_match_tensor_expr', [MatchTensorExpr, None], None, ),  # 3
 )
 all_structs.append(SearchExpr)
 SearchExpr.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'match_exprs', (TType.STRUCT, [MatchExpr, None], False), None, ),  # 1
     (2, TType.LIST, 'knn_exprs', (TType.STRUCT, [KnnExpr, None], False), None, ),  # 2
-    (3, TType.STRUCT, 'fusion_expr', [FusionExpr, None], None, ),  # 3
-)
-all_structs.append(ConstantExpr)
-ConstantExpr.thrift_spec = (
-    None,  # 0
-    (1, TType.I32, 'literal_type', None, None, ),  # 1
-    (2, TType.BOOL, 'bool_value', None, None, ),  # 2
-    (3, TType.I64, 'i64_value', None, None, ),  # 3
-    (4, TType.DOUBLE, 'f64_value', None, None, ),  # 4
-    (5, TType.STRING, 'str_value', 'UTF8', None, ),  # 5
-    (6, TType.LIST, 'i64_array_value', (TType.I64, None, False), None, ),  # 6
-    (7, TType.LIST, 'f64_array_value', (TType.DOUBLE, None, False), None, ),  # 7
+    (3, TType.LIST, 'match_tensor_exprs', (TType.STRUCT, [MatchTensorExpr, None], False), None, ),  # 3
+    (4, TType.LIST, 'fusion_exprs', (TType.STRUCT, [FusionExpr, None], False), None, ),  # 4
 )
 all_structs.append(FunctionExpr)
 FunctionExpr.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'function_name', 'UTF8', None, ),  # 1
     (2, TType.LIST, 'arguments', (TType.STRUCT, [ParsedExpr, None], False), None, ),  # 2
 )
```

## Comparing `infinity_sdk-0.2.0.dev2.dist-info/METADATA` & `infinity_sdk-0.2.0.dev3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinity_sdk
-Version: 0.2.0.dev2
+Version: 0.2.0.dev3
 Summary: infinity
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: sqlglot ~=11.7.1
 Requires-Dist: pydantic ~=2.7.1
 Requires-Dist: thrift ~=0.20.0
 Requires-Dist: setuptools ~=69.5.1
```

## Comparing `infinity_sdk-0.2.0.dev2.dist-info/RECORD` & `infinity_sdk-0.2.0.dev3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 infinity/db.py,sha256=WFZ_BcofXmsxUtV6PyKrOsAwrtkBbXse9RclA590QJw,1387
 infinity/errors.py,sha256=xbx5Sr6hvJ-k2eNCxpYxB8bXqwbOekiER3MOfNHoow8,4527
 infinity/index.py,sha256=XQdc-tCNZ8Zbpvc6ZJdFVnzdQCI_yN8gJluiwf-8CeM,2481
 infinity/infinity.py,sha256=XAS6KQvYlRtpL8SFSbcRcCpwHzB6CcPXtkZxTjwL5hE,1237
 infinity/table.py,sha256=5mZPz8MQDUYV8VWyfXJkTmf3RXZXF9zDLbCy69pZcmM,2487
 infinity/utils.py,sha256=qUy-uwvggvNPrv6lb2YWzu65ewGcolWOUG7uGkjt7qI,1515
 infinity/remote_thrift/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-infinity/remote_thrift/client.py,sha256=Rpy1AfA0L0lUG2XeIDucA6xQuldLNiiaqijxRPgJBO4,13794
+infinity/remote_thrift/client.py,sha256=RhS4i5lFyU_M-WhtGNeMUEKtS31yyptN_fVIUbkbaiI,13987
 infinity/remote_thrift/common.py,sha256=4eyCmKtUP3dNyZmtIPoCc05AAseuJsfqgfTQ6aY9iag,680
-infinity/remote_thrift/db.py,sha256=wjXDb65FPzyF8OZKayPBAB6gF0_75fjg8sMacBUiL_Y,12826
+infinity/remote_thrift/db.py,sha256=FRRQXuARYd55O1oNpCzmi8xGQNoLSRB6PTAXot0Aovg,13148
 infinity/remote_thrift/infinity.py,sha256=FBpOc1KgLJcBTeLpVHWKGwA26vzq4TdoTVrV1j3-sCk,4167
-infinity/remote_thrift/query_builder.py,sha256=aGu4MDfUcnHILWvfmwBGePEiIQYFRtKDNUmyNB6y9Yk,10027
-infinity/remote_thrift/table.py,sha256=0T42krWSjuk5u90soqvoaOaOjB2EWxVdbUG90FeALKE,18214
-infinity/remote_thrift/types.py,sha256=OC8kYe_knx4YnWd0WPe7ruot_SDS_uQTeUnoLe-w2ow,10201
+infinity/remote_thrift/query_builder.py,sha256=ECPemHsF9zRxvgUrNxSXBGN44SAtWKmroYz0n8c9Jjc,11523
+infinity/remote_thrift/table.py,sha256=1U_AWGZ5NlDJpuKPsGQYPgeSi2BDDxPJ0WyhfYGc1FA,19944
+infinity/remote_thrift/types.py,sha256=b4OLPQ5I0nHIdn4_v0kswGPN3F54hMzJQvVGlQ5nGwY,16026
 infinity/remote_thrift/utils.py,sha256=aHAqrMhEbls80T56NUvJJji4ZqZ0r6SMxT5AaYES-fo,7763
 infinity/remote_thrift/infinity_thrift_rpc/InfinityService.py,sha256=zZq0vvzQVVL8MvuK05LhkLNH-_KHyY-iT54B2saUB-U,178466
 infinity/remote_thrift/infinity_thrift_rpc/__init__.py,sha256=ezRvowu7Yojw8xly58EOLQ3_40IK5XUqusB8XPoRlF4,53
 infinity/remote_thrift/infinity_thrift_rpc/constants.py,sha256=fEiYY_X50Lqtkoew_h1qWBH5QmDiygExYB-6WRsifqg,366
-infinity/remote_thrift/infinity_thrift_rpc/ttypes.py,sha256=DYKegXJnLPJMPGoTFj8OUjSjxgH8e0S2da2yuLvfMnc,274464
-infinity_sdk-0.2.0.dev2.dist-info/METADATA,sha256=PCOrt_F-gZ_JJycspmGZ57rgLyQo5expbFZZ-Txy1GA,2241
-infinity_sdk-0.2.0.dev2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-infinity_sdk-0.2.0.dev2.dist-info/top_level.txt,sha256=I5UhBoCrOOXaJN_xGXGoA73npSJ-IRiqYdRL8NYf5VY,9
-infinity_sdk-0.2.0.dev2.dist-info/RECORD,,
+infinity/remote_thrift/infinity_thrift_rpc/ttypes.py,sha256=qTv0Xv0-v5qhSBHaDW0k4sX11MELdLj_b0DJT7y0fYc,285540
+infinity_sdk-0.2.0.dev3.dist-info/METADATA,sha256=gVgcxYQP_2ny62T0sUMAWXC6SocsA5ym2qJF_84imfA,2241
+infinity_sdk-0.2.0.dev3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+infinity_sdk-0.2.0.dev3.dist-info/top_level.txt,sha256=I5UhBoCrOOXaJN_xGXGoA73npSJ-IRiqYdRL8NYf5VY,9
+infinity_sdk-0.2.0.dev3.dist-info/RECORD,,
```

