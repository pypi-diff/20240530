# Comparing `tmp/foundry_platform_sdk-0.3.0.tar.gz` & `tmp/foundry_platform_sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry_platform_sdk-0.3.0.tar", max compression
+gzip compressed data, was "foundry_platform_sdk-0.5.0.tar", max compression
```

## Comparing `foundry_platform_sdk-0.3.0.tar` & `foundry_platform_sdk-0.5.0.tar`

### file list

```diff
@@ -1,120 +1,718 @@
--rw-r--r--   0        0        0    11358 2024-01-24 20:37:37.654353 foundry_platform_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0    26141 2024-01-24 20:37:37.654353 foundry_platform_sdk-0.3.0/README.md
--rw-r--r--   0        0        0     2096 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/__init__.py
--rw-r--r--   0        0        0      601 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/__init__.py
--rw-r--r--   0        0        0     1091 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/auth_utils.py
--rw-r--r--   0        0        0     4802 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/confidential_client_auth.py
--rw-r--r--   0        0        0     1580 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/foundry_token_auth_client.py
--rw-r--r--   0        0        0      731 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/oauth.py
--rw-r--r--   0        0        0     8923 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/oauth_utils.py
--rw-r--r--   0        0        0     6461 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/palantir_session.py
--rw-r--r--   0        0        0     5384 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_core/public_client_auth.py
--rw-r--r--   0        0        0      655 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_errors/environment_not_configured.py
--rw-r--r--   0        0        0      843 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_errors/helpers.py
--rw-r--r--   0        0        0      647 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_errors/not_authenticated.py
--rw-r--r--   0        0        0     1044 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_errors/palantir_rpc_exception.py
--rw-r--r--   0        0        0     2709 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/_errors/sdk_internal_error.py
--rw-r--r--   0        0        0      874 2024-01-24 20:37:37.854353 foundry_platform_sdk-0.3.0/foundry/_versions.py
--rw-r--r--   0        0        0      875 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/api/__init__.py
--rw-r--r--   0        0        0    77203 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/api/datasets_api_service_api.py
--rw-r--r--   0        0        0    37677 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/api/ontologies_api_service_api.py
--rw-r--r--   0        0        0    44797 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/api/ontologies_v2_api_service_api.py
--rw-r--r--   0        0        0    16856 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/api_client.py
--rw-r--r--   0        0        0     1525 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/foundry_client.py
--rw-r--r--   0        0        0     7846 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/__init__.py
--rw-r--r--   0        0        0     5176 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/action_parameter_type.py
--rw-r--r--   0        0        0     3761 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/action_parameter_v2.py
--rw-r--r--   0        0        0     4973 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/action_type.py
--rw-r--r--   0        0        0     5003 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/action_type_v2.py
--rw-r--r--   0        0        0     3292 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/any_type.py
--rw-r--r--   0        0        0     3320 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/attachment_type.py
--rw-r--r--   0        0        0     3304 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/binary_type.py
--rw-r--r--   0        0        0     3308 2024-01-24 20:37:37.658353 foundry_platform_sdk-0.3.0/foundry/models/boolean_type.py
--rw-r--r--   0        0        0     3724 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/branch.py
--rw-r--r--   0        0        0     3296 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/byte_type.py
--rw-r--r--   0        0        0     3747 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/create_branch_request.py
--rw-r--r--   0        0        0     3429 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/create_dataset_request.py
--rw-r--r--   0        0        0     4602 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/create_link_rule.py
--rw-r--r--   0        0        0     3661 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/create_object_rule.py
--rw-r--r--   0        0        0     3501 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/create_transaction_request.py
--rw-r--r--   0        0        0     3571 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/dataset.py
--rw-r--r--   0        0        0     3296 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/date_type.py
--rw-r--r--   0        0        0     3431 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/decimal_type.py
--rw-r--r--   0        0        0     4602 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/delete_link_rule.py
--rw-r--r--   0        0        0     3661 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/delete_object_rule.py
--rw-r--r--   0        0        0     3583 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/deployment_api.py
--rw-r--r--   0        0        0     3625 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/deployment_listing.py
--rw-r--r--   0        0        0     3845 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/deployment_metadata.py
--rw-r--r--   0        0        0     4090 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/deployment_transform_api.py
--rw-r--r--   0        0        0     3304 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/double_type.py
--rw-r--r--   0        0        0     3890 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/file.py
--rw-r--r--   0        0        0     3300 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/float_type.py
--rw-r--r--   0        0        0     4950 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/geo_point.py
--rw-r--r--   0        0        0     3312 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/geo_point_type.py
--rw-r--r--   0        0        0     3312 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/geo_shape_type.py
--rw-r--r--   0        0        0     5786 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/geometry.py
--rw-r--r--   0        0        0     3308 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/integer_type.py
--rw-r--r--   0        0        0     4333 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/line_string.py
--rw-r--r--   0        0        0     4621 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/link_type_side.py
--rw-r--r--   0        0        0     1455 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/link_type_side_cardinality.py
--rw-r--r--   0        0        0     4627 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/link_type_side_v2.py
--rw-r--r--   0        0        0     4151 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_action_types_response.py
--rw-r--r--   0        0        0     4164 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_action_types_response_v2.py
--rw-r--r--   0        0        0     4215 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_branches_response.py
--rw-r--r--   0        0        0     3755 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_deployments_response.py
--rw-r--r--   0        0        0     4183 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_files_response.py
--rw-r--r--   0        0        0     4241 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_object_types_response.py
--rw-r--r--   0        0        0     4254 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_object_types_v2_response.py
--rw-r--r--   0        0        0     3800 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_ontologies_response.py
--rw-r--r--   0        0        0     3813 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_ontologies_v2_response.py
--rw-r--r--   0        0        0     4269 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_outgoing_link_types_response.py
--rw-r--r--   0        0        0     4282 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_outgoing_link_types_response_v2.py
--rw-r--r--   0        0        0     4145 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_query_types_response.py
--rw-r--r--   0        0        0     4158 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/list_query_types_response_v2.py
--rw-r--r--   0        0        0     2011 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/logic_rule.py
--rw-r--r--   0        0        0     3296 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/long_type.py
--rw-r--r--   0        0        0     3890 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/model_api_data_type.py
--rw-r--r--   0        0        0    15634 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/model_api_type.py
--rw-r--r--   0        0        0     6291 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/model_property.py
--rw-r--r--   0        0        0     3661 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/modify_object_rule.py
--rw-r--r--   0        0        0     4351 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/multi_line_string.py
--rw-r--r--   0        0        0     4140 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/multi_point.py
--rw-r--r--   0        0        0     4403 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/multi_polygon.py
--rw-r--r--   0        0        0     3296 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/null_type.py
--rw-r--r--   0        0        0     5474 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/object_property_type.py
--rw-r--r--   0        0        0     5246 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/object_type.py
--rw-r--r--   0        0        0     5241 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/object_type_v2.py
--rw-r--r--   0        0        0     1508 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/object_type_visibility.py
--rw-r--r--   0        0        0     4093 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/object_type_with_link.py
--rw-r--r--   0        0        0     3759 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/ontology.py
--rw-r--r--   0        0        0    16235 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/ontology_data_type.py
--rw-r--r--   0        0        0     5198 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/ontology_full_metadata.py
--rw-r--r--   0        0        0     4040 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/ontology_object_set_type.py
--rw-r--r--   0        0        0     3954 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/ontology_object_type.py
--rw-r--r--   0        0        0     3763 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/ontology_v2.py
--rw-r--r--   0        0        0     6511 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/parameter.py
--rw-r--r--   0        0        0     4319 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/polygon.py
--rw-r--r--   0        0        0     3854 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/property_v2.py
--rw-r--r--   0        0        0     2266 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_key_type.py
--rw-r--r--   0        0        0     1985 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_range_sub_type.py
--rw-r--r--   0        0        0     3711 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_range_type.py
--rw-r--r--   0        0        0     1909 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_value_type.py
--rw-r--r--   0        0        0    16088 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_data_type.py
--rw-r--r--   0        0        0     3690 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_parameter_v2.py
--rw-r--r--   0        0        0     4789 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_type.py
--rw-r--r--   0        0        0     4790 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/query_type_v2.py
--rw-r--r--   0        0        0     1497 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/release_status.py
--rw-r--r--   0        0        0     3300 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/short_type.py
--rw-r--r--   0        0        0     3304 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/string_type.py
--rw-r--r--   0        0        0     1456 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/table_export_format.py
--rw-r--r--   0        0        0     4062 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/three_dimensional_aggregation.py
--rw-r--r--   0        0        0     1807 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/time_series_item_type.py
--rw-r--r--   0        0        0     3659 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/timeseries_type.py
--rw-r--r--   0        0        0     3316 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/timestamp_type.py
--rw-r--r--   0        0        0     4230 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/transaction.py
--rw-r--r--   0        0        0     1484 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/transaction_status.py
--rw-r--r--   0        0        0     1500 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/transaction_type.py
--rw-r--r--   0        0        0     4055 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/two_dimensional_aggregation.py
--rw-r--r--   0        0        0     3448 2024-01-24 20:37:37.662353 foundry_platform_sdk-0.3.0/foundry/models/unsupported_type.py
--rw-r--r--   0        0        0      672 2024-01-24 20:37:38.334355 foundry_platform_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    27071 1970-01-01 00:00:00.000000 foundry_platform_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-29 22:42:43.121224 foundry_platform_sdk-0.5.0/LICENSE
+-rw-r--r--   0        0        0    64699 2024-05-29 22:42:43.121224 foundry_platform_sdk-0.5.0/README.md
+-rw-r--r--   0        0        0     1549 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/__init__.py
+-rw-r--r--   0        0        0      664 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/__init__.py
+-rw-r--r--   0        0        0     1125 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/auth_utils.py
+-rw-r--r--   0        0        0     4857 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/confidential_client_auth.py
+-rw-r--r--   0        0        0     1652 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/foundry_token_auth_client.py
+-rw-r--r--   0        0        0      732 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/oauth.py
+-rw-r--r--   0        0        0     8930 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/oauth_utils.py
+-rw-r--r--   0        0        0     2174 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/page_iterator.py
+-rw-r--r--   0        0        0     6702 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/palantir_session.py
+-rw-r--r--   0        0        0     5434 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/public_client_auth.py
+-rw-r--r--   0        0        0     1605 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/resource_iterator.py
+-rw-r--r--   0        0        0     2672 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_core/utils.py
+-rw-r--r--   0        0        0     1004 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_errors/__init__.py
+-rw-r--r--   0        0        0      655 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_errors/environment_not_configured.py
+-rw-r--r--   0        0        0      863 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_errors/helpers.py
+-rw-r--r--   0        0        0      647 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_errors/not_authenticated.py
+-rw-r--r--   0        0        0     1064 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_errors/palantir_rpc_exception.py
+-rw-r--r--   0        0        0     2508 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_errors/sdk_internal_error.py
+-rw-r--r--   0        0        0     9994 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/datasets/branch.py
+-rw-r--r--   0        0        0    13087 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/datasets/dataset.py
+-rw-r--r--   0        0        0    23990 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/datasets/file.py
+-rw-r--r--   0        0        0     8688 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/datasets/transaction.py
+-rw-r--r--   0        0        0     1486 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/namespaces.py
+-rw-r--r--   0        0        0     7034 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/ontologies/action_type.py
+-rw-r--r--   0        0        0    13153 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/ontologies/object_type.py
+-rw-r--r--   0        0        0     5931 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/ontologies/ontology.py
+-rw-r--r--   0        0        0     7011 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/ontologies/query_type.py
+-rw-r--r--   0        0        0    11133 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/security/group.py
+-rw-r--r--   0        0        0     9285 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/security/group_member.py
+-rw-r--r--   0        0        0     5426 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/security/group_membership.py
+-rw-r--r--   0        0        0    12000 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/_namespaces/security/user.py
+-rw-r--r--   0        0        0      788 2024-05-29 22:42:43.453224 foundry_platform_sdk-0.5.0/foundry/_versions.py
+-rw-r--r--   0        0        0     7648 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/api_client.py
+-rw-r--r--   0        0        0     1410 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/foundry_client.py
+-rw-r--r--   0        0        0    72970 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/__init__.py
+-rw-r--r--   0        0        0     1497 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_absolute_time_range.py
+-rw-r--r--   0        0        0     1112 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_absolute_time_range_dict.py
+-rw-r--r--   0        0        0      733 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_mode.py
+-rw-r--r--   0        0        0     2417 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_parameter_type.py
+-rw-r--r--   0        0        0     2205 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_parameter_type_dict.py
+-rw-r--r--   0        0        0     1452 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_parameter_v2.py
+-rw-r--r--   0        0        0     1124 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_parameter_v2_dict.py
+-rw-r--r--   0        0        0      950 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_results.py
+-rw-r--r--   0        0        0      986 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_results_dict.py
+-rw-r--r--   0        0        0      744 2024-05-29 22:42:43.153224 foundry_platform_sdk-0.5.0/foundry/models/_action_rid.py
+-rw-r--r--   0        0        0     1934 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_action_type.py
+-rw-r--r--   0        0        0      864 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_action_type_api_name.py
+-rw-r--r--   0        0        0     1609 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_action_type_dict.py
+-rw-r--r--   0        0        0      800 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_action_type_rid.py
+-rw-r--r--   0        0        0     1971 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_action_type_v2.py
+-rw-r--r--   0        0        0     1637 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_action_type_v2_dict.py
+-rw-r--r--   0        0        0     1482 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_add_group_members_request.py
+-rw-r--r--   0        0        0     1117 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_add_group_members_request_dict.py
+-rw-r--r--   0        0        0     1551 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_add_link.py
+-rw-r--r--   0        0        0     1140 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_add_link_dict.py
+-rw-r--r--   0        0        0     1394 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_add_object.py
+-rw-r--r--   0        0        0     1046 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_add_object_dict.py
+-rw-r--r--   0        0        0     1770 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_object_set_request_v2.py
+-rw-r--r--   0        0        0     1361 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_object_set_request_v2_dict.py
+-rw-r--r--   0        0        0     1552 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_request.py
+-rw-r--r--   0        0        0     1228 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_request_dict.py
+-rw-r--r--   0        0        0     1759 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_request_v2.py
+-rw-r--r--   0        0        0     1392 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_request_v2_dict.py
+-rw-r--r--   0        0        0     1640 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response.py
+-rw-r--r--   0        0        0     1224 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_dict.py
+-rw-r--r--   0        0        0     1590 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_item.py
+-rw-r--r--   0        0        0     1223 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_item_dict.py
+-rw-r--r--   0        0        0     1624 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_item_v2.py
+-rw-r--r--   0        0        0     1256 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_item_v2_dict.py
+-rw-r--r--   0        0        0     1662 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_v2.py
+-rw-r--r--   0        0        0     1247 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregate_objects_response_v2_dict.py
+-rw-r--r--   0        0        0     1403 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation.py
+-rw-r--r--   0        0        0      750 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_accuracy.py
+-rw-r--r--   0        0        0      778 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_accuracy_request.py
+-rw-r--r--   0        0        0     1494 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_dict.py
+-rw-r--r--   0        0        0     1611 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_duration_grouping.py
+-rw-r--r--   0        0        0     1236 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_duration_grouping_dict.py
+-rw-r--r--   0        0        0     1685 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_duration_grouping_v2.py
+-rw-r--r--   0        0        0     1301 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_duration_grouping_v2_dict.py
+-rw-r--r--   0        0        0     1511 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_exact_grouping.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_exact_grouping_dict.py
+-rw-r--r--   0        0        0     1551 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_exact_grouping_v2.py
+-rw-r--r--   0        0        0     1122 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_exact_grouping_v2_dict.py
+-rw-r--r--   0        0        0     1497 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_fixed_width_grouping.py
+-rw-r--r--   0        0        0     1057 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_fixed_width_grouping_dict.py
+-rw-r--r--   0        0        0     1520 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_fixed_width_grouping_v2.py
+-rw-r--r--   0        0        0     1071 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_fixed_width_grouping_v2_dict.py
+-rw-r--r--   0        0        0     1352 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_by.py
+-rw-r--r--   0        0        0     1442 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_by_dict.py
+-rw-r--r--   0        0        0     1399 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_by_v2.py
+-rw-r--r--   0        0        0     1498 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_by_v2_dict.py
+-rw-r--r--   0        0        0      729 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_key.py
+-rw-r--r--   0        0        0      733 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_key_v2.py
+-rw-r--r--   0        0        0      719 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_value.py
+-rw-r--r--   0        0        0      723 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_group_value_v2.py
+-rw-r--r--   0        0        0      766 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_metric_name.py
+-rw-r--r--   0        0        0     1313 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_metric_result.py
+-rw-r--r--   0        0        0     1001 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_metric_result_dict.py
+-rw-r--r--   0        0        0     1475 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_metric_result_v2.py
+-rw-r--r--   0        0        0     1125 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_metric_result_v2_dict.py
+-rw-r--r--   0        0        0     1386 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_object_type_grouping.py
+-rw-r--r--   0        0        0     1000 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_object_type_grouping_dict.py
+-rw-r--r--   0        0        0     1229 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_order_by.py
+-rw-r--r--   0        0        0      871 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_order_by_dict.py
+-rw-r--r--   0        0        0     1460 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_range.py
+-rw-r--r--   0        0        0     1166 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_range_dict.py
+-rw-r--r--   0        0        0     1369 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_range_v2.py
+-rw-r--r--   0        0        0      985 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_range_v2_dict.py
+-rw-r--r--   0        0        0     1477 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_ranges_grouping.py
+-rw-r--r--   0        0        0     1132 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_ranges_grouping_dict.py
+-rw-r--r--   0        0        0     1516 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_ranges_grouping_v2.py
+-rw-r--r--   0        0        0     1153 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_ranges_grouping_v2_dict.py
+-rw-r--r--   0        0        0     1618 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_v2.py
+-rw-r--r--   0        0        0     1713 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_aggregation_v2_dict.py
+-rw-r--r--   0        0        0     1538 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_all_terms_query.py
+-rw-r--r--   0        0        0     1268 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_all_terms_query_dict.py
+-rw-r--r--   0        0        0     1532 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_any_term_query.py
+-rw-r--r--   0        0        0     1266 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_any_term_query_dict.py
+-rw-r--r--   0        0        0     1101 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_any_type.py
+-rw-r--r--   0        0        0      845 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_any_type_dict.py
+-rw-r--r--   0        0        0      756 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_mode.py
+-rw-r--r--   0        0        0     1325 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_request.py
+-rw-r--r--   0        0        0     1025 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_request_dict.py
+-rw-r--r--   0        0        0     1499 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_request_options.py
+-rw-r--r--   0        0        0     1081 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_request_options_dict.py
+-rw-r--r--   0        0        0     1478 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_request_v2.py
+-rw-r--r--   0        0        0     1228 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_request_v2_dict.py
+-rw-r--r--   0        0        0     1121 2024-05-29 22:42:43.157224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_response.py
+-rw-r--r--   0        0        0      815 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_apply_action_response_dict.py
+-rw-r--r--   0        0        0     1568 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_approximate_distinct_aggregation.py
+-rw-r--r--   0        0        0     1191 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_approximate_distinct_aggregation_dict.py
+-rw-r--r--   0        0        0     1705 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_approximate_distinct_aggregation_v2.py
+-rw-r--r--   0        0        0     1315 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_approximate_distinct_aggregation_v2_dict.py
+-rw-r--r--   0        0        0     1862 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_approximate_percentile_aggregation_v2.py
+-rw-r--r--   0        0        0     1384 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_approximate_percentile_aggregation_v2_dict.py
+-rw-r--r--   0        0        0      739 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_archive_file_format.py
+-rw-r--r--   0        0        0     1540 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_array_size_constraint.py
+-rw-r--r--   0        0        0     1233 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_array_size_constraint_dict.py
+-rw-r--r--   0        0        0      732 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_artifact_repository_rid.py
+-rw-r--r--   0        0        0      945 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_action_status.py
+-rw-r--r--   0        0        0     1272 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_operation_response_v2.py
+-rw-r--r--   0        0        0      847 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_operation_response_v2_dict.py
+-rw-r--r--   0        0        0     1356 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_request.py
+-rw-r--r--   0        0        0     1035 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_request_dict.py
+-rw-r--r--   0        0        0     1399 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_request_v2.py
+-rw-r--r--   0        0        0     1039 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_request_v2_dict.py
+-rw-r--r--   0        0        0     1182 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_response.py
+-rw-r--r--   0        0        0      825 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_response_dict.py
+-rw-r--r--   0        0        0     1319 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_response_v2.py
+-rw-r--r--   0        0        0      888 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_async_apply_action_response_v2_dict.py
+-rw-r--r--   0        0        0     1475 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment.py
+-rw-r--r--   0        0        0     1125 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_dict.py
+-rw-r--r--   0        0        0     1022 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_metadata_response.py
+-rw-r--r--   0        0        0     1060 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_metadata_response_dict.py
+-rw-r--r--   0        0        0     1228 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_property.py
+-rw-r--r--   0        0        0      928 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_property_dict.py
+-rw-r--r--   0        0        0      751 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_rid.py
+-rw-r--r--   0        0        0     1150 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_type.py
+-rw-r--r--   0        0        0      866 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_type_dict.py
+-rw-r--r--   0        0        0     1542 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_v2.py
+-rw-r--r--   0        0        0     1184 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attachment_v2_dict.py
+-rw-r--r--   0        0        0      717 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attribute_name.py
+-rw-r--r--   0        0        0      719 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attribute_value.py
+-rw-r--r--   0        0        0      785 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_attribute_values.py
+-rw-r--r--   0        0        0     1409 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_avg_aggregation.py
+-rw-r--r--   0        0        0     1136 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_avg_aggregation_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_avg_aggregation_v2.py
+-rw-r--r--   0        0        0     1260 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_avg_aggregation_v2_dict.py
+-rw-r--r--   0        0        0     1195 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_b_box.py
+-rw-r--r--   0        0        0     1278 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request.py
+-rw-r--r--   0        0        0      970 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_item.py
+-rw-r--r--   0        0        0     1043 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_item_dict.py
+-rw-r--r--   0        0        0     1433 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_options.py
+-rw-r--r--   0        0        0      989 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_options_dict.py
+-rw-r--r--   0        0        0     1551 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_v2.py
+-rw-r--r--   0        0        0     1244 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_request_v2_dict.py
+-rw-r--r--   0        0        0     1182 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_response.py
+-rw-r--r--   0        0        0      825 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_response_dict.py
+-rw-r--r--   0        0        0     1332 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_response_v2.py
+-rw-r--r--   0        0        0      981 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_batch_apply_action_response_v2_dict.py
+-rw-r--r--   0        0        0     1122 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_binary_type.py
+-rw-r--r--   0        0        0      854 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_binary_type_dict.py
+-rw-r--r--   0        0        0     1129 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_boolean_type.py
+-rw-r--r--   0        0        0      857 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_boolean_type_dict.py
+-rw-r--r--   0        0        0     1403 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_bounding_box_value.py
+-rw-r--r--   0        0        0     1044 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_bounding_box_value_dict.py
+-rw-r--r--   0        0        0     1362 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_branch.py
+-rw-r--r--   0        0        0     1027 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_branch_dict.py
+-rw-r--r--   0        0        0      752 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_branch_id.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_byte_type.py
+-rw-r--r--   0        0        0      848 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_byte_type_dict.py
+-rw-r--r--   0        0        0     1289 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_center_point.py
+-rw-r--r--   0        0        0     1043 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_center_point_dict.py
+-rw-r--r--   0        0        0      738 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_center_point_types.py
+-rw-r--r--   0        0        0      755 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_center_point_types_dict.py
+-rw-r--r--   0        0        0     1251 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_completion_choice.py
+-rw-r--r--   0        0        0      965 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_completion_choice_dict.py
+-rw-r--r--   0        0        0     1836 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_completion_request.py
+-rw-r--r--   0        0        0     1537 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_completion_request_dict.py
+-rw-r--r--   0        0        0     1334 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_completion_response.py
+-rw-r--r--   0        0        0     1031 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_completion_response_dict.py
+-rw-r--r--   0        0        0     1261 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_message.py
+-rw-r--r--   0        0        0      999 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_message_dict.py
+-rw-r--r--   0        0        0      746 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_chat_message_role.py
+-rw-r--r--   0        0        0     1679 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_all_terms_in_order_prefix_last_term.py
+-rw-r--r--   0        0        0     1246 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_all_terms_in_order_prefix_last_term_dict.py
+-rw-r--r--   0        0        0     1556 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_all_terms_in_order_query.py
+-rw-r--r--   0        0        0     1174 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_all_terms_in_order_query_dict.py
+-rw-r--r--   0        0        0     1606 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_all_terms_query.py
+-rw-r--r--   0        0        0     1303 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_all_terms_query_dict.py
+-rw-r--r--   0        0        0     1600 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_any_term_query.py
+-rw-r--r--   0        0        0     1301 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_any_term_query_dict.py
+-rw-r--r--   0        0        0     1330 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_query.py
+-rw-r--r--   0        0        0     1051 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_query_dict.py
+-rw-r--r--   0        0        0     1353 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_query_v2.py
+-rw-r--r--   0        0        0     1065 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_contains_query_v2_dict.py
+-rw-r--r--   0        0        0      717 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_content_length.py
+-rw-r--r--   0        0        0      713 2024-05-29 22:42:43.161224 foundry_platform_sdk-0.5.0/foundry/models/_content_type.py
+-rw-r--r--   0        0        0      715 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_coordinate.py
+-rw-r--r--   0        0        0     1329 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_count_aggregation.py
+-rw-r--r--   0        0        0     1048 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_count_aggregation_dict.py
+-rw-r--r--   0        0        0     1454 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_count_aggregation_v2.py
+-rw-r--r--   0        0        0     1160 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_count_aggregation_v2_dict.py
+-rw-r--r--   0        0        0     1238 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_count_objects_response_v2.py
+-rw-r--r--   0        0        0      929 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_count_objects_response_v2_dict.py
+-rw-r--r--   0        0        0     1426 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_branch_request.py
+-rw-r--r--   0        0        0     1037 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_branch_request_dict.py
+-rw-r--r--   0        0        0     1346 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_dataset_request.py
+-rw-r--r--   0        0        0      975 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_dataset_request_dict.py
+-rw-r--r--   0        0        0     1761 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_group_request.py
+-rw-r--r--   0        0        0     1471 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_group_request_dict.py
+-rw-r--r--   0        0        0     1660 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_link_rule.py
+-rw-r--r--   0        0        0     1175 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_link_rule_dict.py
+-rw-r--r--   0        0        0     1339 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_object_rule.py
+-rw-r--r--   0        0        0      982 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_object_rule_dict.py
+-rw-r--r--   0        0        0     1390 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_temporary_object_set_request_v2.py
+-rw-r--r--   0        0        0      932 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_temporary_object_set_request_v2_dict.py
+-rw-r--r--   0        0        0     1413 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_temporary_object_set_response_v2.py
+-rw-r--r--   0        0        0      934 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_temporary_object_set_response_v2_dict.py
+-rw-r--r--   0        0        0     1385 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_transaction_request.py
+-rw-r--r--   0        0        0      980 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_create_transaction_request_dict.py
+-rw-r--r--   0        0        0      751 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_created_by.py
+-rw-r--r--   0        0        0      745 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_created_time.py
+-rw-r--r--   0        0        0      757 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_custom_type_id.py
+-rw-r--r--   0        0        0     4676 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_data_value.py
+-rw-r--r--   0        0        0     1338 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_dataset.py
+-rw-r--r--   0        0        0     1021 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_dataset_dict.py
+-rw-r--r--   0        0        0      713 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_dataset_name.py
+-rw-r--r--   0        0        0      816 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_dataset_rid.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_date_type.py
+-rw-r--r--   0        0        0      848 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_date_type_dict.py
+-rw-r--r--   0        0        0     1270 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_decimal_type.py
+-rw-r--r--   0        0        0     1004 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_decimal_type_dict.py
+-rw-r--r--   0        0        0     1660 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_delete_link_rule.py
+-rw-r--r--   0        0        0     1175 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_delete_link_rule_dict.py
+-rw-r--r--   0        0        0     1339 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_delete_object_rule.py
+-rw-r--r--   0        0        0      982 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_delete_object_rule_dict.py
+-rw-r--r--   0        0        0     1215 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_deploy_website_request.py
+-rw-r--r--   0        0        0      906 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_deploy_website_request_dict.py
+-rw-r--r--   0        0        0      733 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_display_name.py
+-rw-r--r--   0        0        0     1207 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_distance.py
+-rw-r--r--   0        0        0      948 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_distance_dict.py
+-rw-r--r--   0        0        0      856 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_distance_unit.py
+-rw-r--r--   0        0        0     1556 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_does_not_intersect_bounding_box_query.py
+-rw-r--r--   0        0        0     1171 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_does_not_intersect_bounding_box_query_dict.py
+-rw-r--r--   0        0        0     1513 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_does_not_intersect_polygon_query.py
+-rw-r--r--   0        0        0     1145 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_does_not_intersect_polygon_query_dict.py
+-rw-r--r--   0        0        0     1122 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_double_type.py
+-rw-r--r--   0        0        0      854 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_double_type_dict.py
+-rw-r--r--   0        0        0      730 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_duration.py
+-rw-r--r--   0        0        0     1318 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_equals_query.py
+-rw-r--r--   0        0        0     1047 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_equals_query_dict.py
+-rw-r--r--   0        0        0     1341 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_equals_query_v2.py
+-rw-r--r--   0        0        0     1061 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_equals_query_v2_dict.py
+-rw-r--r--   0        0        0     1331 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_execute_query_request.py
+-rw-r--r--   0        0        0     1027 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_execute_query_request_dict.py
+-rw-r--r--   0        0        0     1198 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_execute_query_response.py
+-rw-r--r--   0        0        0      889 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_execute_query_response_dict.py
+-rw-r--r--   0        0        0     1909 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature.py
+-rw-r--r--   0        0        0     1436 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature_collection.py
+-rw-r--r--   0        0        0     1164 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature_collection_dict.py
+-rw-r--r--   0        0        0      746 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature_collection_types.py
+-rw-r--r--   0        0        0      763 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature_collection_types_dict.py
+-rw-r--r--   0        0        0     1670 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature_dict.py
+-rw-r--r--   0        0        0      727 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_feature_property_key.py
+-rw-r--r--   0        0        0      790 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_field_name_v1.py
+-rw-r--r--   0        0        0     1486 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_file.py
+-rw-r--r--   0        0        0     1128 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_file_dict.py
+-rw-r--r--   0        0        0      809 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_file_path.py
+-rw-r--r--   0        0        0      732 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_filename.py
+-rw-r--r--   0        0        0     1114 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_filesystem_resource.py
+-rw-r--r--   0        0        0      813 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_filesystem_resource_dict.py
+-rw-r--r--   0        0        0      833 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_filter_value.py
+-rw-r--r--   0        0        0     1115 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_float_type.py
+-rw-r--r--   0        0        0      851 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_float_type_dict.py
+-rw-r--r--   0        0        0      708 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_folder_rid.py
+-rw-r--r--   0        0        0      794 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_function_rid.py
+-rw-r--r--   0        0        0      843 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_function_version.py
+-rw-r--r--   0        0        0      784 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_fuzzy.py
+-rw-r--r--   0        0        0      786 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_fuzzy_v2.py
+-rw-r--r--   0        0        0     2073 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_json_object.py
+-rw-r--r--   0        0        0     2194 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_json_object_dict.py
+-rw-r--r--   0        0        0     1282 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_point.py
+-rw-r--r--   0        0        0     1033 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_point_dict.py
+-rw-r--r--   0        0        0     1137 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_point_type.py
+-rw-r--r--   0        0        0      860 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_point_type_dict.py
+-rw-r--r--   0        0        0     1137 2024-05-29 22:42:43.165224 foundry_platform_sdk-0.5.0/foundry/models/_geo_shape_type.py
+-rw-r--r--   0        0        0      860 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_geo_shape_type_dict.py
+-rw-r--r--   0        0        0     2243 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_geometry.py
+-rw-r--r--   0        0        0     2104 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_geometry_dict.py
+-rw-r--r--   0        0        0     1813 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group.py
+-rw-r--r--   0        0        0     1577 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_dict.py
+-rw-r--r--   0        0        0     1335 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_member.py
+-rw-r--r--   0        0        0     1291 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_member_constraint.py
+-rw-r--r--   0        0        0      978 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_member_constraint_dict.py
+-rw-r--r--   0        0        0      974 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_member_dict.py
+-rw-r--r--   0        0        0     1228 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_membership.py
+-rw-r--r--   0        0        0      887 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_membership_dict.py
+-rw-r--r--   0        0        0      750 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_membership_expiration.py
+-rw-r--r--   0        0        0      709 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_name.py
+-rw-r--r--   0        0        0     1263 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_search_filter.py
+-rw-r--r--   0        0        0      966 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_group_search_filter_dict.py
+-rw-r--r--   0        0        0     1305 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gt_query.py
+-rw-r--r--   0        0        0     1050 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gt_query_dict.py
+-rw-r--r--   0        0        0     1328 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gt_query_v2.py
+-rw-r--r--   0        0        0     1064 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gt_query_v2_dict.py
+-rw-r--r--   0        0        0     1335 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gte_query.py
+-rw-r--r--   0        0        0     1076 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gte_query_dict.py
+-rw-r--r--   0        0        0     1358 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gte_query_v2.py
+-rw-r--r--   0        0        0     1090 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_gte_query_v2_dict.py
+-rw-r--r--   0        0        0     1129 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_integer_type.py
+-rw-r--r--   0        0        0      857 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_integer_type_dict.py
+-rw-r--r--   0        0        0     2331 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type.py
+-rw-r--r--   0        0        0      778 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type_api_name.py
+-rw-r--r--   0        0        0      934 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type_cardinality.py
+-rw-r--r--   0        0        0     1920 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type_dict.py
+-rw-r--r--   0        0        0     1124 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type_linked_entity_api_name.py
+-rw-r--r--   0        0        0     1171 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type_linked_entity_api_name_dict.py
+-rw-r--r--   0        0        0      815 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_link_type_rid.py
+-rw-r--r--   0        0        0     2755 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_type.py
+-rw-r--r--   0        0        0      901 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_type_api_name.py
+-rw-r--r--   0        0        0     2393 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_type_dict.py
+-rw-r--r--   0        0        0      801 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_interface_type_rid.py
+-rw-r--r--   0        0        0     1510 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_intersects_bounding_box_query.py
+-rw-r--r--   0        0        0     1151 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_intersects_bounding_box_query_dict.py
+-rw-r--r--   0        0        0     1428 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_intersects_polygon_query.py
+-rw-r--r--   0        0        0     1125 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_intersects_polygon_query_dict.py
+-rw-r--r--   0        0        0     1313 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_is_null_query.py
+-rw-r--r--   0        0        0     1041 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_is_null_query_dict.py
+-rw-r--r--   0        0        0     1336 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_is_null_query_v2.py
+-rw-r--r--   0        0        0     1055 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_is_null_query_v2_dict.py
+-rw-r--r--   0        0        0     1432 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_language_model.py
+-rw-r--r--   0        0        0      833 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_language_model_api_name.py
+-rw-r--r--   0        0        0     1098 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_language_model_dict.py
+-rw-r--r--   0        0        0      743 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_language_model_source.py
+-rw-r--r--   0        0        0     1357 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_line_string.py
+-rw-r--r--   0        0        0      828 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_line_string_coordinates.py
+-rw-r--r--   0        0        0     1096 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_line_string_dict.py
+-rw-r--r--   0        0        0     1181 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_linear_ring.py
+-rw-r--r--   0        0        0     1366 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_side_object.py
+-rw-r--r--   0        0        0      996 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_side_object_dict.py
+-rw-r--r--   0        0        0      830 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_type_api_name.py
+-rw-r--r--   0        0        0     1913 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_type_side.py
+-rw-r--r--   0        0        0      746 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_type_side_cardinality.py
+-rw-r--r--   0        0        0     1457 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_type_side_dict.py
+-rw-r--r--   0        0        0     1926 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_type_side_v2.py
+-rw-r--r--   0        0        0     1461 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_link_type_side_v2_dict.py
+-rw-r--r--   0        0        0     1450 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_linked_interface_type_api_name.py
+-rw-r--r--   0        0        0     1024 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_linked_interface_type_api_name_dict.py
+-rw-r--r--   0        0        0     1381 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_linked_object_type_api_name.py
+-rw-r--r--   0        0        0     1006 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_linked_object_type_api_name_dict.py
+-rw-r--r--   0        0        0     1440 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_action_types_response.py
+-rw-r--r--   0        0        0     1075 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_action_types_response_dict.py
+-rw-r--r--   0        0        0     1490 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_action_types_response_v2.py
+-rw-r--r--   0        0        0     1086 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_action_types_response_v2_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_attachments_response_v2.py
+-rw-r--r--   0        0        0     1143 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_attachments_response_v2_dict.py
+-rw-r--r--   0        0        0     1460 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_branches_response.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_branches_response_dict.py
+-rw-r--r--   0        0        0     1453 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_files_response.py
+-rw-r--r--   0        0        0     1113 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_files_response_dict.py
+-rw-r--r--   0        0        0     1479 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_group_members_response.py
+-rw-r--r--   0        0        0     1080 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_group_members_response_dict.py
+-rw-r--r--   0        0        0     1524 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_group_memberships_response.py
+-rw-r--r--   0        0        0     1100 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_group_memberships_response_dict.py
+-rw-r--r--   0        0        0     1393 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_groups_response.py
+-rw-r--r--   0        0        0     1049 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_groups_response_dict.py
+-rw-r--r--   0        0        0     1506 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_interface_types_response.py
+-rw-r--r--   0        0        0     1090 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_interface_types_response_dict.py
+-rw-r--r--   0        0        0     1354 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_language_models_response.py
+-rw-r--r--   0        0        0      995 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_language_models_response_dict.py
+-rw-r--r--   0        0        0     1494 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_linked_objects_response.py
+-rw-r--r--   0        0        0     1091 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_linked_objects_response_dict.py
+-rw-r--r--   0        0        0     1523 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_linked_objects_response_v2.py
+-rw-r--r--   0        0        0     1089 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_linked_objects_response_v2_dict.py
+-rw-r--r--   0        0        0     1496 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_object_types_response.py
+-rw-r--r--   0        0        0     1131 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_object_types_response_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_object_types_v2_response.py
+-rw-r--r--   0        0        0     1142 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_object_types_v2_response_dict.py
+-rw-r--r--   0        0        0     1478 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_objects_response.py
+-rw-r--r--   0        0        0     1130 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_objects_response_dict.py
+-rw-r--r--   0        0        0     1498 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_objects_response_v2.py
+-rw-r--r--   0        0        0     1128 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_objects_response_v2_dict.py
+-rw-r--r--   0        0        0     1292 2024-05-29 22:42:43.169224 foundry_platform_sdk-0.5.0/foundry/models/_list_ontologies_response.py
+-rw-r--r--   0        0        0      989 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_ontologies_response_dict.py
+-rw-r--r--   0        0        0     1342 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_ontologies_v2_response.py
+-rw-r--r--   0        0        0     1000 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_ontologies_v2_response_dict.py
+-rw-r--r--   0        0        0     1582 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_outgoing_link_types_response.py
+-rw-r--r--   0        0        0     1153 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_outgoing_link_types_response_dict.py
+-rw-r--r--   0        0        0     1602 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_outgoing_link_types_response_v2.py
+-rw-r--r--   0        0        0     1164 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_outgoing_link_types_response_v2_dict.py
+-rw-r--r--   0        0        0     1431 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_query_types_response.py
+-rw-r--r--   0        0        0     1070 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_query_types_response_dict.py
+-rw-r--r--   0        0        0     1481 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_query_types_response_v2.py
+-rw-r--r--   0        0        0     1081 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_query_types_response_v2_dict.py
+-rw-r--r--   0        0        0     1384 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_users_response.py
+-rw-r--r--   0        0        0     1044 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_users_response_dict.py
+-rw-r--r--   0        0        0     1411 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_versions_response.py
+-rw-r--r--   0        0        0     1059 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_list_versions_response_dict.py
+-rw-r--r--   0        0        0     2154 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_load_object_set_request_v2.py
+-rw-r--r--   0        0        0     1667 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_load_object_set_request_v2_dict.py
+-rw-r--r--   0        0        0     1544 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_load_object_set_response_v2.py
+-rw-r--r--   0        0        0     1165 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_load_object_set_response_v2_dict.py
+-rw-r--r--   0        0        0     1085 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_local_file_path.py
+-rw-r--r--   0        0        0      803 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_local_file_path_dict.py
+-rw-r--r--   0        0        0     1206 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_logic_rule.py
+-rw-r--r--   0        0        0     1322 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_logic_rule_dict.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_long_type.py
+-rw-r--r--   0        0        0      848 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_long_type_dict.py
+-rw-r--r--   0        0        0     1299 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lt_query.py
+-rw-r--r--   0        0        0     1044 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lt_query_dict.py
+-rw-r--r--   0        0        0     1322 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lt_query_v2.py
+-rw-r--r--   0        0        0     1058 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lt_query_v2_dict.py
+-rw-r--r--   0        0        0     1329 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lte_query.py
+-rw-r--r--   0        0        0     1070 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lte_query_dict.py
+-rw-r--r--   0        0        0     1352 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lte_query_v2.py
+-rw-r--r--   0        0        0     1084 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_lte_query_v2_dict.py
+-rw-r--r--   0        0        0     1129 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_marking_type.py
+-rw-r--r--   0        0        0      857 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_marking_type_dict.py
+-rw-r--r--   0        0        0     1409 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_max_aggregation.py
+-rw-r--r--   0        0        0     1136 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_max_aggregation_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_max_aggregation_v2.py
+-rw-r--r--   0        0        0     1260 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_max_aggregation_v2_dict.py
+-rw-r--r--   0        0        0      899 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_media_type.py
+-rw-r--r--   0        0        0     1409 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_min_aggregation.py
+-rw-r--r--   0        0        0     1136 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_min_aggregation_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_min_aggregation_v2.py
+-rw-r--r--   0        0        0     1260 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_min_aggregation_v2_dict.py
+-rw-r--r--   0        0        0     1415 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_modify_object.py
+-rw-r--r--   0        0        0     1055 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_modify_object_dict.py
+-rw-r--r--   0        0        0     1339 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_modify_object_rule.py
+-rw-r--r--   0        0        0      982 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_modify_object_rule_dict.py
+-rw-r--r--   0        0        0     1406 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_multi_line_string.py
+-rw-r--r--   0        0        0     1128 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_multi_line_string_dict.py
+-rw-r--r--   0        0        0     1329 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_multi_point.py
+-rw-r--r--   0        0        0     1072 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_multi_point_dict.py
+-rw-r--r--   0        0        0     1356 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_multi_polygon.py
+-rw-r--r--   0        0        0     1091 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_multi_polygon_dict.py
+-rw-r--r--   0        0        0     1299 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_nested_query_aggregation.py
+-rw-r--r--   0        0        0      996 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_nested_query_aggregation_dict.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_null_type.py
+-rw-r--r--   0        0        0      848 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_null_type_dict.py
+-rw-r--r--   0        0        0      982 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_edit.py
+-rw-r--r--   0        0        0     1031 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_edit_dict.py
+-rw-r--r--   0        0        0     1648 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_edits.py
+-rw-r--r--   0        0        0     1176 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_edits_dict.py
+-rw-r--r--   0        0        0     2698 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_property_type.py
+-rw-r--r--   0        0        0     2577 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_property_type_dict.py
+-rw-r--r--   0        0        0     1346 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_property_value_constraint.py
+-rw-r--r--   0        0        0      961 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_property_value_constraint_dict.py
+-rw-r--r--   0        0        0     1333 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_query_result_constraint.py
+-rw-r--r--   0        0        0      956 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_query_result_constraint_dict.py
+-rw-r--r--   0        0        0      791 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_rid.py
+-rw-r--r--   0        0        0     4251 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set.py
+-rw-r--r--   0        0        0     1278 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_base_type.py
+-rw-r--r--   0        0        0      924 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_base_type_dict.py
+-rw-r--r--   0        0        0     2716 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_dict.py
+-rw-r--r--   0        0        0     1255 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_reference_type.py
+-rw-r--r--   0        0        0      938 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_reference_type_dict.py
+-rw-r--r--   0        0        0      714 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_rid.py
+-rw-r--r--   0        0        0     1281 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_static_type.py
+-rw-r--r--   0        0        0      976 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_set_static_type_dict.py
+-rw-r--r--   0        0        0     2277 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type.py
+-rw-r--r--   0        0        0      884 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_api_name.py
+-rw-r--r--   0        0        0     1906 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_dict.py
+-rw-r--r--   0        0        0     1365 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_edits.py
+-rw-r--r--   0        0        0     1013 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_edits_dict.py
+-rw-r--r--   0        0        0     2486 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_full_metadata.py
+-rw-r--r--   0        0        0     1971 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_full_metadata_dict.py
+-rw-r--r--   0        0        0     1494 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_interface_implementation.py
+-rw-r--r--   0        0        0     1081 2024-05-29 22:42:43.173224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_interface_implementation_dict.py
+-rw-r--r--   0        0        0      800 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_rid.py
+-rw-r--r--   0        0        0     2213 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_v2.py
+-rw-r--r--   0        0        0     1801 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_v2_dict.py
+-rw-r--r--   0        0        0      782 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_object_type_visibility.py
+-rw-r--r--   0        0        0     1624 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_one_of_constraint.py
+-rw-r--r--   0        0        0     1284 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_one_of_constraint_dict.py
+-rw-r--r--   0        0        0     1464 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology.py
+-rw-r--r--   0        0        0      721 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_api_name.py
+-rw-r--r--   0        0        0     5020 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_data_type.py
+-rw-r--r--   0        0        0     3737 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_data_type_dict.py
+-rw-r--r--   0        0        0     1122 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_dict.py
+-rw-r--r--   0        0        0     2401 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_full_metadata.py
+-rw-r--r--   0        0        0     1969 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_full_metadata_dict.py
+-rw-r--r--   0        0        0      756 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_identifier.py
+-rw-r--r--   0        0        0     1471 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object.py
+-rw-r--r--   0        0        0     1188 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object_dict.py
+-rw-r--r--   0        0        0     1528 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object_set_type.py
+-rw-r--r--   0        0        0     1095 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object_set_type_dict.py
+-rw-r--r--   0        0        0     1416 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object_type.py
+-rw-r--r--   0        0        0     1018 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object_type_dict.py
+-rw-r--r--   0        0        0      884 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_object_v2.py
+-rw-r--r--   0        0        0      863 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_rid.py
+-rw-r--r--   0        0        0     1475 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_v2.py
+-rw-r--r--   0        0        0     1124 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_ontology_v2_dict.py
+-rw-r--r--   0        0        0     1391 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_order_by.py
+-rw-r--r--   0        0        0      732 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_order_by_direction.py
+-rw-r--r--   0        0        0      720 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_organization_rid.py
+-rw-r--r--   0        0        0      737 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_page_size.py
+-rw-r--r--   0        0        0      972 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_page_token.py
+-rw-r--r--   0        0        0     1535 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter.py
+-rw-r--r--   0        0        0     1203 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_dict.py
+-rw-r--r--   0        0        0     4917 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_evaluated_constraint.py
+-rw-r--r--   0        0        0     5081 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_evaluated_constraint_dict.py
+-rw-r--r--   0        0        0     1705 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_evaluation_result.py
+-rw-r--r--   0        0        0     1311 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_evaluation_result_dict.py
+-rw-r--r--   0        0        0      875 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_id.py
+-rw-r--r--   0        0        0      748 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_key.py
+-rw-r--r--   0        0        0     1499 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_option.py
+-rw-r--r--   0        0        0     1154 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_option_dict.py
+-rw-r--r--   0        0        0      705 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_parameter_value.py
+-rw-r--r--   0        0        0     1333 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_phrase_query.py
+-rw-r--r--   0        0        0     1062 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_phrase_query_dict.py
+-rw-r--r--   0        0        0     1314 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_polygon.py
+-rw-r--r--   0        0        0     1070 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_polygon_dict.py
+-rw-r--r--   0        0        0      726 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_polygon_value.py
+-rw-r--r--   0        0        0      743 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_polygon_value_dict.py
+-rw-r--r--   0        0        0     1557 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_position.py
+-rw-r--r--   0        0        0     1321 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_prefix_query.py
+-rw-r--r--   0        0        0     1050 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_prefix_query_dict.py
+-rw-r--r--   0        0        0      745 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_preview_mode.py
+-rw-r--r--   0        0        0      775 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_primary_key_value.py
+-rw-r--r--   0        0        0      738 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_principal_filter_type.py
+-rw-r--r--   0        0        0      737 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_principal_id.py
+-rw-r--r--   0        0        0      728 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_principal_type.py
+-rw-r--r--   0        0        0     1455 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property.py
+-rw-r--r--   0        0        0      854 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_api_name.py
+-rw-r--r--   0        0        0     1111 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_dict.py
+-rw-r--r--   0        0        0     2671 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_filter.py
+-rw-r--r--   0        0        0      922 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_id.py
+-rw-r--r--   0        0        0     1494 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_v2.py
+-rw-r--r--   0        0        0     1154 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_v2_dict.py
+-rw-r--r--   0        0        0     3676 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_value.py
+-rw-r--r--   0        0        0      801 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_property_value_escaped_string.py
+-rw-r--r--   0        0        0     1155 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation.py
+-rw-r--r--   0        0        0      863 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_dict.py
+-rw-r--r--   0        0        0     1434 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_key_type.py
+-rw-r--r--   0        0        0     1537 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_key_type_dict.py
+-rw-r--r--   0        0        0     1460 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_range.py
+-rw-r--r--   0        0        0     1056 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_range_dict.py
+-rw-r--r--   0        0        0     1134 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_range_sub_type.py
+-rw-r--r--   0        0        0     1195 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_range_sub_type_dict.py
+-rw-r--r--   0        0        0     1437 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_range_type.py
+-rw-r--r--   0        0        0     1047 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_range_type_dict.py
+-rw-r--r--   0        0        0     1063 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_value_type.py
+-rw-r--r--   0        0        0     1106 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_aggregation_value_type_dict.py
+-rw-r--r--   0        0        0      736 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_api_name.py
+-rw-r--r--   0        0        0     4774 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_data_type.py
+-rw-r--r--   0        0        0     3567 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_data_type_dict.py
+-rw-r--r--   0        0        0     1307 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_output_v2.py
+-rw-r--r--   0        0        0      985 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_output_v2_dict.py
+-rw-r--r--   0        0        0     1369 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_parameter_v2.py
+-rw-r--r--   0        0        0     1045 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_parameter_v2_dict.py
+-rw-r--r--   0        0        0     1381 2024-05-29 22:42:43.177224 foundry_platform_sdk-0.5.0/foundry/models/_query_three_dimensional_aggregation.py
+-rw-r--r--   0        0        0      998 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_three_dimensional_aggregation_dict.py
+-rw-r--r--   0        0        0     1350 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_two_dimensional_aggregation.py
+-rw-r--r--   0        0        0      975 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_two_dimensional_aggregation_dict.py
+-rw-r--r--   0        0        0     1916 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_type.py
+-rw-r--r--   0        0        0     1591 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_type_dict.py
+-rw-r--r--   0        0        0     1924 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_type_v2.py
+-rw-r--r--   0        0        0     1594 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_query_type_v2_dict.py
+-rw-r--r--   0        0        0     1466 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_range_constraint.py
+-rw-r--r--   0        0        0     1176 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_range_constraint_dict.py
+-rw-r--r--   0        0        0      898 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_realm.py
+-rw-r--r--   0        0        0     1426 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_relative_time.py
+-rw-r--r--   0        0        0     1150 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_relative_time_dict.py
+-rw-r--r--   0        0        0     1464 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_relative_time_range.py
+-rw-r--r--   0        0        0     1096 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_relative_time_range_dict.py
+-rw-r--r--   0        0        0      744 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_relative_time_relation.py
+-rw-r--r--   0        0        0      826 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_relative_time_series_time_unit.py
+-rw-r--r--   0        0        0      771 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_release_status.py
+-rw-r--r--   0        0        0     1360 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_remove_group_members_request.py
+-rw-r--r--   0        0        0      943 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_remove_group_members_request_dict.py
+-rw-r--r--   0        0        0      735 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_resource_path.py
+-rw-r--r--   0        0        0      730 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_return_edits_mode.py
+-rw-r--r--   0        0        0      719 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sdk_package_name.py
+-rw-r--r--   0        0        0     1521 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_groups_request.py
+-rw-r--r--   0        0        0     1139 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_groups_request_dict.py
+-rw-r--r--   0        0        0     1405 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_groups_response.py
+-rw-r--r--   0        0        0     1053 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_groups_response_dict.py
+-rw-r--r--   0        0        0     3168 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_json_query.py
+-rw-r--r--   0        0        0     2571 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_json_query_dict.py
+-rw-r--r--   0        0        0     4401 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_json_query_v2.py
+-rw-r--r--   0        0        0     3916 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_json_query_v2_dict.py
+-rw-r--r--   0        0        0     3965 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_for_interface_request.py
+-rw-r--r--   0        0        0     3208 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_for_interface_request_dict.py
+-rw-r--r--   0        0        0     1860 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_request.py
+-rw-r--r--   0        0        0     1451 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_request_dict.py
+-rw-r--r--   0        0        0     2186 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_request_v2.py
+-rw-r--r--   0        0        0     1724 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_request_v2_dict.py
+-rw-r--r--   0        0        0     1439 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_response.py
+-rw-r--r--   0        0        0     1083 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_response_dict.py
+-rw-r--r--   0        0        0     1459 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_response_v2.py
+-rw-r--r--   0        0        0     1081 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_objects_response_v2_dict.py
+-rw-r--r--   0        0        0     1267 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_order_by.py
+-rw-r--r--   0        0        0     1000 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_order_by_dict.py
+-rw-r--r--   0        0        0     1285 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_order_by_v2.py
+-rw-r--r--   0        0        0     1009 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_order_by_v2_dict.py
+-rw-r--r--   0        0        0     1345 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_ordering.py
+-rw-r--r--   0        0        0     1071 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_ordering_dict.py
+-rw-r--r--   0        0        0     1370 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_ordering_v2.py
+-rw-r--r--   0        0        0     1087 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_ordering_v2_dict.py
+-rw-r--r--   0        0        0     1512 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_users_request.py
+-rw-r--r--   0        0        0     1134 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_users_request_dict.py
+-rw-r--r--   0        0        0     1396 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_users_response.py
+-rw-r--r--   0        0        0     1048 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_search_users_response_dict.py
+-rw-r--r--   0        0        0     1533 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_selected_property_api_name.py
+-rw-r--r--   0        0        0     1844 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_shared_property_type.py
+-rw-r--r--   0        0        0      924 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_shared_property_type_api_name.py
+-rw-r--r--   0        0        0     1456 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_shared_property_type_dict.py
+-rw-r--r--   0        0        0      817 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_shared_property_type_rid.py
+-rw-r--r--   0        0        0     1115 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_short_type.py
+-rw-r--r--   0        0        0      851 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_short_type_dict.py
+-rw-r--r--   0        0        0      744 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_size_bytes.py
+-rw-r--r--   0        0        0     1358 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_starts_with_query.py
+-rw-r--r--   0        0        0     1070 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_starts_with_query_dict.py
+-rw-r--r--   0        0        0     1338 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_stream_time_series_points_request.py
+-rw-r--r--   0        0        0      975 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_stream_time_series_points_request_dict.py
+-rw-r--r--   0        0        0     1347 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_stream_time_series_points_response.py
+-rw-r--r--   0        0        0      971 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_stream_time_series_points_response_dict.py
+-rw-r--r--   0        0        0     1568 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_string_length_constraint.py
+-rw-r--r--   0        0        0     1249 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_string_length_constraint_dict.py
+-rw-r--r--   0        0        0     1764 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_string_regex_match_constraint.py
+-rw-r--r--   0        0        0     1309 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_string_regex_match_constraint_dict.py
+-rw-r--r--   0        0        0     1122 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_string_type.py
+-rw-r--r--   0        0        0      854 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_string_type_dict.py
+-rw-r--r--   0        0        0      740 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_struct_field_name.py
+-rw-r--r--   0        0        0      743 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_subdomain.py
+-rw-r--r--   0        0        0     1889 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_submission_criteria_evaluation.py
+-rw-r--r--   0        0        0     1427 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_submission_criteria_evaluation_dict.py
+-rw-r--r--   0        0        0     1409 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sum_aggregation.py
+-rw-r--r--   0        0        0     1136 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sum_aggregation_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sum_aggregation_v2.py
+-rw-r--r--   0        0        0     1260 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sum_aggregation_v2_dict.py
+-rw-r--r--   0        0        0     1457 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sync_apply_action_response_v2.py
+-rw-r--r--   0        0        0     1136 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_sync_apply_action_response_v2_dict.py
+-rw-r--r--   0        0        0      752 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_table_export_format.py
+-rw-r--r--   0        0        0     1334 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_third_party_application.py
+-rw-r--r--   0        0        0     1021 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_third_party_application_dict.py
+-rw-r--r--   0        0        0      788 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_third_party_application_rid.py
+-rw-r--r--   0        0        0     1607 2024-05-29 22:42:43.181224 foundry_platform_sdk-0.5.0/foundry/models/_three_dimensional_aggregation.py
+-rw-r--r--   0        0        0     1185 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_three_dimensional_aggregation_dict.py
+-rw-r--r--   0        0        0     1012 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_range.py
+-rw-r--r--   0        0        0     1048 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_range_dict.py
+-rw-r--r--   0        0        0      980 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_series_item_type.py
+-rw-r--r--   0        0        0     1016 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_series_item_type_dict.py
+-rw-r--r--   0        0        0     1307 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_series_point.py
+-rw-r--r--   0        0        0     1019 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_series_point_dict.py
+-rw-r--r--   0        0        0      802 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_time_unit.py
+-rw-r--r--   0        0        0     1307 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_timeseries_type.py
+-rw-r--r--   0        0        0      983 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_timeseries_type_dict.py
+-rw-r--r--   0        0        0     1143 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_timestamp_type.py
+-rw-r--r--   0        0        0      863 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_timestamp_type_dict.py
+-rw-r--r--   0        0        0     1834 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_transaction.py
+-rw-r--r--   0        0        0     1446 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_transaction_dict.py
+-rw-r--r--   0        0        0      828 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_transaction_rid.py
+-rw-r--r--   0        0        0      762 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_transaction_status.py
+-rw-r--r--   0        0        0      768 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_transaction_type.py
+-rw-r--r--   0        0        0     1585 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_two_dimensional_aggregation.py
+-rw-r--r--   0        0        0     1180 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_two_dimensional_aggregation_dict.py
+-rw-r--r--   0        0        0     1409 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_unevaluable_constraint.py
+-rw-r--r--   0        0        0     1097 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_unevaluable_constraint_dict.py
+-rw-r--r--   0        0        0     1281 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_unsupported_type.py
+-rw-r--r--   0        0        0      932 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_unsupported_type_dict.py
+-rw-r--r--   0        0        0      756 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_updated_by.py
+-rw-r--r--   0        0        0      759 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_updated_time.py
+-rw-r--r--   0        0        0     2218 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_user.py
+-rw-r--r--   0        0        0     1880 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_user_dict.py
+-rw-r--r--   0        0        0      716 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_user_id.py
+-rw-r--r--   0        0        0     1257 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_user_search_filter.py
+-rw-r--r--   0        0        0      964 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_user_search_filter_dict.py
+-rw-r--r--   0        0        0      715 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_user_username.py
+-rw-r--r--   0        0        0     1343 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validate_action_request.py
+-rw-r--r--   0        0        0     1031 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validate_action_request_dict.py
+-rw-r--r--   0        0        0     1689 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validate_action_response.py
+-rw-r--r--   0        0        0     1360 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validate_action_response_dict.py
+-rw-r--r--   0        0        0     1732 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validate_action_response_v2.py
+-rw-r--r--   0        0        0     1364 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validate_action_response_v2_dict.py
+-rw-r--r--   0        0        0      758 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_validation_result.py
+-rw-r--r--   0        0        0     3481 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_value_type.py
+-rw-r--r--   0        0        0     1135 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_version.py
+-rw-r--r--   0        0        0      880 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_version_dict.py
+-rw-r--r--   0        0        0      719 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_version_version.py
+-rw-r--r--   0        0        0     1361 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_website.py
+-rw-r--r--   0        0        0     1049 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_website_dict.py
+-rw-r--r--   0        0        0      750 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_bounding_box_point.py
+-rw-r--r--   0        0        0      767 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_bounding_box_point_dict.py
+-rw-r--r--   0        0        0     1460 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_bounding_box_query.py
+-rw-r--r--   0        0        0     1156 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_bounding_box_query_dict.py
+-rw-r--r--   0        0        0     1454 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_distance_of_query.py
+-rw-r--r--   0        0        0     1154 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_distance_of_query_dict.py
+-rw-r--r--   0        0        0     1417 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_polygon_query.py
+-rw-r--r--   0        0        0     1130 2024-05-29 22:42:43.185224 foundry_platform_sdk-0.5.0/foundry/models/_within_polygon_query_dict.py
+-rw-r--r--   0        0        0      638 2024-05-29 22:42:43.993223 foundry_platform_sdk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    65568 1970-01-01 00:00:00.000000 foundry_platform_sdk-0.5.0/PKG-INFO
```

### Comparing `foundry_platform_sdk-0.3.0/LICENSE` & `foundry_platform_sdk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry_platform_sdk-0.3.0/foundry/__init__.py` & `foundry_platform_sdk-0.5.0/foundry/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,54 +8,35 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""
-    Palantir OpenAPI
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
-
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
-
-# The SDK version
-from foundry._versions import __version__
+from foundry._core.confidential_client_auth import ConfidentialClientAuth
+from foundry._core.foundry_token_auth_client import UserTokenAuth
+from foundry._errors.environment_not_configured import EnvironmentNotConfigured
+from foundry._errors.not_authenticated import NotAuthenticated
+from foundry._errors.palantir_rpc_exception import PalantirRPCException
 
 # The OpenAPI document version from the spec information
 # See https://swagger.io/specification/#info-object
