# Comparing `tmp/superlinked-5.8.0.tar.gz` & `tmp/superlinked-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-5.8.0.tar", max compression
+gzip compressed data, was "superlinked-5.8.1.tar", max compression
```

## Comparing `superlinked-5.8.0.tar` & `superlinked-5.8.1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
--rw-r--r--   0        0        0    11354 2024-05-28 12:48:53.249241 superlinked-5.8.0/LICENSE
--rw-r--r--   0        0        0    28655 2024-05-28 12:48:53.249241 superlinked-5.8.0/NOTICE
--rw-r--r--   0        0        0     6840 2024-05-28 12:48:53.249241 superlinked-5.8.0/PYPI_README.md
--rw-r--r--   0        0        0     3698 2024-05-28 12:51:59.034314 superlinked-5.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/evaluation/charts/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     9028 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0      742 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/calculation/distance_metric.py
--rw-r--r--   0        0        0     1510 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      805 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0     2509 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/categorical_similarity_node.py
--rw-r--r--   0        0        0     1520 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     2095 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2606 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0     1106 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4985 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     1854 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/custom_node.py
--rw-r--r--   0        0        0     5923 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1338 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3687 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0     1004 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     2043 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1428 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     5016 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     3083 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     1620 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     2487 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1128 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1463 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1378 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     2250 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     8511 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5201 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py
--rw-r--r--   0        0        0     5890 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1535 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/custom_embedding.py
--rw-r--r--   0        0        0     1280 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/embedding.py
--rw-r--r--   0        0        0     3772 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     8046 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     2134 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1250 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5851 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      808 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/has_aggregation.py
--rw-r--r--   0        0        0      796 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/has_default_vector.py
--rw-r--r--   0        0        0      718 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      940 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1322 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5829 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     5402 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-05-28 12:48:53.297242 superlinked-5.8.0/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4634 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1396 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1533 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3189 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3228 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     6462 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     3170 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3220 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/space/__init__.py
--rw-r--r--   0        0        0     6450 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/space/aggregation.py
--rw-r--r--   0        0        0     2055 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/space/normalization.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      820 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/entity.py
--rw-r--r--   0        0        0      855 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/entity_data.py
--rw-r--r--   0        0        0      696 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/entity_id.py
--rw-r--r--   0        0        0      627 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/exception.py
--rw-r--r--   0        0        0     1656 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/field.py
--rw-r--r--   0        0        0     2627 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/field_data.py
--rw-r--r--   0        0        0      763 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/field_data_type.py
--rw-r--r--   0        0        0     3537 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/field_encoder.py
--rw-r--r--   0        0        0     2888 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/field_type_converter.py
--rw-r--r--   0        0        0      746 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0      769 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/result_entity_data.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/__init__.py
--rw-r--r--   0        0        0     1242 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
--rw-r--r--   0        0        0      671 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
--rw-r--r--   0        0        0      692 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
--rw-r--r--   0        0        0     2397 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/vdb_connector.py
--rw-r--r--   0        0        0     1095 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage/vdb_knn_search_params.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/__init__.py
--rw-r--r--   0        0        0     5459 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/admin_fields.py
--rw-r--r--   0        0        0     5549 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/entity_builder.py
--rw-r--r--   0        0        0      720 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/header.py
--rw-r--r--   0        0        0     1065 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/knn_search_params.py
--rw-r--r--   0        0        0      932 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/search_result_item.py
--rw-r--r--   0        0        0    16295 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/storage_manager.py
--rw-r--r--   0        0        0     1533 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/storage_manager/storage_naming.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0      787 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/collection_util.py
--rw-r--r--   0        0        0     2074 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0     1721 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/generic_class_util.py
--rw-r--r--   0        0        0      707 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0     1642 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/string_util.py
--rw-r--r--   0        0        0      907 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     4383 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     2399 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0      221 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     3836 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     7202 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     7323 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1540 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4834 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10985 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-05-28 12:48:53.301242 superlinked-5.8.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1183 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     4155 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     2739 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0     1128 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    13548 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6144 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0    11142 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     2613 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/registry/__init__.py
--rw-r--r--   0        0        0      636 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/registry/exception.py
--rw-r--r--   0        0        0     1330 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/registry/superlinked_registry.py
--rw-r--r--   0        0        0      214 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2103 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/source/data_loader_source.py
--rw-r--r--   0        0        0     2773 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0     7396 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/categorical_similarity_space.py
--rw-r--r--   0        0        0     5509 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/custom_space.py
--rw-r--r--   0        0        0      856 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     7702 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     8456 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2743 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1295 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4804 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     4808 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2237 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0      801 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/batched_chunk_input_item.py
--rw-r--r--   0        0        0     7597 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1213 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      768 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     6312 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3206 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_categorical_similarity_node.py
--rw-r--r--   0        0        0     3457 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2247 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5138 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2032 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     3282 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_custom_node.py
--rw-r--r--   0        0        0     7908 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     4052 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2351 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     5086 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     5547 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_node_registry.py
--rw-r--r--   0        0        0     3704 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     2713 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3732 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3426 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     3256 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0      794 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/parent_results.py
--rw-r--r--   0        0        0     1322 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/dag/parent_validator.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3877 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1437 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1752 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/__init__.py
--rw-r--r--   0        0        0      787 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/exception.py
--rw-r--r--   0        0        0     6725 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/in_memory_search.py
--rw-r--r--   0        0        0     7121 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/in_memory_vdb.py
--rw-r--r--   0        0        0      921 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/index_config.py
--rw-r--r--   0        0        0     1305 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/json_codec.py
--rw-r--r--   0        0        0     1562 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/framework/storage/in_memory/object_serializer.py
--rw-r--r--   0        0        0        0 2024-05-28 12:48:53.305242 superlinked-5.8.0/superlinked/py.typed
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-28 15:53:38.631380 superlinked-5.8.1/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-28 15:53:38.631380 superlinked-5.8.1/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-28 15:53:38.631380 superlinked-5.8.1/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-28 15:56:50.556151 superlinked-5.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     9028 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1510 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2509 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1520 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2095 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2606 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1106 2024-05-28 15:53:38.679380 superlinked-5.8.1/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1854 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3687 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2043 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1428 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     5016 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     3083 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     1620 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2487 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1463 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2250 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8511 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5201 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1535 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3772 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     8046 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      796 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/has_default_vector.py
+-rw-r--r--   0        0        0      718 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5829 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     5402 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4634 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1396 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1533 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3228 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     6462 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3220 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     6450 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2055 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      855 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1656 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2627 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      763 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3537 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0     2888 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/field_type_converter.py
+-rw-r--r--   0        0        0      746 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0      769 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/result_entity_data.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2397 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1095 2024-05-28 15:53:38.683380 superlinked-5.8.1/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     5459 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/admin_fields.py
+-rw-r--r--   0        0        0     5549 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0      720 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/header.py
+-rw-r--r--   0        0        0     1065 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      932 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/search_result_item.py
+-rw-r--r--   0        0        0    16295 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1533 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0     1721 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/generic_class_util.py
+-rw-r--r--   0        0        0      707 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0     1642 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     4383 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2399 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     3836 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7202 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     7323 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4834 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     4155 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     2739 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13548 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6144 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0    11142 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2613 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1330 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/source/data_loader_source.py
+-rw-r--r--   0        0        0     2773 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7396 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5509 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     7702 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8456 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2743 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1295 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.687380 superlinked-5.8.1/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     4808 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1213 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6312 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3206 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3457 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2247 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5138 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2032 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3282 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     7908 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4052 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2351 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     5086 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5547 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3704 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     2713 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3426 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3256 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3877 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1437 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6725 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/in_memory_search.py
+-rw-r--r--   0        0        0     7121 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/framework/storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:53:38.691380 superlinked-5.8.1/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.8.1/PKG-INFO
```

### Comparing `superlinked-5.8.0/LICENSE` & `superlinked-5.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/NOTICE` & `superlinked-5.8.1/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/PYPI_README.md` & `superlinked-5.8.1/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/pyproject.toml` & `superlinked-5.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superlinked"
-version = "5.8.0"  # The version will be dynamically updated
+version = "5.8.1"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
```

### Comparing `superlinked-5.8.0/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-5.8.1/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/evaluation/vector_sampler.py` & `superlinked-5.8.1/superlinked/evaluation/vector_sampler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/calculation/distance_metric.py` & `superlinked-5.8.1/superlinked/framework/common/calculation/distance_metric.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-5.8.1/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/const.py` & `superlinked-5.8.1/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/categorical_similarity_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/chunking_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/constant_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/context.py` & `superlinked-5.8.1/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/custom_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/dag.py` & `superlinked-5.8.1/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/dag_effect.py` & `superlinked-5.8.1/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/exception.py` & `superlinked-5.8.1/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/index_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/named_function_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/period_time.py` & `superlinked-5.8.1/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/persistence_params.py` & `superlinked-5.8.1/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/recency_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-5.8.1/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/schema_dag.py` & `superlinked-5.8.1/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-5.8.1/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-5.8.1/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/data_types.py` & `superlinked-5.8.1/superlinked/framework/common/data_types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/custom_embedding.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/embedding.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/number_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-5.8.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/exception.py` & `superlinked-5.8.1/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-5.8.1/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-5.8.1/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/has_aggregation.py` & `superlinked-5.8.1/superlinked/framework/common/interface/has_aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/has_default_vector.py` & `superlinked-5.8.1/superlinked/framework/common/interface/has_default_vector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/has_length.py` & `superlinked-5.8.1/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-5.8.1/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/interface/weighted.py` & `superlinked-5.8.1/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/observable.py` & `superlinked-5.8.1/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/parser/data_parser.py` & `superlinked-5.8.1/superlinked/framework/common/parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-5.8.1/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/parser/exception.py` & `superlinked-5.8.1/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/parser/json_parser.py` & `superlinked-5.8.1/superlinked/framework/common/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-5.8.1/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/event_schema.py` & `superlinked-5.8.1/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-5.8.1/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/exception.py` & `superlinked-5.8.1/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/general_type.py` & `superlinked-5.8.1/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-5.8.1/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema_factory.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema_object.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema_reference.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema_type.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/schema/schema_validator.py` & `superlinked-5.8.1/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/source/source.py` & `superlinked-5.8.1/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/source/types.py` & `superlinked-5.8.1/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/space/aggregation.py` & `superlinked-5.8.1/superlinked/framework/common/space/aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/space/normalization.py` & `superlinked-5.8.1/superlinked/framework/common/space/normalization.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/entity.py` & `superlinked-5.8.1/superlinked/framework/common/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/entity_data.py` & `superlinked-5.8.1/superlinked/framework/common/storage/entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/entity_id.py` & `superlinked-5.8.1/superlinked/framework/common/storage/entity_id.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/exception.py` & `superlinked-5.8.1/superlinked/framework/common/storage/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/field.py` & `superlinked-5.8.1/superlinked/framework/common/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/field_data.py` & `superlinked-5.8.1/superlinked/framework/common/storage/field_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/field_data_type.py` & `superlinked-5.8.1/superlinked/framework/common/storage/field_data_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/field_encoder.py` & `superlinked-5.8.1/superlinked/framework/common/storage/field_encoder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/field_type_converter.py` & `superlinked-5.8.1/superlinked/framework/common/storage/field_type_converter.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/persistence_type.py` & `superlinked-5.8.1/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/result_entity_data.py` & `superlinked-5.8.1/superlinked/framework/common/storage/result_entity_data.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py` & `superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py` & `superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py` & `superlinked-5.8.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/vdb_connector.py` & `superlinked-5.8.1/superlinked/framework/common/storage/vdb_connector.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage/vdb_knn_search_params.py` & `superlinked-5.8.1/superlinked/framework/common/storage/vdb_knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/admin_fields.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/admin_fields.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/entity_builder.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/entity_builder.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/header.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/header.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/knn_search_params.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/knn_search_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/search_result_item.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/search_result_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/storage_manager.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/storage_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/storage_manager/storage_naming.py` & `superlinked-5.8.1/superlinked/framework/common/storage_manager/storage_naming.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/collection_util.py` & `superlinked-5.8.1/superlinked/framework/common/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-5.8.1/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/generic_class_util.py` & `superlinked-5.8.1/superlinked/framework/common/util/generic_class_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/immutable_model.py` & `superlinked-5.8.1/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-5.8.1/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/string_util.py` & `superlinked-5.8.1/superlinked/framework/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/time_util.py` & `superlinked-5.8.1/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/common/util/type_validator.py` & `superlinked-5.8.1/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-5.8.1/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/exception.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/executor.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-5.8.1/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/effect.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/index.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-5.8.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/param.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/query.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/query.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/query_filters.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/query/result.py` & `superlinked-5.8.1/superlinked/framework/dsl/query/result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/registry/exception.py` & `superlinked-5.8.1/superlinked/framework/dsl/registry/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/registry/superlinked_registry.py` & `superlinked-5.8.1/superlinked/framework/dsl/registry/superlinked_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/source/data_loader_source.py` & `superlinked-5.8.1/superlinked/framework/dsl/source/data_loader_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     ORC = auto()
 
 
 @dataclass
 class DataLoaderConfig:
     path: str
     format: DataFormat
