# Comparing `tmp/metasequoia-sql-0.5.0.tar.gz` & `tmp/metasequoia-sql-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.5.0.tar", last modified: Mon May 13 00:45:31 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.6.0.tar", last modified: Thu May 30 00:40:11 2024, max compression
```

## Comparing `metasequoia-sql-0.5.0.tar` & `metasequoia-sql-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/
--rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     3449 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2024-05-13 00:44:26.000000 metasequoia-sql-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.196271 metasequoia-sql-0.5.0/metasequoia_sql/
--rw-rw-rw-   0        0        0      249 2024-05-12 04:36:10.000000 metasequoia-sql-0.5.0/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.199192 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/
--rw-rw-rw-   0        0        0      499 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/__init__.py
--rw-rw-rw-   0        0        0     4524 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/base.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.201138 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/
--rw-rw-rw-   0        0        0       33 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/__init__.py
--rw-rw-rw-   0        0        0     6767 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage.py
--rw-rw-rw-   0        0        0    18047 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py
--rw-rw-rw-   0        0        0     1835 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py
--rw-rw-rw-   0        0        0     2666 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/node.py
--rw-rw-rw-   0        0        0     2959 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/tool.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.203085 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/
--rw-rw-rw-   0        0        0      345 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/__init__.py
--rw-rw-rw-   0        0        0     2162 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/all_level_standard_table.py
--rw-rw-rw-   0        0        0     9530 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_column_analyzer.py
--rw-rw-rw-   0        0        0     1333 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py
--rw-rw-rw-   0        0        0     2242 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py
--rw-rw-rw-   0        0        0     2875 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.206005 metasequoia-sql-0.5.0/metasequoia_sql/common/
--rw-rw-rw-   0        0        0      142 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/__init__.py
--rw-rw-rw-   0        0        0     3068 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/basic.py
--rw-rw-rw-   0        0        0      860 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/char_set.py
--rw-rw-rw-   0        0        0      812 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/name_set.py
--rw-rw-rw-   0        0        0     7781 2024-05-12 04:36:10.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/scanner.py
--rw-rw-rw-   0        0        0     6414 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/common/static.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.207952 metasequoia-sql-0.5.0/metasequoia_sql/core/
--rw-rw-rw-   0        0        0      173 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/__init__.py
--rw-rw-rw-   0        0        0    88182 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/node.py
--rw-rw-rw-   0        0        0   114838 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/parser.py
--rw-rw-rw-   0        0        0      295 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/core/sql_type.py
--rw-rw-rw-   0        0        0      683 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.209899 metasequoia-sql-0.5.0/metasequoia_sql/lexical/
--rw-rw-rw-   0        0        0      421 2024-05-04 02:49:22.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/__init__.py
--rw-rw-rw-   0        0        0     4196 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/amt_node.py
--rw-rw-rw-   0        0        0     6824 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_machine.py
--rw-rw-rw-   0        0        0     4247 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_operate.py
--rw-rw-rw-   0        0        0    13589 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_operation_map.py
--rw-rw-rw-   0        0        0     2404 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_status.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.210872 metasequoia-sql-0.5.0/metasequoia_sql/plugins/
--rw-rw-rw-   0        0        0        0 2024-05-01 05:05:38.000000 metasequoia-sql-0.5.0/metasequoia_sql/plugins/__init__.py
--rw-rw-rw-   0        0        0     5778 2024-05-12 04:35:14.000000 metasequoia-sql-0.5.0/metasequoia_sql/plugins/mybaitis.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     3449 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 00:45:31.000000 metasequoia-sql-0.5.0/metasequoia_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 00:45:31.211845 metasequoia-sql-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-05-13 00:45:17.000000 metasequoia-sql-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.992098 metasequoia-sql-0.6.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     6427 2024-05-30 00:40:11.992098 metasequoia-sql-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5548 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.977497 metasequoia-sql-0.6.0/metasequoia_sql/
+-rw-rw-rw-   0        0        0      249 2024-05-12 04:36:10.000000 metasequoia-sql-0.6.0/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.980417 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/
+-rw-rw-rw-   0        0        0      499 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     4524 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/base.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.982364 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/
+-rw-rw-rw-   0        0        0       33 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/__init__.py
+-rw-rw-rw-   0        0        0     6767 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/table_lineage.py
+-rw-rw-rw-   0        0        0    18057 2024-05-19 15:47:46.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py
+-rw-rw-rw-   0        0        0     1835 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py
+-rw-rw-rw-   0        0        0     2666 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/node.py
+-rw-rw-rw-   0        0        0     2959 2024-05-12 04:35:14.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.984310 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/
+-rw-rw-rw-   0        0        0      345 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/all_level_standard_table.py
+-rw-rw-rw-   0        0        0     9540 2024-05-19 15:47:46.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_column_analyzer.py
+-rw-rw-rw-   0        0        0     1323 2024-05-19 06:32:02.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py
+-rw-rw-rw-   0        0        0     2242 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py
+-rw-rw-rw-   0        0        0     2875 2024-05-19 15:47:46.000000 metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.987231 metasequoia-sql-0.6.0/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0      142 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0     3068 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0      860 2024-05-12 04:35:14.000000 metasequoia-sql-0.6.0/metasequoia_sql/common/char_set.py
+-rw-rw-rw-   0        0        0      812 2024-05-12 04:35:14.000000 metasequoia-sql-0.6.0/metasequoia_sql/common/name_set.py
+-rw-rw-rw-   0        0        0    10952 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/common/scanner.py
+-rw-rw-rw-   0        0        0     6414 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/common/static.py
+-rw-rw-rw-   0        0        0      501 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/config.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.989178 metasequoia-sql-0.6.0/metasequoia_sql/core/
+-rw-rw-rw-   0        0        0      173 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/core/__init__.py
+-rw-rw-rw-   0        0        0    89021 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/core/node.py
+-rw-rw-rw-   0        0        0   124135 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/core/parser.py
+-rw-rw-rw-   0        0        0      295 2024-05-04 02:49:22.000000 metasequoia-sql-0.6.0/metasequoia_sql/core/sql_type.py
+-rw-rw-rw-   0        0        0     8758 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/core/static.py
+-rw-rw-rw-   0        0        0     1533 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.991124 metasequoia-sql-0.6.0/metasequoia_sql/lexical/
+-rw-rw-rw-   0        0        0      514 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/__init__.py
+-rw-rw-rw-   0        0        0     5348 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/amt_node.py
+-rw-rw-rw-   0        0        0     2716 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_machine.py
+-rw-rw-rw-   0        0        0      879 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_memory.py
+-rw-rw-rw-   0        0        0    12053 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_operate.py
+-rw-rw-rw-   0        0        0    15235 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_operation_map.py
+-rw-rw-rw-   0        0        0     2594 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_status.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.991124 metasequoia-sql-0.6.0/metasequoia_sql/plugins/
+-rw-rw-rw-   0        0        0        0 2024-05-01 05:05:38.000000 metasequoia-sql-0.6.0/metasequoia_sql/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4677 2024-05-30 00:38:37.000000 metasequoia-sql-0.6.0/metasequoia_sql/plugins/mybaitis.py
+drwxrwxrwx   0        0        0        0 2024-05-30 00:40:11.992098 metasequoia-sql-0.6.0/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     6427 2024-05-30 00:40:11.000000 metasequoia-sql-0.6.0/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2024-05-30 00:40:11.000000 metasequoia-sql-0.6.0/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 00:40:11.000000 metasequoia-sql-0.6.0/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 00:40:11.000000 metasequoia-sql-0.6.0/metasequoia_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 00:40:11.992098 metasequoia-sql-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-05-30 00:39:11.000000 metasequoia-sql-0.6.0/setup.py
```

### Comparing `metasequoia-sql-0.5.0/LICENSE` & `metasequoia-sql-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/base.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/table_lineage.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/table_lineage_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                         for from_standard_column in table_lineage.get_all_standard_columns():
                             standard_column = StandardColumn(column_name=from_standard_column.column_name,
                                                              column_idx=column_idx)
                             column_idx += 1
                             quote_column = QuoteColumn(table_name=standard_table.table_name,
                                                        column_name=from_standard_column.column_name)
                             result.append((standard_column, [quote_column]))