+# The SDK version
 from foundry._versions import __openapi_document_version__
+from foundry._versions import __version__
+from foundry.foundry_client import FoundryClient
 
 # The OpenAPI specification version
 # See https://swagger.io/specification/#versions
-from foundry._versions import __openapi_specification_version__
-
-# The version of the generator used to generate the SDK
-from foundry._versions import __openapi_generator_version__
-
-
-from foundry._core.confidential_client_auth import ConfidentialClientAuth
-from foundry._core.foundry_token_auth_client import UserTokenAuth
-from foundry._errors.not_authenticated import NotAuthenticated
-from foundry._errors.environment_not_configured import EnvironmentNotConfigured
-from foundry._errors.palantir_rpc_exception import PalantirRPCException
-from foundry.foundry_client import FoundryClient
 
 
 __all__ = [
     "__version__",
     "__openapi_document_version__",
-    "__openapi_specification_version__",
-    "__openapi_generator_version__",
     "ConfidentialClientAuth",
     "UserTokenAuth",
     "NotAuthenticated",
     "EnvironmentNotConfigured",
     "PalantirRPCException",
     "FoundryClient",
 ]
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/__init__.py` & `foundry_platform_sdk-0.5.0/foundry/models/_version_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,7 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+
+
+from __future__ import annotations
+
+from pydantic import StrictStr
+
+VersionVersion = StrictStr
+"""VersionVersion"""
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/auth_utils.py` & `foundry_platform_sdk-0.5.0/foundry/_core/oauth.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,32 +8,17 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from abc import ABC, abstractmethod
-from typing import Callable, TypeVar
 
