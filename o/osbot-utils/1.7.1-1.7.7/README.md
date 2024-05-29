# Comparing `tmp/osbot_utils-1.7.1.tar.gz` & `tmp/osbot_utils-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbot_utils-1.7.1.tar", max compression
+gzip compressed data, was "osbot_utils-1.7.7.tar", max compression
```

## Comparing `osbot_utils-1.7.1.tar` & `osbot_utils-1.7.7.tar`

### file list

```diff
@@ -1,261 +1,260 @@
--rw-r--r--   0        0        0    11357 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/LICENSE
--rw-r--r--   0        0        0      649 2023-12-31 16:13:39.000000 osbot_utils-1.7.1/README.md
--rw-r--r--   0        0        0       16 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/__init__.py
--rw-r--r--   0        0        0     5884 2024-05-23 22:51:45.832209 osbot_utils-1.7.1/osbot_utils/base_classes/Cache_Pickle.py
--rw-r--r--   0        0        0     1096 2024-05-23 22:51:45.832285 osbot_utils-1.7.1/osbot_utils/base_classes/Kwargs_To_Disk.py
--rw-r--r--   0        0        0    17741 2024-05-23 22:51:45.930586 osbot_utils-1.7.1/osbot_utils/base_classes/Kwargs_To_Self.py
--rw-r--r--   0        0        0      517 2024-05-23 22:51:45.832957 osbot_utils-1.7.1/osbot_utils/base_classes/Type_Safe__List.py
--rw-r--r--   0        0        0        0 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/base_classes/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.930664 osbot_utils-1.7.1/osbot_utils/context_managers/__init__.py
--rw-r--r--   0        0        0     1187 2024-05-23 22:51:45.930749 osbot_utils-1.7.1/osbot_utils/context_managers/capture_duration.py
--rw-r--r--   0        0        0        0 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/__init__.py
--rw-r--r--   0        0        0        0 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/decorators/classes/__init__.py
--rw-r--r--   0        0        0      332 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/decorators/classes/singleton.py
--rw-r--r--   0        0        0        0 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/lists/__init__.py
--rw-r--r--   0        0        0      610 2024-05-23 22:51:45.833296 osbot_utils-1.7.1/osbot_utils/decorators/lists/filter_list.py
--rw-r--r--   0        0        0      697 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/lists/group_by.py
--rw-r--r--   0        0        0      850 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/decorators/lists/index_by.py
--rw-r--r--   0        0        0        0 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/methods/__init__.py
--rw-r--r--   0        0        0     1062 2024-05-23 22:51:45.833589 osbot_utils-1.7.1/osbot_utils/decorators/methods/cache.py
--rw-r--r--   0        0        0     2694 2024-05-23 22:51:45.833701 osbot_utils-1.7.1/osbot_utils/decorators/methods/cache_on_function.py
--rw-r--r--   0        0        0     3527 2024-05-23 22:51:45.834065 osbot_utils-1.7.1/osbot_utils/decorators/methods/cache_on_self.py
--rw-r--r--   0        0        0     3102 2024-05-23 22:51:45.834330 osbot_utils-1.7.1/osbot_utils/decorators/methods/cache_on_tmp.py
--rw-r--r--   0        0        0     1160 2024-05-23 22:51:45.930855 osbot_utils-1.7.1/osbot_utils/decorators/methods/capture_exception.py
--rw-r--r--   0        0        0      659 2024-05-23 22:51:45.834729 osbot_utils-1.7.1/osbot_utils/decorators/methods/capture_status.py
--rw-r--r--   0        0        0      545 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/methods/catch.py
--rw-r--r--   0        0        0      291 2024-05-23 22:51:45.835045 osbot_utils-1.7.1/osbot_utils/decorators/methods/context.py
--rw-r--r--   0        0        0     2288 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/methods/depreciated.py
--rw-r--r--   0        0        0     2757 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/methods/function_type_check.py
--rw-r--r--   0        0        0      104 2024-05-23 22:51:45.835314 osbot_utils-1.7.1/osbot_utils/decorators/methods/obj_as_context.py
--rw-r--r--   0        0        0     1163 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/decorators/methods/remove_return_value.py
--rw-r--r--   0        0        0      783 2024-05-23 22:51:45.835640 osbot_utils-1.7.1/osbot_utils/decorators/methods/required_fields.py
--rw-r--r--   0        0        0      481 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/fluent/Fluent_Dict.py
--rw-r--r--   0        0        0     1089 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/fluent/Fluent_List.py
--rw-r--r--   0        0        0        1 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/fluent/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.835668 osbot_utils-1.7.1/osbot_utils/graphs/__init__.py
--rw-r--r--   0        0        0     3068 2024-05-23 22:51:45.835920 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid.py
--rw-r--r--   0        0        0     1893 2024-05-23 22:51:45.836228 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Edge.py
--rw-r--r--   0        0        0     2829 2024-05-23 22:51:45.836466 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Graph.py
--rw-r--r--   0        0        0     3322 2024-05-23 22:51:45.836547 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Node.py
--rw-r--r--   0        0        0     2264 2024-05-23 22:51:45.836749 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Renderer.py
--rw-r--r--   0        0        0      212 2024-05-23 22:51:45.836817 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/configs/Mermaid__Edge__Config.py
--rw-r--r--   0        0        0      465 2024-05-23 22:51:45.836884 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/configs/Mermaid__Node__Config.py
--rw-r--r--   0        0        0      216 2024-05-23 22:51:45.837051 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/configs/Mermaid__Render__Config.py
--rw-r--r--   0        0        0     2220 2024-05-23 22:51:45.837182 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/examples/Mermaid_Examples__FlowChart.py
--rw-r--r--   0        0        0      141 2024-05-23 22:51:45.837245 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/models/Mermaid__Diagram_Direction.py
--rw-r--r--   0        0        0      624 2024-05-23 22:51:45.837303 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/models/Mermaid__Diagram__Type.py
--rw-r--r--   0        0        0     1813 2024-05-23 22:51:45.837430 osbot_utils-1.7.1/osbot_utils/graphs/mermaid/models/Mermaid__Node__Shape.py
--rw-r--r--   0        0        0     2193 2024-05-23 22:51:45.837782 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph.py
--rw-r--r--   0        0        0      204 2024-05-23 22:51:45.837848 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Config.py
--rw-r--r--   0        0        0     5746 2024-05-23 22:51:45.837932 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Data.py
--rw-r--r--   0        0        0      916 2024-05-23 22:51:45.838267 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Edge.py
--rw-r--r--   0        0        0      876 2024-05-23 22:51:45.838564 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Node.py
--rw-r--r--   0        0        0      964 2024-05-23 22:51:45.838668 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Random_Graphs.py
--rw-r--r--   0        0        0     1598 2024-05-23 22:51:45.838749 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Serializer.py
--rw-r--r--   0        0        0      636 2024-05-23 22:51:45.838998 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraphs.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.839028 osbot_utils-1.7.1/osbot_utils/graphs/mgraph/__init__.py
--rw-r--r--   0        0        0     4105 2024-05-23 22:51:45.839143 osbot_utils-1.7.1/osbot_utils/helpers/CPrint.py
--rw-r--r--   0        0        0      208 2024-05-23 22:51:45.839199 osbot_utils-1.7.1/osbot_utils/helpers/Dict_To_Attr.py
--rw-r--r--   0        0        0     3046 2024-05-23 22:51:45.839544 osbot_utils-1.7.1/osbot_utils/helpers/Local_Cache.py
--rw-r--r--   0        0        0     1814 2024-05-23 22:51:45.839898 osbot_utils-1.7.1/osbot_utils/helpers/Local_Caches.py
--rw-r--r--   0        0        0    19109 2024-05-23 22:51:45.840013 osbot_utils-1.7.1/osbot_utils/helpers/Print_Table.py
--rw-r--r--   0        0        0     1539 2024-05-23 22:51:45.840098 osbot_utils-1.7.1/osbot_utils/helpers/Python_Audit.py
--rw-r--r--   0        0        0      634 2024-05-23 22:51:45.840263 osbot_utils-1.7.1/osbot_utils/helpers/Random_Seed.py
--rw-r--r--   0        0        0     2687 2024-05-23 22:51:45.930920 osbot_utils-1.7.1/osbot_utils/helpers/SCP.py
--rw-r--r--   0        0        0     6151 2024-05-23 22:51:45.930998 osbot_utils-1.7.1/osbot_utils/helpers/SSH.py
--rw-r--r--   0        0        0      311 2024-05-23 22:51:45.840587 osbot_utils-1.7.1/osbot_utils/helpers/Type_Registry.py
--rw-r--r--   0        0        0        0 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/helpers/__init__.py
--rw-r--r--   0        0        0     1090 2024-05-23 22:51:45.840655 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast.py
--rw-r--r--   0        0        0     3708 2024-05-23 22:51:45.840955 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Base.py
--rw-r--r--   0        0        0      697 2024-05-23 22:51:45.841014 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Data.py
--rw-r--r--   0        0        0     2100 2024-05-23 22:51:45.841078 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Load.py
--rw-r--r--   0        0        0      848 2024-05-23 22:51:45.841140 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Merge.py
--rw-r--r--   0        0        0     5761 2024-05-23 22:51:45.841231 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Node.py
--rw-r--r--   0        0        0     2875 2024-05-23 22:51:45.841297 osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Visit.py
--rw-r--r--   0        0        0     1136 2024-05-23 22:51:45.841355 osbot_utils-1.7.1/osbot_utils/helpers/ast/Call_Tree.py
--rw-r--r--   0        0        0     8157 2024-05-23 22:51:45.841423 osbot_utils-1.7.1/osbot_utils/helpers/ast/__init__.py
--rw-r--r--   0        0        0      131 2024-05-23 22:51:45.841507 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Add.py
--rw-r--r--   0        0        0      190 2024-05-23 22:51:45.841562 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Alias.py
--rw-r--r--   0        0        0      131 2024-05-23 22:51:45.841613 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_And.py
--rw-r--r--   0        0        0      162 2024-05-23 22:51:45.841669 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Argument.py
--rw-r--r--   0        0        0      251 2024-05-23 22:51:45.841721 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Arguments.py
--rw-r--r--   0        0        0      215 2024-05-23 22:51:45.841773 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Assert.py
--rw-r--r--   0        0        0      261 2024-05-23 22:51:45.841841 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Assign.py
--rw-r--r--   0        0        0      331 2024-05-23 22:51:45.841904 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Attribute.py
--rw-r--r--   0        0        0      332 2024-05-23 22:51:45.841966 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Aug_Assign.py
--rw-r--r--   0        0        0      266 2024-05-23 22:51:45.842148 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Bin_Op.py
--rw-r--r--   0        0        0      221 2024-05-23 22:51:45.842198 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Bool_Op.py
--rw-r--r--   0        0        0      177 2024-05-23 22:51:45.842250 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Break.py
--rw-r--r--   0        0        0      554 2024-05-23 22:51:45.842303 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Call.py
--rw-r--r--   0        0        0      364 2024-05-23 22:51:45.842355 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Class_Def.py
--rw-r--r--   0        0        0      356 2024-05-23 22:51:45.842408 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Compare.py
--rw-r--r--   0        0        0      412 2024-05-23 22:51:45.842458 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Comprehension.py
--rw-r--r--   0        0        0      205 2024-05-23 22:51:45.842517 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Constant.py
--rw-r--r--   0        0        0      182 2024-05-23 22:51:45.842570 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Continue.py
--rw-r--r--   0        0        0      253 2024-05-23 22:51:45.842617 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Dict.py
--rw-r--r--   0        0        0      129 2024-05-23 22:51:45.842669 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Eq.py
--rw-r--r--   0        0        0      348 2024-05-23 22:51:45.842726 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Except_Handler.py
--rw-r--r--   0        0        0      200 2024-05-23 22:51:45.842797 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Expr.py
--rw-r--r--   0        0        0      354 2024-05-23 22:51:45.842849 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_For.py
--rw-r--r--   0        0        0      597 2024-05-23 22:51:45.842905 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Function_Def.py
--rw-r--r--   0        0        0      294 2024-05-23 22:51:45.842954 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Generator_Exp.py
--rw-r--r--   0        0        0      170 2024-05-23 22:51:45.843004 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Gt.py
--rw-r--r--   0        0        0      172 2024-05-23 22:51:45.843057 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_GtE.py
--rw-r--r--   0        0        0      300 2024-05-23 22:51:45.843109 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_If.py
--rw-r--r--   0        0        0      357 2024-05-23 22:51:45.843160 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_If_Exp.py
--rw-r--r--   0        0        0      204 2024-05-23 22:51:45.843215 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Import.py
--rw-r--r--   0        0        0      262 2024-05-23 22:51:45.843269 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Import_From.py
--rw-r--r--   0        0        0      129 2024-05-23 22:51:45.843325 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_In.py
--rw-r--r--   0        0        0      129 2024-05-23 22:51:45.843375 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Is.py
--rw-r--r--   0        0        0      178 2024-05-23 22:51:45.843431 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Is_Not.py
--rw-r--r--   0        0        0      260 2024-05-23 22:51:45.843486 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Keyword.py
--rw-r--r--   0        0        0      256 2024-05-23 22:51:45.843540 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Lambda.py
--rw-r--r--   0        0        0      247 2024-05-23 22:51:45.843589 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_List.py
--rw-r--r--   0        0        0      288 2024-05-23 22:51:45.843642 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_List_Comp.py
--rw-r--r--   0        0        0      133 2024-05-23 22:51:45.843690 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Load.py
--rw-r--r--   0        0        0      171 2024-05-23 22:51:45.843739 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Lt.py
--rw-r--r--   0        0        0      172 2024-05-23 22:51:45.843795 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_LtE.py
--rw-r--r--   0        0        0      131 2024-05-23 22:51:45.843847 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Mod.py
--rw-r--r--   0        0        0      576 2024-05-23 22:51:45.843903 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Module.py
--rw-r--r--   0        0        0      133 2024-05-23 22:51:45.843957 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Mult.py
--rw-r--r--   0        0        0      168 2024-05-23 22:51:45.844013 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Name.py
--rw-r--r--   0        0        0      172 2024-05-23 22:51:45.844071 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Not.py
--rw-r--r--   0        0        0      178 2024-05-23 22:51:45.844124 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Not_Eq.py
--rw-r--r--   0        0        0      137 2024-05-23 22:51:45.844178 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Not_In.py
--rw-r--r--   0        0        0      171 2024-05-23 22:51:45.844233 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Or.py
--rw-r--r--   0        0        0      174 2024-05-23 22:51:45.844284 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Pass.py
--rw-r--r--   0        0        0      172 2024-05-23 22:51:45.844329 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Pow.py
--rw-r--r--   0        0        0      251 2024-05-23 22:51:45.844379 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Raise.py
--rw-r--r--   0        0        0      161 2024-05-23 22:51:45.844435 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Return.py
--rw-r--r--   0        0        0      194 2024-05-23 22:51:45.844489 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Set.py
--rw-r--r--   0        0        0      266 2024-05-23 22:51:45.844546 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Slice.py
--rw-r--r--   0        0        0      252 2024-05-23 22:51:45.844596 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Starred.py
--rw-r--r--   0        0        0      176 2024-05-23 22:51:45.844644 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Store.py
--rw-r--r--   0        0        0      172 2024-05-23 22:51:45.844695 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Sub.py
--rw-r--r--   0        0        0      278 2024-05-23 22:51:45.844746 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Subscript.py
--rw-r--r--   0        0        0      337 2024-05-23 22:51:45.844795 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Try.py
--rw-r--r--   0        0        0      302 2024-05-23 22:51:45.844848 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Tuple.py
--rw-r--r--   0        0        0      227 2024-05-23 22:51:45.844905 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Unary_Op.py
--rw-r--r--   0        0        0      268 2024-05-23 22:51:45.844956 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_While.py
--rw-r--r--   0        0        0      211 2024-05-23 22:51:45.845002 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_With.py
--rw-r--r--   0        0        0      260 2024-05-23 22:51:45.845057 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_With_Item.py
--rw-r--r--   0        0        0      197 2024-05-23 22:51:45.845110 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Yield.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.845129 osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/__init__.py
--rw-r--r--   0        0        0     1097 2024-05-23 22:51:45.845380 osbot_utils-1.7.1/osbot_utils/helpers/html/Dict_To_Css.py
--rw-r--r--   0        0        0     3355 2024-05-23 22:51:45.845652 osbot_utils-1.7.1/osbot_utils/helpers/html/Dict_To_Html.py
--rw-r--r--   0        0        0     3766 2024-05-23 22:51:45.931109 osbot_utils-1.7.1/osbot_utils/helpers/html/Dict_To_Tags.py
--rw-r--r--   0        0        0     2623 2024-05-23 22:51:45.931205 osbot_utils-1.7.1/osbot_utils/helpers/html/Html_To_Dict.py
--rw-r--r--   0        0        0      498 2024-05-23 22:51:45.931255 osbot_utils-1.7.1/osbot_utils/helpers/html/Html_To_Tag.py
--rw-r--r--   0        0        0     3128 2024-05-23 22:51:45.931347 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Base.py
--rw-r--r--   0        0        0      109 2024-05-23 22:51:45.846129 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Body.py
--rw-r--r--   0        0        0      109 2024-05-23 22:51:45.846317 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Div.py
--rw-r--r--   0        0        0      295 2024-05-23 22:51:45.846516 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__H.py
--rw-r--r--   0        0        0      107 2024-05-23 22:51:45.846738 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__HR.py
--rw-r--r--   0        0        0     1102 2024-05-23 22:51:45.846942 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Head.py
--rw-r--r--   0        0        0     1131 2024-05-23 22:51:45.931433 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Html.py
--rw-r--r--   0        0        0      437 2024-05-23 22:51:45.847199 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Link.py
--rw-r--r--   0        0        0      846 2024-05-23 22:51:45.847468 osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Style.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.847490 osbot_utils-1.7.1/osbot_utils/helpers/html/__init__.py
--rw-r--r--   0        0        0     3187 2024-05-23 22:51:45.931531 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/Event__Queue.py
--rw-r--r--   0        0        0     2292 2024-05-23 22:51:45.931602 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Client.py
--rw-r--r--   0        0        0      457 2024-05-23 22:51:45.931656 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Room.py
--rw-r--r--   0        0        0     3519 2024-05-23 22:51:45.931719 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Server.py
--rw-r--r--   0        0        0      868 2024-05-23 22:51:45.931779 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Sqlite.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.931797 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/__init__.py
--rw-r--r--   0        0        0      402 2024-05-23 22:51:45.931900 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__Event.py
--rw-r--r--   0        0        0      269 2024-05-23 22:51:45.931952 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__Event__Connect.py
--rw-r--r--   0        0        0      275 2024-05-23 22:51:45.931999 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__Event__Disconnect.py
--rw-r--r--   0        0        0      293 2024-05-23 22:51:45.932046 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__Event__Join_Room.py
--rw-r--r--   0        0        0      295 2024-05-23 22:51:45.932095 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__Event__Leave_Room.py
--rw-r--r--   0        0        0      244 2024-05-23 22:51:45.932148 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__Event__Message.py
--rw-r--r--   0        0        0      239 2024-05-23 22:51:45.932200 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/Schema__PubSub__Client.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.932221 osbot_utils-1.7.1/osbot_utils/helpers/pubsub/schemas/__init__.py
--rw-r--r--   0        0        0     1747 2024-05-23 22:51:45.847744 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Capture_Sqlite_Error.py
--rw-r--r--   0        0        0     3303 2024-05-23 22:51:45.847924 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Cursor.py
--rw-r--r--   0        0        0     5261 2024-05-23 22:51:45.932345 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Database.py
--rw-r--r--   0        0        0     2911 2024-05-23 22:51:45.848640 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Field.py
--rw-r--r--   0        0        0      230 2024-05-23 22:51:45.848893 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Globals.py
--rw-r--r--   0        0        0    14805 2024-05-23 22:51:45.932497 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Table.py
--rw-r--r--   0        0        0     3825 2024-05-23 22:51:45.932589 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Table__Create.py
--rw-r--r--   0        0        0      520 2024-05-23 22:51:45.849938 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Temp_Sqlite__Database__Disk.py
--rw-r--r--   0        0        0      729 2024-05-23 22:51:45.850371 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Temp_Sqlite__Table.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.850391 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-23 22:51:45.932703 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests.py
--rw-r--r--   0        0        0     2322 2024-05-23 22:51:45.932764 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests__Patch.py
--rw-r--r--   0        0        0      768 2024-05-23 22:51:45.932883 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Files.py
--rw-r--r--   0        0        0     1751 2024-05-23 22:51:45.932936 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Graph.py
--rw-r--r--   0        0        0     3808 2024-05-23 22:51:45.850594 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Json.py
--rw-r--r--   0        0        0      882 2024-05-23 22:51:45.933014 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Local.py
--rw-r--r--   0        0        0     1541 2024-05-23 22:51:45.933094 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Requests.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.850744 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/__init__.py
--rw-r--r--   0        0        0      443 2024-05-23 22:51:45.850840 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/schemas/Schema__Table__Requests.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.850863 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/schemas/__init__.py
--rw-r--r--   0        0        0     1023 2024-05-23 22:51:45.851184 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/models/Sqlite__Field__Type.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.851211 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/models/__init__.py
--rw-r--r--   0        0        0     5415 2024-05-23 22:51:45.851566 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sample_data/Sqlite__Sample_Data__Chinook.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.851596 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sample_data/__init__.py
--rw-r--r--   0        0        0    10782 2024-05-23 22:51:45.933198 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sql_builder/SQL_Builder.py
--rw-r--r--   0        0        0      360 2024-05-23 22:51:45.852031 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sql_builder/SQL_Builder__Select.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.852053 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sql_builder/__init__.py
--rw-r--r--   0        0        0     2061 2024-05-23 22:51:45.933280 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Config.py
--rw-r--r--   0        0        0     1635 2024-05-23 22:51:45.933343 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Edges.py
--rw-r--r--   0        0        0     1510 2024-05-23 22:51:45.933395 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Files.py
--rw-r--r--   0        0        0     1721 2024-05-23 22:51:45.933446 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Nodes.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.933468 osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/__init__.py
--rw-r--r--   0        0        0     6329 2024-05-23 22:51:45.933581 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call.py
--rw-r--r--   0        0        0     3250 2024-05-23 22:51:45.933666 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Config.py
--rw-r--r--   0        0        0     1156 2024-05-23 22:51:45.852524 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Graph.py
--rw-r--r--   0        0        0    11533 2024-05-23 22:51:45.852821 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Handler.py
--rw-r--r--   0        0        0     4849 2024-05-23 22:51:45.852892 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Print_Lines.py
--rw-r--r--   0        0        0     8628 2024-05-23 22:51:45.853028 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Print_Traces.py
--rw-r--r--   0        0        0     7462 2024-05-23 22:51:45.853298 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Stack.py
--rw-r--r--   0        0        0     1833 2024-05-23 22:51:45.853364 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Stack_Node.py
--rw-r--r--   0        0        0     2228 2024-05-23 22:51:45.853426 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Stats.py
--rw-r--r--   0        0        0     4545 2024-05-23 22:51:45.853538 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__View_Model.py
--rw-r--r--   0        0        0      978 2024-05-23 22:51:45.853595 osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Files.py
--rw-r--r--   0        0        0        0 2024-05-23 22:51:45.853616 osbot_utils-1.7.1/osbot_utils/helpers/trace/__init__.py
--rw-r--r--   0        0        0     2228 2024-05-23 22:51:45.853968 osbot_utils-1.7.1/osbot_utils/testing/Catch.py
--rw-r--r--   0        0        0     2217 2024-05-23 22:51:45.854191 osbot_utils-1.7.1/osbot_utils/testing/Duration.py
--rw-r--r--   0        0        0     4126 2024-05-23 22:51:45.854289 osbot_utils-1.7.1/osbot_utils/testing/Hook_Method.py
--rw-r--r--   0        0        0     1703 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/testing/Log_To_Queue.py
--rw-r--r--   0        0        0     1216 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/testing/Log_To_String.py
--rw-r--r--   0        0        0     3010 2024-05-23 22:51:45.933764 osbot_utils-1.7.1/osbot_utils/testing/Logging.py
--rw-r--r--   0        0        0     1566 2024-05-23 22:51:45.854340 osbot_utils-1.7.1/osbot_utils/testing/Patch_Print.py
--rw-r--r--   0        0        0     3255 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/testing/Profiler.py
--rw-r--r--   0        0        0      459 2024-05-23 22:51:45.854546 osbot_utils-1.7.1/osbot_utils/testing/Stderr.py
--rw-r--r--   0        0        0      459 2024-05-23 22:51:45.854594 osbot_utils-1.7.1/osbot_utils/testing/Stdout.py
--rw-r--r--   0        0        0     1410 2024-05-23 22:51:45.854808 osbot_utils-1.7.1/osbot_utils/testing/Temp_File.py
--rw-r--r--   0        0        0     4793 2024-05-23 22:51:45.933861 osbot_utils-1.7.1/osbot_utils/testing/Temp_Folder.py
--rw-r--r--   0        0        0      256 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/testing/Temp_Sys_Path.py
--rw-r--r--   0        0        0     3186 2024-05-23 22:51:45.854903 osbot_utils-1.7.1/osbot_utils/testing/Temp_Web_Server.py
--rw-r--r--   0        0        0     1349 2024-05-23 22:51:45.933954 osbot_utils-1.7.1/osbot_utils/testing/Temp_Zip.py
--rw-r--r--   0        0        0     3278 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/testing/Temp_Zip_In_Memory.py
--rw-r--r--   0        0        0     1304 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/testing/Unit_Test.py
--rw-r--r--   0        0        0     1177 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/testing/Unzip_File.py
--rw-r--r--   0        0        0        0 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/testing/__init__.py
--rw-r--r--   0        0        0     1745 2024-05-23 22:51:45.855219 osbot_utils-1.7.1/osbot_utils/utils/Assert.py
--rw-r--r--   0        0        0     6595 2024-05-23 22:51:45.855289 osbot_utils-1.7.1/osbot_utils/utils/Call_Stack.py
--rw-r--r--   0        0        0     1012 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/utils/Csv.py
--rw-r--r--   0        0        0     1203 2024-05-23 22:51:45.855374 osbot_utils-1.7.1/osbot_utils/utils/Dev.py
--rw-r--r--   0        0        0      389 2024-05-23 22:51:45.855534 osbot_utils-1.7.1/osbot_utils/utils/Exceptions.py
--rw-r--r--   0        0        0    17807 2024-05-23 22:51:45.934089 osbot_utils-1.7.1/osbot_utils/utils/Files.py
--rw-r--r--   0        0        0     3498 2024-05-23 22:51:45.855940 osbot_utils-1.7.1/osbot_utils/utils/Functions.py
--rw-r--r--   0        0        0     4572 2024-05-23 22:51:45.856042 osbot_utils-1.7.1/osbot_utils/utils/Http.py
--rw-r--r--   0        0        0      130 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/utils/Int.py
--rw-r--r--   0        0        0     6366 2024-05-23 22:51:45.856135 osbot_utils-1.7.1/osbot_utils/utils/Json.py
--rw-r--r--   0        0        0     2006 2024-05-23 22:51:45.856220 osbot_utils-1.7.1/osbot_utils/utils/Json_Cache.py
--rw-r--r--   0        0        0     5502 2024-05-23 22:51:45.934195 osbot_utils-1.7.1/osbot_utils/utils/Lists.py
--rw-r--r--   0        0        0    16486 2024-05-23 22:51:45.934336 osbot_utils-1.7.1/osbot_utils/utils/Misc.py
--rw-r--r--   0        0        0    13817 2024-05-23 22:51:45.934464 osbot_utils-1.7.1/osbot_utils/utils/Objects.py
--rw-r--r--   0        0        0     1172 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/utils/Png.py
--rw-r--r--   0        0        0     2357 2024-05-23 22:51:45.934552 osbot_utils-1.7.1/osbot_utils/utils/Process.py
--rw-r--r--   0        0        0    11245 2024-05-23 22:51:45.856907 osbot_utils-1.7.1/osbot_utils/utils/Python_Logger.py
--rw-r--r--   0        0        0     4305 2024-05-23 22:51:45.857222 osbot_utils-1.7.1/osbot_utils/utils/Status.py
--rw-r--r--   0        0        0     1398 2024-05-23 22:51:45.857540 osbot_utils-1.7.1/osbot_utils/utils/Str.py
--rw-r--r--   0        0        0      422 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/utils/Version.py
--rw-r--r--   0        0        0     1097 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/utils/Yaml.py
--rw-r--r--   0        0        0     4503 2023-12-31 16:01:47.000000 osbot_utils-1.7.1/osbot_utils/utils/Zip.py
--rw-r--r--   0        0        0      179 2023-12-31 01:52:10.000000 osbot_utils-1.7.1/osbot_utils/utils/__init__.py
--rw-r--r--   0        0        0        7 2024-05-24 00:02:16.905929 osbot_utils-1.7.1/osbot_utils/version
--rw-r--r--   0        0        0      517 2024-05-24 00:03:05.992118 osbot_utils-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1670 1970-01-01 00:00:00.000000 osbot_utils-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/LICENSE
+-rw-r--r--   0        0        0      649 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/README.md
+-rw-r--r--   0        0        0       16 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/__init__.py
+-rw-r--r--   0        0        0     5884 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/base_classes/Cache_Pickle.py
+-rw-r--r--   0        0        0     1096 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/base_classes/Kwargs_To_Disk.py
+-rw-r--r--   0        0        0    17741 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/base_classes/Kwargs_To_Self.py
+-rw-r--r--   0        0        0      517 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/base_classes/Type_Safe__List.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/base_classes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/context_managers/__init__.py
+-rw-r--r--   0        0        0     1187 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/context_managers/capture_duration.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/classes/__init__.py
+-rw-r--r--   0        0        0      332 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/classes/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/lists/__init__.py
+-rw-r--r--   0        0        0      610 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/lists/filter_list.py
+-rw-r--r--   0        0        0      697 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/lists/group_by.py
+-rw-r--r--   0        0        0      850 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/lists/index_by.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/__init__.py
+-rw-r--r--   0        0        0     1062 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/cache.py
+-rw-r--r--   0        0        0     2694 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/cache_on_function.py
+-rw-r--r--   0        0        0     3527 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/cache_on_self.py
+-rw-r--r--   0        0        0     3102 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/cache_on_tmp.py
+-rw-r--r--   0        0        0     1160 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/capture_exception.py
+-rw-r--r--   0        0        0      659 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/capture_status.py
+-rw-r--r--   0        0        0      545 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/catch.py
+-rw-r--r--   0        0        0      291 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/context.py
+-rw-r--r--   0        0        0     2288 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/depreciated.py
+-rw-r--r--   0        0        0     2757 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/function_type_check.py
+-rw-r--r--   0        0        0      104 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/obj_as_context.py
+-rw-r--r--   0        0        0     1163 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/remove_return_value.py
+-rw-r--r--   0        0        0      783 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/decorators/methods/required_fields.py
+-rw-r--r--   0        0        0      481 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/fluent/Fluent_Dict.py
+-rw-r--r--   0        0        0     1089 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/fluent/Fluent_List.py
+-rw-r--r--   0        0        0        1 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/fluent/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/__init__.py
+-rw-r--r--   0        0        0     3068 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid.py
+-rw-r--r--   0        0        0     1893 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Edge.py
+-rw-r--r--   0        0        0     2829 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Graph.py
+-rw-r--r--   0        0        0     3322 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Node.py
+-rw-r--r--   0        0        0     2264 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Renderer.py
+-rw-r--r--   0        0        0      212 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/configs/Mermaid__Edge__Config.py
+-rw-r--r--   0        0        0      465 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/configs/Mermaid__Node__Config.py
+-rw-r--r--   0        0        0      216 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/configs/Mermaid__Render__Config.py
+-rw-r--r--   0        0        0     2220 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/examples/Mermaid_Examples__FlowChart.py
+-rw-r--r--   0        0        0      141 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/models/Mermaid__Diagram_Direction.py
+-rw-r--r--   0        0        0      624 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/models/Mermaid__Diagram__Type.py
+-rw-r--r--   0        0        0     1813 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mermaid/models/Mermaid__Node__Shape.py
+-rw-r--r--   0        0        0     2193 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph.py
+-rw-r--r--   0        0        0      204 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Config.py
+-rw-r--r--   0        0        0     5746 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Data.py
+-rw-r--r--   0        0        0      916 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Edge.py
+-rw-r--r--   0        0        0      876 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Node.py
+-rw-r--r--   0        0        0      964 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Random_Graphs.py
+-rw-r--r--   0        0        0     1408 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Serializer.py
+-rw-r--r--   0        0        0      636 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraphs.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/graphs/mgraph/__init__.py
+-rw-r--r--   0        0        0     4105 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/CPrint.py
+-rw-r--r--   0        0        0      208 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/Dict_To_Attr.py
+-rw-r--r--   0        0        0     3046 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/Local_Cache.py
+-rw-r--r--   0        0        0     1814 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/Local_Caches.py
+-rw-r--r--   0        0        0    19109 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/Print_Table.py
+-rw-r--r--   0        0        0     1539 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/Python_Audit.py
+-rw-r--r--   0        0        0      634 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/Random_Seed.py
+-rw-r--r--   0        0        0     2687 2024-05-24 08:55:53.601008 osbot_utils-1.7.7/osbot_utils/helpers/SCP.py
+-rw-r--r--   0        0        0     6151 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/SSH.py
+-rw-r--r--   0        0        0      311 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/Type_Registry.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/__init__.py
+-rw-r--r--   0        0        0     1090 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast.py
+-rw-r--r--   0        0        0     3708 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Base.py
+-rw-r--r--   0        0        0      697 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Data.py
+-rw-r--r--   0        0        0     2100 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Load.py
+-rw-r--r--   0        0        0      848 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Merge.py
+-rw-r--r--   0        0        0     5761 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Node.py
+-rw-r--r--   0        0        0     2875 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Visit.py
+-rw-r--r--   0        0        0     1136 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/Call_Tree.py
+-rw-r--r--   0        0        0     8157 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Add.py
+-rw-r--r--   0        0        0      190 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Alias.py
+-rw-r--r--   0        0        0      131 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_And.py
+-rw-r--r--   0        0        0      162 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Argument.py
+-rw-r--r--   0        0        0      251 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Arguments.py
+-rw-r--r--   0        0        0      215 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Assert.py
+-rw-r--r--   0        0        0      261 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Assign.py
+-rw-r--r--   0        0        0      331 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Attribute.py
+-rw-r--r--   0        0        0      332 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Aug_Assign.py
+-rw-r--r--   0        0        0      266 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Bin_Op.py
+-rw-r--r--   0        0        0      221 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Bool_Op.py
+-rw-r--r--   0        0        0      177 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Break.py
+-rw-r--r--   0        0        0      554 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Call.py
+-rw-r--r--   0        0        0      364 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Class_Def.py
+-rw-r--r--   0        0        0      356 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Compare.py
+-rw-r--r--   0        0        0      412 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Comprehension.py
+-rw-r--r--   0        0        0      205 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Constant.py
+-rw-r--r--   0        0        0      182 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Continue.py
+-rw-r--r--   0        0        0      253 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Dict.py
+-rw-r--r--   0        0        0      129 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Eq.py
+-rw-r--r--   0        0        0      348 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Except_Handler.py
+-rw-r--r--   0        0        0      200 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Expr.py
+-rw-r--r--   0        0        0      354 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_For.py
+-rw-r--r--   0        0        0      597 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Function_Def.py
+-rw-r--r--   0        0        0      294 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Generator_Exp.py
+-rw-r--r--   0        0        0      170 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Gt.py
+-rw-r--r--   0        0        0      172 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_GtE.py
+-rw-r--r--   0        0        0      300 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_If.py
+-rw-r--r--   0        0        0      357 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_If_Exp.py
+-rw-r--r--   0        0        0      204 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Import.py
+-rw-r--r--   0        0        0      262 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Import_From.py
+-rw-r--r--   0        0        0      129 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_In.py
+-rw-r--r--   0        0        0      129 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Is.py
+-rw-r--r--   0        0        0      178 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Is_Not.py
+-rw-r--r--   0        0        0      260 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Keyword.py
+-rw-r--r--   0        0        0      256 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Lambda.py
+-rw-r--r--   0        0        0      247 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_List.py
+-rw-r--r--   0        0        0      288 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_List_Comp.py
+-rw-r--r--   0        0        0      133 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Load.py
+-rw-r--r--   0        0        0      171 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Lt.py
+-rw-r--r--   0        0        0      172 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_LtE.py
+-rw-r--r--   0        0        0      131 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Mod.py
+-rw-r--r--   0        0        0      576 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Module.py
+-rw-r--r--   0        0        0      133 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Mult.py
+-rw-r--r--   0        0        0      168 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Name.py
+-rw-r--r--   0        0        0      172 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Not.py
+-rw-r--r--   0        0        0      178 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Not_Eq.py
+-rw-r--r--   0        0        0      137 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Not_In.py
+-rw-r--r--   0        0        0      171 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Or.py
+-rw-r--r--   0        0        0      174 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Pass.py
+-rw-r--r--   0        0        0      172 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Pow.py
+-rw-r--r--   0        0        0      251 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Raise.py
+-rw-r--r--   0        0        0      161 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Return.py
+-rw-r--r--   0        0        0      194 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Set.py
+-rw-r--r--   0        0        0      266 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Slice.py
+-rw-r--r--   0        0        0      252 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Starred.py
+-rw-r--r--   0        0        0      176 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Store.py
+-rw-r--r--   0        0        0      172 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Sub.py
+-rw-r--r--   0        0        0      278 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Subscript.py
+-rw-r--r--   0        0        0      337 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Try.py
+-rw-r--r--   0        0        0      302 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Tuple.py
+-rw-r--r--   0        0        0      227 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Unary_Op.py
+-rw-r--r--   0        0        0      268 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_While.py
+-rw-r--r--   0        0        0      211 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_With.py
+-rw-r--r--   0        0        0      260 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_With_Item.py
+-rw-r--r--   0        0        0      197 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Yield.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/__init__.py
+-rw-r--r--   0        0        0     1097 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Dict_To_Css.py
+-rw-r--r--   0        0        0     3355 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Dict_To_Html.py
+-rw-r--r--   0        0        0     3766 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Dict_To_Tags.py
+-rw-r--r--   0        0        0     2623 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Html_To_Dict.py
+-rw-r--r--   0        0        0      498 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Html_To_Tag.py
+-rw-r--r--   0        0        0     3128 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Base.py
+-rw-r--r--   0        0        0      109 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Body.py
+-rw-r--r--   0        0        0      109 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Div.py
+-rw-r--r--   0        0        0      295 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__H.py
+-rw-r--r--   0        0        0      107 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__HR.py
+-rw-r--r--   0        0        0     1102 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Head.py
+-rw-r--r--   0        0        0     1131 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Html.py
+-rw-r--r--   0        0        0      437 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Link.py
+-rw-r--r--   0        0        0      846 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Style.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/html/__init__.py
+-rw-r--r--   0        0        0     3187 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/Event__Queue.py
+-rw-r--r--   0        0        0     2292 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Client.py
+-rw-r--r--   0        0        0      457 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Room.py
+-rw-r--r--   0        0        0     3519 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Server.py
+-rw-r--r--   0        0        0      868 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Sqlite.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/__init__.py
+-rw-r--r--   0        0        0      402 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__Event.py
+-rw-r--r--   0        0        0      269 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__Event__Connect.py
+-rw-r--r--   0        0        0      275 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__Event__Disconnect.py
+-rw-r--r--   0        0        0      293 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__Event__Join_Room.py
+-rw-r--r--   0        0        0      295 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__Event__Leave_Room.py
+-rw-r--r--   0        0        0      244 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__Event__Message.py
+-rw-r--r--   0        0        0      239 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/Schema__PubSub__Client.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/pubsub/schemas/__init__.py
+-rw-r--r--   0        0        0     1747 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Capture_Sqlite_Error.py
+-rw-r--r--   0        0        0     3303 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Cursor.py
+-rw-r--r--   0        0        0     5261 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Database.py
+-rw-r--r--   0        0        0     2911 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Field.py
+-rw-r--r--   0        0        0      230 2024-05-24 08:55:53.605008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Globals.py
+-rw-r--r--   0        0        0    14805 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Table.py
+-rw-r--r--   0        0        0     3825 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Table__Create.py
+-rw-r--r--   0        0        0      520 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Temp_Sqlite__Database__Disk.py
+-rw-r--r--   0        0        0      729 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Temp_Sqlite__Table.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests.py
+-rw-r--r--   0        0        0     2322 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests__Patch.py
+-rw-r--r--   0        0        0      768 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Files.py
+-rw-r--r--   0        0        0     1751 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Graph.py
+-rw-r--r--   0        0        0     3808 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Json.py
+-rw-r--r--   0        0        0      882 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Local.py
+-rw-r--r--   0        0        0     1541 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Requests.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/__init__.py
+-rw-r--r--   0        0        0      443 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/schemas/Schema__Table__Requests.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/schemas/__init__.py
+-rw-r--r--   0        0        0     1023 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/models/Sqlite__Field__Type.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sample_data/Sqlite__Sample_Data__Chinook.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sample_data/__init__.py
+-rw-r--r--   0        0        0    10782 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sql_builder/SQL_Builder.py
+-rw-r--r--   0        0        0      360 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sql_builder/SQL_Builder__Select.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sql_builder/__init__.py
+-rw-r--r--   0        0        0     2061 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Config.py
+-rw-r--r--   0        0        0     1635 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Edges.py
+-rw-r--r--   0        0        0     1510 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Files.py
+-rw-r--r--   0        0        0     1721 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Nodes.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/__init__.py
+-rw-r--r--   0        0        0     6329 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call.py
+-rw-r--r--   0        0        0     3250 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Config.py
+-rw-r--r--   0        0        0     1156 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Graph.py
+-rw-r--r--   0        0        0    11533 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Handler.py
+-rw-r--r--   0        0        0     4849 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Print_Lines.py
+-rw-r--r--   0        0        0     8628 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Print_Traces.py
+-rw-r--r--   0        0        0     7462 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Stack.py
+-rw-r--r--   0        0        0     1833 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Stack_Node.py
+-rw-r--r--   0        0        0     2228 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Stats.py
+-rw-r--r--   0        0        0     4545 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__View_Model.py
+-rw-r--r--   0        0        0      978 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Files.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/helpers/trace/__init__.py
+-rw-r--r--   0        0        0     2228 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Catch.py
+-rw-r--r--   0        0        0     2217 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Duration.py
+-rw-r--r--   0        0        0     4126 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Hook_Method.py
+-rw-r--r--   0        0        0     1703 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Log_To_Queue.py
+-rw-r--r--   0        0        0     1216 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Log_To_String.py
+-rw-r--r--   0        0        0     3010 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Logging.py
+-rw-r--r--   0        0        0     1566 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Patch_Print.py
+-rw-r--r--   0        0        0     3255 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Profiler.py
+-rw-r--r--   0        0        0      459 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Stderr.py
+-rw-r--r--   0        0        0      459 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Stdout.py
+-rw-r--r--   0        0        0     1410 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Temp_File.py
+-rw-r--r--   0        0        0     4793 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Temp_Folder.py
+-rw-r--r--   0        0        0      256 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Temp_Sys_Path.py
+-rw-r--r--   0        0        0     3186 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Temp_Web_Server.py
+-rw-r--r--   0        0        0     1349 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Temp_Zip.py
+-rw-r--r--   0        0        0     3278 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Temp_Zip_In_Memory.py
+-rw-r--r--   0        0        0     1304 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Unit_Test.py
+-rw-r--r--   0        0        0     1177 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/Unzip_File.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/testing/__init__.py
+-rw-r--r--   0        0        0     1745 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Assert.py
+-rw-r--r--   0        0        0     6595 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Call_Stack.py
+-rw-r--r--   0        0        0     1012 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Csv.py
+-rw-r--r--   0        0        0     1203 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Dev.py
+-rw-r--r--   0        0        0      389 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Exceptions.py
+-rw-r--r--   0        0        0    17807 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Files.py
+-rw-r--r--   0        0        0     3498 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Functions.py
+-rw-r--r--   0        0        0     4572 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Http.py
+-rw-r--r--   0        0        0      130 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Int.py
+-rw-r--r--   0        0        0     6366 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Json.py
+-rw-r--r--   0        0        0     2006 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Json_Cache.py
+-rw-r--r--   0        0        0     5502 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Lists.py
+-rw-r--r--   0        0        0    16486 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Misc.py
+-rw-r--r--   0        0        0    13817 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Objects.py
+-rw-r--r--   0        0        0     1172 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Png.py
+-rw-r--r--   0        0        0     2357 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Process.py
+-rw-r--r--   0        0        0    11245 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Python_Logger.py
+-rw-r--r--   0        0        0     4305 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Status.py
+-rw-r--r--   0        0        0     1398 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Str.py
+-rw-r--r--   0        0        0      422 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Version.py
+-rw-r--r--   0        0        0     4503 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/Zip.py
+-rw-r--r--   0        0        0      172 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/utils/__init__.py
+-rw-r--r--   0        0        0        7 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/osbot_utils/version
+-rw-r--r--   0        0        0      609 2024-05-24 08:55:53.609008 osbot_utils-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 osbot_utils-1.7.7/PKG-INFO
```

### Comparing `osbot_utils-1.7.1/LICENSE` & `osbot_utils-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/README.md` & `osbot_utils-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/base_classes/Cache_Pickle.py` & `osbot_utils-1.7.7/osbot_utils/base_classes/Cache_Pickle.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/base_classes/Kwargs_To_Disk.py` & `osbot_utils-1.7.7/osbot_utils/base_classes/Kwargs_To_Disk.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/base_classes/Kwargs_To_Self.py` & `osbot_utils-1.7.7/osbot_utils/base_classes/Kwargs_To_Self.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/base_classes/Type_Safe__List.py` & `osbot_utils-1.7.7/osbot_utils/base_classes/Type_Safe__List.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/context_managers/capture_duration.py` & `osbot_utils-1.7.7/osbot_utils/context_managers/capture_duration.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/lists/filter_list.py` & `osbot_utils-1.7.7/osbot_utils/decorators/lists/filter_list.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/lists/group_by.py` & `osbot_utils-1.7.7/osbot_utils/decorators/lists/group_by.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/lists/index_by.py` & `osbot_utils-1.7.7/osbot_utils/decorators/lists/index_by.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/cache.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/cache.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/cache_on_function.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/cache_on_function.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/cache_on_self.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/cache_on_self.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/cache_on_tmp.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/cache_on_tmp.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/capture_exception.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/capture_exception.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/capture_status.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/capture_status.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/catch.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/catch.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/depreciated.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/depreciated.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/function_type_check.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/function_type_check.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/remove_return_value.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/remove_return_value.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/decorators/methods/required_fields.py` & `osbot_utils-1.7.7/osbot_utils/decorators/methods/required_fields.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/fluent/Fluent_List.py` & `osbot_utils-1.7.7/osbot_utils/fluent/Fluent_List.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Edge.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Edge.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Graph.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Graph.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Node.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Node.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/Mermaid__Renderer.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/Mermaid__Renderer.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/examples/Mermaid_Examples__FlowChart.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/examples/Mermaid_Examples__FlowChart.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/models/Mermaid__Diagram__Type.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/models/Mermaid__Diagram__Type.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mermaid/models/Mermaid__Node__Shape.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mermaid/models/Mermaid__Node__Shape.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Data.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Data.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Edge.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Edge.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Node.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Node.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Random_Graphs.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Random_Graphs.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraph__Serializer.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraph__Serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from osbot_utils.base_classes.Kwargs_To_Self import Kwargs_To_Self
 from osbot_utils.graphs.mgraph.MGraph import MGraph
 
 
 class Serialization_Mode(Enum):
     JSON    = auto()
     PICKLE  = auto()