-    pandas_read_kwargs: dict[str, Any]
+    pandas_read_kwargs: dict[str, Any] | None = None
 
 
 class DataLoaderSource(Source, Generic[SchemaObjectT, SourceTypeT]):
     def __init__(
         self,
         schema: SchemaObjectT,
         data_loader_config: DataLoaderConfig,
```

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-5.8.1/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/source/rest_source.py` & `superlinked-5.8.1/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/source/source.py` & `superlinked-5.8.1/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/categorical_similarity_space.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/categorical_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/custom_space.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/custom_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/exception.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/number_space.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/number_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/recency_space.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/recency_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/space.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-5.8.1/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-5.8.1/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-5.8.1/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-5.8.1/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/batched_chunk_input_item.py` & `superlinked-5.8.1/superlinked/framework/online/dag/batched_chunk_input_item.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/default_online_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-5.8.1/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/exception.py` & `superlinked-5.8.1/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_categorical_similarity_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_categorical_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_custom_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_custom_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_index_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_named_function_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_node_registry.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_node_registry.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-5.8.1/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/parent_results.py` & `superlinked-5.8.1/superlinked/framework/online/dag/parent_results.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/dag/parent_validator.py` & `superlinked-5.8.1/superlinked/framework/online/dag/parent_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-5.8.1/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-5.8.1/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/online/source/in_memory_source.py` & `superlinked-5.8.1/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/storage/in_memory/exception.py` & `superlinked-5.8.1/superlinked/framework/storage/in_memory/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/storage/in_memory/in_memory_search.py` & `superlinked-5.8.1/superlinked/framework/storage/in_memory/in_memory_search.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/storage/in_memory/in_memory_vdb.py` & `superlinked-5.8.1/superlinked/framework/storage/in_memory/in_memory_vdb.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/storage/in_memory/index_config.py` & `superlinked-5.8.1/superlinked/framework/storage/in_memory/index_config.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/storage/in_memory/json_codec.py` & `superlinked-5.8.1/superlinked/framework/storage/in_memory/json_codec.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/superlinked/framework/storage/in_memory/object_serializer.py` & `superlinked-5.8.1/superlinked/framework/storage/in_memory/object_serializer.py`

 * *Files identical despite different names*

### Comparing `superlinked-5.8.0/PKG-INFO` & `superlinked-5.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 5.8.0
+Version: 5.8.1
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