-T = TypeVar("T")
+from pydantic import BaseModel
 
 
-class Token(ABC):
-    @property
-    @abstractmethod
-    def access_token(self) -> str:
-        pass
+class SignInResponse(BaseModel):
+    session: dict
 
 
-class Auth(ABC):
-    @abstractmethod
-    def get_token(self) -> "Token":
-        pass
-
-    @abstractmethod
-    def execute_with_token(self, func: Callable[["Token"], T]) -> T:
-        pass
-
-    @abstractmethod
-    def run_with_token(self, func: Callable[["Token"], None]) -> None:
-        pass
+class SignOutResponse(BaseModel):
+    pass
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/confidential_client_auth.py` & `foundry_platform_sdk-0.5.0/foundry/_core/confidential_client_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+
 import asyncio
-from typing import Callable, Optional, List, TypeVar
+from typing import Callable
+from typing import List
+from typing import Optional
+from typing import TypeVar
 
 import requests
+
 from foundry._core.auth_utils import Auth
+from foundry._core.oauth import SignInResponse
+from foundry._core.oauth import SignOutResponse
 from foundry._core.oauth_utils import ConfidentialClientOAuthFlowProvider
 from foundry._core.oauth_utils import OAuthToken
-from foundry._core.oauth import SignOutResponse
-from foundry._core.oauth import SignInResponse
 from foundry._errors.environment_not_configured import EnvironmentNotConfigured
 from foundry._errors.not_authenticated import NotAuthenticated
 