-    YAML    = auto()
 
 class MGraph__Serializer(Kwargs_To_Self):
 
     caches_name : str                = 'mgraph_tests'
     mode        : Serialization_Mode = Serialization_Mode.PICKLE
 
     local_cache : Local_Cache                                           # todo, refactor this into an MGraph__Storage__Disk class
@@ -28,22 +27,17 @@
 
 
     def save(self):
         if self.mode == Serialization_Mode.JSON:
             return self.save_to_json()
         if self.mode == Serialization_Mode.PICKLE:
             return self.save_to_pickle()
-        if self.mode == Serialization_Mode.YAML:
-            return self.save_to_yaml()
 
     def save_to_json(self):
         graph_data = self.mgraph.data().graph_data()
         #pprint(graph_data)
         self.local_cache.set('graph_data', graph_data)
         return True
 
     def save_to_pickle(self):
         #obj_info(self.local_cache)
         return '...pickle save - to be implemented...'
-
-    def save_to_yaml(self):
-        return '...yaml save - to be implemented...'
```

### Comparing `osbot_utils-1.7.1/osbot_utils/graphs/mgraph/MGraphs.py` & `osbot_utils-1.7.7/osbot_utils/graphs/mgraph/MGraphs.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/CPrint.py` & `osbot_utils-1.7.7/osbot_utils/helpers/CPrint.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/Local_Cache.py` & `osbot_utils-1.7.7/osbot_utils/helpers/Local_Cache.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/Local_Caches.py` & `osbot_utils-1.7.7/osbot_utils/helpers/Local_Caches.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/Print_Table.py` & `osbot_utils-1.7.7/osbot_utils/helpers/Print_Table.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/Python_Audit.py` & `osbot_utils-1.7.7/osbot_utils/helpers/Python_Audit.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/Random_Seed.py` & `osbot_utils-1.7.7/osbot_utils/helpers/Random_Seed.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/SCP.py` & `osbot_utils-1.7.7/osbot_utils/helpers/SCP.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/SSH.py` & `osbot_utils-1.7.7/osbot_utils/helpers/SSH.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Base.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Base.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Data.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Data.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Load.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Load.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Merge.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Merge.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Node.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Node.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Ast_Visit.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Ast_Visit.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/Call_Tree.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/Call_Tree.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/__init__.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Call.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Call.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Function_Def.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Function_Def.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/ast/nodes/Ast_Module.py` & `osbot_utils-1.7.7/osbot_utils/helpers/ast/nodes/Ast_Module.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Dict_To_Css.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Dict_To_Css.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Dict_To_Html.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Dict_To_Html.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Dict_To_Tags.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Dict_To_Tags.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Html_To_Dict.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Html_To_Dict.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Base.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Base.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Head.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Head.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Html.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Html.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/html/Tag__Style.py` & `osbot_utils-1.7.7/osbot_utils/helpers/html/Tag__Style.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/pubsub/Event__Queue.py` & `osbot_utils-1.7.7/osbot_utils/helpers/pubsub/Event__Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Client.py` & `osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Client.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Server.py` & `osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Server.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/pubsub/PubSub__Sqlite.py` & `osbot_utils-1.7.7/osbot_utils/helpers/pubsub/PubSub__Sqlite.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Capture_Sqlite_Error.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Capture_Sqlite_Error.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Cursor.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Cursor.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Database.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Database.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Field.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Field.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Table.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Table.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Sqlite__Table__Create.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Sqlite__Table__Create.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Temp_Sqlite__Database__Disk.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Temp_Sqlite__Database__Disk.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/Temp_Sqlite__Table.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/Temp_Sqlite__Table.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests__Patch.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__Cache__Requests__Patch.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Files.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Files.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Graph.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Graph.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Json.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Json.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Local.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Local.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Requests.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/domains/Sqlite__DB__Requests.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/models/Sqlite__Field__Type.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/models/Sqlite__Field__Type.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sample_data/Sqlite__Sample_Data__Chinook.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sample_data/Sqlite__Sample_Data__Chinook.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/sql_builder/SQL_Builder.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/sql_builder/SQL_Builder.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Config.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Config.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Edges.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Edges.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Files.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Files.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Nodes.py` & `osbot_utils-1.7.7/osbot_utils/helpers/sqlite/tables/Sqlite__Table__Nodes.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Config.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Config.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Graph.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Graph.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Handler.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Handler.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Print_Lines.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Print_Lines.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Print_Traces.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Print_Traces.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Stack.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Stack.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Stack_Node.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Stack_Node.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__Stats.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__Stats.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Call__View_Model.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Call__View_Model.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/helpers/trace/Trace_Files.py` & `osbot_utils-1.7.7/osbot_utils/helpers/trace/Trace_Files.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Catch.py` & `osbot_utils-1.7.7/osbot_utils/testing/Catch.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Duration.py` & `osbot_utils-1.7.7/osbot_utils/testing/Duration.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Hook_Method.py` & `osbot_utils-1.7.7/osbot_utils/testing/Hook_Method.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Log_To_Queue.py` & `osbot_utils-1.7.7/osbot_utils/testing/Log_To_Queue.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Log_To_String.py` & `osbot_utils-1.7.7/osbot_utils/testing/Log_To_String.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Logging.py` & `osbot_utils-1.7.7/osbot_utils/testing/Logging.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Patch_Print.py` & `osbot_utils-1.7.7/osbot_utils/testing/Patch_Print.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Profiler.py` & `osbot_utils-1.7.7/osbot_utils/testing/Profiler.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Temp_File.py` & `osbot_utils-1.7.7/osbot_utils/testing/Temp_File.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Temp_Folder.py` & `osbot_utils-1.7.7/osbot_utils/testing/Temp_Folder.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Temp_Web_Server.py` & `osbot_utils-1.7.7/osbot_utils/testing/Temp_Web_Server.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Temp_Zip.py` & `osbot_utils-1.7.7/osbot_utils/testing/Temp_Zip.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Temp_Zip_In_Memory.py` & `osbot_utils-1.7.7/osbot_utils/testing/Temp_Zip_In_Memory.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Unit_Test.py` & `osbot_utils-1.7.7/osbot_utils/testing/Unit_Test.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/testing/Unzip_File.py` & `osbot_utils-1.7.7/osbot_utils/testing/Unzip_File.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Assert.py` & `osbot_utils-1.7.7/osbot_utils/utils/Assert.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Call_Stack.py` & `osbot_utils-1.7.7/osbot_utils/utils/Call_Stack.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Csv.py` & `osbot_utils-1.7.7/osbot_utils/utils/Csv.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Dev.py` & `osbot_utils-1.7.7/osbot_utils/utils/Dev.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Files.py` & `osbot_utils-1.7.7/osbot_utils/utils/Files.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Functions.py` & `osbot_utils-1.7.7/osbot_utils/utils/Functions.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Http.py` & `osbot_utils-1.7.7/osbot_utils/utils/Http.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Json.py` & `osbot_utils-1.7.7/osbot_utils/utils/Json.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Json_Cache.py` & `osbot_utils-1.7.7/osbot_utils/utils/Json_Cache.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Lists.py` & `osbot_utils-1.7.7/osbot_utils/utils/Lists.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Misc.py` & `osbot_utils-1.7.7/osbot_utils/utils/Misc.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Objects.py` & `osbot_utils-1.7.7/osbot_utils/utils/Objects.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Png.py` & `osbot_utils-1.7.7/osbot_utils/utils/Png.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Process.py` & `osbot_utils-1.7.7/osbot_utils/utils/Process.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Python_Logger.py` & `osbot_utils-1.7.7/osbot_utils/utils/Python_Logger.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Status.py` & `osbot_utils-1.7.7/osbot_utils/utils/Status.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Str.py` & `osbot_utils-1.7.7/osbot_utils/utils/Str.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/osbot_utils/utils/Zip.py` & `osbot_utils-1.7.7/osbot_utils/utils/Zip.py`

 * *Files identical despite different names*

### Comparing `osbot_utils-1.7.1/pyproject.toml` & `osbot_utils-1.7.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 [tool.poetry]
 name        = "osbot_utils"
-version     = "v1.7.1"
+version     = "v1.7.7"
 description = "OWASP Security Bot - Utils"
 authors     = ["Dinis Cruz <dinis.cruz@owasp.org>"]
 license     = "MIT"
 readme      = "README.md"
 homepage    = "https://github.com/owasp-sbot/OSBot-Utils"
 repository  = "https://github.com/owasp-sbot/OSBot-Utils"
 
 [tool.poetry.dependencies]
-python          = "*"
+python          = "^3.11"
 python-dotenv   = "*"
-pyyaml          = "*"
+
+#[tool.poetry.group.test.dependencies]
+#pytest          = "*"
+#pytest-cov      = "*"
+#coveralls       = "*"
+
 
 [build-system]
 requires        = ["poetry-core>=1.0.0"]
 build-backend   = "poetry.core.masonry.api"
```