-            elif isinstance(column.value, core.ASTColumnName):  # 直接使用字段的情况
+            elif isinstance(column.value, core.ASTColumnNameExpression):  # 直接使用字段的情况
                 standard_column = StandardColumn(column_name=column.value.column_name, column_idx=column_idx)
                 column_idx += 1
                 quote_column = QuoteColumn(table_name=column.value.table_name,
                                            column_name=column.value.column_name)
                 result.append((standard_column, [quote_column]))
             else:  # 不是字段名的情况（此时一定不是通配符）
                 standard_column = StandardColumn(column_name=column.value.source(),
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/data_linage/table_lineage_storage.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/node.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/node.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/tool.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/tool.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/all_level_standard_table.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/all_level_standard_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class AllUsedQuoteTables(AnalyzerRecursionASTToListBase):
     """"获取所有层级（递归分析子查询）中，直接使用的表名（仅包含原始表名）"""
 
     @classmethod
     def handle(cls, node: Union[core.ASTBase, tuple]) -> List[StandardTable]:
         """自定义的处理规则"""
-        if isinstance(node, core.ASTTableName):
+        if isinstance(node, core.ASTTableNameExpression):
             return [StandardTable(schema_name=node.schema_name, table_name=node.table_name)]
         return cls.default_handle_node(node)
 
 
 class AllFromClauseUsedQuoteColumn(AnalyzerSelectASTToListBase):
     """获取所有层级（递归分析子查询）的 FROM 子句中，直接使用的表名（仅包含原始表名）"""
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_column_analyzer.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_column_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     @classmethod
     def handle_single_select_statement(cls, node: core.ASTSingleSelectStatement
                                        ) -> Dict[StandardColumn, List[QuoteColumn]]:
         result = {}
         for column_idx, column_expression in enumerate(node.select_clause.columns):
             if column_expression.alias is not None:
                 select_column = StandardColumn(column_name=column_expression.alias.name, column_idx=column_idx)
-            elif isinstance(column_expression.value, core.ASTColumnName):
+            elif isinstance(column_expression.value, core.ASTColumnNameExpression):
                 select_column = StandardColumn(column_name=column_expression.value.column_name,
                                                column_idx=column_idx)
             else:
                 select_column = StandardColumn(column_name=column_expression.value.source(),
                                                column_idx=column_idx)
             result[select_column] = CurrentNodeUsedQuoteColumn.handle(column_expression.value)
         return result
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_sub_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     def get_sub_query_statement(self, alias_name: str) -> core.ASTSelectStatement:
         """获取指定别名的子查询的 SELECT 语句"""
         return self._alias_hash[alias_name]
 
     @classmethod
     def handle(cls, node: object) -> Dict[str, core.ASTSelectStatement]:
         """TODO 待支持不包含别名的子查询"""
-        if (isinstance(node, core.ASTFromTableExpression)
+        if (isinstance(node, core.ASTFromTable)
                 and node.alias is not None and isinstance(node.name, core.ASTSubQueryExpression)):
             return {node.alias.name: node.name.statement}
         if isinstance(node, (core.ASTSubQueryExpression, core.ASTWithClause)):
             return {}
         return cls.default_handle_node(node)
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_table_name_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     def get_all_standard_table(self) -> List[StandardTable]:
         """获取所有的标准表对象"""
         return list(self._alias_name_to_standard_table_hash.values())
 
     @classmethod
     def handle(cls, node: object) -> Dict[str, StandardTable]:
         """TODO 待支持无别名子查询"""
-        if isinstance(node, core.ASTFromTableExpression):
-            if isinstance(node.name, core.ASTTableName):
+        if isinstance(node, core.ASTFromTable):
+            if isinstance(node.name, core.ASTTableNameExpression):
                 alias_name = node.alias.name if node.alias is not None else node.name.table_name
                 standard_table = StandardTable(schema_name=node.name.schema_name, table_name=node.name.table_name)
                 return {alias_name: standard_table}
             if isinstance(node.name, core.ASTSubQueryExpression):
                 alias_name = node.alias.name  #
                 standard_table = StandardTable(schema_name=None, table_name=alias_name)  # 待增加中间表标记
                 return {alias_name: standard_table}
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py` & `metasequoia-sql-0.6.0/metasequoia_sql/analyzer/toolkit/current_level_used_quote_columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 
     @classmethod
     def handle(cls, node: Union[core.ASTBase, tuple]) -> List[QuoteColumn]:
         # pylint: disable=R0911
         # pylint: disable=R0912
         """自定义的处理规则"""
         # 处理类似 COUNT(1) 的场景：如果是聚集函数，但参数中没有引用字段，则返回一个 column_name 为空的引用
-        if isinstance(node, core.ASTAggregationFunctionExpression):
+        if isinstance(node, core.ASTAggregationFunction):
             quote_column_list = cls.default_handle_node(node)
             if len(quote_column_list) > 0:
                 return quote_column_list
             return [QuoteColumn(column_name=None)]
 
         # 处理通配符场景
         if isinstance(node, core.ASTWildcardExpression):
             return [QuoteColumn(table_name=node.table_name, column_name="*")]
 
         # 处理普通表名引用场景
-        if isinstance(node, core.ASTColumnName) and node.source() not in name_set.GLOBAL_VARIABLE_NAME_SET:
+        if isinstance(node, core.ASTColumnNameExpression) and node.source() not in name_set.GLOBAL_VARIABLE_NAME_SET:
             return [QuoteColumn(table_name=node.table_name, column_name=node.column_name)]
 
         # 如果是 GROUP BY 子句，则需要兼容使用字段序号的情况
         if isinstance(node, core.ASTGroupByClause):
             quote_column_list = []
             for column in node.columns:
                 if is_int_literal(column.source()):
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/common/basic.py` & `metasequoia-sql-0.6.0/metasequoia_sql/common/basic.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/common/char_set.py` & `metasequoia-sql-0.6.0/metasequoia_sql/common/char_set.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/common/name_set.py` & `metasequoia-sql-0.6.0/metasequoia_sql/common/name_set.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/common/static.py` & `metasequoia-sql-0.6.0/metasequoia_sql/common/static.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/core/node.py` & `metasequoia-sql-0.6.0/metasequoia_sql/core/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,160 +1,145 @@
 # pylint: disable=C0302
 
 """
 抽象语法树（AST）节点
 
+节点命名规范：
+1. 非语句层级的抽象类统一使用 Base 后缀，语句层级的抽象类可以不使用 Base 后缀
+2. 抽象语法树节点包含语句（Statement）、子句（Clause）、表达式（Expression）、元素共 4 个层级：
+  - 语句层级：是可以执行运行的 SQL 语句，节点统一使用 Statement 后缀
+  - 子句层级：是包括 FROM、WHERE 等在内的子句，是语句的组成部分，节点统一使用 Clause 后缀
+  - 表达式层级：是子句的组成部分，相对于元素来说，表达式更加通用一些，会在不同场景中使用，节点统一使用 Expression 后缀
+  - 元素层级：是表达式或在子句的组成部分，相对于表达式来说，元素层级往往仅在少数特定场景下使用，仅用于封装多个元素或用于封装枚举类，节点没有后缀
+
 在设计上，要求每个节点都是不可变节点，从而保证节点是可哈希的。同时，我们提供专门的修改方法：
 - 当前，我们使用复制并返回新元素的方法，且不提供 inplace 参数
 - 未来，我们为每个元素提供 .changeable() 方法，返回该元素的可变节点形式
 
-一般表达式节点：
-1. 包含使用 AND、OR 关键字连接的一个或多个布尔值表达式
-条件表达式节点：
-1. 可以视作一种特殊的一般表达式
-2. 包含使用比较运算符、IS、LIKE、RLIKE、BETWEEN 等连接的一个或多个多项式表达式
-多项表达式节点：
-1. 可以视作一种特殊的条件表达式
-2. 包含使用计算运算符连接的一个或多个单项式表达式
-单项表达式节点：
-1. 可以视作一种特殊多项表达式
-2. 仅包含一个元素的表达式
-3. 插入语虽然下一层为一般表达式，但是在上一层视作单项表达式
-
-TODO 将 Union 类型的转化为专门的 Type
-TODO 给通用表达式增加不同返回值类型的子类
-TODO 将 ASTExpressionBase 替换为更精确的子类
-TODO 优化各节点之间的继承关系
-TODO 优化需要一元表达式的类型
+其中：
+- 诸如函数调用、CASE、窗口等最终返回一个普通值或布尔值，且在当前层级下可以视作一个任意值节点的元素，均称为元素表达式
+- 诸如比较运算符、BETWEEN、LIKE 等最终返回一个布尔值，且在当前层级下可以视作一个布尔值节点的元素，均称为布尔表达式
+- 第 5 层级到第 8 层级的表达式，可以统称为布尔表达式
 """
 
 import abc
 import dataclasses
-import enum
-from typing import Optional, Tuple, Union, Dict
+from typing import Optional, Tuple, Union, Dict, Any
 
-from metasequoia_sql.common.basic import is_int_literal
+from metasequoia_sql.common.basic import is_int_literal, is_bool_literal, is_float_literal, is_null_literal
+from metasequoia_sql.core import static
 from metasequoia_sql.core.sql_type import SQLType
-from metasequoia_sql.errors import SqlParseError
-from metasequoia_sql.errors import UnSupportSqlTypeError
+from metasequoia_sql.errors import SqlParseError, UnSupportSqlTypeError
 
 __all__ = [
     # ------------------------------ 抽象语法树（AST）节点的抽象类 ------------------------------
     "ASTBase",  # 所有语法树节点的抽象基类
     "ASTStatementBase",  # 语句的抽象基类
-    "ASTExpressionBase",  # 表达式的抽象基类
-    "ASTMonomialExpression",  # 表达式的子类（第 1 层）：单项式节点的抽象基类
-    "AliasPolynomialExpression",  # 表达式类型（第 2 层）：多项式节点
-    "AliasConditionExpression",  # 表达式类型（第 3 层）：条件表达式
-    "AliasGeneralExpression",  # 表达式类型（第 4 层）：一般表达式
-
-    # ------------------------------ 抽象语法树（AST）节点的类型 ------------------------------
-    "AliasPolynomialExpressionElement",  # 多项式节点的元素类型
-    "AliasConditionExpressionElement",  # 条件表达式的元素类型
-    "AliasGeneralExpressionElement",  # 一般表达式的元素类型
-    "AliasTableExpression",  # 表表达式（表名表达式 + 子查询表达式）
-    "AliasCreateTableStatement",  # 建表语句表达式（普通建表语句 + CREATE TABLE ... AS ... 语句）
-    "AliasPartitionParam",  # 分区参数：包含动态分区和非动态分区两种情况
-
-    # ------------------------------ 抽象语法树（AST）节点的枚举类节点 ------------------------------
-    "EnumInsertType", "ASTInsertType",  # 插入类型
-    "EnumJoinType", "ASTJoinType",  # 关联类型
-    "EnumOrderType", "ASTOrderType",  # 排序类型
-    "EnumUnionType", "ASTUnionType",  # 组合类型
-    "EnumCastDataType", "ASTCastDataType",  # CAST 函数中的字段类型枚举类
-    "EnumCompareOperator", "ASTCompareOperator",  # 比较运算符
-    "EnumComputeOperator", "ASTComputeOperator",  # 计算运算符
-    "EnumLogicalOperator", "ASTLogicalOperator",  # 逻辑运算符
-
-    # ------------------------------ 抽象语法树（AST）节点的基础类节点 ------------------------------
-    "ASTTableName",  # 表名表达式
-    "ASTFunctionName",  # 函数名表达式
-    "EnumWindowRowType",  # 窗口函数中的行限制的类型
+    "ASTStatementHasWithClauseBase",  # 包含 WITH 子句的语句的抽象基类
+    "ASTExpressionBase",  # 一般表达式的抽象基类
+
+    # ------------------------------ 抽象语法树（AST）节点的枚举类元素节点 ------------------------------
+    "ASTEnumListBase",  # 抽象语法树枚举类型的基类（枚举值为字符串列表）
+    "ASTEnumElementBase",  # 抽象语法树枚举类型的基类（枚举值为字符串）
+    "ASTInsertType",  # 插入类型
+    "ASTJoinType",  # 关联类型
+    "ASTOrderType",  # 排序类型
+    "ASTUnionType",  # 组合类型
+    "ASTCastDataType",  # CAST 函数中的字段类型枚举类
+    "ASTCompareOperator",  # 比较运算符
+    "ASTComputeOperator",  # 计算运算符
+    "ASTLogicalOperator",  # 逻辑运算符
+
+    # ------------------------------ 抽象语法树（AST）节点的基础表达式节点 ------------------------------
+    "ASTTableNameExpression",  # 表名节点
+    "ASTFunctionNameExpression",  # 函数名节点
+    "ASTAlisaExpression",  # 别名节点
+    "ASTMultiAlisaExpression",  # 多个别名节点（用于在 LATERAL VIEW 子句中配合返回多个字段使用）
+
+    # ------------------------------ 抽象语法树（AST）节点的一般表达式节点 ------------------------------
+    # 运算表达式中的单元素表达式
+    "ASTBinaryExpressionBase",  # 二元表达式的抽象基类
+    "ASTColumnNameExpression",  # 【元素表达式层级】列名表达式节点
+    "ASTLiteralExpression",  # 【元素表达式层级】字面值表达式节点
+    "ASTWildcardExpression",  # 【元素表达式层级】通配符表达式节点
+    "ASTFunctionExpressionBase",  # 【元素表达式层级】函数表达式：函数表达式的抽象类
+    "ASTNormalFunctionExpression",  # 【元素表达式层级】函数表达式：普通函数表达式
+    "ASTAggregationFunction",  # 【元素表达式层级】函数表达式：聚集函数表达式
+    "ASTCastFunctionExpression",  # 【元素表达式层级】函数表达式：CAST 函数表达式
+    "ASTExtractFunctionExpression",  # 【元素表达式层级】函数表达式：EXTRACT 函数表达式
     "ASTWindowRowItem",  # 窗口函数中的行限制
     "ASTWindowRow",  # 窗口函数的行数限制表达式
-    "ASTAlisaExpression",  # 别名表达式
-    "ASTMultiAlisaExpression",  # 多个别名表达式
-
-    # ------------------------------ 抽象语法树（AST）节点的通用表达式类节点 ------------------------------
-    # 单项表达式层级
-    "ASTColumnName",  # 列名表达式
-    "ASTLiteralExpression",  # 字面值表达式
-    "ASTWildcardExpression",  # 通配符表达式
-    "ASTFunctionExpression",  # 函数表达式：函数表达式的抽象类
-    "ASTNormalFunctionExpression",  # 函数表达式：普通函数表达式
-    "ASTAggregationFunctionExpression",  # 函数表达式：聚集函数表达式
-    "ASTCastFunctionExpression",  # 函数表达式：CAST 函数表达式
-    "ASTExtractFunctionExpression",  # 函数表达式：EXTRACT 函数表达式
-    "ASTArrayIndexExpression",  # 数组下标表达式
-    "ASTWindowExpression",  # 窗口表达式
-    "ASTCaseConditionExpression",  # CASE 表达式：CASE 之后没有变量，WHEN 中为条件语句的 CASE 表达式
+    "ASTWindowExpression",  # 【元素表达式层级】窗口表达式
+    "ASTCaseConditionExpression",  # 【元素表达式层级】CASE 表达式：CASE 之后没有变量，WHEN 中为条件语句的 CASE 表达式
     "ASTCaseConditionItem",  # CASE 表达式元素：WHEN ... CASE ... 表达式
-    "ASTCaseValueExpression",  # CASE 表达式：CASE 之后有变量，WHEN 中为该变量的枚举值的 CASE 表达式
+    "ASTCaseValueExpression",  # 【元素表达式层级】CASE 表达式：CASE 之后有变量，WHEN 中为该变量的枚举值的 CASE 表达式
     "ASTCaseValueItem",  # CASE 表达式元素：WHEN ... CASE ... 表达式
-    "ASTParenthesisExpression",  # 插入语表达式
-    "ASTSubQueryExpression",  # 插入语表达式：子查询表达式
-    "ASTSubGeneralExpression",  # 插入语表达式：插入语一般表达式（下层为一般表达式）
-    "ASTSubValueExpression",  # 插入语表达式：值表达式
-
-    # 多项表达式层级
-    "ASTPolynomialExpression",  # 计算表达式
-
-    # 条件表达式层级
-    "ASTConditionExpression",  # 布尔值表达式
-    "ASTBoolCompareExpression",  # 布尔值表达式：使用比较运算符的布尔值表达式
-    "ASTBoolOperatorExpression",  # 布尔值表达式：通过运算符或关键字比较运算符前后两个表达式的抽象类
-    "ASTBoolIsExpression",  # 布尔值表达式：使用 IS 的布尔值表达式
-    "ASTBoolInExpression",  # 布尔值表达式：使用 IN 的布尔值表达式
-    "ASTBoolLikeExpression",  # 布尔值表达式：使用 LIKE 的布尔值表达式
-    "ASTBoolExistsExpression",  # 布尔值表达式：使用 EXISTS 的布尔值表达式
-    "ASTBoolBetweenExpression",  # 布尔值表达式：使用 BETWEEN 的布尔值表达式
-    "ASTBoolRlikeExpression",  # 布尔值表达式：使用 RLIKE 的布尔值表达式
-    "ASTBoolRegexpExpression",  # 布尔值表达式：使用 REGEXP 的布尔值表达式
+    "ASTSubQueryExpression",  # 【元素表达式层级】插入语表达式：子查询表达式
+    "ASTSubValueExpression",  # 【元素表达式层级】插入语表达式：值表达式
+    "ASTIndexExpression",  # 【下标表达式层级】下标表达式
+    "ASTUnaryExpression",  # 【一元表达式层级】一元表达式
+
+    # 运算表达式中的组合表达式
+    "ASTComputeExpression",  # 使用计算运算符的二元表达式：包含异或表达式、单项表达式、多项表达式、移位表达式、按位与表达式和按位或表达式
+
+    # 条件表达式中的元素表达式
+    "ASTOperatorExpressionBase",  # 【关键字条件表达式层级】通过运算符或关键字比较运算符前后两个表达式的抽象类
+    "ASTIsExpression",  # 【关键字条件表达式层级】使用 IS 的布尔值表达式
+    "ASTInExpression",  # 【关键字条件表达式层级】使用 IN 的布尔值表达式
+    "ASTLikeExpression",  # 【关键字条件表达式层级】使用 LIKE 的布尔值表达式
+    "ASTExistsExpression",  # 【关键字条件表达式层级】使用 EXISTS 的布尔值表达式
+    "ASTBetweenExpression",  # 【关键字条件表达式层级】使用 BETWEEN 的布尔值表达式
+    "ASTRlikeExpression",  # 【关键字条件表达式层级】使用 RLIKE 的布尔值表达式
+    "ASTRegexpExpression",  # 【关键字条件表达式层级】使用 REGEXP 的布尔值表达式
+
+    # 条件表达式中的组合表达式
+    "ASTOperatorConditionExpression",  # 【运算符条件表达式层级】运算符条件表达式
+    "ASTLogicalNotExpression",  # 【逻辑否表达式层级】逻辑否表达式
+    "ASTLogicalAndExpression",  # 【逻辑与表达式层级】逻辑与表达式
+    "ASTLogicalXorExpression",  # 【逻辑异或表达式层级】逻辑异或表达式节点
+    "ASTLogicalOrExpression",  # 【逻辑或表达式层级】逻辑或表达式节点
 
-    # 条件表达式层级
-    "ASTGeneralExpression",  # 条件表达式
-
-    # ------------------------------ 抽象语法树（AST）节点的 SELECT 语句节点 ------------------------------
-    "ASTSelectColumnExpression",  # SELECT 子句元素：包含别名的列表达式
-    "ASTFromTableExpression",  # FROM 和 JOIN 子句元素：包含别名的表表达式
-    "ASTOrderByColumnExpression",  # ORDER BY 子句元素：包含排序字段及排序顺序的表达式
-    "ASTJoinExpression",  # JOIN 子句元素：关联表达式的抽象类
-    "ASTJoinOnExpression",  # JOIN 子句元素：使用 ON 关键字的关联表达式
-    "ASTJoinUsingExpression",  # JOIN 子句元素：使用 USING 函数的关联表达式
-    "ASTGroupingSets",  # GROUP BY 子句元素：GROUPING SETS 表达式
+    # ------------------------------ 抽象语法树（AST）节点的子句节点 ------------------------------
+    "ASTSelectColumn",  # SELECT 子句元素：包含别名的列表达式
     "ASTSelectClause",  # SELECT 子句
+    "ASTFromTable",  # FROM 和 JOIN 子句元素：包含别名的表表达式
     "ASTFromClause",  # FROM 子句
     "ASTLateralViewClause",  # LATERAL VIEW 子句
+    "ASTJoinOnExpression",  # JOIN 子句元素：使用 ON 关键字的关联表达式
+    "ASTJoinUsingExpression",  # JOIN 子句元素：使用 USING 函数的关联表达式
     "ASTJoinClause",  # JOIN 子句
     "ASTWhereClause",  # WHERE 子句
+    "ASTGroupingSets",  # GROUP BY 子句元素：GROUPING SETS 表达式
     "ASTGroupByClause",  # GROUP BY 子句
     "ASTHavingClause",  # HAVING 子句
+    "ASTOrderByColumn",  # ORDER BY 子句元素：包含排序字段及排序顺序的表达式
     "ASTOrderByClause",  # ORDER BY 子句
     "ASTSortByClause",  # SORT BY 子句【Hive】
     "ASTDistributeByClause",  # DISTRIBUTE BY 子句【Hive】
     "ASTClusterByClause",  # CLUSTER BY 子句【Hive】
     "ASTLimitClause",  # LIMIT 子句
     "ASTWithClause",  # WITH 子句
     "ASTWithTable",  # WITH 子句元素：WITH 语句中的每个表
+
+    # ------------------------------ 抽象语法树（AST）节点的 SELECT 语句节点 ------------------------------
     "ASTSelectStatement",  # SELECT 语句的抽象类
     "ASTSingleSelectStatement",  # SELECT 语句：没有 UNION 多个 SELECT 语句的 SELECT 语句
     "ASTUnionSelectStatement",  # SELECT 语句：UNION 了多个 SELECT 语句的组合后的 SELECT 语句
 
     # ------------------------------ 抽象语法树（AST）节点的 INSERT 语句节点 ------------------------------
     "ASTPartitionExpression",  # 分区表达式
     "ASTInsertStatement",  # INSERT 语句
     "ASTInsertValuesStatement",  # INSERT ... VALUES ... 语句
     "ASTInsertSelectStatement",  # INSERT ... SELECT ... 语句
 
     # ------------------------------ 抽象语法树（AST）节点的 CREATE TABLE 语句节点 ------------------------------
-    "AliasColumnOrIndex",  # DDL 的字段或索引类型
     "ASTConfigStringExpression",  # 配置值为字符串的配置表达式
     "ASTColumnTypeExpression",  # 字段类型表达式
     "ASTDefineColumnExpression",  # 字段定义表达式
-    "ASTIndexColumn",  # 索引声明表达式中的字段
+    "ASTIndexColumn",  # 索引声明表达式元素：索引声明表达式中的字段
     "ASTIndexExpressionBase",  # 索引声明表达式（抽象类）
     "ASTPrimaryIndexExpression",  # 主键索引声明表达式
     "ASTUniqueIndexExpression",  # 唯一键索引声明表达式
     "ASTNormalIndexExpression",  # 普通索引声明表达式
     "ASTFulltextIndexExpression",  # 全文本索引声明表达式
     "ASTForeignKeyExpression",  # 声明外键表达式
     "ASTCreateTableStatement",  # CREATE TABLE 语句
@@ -175,22 +160,35 @@
     "ASTAlterModifyExpression",  # ALTER TABLE 语句的 MODIFY 子句
     "ASTAlterChangeExpression",  # ALTER TABLE 语句的 CHANGE 子句
     "ASTAlterDropColumnExpression",  # ALTER TABLE 语句的 DROP COLUMN 子句
     "ASTAlterDropPartitionExpression",  # ALTER TABLE 语句的 DROP PARTITION 子句
     "ASTAlterRenameColumnExpression",  # ALTER TABLE 语句的 RENAME ... TO ... 子句
     "ASTAlterTableStatement",  # ALTER TABLE 语句
 
-    # ------------------------------ 抽象语法树（AST）节点的 MCSK REPAIR TABLE 语句节点 ------------------------------
+    # ------------------------------ 抽象语法树（AST）节点的 MSCK REPAIR TABLE 语句节点 ------------------------------
     "ASTMsckRepairTableStatement",  # MSCK REPAIR TABLE 语句
 
     # ------------------------------ 抽象语法树（AST）节点的 USE 语句节点 ------------------------------
     "ASTUseStatement",  # USE 语句
 
     # ------------------------------ 抽象语法树（AST）节点的 TRUNCATE TABLE 语句节点 ------------------------------
     "ASTTruncateTable",  # TRUNCATE TABLE 语句
+
+    # ------------------------------ 抽象语法树（AST）节点的 UPDATE 语句节点 ------------------------------
+    "ASTUpdateSetColumn",  # SET 子句元素：SET 的列
+    "ASTUpdateSetClause",  # UPDATE 语句中的 SET 子句
+    "ASTUpdateStatement",  # UPDATE 语句
+
+    # ------------------------------ 抽象语法树（AST）节点的 DELETE 语句节点 ------------------------------
+    "ASTDeleteStatement",  # DELETE 语句
+
+    # ------------------------------ 抽象语法树（AST）节点的 SHOW 语句节点 ------------------------------
+    "ASTShowDatabasesStatement",  # SHOW DATABASES 语句
+    "ASTShowTablesStatement",  # SHOW TABLES 语句
+    "ASTShowColumnsStatement"  # SHOW COLUMNS 语句
 ]
 
 
 # ---------------------------------------- 抽象基类 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
@@ -215,669 +213,380 @@
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTStatementBase(ASTBase, abc.ABC):
     """抽象语法树（AST）语句节点的抽象基类"""
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTExpressionBase(ASTBase, abc.ABC):
-    """抽象语法树（AST）表达式节点的抽象基类"""
-
+    """抽象语法树（AST）一般表达式节点的抽象基类"""
 
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTMonomialExpression(ASTExpressionBase, abc.ABC):
-    """抽象语法树（AST）单项表达式节点的抽象基类"""
+    @classmethod
+    def node_name(cls):
+        """节点名称：因为括号可以调整计算优先级，所以一般表达式节点的元素没有明确类型，需要允许获取节点类型的类方法"""
+        return cls.__name__
 
-    unary_operator: Optional[Tuple["ASTComputeOperator", ...]] = dataclasses.field(kw_only=True, default=None)  # 一元运算符
 
-    def _get_unary_operator_str(self, sql_type: SQLType = SQLType.DEFAULT):
-        if self.unary_operator is None:
-            return ""
-        return "".join(operator.source(sql_type) for operator in self.unary_operator)
-
-
-AliasPolynomialExpression = Union["ASTPolynomialExpression", ASTMonomialExpression]  # 多项式节点类型
-AliasConditionExpression = Union["ASTConditionExpression", AliasPolynomialExpression]  # 条件表达式节点类型
-AliasGeneralExpression = Union["ASTGeneralExpression", AliasConditionExpression]  # 一般表达式节点类型
-
-
-# ---------------------------------------- 插入类型 ----------------------------------------
-
-
-class EnumInsertType(enum.Enum):
-    """插入类型的枚举类"""
-    INSERT_INTO = ["INSERT", "INTO"]
-    INSERT_IGNORE_INTO = ["INSERT", "IGNORE", "INTO"]
-    INSERT_OVERWRITE = ["INSERT", "OVERWRITE"]
+# ---------------------------------------- 枚举类的抽象语法树节点 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTInsertType(ASTBase):
-    """插入类型"""
+class ASTEnumListBase(ASTBase):
+    """抽象语法树枚举类型的基类（枚举类值为列表）"""
 
-    enum: EnumInsertType = dataclasses.field(kw_only=True)  # 插入类型的枚举类
+    enum: Any = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return " ".join(self.enum.value)
 
 
-# ---------------------------------------- 关联类型 ----------------------------------------
-
-
-class EnumJoinType(enum.Enum):
-    """关联类型的枚举类"""
-    JOIN = ["JOIN"]  # 内连接
-    INNER_JOIN = ["INNER", "JOIN"]  # 内连接
-    LEFT_JOIN = ["LEFT", "JOIN"]  # 左外连接
-    LEFT_OUTER_JOIN = ["LEFT", "OUTER", "JOIN"]  # 左外连接
-    LEFT_SEMI_JOIN = ["LEFT", "SEMI", "JOIN"]  # 左半连接
-    RIGHT_JOIN = ["RIGHT", "JOIN"]  # 右外连接
-    RIGHT_OUTER_JOIN = ["RIGHT", "OUTER", "JOIN"]  # 右外连接
-    RIGHT_SEMI_JOIN = ["RIGHT", "SEMI", "JOIN"]  # 右半连接
-    FULL_JOIN = ["FULL", "JOIN"]  # 全外连接
-    FULL_OUTER_JOIN = ["FULL", "OUTER", "JOIN"]  # 全外连接
-    CROSS_JOIN = ["CROSS", "JOIN"]  # 交叉连接
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTJoinType(ASTBase):
-    """关联类型"""
+class ASTEnumElementBase(ASTBase):
+    """抽象语法树枚举类型的基类（枚举类值为元素）"""
 
-    enum: EnumJoinType = dataclasses.field(kw_only=True)  # 关联类型的枚举类
+    enum: Any = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return " ".join(self.enum.value)
-
+        return self.enum.value
 
-# ---------------------------------------- 排序类型 ----------------------------------------
 
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTInsertType(ASTEnumListBase):
+    """插入类型"""
 
-class EnumOrderType(enum.Enum):
-    """排序类型的枚举类"""
-    ASC = ["ASC"]  # 升序
-    DESC = ["DESC"]  # 降序
+    enum: static.EnumInsertType = dataclasses.field(kw_only=True)  # 插入类型的枚举类
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTOrderType(ASTBase):
-    """排序类型"""
-
-    enum: EnumOrderType = dataclasses.field(kw_only=True)  # 排序类型的枚举类
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        return " ".join(self.enum.value)
+class ASTJoinType(ASTEnumListBase):
+    """关联类型"""
 
+    enum: static.EnumJoinType = dataclasses.field(kw_only=True)  # 关联类型的枚举类
 
-# ---------------------------------------- 组合类型 ----------------------------------------
 
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTOrderType(ASTEnumListBase):
+    """排序类型"""
 
-class EnumUnionType(enum.Enum):
-    """组合类型的枚举类"""
-    UNION_ALL = ["UNION", "ALL"]
-    UNION = ["UNION"]
-    EXCEPT = ["EXCEPT"]
-    INTERSECT = ["INTERSECT"]
-    MINUS = ["MINUS"]
+    enum: static.EnumOrderType = dataclasses.field(kw_only=True)  # 排序类型的枚举类
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTUnionType(ASTBase):
+class ASTUnionType(ASTEnumListBase):
     """组合类型"""
 
-    enum: EnumUnionType = dataclasses.field(kw_only=True)  # 组合类型的枚举类
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        return " ".join(self.enum.value)
-
-
-# ---------------------------------------- 比较运算符 ----------------------------------------
-
-class EnumCompareOperator(enum.Enum):
-    """比较运算符的枚举类"""
-    EQ = ["="]
-    EQUAL_TO = ["="]
-    NEQ = ["!="]
-    NOT_EQUAL_TO = ["!="]
-    LT = ["<"]
-    LESS_THAN = ["<"]
-    LTE = ["<="]
-    LESS_THAN_OR_EQUAL = ["<="]
-    GT = [">"]
-    GREATER_THAN = [">"]
-    GTE = [">="]
-    GREATER_THAN_OR_EQUAL = [">="]
+    enum: static.EnumUnionType = dataclasses.field(kw_only=True)  # 组合类型的枚举类
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTCompareOperator(ASTBase):
+class ASTCompareOperator(ASTEnumListBase):
     """比较运算符"""
 
-    enum: EnumCompareOperator = dataclasses.field(kw_only=True)  # 比较运算符的枚举类
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        return " ".join(self.enum.value)
-
-
-# ---------------------------------------- 计算运算符 ----------------------------------------
-
-class EnumComputeOperator(enum.Enum):
-    """计算运算符的枚举类"""
-    PLUS = ["+"]  # 加法运算符
-    SUBTRACT = ["-"]  # 减法运算符
-    MULTIPLE = ["*"]  # 乘法运算符
-    DIVIDE = ["/"]  # 除法运算符
-    MOD = ["%"]  # 取模运算符
-    CONCAT = ["||"]  # 字符串拼接运算符（仅 Oracle、DB2、PostgreSQL 中适用）
-    AMPERSAND = ["&"]  # 按位与（仅 Hive 中适用）
+    enum: static.EnumCompareOperator = dataclasses.field(kw_only=True)  # 比较运算符的枚举类
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTComputeOperator(ASTBase):
+class ASTComputeOperator(ASTEnumElementBase):
     """计算运算符"""
 
-    enum: EnumComputeOperator = dataclasses.field(kw_only=True)  # 计算运算符的枚举类
+    enum: static.EnumComputeOperator = dataclasses.field(kw_only=True)  # 计算运算符的枚举类
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        # pylint: disable=R1725
         """返回语法节点的 SQL 源码"""
-        if self.enum == EnumComputeOperator.MOD and sql_type not in {SQLType.SQL_SERVER, SQLType.HIVE}:
+        if (self.enum == static.EnumComputeOperator.MOD
+                and sql_type not in {SQLType.DEFAULT, SQLType.MYSQL, SQLType.SQL_SERVER, SQLType.HIVE}):
             raise UnSupportSqlTypeError(f"{sql_type} 不支持使用 % 运算符")
-        if (self.enum == EnumComputeOperator.CONCAT
-                and sql_type not in {SQLType.ORACLE, SQLType.DB2, SQLType.POSTGRE_SQL}):
-            raise UnSupportSqlTypeError(f"{sql_type} 不支持使用 || 运算符")
-        return " ".join(self.enum.value)
-
-
-# ---------------------------------------- 逻辑运算符 ----------------------------------------
-
-
-class EnumLogicalOperator(enum.Enum):
-    """逻辑运算符的枚举类"""
-    AND = ["AND"]
-    OR = ["OR"]
-    NOT = ["NOT"]
+        return super(ASTComputeOperator, self).source(sql_type)
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTLogicalOperator(ASTBase):
+class ASTLogicalOperator(ASTEnumListBase):
     """逻辑运算符"""
 
-    enum: EnumLogicalOperator = dataclasses.field(kw_only=True)  # 逻辑运算符的枚举类
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        return " ".join(self.enum.value)
+    enum: static.EnumLogicalOperator = dataclasses.field(kw_only=True)  # 逻辑运算符的枚举类
 
 
 # ---------------------------------------- CASE 函数中的字段类型表达式 ----------------------------------------
 
 
-class EnumCastDataType(enum.Enum):
-    """CAST 函数的字段类型"""
-    # MySQL 类型
-    CHAR = "CHAR"
-    ENUM = "ENUM"
-    LONGTEXT = "LONGTEXT"
-    MEDIUMTEXT = "MEDIUMTEXT"
-    SET = "SET"
-    TEXT = "TEXT"
-    TINYTEXT = "TINYTEXT"
-    VARCHAR = "VARCHAR"
-    BIT = "BIT"
-    BIGINT = "BIGINT"
-    BOOLEAN = "BOOLEAN"
-    BOOL = "BOOL"
-    DECIMAL = "DECIMAL"
-    DEC = "DEC"
-    DOUBLE = "DOUBLE"
-    INT = "INT"
-    INTEGER = "INTEGER"
-    MEDIUMINT = "MEDIUMINT"
-    REAL = "REAL"
-    SMALLINT = "SMALLINT"
-    TINYINT = "TINYINT"
-    DATE = "DATE"
-    DATETIME = "DATETIME"
-    TIMESTAMP = "TIMESTAMP"
-    TIME = "TIME"
-    YEAR = "YEAR"
-    BOLB = "BOLB"
-    MEDIUMBLOB = "MEDIUMBLOB"
-    LONGBLOB = "LONGBLOB"
-    TINYBLOB = "TINYBLOB"
-
-    # Hive 类型
-    STRING = "STRING"
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTCastDataType(ASTBase):
     """CAST 语句中的数据类型"""
 
     signed: bool = dataclasses.field(kw_only=True)  # 是否包含 SIGNED 关键字
-    type: EnumCastDataType = dataclasses.field(kw_only=True)  # 目标转换的数据类型
+    type: static.EnumCastDataType = dataclasses.field(kw_only=True)  # 目标转换的数据类型
     params: Optional[Tuple[int, ...]] = dataclasses.field(kw_only=True)  # 目标转换的数据类型的参数列表
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         result = []
         if self.signed is True:
             result.append("SIGNED")
         result.append(self.type.value)
         if self.params is not None:
             param_str = ", ".join(str(param) for param in self.params)
             result.append(f"({param_str})")
         return " ".join(result)
 
 
-# ---------------------------------------- 各层级表达式元素类型 ----------------------------------------
-
-
-AliasPolynomialExpressionElement = Union[ASTMonomialExpression, ASTComputeOperator]
-AliasConditionExpressionElement = Union[AliasPolynomialExpression, ASTCompareOperator]
-AliasGeneralExpressionElement = Union[AliasConditionExpression, ASTLogicalOperator]
-
-
-# ---------------------------------------- 列名表达式 ----------------------------------------
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTColumnName(ASTMonomialExpression):
-    """列名表达式"""
-
-    table_name: Optional[str] = dataclasses.field(kw_only=True, default=None)  # 表名称
-    column_name: str = dataclasses.field(kw_only=True)  # 字段名称
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        if self.column_name not in {"*", "CURRENT_DATE", "CURRENT_TIME", "CURRENT_TIMESTAMP"}:
-            result = (f"`{self.table_name}`.`{self.column_name}`" if self.table_name is not None
-                      else f"`{self.column_name}`")
-        else:
-            result = f"`{self.table_name}`.{self.column_name}" if self.table_name is not None else f"{self.column_name}"
-        if sql_type == SQLType.DB2:
-            # 兼容 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
-            result = result.replace("CURRENT_DATE", "CURRENT DATE")
-            result = result.replace("CURRENT_TIME", "CURRENT TIME")
-            result = result.replace("CURRENT_TIMESTAMP", "CURRENT TIMESTAMP")
-        return result
-
-
 # ---------------------------------------- 表名表达式 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTTableName(ASTBase):
+class ASTTableNameExpression(ASTBase):
     """表名表达式"""
 
     schema_name: Optional[str] = dataclasses.field(kw_only=True, default=None)
     table_name: str = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"`{self.schema_name}.{self.table_name}`" if self.schema_name is not None else f"`{self.table_name}`"
 
 
 # ---------------------------------------- 函数名表达式 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTFunctionName(ASTBase):
+class ASTFunctionNameExpression(ASTBase):
     """函数名表达式"""
 
     schema_name: Optional[str] = dataclasses.field(kw_only=True, default=None)
     function_name: str = dataclasses.field(kw_only=True)
 
     @staticmethod
-    def by_name(function_name: str) -> "ASTFunctionName":
+    def by_name(function_name: str) -> "ASTFunctionNameExpression":
         """使用函数名构造"""
-        return ASTFunctionName(function_name=function_name)
+        return ASTFunctionNameExpression(function_name=function_name)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"`{self.schema_name}`.{self.function_name}" if self.schema_name is not None else f"{self.function_name}"
 
 
-# ---------------------------------------- 字面值表达式 ----------------------------------------
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTLiteralExpression(ASTMonomialExpression):
-    """字面值表达式"""
-
-    value: str = dataclasses.field(kw_only=True)  # 字面值
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        return self.value
-
-    def as_int(self) -> int:
-        """将字面值作为整形返回"""
-        if is_int_literal(self.value):
-            return int(self.value)
-        raise SqlParseError(f"无法字面值 {self.value} 转化为整型")
-
-    def as_string(self) -> str:
-        """将字面值作为字符串返回"""
-        return self.value
-
-
-# ---------------------------------------- 窗口函数的行数限制 ----------------------------------------
-
-
-class EnumWindowRowType(enum.Enum):
-    """窗口函数中的行限制的类型"""
-    PRECEDING = "PRECEDING"
-    CURRENT_ROW = "CURRENT ROW"
-    FOLLOWING = "FOLLOWING"
+# ---------------------------------------- 别名表达式 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTWindowRowItem(ASTBase):
-    """窗口函数中的行限制
-
-    unbounded preceding = 当前行的所有行
-    n preceding = 当前行之前的 n 行
-    current row = 当前行
-    n following = 当前行之后的 n行
-    unbounded following = 当前行之后的所有行
-    """
+class ASTAlisaExpression(ASTBase):
+    """别名表达式，例如：AS name"""
 
-    row_type: EnumWindowRowType = dataclasses.field(kw_only=True)
-    is_unbounded: bool = dataclasses.field(kw_only=True, default=False)
-    row_num: Optional[int] = dataclasses.field(kw_only=True, default=None)
+    name: str = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        if self.row_type == EnumWindowRowType.CURRENT_ROW:
-            return "CURRENT ROW"
-        row_type_str = self.row_type.value
-        if self.is_unbounded is True:
-            return f"UNBOUNDED {row_type_str}"
-        return f"{self.row_num} {row_type_str}"
+        return f"AS {self.name}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTWindowRow(ASTBase):
-    """窗口函数中的行限制表达式
-
-    ROWS BETWEEN {SQLWindowRow} AND {SQLWindowRow}
-    """
+class ASTMultiAlisaExpression(ASTBase):
+    """多个别名表达式，例如：AS name1, name2, name3（在 Hive 的 LATERAL VIEW 语句中配合 json_tuple 等返回多个值的函数使用）"""
 
-    from_row: ASTWindowRowItem = dataclasses.field(kw_only=True)
-    to_row: ASTWindowRowItem = dataclasses.field(kw_only=True)
+    names: Tuple[str, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return f"ROWS BETWEEN {self.from_row.source(sql_type)} AND {self.to_row.source(sql_type)}"
+        names_str = ", ".join(self.names)
+        return f"AS {names_str}"
 
 
-# ---------------------------------------- 通配符表达式 ----------------------------------------
+# ---------------------------------------- 抽象语法树的一般表达式节点 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTWildcardExpression(ASTMonomialExpression):
-    """通配符表达式"""
+class ASTBinaryExpressionBase(ASTExpressionBase):
+    """二元表达式的抽象基类"""
 
-    table_name: Optional[str] = dataclasses.field(kw_only=True, default=None)
+    before_value: ASTExpressionBase = dataclasses.field(kw_only=True)
+    operator = None
+    after_value: ASTExpressionBase = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return f"{self.table_name}.*" if self.table_name is not None else "*"
-
-
-# ---------------------------------------- 别名表达式 ----------------------------------------
+        return (f"{self.before_value.source(sql_type)} {self.operator.source(sql_type)} "
+                f"{self.after_value.source(sql_type)}")
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTAlisaExpression(ASTBase):
-    """别名表达式，例如：AS name"""
+class ASTColumnNameExpression(ASTExpressionBase):
+    """列名表达式"""
 
-    name: str = dataclasses.field(kw_only=True)
+    table_name: Optional[str] = dataclasses.field(kw_only=True, default=None)  # 表名称
+    column_name: str = dataclasses.field(kw_only=True)  # 字段名称
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return f"AS {self.name}"
+        if self.column_name not in {"*", "CURRENT_DATE", "CURRENT_TIME", "CURRENT_TIMESTAMP"}:
+            result = (f"`{self.table_name}`.`{self.column_name}`" if self.table_name is not None
+                      else f"`{self.column_name}`")
+        else:
+            result = f"`{self.table_name}`.{self.column_name}" if self.table_name is not None else f"{self.column_name}"
+        if sql_type == SQLType.DB2:
+            # 兼容 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
+            result = result.replace("CURRENT_DATE", "CURRENT DATE")
+            result = result.replace("CURRENT_TIME", "CURRENT TIME")
+            result = result.replace("CURRENT_TIMESTAMP", "CURRENT TIMESTAMP")
+        return result
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTMultiAlisaExpression(ASTBase):
-    """多个别名表达式，例如：AS name1, name2, name3（在 Hive 的 LATERAL VIEW 语句中配合 json_tuple 等返回多个值的函数使用）"""
+class ASTLiteralExpression(ASTExpressionBase):
+    """字面值表达式"""
 
-    names: Tuple[str, ...] = dataclasses.field(kw_only=True)
+    value: str = dataclasses.field(kw_only=True)  # 字面值
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        names_str = ", ".join(self.names)
-        return f"AS {names_str}"
+        return self.value
+
+    def as_int(self) -> int:
+        """将字面值作为整形返回"""
+        if is_int_literal(self.value):
+            return int(self.value)
+        raise SqlParseError(f"无法字面值 {self.value} 转化为整型")
 
+    def as_string(self) -> str:
+        """将字面值作为字符串返回"""
+        return self.value
 
-# ---------------------------------------- ORDER BY 子句元素：排序字段及排序顺序的组合 ----------------------------------------
+    def get_value(self) -> Any:
+        """返回当前字面值类型的返回值"""
+        if is_int_literal(self.value):
+            return int(self.value)
+        if is_bool_literal(self.value):
+            return self.value.upper() == "TRUE"
+        if is_float_literal(self.value):
+            return float(self.value)
+        if is_null_literal(self.value):
+            return None
+        raise KeyError(f"未知的字面值元素类型: {self.value}")
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTOrderByColumnExpression(ASTBase):
-    """ORDER BY 子句中每一个字段及排序顺序的节点"""
+class ASTWildcardExpression(ASTExpressionBase):
+    """通配符表达式"""
 
-    column: ASTExpressionBase = dataclasses.field(kw_only=True)  # 排序字段
-    order: ASTOrderType = dataclasses.field(kw_only=True)  # 排序类型
-    nulls_first: bool = dataclasses.field(kw_only=True)  # 是否包含 NULLS FIRST 关键字（将 NULL 值放到开头）
-    nulls_last: bool = dataclasses.field(kw_only=True)  # 是否包含 NULLS LAST 关键字（将 NULL 值放到末尾）
+    table_name: Optional[str] = dataclasses.field(kw_only=True, default=None)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        nulls_first_str = " NULLS FIRST" if self.nulls_first else ""
-        nulls_last_str = " NULLS LAST" if self.nulls_last else ""
-        if self.order.source(sql_type) == "ASC":
-            return f"{self.column.source(sql_type)}{nulls_first_str}{nulls_last_str}"
-        return f"{self.column.source(sql_type)} DESC{nulls_first_str}{nulls_last_str}"
-
-
-# ---------------------------------------- 函数表达式 ----------------------------------------
+        return f"{self.table_name}.*" if self.table_name is not None else "*"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTFunctionExpression(ASTMonomialExpression, abc.ABC):
+class ASTFunctionExpressionBase(ASTExpressionBase, abc.ABC):
     """函数表达式的抽象基类"""
 
-    name: ASTFunctionName = dataclasses.field(kw_only=True)
+    name: ASTFunctionNameExpression = dataclasses.field(kw_only=True)
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTNormalFunctionExpression(ASTFunctionExpression):
+class ASTNormalFunctionExpression(ASTFunctionExpressionBase):
     """包含一般参数的函数表达式"""
 
-    params: Tuple[AliasGeneralExpression] = dataclasses.field(kw_only=True)  # 函数表达式的参数
+    params: Tuple[ASTExpressionBase, ...] = dataclasses.field(kw_only=True)  # 函数表达式的参数
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"{self.name.source()}({self._get_param_str(sql_type)})"
 
     def _get_param_str(self, sql_type: SQLType) -> str:
         return ", ".join(param.source(sql_type) for param in self.params)
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTAggregationFunctionExpression(ASTNormalFunctionExpression):
+class ASTAggregationFunction(ASTNormalFunctionExpression):
     """聚合函数表达式"""
 
     is_distinct: bool = dataclasses.field(kw_only=True)  # 是否包含 DISTINCT 关键字
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         is_distinct = "DISTINCT " if self.is_distinct is True else ""
         return f"{self.name.source()}({is_distinct}{self._get_param_str(sql_type)})"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTCastFunctionExpression(ASTFunctionExpression):
+class ASTCastFunctionExpression(ASTFunctionExpressionBase):
     """Cast 函数表达式"""
 
-    name: ASTFunctionName = dataclasses.field(init=False, default=ASTFunctionName.by_name("CAST"))
+    name: ASTFunctionNameExpression = dataclasses.field(init=False, default=ASTFunctionNameExpression.by_name("CAST"))
     column_expression: ASTExpressionBase = dataclasses.field(kw_only=True)  # CAST 表达式中要转换的列表达式
     cast_type: ASTCastDataType = dataclasses.field(kw_only=True)  # CAST 参数中目标要转换的函数类型
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return (f"{self.name.source()}"
                 f"({self.column_expression.source(sql_type)} AS {self.cast_type.source(sql_type)})")
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTExtractFunctionExpression(ASTFunctionExpression):
+class ASTExtractFunctionExpression(ASTFunctionExpressionBase):
     """Extract 函数表达式"""
 
-    name: ASTFunctionName = dataclasses.field(init=False, default=ASTFunctionName.by_name("EXTRACT"))
+    name: ASTFunctionNameExpression = dataclasses.field(init=False,
+                                                        default=ASTFunctionNameExpression.by_name("EXTRACT"))
     extract_name: ASTExpressionBase = dataclasses.field(kw_only=True)  # FROM 关键字之前的提取名称
     column_expression: ASTExpressionBase = dataclasses.field(kw_only=True)  # FROM 关键字之后的一般表达式
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return (f"{self.name.source()}({self.extract_name.source(sql_type)} "
                 f"FROM {self.column_expression.source(sql_type)})")
 
 
-# ---------------------------------------- 布尔值表达式 ----------------------------------------
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTConditionExpression(ASTExpressionBase, abc.ABC):
-    """条件表达式"""
-
-    is_not: bool = dataclasses.field(kw_only=True)  # 一元表达式
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolOperatorExpression(ASTConditionExpression, abc.ABC):
-    """布尔值表达式：通过运算符或关键字比较运算符前后两个表达式的抽象类"""
-
-    before_value: AliasConditionExpression = dataclasses.field(kw_only=True)
-    after_value: AliasConditionExpression = dataclasses.field(kw_only=True)
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolCompareExpression(ASTBoolOperatorExpression):
-    """比较运算符布尔值表达式"""
-
-    operator: ASTCompareOperator = dataclasses.field(kw_only=True)
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        is_not_str = "NOT " if self.is_not else ""
-        return (f"{is_not_str}{self.before_value.source(sql_type)} {self.operator.source(sql_type)} "
-                f"{self.after_value.source(sql_type)}")
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolIsExpression(ASTBoolOperatorExpression):
-    """IS运算符布尔值表达式"""
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        keyword = "IS NOT" if self.is_not else "IS"
-        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolInExpression(ASTBoolOperatorExpression):
-    """In 关键字的布尔值表达式"""
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        keyword = "NOT IN " if self.is_not else "IN"
-        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolLikeExpression(ASTBoolOperatorExpression):
-    """LIKE 运算符关联表达式"""
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        keyword = "NOT LIKE" if self.is_not else "LIKE"
-        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolRlikeExpression(ASTBoolOperatorExpression):
-    """RLIKE 运算符关联表达式"""
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        keyword = "NOT RLIKE" if self.is_not else "RLIKE"
-        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolRegexpExpression(ASTBoolOperatorExpression):
-    """RLIKE 运算符关联表达式"""
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        keyword = "NOT REGEXP" if self.is_not else "REGEXP"
-        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
-
+class ASTWindowRowItem(ASTBase):
+    """窗口函数中的行限制
 
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolExistsExpression(ASTConditionExpression):
-    """Exists 运算符关联表达式"""
+    unbounded preceding = 当前行的所有行
+    n preceding = 当前行之前的 n 行
+    current row = 当前行
+    n following = 当前行之后的 n行
+    unbounded following = 当前行之后的所有行
+    """
 
-    after_value: AliasPolynomialExpression = dataclasses.field(kw_only=True)
+    row_type: static.EnumWindowRowType = dataclasses.field(kw_only=True)
+    is_unbounded: bool = dataclasses.field(kw_only=True, default=False)
+    row_num: Optional[int] = dataclasses.field(kw_only=True, default=None)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        keyword = "NOT EXISTS" if self.is_not else "EXISTS"
-        return f"{keyword} {self.after_value.source(sql_type)}"
+        if self.row_type == static.EnumWindowRowType.CURRENT_ROW:
+            return "CURRENT ROW"
+        row_type_str = self.row_type.value
+        if self.is_unbounded is True:
+            return f"UNBOUNDED {row_type_str}"
+        return f"{self.row_num} {row_type_str}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTBoolBetweenExpression(ASTConditionExpression):
-    """BETWEEN 关联表达式"""
-
-    before_value: AliasPolynomialExpression = dataclasses.field(kw_only=True)
-    from_value: AliasPolynomialExpression = dataclasses.field(kw_only=True)
-    to_value: AliasPolynomialExpression = dataclasses.field(kw_only=True)
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        if_not_str = "NOT " if self.is_not else ""
-        return (f"{self.before_value.source(sql_type)} {if_not_str}"
-                f"BETWEEN {self.from_value.source(sql_type)} AND {self.to_value.source(sql_type)}")
-
-
-# ---------------------------------------- 数组下标表达式 ----------------------------------------
-
+class ASTWindowRow(ASTBase):
+    """窗口函数中的行限制表达式
 
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTArrayIndexExpression(ASTMonomialExpression):
-    """数组下标表达式"""
+    ROWS BETWEEN {SQLWindowRow} AND {SQLWindowRow}
+    """
 
-    array: ASTExpressionBase = dataclasses.field(kw_only=True)
-    idx: AliasPolynomialExpression = dataclasses.field(kw_only=True)
+    from_row: ASTWindowRowItem = dataclasses.field(kw_only=True)
+    to_row: ASTWindowRowItem = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        if sql_type != SQLType.HIVE:
-            raise UnSupportSqlTypeError(f"数组下标不支持SQL类型:{sql_type}")
-        return f"{self.array.source(sql_type)}"
-
-
-# ---------------------------------------- 窗口表达式 ----------------------------------------
+        return f"ROWS BETWEEN {self.from_row.source(sql_type)} AND {self.to_row.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTWindowExpression(ASTMonomialExpression):
-    """【单项表达式】窗口表达式"""
+class ASTWindowExpression(ASTExpressionBase):
+    """【元素表达式】窗口表达式"""
 
-    window_function: Union[ASTNormalFunctionExpression, ASTArrayIndexExpression] = dataclasses.field(kw_only=True)
+    window_function: Union[ASTNormalFunctionExpression, "ASTIndexExpression"] = dataclasses.field(kw_only=True)
     partition_by_columns: Tuple[ASTExpressionBase, ...] = dataclasses.field(kw_only=True)
-    order_by_columns: Tuple[ASTOrderByColumnExpression, ...] = dataclasses.field(kw_only=True)
+    order_by_columns: Tuple["ASTOrderByColumn", ...] = dataclasses.field(kw_only=True)
     row_expression: Optional[ASTWindowRow] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         result = f"{self.window_function.source(sql_type)} OVER ("
         parenthesis = []
         if len(self.partition_by_columns) > 0:
@@ -888,45 +597,28 @@
             parenthesis.append(f"ORDER BY {order_by_str}")
         if self.row_expression is not None:
             parenthesis.append(self.row_expression.source(sql_type))
         result += " ".join(parenthesis) + ")"
         return result
 
 
-# ---------------------------------------- 条件表达式 ----------------------------------------
-
-
-@dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTGeneralExpression(ASTExpressionBase):
-    """一般表达式"""
-
-    elements: Tuple[AliasGeneralExpressionElement, ...] = dataclasses.field(kw_only=True)
-
-    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        return " ".join(element.source(sql_type) for element in self.elements)
-
-
-# ---------------------------------------- CASE 表达式 ----------------------------------------
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTCaseConditionItem(ASTBase):
     """第 1 种格式的 CASE 表达式的 WHEN ... THEN ... 语句节点"""
 
-    when: ASTGeneralExpression = dataclasses.field(kw_only=True)
+    when: ASTExpressionBase = dataclasses.field(kw_only=True)
     then: ASTExpressionBase = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"WHEN {self.when.source(sql_type)} THEN {self.then.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTCaseConditionExpression(ASTMonomialExpression):
+class ASTCaseConditionExpression(ASTExpressionBase):
     """第 1 种格式的 CASE 表达式
 
     CASE
         WHEN {条件表达式} THEN {一般表达式}
         ELSE {一般表达式}
     END
     """
@@ -954,15 +646,15 @@
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"WHEN {self.when.source(sql_type)} THEN {self.then.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTCaseValueExpression(ASTMonomialExpression):
+class ASTCaseValueExpression(ASTExpressionBase):
     """第 2 种格式的 CASE 表达式
 
     CASE {一般表达式}
         WHEN {一般表达式} THEN {一般表达式}
         ELSE {一般表达式}
     END
     """
@@ -978,143 +670,239 @@
             result.append(f"    {item.source(sql_type)}")
         if self.else_value is not None:
             result.append(f"    ELSE {self.else_value.source(sql_type)}")
         result.append("END")
         return "\n".join(result)
 
 
-# ---------------------------------------- 计算表达式 ----------------------------------------
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTSubQueryExpression(ASTExpressionBase):
+    """【元素表达式】子查询表达式"""
+
+    statement: "ASTSelectStatement" = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return f"({self.statement.source(sql_type)})"
+
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTPolynomialExpression(ASTExpressionBase):
-    """【多项表达式】计算表达式"""
+class ASTSubValueExpression(ASTExpressionBase):
+    """【元素表达式】值表达式：INSERT INTO 表达式中，VALUES 里的表达式"""
 
-    elements: Tuple[AliasPolynomialExpressionElement, ...] = dataclasses.field(kw_only=True)
+    values: Tuple[ASTExpressionBase, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return " ".join(element.source(sql_type) for element in self.elements)
+        values_str = ", ".join(value.source(sql_type) for value in self.values)
+        return f"({values_str})"
 
 
-# ---------------------------------------- 子查询表达式 ----------------------------------------
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTIndexExpression(ASTExpressionBase):
+    """下标表达式"""
+
+    array: ASTExpressionBase = dataclasses.field(kw_only=True)
+    idx: ASTExpressionBase = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        if sql_type != SQLType.HIVE:
+            raise UnSupportSqlTypeError(f"数组下标不支持SQL类型:{sql_type}")
+        return f"{self.array.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTParenthesisExpression(ASTMonomialExpression, abc.ABC):
-    """【单项表达式】插入语表达式"""
+class ASTUnaryExpression(ASTExpressionBase):
+    """一元表达式
+
+    样例：~1、+1、-1
+    """
+
+    operator: ASTComputeOperator = dataclasses.field(kw_only=True)  # 一元运算符
+    expression: ASTExpressionBase = dataclasses.field(kw_only=True)  # 表达式
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return f"{self.operator.source(sql_type=sql_type)}{self.expression.source(sql_type=sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTSubQueryExpression(ASTParenthesisExpression):
-    """【单项表达式】子查询表达式"""
+class ASTComputeExpression(ASTBinaryExpressionBase):
+    """运算表达式"""
+
+    operator: ASTComputeOperator = dataclasses.field(kw_only=True)
 
-    statement: "ASTSelectStatement" = dataclasses.field(kw_only=True)
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTOperatorExpressionBase(ASTExpressionBase, abc.ABC):
+    """【一般表达式：关键字条件表达式层级】包含前后两个元素的关键字条件表达式"""
+
+    is_not: bool = dataclasses.field(kw_only=True)
+    before_value: ASTExpressionBase = dataclasses.field(kw_only=True)
+    after_value: ASTExpressionBase = dataclasses.field(kw_only=True)
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTIsExpression(ASTOperatorExpressionBase):
+    """【一般表达式：关键字条件表达式层级】IS 运算符布尔值表达式"""
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return f"({self.statement.source(sql_type)})"
+        keyword = "IS NOT" if self.is_not else "IS"
+        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTSubGeneralExpression(ASTParenthesisExpression):
-    """【单项表达式】插入语一般表达式"""
+class ASTInExpression(ASTOperatorExpressionBase):
+    """【一般表达式：关键字条件表达式层级】IN 关键字的布尔值表达式"""
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        keyword = "NOT IN " if self.is_not else "IN"
+        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
 
-    expression: AliasGeneralExpression = dataclasses.field(kw_only=True)
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTLikeExpression(ASTOperatorExpressionBase):
+    """【一般表达式：关键字条件表达式层级】LIKE 运算符关联表达式"""
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        return f"({self.expression.source(sql_type)})"
+        """返回语法节点的 SQL 源码"""
+        keyword = "NOT LIKE" if self.is_not else "LIKE"
+        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTSubValueExpression(ASTParenthesisExpression):
-    """【单项表达式】值表达式：INSERT INTO 表达式中，VALUES 里的表达式"""
+class ASTRlikeExpression(ASTOperatorExpressionBase):
+    """【一般表达式：关键字条件表达式层级】RLIKE 运算符关联表达式"""
 
-    values: Tuple[ASTExpressionBase, ...] = dataclasses.field(kw_only=True)
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        keyword = "NOT RLIKE" if self.is_not else "RLIKE"
+        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTRegexpExpression(ASTOperatorExpressionBase):
+    """【一般表达式：关键字条件表达式层级】REGEXP 运算符关联表达式"""
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        values_str = ", ".join(value.source(sql_type) for value in self.values)
-        return f"({values_str})"
+        keyword = "NOT REGEXP" if self.is_not else "REGEXP"
+        return f"{self.before_value.source(sql_type)} {keyword} {self.after_value.source(sql_type)}"
 
 
-# ---------------------------------------- 关联表达式 ----------------------------------------
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTExistsExpression(ASTExpressionBase):
+    """【一般表达式：关键字条件表达式层级】Exists 运算符关联表达式"""
 
+    value: ASTExpressionBase = dataclasses.field(kw_only=True)  # 子查询
 
-class ASTJoinExpression(ASTBase, abc.ABC):
-    """关联表达式"""
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return f"EXISTS {self.value.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTJoinOnExpression(ASTJoinExpression):
-    """ON 关联表达式"""
+class ASTBetweenExpression(ASTExpressionBase):
+    """【一般表达式：关键字条件表达式层级】BETWEEN 关联表达式"""
 
-    condition: ASTGeneralExpression = dataclasses.field(kw_only=True)
+    is_not: bool = dataclasses.field(kw_only=True)  # 一元表达式
+    before_value: ASTExpressionBase = dataclasses.field(kw_only=True)
+    from_value: ASTExpressionBase = dataclasses.field(kw_only=True)
+    to_value: ASTExpressionBase = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return f"ON {self.condition.source(sql_type)}"
+        if_not_str = "NOT " if self.is_not else ""
+        return (f"{self.before_value.source(sql_type)} {if_not_str}"
+                f"BETWEEN {self.from_value.source(sql_type)} AND {self.to_value.source(sql_type)}")
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTJoinUsingExpression(ASTJoinExpression):
-    """USING 关联表达式"""
+class ASTOperatorConditionExpression(ASTBinaryExpressionBase):
+    """运算符条件表达式"""
+
+    operator: ASTCompareOperator = dataclasses.field(kw_only=True)
 
-    using_function: ASTFunctionExpression = dataclasses.field(kw_only=True)
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTLogicalNotExpression(ASTExpressionBase):
+    """逻辑否表达式"""
+
+    operator = ASTLogicalOperator(enum=static.EnumLogicalOperator.LOGICAL_NOT)
+    expression: ASTExpressionBase = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
-        return f"{self.using_function.source(sql_type)}"
+        return f"{self.operator.source(sql_type)} {self.expression.source(sql_type)}"
 
 
-# ---------------------------------------- 表表达式 ----------------------------------------
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTLogicalAndExpression(ASTBinaryExpressionBase):
+    """逻辑与表达式"""
 
+    operator = ASTLogicalOperator(enum=static.EnumLogicalOperator.LOGICAL_AND)
 
-AliasTableExpression = Union[ASTTableName, ASTSubQueryExpression]  # 表表达式（表名表达式或子查询表达式）
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTLogicalXorExpression(ASTBinaryExpressionBase):
+    """逻辑异或表达式"""
+
+    operator = ASTLogicalOperator(enum=static.EnumLogicalOperator.LOGICAL_XOR)
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTFromTableExpression(ASTBase):
+class ASTLogicalOrExpression(ASTBinaryExpressionBase):
+    """逻辑或表达式"""
+
+    operator = ASTLogicalOperator(enum=static.EnumLogicalOperator.LOGICAL_OR)
+
+
+# ---------------------------------------- 表表达式 ----------------------------------------
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTFromTable(ASTBase):
     """表表达式"""
 
-    name: AliasTableExpression = dataclasses.field(kw_only=True)
+    name: Union[ASTTableNameExpression, ASTSubQueryExpression] = dataclasses.field(kw_only=True)
     alias: Optional[ASTAlisaExpression] = dataclasses.field(kw_only=True, default=None)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         if self.alias is not None:
             return f"{self.name.source(sql_type)} {self.alias.source(sql_type)}"
         return f"{self.name.source(sql_type)}"
 
 
-# ---------------------------------------- 列表达式 ----------------------------------------
+# ---------------------------------------- SELECT 子句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTSelectColumnExpression(ASTBase):
+class ASTSelectColumn(ASTBase):
     """在 SELECT 语句中的每一列的表达式"""
 
     value: ASTExpressionBase = dataclasses.field(kw_only=True)
     alias: Optional[ASTAlisaExpression] = dataclasses.field(kw_only=True, default=None)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         if self.alias is not None:
             return f"{self.value.source(sql_type)} {self.alias.source(sql_type)}"
         return f"{self.value.source(sql_type)}"
 
 
-# ---------------------------------------- SELECT 子句 ----------------------------------------
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTSelectClause(ASTBase):
     """SELECT 子句"""
 
     distinct: bool = dataclasses.field(kw_only=True)
-    columns: Tuple[ASTSelectColumnExpression, ...] = dataclasses.field(kw_only=True)
+    columns: Tuple[ASTSelectColumn, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         result = ["SELECT"]
         if self.distinct is True:
             result.append("DISTINCT")
         result.append(", ".join(column.source(sql_type) for column in self.columns))
@@ -1123,49 +911,71 @@
 
 # ---------------------------------------- FROM 子句 ----------------------------------------
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTFromClause(ASTBase):
     """FROM 子句"""
 
-    tables: Tuple[ASTFromTableExpression, ...] = dataclasses.field(kw_only=True)
+    tables: Tuple[ASTFromTable, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return "FROM " + ", ".join(table.source(sql_type) for table in self.tables)
 
 
 # ---------------------------------------- LATERAL VIEW 子句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTLateralViewClause(ASTBase):
     """LATERAL VIEW 子句"""
 
     outer: bool = dataclasses.field(kw_only=True)
-    function: ASTFunctionExpression = dataclasses.field(kw_only=True)
+    function: ASTFunctionExpressionBase = dataclasses.field(kw_only=True)
     view_name: str = dataclasses.field(kw_only=True)
     alias: ASTMultiAlisaExpression = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         outer_str = "OUT " if self.outer is True else ""
         return (f"LATERAL VIEW {outer_str}{self.function.source(sql_type)} "
                 f"{self.view_name} {self.alias.source(sql_type)}")
 
 
 # ---------------------------------------- JOIN 子句 ----------------------------------------
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTJoinOnExpression(ASTBase):
+    """ON 关联表达式"""
+
+    condition: ASTLogicalOrExpression = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return f"ON {self.condition.source(sql_type)}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTJoinUsingExpression(ASTBase):
+    """USING 关联表达式"""
+
+    using_function: ASTFunctionExpressionBase = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return f"{self.using_function.source(sql_type)}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTJoinClause(ASTBase):
     """JOIN 子句"""
 
     type: ASTJoinType = dataclasses.field(kw_only=True)
-    table: ASTFromTableExpression = dataclasses.field(kw_only=True)
-    rule: Optional[ASTJoinExpression] = dataclasses.field(kw_only=True)
+    table: ASTFromTable = dataclasses.field(kw_only=True)
+    rule: Optional[Union[ASTJoinOnExpression, ASTJoinUsingExpression]] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         if self.rule is not None:
             return (f"{self.type.source(sql_type)} {self.table.source(sql_type)} "
                     f"{self.rule.source(sql_type)}")
         return f"{self.type.source(sql_type)} {self.table.source(sql_type)}"
@@ -1174,15 +984,15 @@
 # ---------------------------------------- WHERE 子句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTWhereClause(ASTBase):
     """WHERE 子句"""
 
-    condition: ASTGeneralExpression = dataclasses.field(kw_only=True)
+    condition: ASTLogicalOrExpression = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"WHERE {self.condition.source(sql_type)}"
 
 
 # ---------------------------------------- GROUP BY 子句 ----------------------------------------
@@ -1206,61 +1016,81 @@
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTGroupByClause(ASTBase):
     """GROUP BY 子句"""
 
     columns: Tuple[ASTExpressionBase, ...] = dataclasses.field(kw_only=True)
     grouping_sets: ASTGroupingSets = dataclasses.field(kw_only=True)
+    with_cube: bool = dataclasses.field(kw_only=True)
     with_rollup: bool = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         columns_str = ", ".join(column.source(sql_type) for column in self.columns)
         grouping_sets_str = f" {self.grouping_sets.source(sql_type)}" if self.grouping_sets is not None else ""
+        with_cube_str = " WITH CUBE" if self.with_cube is True else ""
         with_rollup_str = " WITH ROLLUP" if self.with_rollup is True else ""
-        return f"GROUP BY {columns_str}{grouping_sets_str}{with_rollup_str}"
+        return f"GROUP BY {columns_str}{grouping_sets_str}{with_cube_str}{with_rollup_str}"
 
 
 # ---------------------------------------- HAVING 子句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTHavingClause(ASTBase):
     """HAVING 子句"""
 
-    condition: ASTGeneralExpression = dataclasses.field(kw_only=True)
+    condition: ASTLogicalOrExpression = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"HAVING {self.condition.source(sql_type)}"
 
 
 # ---------------------------------------- ORDER BY 子句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTOrderByColumn(ASTBase):
+    """ORDER BY 子句中每一个字段及排序顺序的节点"""
+
+    column: ASTExpressionBase = dataclasses.field(kw_only=True)  # 排序字段
+    order: ASTOrderType = dataclasses.field(kw_only=True)  # 排序类型
+    nulls_first: bool = dataclasses.field(kw_only=True)  # 是否包含 NULLS FIRST 关键字（将 NULL 值放到开头）
+    nulls_last: bool = dataclasses.field(kw_only=True)  # 是否包含 NULLS LAST 关键字（将 NULL 值放到末尾）
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        nulls_first_str = " NULLS FIRST" if self.nulls_first else ""
+        nulls_last_str = " NULLS LAST" if self.nulls_last else ""
+        if self.order.source(sql_type) == "ASC":
+            return f"{self.column.source(sql_type)}{nulls_first_str}{nulls_last_str}"
+        return f"{self.column.source(sql_type)} DESC{nulls_first_str}{nulls_last_str}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTOrderByClause(ASTBase):
     """ORDER BY 子句"""
 
-    columns: Tuple[ASTOrderByColumnExpression, ...] = dataclasses.field(kw_only=True)
+    columns: Tuple[ASTOrderByColumn, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         result = [column.source(sql_type) for column in self.columns]
         return "ORDER BY " + ", ".join(result)
 
 
 # ---------------------------------------- SORT BY 子句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTSortByClause(ASTBase):
     """SORT BY 子句（Hive）"""
 
-    columns: Tuple[ASTOrderByColumnExpression, ...] = dataclasses.field(kw_only=True)
+    columns: Tuple[ASTOrderByColumn, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         result = [column.source(sql_type) for column in self.columns]
         return "SORT BY " + ", ".join(result)
 
 
@@ -1345,19 +1175,24 @@
         return len(self.tables) == 0
 
 
 # ---------------------------------------- SELECT 语句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTSelectStatement(ASTStatementBase, abc.ABC):
-    """SELECT 语句"""
+class ASTStatementHasWithClauseBase(ASTStatementBase, abc.ABC):
+    """包含 WITH 语句的语句的抽象基类"""
 
     with_clause: Optional[ASTWithClause] = dataclasses.field(kw_only=True, default=None)
 
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTSelectStatement(ASTStatementHasWithClauseBase, abc.ABC):
+    """SELECT 语句"""
+
     @abc.abstractmethod
     def set_with_clauses(self, with_clause: Optional[ASTWithClause]) -> "ASTSelectStatement":
         """设置 WITH 语句"""
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTSingleSelectStatement(ASTSelectStatement):
@@ -1420,48 +1255,44 @@
         params["with_clause"] = with_clause
         return ASTUnionSelectStatement(**params)
 
 
 # ---------------------------------------- 分区表达式 ----------------------------------------
 
 
-AliasPartitionParam = Union[ASTPolynomialExpression, ASTBoolCompareExpression]  # 分区参数：包含动态分区和非动态分区两种情况
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTPartitionExpression(ASTBase):
     """分区表达式：PARTITION (<partition_expression>)"""
 
-    partitions: Tuple[AliasPartitionParam, ...] = dataclasses.field(kw_only=True)
+    partitions: Tuple[ASTExpressionBase, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         partition_list_str = ", ".join(partition.source(sql_type) for partition in self.partitions)
         return f"PARTITION ({partition_list_str})"
 
 
 # ---------------------------------------- INSERT 语句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
-class ASTInsertStatement(ASTStatementBase, abc.ABC):
+class ASTInsertStatement(ASTStatementHasWithClauseBase, abc.ABC):
     """INSERT 表达式
 
     两个子类包含 VALUES 和 SELECT 两种方式
 
     INSERT {INTO|OVERWRITE} [TABLE] <table_name_expression> [PARTITION (<partition_expression>)]
     [(<colum_name_expression [,<column_name_expression> ...]>)]
     {VALUES <value_expression> [,<value_expression> ...] | <select_statement>}
     """
 
-    with_clause: Optional[ASTWithClause] = dataclasses.field(kw_only=True, default=None)
     insert_type: ASTInsertType = dataclasses.field(kw_only=True)
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
     partition: Optional[ASTPartitionExpression] = dataclasses.field(kw_only=True)
-    columns: Optional[Tuple[ASTColumnName, ...]] = dataclasses.field(kw_only=True)
+    columns: Optional[Tuple[ASTColumnNameExpression, ...]] = dataclasses.field(kw_only=True)
 
     def _insert_str(self, sql_type: SQLType) -> str:
         insert_type_str = self.insert_type.source(sql_type)
         table_keyword_str = "TABLE " if sql_type == SQLType.HIVE else ""
         partition_str = f"{self.partition.source(sql_type)} " if self.partition is not None else ""
         if self.columns is not None:
             columns_str = "(" + ", ".join(column.source(sql_type) for column in self.columns) + ") "
@@ -1513,16 +1344,23 @@
 class ASTColumnTypeExpression(ASTBase):
     """字段类型表达式"""
 
     name: str = dataclasses.field(kw_only=True)
     params: Optional[Tuple[ASTExpressionBase, ...]] = dataclasses.field(kw_only=True, default=None)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
-        """返回语法节点的 SQL 源码"""
-        if self.params is None or sql_type == SQLType.HIVE:
+        """返回语法节点的 SQL 源码
+        
+        TODO：后续计划将类型的处理，移动到翻译器中，而不是放置在 Node 节点中，因为这并不是一个适用于所有应用场景的功能，可能会引发特殊的 Bug
+        """
+        # 如果没有参数，则不添加参数
+        if self.params is None:
+            return self.name
+        # 如果为 Hive 中没有参数的类型，也不添加参数
+        if sql_type == SQLType.HIVE and self.name.upper() not in {"DECIMAL", "VARCHAR", "CHAR"}:
             return self.name
         # MySQL 标准导出逗号间没有空格
         type_params = "(" + ",".join([param.source(sql_type) for param in self.params]) + ")"
         return f"{self.name}{type_params}"
 
 
 # ---------------------------------------- 声明字段表达式 ----------------------------------------
@@ -1678,20 +1516,17 @@
 # ---------------------------------------- CREATE TABLE 语句 ----------------------------------------
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTCreateTableStatement(ASTStatementBase):
     # pylint: disable=R0902 忽略对象属性过多的问题
 
-    """【DDL】CREATE TABLE 语句
-
-    TODO Hive 的 ROW FORMAT 和 STORED AS 属性整合
-    """
+    """【DDL】CREATE TABLE 语句"""
 
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
     if_not_exists: bool = dataclasses.field(kw_only=True)
     columns: Optional[Tuple[ASTDefineColumnExpression, ...]] = dataclasses.field(kw_only=True)
     primary_key: Optional[ASTPrimaryIndexExpression] = dataclasses.field(kw_only=True)  # MySQL
     unique_key: Optional[Tuple[ASTUniqueIndexExpression, ...]] = dataclasses.field(kw_only=True)  # MySQL
     key: Optional[Tuple[ASTNormalIndexExpression, ...]] = dataclasses.field(kw_only=True)  # MySQL
     fulltext_key: Optional[Tuple[ASTFulltextIndexExpression, ...]] = dataclasses.field(kw_only=True)  # MySQL
     foreign_key: Tuple[ASTForeignKeyExpression, ...] = dataclasses.field(kw_only=True)  # MySQL
@@ -1708,15 +1543,15 @@
     stored_as_inputformat: Optional[str] = dataclasses.field(kw_only=True, default=None)  # Hive
     stored_as_textfile: bool = dataclasses.field(kw_only=True, default=False)  # Hive
     outputformat: Optional[str] = dataclasses.field(kw_only=True, default=None)  # Hive
     location: Optional[str] = dataclasses.field(kw_only=True, default=None)  # Hive
     tblproperties: Optional[Tuple[ASTConfigStringExpression, ...]] = dataclasses.field(
         kw_only=True, default=None)  # Hive
 
-    def set_table_name(self, table_name_expression: ASTTableName) -> "ASTCreateTableStatement":
+    def set_table_name(self, table_name_expression: ASTTableNameExpression) -> "ASTCreateTableStatement":
         """设置表名并返回新对象"""
         params = self.get_params_dict()
         params["table_name"] = table_name_expression
         return ASTCreateTableStatement(**params)
 
     def change_type(self, hashmap: Dict[str, str], remove_param: bool = True):
         """更新每个字段的变量类型"""
@@ -1812,31 +1647,28 @@
         return f"CREATE TABLE{is_not_exists_str} {self.table_name.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTCreateTableAsStatement(ASTStatementBase):
     """CREATE TABLE ... AS ... 语句"""
 
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
     select_statement: ASTSelectStatement = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"CREATE TABLE {self.table_name.source(sql_type)} AS {self.select_statement.source(sql_type)}"
 
 
-AliasCreateTableStatement = Union[ASTCreateTableStatement, ASTCreateTableAsStatement]
-
-
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTDropTableStatement(ASTStatementBase):
     """DROP TABLE 语句"""
 
     if_exists: bool = dataclasses.field(kw_only=True, default=False)  # 是否包含 IF EXISTS 关键字
-    table_name: ASTTableName = dataclasses.field(kw_only=True)  # 表名
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)  # 表名
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         if_exists_str = "IF EXISTS " if self.if_exists is True else ""
         return f"DROP TABLE {if_exists_str}{self.table_name.source(sql_type)}"
 
 
@@ -1851,15 +1683,15 @@
         return f"SET {self.config.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTAnalyzeTableStatement(ASTStatementBase):
     """ANALYZE TABLE 语句"""
 
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
     partition: Optional[ASTPartitionExpression] = dataclasses.field(kw_only=True, default=None)
     for_columns: bool = dataclasses.field(kw_only=True, default=False)  # [Hive]
     cache_metadata: bool = dataclasses.field(kw_only=True, default=False)  # [Hive]
     noscan: bool = dataclasses.field(kw_only=True, default=False)  # [Hive]
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
@@ -1950,28 +1782,28 @@
         return f"DROP{if_exists_str} {self.partition.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTAlterTableStatement(ASTStatementBase):
     """ALTER TABLE 语句"""
 
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
     expressions: Tuple[ASTAlterExpressionBase, ...] = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         expressions_str = ",\n".join(expression.source(sql_type) for expression in self.expressions)
         return f"ALTER TABLE {self.table_name.source(sql_type)} \n{expressions_str}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTMsckRepairTableStatement(ASTStatementBase):
     """MSCK REPAIR TABLE 语句：扫描 HDFS 上的文件并更新元数据的分区信息"""
 
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"MSCK REPAIR TABLE {self.table_name.source(sql_type)}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
@@ -1985,12 +1817,111 @@
         return f"USE {self.schema_name}"
 
 
 @dataclasses.dataclass(slots=True, frozen=True, eq=True)
 class ASTTruncateTable(ASTStatementBase):
     """TRUNCATE TABLE 语句"""
 
-    table_name: ASTTableName = dataclasses.field(kw_only=True)
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
 
     def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
         """返回语法节点的 SQL 源码"""
         return f"TRUNCATE TABLE {self.table_name.source(sql_type)}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTUpdateSetColumn(ASTBase):
+    """UPDATE 语句的 SET 子句中的元素"""
+
+    column_name: str = dataclasses.field(kw_only=True)
+    column_value: ASTLogicalOrExpression = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return f"{self.column_name} = {self.column_value.source(sql_type)}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTUpdateSetClause(ASTBase):
+    """UPDATE 语句的 SET 子句"""
+
+    columns: Tuple[ASTUpdateSetColumn, ...] = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        columns_str = ", ".join(column.source(sql_type) for column in self.columns)
+        return f"SET {columns_str}"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTUpdateStatement(ASTStatementHasWithClauseBase):
+    """UPDATE 语句"""
+
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
+    set_clause: ASTUpdateSetClause = dataclasses.field(kw_only=True)
+    where_clause: Optional[ASTWhereClause] = dataclasses.field(kw_only=True)
+    order_by_clause: Optional[ASTOrderByClause] = dataclasses.field(kw_only=True)
+    limit_clause: Optional[ASTLimitClause] = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        with_clause_str = self.with_clause.source(sql_type) + "\n\n" if not self.with_clause.is_empty() else ""
+        result = f"{with_clause_str}UPDATE {self.table_name.source(sql_type)} {self.set_clause.source(sql_type)}"
+        if self.where_clause is not None:
+            result += f" {self.where_clause.source(sql_type)}"
+        if self.order_by_clause is not None:
+            result += f" {self.order_by_clause.source(sql_type)}"
+        if self.limit_clause is not None:
+            result += f" {self.limit_clause.source(sql_type)}"
+        return result
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTDeleteStatement(ASTStatementBase):
+    """DELETE 语句"""
+
+    table_name: ASTTableNameExpression = dataclasses.field(kw_only=True)
+    where_clause: Optional[ASTWhereClause] = dataclasses.field(kw_only=True)
+    order_by_clause: Optional[ASTOrderByClause] = dataclasses.field(kw_only=True)
+    limit_clause: Optional[ASTLimitClause] = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        result = f"DELETE FROM {self.table_name.source(sql_type)} "
+        if self.where_clause is not None:
+            result += f" {self.where_clause.source(sql_type)}"
+        if self.order_by_clause is not None:
+            result += f" {self.order_by_clause.source(sql_type)}"
+        if self.limit_clause is not None:
+            result += f" {self.limit_clause.source(sql_type)}"
+        return result
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTShowDatabasesStatement(ASTStatementBase):
+    """SHOW DATABASES 语句"""
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return "SHOW DATABASES"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTShowTablesStatement(ASTStatementBase):
+    """SHOW TABLES 语句"""
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        return "SHOW TABLES"
+
+
+@dataclasses.dataclass(slots=True, frozen=True, eq=True)
+class ASTShowColumnsStatement(ASTStatementBase):
+    """SHOW COLUMNS 语句"""
+
+    from_clause: ASTFromClause = dataclasses.field(kw_only=True)
+    where_clause: Optional[ASTWhereClause] = dataclasses.field(kw_only=True)
+
+    def source(self, sql_type: SQLType = SQLType.DEFAULT) -> str:
+        """返回语法节点的 SQL 源码"""
+        where_clause_str = f" {self.where_clause.source(sql_type)}" if self.where_clause is not None else ""
+        return f"SHOW COLUMNS {self.from_clause.source(sql_type)}{where_clause_str}"
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/core/parser.py` & `metasequoia-sql-0.6.0/metasequoia_sql/core/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,92 @@
 # pylint: disable=C0302
 
 """
 SQL 语法解析器
 
 将所有解析方法合并到这个类中，以支持插件开发。
 如需替换词法解析器，重写 build_token_scanner 方法即可。
-
-TODO 将 CURRENT_TIMESTAMP、CURRENT_DATE、CURRENT_TIME 改为单独节点处理
-TODO 兼容各个场景下额外添加的括号
-TODO 将多项表达式、条件表达式、一般表达式中，根据计算优先级，按计算顺序生成嵌套的二元表达式
-TODO 待统一额外的插入语的实现方案
 """
 
 from typing import Optional, Tuple, List, Union
 
 from metasequoia_sql.common import TokenScanner
 from metasequoia_sql.common import name_set
-from metasequoia_sql.core import node
+from metasequoia_sql.core import node, static
 from metasequoia_sql.core.sql_type import SQLType
-from metasequoia_sql.errors import SqlParseError, UnSupportSqlTypeError
+from metasequoia_sql.errors import SqlParseError
 from metasequoia_sql.lexical import AMTMark, AMTSingle, FSMMachine
 
 __all__ = ["SQLParser"]
 
+# 输入参数的类型别名
+ScannerOrString = Union[TokenScanner, str]
+
+# 两种 CREATE TABLE 语句的通用类型别名
+AliasCreateTableStatement = Union[node.ASTCreateTableStatement, node.ASTCreateTableAsStatement]
+
+# 两种 CASE 语句的通用类型别名
+AliasCaseExpression = Union[node.ASTCaseConditionExpression, node.ASTCaseValueExpression]
+
+# 表名表达式和子查询表达式的通用类型别名
+AliasTableExpression = Union[node.ASTTableNameExpression, node.ASTSubQueryExpression]
+
+# 两种 JOIN 表达式的通用类型别名
+AliasJoinExpression = Union[node.ASTJoinOnExpression, node.ASTJoinUsingExpression]
+
+# ---------------------------------------- 一般表达式层级类型 ----------------------------------------
+
+# 元素表达式层级
+NodeElementLevel = Union[
+    node.ASTColumnNameExpression, node.ASTLiteralExpression, node.ASTWildcardExpression, node.ASTFunctionExpressionBase,
+    node.ASTWindowExpression, node.ASTCaseConditionExpression, node.ASTCaseValueExpression, node.ASTSubQueryExpression,
+    node.ASTSubValueExpression]
+
+# 下标表达式层级
+NodeIndexLevel = Union[NodeElementLevel, node.ASTIndexExpression]
+
+# 一元表达式层级
+NodeUnaryLevel = Union[NodeIndexLevel, node.ASTUnaryExpression]
+
+# 按位或表达式层级
+NodeBitwiseOrLevel = Union[NodeUnaryLevel, node.ASTComputeExpression]
+
+# 关键字条件表达式层级
+NodeKeywordConditionLevel = Union[
+    NodeBitwiseOrLevel, node.ASTOperatorExpressionBase, node.ASTExistsExpression, node.ASTBetweenExpression]
+
+# 运算符条件表达式层级
+NodeOperatorConditionLevel = Union[NodeKeywordConditionLevel, node.ASTOperatorConditionExpression]
+
+# 逻辑否表达式层级
+NodeLogicalNotLevel = Union[NodeOperatorConditionLevel, node.ASTLogicalNotExpression]
+
+# 逻辑与表达式层级
+NodeLogicalAndLevel = Union[NodeLogicalNotLevel, node.ASTLogicalAndExpression]
+
+# 逻辑异或表达式层级
+NodeLogicalXorLevel = Union[NodeLogicalAndLevel, node.ASTLogicalXorExpression]
+
+# 逻辑或表达式层级（通用表达式）
+GeneralExpression = Union[NodeLogicalXorLevel, node.ASTLogicalOrExpression]
+
 
 class SQLParser:
     # pylint: disable=R0904
     """SQL 语法解析器"""
 
+    # ------------------------------ 词法扫描器构造方法 ------------------------------
+
     @classmethod
-    def build_token_scanner(cls, string: str) -> TokenScanner:
+    def _build_token_scanner(cls, string: str) -> TokenScanner:
         """构造词法扫描器"""
-        return TokenScanner(FSMMachine.parse(string), ignore_space=True, ignore_comment=True)
+        return TokenScanner(FSMMachine.parse(string))
 
     @classmethod
-    def _unify_input_scanner(cls, scanner_or_string: Union[TokenScanner, str],
+    def _unify_input_scanner(cls, scanner_or_string: ScannerOrString,
                              sql_type: SQLType = SQLType.DEFAULT) -> TokenScanner:
         """格式化输入的参数，将字符串格式的 SQL 语句统一为词法扫描器 TokenScanner"""
         if isinstance(scanner_or_string, TokenScanner):
             return scanner_or_string
         if isinstance(scanner_or_string, str):
             if sql_type == SQLType.DB2:
                 # 兼容 DB2 的 CURRENT DATE、CURRENT TIME、CURRENT TIMESTAMP 语法
@@ -46,1238 +94,1376 @@
                 scanner_or_string = scanner_or_string.replace("CURRENT TIME", "CURRENT_TIME")
                 scanner_or_string = scanner_or_string.replace("CURRENT TIMESTAMP", "CURRENT_TIMESTAMP")
 
             if sql_type == SQLType.HIVE:
                 # 兼容 HIVE 的 == 语法
                 scanner_or_string = scanner_or_string.replace("==", "=")
 
-            return cls.build_token_scanner(scanner_or_string)
+            return cls._build_token_scanner(scanner_or_string)
         raise SqlParseError(f"未知的参数类型: {scanner_or_string} (type={type(scanner_or_string)})")
 
-    # ------------------------------ 枚举类节点的解析方法 ------------------------------
+    # ------------------------------ 通用工具方法 ------------------------------
 
     @classmethod
-    def check_insert_type(cls, scanner_or_string: Union[TokenScanner, str],
-                          sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为插入类型"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return (scanner.search_and_move("INSERT", "INTO") or
-                scanner.search_and_move("INSERT", "OVERWRITE"))
+    def _unify_name(cls, text: Optional[str]) -> Optional[str]:
+        """格式化名称标识符：剔除名称前后的引号"""
+        return text.strip("`") if text is not None else None
+
+    @classmethod
+    def _get_alias_name(cls, scanner: TokenScanner) -> str:
+        """获取别名：如果抽象词法树（AMT）没有 NAME 标记，则抛出异常"""
+        if not scanner.search_one_type_mark(AMTMark.NAME):
+            raise SqlParseError(f"无法解析为名称: {scanner}")
+        return cls._unify_name(scanner.pop_as_source())
+
+    @classmethod
+    def _parse_config_string(cls, scanner: TokenScanner) -> str:
+        """解析配置名称或配置值：字符串中允许包含 . 符合和 - 符合"""
+        column_string = [scanner.pop_as_source()]
+        while True:
+            if scanner.search_and_move_one_type_str("."):
+                column_string.append(".")
+                column_string.append(scanner.pop_as_source())
+            elif scanner.search_and_move_one_type_str("-"):
+                column_string.append("-")
+                column_string.append(scanner.pop_as_source())
+            else:
+                break
+        return "".join(column_string)
+
+    # ------------------------------ 枚举类节点的解析方法 ------------------------------
 
     @classmethod
-    def parse_insert_type(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_insert_type(cls, scanner_or_string: ScannerOrString,
                           sql_type: SQLType = SQLType.DEFAULT) -> node.ASTInsertType:
         """解析插入类型"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("INSERT", "INTO"):
-            return node.ASTInsertType(enum=node.EnumInsertType.INSERT_INTO)
-        if scanner.search_and_move("INSERT", "IGNORE", "INTO"):
-            return node.ASTInsertType(enum=node.EnumInsertType.INSERT_INTO)
-        if scanner.search_and_move("INSERT", "OVERWRITE"):
-            return node.ASTInsertType(enum=node.EnumInsertType.INSERT_OVERWRITE)
-        raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
+        return cls._parse_insert_type(scanner)
 
     @classmethod
-    def check_join_type(cls, scanner_or_string: Union[TokenScanner, str], sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为关联类型"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for join_type in node.EnumJoinType:
-            if scanner.search(*join_type.value):
-                return True
-        return False
+    def _parse_insert_type(cls, scanner: TokenScanner) -> node.ASTInsertType:
+        if scanner.search_and_move_two_type_str_use_upper("INSERT", "INTO"):
+            return node.ASTInsertType(enum=static.EnumInsertType.INSERT_INTO)
+        if scanner.search_and_move_three_type_str_use_upper("INSERT", "IGNORE", "INTO"):
+            return node.ASTInsertType(enum=static.EnumInsertType.INSERT_INTO)
+        if scanner.search_and_move_two_type_str_use_upper("INSERT", "OVERWRITE"):
+            return node.ASTInsertType(enum=static.EnumInsertType.INSERT_OVERWRITE)
+        raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
 
     @classmethod
-    def parse_join_type(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_join_type(cls, scanner_or_string: ScannerOrString,
                         sql_type: SQLType = SQLType.DEFAULT) -> node.ASTJoinType:
         """解析关联类型"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for join_type in node.EnumJoinType:
+        return cls._parse_join_type(scanner)
+
+    @classmethod
+    def _parse_join_type(cls, scanner: TokenScanner) -> node.ASTJoinType:
+        for join_type in static.EnumJoinType:
             if scanner.search_and_move(*join_type.value):
                 return node.ASTJoinType(enum=join_type)
         raise SqlParseError(f"无法解析的关联类型: {scanner}")
 
     @classmethod
-    def parse_order_type(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_order_type(cls, scanner_or_string: ScannerOrString,
                          sql_type: SQLType = SQLType.DEFAULT) -> node.ASTOrderType:
         """解析排序类型"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("DESC"):
-            return node.ASTOrderType(enum=node.EnumOrderType.DESC)
-        if scanner.search_and_move("ASC"):
-            return node.ASTOrderType(enum=node.EnumOrderType.ASC)
-        return node.ASTOrderType(enum=node.EnumOrderType.ASC)
+        return cls._parse_order_type(scanner)
 
     @classmethod
-    def check_union_type(cls, scanner_or_string: Union[TokenScanner, str], sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为组合类型"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for union_type in node.EnumUnionType:
-            if scanner.search(*union_type.value):
-                return True
-        return False
+    def _parse_order_type(cls, scanner: TokenScanner) -> node.ASTOrderType:
+        if scanner.search_and_move_one_type_str_use_upper("DESC"):
+            return node.ASTOrderType(enum=static.EnumOrderType.DESC)
+        if scanner.search_and_move_one_type_str_use_upper("ASC"):
+            return node.ASTOrderType(enum=static.EnumOrderType.ASC)
+        return node.ASTOrderType(enum=static.EnumOrderType.ASC)
 
     @classmethod
-    def parse_union_type(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_union_type(cls, scanner_or_string: ScannerOrString,
                          sql_type: SQLType = SQLType.DEFAULT) -> node.ASTUnionType:
         """解析组合类型"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for union_type in node.EnumUnionType:
+        return cls._parse_union_type(scanner)
+
+    @classmethod
+    def _parse_union_type(cls, scanner: TokenScanner) -> node.ASTUnionType:
+        for union_type in static.EnumUnionType:
             if scanner.search_and_move(*union_type.value):
                 return node.ASTUnionType(enum=union_type)
         raise SqlParseError(f"无法解析的组合类型: {scanner}")
 
     @classmethod
-    def check_compare_operator(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为比较运算符"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return (scanner.search("=") or scanner.search("!=") or scanner.search("<>") or scanner.search("<") or
-                scanner.search("<=") or scanner.search(">") or scanner.search(">=") or scanner.search("<>") or
-                scanner.search("<=>"))
-
-    @classmethod
-    def parse_compare_operator(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_compare_operator(cls, scanner_or_string: ScannerOrString,
                                sql_type: SQLType = SQLType.DEFAULT) -> node.ASTCompareOperator:
         """解析比较运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        compare_operator_hash = {
-            "=": node.EnumCompareOperator.EQUAL_TO,
-            "<": node.EnumCompareOperator.LESS_THAN,
-            "<=": node.EnumCompareOperator.LESS_THAN_OR_EQUAL,
-            ">": node.EnumCompareOperator.GREATER_THAN,
-            ">=": node.EnumCompareOperator.GREATER_THAN_OR_EQUAL,
-            "!=": node.EnumCompareOperator.NOT_EQUAL_TO,
-            "<>": node.EnumCompareOperator.NOT_EQUAL_TO,
-            "<=>": node.EnumCompareOperator.NOT_EQUAL_TO
-        }
-        compare_operator = compare_operator_hash.get(scanner.pop_as_source())
-        if compare_operator is not None:
-            return node.ASTCompareOperator(enum=compare_operator)
-        raise SqlParseError(f"无法解析的比较运算符: {scanner}")
-
-    @classmethod
-    def check_compute_operator(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为计算运算符"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for compute_operator in node.EnumComputeOperator:
-            if scanner.search(*compute_operator.value):
-                return True
-        return False
+        return cls._parse_compare_operator(scanner)
 
     @classmethod
-    def parse_compute_operator(cls, scanner_or_string: Union[TokenScanner, str],
+    def _parse_compare_operator(cls, scanner: TokenScanner) -> node.ASTCompareOperator:
+        compare_operator = static.COMPARE_OPERATOR_HASH.get(scanner.pop_as_source())
+        if compare_operator is None:
+            raise SqlParseError(f"无法解析的比较运算符: {scanner}")
+        return node.ASTCompareOperator(enum=compare_operator)
+
+    @classmethod
+    def parse_compute_operator(cls, scanner_or_string: ScannerOrString,
                                sql_type: SQLType = SQLType.DEFAULT) -> node.ASTComputeOperator:
         """解析计算运算符"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for compute_operator in node.EnumComputeOperator:
-            if scanner.search_and_move(*compute_operator.value):
-                return node.ASTComputeOperator(enum=compute_operator)
-        raise SqlParseError(f"无法解析的计算运算符: {scanner}")
-
-    @classmethod
-    def check_logical_operator(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为逻辑运算符"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.get_as_source() in {"AND", "OR", "NOT", "!"}
-
-    @classmethod
-    def parse_logical_operator(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTLogicalOperator:
-        """解析逻辑运算符"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("AND"):
-            return node.ASTLogicalOperator(enum=node.EnumLogicalOperator.AND)
-        if scanner.search_and_move("OR"):
-            return node.ASTLogicalOperator(enum=node.EnumLogicalOperator.OR)
-        if scanner.search_and_move("NOT"):
-            return node.ASTLogicalOperator(enum=node.EnumLogicalOperator.NOT)
-        if scanner.search_and_move("!"):
-            if sql_type not in {SQLType.HIVE, SQLType.MYSQL}:
-                raise UnSupportSqlTypeError(f"当前 SQL 类型不支持 ! 运算符: sql_type={sql_type}")
-            return node.ASTLogicalOperator(enum=node.EnumLogicalOperator.NOT)
-        for logical_operator in node.EnumLogicalOperator:
-            if scanner.search_and_move(*logical_operator.value):
-                return node.ASTLogicalOperator(enum=logical_operator)
-        raise SqlParseError(f"无法解析的逻辑运算符: {scanner}")
+        return cls._parse_compute_operator(scanner)
+
+    @classmethod
+    def _parse_compute_operator(cls, scanner: TokenScanner) -> node.ASTComputeOperator:
+        compute_operator = static.COMPUTE_OPERATOR_HASH.get(scanner.pop_as_source())
+        if compute_operator is None:
+            raise SqlParseError(f"无法解析的计算运算符: {scanner}")
+        return node.ASTComputeOperator(enum=compute_operator)
 
     @classmethod
-    def parse_cast_data_type(cls, scanner_or_string: Union[TokenScanner, str],
-                             sql_type: SQLType = SQLType.DEFAULT) -> node.EnumCastDataType:
+    def parse_cast_data_type(cls, scanner_or_string: ScannerOrString,
+                             sql_type: SQLType = SQLType.DEFAULT) -> static.EnumCastDataType:
         """解析 CAST 函数表达式中的类型"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        for cast_type in node.EnumCastDataType:
+        return cls._parse_cast_data_type(scanner)
+
+    @classmethod
+    def _parse_cast_data_type(cls, scanner: TokenScanner) -> static.EnumCastDataType:
+        for cast_type in static.EnumCastDataType:
             if scanner.search_and_move(cast_type.value):
                 return cast_type
         raise SqlParseError(f"无法解析的 CAST 函数表达式中的类型: {scanner}")
 
     # ------------------------------ 基础节点的解析方法 ------------------------------
 
     @classmethod
-    def check_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                     sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """是否可能为列名表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return ((scanner.search(AMTMark.NAME, ".", AMTMark.NAME)
-                 and not scanner.search(AMTMark.NAME, ".", AMTMark.NAME, AMTMark.PARENTHESIS))
-                or (scanner.search(AMTMark.NAME)
-                    and not scanner.search(AMTMark.NAME, ".")
-                    and not scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS)))
-
-    @classmethod
-    def parse_column_name_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                     unary_operator: Optional[Tuple[node.ASTComputeOperator]],
-                                     sql_type: SQLType = SQLType.DEFAULT) -> node.ASTColumnName:
+    def parse_column_name_expression(cls, scanner_or_string: ScannerOrString,
+                                     sql_type: SQLType = SQLType.DEFAULT) -> node.ASTColumnNameExpression:
         """解析列名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if (scanner.search(AMTMark.NAME, ".", AMTMark.NAME) and
-                not scanner.search(AMTMark.NAME, ".", AMTMark.NAME, AMTMark.PARENTHESIS)):
-            table_name = scanner.pop_as_source()
-            scanner.match(".")
+        return cls._parse_column_name_expression(scanner)
+
+    @classmethod
+    def _parse_column_name_expression(cls, scanner: TokenScanner) -> node.ASTColumnNameExpression:
+        if not scanner.search_one_type_mark(AMTMark.NAME):
+            raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+        first_name = scanner.pop_as_source()
+        if scanner.search_and_move_one_type_str("."):  # table.name 的形式
+            if not scanner.search_one_type_mark(AMTMark.NAME):
+                raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+            table_name = first_name
             column_name = scanner.pop_as_source()
-            return node.ASTColumnName(
-                unary_operator=unary_operator,
-                table_name=unify_name(table_name),
-                column_name=unify_name(column_name)
-            )
-        if (scanner.search(AMTMark.NAME)
-                and not scanner.search(AMTMark.NAME, ".")
-                and not scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS)):
-            return node.ASTColumnName(
-                unary_operator=unary_operator,
-                column_name=unify_name(scanner.pop_as_source())
-            )
-        raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+        else:
+            table_name = None
+            column_name = first_name
+        return node.ASTColumnNameExpression(
+            table_name=cls._unify_name(table_name),
+            column_name=cls._unify_name(column_name)
+        )
 
     @classmethod
-    def parse_column_name_expression_maybe_with_array_index(
-            cls,
-            scanner_or_string: Union[TokenScanner, str],
-            unary_operator: Optional[Tuple[node.ASTComputeOperator]],
-            sql_type: SQLType = SQLType.DEFAULT
-    ) -> Union[node.ASTColumnName, node.ASTArrayIndexExpression]:
-        """解析函数表达式，并解析函数表达式后可能包含的数组下标"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        column_name_expression = cls.parse_column_name_expression(scanner, unary_operator, sql_type=sql_type)
-        if not scanner.search(AMTMark.ARRAY_INDEX):
-            return column_name_expression  # 如果没有数组下标则直接返回
-        # 解析数组下标
-        children_scanner = scanner.pop_as_children_scanner()
-        idx = cls.parse_polynomial_expression(children_scanner, sql_type=sql_type)
-        children_scanner.close()
-        return node.ASTArrayIndexExpression(
-            unary_operator=unary_operator,
-            array=column_name_expression,
-            idx=idx
+    def _parse_column_name_expression_with_table(cls, scanner: TokenScanner) -> node.ASTColumnNameExpression:
+        """解析已确定包含表名的列名表达式"""
+        table_name = scanner.pop_as_source()
+        scanner.match(".")
+        column_name = scanner.pop_as_source()
+        return node.ASTColumnNameExpression(
+            table_name=cls._unify_name(table_name),
+            column_name=cls._unify_name(column_name)
+        )
+
+    @classmethod
+    def _parse_column_name_expression_without_table(cls, scanner: TokenScanner) -> node.ASTColumnNameExpression:
+        """解析已确定不包含表名的列名表达式"""
+        column_name = scanner.pop_as_source()
+        return node.ASTColumnNameExpression(
+            column_name=cls._unify_name(column_name)
         )
 
     @classmethod
-    def parse_table_name_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                    sql_type: SQLType = SQLType.DEFAULT) -> node.ASTTableName:
+    def parse_table_name_expression(cls, scanner_or_string: ScannerOrString,
+                                    sql_type: SQLType = SQLType.DEFAULT) -> node.ASTTableNameExpression:
         """解析表名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search(AMTMark.NAME, ".", AMTMark.NAME):
-            schema_name = scanner.pop_as_source()
-            scanner.pop()
-            table_name = scanner.pop_as_source()
-            return node.ASTTableName(schema_name=unify_name(schema_name), table_name=unify_name(table_name))
-        if scanner.search(AMTMark.NAME):
-            name_source = scanner.pop_as_source()
-            if name_source.count(".") == 1:
-                schema_name, table_name = name_source.strip("`").split(".")
-            else:
-                schema_name, table_name = None, name_source
-            return node.ASTTableName(schema_name=unify_name(schema_name), table_name=unify_name(table_name))
-        raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+        return cls._parse_table_name_expression(scanner)
+
+    @classmethod
+    def _parse_table_name_expression(cls, scanner: TokenScanner) -> node.ASTTableNameExpression:
+        node_0 = scanner.pop()
+        if not node_0.has_mark(AMTMark.NAME):
+            raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+
+        if scanner.search_and_move_one_type_str("."):
+            # 解析包含 schema 的表名
+            node_2 = scanner.pop()
+            if not node_0.has_mark(AMTMark.NAME):
+                raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+            return node.ASTTableNameExpression(
+                schema_name=cls._unify_name(node_0.source),
+                table_name=cls._unify_name(node_2.source)
+            )
+
+        # 解析没有 schema 或 `schema.table` 格式的表名
+        name_source = node_0.source
+        if name_source.count(".") == 1:
+            schema_name, table_name = name_source.strip("`").split(".")
+        else:
+            schema_name, table_name = None, name_source
+        return node.ASTTableNameExpression(
+            schema_name=cls._unify_name(schema_name),
+            table_name=cls._unify_name(table_name)
+        )
 
     @classmethod
-    def parse_function_name_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_function_name_expression(cls, scanner_or_string: ScannerOrString,
                                        sql_type: SQLType = SQLType.DEFAULT
-                                       ) -> node.ASTFunctionName:
+                                       ) -> node.ASTFunctionNameExpression:
         """解析函数名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_function_name_expression(scanner)
+
+    @classmethod
+    def _parse_function_name_expression(cls, scanner: TokenScanner) -> node.ASTFunctionNameExpression:
         if scanner.search(AMTMark.NAME, ".", AMTMark.NAME):
             schema_name = scanner.pop_as_source()
-            scanner.pop()
+            scanner.move()
             table_name = scanner.pop_as_source()
-            return node.ASTFunctionName(schema_name=unify_name(schema_name),
-                                        function_name=unify_name(table_name))
-        if scanner.search(AMTMark.NAME):
+            return node.ASTFunctionNameExpression(
+                schema_name=cls._unify_name(schema_name),
+                function_name=cls._unify_name(table_name)
+            )
+        if scanner.search_one_type_mark(AMTMark.NAME):
             name_source = scanner.pop_as_source()
             if name_source.count(".") == 1:
                 schema_name, table_name = name_source.strip("`").split(".")
             else:
                 schema_name, table_name = None, name_source
-            return node.ASTFunctionName(schema_name=unify_name(schema_name),
-                                        function_name=unify_name(table_name))
+            return node.ASTFunctionNameExpression(
+                schema_name=cls._unify_name(schema_name),
+                function_name=cls._unify_name(table_name)
+            )
         raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
     @classmethod
-    def check_literal_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                 sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search(AMTMark.LITERAL) or scanner.search("-")
-
-    @classmethod
-    def parse_literal_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                 unary_operator: Optional[Tuple[node.ASTComputeOperator]],
+    def parse_literal_expression(cls, scanner_or_string: ScannerOrString,
                                  sql_type: SQLType = SQLType.DEFAULT) -> node.ASTLiteralExpression:
         """解析字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return node.ASTLiteralExpression(unary_operator=unary_operator, value=scanner.pop_as_source())
+        return cls._parse_literal_expression(scanner)
 
     @classmethod
-    def parse_window_row_item(cls, scanner_or_string: Union[TokenScanner, str],
+    def _parse_literal_expression(cls, scanner: TokenScanner) -> node.ASTLiteralExpression:
+        return node.ASTLiteralExpression(value=scanner.pop_as_source())
+
+    @classmethod
+    def parse_window_row_item(cls, scanner_or_string: ScannerOrString,
                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWindowRowItem:
         """解析窗口函数行限制中的行"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("CURRENT", "ROW"):
-            return node.ASTWindowRowItem(row_type=node.EnumWindowRowType.CURRENT_ROW)
-        if scanner.search_and_move("UNBOUNDED"):
-            if scanner.search_and_move("PRECEDING"):
-                return node.ASTWindowRowItem(row_type=node.EnumWindowRowType.PRECEDING, is_unbounded=True)
-            if scanner.search_and_move("FOLLOWING"):
-                return node.ASTWindowRowItem(row_type=node.EnumWindowRowType.FOLLOWING, is_unbounded=True)
+        return cls._parse_window_row_item(scanner)
+
+    @classmethod
+    def _parse_window_row_item(cls, scanner: TokenScanner) -> node.ASTWindowRowItem:
+        if scanner.search_and_move_two_type_str_use_upper("CURRENT", "ROW"):
+            return node.ASTWindowRowItem(row_type=static.EnumWindowRowType.CURRENT_ROW)
+        if scanner.search_and_move_one_type_str_use_upper("UNBOUNDED"):
+            if scanner.search_and_move_one_type_str_use_upper("PRECEDING"):
+                return node.ASTWindowRowItem(row_type=static.EnumWindowRowType.PRECEDING, is_unbounded=True)
+            if scanner.search_and_move_one_type_str_use_upper("FOLLOWING"):
+                return node.ASTWindowRowItem(row_type=static.EnumWindowRowType.FOLLOWING, is_unbounded=True)
             raise SqlParseError(f"无法解析的窗口函数限制行: {scanner}")
         row_num = int(scanner.pop_as_source())
-        if scanner.search_and_move("PRECEDING"):
-            return node.ASTWindowRowItem(row_type=node.EnumWindowRowType.PRECEDING, row_num=row_num)
-        if scanner.search_and_move("FOLLOWING"):
-            return node.ASTWindowRowItem(row_type=node.EnumWindowRowType.FOLLOWING, row_num=row_num)
+        if scanner.search_and_move_one_type_str_use_upper("PRECEDING"):
+            return node.ASTWindowRowItem(row_type=static.EnumWindowRowType.PRECEDING, row_num=row_num)
+        if scanner.search_and_move_one_type_str_use_upper("FOLLOWING"):
+            return node.ASTWindowRowItem(row_type=static.EnumWindowRowType.FOLLOWING, row_num=row_num)
         raise SqlParseError(f"无法解析的窗口函数限制行: {scanner}")
 
     @classmethod
-    def parse_window_row(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_window_row(cls, scanner_or_string: ScannerOrString,
                          sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWindowRow:
         """解析窗口语句限制行的表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_window_row(scanner)
+
+    @classmethod
+    def _parse_window_row(cls, scanner: TokenScanner) -> node.ASTWindowRow:
         scanner.match("ROWS", "BETWEEN")
-        from_row = cls.parse_window_row_item(scanner, sql_type=sql_type)
+        from_row = cls._parse_window_row_item(scanner)
         scanner.match("AND")
-        to_row = cls.parse_window_row_item(scanner, sql_type=sql_type)
+        to_row = cls._parse_window_row_item(scanner)
         return node.ASTWindowRow(from_row=from_row, to_row=to_row)
 
     @classmethod
-    def check_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                  sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为通配符表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("*") or scanner.search(AMTMark.NAME, ".", "*")
-
-    @classmethod
-    def parse_wildcard_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                  unary_operator: Optional[Tuple[node.ASTComputeOperator]],
+    def parse_wildcard_expression(cls, scanner_or_string: ScannerOrString,
                                   sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWildcardExpression:
         """解析通配符表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("*"):
+        return cls._parse_wildcard_expression(scanner)
+
+    @classmethod
+    def _parse_wildcard_expression(cls, scanner: TokenScanner) -> node.ASTWildcardExpression:
+        if scanner.search_and_move_one_type_str("*"):
             return node.ASTWildcardExpression()
         if scanner.search(AMTMark.NAME, ".", "*"):
             schema_name = scanner.pop_as_source()
-            scanner.pop()
-            scanner.pop()
-            return node.ASTWildcardExpression(unary_operator=unary_operator, table_name=schema_name)
+            scanner.move(2)
+            return node.ASTWildcardExpression(table_name=schema_name)
         raise SqlParseError("无法解析为通配符表达式")
 
     @classmethod
-    def check_alias_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为别名表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("AS") or scanner.search(AMTMark.NAME)
+    def _parse_wildcard_expression_with_table(cls, scanner: TokenScanner) -> node.ASTWildcardExpression:
+        """直接解析为包含 schema 的通配符格式"""
+        schema_name = scanner.pop_as_source()
+        scanner.move(2)
+        return node.ASTWildcardExpression(table_name=schema_name)
 
     @classmethod
-    def _get_name(cls, scanner: TokenScanner) -> str:
-        """获取名称或别名：如果抽象词法树（AMT）没有 NAME 标记，则抛出异常"""
-        if not scanner.search(AMTMark.NAME):
-            raise SqlParseError(f"无法解析为名称: {scanner}")
-        return unify_name(scanner.pop_as_source())
+    def _parse_wildcard_expression_without_table(cls, scanner: TokenScanner) -> node.ASTWildcardExpression:
+        """直接解析为包含 schema 的通配符格式"""
+        scanner.move()
+        return node.ASTWildcardExpression()
 
     @classmethod
-    def parse_alias_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTAlisaExpression:
-        """解析别名表达式"""
+    def parse_alias_expression(cls, scanner_or_string: ScannerOrString,
+                               sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTAlisaExpression]:
+        """解析别名表达式：如果当前位置是别名表达式则返回别名表达式节点，否则返回 None"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.search_and_move("AS")
-        return node.ASTAlisaExpression(name=cls._get_name(scanner))
+        return cls._parse_alias_expression(scanner)
+
+    @classmethod
+    def _parse_alias_expression(cls, scanner: TokenScanner) -> Optional[node.ASTAlisaExpression]:
+        if scanner.search_and_move_one_type_str_use_upper("AS"):
+            return node.ASTAlisaExpression(name=cls._get_alias_name(scanner))
+        if scanner.search_one_type_mark(AMTMark.NAME):
+            return node.ASTAlisaExpression(name=cls._unify_name(scanner.pop_as_source()))
+        return None
 
     @classmethod
-    def parse_multi_alias_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_multi_alias_expression(cls, scanner_or_string: ScannerOrString,
                                      sql_type: SQLType = SQLType.DEFAULT) -> node.ASTMultiAlisaExpression:
         """解析多个别名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_multi_alias_expression(scanner)
+
+    @classmethod
+    def _parse_multi_alias_expression(cls, scanner: TokenScanner) -> node.ASTMultiAlisaExpression:
         scanner.match("AS")
-        names = [cls._get_name(scanner)]
-        while scanner.search_and_move(","):
-            names.append(cls._get_name(scanner))
+        names = [cls._get_alias_name(scanner)]
+        while scanner.search_and_move_one_type_str(","):
+            names.append(cls._get_alias_name(scanner))
         return node.ASTMultiAlisaExpression(names=tuple(names))
 
     # ------------------------------ SELECT 语句节点的解析方法 ------------------------------
 
     @classmethod
-    def check_function_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                  sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """是否可能为函数表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return (scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS) or
-                scanner.search(AMTMark.NAME, ".", AMTMark.NAME, AMTMark.PARENTHESIS))
-
-    @classmethod
-    def parse_extract_function_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_extract_function_expression(cls, scanner_or_string: ScannerOrString,
                                           sql_type: SQLType = SQLType.DEFAULT
                                           ) -> node.ASTExtractFunctionExpression:
         """解析 EXTRACT 函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        extract_name = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-        scanner.match("FROM")
-        column_expression = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-        scanner.close()
-        return node.ASTExtractFunctionExpression(extract_name=extract_name, column_expression=column_expression)
+        return cls._parse_extract_function_expression(scanner, sql_type)
 
     @classmethod
-    def parse_cast_function_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def _parse_extract_function_expression(cls, scanner: TokenScanner, sql_type: SQLType
+                                           ) -> node.ASTExtractFunctionExpression:
+        inner_scanner = scanner.pop_as_children_scanner()
+        extract_name = cls._parse_compute_expression(inner_scanner, sql_type)
+        inner_scanner.match("FROM")
+        column_expression = cls._parse_compute_expression(inner_scanner, sql_type)
+        inner_scanner.close()
+        return node.ASTExtractFunctionExpression(
+            extract_name=extract_name,
+            column_expression=column_expression
+        )
+
+    @classmethod
+    def parse_cast_function_expression(cls, scanner_or_string: ScannerOrString,
                                        sql_type: SQLType = SQLType.DEFAULT
                                        ) -> node.ASTCastFunctionExpression:
         """解析 CAST 函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        column_expression = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-        scanner.match("AS")
-        signed = scanner.search_and_move("SIGNED")
-        cast_type = cls.parse_cast_data_type(scanner, sql_type=sql_type)
-        if scanner.search(AMTMark.PARENTHESIS):
-            parenthesis_scanner = scanner.pop_as_children_scanner()
+        return cls._parse_cast_function_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_cast_function_expression(cls, scanner: TokenScanner, sql_type: SQLType):
+        inner_scanner = scanner.pop_as_children_scanner()
+        column_expression = cls._parse_compute_expression(inner_scanner, sql_type)
+        inner_scanner.match("AS")
+        signed = inner_scanner.search_and_move_one_type_str_use_upper("SIGNED")
+        cast_type = cls._parse_cast_data_type(inner_scanner)
+        if inner_scanner.search_one_type_mark(AMTMark.PARENTHESIS):
+            parenthesis_scanner = inner_scanner.pop_as_children_scanner()
             cast_params: Optional[List[int] | Tuple[int, ...]] = []
-            for param_scanner in parenthesis_scanner.split_by(","):
-                cast_params.append(int(param_scanner.pop_as_source()))
-                param_scanner.close()
+            if not parenthesis_scanner.is_finish:
+                cast_params.append(int(parenthesis_scanner.pop_as_source()))
+            while parenthesis_scanner.search_and_move_one_type_str(","):
+                cast_params.append(int(parenthesis_scanner.pop_as_source()))
             cast_params = tuple(cast_params)
         else:
             cast_params = None
-        scanner.close()
+        inner_scanner.close()
         cast_data_type = node.ASTCastDataType(signed=signed, type=cast_type, params=cast_params)
-        return node.ASTCastFunctionExpression(column_expression=column_expression, cast_type=cast_data_type)
+        return node.ASTCastFunctionExpression(
+            column_expression=column_expression,
+            cast_type=cast_data_type
+        )
 
     @classmethod
-    def parse_if_function_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_if_function_expression(cls, scanner_or_string: ScannerOrString,
                                      sql_type: SQLType = SQLType.DEFAULT
                                      ) -> node.ASTNormalFunctionExpression:
         """解析 IF 函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        function_params: List[node.AliasGeneralExpression] = []
-        first_param = True
-        for param_scanner in scanner.split_by(","):
-            if first_param is True:
-                function_params.append(cls.parse_general_expression(param_scanner, sql_type=sql_type))
-                first_param = False
-            else:
-                function_params.append(cls.parse_general_expression(param_scanner, sql_type=sql_type))
-            param_scanner.close()
-        return node.ASTNormalFunctionExpression(name=node.ASTFunctionName(function_name="IF"),
-                                                params=tuple(function_params))
+        return cls._parse_if_function_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_if_function_expression(cls, scanner: TokenScanner,
+                                      sql_type: SQLType) -> node.ASTNormalFunctionExpression:
+        inner_scanner = scanner.pop_as_children_scanner()
+        function_params: List[GeneralExpression] = []
+        if not inner_scanner.is_finish:
+            cls._parse_logical_or_level_expression(inner_scanner, sql_type=sql_type)
+        while inner_scanner.search_and_move_one_type_str(","):
+            function_params.append(cls._parse_logical_or_level_expression(inner_scanner, sql_type=sql_type))
+        inner_scanner.close()
+        return node.ASTNormalFunctionExpression(
+            name=node.ASTFunctionNameExpression(function_name="IF"),
+            params=tuple(function_params)
+        )
 
     @classmethod
-    def parse_function_expression(cls, scanner_or_string: Union[TokenScanner, str], sql_type: SQLType = SQLType.DEFAULT
-                                  ) -> Union[node.ASTFunctionExpression]:
+    def parse_function_expression(cls, scanner_or_string: ScannerOrString, sql_type: SQLType = SQLType.DEFAULT
+                                  ) -> node.ASTFunctionExpressionBase:
         """解析函数表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        function_name = cls.parse_function_name_expression(scanner, sql_type=sql_type)
+        return cls._parse_function_expression(scanner, sql_type=sql_type)
 
-        if function_name.function_name.upper() == "CAST":
-            return cls.parse_cast_function_expression(scanner.pop_as_children_scanner(), sql_type=sql_type)
-        if function_name.function_name.upper() == "EXTRACT":
-            return cls.parse_extract_function_expression(scanner.pop_as_children_scanner(), sql_type=sql_type)
-        if function_name.function_name.upper() == "IF":
-            return cls.parse_if_function_expression(scanner.pop_as_children_scanner(), sql_type=sql_type)
+    @classmethod
+    def _parse_function_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTFunctionExpressionBase:
+        function_name_expression = cls._parse_function_name_expression(scanner)
+        function_name_upper = function_name_expression.function_name.upper()
+
+        if function_name_upper == "CAST":
+            return cls._parse_cast_function_expression(scanner, sql_type)
+        if function_name_upper == "EXTRACT":
+            return cls._parse_extract_function_expression(scanner, sql_type)
+        if function_name_upper == "IF":
+            return cls._parse_if_function_expression(scanner, sql_type)
 
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        if function_name.function_name.upper() == "SUBSTRING":
+        if function_name_upper == "SUBSTRING":
             # 将 MySQL 和 PostgreSQL 中的 "SUBSTRING(str1 FROM 3 FOR 2)" 格式化为 "SUBSTRING(str1, 3, 2)"
             parenthesis_scanner = TokenScanner([
-                element if not element.equals("FROM") and not element.equals("FOR") else AMTSingle(",")
+                element if not element.source_in_set_use_upper({"FROM", "FOR"}) else AMTSingle(",")
                 for element in parenthesis_scanner.elements])
 
         is_distinct = False
-        if (function_name.function_name.upper() in name_set.AGGREGATION_FUNCTION_NAME_SET
-                and parenthesis_scanner.search_and_move("DISTINCT")):
+        if (function_name_upper in name_set.AGGREGATION_FUNCTION_NAME_SET
+                and parenthesis_scanner.search_and_move_one_type_str_use_upper("DISTINCT")):
             is_distinct = True
 
-        function_params: List[node.AliasGeneralExpression] = []
-        for param_scanner in parenthesis_scanner.split_by(","):
-            function_params.append(cls.parse_general_expression(param_scanner, sql_type=sql_type))
-            if not param_scanner.is_finish:
-                raise SqlParseError(f"无法解析函数参数: {param_scanner}")
+        function_params: List[GeneralExpression] = []
+        if not parenthesis_scanner.is_finish:
+            function_params.append(cls._parse_logical_or_level_expression(parenthesis_scanner, sql_type))
+        while parenthesis_scanner.search_and_move_one_type_str(","):
+            function_params.append(cls._parse_logical_or_level_expression(parenthesis_scanner, sql_type))
 
         parenthesis_scanner.close()
 
-        if (function_name.schema_name is None
-                and function_name.function_name.upper() in name_set.AGGREGATION_FUNCTION_NAME_SET):
-            return node.ASTAggregationFunctionExpression(
-                name=function_name,
+        if (function_name_expression.schema_name is None
+                and function_name_upper in name_set.AGGREGATION_FUNCTION_NAME_SET):
+            return node.ASTAggregationFunction(
+                name=function_name_expression,
                 params=tuple(function_params),
                 is_distinct=is_distinct)
         return node.ASTNormalFunctionExpression(
-            name=function_name,
-            params=tuple(function_params))
+            name=function_name_expression,
+            params=tuple(function_params)
+        )
 
     @classmethod
-    def parse_function_expression_maybe_with_array_index(
-            cls,
-            scanner_or_string: Union[TokenScanner, str],
-            unary_operator: Optional[Tuple[node.ASTComputeOperator]],
-            sql_type: SQLType = SQLType.DEFAULT
-    ) -> Union[node.ASTFunctionExpression, node.ASTArrayIndexExpression]:
+    def parse_function_expression_and_index(cls, scanner_or_string: ScannerOrString,
+                                            sql_type: SQLType = SQLType.DEFAULT
+                                            ) -> Union[node.ASTFunctionExpressionBase, node.ASTIndexExpression]:
         """解析函数表达式，并解析函数表达式后可能包含的数组下标"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        array_expression = cls.parse_function_expression(scanner, sql_type=sql_type)
-        if not scanner.search(AMTMark.ARRAY_INDEX):
-            return array_expression  # 如果没有数组下标则直接返回
-        # 解析数组下标
-        children_scanner = scanner.pop_as_children_scanner()
-        idx = cls.parse_polynomial_expression(children_scanner, sql_type=sql_type)
-        children_scanner.close()
-        return node.ASTArrayIndexExpression(
-            unary_operator=unary_operator,
-            array=array_expression,
-            idx=idx
-        )
+        return cls._parse_function_expression_and_index(scanner, sql_type=sql_type)
 
     @classmethod
-    def _parse_in_parenthesis(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> node.ASTMonomialExpression:
-        """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if cls.check_sub_query_parenthesis(scanner, sql_type=sql_type):
-            return cls.parse_sub_query_expression(scanner, unary_operator=None, sql_type=sql_type)
-        return cls.parse_value_expression(scanner, sql_type=sql_type)
+    def _parse_function_expression_and_index(cls, scanner: TokenScanner, sql_type: SQLType
+                                             ) -> Union[node.ASTFunctionExpressionBase, node.ASTIndexExpression]:
+        before_expression = cls._parse_function_expression(scanner, sql_type=sql_type)
+        return cls._parse_array_index_expression(scanner, before_expression, sql_type)
 
     @classmethod
-    def check_window_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为窗口函数"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return (scanner.search(AMTMark.NAME, AMTMark.PARENTHESIS, "OVER", AMTMark.PARENTHESIS)
-                and scanner.get_as_source().upper() in name_set.WINDOW_FUNCTION_NAME_SET)
+    def _parse_in_parenthesis(cls, scanner: TokenScanner, sql_type: SQLType) -> NodeElementLevel:
+        """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
+        if scanner.get_as_children_scanner().search_one_type_set_use_upper({"SELECT", "WITH"}):
+            return cls._parse_sub_query_expression(scanner, sql_type=sql_type)
+        return cls._parse_sub_value_expression(scanner, sql_type=sql_type)
 
     @classmethod
-    def parse_window_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                unary_operator: Optional[Tuple[node.ASTComputeOperator]],
+    def parse_window_expression(cls, scanner_or_string: ScannerOrString,
                                 sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWindowExpression:
         """解析窗口函数"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        window_function = cls.parse_function_expression_maybe_with_array_index(scanner,
-                                                                               unary_operator=None,
-                                                                               sql_type=sql_type)
+        return cls._parse_window_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_window_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTWindowExpression:
+        # 解析函数（因为这个函数可能是 UDF 函数，所以不作限制）
+        window_function = cls._parse_function_expression_and_index(scanner, sql_type=sql_type)
         partition_by_columns = []
         order_by_columns = []
         row_expression = None
         scanner.match("OVER")
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        if parenthesis_scanner.search_and_move("PARTITION", "BY"):
-            partition_by_columns = [cls.parse_polynomial_expression(parenthesis_scanner,
-                                                                    maybe_window=False, sql_type=sql_type)]
-            while parenthesis_scanner.search_and_move(","):
-                partition_by_columns.append(cls.parse_polynomial_expression(parenthesis_scanner,
-                                                                            maybe_window=False, sql_type=sql_type))
-        if parenthesis_scanner.search_and_move("ORDER", "BY"):
-            order_by_columns = [cls._parse_order_by_item(parenthesis_scanner, sql_type=sql_type)]
-            while parenthesis_scanner.search_and_move(","):
-                order_by_columns.append(cls._parse_order_by_item(parenthesis_scanner, sql_type=sql_type))
-        if parenthesis_scanner.search("ROWS", "BETWEEN"):
-            row_expression = cls.parse_window_row(parenthesis_scanner, sql_type=sql_type)
+        if parenthesis_scanner.search_and_move_two_type_str_use_upper("PARTITION", "BY"):
+            partition_by_columns = [cls._parse_compute_expression(parenthesis_scanner, sql_type)]
+            while parenthesis_scanner.search_and_move_one_type_str(","):
+                partition_by_columns.append(cls._parse_compute_expression(parenthesis_scanner, sql_type))
+        if parenthesis_scanner.search_and_move_two_type_str_use_upper("ORDER", "BY"):
+            order_by_columns = [cls._parse_order_by_column(parenthesis_scanner, sql_type)]
+            while parenthesis_scanner.search_and_move_one_type_str(","):
+                order_by_columns.append(cls._parse_order_by_column(parenthesis_scanner, sql_type))
+        if parenthesis_scanner.search_two_type_str_use_upper("ROWS", "BETWEEN"):
+            row_expression = cls._parse_window_row(parenthesis_scanner)
         parenthesis_scanner.close()
-        return node.ASTWindowExpression(unary_operator=unary_operator,
-                                        window_function=window_function,
-                                        partition_by_columns=tuple(partition_by_columns),
-                                        order_by_columns=tuple(order_by_columns),
-                                        row_expression=row_expression)
-
-    @classmethod
-    def check_case_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为 CASE 表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("CASE")
+        return node.ASTWindowExpression(
+            window_function=window_function,
+            partition_by_columns=tuple(partition_by_columns),
+            order_by_columns=tuple(order_by_columns),
+            row_expression=row_expression
+        )
 
     @classmethod
-    def parse_case_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                              unary_operator: Optional[Tuple[node.ASTComputeOperator]],
+    def parse_case_expression(cls, scanner_or_string: ScannerOrString,
                               sql_type: SQLType = SQLType.DEFAULT
-                              ) -> Union[node.ASTCaseConditionExpression, node.ASTCaseValueExpression]:
+                              ) -> AliasCaseExpression:
         """解析 CASE 表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_case_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_case_expression(cls, scanner: TokenScanner, sql_type: SQLType):
         scanner.match("CASE")
-        if scanner.search("WHEN"):
+        if scanner.search_one_type_str_use_upper("WHEN"):
             # 第 1 种格式的 CASE 表达式
             cases = []
             else_value = None
-            while scanner.search_and_move("WHEN"):
-                when_expression = cls.parse_general_expression(scanner, sql_type=sql_type)
+            while scanner.search_and_move_one_type_str_use_upper("WHEN"):
+                when_expression = cls._parse_logical_or_level_expression(scanner, sql_type=sql_type)
                 scanner.match("THEN")
-                case_expression = cls.parse_general_expression(scanner, sql_type=sql_type)
+                case_expression = cls._parse_logical_or_level_expression(scanner, sql_type=sql_type)
                 cases.append(node.ASTCaseConditionItem(when=when_expression, then=case_expression))
-            if scanner.search_and_move("ELSE"):
-                else_value = cls.parse_general_expression(scanner)
+            if scanner.search_and_move_one_type_str_use_upper("ELSE"):
+                else_value = cls._parse_logical_or_level_expression(scanner, sql_type)
             scanner.match("END")
             return node.ASTCaseConditionExpression(
-                unary_operator=unary_operator,
                 cases=tuple(cases),
                 else_value=else_value
             )
 
         # 第 2 种格式的 CASE 表达式
-        case_value = cls.parse_general_expression(scanner, sql_type=sql_type)
+        case_value = cls._parse_logical_or_level_expression(scanner, sql_type=sql_type)
         cases = []
         else_value = None
-        while scanner.search_and_move("WHEN"):
-            when_expression = cls.parse_general_expression(scanner, sql_type=sql_type)
+        while scanner.search_and_move_one_type_str_use_upper("WHEN"):
+            when_expression = cls._parse_logical_or_level_expression(scanner, sql_type=sql_type)
             scanner.match("THEN")
-            case_expression = cls.parse_general_expression(scanner, sql_type=sql_type)
+            case_expression = cls._parse_logical_or_level_expression(scanner, sql_type=sql_type)
             cases.append(node.ASTCaseValueItem(when=when_expression, then=case_expression))
-        if scanner.search_and_move("ELSE"):
-            else_value = cls.parse_general_expression(scanner, sql_type=sql_type)
+        if scanner.search_and_move_one_type_str_use_upper("ELSE"):
+            else_value = cls._parse_logical_or_level_expression(scanner, sql_type=sql_type)
         scanner.match("END")
         return node.ASTCaseValueExpression(
-            unary_operator=unary_operator,
             case_value=case_value,
             cases=tuple(cases),
             else_value=else_value
         )
 
     @classmethod
-    def check_sub_query_parenthesis(cls, scanner_or_string: Union[TokenScanner, str],
-                                    sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为子查询的插入语
-
-        1. 在子查询中，也可以使用包含 WITH 子句的 SELECT 语句
-        """
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        parenthesis_scanner = scanner.get_as_children_scanner()
-        return parenthesis_scanner.search("SELECT") or parenthesis_scanner.search("WITH")
-
-    @classmethod
-    def parse_sub_query_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                   unary_operator: Optional[Tuple[node.ASTComputeOperator]],
+    def parse_sub_query_expression(cls, scanner_or_string: ScannerOrString,
                                    sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSubQueryExpression:
         """解析子查询表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_sub_query_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_sub_query_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTSubQueryExpression:
         parenthesis_scanner = scanner.pop_as_children_scanner()
         result = node.ASTSubQueryExpression(
-            unary_operator=unary_operator,
-            statement=cls.parse_select_statement(parenthesis_scanner, sql_type=sql_type)
+            statement=cls._parse_select_statement(parenthesis_scanner, None, sql_type=sql_type)
         )
         parenthesis_scanner.close()
         return result
 
     @classmethod
-    def parse_value_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSubValueExpression:
+    def parse_sub_value_expression(cls, scanner_or_string: ScannerOrString,
+                                   sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSubValueExpression:
         """解析值表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_sub_value_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_sub_value_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTSubValueExpression:
         values = []
         for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            values.append(cls.parse_polynomial_expression(value_scanner, sql_type=sql_type))
+            values.append(cls._parse_compute_expression(value_scanner, sql_type))
             value_scanner.close()
         return node.ASTSubValueExpression(values=tuple(values))
 
     @classmethod
-    def parse_parenthesis_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                     unary_operator: Optional[Tuple[node.ASTComputeOperator]],
-                                     sql_type: SQLType = SQLType.DEFAULT) -> node.ASTParenthesisExpression:
-        """解析插入语表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if cls.check_sub_query_parenthesis(scanner, sql_type=sql_type):  # 子查询的情况
-            return cls.parse_sub_query_expression(scanner, unary_operator=unary_operator, sql_type=sql_type)
+    def _parse_general_parenthesis(cls, scanner: TokenScanner, sql_type: SQLType) -> GeneralExpression:
+        """解析一般表达式中的插入语"""
+        # 处理插入语中是子查询的情况
+        if scanner.get_as_children_scanner().search_one_type_set_use_upper({"SELECT", "WITH"}):
+            return cls._parse_sub_query_expression(scanner, sql_type=sql_type)
+        # 处理插入语中是一般表达式的情况：如果有嵌套的插入语，那么会自动压缩为一层
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        result = node.ASTSubGeneralExpression(
-            unary_operator=unary_operator,
-            expression=cls.parse_general_expression(parenthesis_scanner, sql_type=sql_type)
-        )
+        result = cls._parse_logical_or_level_expression(parenthesis_scanner, sql_type=sql_type)
         parenthesis_scanner.close()
         return result
 
     @classmethod
-    def parse_monomial_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                  maybe_window: bool,
-                                  sql_type: SQLType = SQLType.DEFAULT) -> node.ASTMonomialExpression:
+    def _parse_array_index_expression(cls, scanner: TokenScanner, before_expression: GeneralExpression,
+                                      sql_type: SQLType) -> GeneralExpression:
+        """解析下标表达式
+
+        Parameters
+        ----------
+        scanner : TokenScanner
+        before_expression : NodeLogicalOrLevel
+            下标表达式之前的表达式
+        sql_type : SQLType
+        """
+        if not scanner.search_one_type_mark(AMTMark.ARRAY_INDEX):
+            return before_expression  # 如果没有下标则直接返回
+        # 解析数组下标
+        children_scanner = scanner.pop_as_children_scanner()
+        idx = cls._parse_compute_expression(children_scanner, sql_type)
+        children_scanner.close()
+        return node.ASTIndexExpression(
+            array=before_expression,
+            idx=idx
+        )
+
+    @classmethod
+    def parse_element_level_expression(cls, scanner_or_string: ScannerOrString,
+                                       sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
         # pylint: disable=R0911
-        """解析单项表达式"""
+        """解析元素表达式层级"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_element_level_expression(scanner, sql_type=sql_type)
 
-        # 解析一元运算符（允许连续使用多个一元运算符）
-        unary_operator = []
-        while scanner.search("-") or scanner.search("+"):
-            unary_operator.append(cls.parse_compute_operator(scanner))
-
-        if cls.check_case_expression(scanner, sql_type=sql_type):
-            return cls.parse_case_expression(scanner, unary_operator=tuple(unary_operator), sql_type=sql_type)
-        if maybe_window is True and cls.check_window_expression(scanner, sql_type=sql_type):
-            return cls.parse_window_expression(scanner, unary_operator=tuple(unary_operator), sql_type=sql_type)
-        if cls.check_function_expression(scanner, sql_type=sql_type):
-            return cls.parse_function_expression_maybe_with_array_index(scanner,
-                                                                        unary_operator=tuple(unary_operator),
-                                                                        sql_type=sql_type)
-        if cls.check_literal_expression(scanner, sql_type=sql_type):
-            return cls.parse_literal_expression(scanner, unary_operator=tuple(unary_operator), sql_type=sql_type)
-        if cls.check_column_name_expression(scanner, sql_type=sql_type):
-            return cls.parse_column_name_expression_maybe_with_array_index(scanner,
-                                                                           unary_operator=tuple(unary_operator),
-                                                                           sql_type=sql_type)
-        if cls.check_wildcard_expression(scanner, sql_type=sql_type):
-            return cls.parse_wildcard_expression(scanner, unary_operator=tuple(unary_operator), sql_type=sql_type)
-        if scanner.search(AMTMark.PARENTHESIS):
-            return cls.parse_parenthesis_expression(scanner, unary_operator=tuple(unary_operator), sql_type=sql_type)
-        raise SqlParseError(f"未知的一般表达式元素: {scanner}")
-
-    @classmethod
-    def parse_polynomial_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                    sql_type: SQLType = SQLType.DEFAULT,
-                                    maybe_window: bool = True) -> node.AliasPolynomialExpression:
-        """解析多项表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        elements = [cls.parse_monomial_expression(scanner, maybe_window, sql_type=sql_type)]
-        while cls.check_compute_operator(scanner, sql_type=sql_type):
-            elements.append(cls.parse_compute_operator(scanner, sql_type=sql_type))
-            elements.append(cls.parse_monomial_expression(scanner, maybe_window))
-        if len(elements) == 1:
-            # 如果只有 1 个元素，则返回单项式表达式
-            return elements[0]
-        # 如果超过 1 个原则，则返回多项式表达式
-        return node.ASTPolynomialExpression(elements=tuple(elements))
-
-    @classmethod
-    def parse_condition_expression_item(cls, scanner_or_string: Union[TokenScanner, str],
-                                        before_value: node.AliasPolynomialExpression,
-                                        is_not: bool,
-                                        sql_type: SQLType = SQLType.DEFAULT) -> node.AliasConditionExpression:
+    @classmethod
+    def _parse_element_level_expression(cls, scanner: TokenScanner, sql_type: SQLType
+                                        ) -> GeneralExpression:
         # pylint: disable=R0911
-        """解析条件表达式中的一个元素
-        
-        TODO 待根据运算优先级，生成嵌套的二元运算逻辑后，这个逻辑需要被移除
-        """
+        # pylint: disable=R0912
+        """已进行性能优化，使用专有解析逻辑而非通用解析逻辑"""
+        node_0 = scanner.get_offset()
+        if node_0.has_mark(AMTMark.LITERAL):
+            return cls._parse_literal_expression(scanner)
+        if node_0.has_mark(AMTMark.PARENTHESIS):  # 处理包含插入语的情况
+            return cls._parse_general_parenthesis(scanner, sql_type=sql_type)
+        if node_0.source_equal_use_upper("CASE"):
+            return cls._parse_case_expression(scanner, sql_type=sql_type)
+        if node_0.source_equal("*"):
+            return cls._parse_wildcard_expression_without_table(scanner)
+
+        node_1 = scanner.get_offset_or_null(1)
+        if node_1 is not None and node_1.has_mark(AMTMark.PARENTHESIS):
+            node_2 = scanner.get_offset_or_null(2)
+            if node_2 is None or not node_2.source_equal_use_upper("OVER"):
+                return cls._parse_function_expression_and_index(scanner, sql_type=sql_type)
+            return cls._parse_window_expression(scanner, sql_type=sql_type)
+        if node_1 is not None and node_1.source_equal("."):
+            node_2 = scanner.get_offset(2)
+            if node_2.has_mark(AMTMark.NAME):
+                node_3 = scanner.get_offset_or_null(3)
+                if node_3 is None or not node_3.has_mark(AMTMark.PARENTHESIS):
+                    column_name_expression = cls._parse_column_name_expression_with_table(scanner)
+                    return cls._parse_array_index_expression(scanner, column_name_expression, sql_type)
+                return cls._parse_function_expression_and_index(scanner, sql_type=sql_type)
+            if node_2.source_equal("*"):
+                return cls._parse_wildcard_expression_with_table(scanner)
+            raise SqlParseError(f"{node_1.source}. 之后不是名称或通配符")
+        column_name_expression = cls._parse_column_name_expression_without_table(scanner)
+        return cls._parse_array_index_expression(scanner, column_name_expression, sql_type)
+
+    @classmethod
+    def parse_unary_level_expression(cls, scanner_or_string: ScannerOrString,
+                                     sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析一元表达式层级"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_unary_level_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_unary_level_expression(cls, scanner: TokenScanner, sql_type: SQLType
+                                      ) -> GeneralExpression:
+        if scanner.search_one_type_set(static.get_unary_operator_set(sql_type)):
+            unary_operator = cls._parse_compute_operator(scanner)
+            return node.ASTUnaryExpression(
+                operator=unary_operator,
+                expression=cls._parse_unary_level_expression(scanner, sql_type)
+            )
+        return cls._parse_element_level_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def parse_compute_expression(cls, scanner_or_string: ScannerOrString,
+                                 sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析按位或层级表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("BETWEEN"):  # "... BETWEEN ... AND ..."
-            from_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            scanner.match("AND")
-            to_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            return node.ASTBoolBetweenExpression(is_not=is_not, before_value=before_value, from_value=from_value,
-                                                 to_value=to_value)
-        if scanner.search_and_move("IS"):  # ".... IS ...." 或 "... IS NOT ..."
-            is_not = is_not or scanner.search_and_move("NOT") or scanner.search_and_move("!")
-            after_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            return node.ASTBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-        if scanner.search_and_move("IN"):  # "... IN (1, 2, 3)" 或 "... IN (SELECT ... )"
-            after_value = cls._parse_in_parenthesis(scanner, sql_type=sql_type)
-            return node.ASTBoolInExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-        if scanner.search_and_move("LIKE"):
-            after_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            return node.ASTBoolLikeExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-        if scanner.search_and_move("RLIKE"):
-            after_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            return node.ASTBoolRlikeExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-        if scanner.search_and_move("REGEXP"):
-            after_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            return node.ASTBoolRegexpExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-        if cls.check_compare_operator(scanner, sql_type=sql_type):  # "... > ..."
-            compare_operator = cls.parse_compare_operator(scanner, sql_type=sql_type)
-            after_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            return node.ASTBoolCompareExpression(
-                is_not=is_not,
-                operator=compare_operator,
+        return cls._parse_compute_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_compute_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> GeneralExpression:
+        stack: List[Union[GeneralExpression, static.EnumComputeOperator]]
+        stack = [cls._parse_unary_level_expression(scanner, sql_type)]
+        while compute_operator := static.COMPUTE_OPERATOR_HASH.get(scanner.get_as_source_or_null()):
+            while len(stack) >= 3 and compute_operator.level >= stack[-2].level:
+                after_value: GeneralExpression = stack.pop()
+                last_compute_operator = stack.pop()
+                before_value: GeneralExpression = stack.pop()
+                stack.append(node.ASTComputeExpression(
+                    before_value=before_value,
+                    operator=node.ASTComputeOperator(enum=last_compute_operator),
+                    after_value=after_value
+                ))
+            scanner.move()
+            stack.append(compute_operator)
+            stack.append(cls._parse_unary_level_expression(scanner, sql_type))
+        while len(stack) >= 3:
+            after_value: GeneralExpression = stack.pop()
+            last_compute_operator = stack.pop()
+            before_value: GeneralExpression = stack.pop()
+            stack.append(node.ASTComputeExpression(
                 before_value=before_value,
+                operator=node.ASTComputeOperator(enum=last_compute_operator),
                 after_value=after_value
-            )
-        return before_value  # 如果无法构成条件表达式，则返回多项式表达式或单项式表达式
+            ))
+
+        return stack[0]
 
     @classmethod
-    def parse_condition_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                   sql_type: SQLType = SQLType.DEFAULT) -> node.AliasConditionExpression:
+    def parse_keyword_condition_level_expression(cls, scanner_or_string: ScannerOrString,
+                                                 sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
         # pylint: disable=R0911
-        """解析条件表达式
+        """解析关键字条件表达式（不包含前置 NOT，但包含中间的 NOT）
 
-        TODO 待根据运算优先级，生成嵌套的二元运算逻辑
+        Parameters
+        ----------
+        scanner_or_string : ScannerOrString
+            扫描器
+        sql_type : SQLType
+            SQL 类型
         """
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        is_not = scanner.search_and_move("NOT") or scanner.search_and_move("!")
-        if scanner.search_and_move("EXISTS"):
-            after_value = cls.parse_sub_query_expression(scanner, unary_operator=None, sql_type=sql_type)
-            return node.ASTBoolExistsExpression(is_not=is_not, after_value=after_value)
-        before_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-        is_not = is_not or scanner.search_and_move("NOT") or scanner.search_and_move("!")
-        # 解析第一个条件表达式
-        before_value = cls.parse_condition_expression_item(scanner, before_value, is_not, sql_type=sql_type)
-        # 如果后续还有更多的等号，则继续合并为二元表达式
-        while cls.check_compare_operator(scanner, sql_type=sql_type):
-            compare_operator = cls.parse_compare_operator(scanner, sql_type=sql_type)
-            after_value = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            before_value = node.ASTBoolCompareExpression(is_not=is_not, operator=compare_operator,
-                                                         before_value=before_value,
-                                                         after_value=after_value)
+        return cls._parse_keyword_condition_level_expression(scanner, None, sql_type=sql_type)
+
+    @classmethod
+    def _parse_keyword_condition_level_expression(cls, scanner: TokenScanner,
+                                                  before_value: Optional[NodeKeywordConditionLevel],
+                                                  sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析关键字条件表达式
+
+        Parameters
+        ----------
+        scanner
+        before_value : Optional[NodeKeywordConditionLevel], default = None
+            已经遍历的上一个关键字条件表达式，用于递归，在第一次时置为 None 即可
+        sql_type
+        """
+        # 首先尝试解析第一个关键字条件表达式
+        if before_value is None and scanner.search_and_move_one_type_str_use_upper("EXISTS"):
+            # 正在解析第一个关键字表达式，且开头的关键字表达式为 EXISTS 语句
+            value = cls._parse_sub_query_expression(scanner, sql_type=sql_type)
+            result_value = node.ASTExistsExpression(value=value)
+        else:
+            if before_value is None:
+                # 如果正在解析第一个关键字表达式，则解析按位或表达式或更低等级表达式作为关键字之前的部分
+                before_value = cls._parse_compute_expression(scanner, sql_type)
+
+            # 解析可能存在于关键字之间的 NOT
+            is_not = scanner.search_and_move_one_type_set_use_upper(static.get_not_operator_set(sql_type))
+
+            if scanner.is_finish:
+                return before_value  # 如果已经匹配结果，则直接返回
+
+            next_ch = scanner.get_as_source_or_null().upper()
+            if next_ch == "BETWEEN":
+                scanner.move()
+                from_value = cls._parse_compute_expression(scanner, sql_type)
+                scanner.match("AND")
+                to_value = cls._parse_compute_expression(scanner, sql_type)
+                result_value = node.ASTBetweenExpression(
+                    is_not=is_not,
+                    before_value=before_value,
+                    from_value=from_value,
+                    to_value=to_value
+                )
+            elif next_ch == "IS":
+                scanner.move()
+                is_not = is_not or scanner.search_and_move_one_type_str_use_upper("NOT")
+                after_value = cls._parse_compute_expression(scanner, sql_type)
+                result_value = node.ASTIsExpression(
+                    is_not=is_not,
+                    before_value=before_value,
+                    after_value=after_value
+                )
+            elif next_ch == "IN":
+                scanner.move()
+                after_value = cls._parse_in_parenthesis(scanner, sql_type=sql_type)
+                result_value = node.ASTInExpression(
+                    is_not=is_not,
+                    before_value=before_value,
+                    after_value=after_value
+                )
+            elif next_ch == "LIKE":
+                scanner.move()
+                after_value = cls._parse_compute_expression(scanner, sql_type)
+                result_value = node.ASTLikeExpression(
+                    is_not=is_not,
+                    before_value=before_value,
+                    after_value=after_value
+                )
+            elif next_ch == "RLIKE":
+                scanner.move()
+                after_value = cls._parse_compute_expression(scanner, sql_type)
+                result_value = node.ASTRlikeExpression(
+                    is_not=is_not,
+                    before_value=before_value,
+                    after_value=after_value
+                )
+            elif next_ch == "REGEXP":
+                scanner.move()
+                after_value = cls._parse_compute_expression(scanner, sql_type)
+                result_value = node.ASTRegexpExpression(
+                    is_not=is_not,
+                    before_value=before_value,
+                    after_value=after_value
+                )
+            else:
+                # 没有关键字表达式，直接返回按位或表达式或更低等级表达式
+                return before_value
+
+        # 如果后续是连续的关键字条件表达式的关键字，则将当前关键字表达式作为下一个关键字表达式的 before_value 继续解析
+        if scanner.get_as_source_or_null() in {"NOT", "BETWEEN", "IS", "IN", "LIKE", "RLIKE", "REGEXP"}:
+            return cls._parse_keyword_condition_level_expression(scanner, result_value, sql_type=sql_type)
+
+        # 如果后续不是关键字条件表达式的关键字，则直接返回当前的关键字条件表达式
+        return result_value
+
+    @classmethod
+    def parse_operator_condition_level_expression(cls, scanner_or_string: ScannerOrString,
+                                                  sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析运算符条件表达式"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_operator_condition_level_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_operator_condition_level_expression(cls, scanner: TokenScanner,
+                                                   sql_type: SQLType) -> GeneralExpression:
+        before_value = cls._parse_keyword_condition_level_expression(scanner, None, sql_type=sql_type)
+        while scanner.search_one_type_set(static.COMPARE_OPERATOR_SET):
+            compare_operator = cls._parse_compare_operator(scanner)
+            after_value = cls._parse_keyword_condition_level_expression(scanner, None, sql_type=sql_type)
+            before_value = node.ASTOperatorConditionExpression(
+                operator=compare_operator,
+                before_value=before_value,
+                after_value=after_value
+            )
         return before_value
 
     @classmethod
-    def parse_general_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                 sql_type: SQLType = SQLType.DEFAULT) -> node.AliasGeneralExpression:
-        """解析一般表达式"""
+    def parse_logical_not_level_expression(cls, scanner_or_string: ScannerOrString,
+                                           sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析逻辑否表达式层级"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        first_element = cls.parse_condition_expression(scanner, sql_type=sql_type)
-        if scanner.search("AND") or scanner.search("OR"):
-            elements: List[node.AliasGeneralExpressionElement] = [first_element]
-            while scanner.search("AND") or scanner.search("OR"):  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
-                elements.append(cls.parse_logical_operator(scanner, sql_type=sql_type))
-                elements.append(cls.parse_condition_expression(scanner, sql_type=sql_type))
-            return node.ASTGeneralExpression(elements=tuple(elements))
-        return first_element
+        return cls._parse_logical_not_level_expression(scanner, sql_type=sql_type)
+
+    @classmethod
+    def _parse_logical_not_level_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> GeneralExpression:
+        if scanner.search_and_move_one_type_set_use_upper(static.get_not_operator_set(sql_type)):
+            return node.ASTLogicalNotExpression(
+                expression=cls._parse_logical_not_level_expression(scanner, sql_type=sql_type)
+            )
+        return cls._parse_operator_condition_level_expression(scanner, sql_type=sql_type)
 
     @classmethod
-    def check_join_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为关联表达式"""
+    def parse_logical_and_level_expression(cls, scanner_or_string: ScannerOrString,
+                                           sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析逻辑与表达式层级"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("ON") or scanner.search("USING")
+        return cls._parse_logical_and_level_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_logical_and_level_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> GeneralExpression:
+        before_value = cls._parse_logical_not_level_expression(scanner, sql_type=sql_type)
+        while scanner.search_and_move_one_type_set_use_upper({"AND", "&&"}):
+            after_value = cls._parse_logical_not_level_expression(scanner, sql_type=sql_type)
+            before_value = node.ASTLogicalAndExpression(
+                before_value=before_value,
+                after_value=after_value
+            )
+        return before_value
 
     @classmethod
-    def parse_join_on_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_logical_xor_level_expression(cls, scanner_or_string: ScannerOrString,
+                                           sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析逻辑异或表达式层级"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_logical_xor_level_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_logical_xor_level_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> GeneralExpression:
+        before_value = cls._parse_logical_and_level_expression(scanner, sql_type=sql_type)
+        while scanner.search_and_move_one_type_str_use_upper("XOR"):
+            after_value = cls._parse_logical_and_level_expression(scanner, sql_type=sql_type)
+            before_value = node.ASTLogicalXorExpression(
+                before_value=before_value,
+                after_value=after_value
+            )
+        return before_value
+
+    @classmethod
+    def parse_logical_or_level_expression(cls, scanner_or_string: ScannerOrString,
+                                          sql_type: SQLType = SQLType.DEFAULT) -> GeneralExpression:
+        """解析逻辑或表达式层级"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_logical_or_level_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_logical_or_level_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> GeneralExpression:
+        before_value = cls._parse_logical_xor_level_expression(scanner, sql_type=sql_type)
+        while scanner.search_and_move_one_type_set_use_upper({"OR", "||"}):
+            after_value = cls._parse_logical_xor_level_expression(scanner, sql_type=sql_type)
+            before_value = node.ASTLogicalOrExpression(
+                before_value=before_value,
+                after_value=after_value
+            )
+        return before_value
+
+    @classmethod
+    def parse_join_on_expression(cls, scanner_or_string: ScannerOrString,
                                  sql_type: SQLType = SQLType.DEFAULT) -> node.ASTJoinOnExpression:
         """解析 ON 关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if not scanner.search_and_move("ON"):
-            raise SqlParseError(f"无法解析为 ON 关联表达式: {scanner}")
-        return node.ASTJoinOnExpression(condition=cls.parse_general_expression(scanner, sql_type=sql_type))
+        return cls._parse_join_on_expression(scanner, sql_type)
 
     @classmethod
-    def parse_join_using_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def _parse_join_on_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTJoinOnExpression:
+        scanner.match("ON")
+        return node.ASTJoinOnExpression(condition=cls._parse_logical_or_level_expression(scanner, sql_type=sql_type))
+
+    @classmethod
+    def parse_join_using_expression(cls, scanner_or_string: ScannerOrString,
                                     sql_type: SQLType = SQLType.DEFAULT) -> node.ASTJoinUsingExpression:
         """解析 USING 关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if not scanner.search("USING"):
-            raise SqlParseError(f"无法解析为 USING 关联表达式: {scanner}")
-        return node.ASTJoinUsingExpression(using_function=cls.parse_function_expression(scanner, sql_type=sql_type))
+        return cls._parse_join_using_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_join_using_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTJoinUsingExpression:
+        return node.ASTJoinUsingExpression(using_function=cls._parse_function_expression(scanner, sql_type=sql_type))
 
     @classmethod
-    def parse_join_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> node.ASTJoinExpression:
+    def parse_join_expression(cls, scanner_or_string: ScannerOrString,
+                              sql_type: SQLType = SQLType.DEFAULT) -> AliasJoinExpression:
         """解析关联表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search("ON"):
-            return cls.parse_join_on_expression(scanner, sql_type=sql_type)
-        if scanner.search("USING"):
-            return cls.parse_join_using_expression(scanner, sql_type=sql_type)
+        return cls._parse_join_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_join_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> AliasJoinExpression:
+        if scanner.search_one_type_str_use_upper("ON"):
+            return cls._parse_join_on_expression(scanner, sql_type)
+        if scanner.search_one_type_str_use_upper("USING"):
+            return cls._parse_join_using_expression(scanner, sql_type)
         raise SqlParseError(f"无法解析为关联表达式: {scanner}")
 
     @classmethod
-    def parse_type_table_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                    sql_type: SQLType = SQLType.DEFAULT) -> node.AliasTableExpression:
+    def parse_table_expression(cls, scanner_or_string: ScannerOrString,
+                               sql_type: SQLType = SQLType.DEFAULT) -> AliasTableExpression:
         """解析表表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if cls.check_sub_query_parenthesis(scanner, sql_type=sql_type):  # 子查询
-            return cls.parse_sub_query_expression(scanner, unary_operator=None, sql_type=sql_type)
-        if scanner.search(AMTMark.PARENTHESIS):  # 额外的插入语（因为只有一个元素，所以直接递归解析即可）
-            return cls.parse_type_table_expression(scanner.pop_as_children_scanner(), sql_type=sql_type)
-        return cls.parse_table_name_expression(scanner, sql_type=sql_type)  # 表名
+        return cls._parse_table_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_table_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> AliasTableExpression:
+        if scanner.get_as_children_scanner().search_one_type_set_use_upper({"SELECT", "WITH"}):
+            return cls._parse_sub_query_expression(scanner, sql_type=sql_type)
+        if scanner.search_one_type_mark(AMTMark.PARENTHESIS):  # 额外的插入语（因为只有一个元素，所以直接递归解析即可）
+            return cls._parse_table_expression(scanner.pop_as_children_scanner(), sql_type=sql_type)
+        return cls._parse_table_name_expression(scanner)
 
     @classmethod
-    def parse_table_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTFromTableExpression:
+    def parse_from_table(cls, scanner_or_string: ScannerOrString,
+                         sql_type: SQLType = SQLType.DEFAULT) -> node.ASTFromTable:
         """解析 FROM 和 JOIN 子句元素：包含别名的表表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        name_expression = cls.parse_type_table_expression(scanner, sql_type=sql_type)
-        alias_expression = (cls.parse_alias_expression(scanner, sql_type=sql_type)
-                            if cls.check_alias_expression(scanner, sql_type=sql_type) else None)
-        return node.ASTFromTableExpression(name=name_expression, alias=alias_expression)
+        return cls._parse_from_table(scanner, sql_type)
+
+    @classmethod
+    def _parse_from_table(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTFromTable:
+        name_expression = cls._parse_table_expression(scanner, sql_type=sql_type)
+        alias_expression = cls._parse_alias_expression(scanner)
+        return node.ASTFromTable(name=name_expression, alias=alias_expression)
 
     @classmethod
-    def parse_column_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSelectColumnExpression:
+    def parse_select_column(cls, scanner_or_string: ScannerOrString,
+                            sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSelectColumn:
         """解析列名表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        general_expression = cls.parse_general_expression(scanner, sql_type=sql_type)
-        alias_expression = (cls.parse_alias_expression(scanner, sql_type=sql_type)
-                            if cls.check_alias_expression(scanner, sql_type=sql_type) else None)
-        return node.ASTSelectColumnExpression(value=general_expression, alias=alias_expression)
+        return cls._parse_select_column(scanner, sql_type)
 
     @classmethod
-    def check_select_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                            sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 SELECT 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("SELECT")
+    def _parse_select_column(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTSelectColumn:
+        general_expression = cls._parse_logical_or_level_expression(scanner, sql_type)
+        alias_expression = cls._parse_alias_expression(scanner)
+        return node.ASTSelectColumn(value=general_expression, alias=alias_expression)
 
     @classmethod
-    def parse_select_clause(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_select_clause(cls, scanner_or_string: ScannerOrString,
                             sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSelectClause:
         """解析 SELECT 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("SELECT")
-        distinct = scanner.search_and_move("DISTINCT")
-        columns = [cls.parse_column_expression(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            columns.append(cls.parse_column_expression(scanner, sql_type=sql_type))
-        return node.ASTSelectClause(distinct=distinct, columns=tuple(columns))
+        return cls._parse_select_clause(scanner, sql_type)
 
     @classmethod
-    def check_from_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                          sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 FROM 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("FROM")
+    def _parse_select_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTSelectClause:
+        scanner.match("SELECT")
+        distinct = scanner.search_and_move_one_type_str_use_upper("DISTINCT")
+        columns = [cls._parse_select_column(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            columns.append(cls._parse_select_column(scanner, sql_type))
+        return node.ASTSelectClause(distinct=distinct, columns=tuple(columns))
 
     @classmethod
-    def parse_from_clause(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_from_clause(cls, scanner_or_string: ScannerOrString,
                           sql_type: SQLType = SQLType.DEFAULT) -> node.ASTFromClause:
         """解析 FROM 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("FROM")
-        tables = [cls.parse_table_expression(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            tables.append(cls.parse_table_expression(scanner, sql_type=sql_type))
-        return node.ASTFromClause(tables=tuple(tables))
+        return cls._parse_from_clause(scanner, sql_type)
 
     @classmethod
-    def check_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                                  sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 LATERAL VIEW 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("LATERAL", "VIEW")
+    def _parse_from_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTFromClause:
+        scanner.match("FROM")
+        tables = [cls._parse_from_table(scanner, sql_type=sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            tables.append(cls._parse_from_table(scanner, sql_type=sql_type))
+        return node.ASTFromClause(tables=tuple(tables))
 
     @classmethod
-    def parse_lateral_view_clause(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_lateral_view_clause(cls, scanner_or_string: ScannerOrString,
                                   sql_type: SQLType = SQLType.DEFAULT) -> node.ASTLateralViewClause:
         """解析 LATERAL VIEW 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_lateral_view_clause(scanner, sql_type)
+
+    @classmethod
+    def _parse_lateral_view_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTLateralViewClause:
         scanner.match("LATERAL", "VIEW")
-        outer = scanner.search_and_move("OUTER")
-        function = cls.parse_function_expression(scanner, sql_type=sql_type)
+        outer = scanner.search_and_move_one_type_str_use_upper("OUTER")
+        function = cls._parse_function_expression(scanner, sql_type=sql_type)
         view_name = scanner.pop_as_source()
-        alias = cls.parse_multi_alias_expression(scanner, sql_type=sql_type)
+        alias = cls._parse_multi_alias_expression(scanner)
         return node.ASTLateralViewClause(outer=outer, function=function, view_name=view_name, alias=alias)
 
     @classmethod
-    def check_join_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                          sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 JOIN 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return cls.check_join_type(scanner, sql_type=sql_type)
-
-    @classmethod
-    def parse_join_clause(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_join_clause(cls, scanner_or_string: ScannerOrString,
                           sql_type: SQLType = SQLType.DEFAULT) -> node.ASTJoinClause:
         """解析 JOIN 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        join_type = cls.parse_join_type(scanner, sql_type=sql_type)
-        table_expression = cls.parse_table_expression(scanner, sql_type=sql_type)
-        if cls.check_join_expression(scanner, sql_type=sql_type):
-            join_rule = cls.parse_join_expression(scanner, sql_type=sql_type)
+        return cls._parse_join_clause(scanner, sql_type)
+
+    @classmethod
+    def _parse_join_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTJoinClause:
+        join_type = cls._parse_join_type(scanner)
+        table_expression = cls._parse_from_table(scanner, sql_type=sql_type)
+        if scanner.search_one_type_set_use_upper({"ON", "USING"}):
+            join_rule = cls._parse_join_expression(scanner, sql_type=sql_type)
         else:
             join_rule = None
         return node.ASTJoinClause(type=join_type, table=table_expression, rule=join_rule)
 
     @classmethod
-    def check_where_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                           sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为 WHERE 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("WHERE")
-
-    @classmethod
-    def parse_where_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                           sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWhereClause:
+    def parse_where_clause(cls, scanner_or_string: ScannerOrString,
+                           sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTWhereClause]:
         """解析 WHERE 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("WHERE")
-        return node.ASTWhereClause(condition=cls.parse_general_expression(scanner, sql_type=sql_type))
-
-    @classmethod
-    def check_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为 GROUP BY 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("GROUP", "BY")
+        return cls._parse_where_clause(scanner, sql_type)
 
     @classmethod
-    def check_grouping_sets(cls, scanner_or_string: Union[TokenScanner, str],
-                            sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 GROUPING SETS 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("GROUPING", "SETS")
+    def _parse_where_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTWhereClause]:
+        if not scanner.search_and_move_one_type_str_use_upper("WHERE"):
+            return None
+        return node.ASTWhereClause(condition=cls._parse_logical_or_level_expression(scanner, sql_type=sql_type))
 
     @classmethod
-    def parse_grouping_sets(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_grouping_sets(cls, scanner_or_string: ScannerOrString,
                             sql_type: SQLType = SQLType.DEFAULT) -> node.ASTGroupingSets:
         """解析 GROUP BY 子句的元素"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_grouping_sets(scanner, sql_type)
+
+    @classmethod
+    def _parse_grouping_sets(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTGroupingSets:
         scanner.match("GROUPING", "SETS")
         grouping_list = []
         for grouping_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            if grouping_scanner.search(AMTMark.PARENTHESIS):
+            if grouping_scanner.search_one_type_mark(AMTMark.PARENTHESIS):
                 parenthesis_scanner_list = grouping_scanner.pop_as_children_scanner_list_split_by(",")
                 columns_list = []
                 for parenthesis_scanner in parenthesis_scanner_list:
-                    columns_list.append(cls.parse_polynomial_expression(parenthesis_scanner, sql_type=sql_type))
+                    columns_list.append(cls._parse_compute_expression(parenthesis_scanner, sql_type))
                     parenthesis_scanner.close()
                 grouping_list.append(tuple(columns_list))
             else:
                 grouping_list.append(
-                    tuple([cls.parse_polynomial_expression(grouping_scanner, sql_type=sql_type)]))
+                    tuple([cls._parse_compute_expression(grouping_scanner, sql_type)]))
             grouping_scanner.close()
         return node.ASTGroupingSets(grouping_list=tuple(grouping_list))
 
     @classmethod
-    def parse_group_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> node.ASTGroupByClause:
+    def parse_group_by_clause(cls, scanner_or_string: ScannerOrString,
+                              sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTGroupByClause]:
         """解析 GROUP BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("GROUP", "BY")
+        return cls._parse_group_by_clause(scanner, sql_type)
+
+    @classmethod
+    def _parse_group_by_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTGroupByClause]:
+        if not scanner.search_and_move_two_type_str_use_upper("GROUP", "BY"):
+            return None
         columns = []
-        if not cls.check_grouping_sets(scanner, sql_type=sql_type):
+        if not scanner.search_two_type_str_use_upper("GROUPING", "SETS"):
             # 如果当 GROUP BY 子句中直接就是 GROUPING SETS 时，则不尝试解析字段
-            columns.append(cls.parse_polynomial_expression(scanner, sql_type=sql_type))
-            while scanner.search_and_move(","):
-                columns.append(cls.parse_polynomial_expression(scanner, sql_type=sql_type))
-        if cls.check_grouping_sets(scanner, sql_type=sql_type):
-            grouping_sets = cls.parse_grouping_sets(scanner, sql_type=sql_type)
+            columns.append(cls._parse_compute_expression(scanner, sql_type))
+            while scanner.search_and_move_one_type_str(","):
+                columns.append(cls._parse_compute_expression(scanner, sql_type))
+        if scanner.search_two_type_str_use_upper("GROUPING", "SETS"):
+            grouping_sets = cls._parse_grouping_sets(scanner, sql_type)
         else:
             grouping_sets = None
-        with_rollup = scanner.search_and_move("WITH", "ROLLUP")
+        with_cube = scanner.search_and_move_two_type_str_use_upper("WITH", "CUBE")
+        with_rollup = scanner.search_and_move_two_type_str_use_upper("WITH", "ROLLUP")
         return node.ASTGroupByClause(
             columns=tuple(columns),
             grouping_sets=grouping_sets,
+            with_cube=with_cube,
             with_rollup=with_rollup
         )
 
     @classmethod
-    def check_having_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                            sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """是否可能为 HAVING 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("HAVING")
-
-    @classmethod
-    def parse_having_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                            sql_type: SQLType = SQLType.DEFAULT) -> node.ASTHavingClause:
+    def parse_having_clause(cls, scanner_or_string: ScannerOrString,
+                            sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTHavingClause]:
         """解析 HAVING 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("HAVING")
-        return node.ASTHavingClause(condition=cls.parse_general_expression(scanner, sql_type=sql_type))
+        return cls._parse_having_clause(scanner, sql_type)
 
     @classmethod
-    def check_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """是否可能为 ORDER BY 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("ORDER", "BY")
+    def _parse_having_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTHavingClause]:
+        if not scanner.search_and_move_one_type_str_use_upper("HAVING"):
+            return None
+        return node.ASTHavingClause(condition=cls._parse_logical_or_level_expression(scanner, sql_type=sql_type))
 
     @classmethod
-    def _parse_order_by_item(cls, scanner: TokenScanner,
-                             sql_type: SQLType = SQLType.DEFAULT) -> node.ASTOrderByColumnExpression:
-        column = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-        order = cls.parse_order_type(scanner, sql_type=sql_type)
-        nulls_first = scanner.search_and_move("NULLS", "FIRST")
-        nulls_last = scanner.search_and_move("NULLS", "LAST")
+    def _parse_order_by_column(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTOrderByColumn:
+        """解析 ORDER BY 子句的元素"""
+        column = cls._parse_compute_expression(scanner, sql_type)
+        order = cls._parse_order_type(scanner)
+        nulls_first = scanner.search_and_move_two_type_str_use_upper("NULLS", "FIRST")
+        nulls_last = scanner.search_and_move_two_type_str_use_upper("NULLS", "LAST")
         if nulls_first is True and nulls_last is True:
             raise SqlParseError("同时定义了 NULLS FIRST 和 NULLS LAST")
-        return node.ASTOrderByColumnExpression(
+        return node.ASTOrderByColumn(
             column=column,
             order=order,
             nulls_first=nulls_first,
             nulls_last=nulls_last
         )
 
     @classmethod
-    def parse_order_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                              sql_type: SQLType = SQLType.DEFAULT) -> node.ASTOrderByClause:
+    def parse_order_by_clause(cls, scanner_or_string: ScannerOrString,
+                              sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTOrderByClause]:
         """解析 ORDER BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("ORDER", "BY")
-        columns = [cls._parse_order_by_item(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            columns.append(cls._parse_order_by_item(scanner, sql_type=sql_type))
-        return node.ASTOrderByClause(columns=tuple(columns))
+        return cls._parse_order_by_clause(scanner, sql_type)
 
     @classmethod
-    def check_sort_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                             sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """是否可能为 SORT BY 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("SORT", "BY")
+    def _parse_order_by_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTOrderByClause]:
+        if not scanner.search_and_move_two_type_str_use_upper("ORDER", "BY"):
+            return None
+        columns = [cls._parse_order_by_column(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            columns.append(cls._parse_order_by_column(scanner, sql_type))
+        return node.ASTOrderByClause(columns=tuple(columns))
 
     @classmethod
-    def parse_sort_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                             sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSortByClause:
+    def parse_sort_by_clause(cls, scanner_or_string: ScannerOrString,
+                             sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTSortByClause]:
         """解析 SORT BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("SORT", "BY")
-        columns = [cls._parse_order_by_item(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            columns.append(cls._parse_order_by_item(scanner, sql_type=sql_type))
-        return node.ASTSortByClause(columns=tuple(columns))
+        return cls._parse_sort_by_clause(scanner, sql_type)
 
     @classmethod
-    def check_distribute_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                                   sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为 DISTRIBUTE BY 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("DISTRIBUTE", "BY")
+    def _parse_sort_by_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTSortByClause]:
+        if not scanner.search_and_move_two_type_str_use_upper("SORT", "BY"):
+            return None
+        columns = [cls._parse_order_by_column(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            columns.append(cls._parse_order_by_column(scanner, sql_type))
+        return node.ASTSortByClause(columns=tuple(columns))
 
     @classmethod
-    def parse_distribute_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                                   sql_type: SQLType = SQLType.DEFAULT) -> node.ASTDistributeByClause:
+    def parse_distribute_by_clause(cls, scanner_or_string: ScannerOrString,
+                                   sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTDistributeByClause]:
         """解析 DISTRIBUTE BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("DISTRIBUTE", "BY")
-        columns = [cls.parse_polynomial_expression(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            columns.append(cls.parse_polynomial_expression(scanner, sql_type=sql_type))
-        return node.ASTDistributeByClause(columns=tuple(columns))
+        return cls._parse_distribute_by_clause(scanner, sql_type)
 
     @classmethod
-    def check_cluster_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                                sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为 CLUSTER BY 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("CLUSTER", "BY")
+    def _parse_distribute_by_clause(cls, scanner: TokenScanner,
+                                    sql_type: SQLType) -> Optional[node.ASTDistributeByClause]:
+        if not scanner.search_and_move_two_type_str_use_upper("DISTRIBUTE", "BY"):
+            return None
+        columns = [cls._parse_compute_expression(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            columns.append(cls._parse_compute_expression(scanner, sql_type))
+        return node.ASTDistributeByClause(columns=tuple(columns))
 
     @classmethod
-    def parse_cluster_by_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                                sql_type: SQLType = SQLType.DEFAULT) -> node.ASTClusterByClause:
+    def parse_cluster_by_clause(cls, scanner_or_string: ScannerOrString,
+                                sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTClusterByClause]:
         """解析 CLUSTER BY 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("DISTRIBUTE", "BY")
-        columns = [cls.parse_polynomial_expression(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            columns.append(cls.parse_polynomial_expression(scanner, sql_type=sql_type))
-        return node.ASTClusterByClause(columns=tuple(columns))
+        return cls._parse_cluster_by_clause(scanner, sql_type)
 
     @classmethod
-    def check_limit_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                           sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """是否可能为 LIMIT 子句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("LIMIT")
+    def _parse_cluster_by_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTClusterByClause]:
+        if not scanner.search_and_move_two_type_str_use_upper("CLUSTER", "BY"):
+            return None
+        columns = [cls._parse_compute_expression(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            columns.append(cls._parse_compute_expression(scanner, sql_type))
+        return node.ASTClusterByClause(columns=tuple(columns))
 
     @classmethod
-    def parse_limit_clause(cls, scanner_or_string: Union[TokenScanner, str],
-                           sql_type: SQLType = SQLType.DEFAULT) -> node.ASTLimitClause:
+    def parse_limit_clause(cls, scanner_or_string: ScannerOrString,
+                           sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTLimitClause]:
         """解析 LIMIT 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if not scanner.search_and_move("LIMIT"):
-            raise SqlParseError("无法解析为 LIMIT 子句")
-        cnt_1 = cls.parse_literal_expression(scanner, unary_operator=None, sql_type=sql_type).as_int()
-        if scanner.search_and_move(","):
+        return cls._parse_limit_clause(scanner)
+
+    @classmethod
+    def _parse_limit_clause(cls, scanner: TokenScanner) -> Optional[node.ASTLimitClause]:
+        if not scanner.search_and_move_one_type_str_use_upper("LIMIT"):
+            return None
+        cnt_1 = cls._parse_literal_expression(scanner).as_int()
+        if scanner.search_and_move_one_type_str(","):
             offset_int = cnt_1
-            limit_int = cls.parse_literal_expression(scanner, unary_operator=None, sql_type=sql_type).as_int()
-        elif scanner.search_and_move("OFFSET"):
-            offset_int = cls.parse_literal_expression(scanner, unary_operator=None, sql_type=sql_type).as_int()
+            limit_int = cls._parse_literal_expression(scanner).as_int()
+        elif scanner.search_and_move_one_type_str_use_upper("OFFSET"):
+            offset_int = cls._parse_literal_expression(scanner).as_int()
             limit_int = cnt_1
         else:
             offset_int = None
             limit_int = cnt_1
         return node.ASTLimitClause(limit=limit_int, offset=offset_int)
 
     @classmethod
-    def _parse_single_with_table(cls, scanner_or_string: Union[TokenScanner, str],
-                                 sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWithTable:
+    def parse_with_table(cls, scanner_or_string: ScannerOrString,
+                         sql_type: SQLType = SQLType.DEFAULT) -> node.ASTWithTable:
         """解析一个 WITH 临时表"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        table_name = unify_name(scanner.pop_as_source())
+        return cls._parse_with_table(scanner, sql_type)
+
+    @classmethod
+    def _parse_with_table(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTWithTable:
+        table_name = cls._unify_name(scanner.pop_as_source())
         scanner.match("AS")
         parenthesis_scanner = scanner.pop_as_children_scanner()
-        table_statement = cls.parse_select_statement(parenthesis_scanner,
-                                                     with_clause=node.ASTWithClause.empty(),
-                                                     sql_type=sql_type)
+        table_statement = cls._parse_select_statement(parenthesis_scanner, node.ASTWithClause.empty(), sql_type)
         parenthesis_scanner.close()
         return node.ASTWithTable(name=table_name, statement=table_statement)
 
     @classmethod
-    def parse_with_clause(cls, scanner_or_string: Union[TokenScanner, str], sql_type: SQLType = SQLType.DEFAULT) -> \
-            Optional[node.ASTWithClause]:
+    def parse_with_clause(cls,
+                          scanner_or_string: ScannerOrString,
+                          sql_type: SQLType = SQLType.DEFAULT) -> Optional[node.ASTWithClause]:
         """解析 WITH 子句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("WITH"):
-            tables = [cls._parse_single_with_table(scanner, sql_type=sql_type)]
-            while scanner.search_and_move(","):
-                table_statement = cls._parse_single_with_table(scanner, sql_type=sql_type)
+        return cls._parse_with_clause(scanner, sql_type)
+
+    @classmethod
+    def _parse_with_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> Optional[node.ASTWithClause]:
+        if scanner.search_and_move_one_type_str_use_upper("WITH"):
+            tables = [cls._parse_with_table(scanner, sql_type)]
+            while scanner.search_and_move_one_type_str(","):
+                table_statement = cls._parse_with_table(scanner, sql_type)
                 tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
             return node.ASTWithClause(tables=tuple(tables))
         return node.ASTWithClause.empty()
 
     @classmethod
-    def check_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为 SELECT 语句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("SELECT")
-
-    @classmethod
-    def parse_single_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_single_select_statement(cls, scanner_or_string: ScannerOrString,
                                       with_clause: Optional[node.ASTWithClause] = None,
                                       sql_type: SQLType = SQLType.DEFAULT
                                       ) -> node.ASTSingleSelectStatement:
-        # pylint: disable=R0912
-        # pylint: disable=R0914
         """
 
         Parameters
         ----------
-        scanner_or_string : Union[TokenScanner, str]
+        scanner_or_string : ScannerOrString
             扫描器
         with_clause : Optional[SQLWithClause], default = None
             前置 with 语句，如果该参数为 None 的话，则会尝试匹配 WITH 语句
         sql_type : SQLType
             SQL 类型
         """
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_single_select_statement(scanner, with_clause, sql_type)
+
+    @classmethod
+    def _parse_single_select_statement(cls, scanner: TokenScanner,
+                                       with_clause: Optional[node.ASTWithClause],
+                                       sql_type: SQLType) -> node.ASTSingleSelectStatement:
+        # pylint: disable=R0912
+        # pylint: disable=R0914
         if with_clause is None:
-            with_clause = cls.parse_with_clause(scanner, sql_type=sql_type)
+            with_clause = cls._parse_with_clause(scanner, sql_type)
 
         # 允许在外层添加任意数量的括号
         inner_scanner = scanner
         parenthesis_stack = []
-        while inner_scanner.search(AMTMark.PARENTHESIS):
+        while inner_scanner.search_one_type_mark(AMTMark.PARENTHESIS):
             inner_scanner = scanner.pop_as_children_scanner()
             parenthesis_stack.append(inner_scanner)
 
-        select_clause = cls.parse_select_clause(inner_scanner, sql_type=sql_type)
-        from_clause = (cls.parse_from_clause(inner_scanner, sql_type=sql_type)
-                       if cls.check_from_clause(inner_scanner, sql_type=sql_type) else None)
+        select_clause = cls._parse_select_clause(inner_scanner, sql_type)
+        from_clause = (cls._parse_from_clause(inner_scanner, sql_type)
+                       if inner_scanner.search_one_type_str_use_upper("FROM") else None)
         lateral_view_clauses = []
-        while cls.check_lateral_view_clause(inner_scanner, sql_type=sql_type):
-            lateral_view_clauses.append(cls.parse_lateral_view_clause(inner_scanner, sql_type=sql_type))
+        while scanner.search_two_type_str_use_upper("LATERAL", "VIEW"):
+            lateral_view_clauses.append(cls._parse_lateral_view_clause(inner_scanner, sql_type))
         join_clause = []
-        while cls.check_join_clause(inner_scanner, sql_type=sql_type):
-            join_clause.append(cls.parse_join_clause(inner_scanner, sql_type=sql_type))
-        where_clause = (cls.parse_where_clause(inner_scanner, sql_type=sql_type)
-                        if cls.check_where_clause(inner_scanner, sql_type=sql_type) else None)
-        group_by_clause = (cls.parse_group_by_clause(inner_scanner, sql_type=sql_type)
-                           if cls.check_group_by_clause(inner_scanner, sql_type=sql_type) else None)
-        having_clause = (cls.parse_having_clause(inner_scanner, sql_type=sql_type)
-                         if cls.check_having_clause(inner_scanner, sql_type=sql_type) else None)
-        order_by_clause = (cls.parse_order_by_clause(inner_scanner, sql_type=sql_type)
-                           if cls.check_order_by_clause(inner_scanner, sql_type=sql_type) else None)
-
-        if sql_type == SQLType.HIVE and cls.check_sort_by_clause(inner_scanner, sql_type=sql_type):
-            sort_by_clause = cls.parse_sort_by_clause(inner_scanner, sql_type=sql_type)
-        else:
-            sort_by_clause = None
-
-        if sql_type == SQLType.HIVE and cls.check_distribute_by_clause(inner_scanner, sql_type=sql_type):
-            distribute_by_clause = cls.parse_distribute_by_clause(inner_scanner, sql_type=sql_type)
-        else:
-            distribute_by_clause = None
-
-        if sql_type == SQLType.HIVE and cls.check_cluster_by_clause(inner_scanner, sql_type=sql_type):
-            cluster_by_clause = cls.parse_cluster_by_clause(inner_scanner, sql_type=sql_type)
-        else:
-            cluster_by_clause = None
-
-        if cls.check_limit_clause(inner_scanner, sql_type=sql_type):
-            limit_clause = cls.parse_limit_clause(inner_scanner, sql_type=sql_type)
-        else:
-            limit_clause = None
+        while scanner.search_one_type_set_use_upper({"JOIN", "INNER", "LEFT", "RIGHT", "FULL", "CROSS"}):
+            join_clause.append(cls._parse_join_clause(inner_scanner, sql_type))
+        where_clause = cls._parse_where_clause(inner_scanner, sql_type)
+        group_by_clause = cls._parse_group_by_clause(inner_scanner, sql_type)
+        having_clause = cls._parse_having_clause(inner_scanner, sql_type)
+        order_by_clause = cls._parse_order_by_clause(inner_scanner, sql_type)
+        sort_by_clause = cls._parse_sort_by_clause(inner_scanner, sql_type)
+        distribute_by_clause = cls._parse_distribute_by_clause(inner_scanner, sql_type)
+        cluster_by_clause = cls._parse_cluster_by_clause(inner_scanner, sql_type)
+        limit_clause = cls._parse_limit_clause(inner_scanner)
 
         while parenthesis_stack:
             parenthesis_stack.pop().close()
 
         return node.ASTSingleSelectStatement(
             with_clause=with_clause,
             select_clause=select_clause,
@@ -1291,446 +1477,440 @@
             sort_by_clause=sort_by_clause,
             distribute_by_clause=distribute_by_clause,
             cluster_by_clause=cluster_by_clause,
             limit_clause=limit_clause
         )
 
     @classmethod
-    def parse_select_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_select_statement(cls, scanner_or_string: ScannerOrString,
                                with_clause: Optional[node.ASTWithClause] = None,
                                sql_type: SQLType = SQLType.DEFAULT
                                ) -> node.ASTSelectStatement:
         """解析 SELECT 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_select_statement(scanner, with_clause, sql_type)
+
+    @classmethod
+    def _parse_select_statement(cls, scanner: TokenScanner,
+                                with_clause: Optional[node.ASTWithClause],
+                                sql_type: SQLType) -> node.ASTSelectStatement:
         if with_clause is None:
-            with_clause = cls.parse_with_clause(scanner, sql_type=sql_type)
-        result = [cls.parse_single_select_statement(scanner, with_clause=with_clause, sql_type=sql_type)]
-        while not scanner.is_finish and cls.check_union_type(scanner, sql_type=sql_type):
-            result.append(cls.parse_union_type(scanner, sql_type=sql_type))
-            result.append(cls.parse_single_select_statement(scanner, with_clause=with_clause, sql_type=sql_type))
+            with_clause = cls._parse_with_clause(scanner, sql_type)
+        result = [cls._parse_single_select_statement(scanner, with_clause, sql_type)]
+        while scanner.search_one_type_set_use_upper({"UNION", "EXCEPT", "INTERSECT", "MINUS"}):
+            result.append(cls._parse_union_type(scanner))
+            result.append(cls._parse_single_select_statement(scanner, with_clause, sql_type))
         if len(result) == 1:
             return result[0]
         return node.ASTUnionSelectStatement(with_clause=with_clause, elements=tuple(result))
 
     @classmethod
-    def _parse_config_string(cls, scanner: TokenScanner) -> str:
-        """解析配置名称或配置值：字符串中允许包含 . 符合和 - 符合"""
-        column_string = [scanner.pop_as_source()]
-        while True:
-            if scanner.search_and_move("."):
-                column_string.append(".")
-                column_string.append(scanner.pop_as_source())
-            elif scanner.search_and_move("-"):
-                column_string.append("-")
-                column_string.append(scanner.pop_as_source())
-            else:
-                break
-        return "".join(column_string)
-
-    @classmethod
-    def parse_config_string_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_config_string_expression(cls, scanner_or_string: ScannerOrString,
                                        sql_type: SQLType = SQLType.DEFAULT
                                        ) -> node.ASTConfigStringExpression:
         """解析配置值为字符串的配置表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_config_string_expression(scanner)
+
+    @classmethod
+    def _parse_config_string_expression(cls, scanner: TokenScanner) -> node.ASTConfigStringExpression:
         config_name = cls._parse_config_string(scanner)
         scanner.match("=")
         config_value = cls._parse_config_string(scanner)
         return node.ASTConfigStringExpression(name=config_name, value=config_value)
 
     @classmethod
-    def parse_column_type_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_column_type_expression(cls, scanner_or_string: ScannerOrString,
                                      sql_type: SQLType = SQLType.DEFAULT) -> node.ASTColumnTypeExpression:
         """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_column_type_expression(scanner, sql_type)
 
+    @classmethod
+    def _parse_column_type_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTColumnTypeExpression:
         # 解析字段类型名称
         function_name: str = scanner.pop_as_source()
 
         # 解析字段类型参数
-        if scanner.search(AMTMark.PARENTHESIS):
+        if scanner.search_one_type_mark(AMTMark.PARENTHESIS):
             function_params: List[node.ASTExpressionBase] = []
             for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-                function_params.append(cls.parse_polynomial_expression(param_scanner, sql_type=sql_type))
+                function_params.append(cls._parse_compute_expression(param_scanner, sql_type))
                 param_scanner.close()
             return node.ASTColumnTypeExpression(name=function_name, params=tuple(function_params))
         return node.ASTColumnTypeExpression(name=function_name)
 
     @classmethod
-    def check_partition_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                   sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否可能为分区表达式"""
+    def parse_partition_expression(cls, scanner_or_string: ScannerOrString,
+                                   already_match_partition: bool = False,
+                                   sql_type: SQLType = SQLType.DEFAULT) -> node.ASTPartitionExpression:
+        """解析分区表达式
+
+        already_match_partition : bool, default = False
+            是否已匹配 PARTITION 关键字
+        """
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("PARTITION")
+        return cls._parse_partition_expression(scanner, already_match_partition, sql_type)
 
     @classmethod
-    def parse_partition_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                   sql_type: SQLType = SQLType.DEFAULT) -> node.ASTPartitionExpression:
-        """解析分区表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        scanner.match("PARTITION")
+    def _parse_partition_expression(cls, scanner: TokenScanner, already_match_partition: bool,
+                                    sql_type: SQLType) -> node.ASTPartitionExpression:
+        if not already_match_partition:
+            scanner.match("PARTITION")
         partition_list = []
         is_dynamic_partition = False  # 是否有动态分区
         is_non_dynamic_partition = False  # 是否有非动态分区
         for partition_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            before_value = cls.parse_polynomial_expression(partition_scanner, sql_type=sql_type)
-            if cls.check_compare_operator(partition_scanner, sql_type=sql_type):  # 非动态分区
+            before_value = cls._parse_compute_expression(partition_scanner, sql_type)
+            if partition_scanner.search_one_type_set(static.COMPARE_OPERATOR_SET):  # 非动态分区
                 is_non_dynamic_partition = True
-                operator = cls.parse_compare_operator(partition_scanner, sql_type=sql_type)
-                after_value = cls.parse_polynomial_expression(partition_scanner, sql_type=sql_type)
-                partition_list.append(node.ASTBoolCompareExpression(
-                    is_not=False,
+                operator = cls._parse_compare_operator(partition_scanner)
+                after_value = cls._parse_compute_expression(partition_scanner, sql_type)
+                partition_list.append(node.ASTOperatorConditionExpression(
                     before_value=before_value,
                     operator=operator,
                     after_value=after_value
                 ))
             else:
                 is_dynamic_partition = True
                 partition_list.append(before_value)  # 动态分区
             partition_scanner.close()
         if is_dynamic_partition is True and is_non_dynamic_partition is True:
             raise SqlParseError("分区表达式同时包含动态分区和非动态分区")
         return node.ASTPartitionExpression(partitions=tuple(partition_list))
 
     @classmethod
-    def check_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                     sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为外键表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("CONSTRAINT")
-
-    @classmethod
-    def parse_foreign_key_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_foreign_key_expression(cls, scanner_or_string: ScannerOrString,
                                      sql_type: SQLType = SQLType.DEFAULT) -> node.ASTForeignKeyExpression:
         """解析外键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_foreign_key_expression(scanner)
+
+    @classmethod
+    def _parse_foreign_key_expression(cls, scanner: TokenScanner) -> node.ASTForeignKeyExpression:
         scanner.match("CONSTRAINT")
         constraint_name = scanner.pop_as_source()
         scanner.match("FOREIGN", "KEY")
         slave_columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
             slave_columns.append(column_scanner.pop_as_source())
             column_scanner.close()
         scanner.match("REFERENCES")
         master_table_name = scanner.pop_as_source()
         master_columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
             master_columns.append(column_scanner.pop_as_source())
             column_scanner.close()
-        on_delete_cascade = scanner.search_and_move("ON", "DELETE", "CASCADE")
+        on_delete_cascade = scanner.search_and_move_three_type_str_use_upper("ON", "DELETE", "CASCADE")
         return node.ASTForeignKeyExpression(
             constraint_name=constraint_name,
             slave_columns=tuple(slave_columns),
             master_table_name=master_table_name,
             master_columns=tuple(master_columns),
             on_delete_cascade=on_delete_cascade
         )
 
     @classmethod
-    def parse_index_column(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_index_column(cls, scanner_or_string: ScannerOrString,
                            sql_type: SQLType = SQLType.DEFAULT) -> node.ASTIndexColumn:
         """解析索引声明表达式中的字段"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        name = unify_name(scanner.pop_as_source())
+        return cls._parse_index_column(scanner)
+
+    @classmethod
+    def _parse_index_column(cls, scanner: TokenScanner) -> node.ASTIndexColumn:
+        name = cls._unify_name(scanner.pop_as_source())
         max_length = None
-        if scanner.search(AMTMark.PARENTHESIS):
+        if scanner.search_one_type_mark(AMTMark.PARENTHESIS):
             parenthesis_scanner = scanner.pop_as_children_scanner()
             max_length = int(parenthesis_scanner.pop_as_source())
             parenthesis_scanner.close()
         return node.ASTIndexColumn(name=name, max_length=max_length)
 
     @classmethod
-    def _get_index_columns(cls, scanner: TokenScanner,
-                           sql_type: SQLType = SQLType.DEFAULT
-                           ) -> Tuple[node.ASTIndexColumn, ...]:
+    def _get_index_columns(cls, scanner: TokenScanner) -> Tuple[node.ASTIndexColumn, ...]:
         """解析索引表达式中的索引字段"""
         columns = []
         for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            columns.append(cls.parse_index_column(column_scanner, sql_type=sql_type))
+            columns.append(cls._parse_index_column(column_scanner))
             column_scanner.close()
         return tuple(columns)
 
     @classmethod
-    def check_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                       sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为主键表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("PRIMARY", "KEY")
-
-    @classmethod
-    def parse_primary_index_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_primary_index_expression(cls, scanner_or_string: ScannerOrString,
                                        sql_type: SQLType = SQLType.DEFAULT
                                        ) -> node.ASTPrimaryIndexExpression:
         """解析主键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_primary_index_expression(scanner)
+
+    @classmethod
+    def _parse_primary_index_expression(cls, scanner: TokenScanner) -> node.ASTPrimaryIndexExpression:
         scanner.match("PRIMARY", "KEY")
-        columns = cls._get_index_columns(scanner, sql_type=sql_type)
-        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
-        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
-        key_block_size = int(scanner.pop_as_source()) if scanner.search_and_move("KEY_BLOCK_SIZE", "=") else None
+        columns = cls._get_index_columns(scanner)
+        using = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("COMMENT") else None
+        key_block_size = (int(scanner.pop_as_source())
+                          if scanner.search_and_move_two_type_str_use_upper("KEY_BLOCK_SIZE", "=") else None)
         return node.ASTPrimaryIndexExpression(columns=columns, using=using, comment=comment,
                                               key_block_size=key_block_size)
 
     @classmethod
-    def check_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                      sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为唯一键表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("UNIQUE", "KEY")
-
-    @classmethod
-    def parse_unique_index_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_unique_index_expression(cls, scanner_or_string: ScannerOrString,
                                       sql_type: SQLType = SQLType.DEFAULT
                                       ) -> node.ASTUniqueIndexExpression:
         """解析唯一键表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_unique_index_expression(scanner)
+
+    @classmethod
+    def _parse_unique_index_expression(cls, scanner: TokenScanner) -> node.ASTUniqueIndexExpression:
         scanner.match("UNIQUE", "KEY")
         name = scanner.pop_as_source()
-        columns = cls._get_index_columns(scanner, sql_type=sql_type)
-        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
-        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
-        key_block_size = int(scanner.pop_as_source()) if scanner.search_and_move("KEY_BLOCK_SIZE", "=") else None
+        columns = cls._get_index_columns(scanner)
+        using = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("COMMENT") else None
+        key_block_size = (int(scanner.pop_as_source())
+                          if scanner.search_and_move_two_type_str_use_upper("KEY_BLOCK_SIZE", "=") else None)
         return node.ASTUniqueIndexExpression(name=name, columns=columns, using=using, comment=comment,
                                              key_block_size=key_block_size)
 
     @classmethod
-    def check_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                      sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为一般索引表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("KEY")
-
-    @classmethod
-    def parse_normal_index_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_normal_index_expression(cls, scanner_or_string: ScannerOrString,
                                       sql_type: SQLType = SQLType.DEFAULT
                                       ) -> node.ASTNormalIndexExpression:
         """解析一般索引表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_normal_index_expression(scanner)
+
+    @classmethod
+    def _parse_normal_index_expression(cls, scanner: TokenScanner) -> node.ASTNormalIndexExpression:
         scanner.match("KEY")
         name = scanner.pop_as_source()
-        columns = cls._get_index_columns(scanner, sql_type=sql_type)
-        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
-        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
-        key_block_size = int(scanner.pop_as_source()) if scanner.search_and_move("KEY_BLOCK_SIZE", "=") else None
+        columns = cls._get_index_columns(scanner)
+        using = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("COMMENT") else None
+        key_block_size = (int(scanner.pop_as_source())
+                          if scanner.search_and_move_two_type_str_use_upper("KEY_BLOCK_SIZE", "=") else None)
         return node.ASTNormalIndexExpression(name=name, columns=columns, using=using, comment=comment,
                                              key_block_size=key_block_size)
 
     @classmethod
-    def check_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                                  sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为全文索引表达式"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("FULLTEXT", "KEY")
-
-    @classmethod
-    def parse_fulltext_expression(cls, scanner_or_string: Union[TokenScanner, str], sql_type: SQLType = SQLType.DEFAULT
+    def parse_fulltext_expression(cls, scanner_or_string: ScannerOrString, sql_type: SQLType = SQLType.DEFAULT
                                   ) -> node.ASTFulltextIndexExpression:
         """解析全文索引表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_fulltext_expression(scanner)
+
+    @classmethod
+    def _parse_fulltext_expression(cls, scanner: TokenScanner) -> node.ASTFulltextIndexExpression:
         scanner.match("FULLTEXT", "KEY")
         name = scanner.pop_as_source()
-        columns = cls._get_index_columns(scanner, sql_type=sql_type)
-        using = scanner.pop_as_source() if scanner.search_and_move("USING") else None
-        comment = scanner.pop_as_source() if scanner.search_and_move("COMMENT") else None
-        key_block_size = int(scanner.pop_as_source()) if scanner.search_and_move("KEY_BLOCK_SIZE", "=") else None
+        columns = cls._get_index_columns(scanner)
+        using = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("USING") else None
+        comment = scanner.pop_as_source() if scanner.search_and_move_one_type_str_use_upper("COMMENT") else None
+        key_block_size = (int(scanner.pop_as_source())
+                          if scanner.search_and_move_two_type_str_use_upper("KEY_BLOCK_SIZE", "=") else None)
         return node.ASTFulltextIndexExpression(name=name, columns=columns, using=using, comment=comment,
                                                key_block_size=key_block_size)
 
     @classmethod
-    def parse_define_column_expression(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_define_column_expression(cls, scanner_or_string: ScannerOrString,
                                        sql_type: SQLType = SQLType.DEFAULT
                                        ) -> node.ASTDefineColumnExpression:
         # pylint: disable=R0914
-
         """解析 DDL 的字段表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_define_column_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_define_column_expression(cls, scanner: TokenScanner, sql_type: SQLType
+                                        ) -> node.ASTDefineColumnExpression:
         # 解析顺序固定的信息
         column_name = scanner.pop_as_source()
-        column_type = cls.parse_column_type_expression(scanner, sql_type=sql_type)
+        column_type = cls._parse_column_type_expression(scanner, sql_type)
 
         # 解析顺序可能不定的字段信息
         comment: Optional[str] = None
         is_unsigned: bool = False
         is_zerofill: bool = False
         character_set: Optional[str] = None
         collate: Optional[str] = None
         is_allow_null: bool = False
         is_not_null: bool = False
         is_auto_increment: bool = False
         default: Optional[node.ASTExpressionBase] = None
         on_update: Optional[node.ASTExpressionBase] = None
         while not scanner.is_finish:
-            if scanner.search_and_move("NOT", "NULL"):
+            if scanner.search_and_move_two_type_str_use_upper("NOT", "NULL"):
                 is_not_null = True
-            elif scanner.search_and_move("NULL"):
+            elif scanner.search_and_move_one_type_str_use_upper("NULL"):
                 is_allow_null = True
-            elif scanner.search_and_move("CHARACTER", "SET"):
+            elif scanner.search_and_move_two_type_str_use_upper("CHARACTER", "SET"):
                 character_set = scanner.pop_as_source()
-            elif scanner.search_and_move("COLLATE"):
+            elif scanner.search_and_move_one_type_str_use_upper("COLLATE"):
                 collate = scanner.pop_as_source()
-            elif scanner.search_and_move("DEFAULT"):
-                default = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            elif scanner.search_and_move("COMMENT"):
+            elif scanner.search_and_move_one_type_str_use_upper("DEFAULT"):
+                default = cls._parse_compute_expression(scanner, sql_type)
+            elif scanner.search_and_move_one_type_str_use_upper("COMMENT"):
                 comment = scanner.pop_as_source()
-            elif scanner.search_and_move("ON", "UPDATE"):  # ON UPDATE
-                on_update = cls.parse_polynomial_expression(scanner, sql_type=sql_type)
-            elif scanner.search_and_move("AUTO_INCREMENT"):
+            elif scanner.search_and_move_two_type_str_use_upper("ON", "UPDATE"):
+                on_update = cls._parse_compute_expression(scanner, sql_type)
+            elif scanner.search_and_move_one_type_str_use_upper("AUTO_INCREMENT"):
                 is_auto_increment = True
-            elif scanner.search_and_move("UNSIGNED"):
+            elif scanner.search_and_move_one_type_str_use_upper("UNSIGNED"):
                 is_unsigned = True
-            elif scanner.search_and_move("ZEROFILL"):
+            elif scanner.search_and_move_one_type_str_use_upper("ZEROFILL"):
                 is_zerofill = True
             else:
                 raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
 
         # 构造 DDL 字段表达式对象
         return node.ASTDefineColumnExpression(
-            column_name=unify_name(column_name),
+            column_name=cls._unify_name(column_name),
             column_type=column_type,
             comment=comment,
             is_unsigned=is_unsigned,
             is_zerofill=is_zerofill,
             character_set=character_set,
             collate=collate,
             is_allow_null=is_allow_null,
             is_not_null=is_not_null,
             is_auto_increment=is_auto_increment,
             default=default,
             on_update=on_update
         )
 
     @classmethod
-    def check_insert_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 INSERT 语句（已匹配过 WITH 语句才可以调用）"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("INSERT")
-
-    @classmethod
-    def parse_insert_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_insert_statement(cls, scanner_or_string: ScannerOrString,
                                with_clause: Optional[node.ASTWithClause],
                                sql_type: SQLType = SQLType.DEFAULT,
                                ) -> node.ASTInsertStatement:
         """解析 INSERT 表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_insert_statement(scanner, with_clause, sql_type)
 
+    @classmethod
+    def _parse_insert_statement(cls, scanner: TokenScanner,
+                                with_clause: Optional[node.ASTWithClause],
+                                sql_type: SQLType
+                                ) -> node.ASTInsertStatement:
         if with_clause is None:
-            with_clause = cls.parse_with_clause(scanner, sql_type=sql_type)
+            with_clause = cls._parse_with_clause(scanner, sql_type)
 
-        insert_type = cls.parse_insert_type(scanner, sql_type=sql_type)
+        insert_type = cls._parse_insert_type(scanner)
 
         # 匹配可能包含的 TABLE 关键字
-        scanner.search_and_move("TABLE")
+        scanner.search_and_move_one_type_str_use_upper("TABLE")
 
         # 匹配表名
-        table_name = cls.parse_table_name_expression(scanner, sql_type=sql_type)
+        table_name = cls._parse_table_name_expression(scanner)
 
         # 匹配分区表达式
-        if cls.check_partition_expression(scanner, sql_type=sql_type):
-            partition = cls.parse_partition_expression(scanner, sql_type=sql_type)
+        if scanner.search_one_type_str_use_upper("PARTITION"):
+            partition = cls._parse_partition_expression(scanner, False, sql_type)
         else:
             partition = None
 
         # 匹配列名列表
-        if scanner.search(AMTMark.PARENTHESIS):
+        if scanner.search_one_type_mark(AMTMark.PARENTHESIS):
             columns = []
             for column_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-                columns.append(cls.parse_column_name_expression(column_scanner, unary_operator=None, sql_type=sql_type))
+                columns.append(cls._parse_column_name_expression(column_scanner))
                 column_scanner.close()
         else:
             columns = None
 
         # 匹配 VALUES 类型
-        if scanner.search_and_move("VALUES"):
+        if scanner.search_and_move_one_type_str_use_upper("VALUES"):
             values = []
-            while scanner.search(AMTMark.PARENTHESIS):
-                values.append(cls.parse_value_expression(scanner, sql_type=sql_type))
-                scanner.search_and_move(",")
+            while scanner.search_one_type_mark(AMTMark.PARENTHESIS):
+                values.append(cls._parse_sub_value_expression(scanner, sql_type=sql_type))
+                scanner.search_and_move_one_type_str(",")
 
             return node.ASTInsertValuesStatement(
                 with_clause=with_clause,
                 insert_type=insert_type,
                 table_name=table_name,
                 partition=partition,
                 columns=tuple(columns) if columns is not None else None,
                 values=tuple(values)
             )
 
-        if scanner.search("SELECT"):
-            select_statement = cls.parse_select_statement(scanner,
-                                                          with_clause=node.ASTWithClause.empty(), sql_type=sql_type)
+        if scanner.search_one_type_str_use_upper("SELECT"):
+            select_statement = cls._parse_select_statement(scanner, node.ASTWithClause.empty(), sql_type)
             return node.ASTInsertSelectStatement(
                 with_clause=with_clause,
                 insert_type=insert_type,
                 table_name=table_name,
                 partition=partition,
                 columns=tuple(columns) if columns is not None else None,
                 select_statement=select_statement
             )
 
         raise SqlParseError(f"未知的 INSERT 语句类型 {scanner}")
 
     @classmethod
-    def check_set_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                            sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 SET 语句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("SET")
-
-    @classmethod
-    def parse_set_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_set_statement(cls, scanner_or_string: ScannerOrString,
                             sql_type: SQLType = SQLType.DEFAULT) -> node.ASTSetStatement:
         """解析 SET 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_set_statement(scanner)
+
+    @classmethod
+    def _parse_set_statement(cls, scanner: TokenScanner) -> node.ASTSetStatement:
         scanner.match("SET")
-        config = cls.parse_config_string_expression(scanner, sql_type=sql_type)
+        config = cls._parse_config_string_expression(scanner)
         return node.ASTSetStatement(config=config)
 
     @classmethod
-    def parse_create_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                                     sql_type: SQLType = SQLType.DEFAULT
-                                     ) -> node.AliasCreateTableStatement:
+    def parse_create_table_statement(cls, scanner_or_string: ScannerOrString,
+                                     sql_type: SQLType = SQLType.DEFAULT) -> AliasCreateTableStatement:
+        """解析 CREATE TABLE 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_create_table_statement(scanner, sql_type)
+
+    @classmethod
+    def _parse_create_table_statement(cls, scanner: TokenScanner, sql_type: SQLType) -> AliasCreateTableStatement:
         # pylint: disable=R0912
         # pylint: disable=R0914
         # pylint: disable=R0915
-        """解析 CREATE TABLE 语句"""
         # 解析字段、索引括号前的部分
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
         scanner.match("CREATE", "TABLE")
-        if_not_exists = scanner.search_and_move("IF", "NOT", "EXISTS")
-        table_name = cls.parse_table_name_expression(scanner, sql_type=sql_type)
+        if_not_exists = scanner.search_and_move_three_type_str_use_upper("IF", "NOT", "EXISTS")
+        table_name = cls._parse_table_name_expression(scanner)
 
         # CREATE TABLE ... AS ... 语句
-        if scanner.search_and_move("AS"):
-            select_statement = cls.parse_select_statement(scanner, sql_type=sql_type)
+        if scanner.search_and_move_one_type_str_use_upper("AS"):
+            select_statement = cls._parse_select_statement(scanner, None, sql_type)
             return node.ASTCreateTableAsStatement(
                 table_name=table_name,
                 select_statement=select_statement
             )
 
         # 解析字段和索引
         columns: List[node.ASTDefineColumnExpression] = []
         primary_key: Optional[node.ASTPrimaryIndexExpression] = None
         unique_key: List[node.ASTUniqueIndexExpression] = []
         key: List[node.ASTNormalIndexExpression] = []
         fulltext_key: List[node.ASTFulltextIndexExpression] = []
         foreign_key: List[node.ASTForeignKeyExpression] = []
         for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            if cls.check_primary_index_expression(group_scanner, sql_type=sql_type):
-                primary_key = cls.parse_primary_index_expression(group_scanner, sql_type=sql_type)
-            elif cls.check_unique_index_expression(group_scanner, sql_type=sql_type):
-                unique_key.append(cls.parse_unique_index_expression(group_scanner, sql_type=sql_type))
-            elif cls.check_normal_index_expression(group_scanner, sql_type=sql_type):
-                key.append(cls.parse_normal_index_expression(group_scanner, sql_type=sql_type))
-            elif cls.check_fulltext_expression(group_scanner, sql_type=sql_type):
-                fulltext_key.append(cls.parse_fulltext_expression(group_scanner, sql_type=sql_type))
-            elif cls.check_foreign_key_expression(group_scanner, sql_type=sql_type):
-                foreign_key.append(cls.parse_foreign_key_expression(group_scanner, sql_type=sql_type))
+            if group_scanner.search_two_type_str_use_upper("PRIMARY", "KEY"):
+                primary_key = cls._parse_primary_index_expression(group_scanner)
+            elif group_scanner.search_two_type_str_use_upper("UNIQUE", "KEY"):
+                unique_key.append(cls._parse_unique_index_expression(group_scanner))
+            elif group_scanner.search_one_type_str_use_upper("KEY"):
+                key.append(cls._parse_normal_index_expression(group_scanner))
+            elif group_scanner.search_two_type_str_use_upper("FULLTEXT", "KEY"):
+                fulltext_key.append(cls._parse_fulltext_expression(group_scanner))
+            elif group_scanner.search_one_type_str_use_upper("CONSTRAINT"):
+                foreign_key.append(cls._parse_foreign_key_expression(group_scanner))
             else:
-                columns.append(cls.parse_define_column_expression(group_scanner, sql_type=sql_type))
+                columns.append(cls._parse_define_column_expression(group_scanner, sql_type))
             group_scanner.close()
 
         # 解析表属性
         partitioned_by: List[node.ASTDefineColumnExpression] = []
         comment: Optional[str] = None
         engine: Optional[str] = None
         auto_increment: Optional[int] = None
@@ -1741,64 +1921,64 @@
         row_format_serde: Optional[str] = None
         row_format_delimited_fields_terminated_by: Optional[str] = None
         stored_as_inputformat: Optional[str] = None
         stored_as_textfile: bool = False
         outputformat: Optional[str] = None
         location: Optional[str] = None
         tblproperties: Optional[List[node.ASTConfigStringExpression]] = []
-        while not scanner.is_finish and not scanner.search(";"):
-            if scanner.search_and_move("ENGINE"):
-                scanner.search_and_move("=")
+        while not scanner.is_finish and not scanner.search_one_type_str(";"):
+            if scanner.search_and_move_one_type_str_use_upper("ENGINE"):
+                scanner.search_and_move_one_type_str("=")
                 engine = scanner.pop_as_source()
-            elif scanner.search_and_move("AUTO_INCREMENT"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("AUTO_INCREMENT"):
+                scanner.search_and_move_one_type_str("=")
                 auto_increment = int(scanner.pop_as_source())
-            elif scanner.search_and_move("DEFAULT", "CHARSET"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_two_type_str_use_upper("DEFAULT", "CHARSET"):
+                scanner.search_and_move_one_type_str("=")
                 default_charset = scanner.pop_as_source()
-            elif scanner.search_and_move("ROW_FORMAT"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("ROW_FORMAT"):
+                scanner.search_and_move_one_type_str("=")
                 row_format = scanner.pop_as_source()
-            elif scanner.search_and_move("COLLATE"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("COLLATE"):
+                scanner.search_and_move_one_type_str("=")
                 collate = scanner.pop_as_source()
-            elif scanner.search_and_move("COMMENT"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("COMMENT"):
+                scanner.search_and_move_one_type_str("=")
                 comment = scanner.pop_as_source()
-            elif scanner.search_and_move("STATS_PERSISTENT"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("STATS_PERSISTENT"):
+                scanner.search_and_move_one_type_str("=")
                 states_persistent = scanner.pop_as_source()
-            elif scanner.search_and_move("PARTITIONED", "BY"):
+            elif scanner.search_and_move_two_type_str_use_upper("PARTITIONED", "BY"):
                 for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-                    partitioned_by.append(cls.parse_define_column_expression(group_scanner, sql_type=sql_type))
+                    partitioned_by.append(cls._parse_define_column_expression(group_scanner, sql_type))
                     group_scanner.close()
-            elif scanner.search_and_move("ROW", "FORMAT", "SERDE"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_three_type_str_use_upper("ROW", "FORMAT", "SERDE"):
+                scanner.search_and_move_one_type_str("=")
                 row_format_serde = scanner.pop_as_source()
             elif scanner.search_and_move("ROW", "FORMAT", "DELIMITED", "FIELDS", "TERMINATED", "BY"):
-                scanner.search_and_move("=")
+                scanner.search_and_move_one_type_str("=")
                 row_format_delimited_fields_terminated_by = scanner.pop_as_source()
-            elif scanner.search_and_move("STORED", "AS", "INPUTFORMAT"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_three_type_str_use_upper("STORED", "AS", "INPUTFORMAT"):
+                scanner.search_and_move_one_type_str("=")
                 stored_as_inputformat = scanner.pop_as_source()
-            elif scanner.search_and_move("STORED", "AS", "TEXTFILE"):
+            elif scanner.search_and_move_three_type_str_use_upper("STORED", "AS", "TEXTFILE"):
                 stored_as_textfile = True
-            elif scanner.search_and_move("OUTPUTFORMAT"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("OUTPUTFORMAT"):
+                scanner.search_and_move_one_type_str("=")
                 outputformat = scanner.pop_as_source()
-            elif scanner.search_and_move("LOCATION"):
-                scanner.search_and_move("=")
+            elif scanner.search_and_move_one_type_str_use_upper("LOCATION"):
+                scanner.search_and_move_one_type_str("=")
                 location = scanner.pop_as_source()
-            elif scanner.search_and_move("TBLPROPERTIES"):
+            elif scanner.search_and_move_one_type_str_use_upper("TBLPROPERTIES"):
                 for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-                    tblproperties.append(cls.parse_config_string_expression(group_scanner, sql_type=sql_type))
+                    tblproperties.append(cls._parse_config_string_expression(group_scanner))
                     group_scanner.close()
             else:
                 raise SqlParseError(f"未知的 DDL 表属性: {scanner}")
-        scanner.search_and_move(";")
+        scanner.search_and_move_one_type_str(";")
 
         return node.ASTCreateTableStatement(
             table_name=table_name,
             comment=comment,
             if_not_exists=if_not_exists,
             columns=tuple(columns),
             primary_key=primary_key,
@@ -1819,247 +1999,362 @@
             stored_as_textfile=stored_as_textfile,
             outputformat=outputformat,
             location=location,
             tblproperties=tuple(tblproperties)
         )
 
     @classmethod
-    def parse_drop_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_drop_table_statement(cls, scanner_or_string: ScannerOrString,
                                    sql_type: SQLType = SQLType.DEFAULT) -> node.ASTDropTableStatement:
         """解析 DROP TABLE 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_drop_table_statement(scanner)
+
+    @classmethod
+    def _parse_drop_table_statement(cls, scanner: TokenScanner) -> node.ASTDropTableStatement:
         scanner.match("DROP", "TABLE")
-        if_exists = scanner.search_and_move("IF", "EXISTS")
-        table_name = cls.parse_table_name_expression(scanner, sql_type=sql_type)
+        if_exists = scanner.search_and_move_two_type_str_use_upper("IF", "EXISTS")
+        table_name = cls._parse_table_name_expression(scanner)
         return node.ASTDropTableStatement(if_exists=if_exists, table_name=table_name)
 
     @classmethod
-    def parse_analyze_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_analyze_table_statement(cls, scanner_or_string: ScannerOrString,
                                       sql_type: SQLType = SQLType.DEFAULT) -> node.ASTAnalyzeTableStatement:
         """解析 ANALYZE TABLE 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_analyze_table_statement(scanner, sql_type)
+
+    @classmethod
+    def _parse_analyze_table_statement(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTAnalyzeTableStatement:
         scanner.match("ANALYZE", "TABLE")
-        table_name = cls.parse_table_name_expression(scanner, sql_type=sql_type)
+        table_name = cls._parse_table_name_expression(scanner)
 
-        if cls.check_partition_expression(scanner, sql_type=sql_type):
-            partition = cls.parse_partition_expression(scanner, sql_type=sql_type)
+        if scanner.search_one_type_str_use_upper("PARTITION"):
+            partition = cls._parse_partition_expression(scanner, False, sql_type)
         else:
             partition = None
 
-        scanner.search_and_move("COMPUTE", "STATISTICS")  # [Hive]
-        for_columns = scanner.search_and_move("FOR", "COLUMNS")  # [Hive]
-        cache_metadata = scanner.search_and_move("CACHE", "METADATA")  # [Hive]
-        noscan = scanner.search_and_move("NOSCAN")  # [Hive]
+        scanner.search_and_move_two_type_str_use_upper("COMPUTE", "STATISTICS")  # [Hive]
+        for_columns = scanner.search_and_move_two_type_str_use_upper("FOR", "COLUMNS")  # [Hive]
+        cache_metadata = scanner.search_and_move_two_type_str_use_upper("CACHE", "METADATA")  # [Hive]
+        noscan = scanner.search_and_move_one_type_str_use_upper("NOSCAN")  # [Hive]
 
         return node.ASTAnalyzeTableStatement(
             table_name=table_name,
             partition=partition,
             for_columns=for_columns,
             cache_metadata=cache_metadata,
             noscan=noscan
         )
 
     @classmethod
-    def parse_type_column_or_index(cls, scanner_or_string: Union[TokenScanner, str],
-                                   sql_type: SQLType = SQLType.DEFAULT) -> node.AliasColumnOrIndex:
+    def parse_column_or_index(cls, scanner_or_string: ScannerOrString,
+                              sql_type: SQLType = SQLType.DEFAULT) -> node.AliasColumnOrIndex:
         """解析字段声明表达式或索引声明表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if cls.check_primary_index_expression(scanner, sql_type=sql_type):
-            return cls.parse_primary_index_expression(scanner, sql_type=sql_type)
-        if cls.check_unique_index_expression(scanner, sql_type=sql_type):
-            return cls.parse_unique_index_expression(scanner, sql_type=sql_type)
-        if cls.check_normal_index_expression(scanner, sql_type=sql_type):
-            return cls.parse_normal_index_expression(scanner, sql_type=sql_type)
-        if cls.check_fulltext_expression(scanner, sql_type=sql_type):
-            return cls.parse_fulltext_expression(scanner, sql_type=sql_type)
-        if cls.check_foreign_key_expression(scanner, sql_type=sql_type):
-            return cls.parse_foreign_key_expression(scanner, sql_type=sql_type)
-        return cls.parse_define_column_expression(scanner, sql_type=sql_type)
+        return cls._parse_column_or_index(scanner, sql_type)
 
     @classmethod
-    def parse_alter_expression(cls, scanner_or_string: Union[TokenScanner, str],
-                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTAlterExpressionBase:
-        # pylint: disable=R0911
-        """解析 ALTER TABLE 的子句表达式
+    def _parse_column_or_index(cls, scanner: TokenScanner, sql_type: SQLType) -> node.AliasColumnOrIndex:
+        if scanner.search_two_type_str_use_upper("PRIMARY", "KEY"):
+            return cls._parse_primary_index_expression(scanner)
+        if scanner.search_two_type_str_use_upper("UNIQUE", "KEY"):
+            return cls._parse_unique_index_expression(scanner)
+        if scanner.search_one_type_str_use_upper("KEY"):
+            return cls._parse_normal_index_expression(scanner)
+        if scanner.search_two_type_str_use_upper("FULLTEXT", "KEY"):
+            return cls._parse_fulltext_expression(scanner)
+        if scanner.search_one_type_str_use_upper("CONSTRAINT"):
+            return cls._parse_foreign_key_expression(scanner)
+        return cls._parse_define_column_expression(scanner, sql_type)
 
-        TODO 优化 PARTITION 的解析逻辑，将 search 和 match 合并为 1 个
-        """
+    @classmethod
+    def parse_alter_expression(cls, scanner_or_string: ScannerOrString,
+                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTAlterExpressionBase:
+        """解析 ALTER TABLE 的子句表达式"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        if scanner.search_and_move("ADD"):
+        return cls._parse_alter_expression(scanner, sql_type)
+
+    @classmethod
+    def _parse_alter_expression(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTAlterExpressionBase:
+        # pylint: disable=R0911
+        if scanner.search_and_move_one_type_str_use_upper("ADD"):
             return node.ASTAlterAddExpression(
-                expression=cls.parse_type_column_or_index(scanner, sql_type=sql_type)
+                expression=cls._parse_column_or_index(scanner, sql_type)
             )
-        if scanner.search_and_move("MODIFY"):
+        if scanner.search_and_move_one_type_str_use_upper("MODIFY"):
             return node.ASTAlterModifyExpression(
-                expression=cls.parse_type_column_or_index(scanner, sql_type=sql_type)
+                expression=cls._parse_column_or_index(scanner, sql_type)
             )
-        if scanner.search_and_move("CHANGE"):
-            from_column_name = unify_name(scanner.pop_as_source())
-            to_expression = cls.parse_type_column_or_index(scanner, sql_type=sql_type)
+        if scanner.search_and_move_one_type_str_use_upper("CHANGE"):
+            from_column_name = cls._unify_name(scanner.pop_as_source())
+            to_expression = cls._parse_column_or_index(scanner, sql_type)
             return node.ASTAlterChangeExpression(
                 from_column_name=from_column_name,
                 to_expression=to_expression
             )
-        if scanner.search_and_move("RENAME", "COLUMN"):
-            from_column_name = unify_name(scanner.pop_as_source())
+        if scanner.search_and_move_two_type_str_use_upper("RENAME", "COLUMN"):
+            from_column_name = cls._unify_name(scanner.pop_as_source())
             scanner.match("TO")
-            to_column_name = unify_name(scanner.pop_as_source())
+            to_column_name = cls._unify_name(scanner.pop_as_source())
             return node.ASTAlterRenameColumnExpression(
                 from_column_name=from_column_name,
                 to_column_name=to_column_name
             )
-        if scanner.search_and_move("DROP", "COLUMN"):
+        if scanner.search_and_move_two_type_str_use_upper("DROP", "COLUMN"):
             return node.ASTAlterDropColumnExpression(
-                column_name=unify_name(scanner.pop_as_source())
+                column_name=cls._unify_name(scanner.pop_as_source())
             )
-        if scanner.search("DROP", "PARTITION"):
-            scanner.match("DROP")
+        if scanner.search_and_move_two_type_str_use_upper("DROP", "PARTITION"):
             return node.ASTAlterDropPartitionExpression(
                 if_exists=False,
-                partition=cls.parse_partition_expression(scanner, sql_type=sql_type)
+                partition=cls._parse_partition_expression(scanner, True, sql_type)
             )
-        if scanner.search("DROP", "IF", "EXISTS", "PARTITION"):
-            scanner.match("DROP", "IF", "EXISTS")
+        if scanner.search_and_move("DROP", "IF", "EXISTS", "PARTITION"):
             return node.ASTAlterDropPartitionExpression(
                 if_exists=True,
-                partition=cls.parse_partition_expression(scanner, sql_type=sql_type)
+                partition=cls._parse_partition_expression(scanner, True, sql_type)
             )
         raise SqlParseError(f"未知的 ALTER TABLE 类型: {scanner}")
 
     @classmethod
-    def check_alter_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                                    sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 ALTER TABLE 语句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("ALTER", "TABLE")
-
-    @classmethod
-    def parse_alter_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_alter_table_statement(cls, scanner_or_string: ScannerOrString,
                                     sql_type: SQLType = SQLType.DEFAULT) -> node.ASTAlterTableStatement:
         """解析 ALTER TABLE 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_alter_table_statement(scanner, sql_type)
+
+    @classmethod
+    def _parse_alter_table_statement(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTAlterTableStatement:
         scanner.match("ALTER", "TABLE")
-        table_name = cls.parse_table_name_expression(scanner, sql_type=sql_type)
-        expressions = [cls.parse_alter_expression(scanner, sql_type=sql_type)]
-        while scanner.search_and_move(","):
-            expressions.append(cls.parse_alter_expression(scanner, sql_type=sql_type))
+        table_name = cls._parse_table_name_expression(scanner)
+        expressions = [cls._parse_alter_expression(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            expressions.append(cls._parse_alter_expression(scanner, sql_type))
         return node.ASTAlterTableStatement(
             table_name=table_name,
             expressions=tuple(expressions)
         )
 
     @classmethod
-    def check_msck_repair_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                                          sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 MSCK REPAIR 语句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("MSCK", "REPAIR", "TABLE")
-
-    @classmethod
-    def parse_msck_repair_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_msck_repair_table_statement(cls, scanner_or_string: ScannerOrString,
                                           sql_type: SQLType = SQLType.DEFAULT) -> node.ASTMsckRepairTableStatement:
         """解析 MSCK REPAIR 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_msck_repair_table_statement(scanner)
+
+    @classmethod
+    def _parse_msck_repair_table_statement(cls, scanner: TokenScanner) -> node.ASTMsckRepairTableStatement:
         scanner.match("MSCK", "REPAIR", "TABLE")
-        table_name = cls.parse_table_name_expression(scanner, sql_type=sql_type)
+        table_name = cls._parse_table_name_expression(scanner)
         return node.ASTMsckRepairTableStatement(
             table_name=table_name
         )
 
     @classmethod
-    def check_use_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                            sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 USE 语句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("USE")
-
-    @classmethod
-    def parse_use_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_use_statement(cls, scanner_or_string: ScannerOrString,
                             sql_type: SQLType = SQLType.DEFAULT) -> node.ASTUseStatement:
         """解析 USE 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_use_statement(scanner)
+
+    @classmethod
+    def _parse_use_statement(cls, scanner: TokenScanner) -> node.ASTUseStatement:
         scanner.match("USE")
         return node.ASTUseStatement(
             schema_name=scanner.pop_as_source()
         )
 
     @classmethod
-    def check_truncate_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
-                                       sql_type: SQLType = SQLType.DEFAULT) -> bool:
-        """判断是否为 TRUNCATE TABLE 语句"""
-        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
-        return scanner.search("TRUNCATE", "TABLE")
-
-    @classmethod
-    def parse_truncate_table_statement(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_truncate_table_statement(cls, scanner_or_string: ScannerOrString,
                                        sql_type: SQLType = SQLType.DEFAULT) -> node.ASTTruncateTable:
         """解析 TRUNCATE TABLE 语句"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_truncate_table_statement(scanner)
+
+    @classmethod
+    def _parse_truncate_table_statement(cls, scanner: TokenScanner) -> node.ASTTruncateTable:
         scanner.match("TRUNCATE", "TABLE")
-        table_name = cls.parse_table_name_expression(scanner)
+        table_name = cls._parse_table_name_expression(scanner)
         return node.ASTTruncateTable(
             table_name=table_name
         )
 
     @classmethod
-    def parse_statements(cls, scanner_or_string: Union[TokenScanner, str],
+    def parse_update_set_column(cls, scanner_or_string: ScannerOrString,
+                                sql_type: SQLType = SQLType.DEFAULT) -> node.ASTUpdateSetColumn:
+        """解析 UPDATE 语句中 SET 中的字段元素"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_update_set_column(scanner, sql_type)
+
+    @classmethod
+    def _parse_update_set_column(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTUpdateSetColumn:
+        column_name = scanner.pop_as_source()
+        scanner.match("=")
+        column_value = cls._parse_logical_or_level_expression(scanner, sql_type)
+        return node.ASTUpdateSetColumn(
+            column_name=column_name,
+            column_value=column_value
+        )
+
+    @classmethod
+    def parse_update_set_clause(cls, scanner_or_string: ScannerOrString,
+                                sql_type: SQLType = SQLType.DEFAULT) -> node.ASTUpdateSetClause:
+        """解析 UPDATE 语句的 SET 子句"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_update_set_clause(scanner, sql_type)
+
+    @classmethod
+    def _parse_update_set_clause(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTUpdateSetClause:
+        scanner.match("SET")
+        columns = [cls._parse_update_set_column(scanner, sql_type)]
+        while scanner.search_and_move_one_type_str(","):
+            columns.append(cls._parse_update_set_column(scanner, sql_type))
+        return node.ASTUpdateSetClause(
+            columns=tuple(columns)
+        )
+
+    @classmethod
+    def parse_update_statement(cls, scanner_or_string: ScannerOrString,
+                               with_clause: Optional[node.ASTWithClause],
+                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTUpdateStatement:
+        """解析 UPDATE 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_update_statement(scanner, with_clause, sql_type)
+
+    @classmethod
+    def _parse_update_statement(cls, scanner: TokenScanner,
+                                with_clause: Optional[node.ASTWithClause],
+                                sql_type: SQLType) -> node.ASTUpdateStatement:
+        scanner.match("UPDATE")
+        table_name = cls._parse_table_name_expression(scanner)
+        set_clause = cls._parse_update_set_clause(scanner, sql_type)
+        where_clause = cls._parse_where_clause(scanner, sql_type)
+        order_by_clause = cls._parse_order_by_clause(scanner, sql_type)
+        limit_clause = cls._parse_limit_clause(scanner)
+        return node.ASTUpdateStatement(
+            with_clause=with_clause,
+            table_name=table_name,
+            set_clause=set_clause,
+            where_clause=where_clause,
+            order_by_clause=order_by_clause,
+            limit_clause=limit_clause
+        )
+
+    @classmethod
+    def parse_delete_statement(cls, scanner_or_string: ScannerOrString,
+                               sql_type: SQLType = SQLType.DEFAULT) -> node.ASTDeleteStatement:
+        """解析 UPDATE 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_delete_statement(scanner, sql_type)
+
+    @classmethod
+    def _parse_delete_statement(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTDeleteStatement:
+        scanner.match("DELETE", "FROM")
+        table_name = cls._parse_table_name_expression(scanner)
+        where_clause = cls._parse_where_clause(scanner, sql_type)
+        order_by_clause = cls._parse_order_by_clause(scanner, sql_type)
+        limit_clause = cls._parse_limit_clause(scanner)
+        return node.ASTDeleteStatement(
+            table_name=table_name,
+            where_clause=where_clause,
+            order_by_clause=order_by_clause,
+            limit_clause=limit_clause
+        )
+
+    @classmethod
+    def parse_show_columns_statement(cls, scanner_or_string: ScannerOrString,
+                                     sql_type: SQLType = SQLType.DEFAULT) -> node.ASTShowColumnsStatement:
+        """解析 SHOW COLUMNS 语句"""
+        scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
+        return cls._parse_show_columns_statement(scanner, sql_type)
+
+    @classmethod
+    def _parse_show_columns_statement(cls, scanner: TokenScanner, sql_type: SQLType) -> node.ASTShowColumnsStatement:
+        scanner.match("SHOW", "COLUMNS")
+        from_clause = cls._parse_from_clause(scanner, sql_type)
+        where_clause = cls._parse_where_clause(scanner, sql_type)
+        return node.ASTShowColumnsStatement(
+            from_clause=from_clause,
+            where_clause=where_clause
+        )
+
+    @classmethod
+    def parse_statements(cls, scanner_or_string: ScannerOrString,
                          sql_type: SQLType = SQLType.DEFAULT) -> List[node.ASTStatementBase]:
         # pylint: disable=R0912
         """解析一段 SQL 语句，返回表达式的列表"""
         scanner = cls._unify_input_scanner(scanner_or_string, sql_type=sql_type)
         statement_list = []
         while not scanner.is_finish:
             # 解析 SET 语句
-            if cls.check_set_statement(scanner, sql_type=sql_type):
-                statement_list.append(cls.parse_set_statement(scanner, sql_type=sql_type))
+            if scanner.search_one_type_str_use_upper("SET"):
+                statement_list.append(cls._parse_set_statement(scanner))
+
+            # 解析 DELETE 语句
+            elif scanner.search_two_type_str_use_upper("DELETE", "FROM"):
+                statement_list.append(cls._parse_delete_statement(scanner, sql_type))
 
             # 解析 DROP TABLE 语句
-            elif scanner.search("DROP", "TABLE"):
-                statement_list.append(cls.parse_drop_table_statement(scanner, sql_type=sql_type))
+            elif scanner.search_two_type_str_use_upper("DROP", "TABLE"):
+                statement_list.append(cls._parse_drop_table_statement(scanner))
 
             # 解析 CREATE TABLE 语句
-            elif scanner.search("CREATE", "TABLE"):
-                statement_list.append(cls.parse_create_table_statement(scanner, sql_type=sql_type))
+            elif scanner.search_two_type_str_use_upper("CREATE", "TABLE"):
+                statement_list.append(cls._parse_create_table_statement(scanner, sql_type))
 
             # 解析 ANALYZE TABLE 语句
-            elif scanner.search("ANALYZE", "TABLE"):
-                statement_list.append(cls.parse_analyze_table_statement(scanner, sql_type=sql_type))
+            elif scanner.search_two_type_str_use_upper("ANALYZE", "TABLE"):
+                statement_list.append(cls._parse_analyze_table_statement(scanner, sql_type))
 
             # 解析 ALTER TABLE 语句
-            elif cls.check_alter_table_statement(scanner, sql_type=sql_type):
-                statement_list.append(cls.parse_alter_table_statement(scanner, sql_type=sql_type))
+            elif scanner.search_two_type_str_use_upper("ALTER", "TABLE"):
+                statement_list.append(cls._parse_alter_table_statement(scanner, sql_type))
 
             # 解析 MSCK REPAIR TABLE 语句
-            elif cls.check_msck_repair_table_statement(scanner, sql_type=sql_type):
-                statement_list.append(cls.parse_msck_repair_table_statement(scanner, sql_type=sql_type))
+            elif scanner.search_three_type_str_use_upper("MSCK", "REPAIR", "TABLE"):
+                statement_list.append(cls._parse_msck_repair_table_statement(scanner))
 
             # 解析 USE 语句
-            elif cls.check_use_statement(scanner, sql_type=sql_type):
-                statement_list.append(cls.parse_use_statement(scanner, sql_type=sql_type))
+            elif scanner.search_one_type_str_use_upper("USE"):
+                statement_list.append(cls._parse_use_statement(scanner))
 
             # 解析 TRUNCATE TABLE 语句
-            elif cls.check_truncate_table_statement(scanner, sql_type=sql_type):
-                statement_list.append(cls.parse_truncate_table_statement(scanner, sql_type=sql_type))
+            elif scanner.search_two_type_str_use_upper("TRUNCATE", "TABLE"):
+                statement_list.append(cls._parse_truncate_table_statement(scanner))
+
+            # 解析 SHOW DATABASES 语句
+            elif scanner.search_and_move_two_type_str_use_upper("SHOW", "DATABASES"):
+                statement_list.append(node.ASTShowDatabasesStatement())
+
+            # 解析 SHOW TABLES 语句
+            elif scanner.search_and_move_two_type_str_use_upper("SHOW", "TABLES"):
+                statement_list.append(node.ASTShowTablesStatement())
+
+            # 解析 SHOW COLUMNS 语句
+            elif scanner.search_and_move_two_type_str_use_upper("SHOW", "COLUMNS"):
+                statement_list.append(cls._parse_show_columns_statement(scanner, sql_type))
 
             else:
                 # 解析可能包含 WITH 子句的语句类型
-                with_clause = cls.parse_with_clause(scanner, sql_type=sql_type)
+                with_clause = cls._parse_with_clause(scanner, sql_type)
+
+                # 解析 SELECT 语句
+                if scanner.search_one_type_str_use_upper("SELECT"):
+                    statement_list.append(cls._parse_select_statement(scanner, with_clause, sql_type))
+
+                # 解析 INSERT 语句
+                elif scanner.search_one_type_str_use_upper("INSERT"):
+                    statement_list.append(cls._parse_insert_statement(scanner, with_clause, sql_type))
+
+                # 解析 UPDATE 语句
+                elif scanner.search_one_type_str_use_upper("UPDATE"):
+                    statement_list.append(cls._parse_update_statement(scanner, with_clause, sql_type))
 
-                if cls.check_select_statement(scanner, sql_type=sql_type):
-                    statement_list.append(cls.parse_select_statement(scanner,
-                                                                     with_clause=with_clause, sql_type=sql_type))
-                elif cls.check_insert_statement(scanner, sql_type=sql_type):
-                    statement_list.append(cls.parse_insert_statement(scanner,
-                                                                     with_clause=with_clause, sql_type=sql_type))
                 else:
                     raise SqlParseError(f"未知语句类型: {scanner}")
 
-            scanner.search_and_move(";")
+            scanner.search_and_move_one_type_str(";")
 
         scanner.close()
 
         return statement_list
-
-
-def unify_name(text: Optional[str]) -> Optional[str]:
-    """格式化名称标识符：统一剔除当前引号并添加引号"""
-    return text.strip("`") if text is not None else None
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_operation_map.py` & `metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_operation_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,290 +1,312 @@
 """
 词法分析有限状态机，针对不同状态、不同输入值的行为映射表
 """
 
-from typing import Dict
+from typing import Dict, Tuple
 
 from metasequoia_sql.common import char_set
+from metasequoia_sql.config import LEXICAL_IGNORE_SPACE, LEXICAL_IGNORE_LINEBREAK, LEXICAL_IGNORE_COMMENT
 from metasequoia_sql.errors import AMTParseError
 from metasequoia_sql.lexical.amt_node import AMTMark
 from metasequoia_sql.lexical.fsm_operate import FSMOperate
 from metasequoia_sql.lexical.fsm_status import FSMStatus
 
-__all__ = ["END", "DEFAULT", "FSM_OPERATION_MAP"]
+__all__ = ["END", "DEFAULT", "FSM_OPERATION_MAP", "FSM_OPERATION_MAP_DEFAULT"]
 
 END = "<end>"  # 结束标识符
 DEFAULT = "<default>"  # 默认标识符
 
 # 行为映射表设置表（用于设置配置信息，输入参数允许是一个不可变集合）
 FSM_OPERATION_MAP_SOURCE = {
     # 等待下一个词语
     FSMStatus.WAIT: {
-        "!": FSMOperate.add_cache(new_status=FSMStatus.AFTER_21),
-        "&": FSMOperate.add_cache(new_status=FSMStatus.AFTER_26),
-        "-": FSMOperate.add_cache(new_status=FSMStatus.AFTER_2D),
-        "/": FSMOperate.add_cache(new_status=FSMStatus.AFTER_2F),
-        "<": FSMOperate.add_cache(new_status=FSMStatus.AFTER_3C),
-        ">": FSMOperate.add_cache(new_status=FSMStatus.AFTER_3E),
-        "|": FSMOperate.add_cache(new_status=FSMStatus.AFTER_7C),
-        "0": FSMOperate.add_cache(new_status=FSMStatus.AFTER_0),
-        frozenset({" ", "\n"}): FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.SPACE}),
-        "*": FSMOperate.add_and_handle_cache_to_wait(marks=set()),
-        frozenset({",", ";", "=", "+", ".", "%"}): FSMOperate.add_and_handle_cache_to_wait(marks=set()),
-        "\"": FSMOperate.add_cache(new_status=FSMStatus.IN_DOUBLE_QUOTE),
-        "'": FSMOperate.add_cache(new_status=FSMStatus.IN_SINGLE_QUOTE),
-        "`": FSMOperate.add_cache(new_status=FSMStatus.IN_BACK_QUOTE),
-        "#": FSMOperate.add_cache(new_status=FSMStatus.IN_EXPLAIN_1),
-        frozenset({"b", "B"}): FSMOperate.add_cache(new_status=FSMStatus.AFTER_B),
-        frozenset({"x", "X"}): FSMOperate.add_cache(new_status=FSMStatus.AFTER_X),
-        char_set.NUMBER: FSMOperate.add_cache(new_status=FSMStatus.IN_INT),
+        "!": FSMOperate.add_cache_to(status=FSMStatus.AFTER_21),
+        "&": FSMOperate.add_cache_to(status=FSMStatus.AFTER_26),
+        "-": FSMOperate.add_cache_to(status=FSMStatus.AFTER_2D),
+        "/": FSMOperate.add_cache_to(status=FSMStatus.AFTER_2F),
+        "<": FSMOperate.add_cache_to(status=FSMStatus.AFTER_3C),
+        ">": FSMOperate.add_cache_to(status=FSMStatus.AFTER_3E),
+        "|": FSMOperate.add_cache_to(status=FSMStatus.AFTER_7C),
+        "0": FSMOperate.add_cache_to(status=FSMStatus.AFTER_0),
+        " ": (FSMOperate.add_and_handle_cache(marks=AMTMark.SPACE)
+              if not LEXICAL_IGNORE_SPACE else FSMOperate.move_and_clean_cache()),
+        "\n": (FSMOperate.add_and_handle_cache(marks=AMTMark.SPACE)
+               if not LEXICAL_IGNORE_LINEBREAK else FSMOperate.move_and_clean_cache()),
+        "~": FSMOperate.add_and_handle_cache(marks=AMTMark.NONE),
+        "*": FSMOperate.add_and_handle_cache(marks=AMTMark.NONE),
+        "^": FSMOperate.add_and_handle_cache(marks=AMTMark.NONE),
+        frozenset({",", ";", "=", "+", ".", "%"}): FSMOperate.add_and_handle_cache(marks=AMTMark.NONE),
+        "\"": FSMOperate.add_cache_to(status=FSMStatus.IN_DOUBLE_QUOTE),
+        "'": FSMOperate.add_cache_to(status=FSMStatus.IN_SINGLE_QUOTE),
+        "`": FSMOperate.add_cache_to(status=FSMStatus.IN_BACK_QUOTE),
+        "#": FSMOperate.add_cache_to(status=FSMStatus.IN_EXPLAIN_1),
+        frozenset({"b", "B"}): FSMOperate.add_cache_to(status=FSMStatus.AFTER_B),
+        frozenset({"x", "X"}): FSMOperate.add_cache_to(status=FSMStatus.AFTER_X),
+        char_set.NUMBER: FSMOperate.add_cache_to(status=FSMStatus.IN_INT),
         "(": FSMOperate.start_parenthesis(),
         ")": FSMOperate.end_parenthesis(),
         "[": FSMOperate.start_slice(),
         "]": FSMOperate.end_slice(),
-        END: FSMOperate.set_status(FSMStatus.END),
-        DEFAULT: FSMOperate.add_cache(FSMStatus.IN_WORD)
+        END: FSMOperate.do_nothing_to_end(),
+        DEFAULT: FSMOperate.add_cache_to(FSMStatus.IN_WORD)
     },
 
     # 在 ! 符号之后
     FSMStatus.AFTER_21: {
-        "=": FSMOperate.add_and_handle_cache_to_wait(marks=set()),  # 符号：!=
+        "=": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：!=
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set()),  # 符号：!
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：!
     },
 
     # 在 & 符号之后
     FSMStatus.AFTER_26: {
+        "&": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：&&
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set()),  # 符号：&
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：&
     },
 
     # 在 - 符号之后
     FSMStatus.AFTER_2D: {
-        "-": FSMOperate.add_cache(new_status=FSMStatus.IN_EXPLAIN_1),  # 符号：--
+        "-": FSMOperate.add_cache_to(status=FSMStatus.IN_EXPLAIN_1),  # 符号：--
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set())
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE)
     },
 
     # 在 / 符号之后
     FSMStatus.AFTER_2F: {
-        "*": FSMOperate.add_cache(new_status=FSMStatus.IN_EXPLAIN_2),  # 符号：/*
+        "*": FSMOperate.add_cache_to(status=FSMStatus.IN_EXPLAIN_2),  # 符号：/*
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set())
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE)
     },
 
     # 在 < 符号之后
     FSMStatus.AFTER_3C: {
-        "=": FSMOperate.add_cache(new_status=FSMStatus.AFTER_3C_3D),  # 符号：<=
-        ">": FSMOperate.add_and_handle_cache_to_wait(marks=set()),  # 符号：<>
+        "=": FSMOperate.add_cache_to(status=FSMStatus.AFTER_3C_3D),  # 符号：<=
+        ">": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：<>
+        "<": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：<<
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set())  # 符号：<
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE)  # 符号：<
     },
 
     # 在 < 符号之后
     FSMStatus.AFTER_3C_3D: {
-        ">": FSMOperate.add_and_handle_cache_to_wait(marks=set()),  # 符号：<=>
+        ">": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：<=>
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set())  # 符号：<=
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE)  # 符号：<=
     },
 
     # 在 > 符号之后
     FSMStatus.AFTER_3E: {
-        "=": FSMOperate.add_and_handle_cache_to_wait(marks=set()),  # 符号：>=
+        "=": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：>=
+        ">": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：>>
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks=set())  # 符号：>
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE)  # 符号：>
     },
 
     # 在 | 符号之后
     FSMStatus.AFTER_7C: {
-        "|": FSMOperate.add_and_handle_cache_to_wait(marks=set()),  # 符号：||
+        "|": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：||
+        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks=AMTMark.NONE),  # 符号：|
         END: FSMOperate.raise_error(),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在 0 之后
     FSMStatus.AFTER_0: {
-        "x": FSMOperate.add_cache(new_status=FSMStatus.IN_HEX_LITERAL_AFTER_0X),  # "0x" 开头的十六进制字面值
-        "b": FSMOperate.add_cache(new_status=FSMStatus.IN_BIT_LITERAL_AFTER_0B),  # "0b" 开头的位值字面值
-        ".": FSMOperate.add_cache(new_status=FSMStatus.IN_FLOAT),  # "0." 开头的浮点数
-        char_set.NUMBER: FSMOperate.add_cache(new_status=FSMStatus.IN_INT),  # "0+整数" 开头的整数
-        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_INT}),  # 0
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.LITERAL_INT}),  # 0
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_WORD)
+        "x": FSMOperate.add_cache_to(status=FSMStatus.IN_HEX_LITERAL_AFTER_0X),  # "0x" 开头的十六进制字面值
+        "b": FSMOperate.add_cache_to(status=FSMStatus.IN_BIT_LITERAL_AFTER_0B),  # "0b" 开头的位值字面值
+        ".": FSMOperate.add_cache_to(status=FSMStatus.IN_FLOAT),  # "0." 开头的浮点数
+        char_set.NUMBER: FSMOperate.add_cache_to(status=FSMStatus.IN_INT),  # "0+整数" 开头的整数
+        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_INT),  # 0
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.LITERAL_INT),  # 0
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_WORD)
     },
 
     # 在 b 或 B 之后
     FSMStatus.AFTER_B: {
-        "\"": FSMOperate.add_cache(new_status=FSMStatus.IN_BIT_LITERAL_OF_DOUBLE_QUOTE),  # 位值字面值
-        "'": FSMOperate.add_cache(new_status=FSMStatus.IN_BIT_LITERAL_OF_SINGLE_QUOTE),  # 位值字面值
+        "\"": FSMOperate.add_cache_to(status=FSMStatus.IN_BIT_LITERAL_OF_DOUBLE_QUOTE),  # 位值字面值
+        "'": FSMOperate.add_cache_to(status=FSMStatus.IN_BIT_LITERAL_OF_SINGLE_QUOTE),  # 位值字面值
         ".": FSMOperate.handle_cache_word_to_wait(),
-        char_set.END_TOKEN_WITHOUT_QUOTE: FSMOperate.handle_cache_to_wait(marks={AMTMark.NAME}),  # b 或 B
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.NAME}),  # b 或 B
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_WORD)
+        char_set.END_TOKEN_WITHOUT_QUOTE: FSMOperate.handle_cache_to_wait(marks=AMTMark.NAME),  # b 或 B
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.NAME),  # b 或 B
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_WORD)
     },
 
     # 在 x 或 X 之后
     FSMStatus.AFTER_X: {
-        "\"": FSMOperate.add_cache(new_status=FSMStatus.IN_HEX_LITERAL_OF_DOUBLE_QUOTE),  # 十六进制字面值
-        "'": FSMOperate.add_cache(new_status=FSMStatus.IN_HEX_LITERAL_OF_SINGLE_QUOTE),  # 十六进制字面值
+        "\"": FSMOperate.add_cache_to(status=FSMStatus.IN_HEX_LITERAL_OF_DOUBLE_QUOTE),  # 十六进制字面值
+        "'": FSMOperate.add_cache_to(status=FSMStatus.IN_HEX_LITERAL_OF_SINGLE_QUOTE),  # 十六进制字面值
         ".": FSMOperate.handle_cache_word_to_wait(),
-        char_set.END_TOKEN_WITHOUT_QUOTE: FSMOperate.handle_cache_to_wait(marks={AMTMark.NAME}),  # x 或 X
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.NAME}),  # x 或 X
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_WORD)
+        char_set.END_TOKEN_WITHOUT_QUOTE: FSMOperate.handle_cache_to_wait(marks=AMTMark.NAME),  # x 或 X
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.NAME),  # x 或 X
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_WORD)
     },
 
     # 在十六机制字面值的双引号中
     FSMStatus.IN_HEX_LITERAL_OF_DOUBLE_QUOTE: {
-        "\"": FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_HEX}),
-        char_set.HEX_LITERAL: FSMOperate.add_cache(new_status=FSMStatus.IN_HEX_LITERAL_OF_DOUBLE_QUOTE),
+        "\"": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_HEX),
+        char_set.HEX_LITERAL: FSMOperate.add_cache_to(status=FSMStatus.IN_HEX_LITERAL_OF_DOUBLE_QUOTE),
         END: FSMOperate.raise_error(),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在十六进制字面值的单引号中
     FSMStatus.IN_HEX_LITERAL_OF_SINGLE_QUOTE: {
-        "'": FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_HEX}),
-        char_set.HEX_LITERAL: FSMOperate.add_cache(new_status=FSMStatus.IN_HEX_LITERAL_OF_SINGLE_QUOTE),
+        "'": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_HEX),
+        char_set.HEX_LITERAL: FSMOperate.add_cache_to(status=FSMStatus.IN_HEX_LITERAL_OF_SINGLE_QUOTE),
         END: FSMOperate.raise_error(),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在 0x 开头的十六进制字面值中，例如：0x2F
     FSMStatus.IN_HEX_LITERAL_AFTER_0X: {
-        char_set.HEX_LITERAL: FSMOperate.add_cache(new_status=FSMStatus.IN_HEX_LITERAL_AFTER_0X),
-        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_HEX}),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.LITERAL_HEX}),
+        char_set.HEX_LITERAL: FSMOperate.add_cache_to(status=FSMStatus.IN_HEX_LITERAL_AFTER_0X),
+        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_HEX),
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.LITERAL_HEX),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在二进制字面值的双引号中
     FSMStatus.IN_BIT_LITERAL_OF_DOUBLE_QUOTE: {
-        "\"": FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_BIT}),
-        char_set.BIT_LITERAL: FSMOperate.add_cache(new_status=FSMStatus.IN_BIT_LITERAL_OF_DOUBLE_QUOTE),
+        "\"": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_BIT),
+        char_set.BIT_LITERAL: FSMOperate.add_cache_to(status=FSMStatus.IN_BIT_LITERAL_OF_DOUBLE_QUOTE),
         END: FSMOperate.raise_error(),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在二进制字面值的单引号中
     FSMStatus.IN_BIT_LITERAL_OF_SINGLE_QUOTE: {
-        "'": FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_BIT}),
-        char_set.BIT_LITERAL: FSMOperate.add_cache(new_status=FSMStatus.IN_BIT_LITERAL_OF_SINGLE_QUOTE),
+        "'": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_BIT),
+        char_set.BIT_LITERAL: FSMOperate.add_cache_to(status=FSMStatus.IN_BIT_LITERAL_OF_SINGLE_QUOTE),
         END: FSMOperate.raise_error(),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在 0b 开头的位值字面值中，例如：0b01
     FSMStatus.IN_BIT_LITERAL_AFTER_0B: {
-        char_set.BIT_LITERAL: FSMOperate.add_cache(new_status=FSMStatus.IN_BIT_LITERAL_AFTER_0B),
-        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_BIT}),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.LITERAL_BIT}),
+        char_set.BIT_LITERAL: FSMOperate.add_cache_to(status=FSMStatus.IN_BIT_LITERAL_AFTER_0B),
+        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_BIT),
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.LITERAL_BIT),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在整型中，例如：25
     FSMStatus.IN_INT: {
-        ".": FSMOperate.add_cache(new_status=FSMStatus.IN_FLOAT),
-        char_set.NUMBER: FSMOperate.add_cache(new_status=FSMStatus.IN_INT),
-        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_INT}),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.LITERAL_INT}),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_WORD),
+        ".": FSMOperate.add_cache_to(status=FSMStatus.IN_FLOAT),
+        char_set.NUMBER: FSMOperate.add_cache_to(status=FSMStatus.IN_INT),
+        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_INT),
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.LITERAL_INT),
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_WORD),
     },
 
     # 在浮点数中
     FSMStatus.IN_FLOAT: {
-        char_set.NUMBER: FSMOperate.add_cache(new_status=FSMStatus.IN_FLOAT),
-        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.LITERAL_FLOAT}),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.LITERAL_FLOAT}),
+        char_set.NUMBER: FSMOperate.add_cache_to(status=FSMStatus.IN_FLOAT),
+        char_set.END_TOKEN: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.LITERAL_FLOAT),
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.LITERAL_FLOAT),
         DEFAULT: FSMOperate.raise_error()
     },
 
     # 在双引号中
     FSMStatus.IN_DOUBLE_QUOTE: {
-        "\\": FSMOperate.add_cache(new_status=FSMStatus.IN_DOUBLE_QUOTE_AFTER_5C),
-        "\"": FSMOperate.add_cache(new_status=FSMStatus.IN_DOUBLE_QUOTE_AFTER_22),
+        "\\": FSMOperate.add_cache_to(status=FSMStatus.IN_DOUBLE_QUOTE_AFTER_5C),
+        "\"": FSMOperate.add_cache_to(status=FSMStatus.IN_DOUBLE_QUOTE_AFTER_22),
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_DOUBLE_QUOTE)
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_DOUBLE_QUOTE)
     },
 
     # 在双引号中的、的 \" 符号之后
     FSMStatus.IN_DOUBLE_QUOTE_AFTER_22: {
-        "\"": FSMOperate.add_cache(new_status=FSMStatus.IN_DOUBLE_QUOTE),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.NAME}),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.NAME})
+        "\"": FSMOperate.add_cache_to(status=FSMStatus.IN_DOUBLE_QUOTE),
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.NAME),
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.NAME)
     },
 
     # 在双引号中的 \\ 符号之后
     FSMStatus.IN_DOUBLE_QUOTE_AFTER_5C: {
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(FSMStatus.IN_DOUBLE_QUOTE)
+        DEFAULT: FSMOperate.add_cache_to(FSMStatus.IN_DOUBLE_QUOTE)
     },
 
     # 在单引号中
     FSMStatus.IN_SINGLE_QUOTE: {
-        "\\": FSMOperate.add_cache(new_status=FSMStatus.IN_SINGLE_QUOTE_AFTER_5C),
-        "'": FSMOperate.add_cache(new_status=FSMStatus.IN_SINGLE_QUOTE_AFTER_27),
+        "\\": FSMOperate.add_cache_to(status=FSMStatus.IN_SINGLE_QUOTE_AFTER_5C),
+        "'": FSMOperate.add_cache_to(status=FSMStatus.IN_SINGLE_QUOTE_AFTER_27),
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_SINGLE_QUOTE)
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_SINGLE_QUOTE)
     },
 
     # 在单引号中的、的 ' 符号之后
     FSMStatus.IN_SINGLE_QUOTE_AFTER_27: {
-        "'": FSMOperate.add_cache(new_status=FSMStatus.IN_SINGLE_QUOTE),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.LITERAL, AMTMark.NAME}),
-        DEFAULT: FSMOperate.handle_cache_to_wait(marks={AMTMark.LITERAL, AMTMark.NAME})
+        "'": FSMOperate.add_cache_to(status=FSMStatus.IN_SINGLE_QUOTE),
+        END: FSMOperate.handle_cache_to_end(marks=AMTMark.LITERAL | AMTMark.NAME),
+        DEFAULT: FSMOperate.handle_cache_to_wait(marks=AMTMark.LITERAL | AMTMark.NAME)
     },
 
     # 在单引号中的 \\ 符号之后
     FSMStatus.IN_SINGLE_QUOTE_AFTER_5C: {
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_SINGLE_QUOTE)
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_SINGLE_QUOTE)
     },
 
     # 在反引号中
     FSMStatus.IN_BACK_QUOTE: {
-        "`": FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.NAME}),
+        "`": FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.NAME),
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_BACK_QUOTE)
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_BACK_QUOTE)
     },
 
     # 在 # 或 -- 标记的单行注释中
     FSMStatus.IN_EXPLAIN_1: {
-        "\n": FSMOperate.handle_cache_to_wait(marks={AMTMark.COMMENT}),
-        END: FSMOperate.handle_cache_to_end(marks={AMTMark.COMMENT}),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_EXPLAIN_1)
+        "\n": (FSMOperate.handle_cache_to_wait(marks=AMTMark.COMMENT)
+               if not LEXICAL_IGNORE_COMMENT else FSMOperate.clean_cache_to_wait()),
+        END: (FSMOperate.handle_cache_to_end(marks=AMTMark.COMMENT)
+              if not LEXICAL_IGNORE_COMMENT else FSMOperate.clean_cache_to_end()),
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_EXPLAIN_1)
     },
 
     # 在多行注释中
     FSMStatus.IN_EXPLAIN_2: {
-        "*": FSMOperate.add_cache(FSMStatus.IN_EXPLAIN_2_AFTER_2A),
+        "*": FSMOperate.add_cache_to(FSMStatus.IN_EXPLAIN_2_AFTER_2A),
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(FSMStatus.IN_EXPLAIN_2)
+        DEFAULT: FSMOperate.add_cache_to(FSMStatus.IN_EXPLAIN_2)
     },
 
     # 在多行注释中的 * 符号之后
     FSMStatus.IN_EXPLAIN_2_AFTER_2A: {
-        "/": FSMOperate.add_and_handle_cache_to_wait(marks={AMTMark.COMMENT}),
+        "/": (FSMOperate.add_and_handle_cache_to_wait(marks=AMTMark.COMMENT)
+              if not LEXICAL_IGNORE_COMMENT else FSMOperate.move_and_clean_cache_to_wait()),
         END: FSMOperate.raise_error(),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_EXPLAIN_2)
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_EXPLAIN_2)
     },
 
     # 在普通词语中
     FSMStatus.IN_WORD: {
         ".": FSMOperate.handle_cache_word_to_wait(),
         char_set.END_TOKEN: FSMOperate.handle_cache_word_to_wait(),
         END: FSMOperate.handle_cache_word_to_end(),
-        DEFAULT: FSMOperate.add_cache(new_status=FSMStatus.IN_WORD)
+        DEFAULT: FSMOperate.add_cache_to(status=FSMStatus.IN_WORD)
     }
 }
 
 # 状态行为映射表（用于用时行为映射信息，输入参数必须是一个字符）
-FSM_OPERATION_MAP: Dict[FSMStatus, Dict[str, FSMOperate]] = {}
+FSM_OPERATION_MAP: Dict[Tuple[FSMStatus, str], FSMOperate] = {}
+FSM_OPERATION_MAP_DEFAULT: Dict[FSMStatus, FSMOperate] = {}
 for status, operation_map in FSM_OPERATION_MAP_SOURCE.items():
-    FSM_OPERATION_MAP[status] = {}
+    # 遍历并添加定义的字符到行为映射表中
     for ch_or_set, fsm_operation in operation_map.items():
-        if isinstance(ch_or_set, str):
-            FSM_OPERATION_MAP[status][ch_or_set] = fsm_operation
+        if ch_or_set is DEFAULT:
+            FSM_OPERATION_MAP_DEFAULT[status] = fsm_operation
+        elif isinstance(ch_or_set, str):
+            FSM_OPERATION_MAP[(status, ch_or_set)] = fsm_operation
         elif isinstance(ch_or_set, frozenset):
             for ch in ch_or_set:
-                FSM_OPERATION_MAP[status][ch] = fsm_operation
+                FSM_OPERATION_MAP[(status, ch)] = fsm_operation
         else:
             raise AMTParseError("非法的行为映射表设置表")
+
+    # 将 ASCII 编码 20 - 7E 之间的字符添加到行为映射表中（从而令第一次查询的命中率提高，避免第二次查询）
+    for dec in range(32, 127):
+        ch = chr(dec)
+        if (status, ch) not in FSM_OPERATION_MAP:
+            FSM_OPERATION_MAP[(status, ch)] = FSM_OPERATION_MAP_DEFAULT[status]
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql/lexical/fsm_status.py` & `metasequoia-sql-0.6.0/metasequoia_sql/lexical/fsm_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,62 +3,62 @@
 """
 
 import enum
 
 __all__ = ["FSMStatus"]
 
 
-class FSMStatus(enum.Enum):
+class FSMStatus(enum.IntEnum):
     """词法分析的有限状态机的状态枚举类
 
     其中，FSMStatus.value 为枚举类的含义，用于在抛出异常时显示
     """
-    WAIT = "等待下一个词语"
+    WAIT = 0  # 等待下一个词语
 
     # 能够组成多字符组合的单字符之后
-    AFTER_21 = "在 ! 符号之后"
-    AFTER_26 = "在 & 符号之后"
-    AFTER_2D = "在 - 符号之后"
-    AFTER_2F = "在 / 符号之后"
-    AFTER_3C = "在 < 符号之后"
-    AFTER_3C_3D = "在 <= 符号之后"
-    AFTER_3E = "在 > 符号之后"
-    AFTER_7C = "在 | 符号之后"
-    AFTER_0 = "在 0 之后"
-    AFTER_B = "在 b 或 B 之后"
-    AFTER_X = "在 x 或 X 之后"
+    AFTER_21 = 11  # 在 ! 符号之后
+    AFTER_26 = 12  # 在 & 符号之后
+    AFTER_2D = 13  # 在 - 符号之后
+    AFTER_2F = 14  # 在 / 符号之后
+    AFTER_3C = 15  # 在 < 符号之后
+    AFTER_3C_3D = 16  # 在 <= 符号之后
+    AFTER_3E = 17  # 在 > 符号之后
+    AFTER_7C = 18  # 在 | 符号之后
+    AFTER_0 = 19  # 在 0 之后
+    AFTER_B = 20  # 在 b 或 B 之后
+    AFTER_X = 21  # 在 x 或 X 之后
 
     # 正在匹配特定类型的字符
-    IN_HEX_LITERAL_OF_DOUBLE_QUOTE = "在十六机制字面值的双引号中"
-    IN_HEX_LITERAL_OF_SINGLE_QUOTE = "在十六进制字面值的单引号中"
-    IN_HEX_LITERAL_AFTER_0X = "在0x开头的十六进制字面值中"
-    IN_BIT_LITERAL_OF_DOUBLE_QUOTE = "在二进制字面值的双引号中"
-    IN_BIT_LITERAL_OF_SINGLE_QUOTE = "在二进制字面值的单引号中"
-    IN_BIT_LITERAL_AFTER_0B = "在0b开头的位值字面值中"
-    IN_INT = "在整型中"
-    IN_FLOAT = "在浮点数中"
-    IN_DOUBLE_QUOTE = "在双引号中"
-    IN_DOUBLE_QUOTE_AFTER_22 = "在双引号中的、的 \" 符号之后"
-    IN_DOUBLE_QUOTE_AFTER_5C = "在双引号中的 \\ 符号之后"
-    IN_SINGLE_QUOTE = "在单引号中"
-    IN_SINGLE_QUOTE_AFTER_27 = "在单引号中的、的 ' 符号之后"
-    IN_SINGLE_QUOTE_AFTER_5C = "在单引号中的 \\ 符号之后"
-    IN_BACK_QUOTE = "在反引号中"
-    IN_EXPLAIN_1 = "在 # 或 -- 标记的单行注释中"
-    IN_EXPLAIN_2 = "在多行注释中"
-    IN_EXPLAIN_2_AFTER_2A = "在多行注释中的 * 符号之后"
-    IN_WORD = "在普通词语中"
+    IN_HEX_LITERAL_OF_DOUBLE_QUOTE = 41  # 在十六机制字面值的双引号中
+    IN_HEX_LITERAL_OF_SINGLE_QUOTE = 42  # 在十六进制字面值的单引号中
+    IN_HEX_LITERAL_AFTER_0X = 43  # 在0x开头的十六进制字面值中
+    IN_BIT_LITERAL_OF_DOUBLE_QUOTE = 44  # 在二进制字面值的双引号中
+    IN_BIT_LITERAL_OF_SINGLE_QUOTE = 45  # 在二进制字面值的单引号中
+    IN_BIT_LITERAL_AFTER_0B = 46  # 在0b开头的位值字面值中
+    IN_INT = 47  # 在整型中
+    IN_FLOAT = 48  # 在浮点数中
+    IN_DOUBLE_QUOTE = 49  # 在双引号中
+    IN_DOUBLE_QUOTE_AFTER_22 = 50  # 在双引号中的、的 \ 符号之后
+    IN_DOUBLE_QUOTE_AFTER_5C = 51  # 在双引号中的 \\ 符号之后
+    IN_SINGLE_QUOTE = 52  # 在单引号中
+    IN_SINGLE_QUOTE_AFTER_27 = 53  # 在单引号中的、的 ' 符号之后
+    IN_SINGLE_QUOTE_AFTER_5C = 54  # 在单引号中的 \\ 符号之后
+    IN_BACK_QUOTE = 55  # 在反引号中
+    IN_EXPLAIN_1 = 56  # 在 # 或 -- 标记的单行注释中
+    IN_EXPLAIN_2 = 57  # 在多行注释中
+    IN_EXPLAIN_2_AFTER_2A = 58  # 在多行注释中的 * 符号之后
+    IN_WORD = 59  # 在普通词语中
 
     # 匹配状态已结束
-    END = "已结束"
+    END = 255  # 已结束
 
     # 自定义状态，用于插件开发
-    CUSTOM_1 = "自定义状态1"
-    CUSTOM_2 = "自定义状态2"
-    CUSTOM_3 = "自定义状态3"
-    CUSTOM_4 = "自定义状态4"
-    CUSTOM_5 = "自定义状态5"
-    CUSTOM_6 = "自定义状态6"
-    CUSTOM_7 = "自定义状态7"
-    CUSTOM_8 = "自定义状态8"
-    CUSTOM_9 = "自定义状态9"
-    CUSTOM_10 = "自定义状态10"
+    CUSTOM_1 = 201  # 自定义状态 1
+    CUSTOM_2 = 202  # 自定义状态 2
+    CUSTOM_3 = 203  # 自定义状态 3
+    CUSTOM_4 = 204  # 自定义状态 4
+    CUSTOM_5 = 205  # 自定义状态 5
+    CUSTOM_6 = 206  # 自定义状态 6
+    CUSTOM_7 = 207  # 自定义状态 7
+    CUSTOM_8 = 208  # 自定义状态 8
+    CUSTOM_9 = 209  # 自定义状态 9
+    CUSTOM_10 = 210  # 自定义状态 10
```

### Comparing `metasequoia-sql-0.5.0/metasequoia_sql.egg-info/SOURCES.txt` & `metasequoia-sql-0.6.0/metasequoia_sql.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 metasequoia_sql/__init__.py
+metasequoia_sql/config.py
 metasequoia_sql/errors.py
 metasequoia_sql.egg-info/PKG-INFO
 metasequoia_sql.egg-info/SOURCES.txt
 metasequoia_sql.egg-info/dependency_links.txt
 metasequoia_sql.egg-info/top_level.txt
 metasequoia_sql/analyzer/__init__.py
 metasequoia_sql/analyzer/base.py
@@ -27,15 +28,17 @@
 metasequoia_sql/common/name_set.py
 metasequoia_sql/common/scanner.py
 metasequoia_sql/common/static.py
 metasequoia_sql/core/__init__.py
 metasequoia_sql/core/node.py
 metasequoia_sql/core/parser.py
 metasequoia_sql/core/sql_type.py
+metasequoia_sql/core/static.py
 metasequoia_sql/lexical/__init__.py
 metasequoia_sql/lexical/amt_node.py
 metasequoia_sql/lexical/fsm_machine.py
+metasequoia_sql/lexical/fsm_memory.py
 metasequoia_sql/lexical/fsm_operate.py
 metasequoia_sql/lexical/fsm_operation_map.py
 metasequoia_sql/lexical/fsm_status.py
 metasequoia_sql/plugins/__init__.py
 metasequoia_sql/plugins/mybaitis.py
```

### Comparing `metasequoia-sql-0.5.0/setup.py` & `metasequoia-sql-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.5.0",
-    description="SQL语法解析器，包含词法树解析、语法树解析和语法树分析功能。",
+    version="0.6.0",
+    description="metasequoia-sql 是一款注重性能的 SQL 语法的解析和分析器，适用于 SQL 的格式化、执行和分析场景，致力于打造性能最高的 Python 版 SQL 解析器。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
     license="MIT License",
```