-
 T = TypeVar("T")
 
 
 class ConfidentialClientAuth(Auth):
     """
     Client for Confidential Client OAuth-authenticated Ontology applications.
     Runs a background thread to periodically refresh access token.
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/foundry_token_auth_client.py` & `foundry_platform_sdk-0.5.0/foundry/_core/foundry_token_auth_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+
 import os
-from typing import Tuple, TypeVar, Callable
+from typing import Callable
+from typing import Tuple
+from typing import TypeVar
 
-from foundry._core.auth_utils import Auth, Token
+from foundry._core.auth_utils import Auth
+from foundry._core.auth_utils import Token
 from foundry._errors.environment_not_configured import EnvironmentNotConfigured
 from foundry._errors.not_authenticated import NotAuthenticated
 
-
 T = TypeVar("T")
 
 
 class _UserToken(Token):
     def __init__(self, token: str) -> None:
         self._token = token
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/oauth.py` & `foundry_platform_sdk-0.5.0/foundry/models/_page_size.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from pydantic import BaseModel
 
+from __future__ import annotations
 
-class SignInResponse(BaseModel):
-    session: dict
+from pydantic import StrictInt
 
-
-class SignOutResponse(BaseModel):
-    pass
+PageSize = StrictInt
+"""The page size to use for the endpoint."""
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/oauth_utils.py` & `foundry_platform_sdk-0.5.0/foundry/_core/oauth_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+
+import base64
 import hashlib
 import secrets
-import time
 import string
-import base64
-
-from urllib.parse import urlencode
-from typing import Optional
+import time
 from typing import List
+from typing import Optional
+from urllib.parse import urlencode
 
 import requests
 from pydantic import BaseModel
 
 from foundry._core.auth_utils import Token
 
 
@@ -61,16 +61,16 @@
         else:
             return "https://" + base_uri + context_path + request_path
 
 
 class OAuthTokenResponse(BaseModel):
     access_token: str
     token_type: str
-    refresh_token: Optional[str]
     expires_in: int
+    refresh_token: Optional[str] = None
 
     def __init__(self, token_response: dict) -> None:
         super().__init__(**token_response)
 
 
 class OAuthToken(Token):
     def __init__(self, token: OAuthTokenResponse):
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/palantir_session.py` & `foundry_platform_sdk-0.5.0/foundry/_core/palantir_session.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Mapping
+from typing import Optional
+from typing import Tuple
+from typing import Union
+
 import requests
-from typing import Any, Callable, Mapping, Optional, Dict
 
-import foundry
-from foundry._core.auth_utils import Auth, Token
+from foundry._core.auth_utils import Auth
+from foundry._core.auth_utils import Token
 
 
 def _run_with_401_status_check(
     callable: Callable[[Token], requests.Response]
 ) -> Callable[[Token], requests.Response]:
     def f(token: Token) -> requests.Response:
         response = callable(token)
@@ -28,14 +37,17 @@
             response.raise_for_status()
         return response
 
     func: Callable[[Token], requests.Response] = lambda token: f(token)
     return func
 
 
+_Params = Union[Mapping[str, Any], List[Tuple[str, Any]]]
+
+
 class PalantirSession:
     """Submits http requests with a dependency-injected authentication token provider.
 
     :param auth: Dependency that provides credentials for authentication.
     :param preview: Boolean that enables access to endpoints in Preview Mode by default. Defaults to False.
     """
 
@@ -50,37 +62,39 @@
         return self._remove_host_prefix(self._hostname)
 
     def request(
         self,
         method: str,
         url: str,
         headers: Optional[Mapping[str, Any]] = None,
-        params: Optional[Mapping[str, Any]] = None,
+        params: Optional[_Params] = None,
         data: Optional[bytes] = None,
         json: Optional[Any] = None,
         stream: bool = True,
+        timeout: Optional[int] = None,
     ) -> requests.Response:
         request_fn = _run_with_401_status_check(
             lambda token: self._session.request(
                 method=method,
                 url=url,
                 params=params,
                 data=data,
                 json=json,
                 headers=self._add_user_agent_and_auth_headers(token, headers),
                 stream=stream,
+                timeout=timeout,
             )
         )
         return self._auth.execute_with_token(request_fn)
 
     def get(
         self,
         url: str,
         headers: Optional[Mapping[str, Any]] = None,
-        params: Optional[Mapping[str, Any]] = None,
+        params: Optional[_Params] = None,
         data: Optional[bytes] = None,
         json: Optional[Any] = None,
         stream: bool = True,
     ) -> requests.Response:
         request_fn = _run_with_401_status_check(
             lambda token: self._session.get(
                 url=url,
@@ -93,15 +107,15 @@
         )
         return self._auth.execute_with_token(request_fn)
 
     def post(
         self,
         url: str,
         headers: Optional[Mapping[str, Any]] = None,
-        params: Optional[Mapping[str, Any]] = None,
+        params: Optional[_Params] = None,
         data: Optional[bytes] = None,
         json: Optional[Any] = None,
         stream: bool = True,
     ) -> requests.Response:
         request_fn = _run_with_401_status_check(
             lambda token: self._session.post(
                 url=url,
@@ -114,15 +128,15 @@
         )
         return self._auth.execute_with_token(request_fn)
 
     def put(
         self,
         url: str,
         headers: Optional[Mapping[str, Any]] = None,
-        params: Optional[Mapping[str, Any]] = None,
+        params: Optional[_Params] = None,
         data: Optional[bytes] = None,
         json: Optional[Any] = None,
         stream: bool = True,
     ) -> requests.Response:
         request_fn = _run_with_401_status_check(
             lambda token: self._session.put(
                 url=url,
@@ -135,15 +149,15 @@
         )
         return self._auth.execute_with_token(request_fn)
 
     def delete(
         self,
         url: str,
         headers: Optional[Mapping[str, Any]] = None,
-        params: Optional[Mapping[str, Any]] = None,
+        params: Optional[_Params] = None,
         data: Optional[bytes] = None,
         json: Optional[Any] = None,
         stream: bool = True,
     ) -> requests.Response:
         request_fn = _run_with_401_status_check(
             lambda token: self._session.delete(
                 url=url,
@@ -156,15 +170,15 @@
         )
         return self._auth.execute_with_token(request_fn)
 
     def patch(
         self,
         url: str,
         headers: Optional[Mapping[str, Any]] = None,
-        params: Optional[Mapping[str, Any]] = None,
+        params: Optional[_Params] = None,
         data: Optional[bytes] = None,
         json: Optional[Any] = None,
         stream: bool = True,
     ) -> requests.Response:
         request_fn = _run_with_401_status_check(
             lambda token: self._session.patch(
                 url=url,
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_core/public_client_auth.py` & `foundry_platform_sdk-0.5.0/foundry/_core/public_client_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,38 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import requests
+
 import threading
 import time
-from typing import Callable, Optional, TypeVar
+import webbrowser
+from typing import Callable
+from typing import List
+from typing import Optional
+from typing import TypeVar
+
+import requests
 
 from foundry._core.auth_utils import Auth
+from foundry._core.oauth import SignOutResponse
 from foundry._core.oauth_utils import AuthorizeRequest
 from foundry._core.oauth_utils import OAuthToken
 from foundry._core.oauth_utils import PublicClientOAuthFlowProvider
-from foundry._core.oauth import SignOutResponse
 from foundry._errors.not_authenticated import NotAuthenticated
-import webbrowser
-
+from foundry._errors.sdk_internal_error import SDKInternalError
 
 T = TypeVar("T")
 
 
 class PublicClientAuth(Auth):
-    scopes: list[str] = ["api:read-data", "api:write-data", "offline_access"]
+    scopes: List[str] = ["api:read-data", "api:write-data", "offline_access"]
 
     """
     Client for Public Client OAuth-authenticated Ontology applications.
     Runs a background thread to periodically refresh access token.
 
     :param client_id: OAuth client id to be used by the application.
     :param client_secret: OAuth client secret to be used by the application.
@@ -73,15 +78,14 @@
             self._run_with_attempted_refresh(func)
         except Exception as e:
             self.sign_out()
             raise e
 
     def _refresh_token(self):
         if self._token is None:
-            # TODO
             raise Exception("")
 
         self._token = self._server_oauth_flow_provider.refresh_token(
             refresh_token=self._token.refresh_token
         )
 
     def _run_with_attempted_refresh(self, func: Callable[[OAuthToken], T]) -> T:
@@ -120,20 +124,17 @@
                     # Wait 10 seconds and check again if the token is set
                     time.sleep(10)
 
         refresh_thread = threading.Thread(target=_auto_refresh_token, daemon=True)
         refresh_thread.start()
 
     def set_token(self, code: str, state: str) -> None:
-        if self._auth_request is None:
-            raise Exception("")
-            # TODO
+        if self._auth_request is None or state != self._auth_request.state:
+            raise RuntimeError("Unable to verify the state")
 
-        if state != self._auth_request.state:
-            raise RuntimeError("Unable to verify state")
         self._token = self._server_oauth_flow_provider.get_token(
             code=code, code_verifier=self._auth_request.code_verifier
         )
 
         if self._should_refresh:
             self._start_auto_refresh()
         return
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_errors/environment_not_configured.py` & `foundry_platform_sdk-0.5.0/foundry/_errors/environment_not_configured.py`

 * *Files identical despite different names*

### Comparing `foundry_platform_sdk-0.3.0/foundry/_errors/helpers.py` & `foundry_platform_sdk-0.5.0/foundry/_errors/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+
 import json
-import requests
 from importlib import import_module
 from json import JSONDecodeError
-from typing import Dict, Any
+from typing import Any
+from typing import Dict
+
+import requests
 
 
 def format_error_message(fields: Dict[str, Any]) -> str:
     return json.dumps(fields, sort_keys=True, indent=4)
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_errors/not_authenticated.py` & `foundry_platform_sdk-0.5.0/foundry/_errors/not_authenticated.py`

 * *Files identical despite different names*

### Comparing `foundry_platform_sdk-0.3.0/foundry/_errors/palantir_rpc_exception.py` & `foundry_platform_sdk-0.5.0/foundry/_errors/palantir_rpc_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any, Dict
+
+from typing import Any
+from typing import Dict
+
 from foundry._errors.helpers import format_error_message
 
 
 class PalantirRPCException(Exception):
     def __init__(self, error_metadata: Dict[str, Any]):
         super().__init__(format_error_message(error_metadata))
         self.name: str = error_metadata["errorName"]
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_errors/sdk_internal_error.py` & `foundry_platform_sdk-0.5.0/foundry/_errors/sdk_internal_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,41 +8,40 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+
 import functools
 import sys
 from typing import Any
 from typing import Callable
 from typing import TypeVar
 
-from pydantic import __version__ as __pydantic__version__
 from pydantic import ValidationError
+from pydantic import __version__ as __pydantic__version__
 from pydantic_core import __version__ as __pydantic_core_version__
 from requests import __version__ as __requests_version__
+from requests.exceptions import ConnectionError
 
 from foundry._errors.palantir_rpc_exception import PalantirRPCException
-from foundry._versions import __version__
 from foundry._versions import __openapi_document_version__
-from foundry._versions import __openapi_specification_version__
-from foundry._versions import __openapi_generator_version__
-
+from foundry._versions import __version__
 
 AnyCallableT = TypeVar("AnyCallableT", bound=Callable[..., Any])
 
 
 def handle_unexpected(__func: AnyCallableT) -> AnyCallableT:
     @functools.wraps(__func)
     def validate(*args, **kwargs):
         try:
             return __func(*args, **kwargs)
-        except (PalantirRPCException, ValidationError) as e:
+        except (PalantirRPCException, SDKInternalError, ValidationError, ConnectionError) as e:
             # pass through these exceptions
             raise e
         except Exception as e:
             raise SDKInternalError(str(e)) from e
 
     return validate  # type: ignore
 
@@ -59,15 +58,13 @@
             "\n\nThis is an unexpected issue and should be reported. "
             "When filing an issue, make sure to copy the package information "
             "listed below.\n\n"
             f"OS: {sys.platform}\n"
             f"Python Version: {sys_version}\n"
             f"SDK Version: {__version__}\n"
             f"OpenAPI Document Version: {__openapi_document_version__}\n"
-            f"OpenAPI Specification Version: {__openapi_specification_version__}\n"
-            f"OpenAPI Generator Version: {__openapi_generator_version__}\n"
             f"Pydantic Version: {__pydantic__version__}\n"
             f"Pydantic Core Version: {__pydantic_core_version__}\n"
             f"Requests Version: {__requests_version__}\n"
         )
 
         return message
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/_versions.py` & `foundry_platform_sdk-0.5.0/foundry/_versions.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,10 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 
 # The version is set during the publishing step (since we can't know the version in advance)
 # using the autorelease bot
-__version__ = "0.3.0"
+__version__ = "0.5.0"
 
-__openapi_document_version__ = "1.738.0"
-
-__openapi_specification_version__ = "3.0.1"
-
-__openapi_generator_version__ = "7.1.0"
+__openapi_document_version__ = "1.839.0"
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/api/__init__.py` & `foundry_platform_sdk-0.5.0/foundry/models/_custom_type_id.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# flake8: noqa
 
-# import apis into api package
-from foundry.api.datasets_api_service_api import DatasetsApiServiceApi
-from foundry.api.ontologies_api_service_api import OntologiesApiServiceApi
-from foundry.api.ontologies_v2_api_service_api import OntologiesV2ApiServiceApi
+from __future__ import annotations
+
+from pydantic import StrictStr
+
+CustomTypeId = StrictStr
+"""A UUID representing a custom type in a given Function."""
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/foundry_client.py` & `foundry_platform_sdk-0.5.0/foundry/_namespaces/namespaces.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from foundry._core.auth_utils import Auth
-from foundry.api.ontologies_v2_api_service_api import OntologiesV2ApiServiceApi
-from foundry.api.datasets_api_service_api import DatasetsApiServiceApi
-from foundry.api.ontologies_api_service_api import OntologiesApiServiceApi
+
+from __future__ import annotations
+
+from foundry._namespaces.datasets.dataset import DatasetResource
+from foundry._namespaces.datasets.file import FileResource
+from foundry._namespaces.ontologies.ontology import OntologyResource
+from foundry._namespaces.security.group import GroupResource
+from foundry._namespaces.security.user import UserResource
 from foundry.api_client import ApiClient
-from foundry._errors.environment_not_configured import EnvironmentNotConfigured
 
 
-class FoundryClient:
-    """
-    The Foundry API client.
-
-    :param auth: Your auth configuration.
-    :param hostname: Your Foundry hostname (for example, "myfoundry.palantirfoundry.com").
-    """
-
-    def __init__(self, auth: Auth, hostname: str):
-        api_client = ApiClient(auth=auth, hostname=hostname)
-        self.ontologies_v2 = OntologiesV2ApiServiceApi(api_client=api_client)
-        self.datasets = DatasetsApiServiceApi(api_client=api_client)
-        self.ontologies = OntologiesApiServiceApi(api_client=api_client)
+class Datasets:
+    def __init__(self, api_client: ApiClient):
+        self.Dataset = DatasetResource(api_client=api_client)
+        self.File = FileResource(api_client=api_client)
+
+
+class Ontologies:
+    def __init__(self, api_client: ApiClient):
+        self.Ontology = OntologyResource(api_client=api_client)
+
+
+class Security:
+    def __init__(self, api_client: ApiClient):
+        self.Group = GroupResource(api_client=api_client)
+        self.User = UserResource(api_client=api_client)
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/link_type_side_cardinality.py` & `foundry_platform_sdk-0.5.0/foundry/models/_array_size_constraint.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,49 +8,42 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Any
+from typing import Literal
+from typing import Optional
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._array_size_constraint_dict import ArraySizeConstraintDict
 
 
-from __future__ import annotations
-import json
-import pprint
-import re  # noqa: F401
-from enum import Enum
-
-
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-
-class LinkTypeSideCardinality(str, Enum):
-    """
-    LinkTypeSideCardinality
-    """
-
-    """
-    allowed enum values
-    """
-    ONE = "ONE"
-    MANY = "MANY"
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of LinkTypeSideCardinality from a JSON string"""
-        return cls(json.loads(json_str))
+class ArraySizeConstraint(BaseModel):
+    """The parameter expects an array of values and the size of the array must fall within the defined range."""
+
+    lt: Optional[Any] = None
+    """Less than"""
+
+    lte: Optional[Any] = None
+    """Less than or equal"""
+
+    gt: Optional[Any] = None
+    """Greater than"""
+
+    gte: Optional[Any] = None
+    """Greater than or equal"""
+
+    type: Literal["arraySize"]
+
+    model_config = {"extra": "allow"}
+
+    def to_dict(self) -> ArraySizeConstraintDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(ArraySizeConstraintDict, self.model_dump(by_alias=True, exclude_unset=True))
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/logic_rule.py` & `foundry_platform_sdk-0.5.0/foundry/models/_list_linked_objects_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,55 +8,36 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import List
+from typing import Optional
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
+from pydantic import Field
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._list_linked_objects_response_dict import ListLinkedObjectsResponseDict  # NOQA
+from foundry.models._ontology_object import OntologyObject
+from foundry.models._page_token import PageToken
 
 
-from __future__ import annotations
-import json
-import pprint
-from typing import Union
-
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set
-from pydantic import Field
-from pydantic import TypeAdapter
-from typing_extensions import Self
+class ListLinkedObjectsResponse(BaseModel):
+    """ListLinkedObjectsResponse"""
+
+    next_page_token: Optional[PageToken] = Field(alias="nextPageToken", default=None)
+
+    data: List[OntologyObject]
+
+    model_config = {"extra": "allow"}
 
-from foundry.models.create_link_rule import CreateLinkRule
-from foundry.models.create_object_rule import CreateObjectRule
-from foundry.models.delete_link_rule import DeleteLinkRule
-from foundry.models.delete_object_rule import DeleteObjectRule
-from foundry.models.modify_object_rule import ModifyObjectRule
-
-
-"""
-LogicRule
-"""
-LogicRule = Annotated[
-    Union[CreateLinkRule, CreateObjectRule, DeleteLinkRule, DeleteObjectRule, ModifyObjectRule],
-    Field(discriminator="type"),
-]
-
-
-# Create an instance of a type adapter. This has a non-trivial overhead according
-# to the documentation so we do this once. This also forces us to validate the
-# correctness of the discriminator.
-object.__setattr__(LogicRule, "type_adapter", TypeAdapter(LogicRule))
+    def to_dict(self) -> ListLinkedObjectsResponseDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(
+            ListLinkedObjectsResponseDict, self.model_dump(by_alias=True, exclude_unset=True)
+        )
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/object_type_visibility.py` & `foundry_platform_sdk-0.5.0/foundry/models/_geo_point_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,50 +8,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Literal
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._geo_point_type_dict import GeoPointTypeDict
 
 
-from __future__ import annotations
-import json
-import pprint
-import re  # noqa: F401
-from enum import Enum
-
-
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-
-class ObjectTypeVisibility(str, Enum):
-    """
-    The suggested visibility of the object type.
-    """
-
-    """
-    allowed enum values
-    """
-    NORMAL = "NORMAL"
-    PROMINENT = "PROMINENT"
-    HIDDEN = "HIDDEN"
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ObjectTypeVisibility from a JSON string"""
-        return cls(json.loads(json_str))
+class GeoPointType(BaseModel):
+    """GeoPointType"""
+
+    type: Literal["geopoint"]
+
+    model_config = {"extra": "allow"}
+
+    def to_dict(self) -> GeoPointTypeDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(GeoPointTypeDict, self.model_dump(by_alias=True, exclude_unset=True))
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_key_type.py` & `foundry_platform_sdk-0.5.0/foundry/models/_geo_json_object.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,65 +8,53 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
-
-"""
-    Palantir OpenAPI
-
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
-
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""  # noqa: E501
-
 
 from __future__ import annotations
-import json
-import pprint
+
+from typing import Annotated
 from typing import Union
 
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set
 from pydantic import Field
-from pydantic import TypeAdapter
-from typing_extensions import Self
 
-from foundry.models.boolean_type import BooleanType
-from foundry.models.date_type import DateType
-from foundry.models.double_type import DoubleType
-from foundry.models.integer_type import IntegerType
-from foundry.models.query_aggregation_range_type import QueryAggregationRangeType
-from foundry.models.string_type import StringType
-from foundry.models.timestamp_type import TimestampType
+from foundry.models._feature import Feature
+from foundry.models._feature_collection import FeatureCollection
+from foundry.models._geo_point import GeoPoint
+from foundry.models._geometry import GeometryCollection
+from foundry.models._line_string import LineString
+from foundry.models._multi_line_string import MultiLineString
+from foundry.models._multi_point import MultiPoint
+from foundry.models._multi_polygon import MultiPolygon
+from foundry.models._polygon import Polygon
 
-
-"""
-A union of all the types supported by query aggregation keys. 
-"""
-QueryAggregationKeyType = Annotated[
+GeoJsonObject = Annotated[
     Union[
-        BooleanType,
-        DateType,
-        DoubleType,
-        IntegerType,
-        QueryAggregationRangeType,
-        StringType,
-        TimestampType,
+        Feature,
+        FeatureCollection,
+        GeoPoint,
+        MultiPoint,
+        LineString,
+        MultiLineString,
+        Polygon,
+        MultiPolygon,
+        GeometryCollection,
     ],
     Field(discriminator="type"),
 ]
+"""
+GeoJSon object
 
-
-# Create an instance of a type adapter. This has a non-trivial overhead according
-# to the documentation so we do this once. This also forces us to validate the
-# correctness of the discriminator.
-object.__setattr__(QueryAggregationKeyType, "type_adapter", TypeAdapter(QueryAggregationKeyType))
+The coordinate reference system for all GeoJSON coordinates is a
+geographic coordinate reference system, using the World Geodetic System
+1984 (WGS 84) datum, with longitude and latitude units of decimal
+degrees.
+This is equivalent to the coordinate reference system identified by the
+Open Geospatial Consortium (OGC) URN
+An OPTIONAL third-position element SHALL be the height in meters above
+or below the WGS 84 reference ellipsoid.
+In the absence of elevation values, applications sensitive to height or
+depth SHOULD interpret positions as being at local ground or sea level.
+"""
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_range_sub_type.py` & `foundry_platform_sdk-0.5.0/foundry/models/_aggregation_exact_grouping_v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,55 +8,40 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Literal
+from typing import Optional
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
+from pydantic import Field
+from pydantic import StrictInt
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._aggregation_exact_grouping_v2_dict import (
+    AggregationExactGroupingV2Dict,
+)  # NOQA
+from foundry.models._property_api_name import PropertyApiName
 
 
-from __future__ import annotations
-import json
-import pprint
-from typing import Union
-
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set
-from pydantic import Field
-from pydantic import TypeAdapter
-from typing_extensions import Self
+class AggregationExactGroupingV2(BaseModel):
+    """Divides objects into groups according to an exact value."""
+
+    field: PropertyApiName
+
+    max_group_count: Optional[StrictInt] = Field(alias="maxGroupCount", default=None)
+
+    type: Literal["exact"]
+
+    model_config = {"extra": "allow"}
 
-from foundry.models.date_type import DateType
-from foundry.models.double_type import DoubleType
-from foundry.models.integer_type import IntegerType
-from foundry.models.timestamp_type import TimestampType
-
-
-"""
-A union of all the types supported by query aggregation ranges. 
-"""
-QueryAggregationRangeSubType = Annotated[
-    Union[DateType, DoubleType, IntegerType, TimestampType], Field(discriminator="type")
-]
-
-
-# Create an instance of a type adapter. This has a non-trivial overhead according
-# to the documentation so we do this once. This also forces us to validate the
-# correctness of the discriminator.
-object.__setattr__(
-    QueryAggregationRangeSubType, "type_adapter", TypeAdapter(QueryAggregationRangeSubType)
-)
+    def to_dict(self) -> AggregationExactGroupingV2Dict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(
+            AggregationExactGroupingV2Dict, self.model_dump(by_alias=True, exclude_unset=True)
+        )
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/query_aggregation_value_type.py` & `foundry_platform_sdk-0.5.0/foundry/models/_list_attachments_response_v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,54 +8,39 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import List
+from typing import Literal
+from typing import Optional
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
+from pydantic import Field
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._attachment_v2 import AttachmentV2
+from foundry.models._list_attachments_response_v2_dict import ListAttachmentsResponseV2Dict  # NOQA
+from foundry.models._page_token import PageToken
 
 
-from __future__ import annotations
-import json
-import pprint
-from typing import Union
-
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set
-from pydantic import Field
-from pydantic import TypeAdapter
-from typing_extensions import Self
+class ListAttachmentsResponseV2(BaseModel):
+    """ListAttachmentsResponseV2"""
+
+    data: List[AttachmentV2]
+
+    next_page_token: Optional[PageToken] = Field(alias="nextPageToken", default=None)
+
+    type: Literal["multiple"]
+
+    model_config = {"extra": "allow"}
 
-from foundry.models.date_type import DateType
-from foundry.models.double_type import DoubleType
-from foundry.models.timestamp_type import TimestampType
-
-
-"""
-A union of all the types supported by query aggregation keys. 
-"""
-QueryAggregationValueType = Annotated[
-    Union[DateType, DoubleType, TimestampType], Field(discriminator="type")
-]
-
-
-# Create an instance of a type adapter. This has a non-trivial overhead according
-# to the documentation so we do this once. This also forces us to validate the
-# correctness of the discriminator.
-object.__setattr__(
-    QueryAggregationValueType, "type_adapter", TypeAdapter(QueryAggregationValueType)
-)
+    def to_dict(self) -> ListAttachmentsResponseV2Dict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(
+            ListAttachmentsResponseV2Dict, self.model_dump(by_alias=True, exclude_unset=True)
+        )
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/release_status.py` & `foundry_platform_sdk-0.5.0/foundry/models/_boolean_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,50 +8,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Literal
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._boolean_type_dict import BooleanTypeDict
 
 
-from __future__ import annotations
-import json
-import pprint
-import re  # noqa: F401
-from enum import Enum
-
-
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-
-class ReleaseStatus(str, Enum):
-    """
-    The release status of the entity.
-    """
-
-    """
-    allowed enum values
-    """
-    ACTIVE = "ACTIVE"
-    EXPERIMENTAL = "EXPERIMENTAL"
-    DEPRECATED = "DEPRECATED"
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ReleaseStatus from a JSON string"""
-        return cls(json.loads(json_str))
+class BooleanType(BaseModel):
+    """BooleanType"""
+
+    type: Literal["boolean"]
+
+    model_config = {"extra": "allow"}
+
+    def to_dict(self) -> BooleanTypeDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(BooleanTypeDict, self.model_dump(by_alias=True, exclude_unset=True))
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/table_export_format.py` & `foundry_platform_sdk-0.5.0/foundry/models/_gte_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,49 +8,35 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Any
+from typing import Literal
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._field_name_v1 import FieldNameV1
+from foundry.models._gte_query_dict import GteQueryDict
 
 
-from __future__ import annotations
-import json
-import pprint
-import re  # noqa: F401
-from enum import Enum
-
-
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-
-class TableExportFormat(str, Enum):
-    """
-    Format for tabular dataset export.
-    """
-
-    """
-    allowed enum values
-    """
-    ARROW = "ARROW"
-    CSV = "CSV"
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TableExportFormat from a JSON string"""
-        return cls(json.loads(json_str))
+class GteQuery(BaseModel):
+    """Returns objects where the specified field is greater than or equal to a value."""
+
+    field: FieldNameV1
+
+    value: Any
+    """Greater than or equal to value"""
+
+    type: Literal["gte"]
+
+    model_config = {"extra": "allow"}
+
+    def to_dict(self) -> GteQueryDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(GteQueryDict, self.model_dump(by_alias=True, exclude_unset=True))
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/time_series_item_type.py` & `foundry_platform_sdk-0.5.0/foundry/models/_avg_aggregation_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,49 +8,29 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Literal
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from typing_extensions import NotRequired
+from typing_extensions import TypedDict
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._aggregation_metric_name import AggregationMetricName
+from foundry.models._field_name_v1 import FieldNameV1
 
 
-from __future__ import annotations
-import json
-import pprint
-from typing import Union
-
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set
-from pydantic import Field
-from pydantic import TypeAdapter
-from typing_extensions import Self
-
-from foundry.models.double_type import DoubleType
-from foundry.models.string_type import StringType
-
-
-"""
-A union of the types supported by time series properties. 
-"""
-TimeSeriesItemType = Annotated[Union[DoubleType, StringType], Field(discriminator="type")]
-
-
-# Create an instance of a type adapter. This has a non-trivial overhead according
-# to the documentation so we do this once. This also forces us to validate the
-# correctness of the discriminator.
-object.__setattr__(TimeSeriesItemType, "type_adapter", TypeAdapter(TimeSeriesItemType))
+class AvgAggregationDict(TypedDict):
+    """Computes the average value for the provided field."""
+
+    __pydantic_config__ = {"extra": "allow"}  # type: ignore
+
+    field: FieldNameV1
+
+    name: NotRequired[AggregationMetricName]
+
+    type: Literal["avg"]
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/transaction_status.py` & `foundry_platform_sdk-0.5.0/foundry/models/_short_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,50 +8,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Literal
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._short_type_dict import ShortTypeDict
 
 
-from __future__ import annotations
-import json
-import pprint
-import re  # noqa: F401
-from enum import Enum
-
-
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-
-class TransactionStatus(str, Enum):
-    """
-    The status of a Transaction.
-    """
-
-    """
-    allowed enum values
-    """
-    ABORTED = "ABORTED"
-    COMMITTED = "COMMITTED"
-    OPEN = "OPEN"
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TransactionStatus from a JSON string"""
-        return cls(json.loads(json_str))
+class ShortType(BaseModel):
+    """ShortType"""
+
+    type: Literal["short"]
+
+    model_config = {"extra": "allow"}
+
+    def to_dict(self) -> ShortTypeDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(ShortTypeDict, self.model_dump(by_alias=True, exclude_unset=True))
```

### Comparing `foundry_platform_sdk-0.3.0/foundry/models/transaction_type.py` & `foundry_platform_sdk-0.5.0/foundry/models/_lt_query.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,51 +8,35 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-# coding: utf-8
 
-"""
-    Palantir OpenAPI
+from __future__ import annotations
 
-    The Palantir REST API. Please see https://www.palantir.com/docs for more details.
+from typing import Any
+from typing import Literal
+from typing import cast
 
-    The version of the OpenAPI document: 1.738.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
+from pydantic import BaseModel
 
-    Do not edit the class manually.
-"""  # noqa: E501
+from foundry.models._field_name_v1 import FieldNameV1
+from foundry.models._lt_query_dict import LtQueryDict
 
 
-from __future__ import annotations
-import json
-import pprint
-import re  # noqa: F401
-from enum import Enum
-
-
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-
-class TransactionType(str, Enum):
-    """
-    The type of a Transaction.
-    """
-
-    """
-    allowed enum values
-    """
-    APPEND = "APPEND"
-    UPDATE = "UPDATE"
-    SNAPSHOT = "SNAPSHOT"
-    DELETE = "DELETE"
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TransactionType from a JSON string"""
-        return cls(json.loads(json_str))
+class LtQuery(BaseModel):
+    """Returns objects where the specified field is less than a value."""
+
+    field: FieldNameV1
+
+    value: Any
+    """Less than value"""
+
+    type: Literal["lt"]
+
+    model_config = {"extra": "allow"}
+
+    def to_dict(self) -> LtQueryDict:
+        """Return the dictionary representation of the model using the field aliases."""
+        return cast(LtQueryDict, self.model_dump(by_alias=True, exclude_unset=True))
```

