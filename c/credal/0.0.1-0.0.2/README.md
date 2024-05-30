# Comparing `tmp/credal-0.0.1.tar.gz` & `tmp/credal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credal-0.0.1.tar", max compression
+gzip compressed data, was "credal-0.0.2.tar", max compression
```

## Comparing `credal-0.0.1.tar` & `credal-0.0.2.tar`

### file list

```diff
@@ -1,77 +1,69 @@
--rw-r--r--   0        0        0     1754 2024-05-23 14:12:54.358313 credal-0.0.1/README.md
--rw-r--r--   0        0        0      589 2024-05-23 14:12:54.358313 credal-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2947 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/__init__.py
--rw-r--r--   0        0        0     7262 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/client.py
--rw-r--r--   0        0        0      407 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/common/__init__.py
--rw-r--r--   0        0        0      467 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/common/types/__init__.py
--rw-r--r--   0        0        0     1376 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/common/types/external_resource_id.py
--rw-r--r--   0        0        0     2533 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/common/types/resource_identifier.py
--rw-r--r--   0        0        0      541 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/common/types/resource_type.py
--rw-r--r--   0        0        0     1104 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/common/types/url.py
--rw-r--r--   0        0        0      655 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/__init__.py
--rw-r--r--   0        0        0    13525 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/client.py
--rw-r--r--   0        0        0      863 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/__init__.py
--rw-r--r--   0        0        0     1279 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/create_conversation_response.py
--rw-r--r--   0        0        0     1134 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/inserted_audit_log.py
--rw-r--r--   0        0        0     1507 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/message_blocked.py
--rw-r--r--   0        0        0     1653 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/message_reply.py
--rw-r--r--   0        0        0     1148 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/policy_trigger.py
--rw-r--r--   0        0        0     1255 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/response_chunk.py
--rw-r--r--   0        0        0     1331 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/send_agent_message_response.py
--rw-r--r--   0        0        0     3144 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/copilots/types/send_message_response.py
--rw-r--r--   0        0        0      973 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/api_error.py
--rw-r--r--   0        0        0     1915 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/jsonable_encoder.py
--rw-r--r--   0        0        0      748 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/pydantic_utilities.py
--rw-r--r--   0        0        0     1215 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/query_encoder.py
--rw-r--r--   0        0        0      330 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/core/request_options.py
--rw-r--r--   0        0        0      255 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_catalog/__init__.py
--rw-r--r--   0        0        0    34230 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_catalog/client.py
--rw-r--r--   0        0        0      354 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_catalog/types/__init__.py
--rw-r--r--   0        0        0     1624 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_catalog/types/document_metadata_patch.py
--rw-r--r--   0        0        0     1378 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_catalog/types/document_metadata_patch_request.py
--rw-r--r--   0        0        0     1267 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_catalog/types/upload_document_response.py
--rw-r--r--   0        0        0      453 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/__init__.py
--rw-r--r--   0        0        0    52058 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/client.py
--rw-r--r--   0        0        0      630 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/__init__.py
--rw-r--r--   0        0        0     1298 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/create_document_collection_response.py
--rw-r--r--   0        0        0      182 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/data_type.py
--rw-r--r--   0        0        0      175 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/distance_metric.py
--rw-r--r--   0        0        0     1296 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/indexed_document.py
--rw-r--r--   0        0        0     1300 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/list_document_collection_response.py
--rw-r--r--   0        0        0     1166 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/metadata_field.py
--rw-r--r--   0        0        0     1254 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/document_collections/types/metadata_schema.py
--rw-r--r--   0        0        0      163 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/environment.py
--rw-r--r--   0        0        0      629 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/permissions_service/__init__.py
--rw-r--r--   0        0        0    24722 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/permissions_service/client.py
--rw-r--r--   0        0        0      849 2024-05-23 14:12:54.358313 credal-0.0.1/src/credal/permissions_service/types/__init__.py
--rw-r--r--   0        0        0      138 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/action.py
--rw-r--r--   0        0        0      235 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/check_bulk_resources_authorization_response.py
--rw-r--r--   0        0        0     1143 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/check_resource_authorization_response.py
--rw-r--r--   0        0        0     1143 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/group.py
--rw-r--r--   0        0        0     2292 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/principal.py
--rw-r--r--   0        0        0     1354 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/principal_list_page.py
--rw-r--r--   0        0        0     1373 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/resource_authorization_result.py
--rw-r--r--   0        0        0     1218 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/resource_list_page.py
--rw-r--r--   0        0        0     1181 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/permissions_service/types/user.py
--rw-r--r--   0        0        0        0 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/py.typed
--rw-r--r--   0        0        0      457 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/__init__.py
--rw-r--r--   0        0        0    10697 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/client.py
--rw-r--r--   0        0        0      636 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/__init__.py
--rw-r--r--   0        0        0     2560 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/document_collection_search_options.py
--rw-r--r--   0        0        0     1625 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/document_collection_search_result.py
--rw-r--r--   0        0        0      178 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/operator.py
--rw-r--r--   0        0        0     1408 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/search_document_collection_response.py
--rw-r--r--   0        0        0     1520 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/search_result_chunk.py
--rw-r--r--   0        0        0     1189 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/search/types/single_field_filter.py
--rw-r--r--   0        0        0      135 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/users/__init__.py
--rw-r--r--   0        0        0     6577 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/users/client.py
--rw-r--r--   0        0        0      149 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/users/types/__init__.py
--rw-r--r--   0        0        0     1445 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/users/types/user_metadata_patch.py
--rw-r--r--   0        0        0       74 2024-05-23 14:12:54.362313 credal-0.0.1/src/credal/version.py
--rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 credal-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1754 2024-05-30 20:42:40.589888 credal-0.0.2/README.md
+-rw-r--r--   0        0        0      589 2024-05-30 20:42:40.589888 credal-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2559 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/__init__.py
+-rw-r--r--   0        0        0     7262 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/client.py
+-rw-r--r--   0        0        0      407 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/common/__init__.py
+-rw-r--r--   0        0        0      467 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/common/types/__init__.py
+-rw-r--r--   0        0        0     1376 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/common/types/external_resource_id.py
+-rw-r--r--   0        0        0     2533 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/common/types/resource_identifier.py
+-rw-r--r--   0        0        0      541 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/common/types/resource_type.py
+-rw-r--r--   0        0        0     1104 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/common/types/url.py
+-rw-r--r--   0        0        0      655 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/__init__.py
+-rw-r--r--   0        0        0    13525 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/client.py
+-rw-r--r--   0        0        0      863 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/create_conversation_response.py
+-rw-r--r--   0        0        0     1134 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/inserted_audit_log.py
+-rw-r--r--   0        0        0     1507 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/message_blocked.py
+-rw-r--r--   0        0        0     1653 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/message_reply.py
+-rw-r--r--   0        0        0     1148 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/policy_trigger.py
+-rw-r--r--   0        0        0     1255 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/response_chunk.py
+-rw-r--r--   0        0        0     1331 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/send_agent_message_response.py
+-rw-r--r--   0        0        0     3144 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/copilots/types/send_message_response.py
+-rw-r--r--   0        0        0      973 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/api_error.py
+-rw-r--r--   0        0        0     1915 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1215 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/core/request_options.py
+-rw-r--r--   0        0        0      255 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_catalog/__init__.py
+-rw-r--r--   0        0        0    21084 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_catalog/client.py
+-rw-r--r--   0        0        0      354 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_catalog/types/__init__.py
+-rw-r--r--   0        0        0     1624 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_catalog/types/document_metadata_patch.py
+-rw-r--r--   0        0        0     1378 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_catalog/types/document_metadata_patch_request.py
+-rw-r--r--   0        0        0     1267 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_catalog/types/upload_document_response.py
+-rw-r--r--   0        0        0       65 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_collections/__init__.py
+-rw-r--r--   0        0        0     8634 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/document_collections/client.py
+-rw-r--r--   0        0        0      163 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/environment.py
+-rw-r--r--   0        0        0      629 2024-05-30 20:42:40.589888 credal-0.0.2/src/credal/permissions_service/__init__.py
+-rw-r--r--   0        0        0    24722 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/client.py
+-rw-r--r--   0        0        0      849 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/action.py
+-rw-r--r--   0        0        0      235 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/check_bulk_resources_authorization_response.py
+-rw-r--r--   0        0        0     1143 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/check_resource_authorization_response.py
+-rw-r--r--   0        0        0     1143 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/group.py
+-rw-r--r--   0        0        0     2292 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/principal.py
+-rw-r--r--   0        0        0     1354 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/principal_list_page.py
+-rw-r--r--   0        0        0     1373 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/resource_authorization_result.py
+-rw-r--r--   0        0        0     1218 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/resource_list_page.py
+-rw-r--r--   0        0        0     1181 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/permissions_service/types/user.py
+-rw-r--r--   0        0        0        0 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/py.typed
+-rw-r--r--   0        0        0      457 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/__init__.py
+-rw-r--r--   0        0        0    10697 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/client.py
+-rw-r--r--   0        0        0      636 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/__init__.py
+-rw-r--r--   0        0        0     2560 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/document_collection_search_options.py
+-rw-r--r--   0        0        0     1625 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/document_collection_search_result.py
+-rw-r--r--   0        0        0      178 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/operator.py
+-rw-r--r--   0        0        0     1661 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/search_document_collection_response.py
+-rw-r--r--   0        0        0     1520 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/search_result_chunk.py
+-rw-r--r--   0        0        0     1189 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/search/types/single_field_filter.py
+-rw-r--r--   0        0        0      135 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/users/__init__.py
+-rw-r--r--   0        0        0     6577 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/users/client.py
+-rw-r--r--   0        0        0      149 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/users/types/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/users/types/user_metadata_patch.py
+-rw-r--r--   0        0        0       74 2024-05-30 20:42:40.593888 credal-0.0.2/src/credal/version.py
+-rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 credal-0.0.2/PKG-INFO
```

### Comparing `credal-0.0.1/README.md` & `credal-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/pyproject.toml` & `credal-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "credal"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "credal", from = "src"}
 ]
```

### Comparing `credal-0.0.1/src/credal/client.py` & `credal-0.0.2/src/credal/client.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/common/types/external_resource_id.py` & `credal-0.0.2/src/credal/common/types/external_resource_id.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/common/types/resource_identifier.py` & `credal-0.0.2/src/credal/common/types/resource_identifier.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/common/types/resource_type.py` & `credal-0.0.2/src/credal/common/types/resource_type.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/common/types/url.py` & `credal-0.0.2/src/credal/common/types/url.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/__init__.py` & `credal-0.0.2/src/credal/copilots/__init__.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/client.py` & `credal-0.0.2/src/credal/copilots/client.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/__init__.py` & `credal-0.0.2/src/credal/copilots/types/__init__.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/create_conversation_response.py` & `credal-0.0.2/src/credal/copilots/types/create_conversation_response.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/inserted_audit_log.py` & `credal-0.0.2/src/credal/copilots/types/inserted_audit_log.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/message_blocked.py` & `credal-0.0.2/src/credal/copilots/types/message_blocked.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/message_reply.py` & `credal-0.0.2/src/credal/copilots/types/message_reply.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/policy_trigger.py` & `credal-0.0.2/src/credal/copilots/types/policy_trigger.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/response_chunk.py` & `credal-0.0.2/src/credal/copilots/types/response_chunk.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/send_agent_message_response.py` & `credal-0.0.2/src/credal/copilots/types/send_agent_message_response.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/copilots/types/send_message_response.py` & `credal-0.0.2/src/credal/copilots/types/send_message_response.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/__init__.py` & `credal-0.0.2/src/credal/core/__init__.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/client_wrapper.py` & `credal-0.0.2/src/credal/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "credal",
-            "X-Fern-SDK-Version": "0.0.1",
+            "X-Fern-SDK-Version": "0.0.2",
         }
         headers["Authorization"] = f"Bearer {self._get_api_key()}"
         return headers
 
     def _get_api_key(self) -> str:
         if isinstance(self._api_key, str):
             return self._api_key
```

### Comparing `credal-0.0.1/src/credal/core/datetime_utils.py` & `credal-0.0.2/src/credal/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/file.py` & `credal-0.0.2/src/credal/core/file.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/http_client.py` & `credal-0.0.2/src/credal/core/http_client.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/jsonable_encoder.py` & `credal-0.0.2/src/credal/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/pydantic_utilities.py` & `credal-0.0.2/src/credal/core/pydantic_utilities.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/query_encoder.py` & `credal-0.0.2/src/credal/core/query_encoder.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/core/request_options.py` & `credal-0.0.2/src/credal/core/request_options.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/document_catalog/client.py` & `credal-0.0.2/src/credal/document_catalog/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
@@ -19,105 +18,14 @@
 OMIT = typing.cast(typing.Any, ...)
 
 
 class DocumentCatalogClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def upload_document_url(
-        self,
-        *,
-        document_url: str,
-        upload_as_user_email: typing.Optional[str] = OMIT,
-        custom_metadata: typing.Optional[typing.Any] = OMIT,
-        collection_id: typing.Optional[str] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> UploadDocumentResponse:
-        """
-        Upload a document using its URL.
-
-        Parameters
-        ----------
-        document_url : str
-            The URL for the document you want to upload. Credal will automatically connect to source systems like Google Drive, Office 365, Confluence, etc. to fetch and upload the document contents.
-
-
-        upload_as_user_email : typing.Optional[str]
-            The user email to upload this document for. This user will be the owner of the document. User must be a collaborator on the API key.
-
-
-        custom_metadata : typing.Optional[typing.Any]
-            Optional JSON representing any custom metdata for this document
-
-
-        collection_id : typing.Optional[str]
-            If specified, document will also be added to a particular document collection
-
-
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        UploadDocumentResponse
-
-        Examples
-        --------
-        from credal.client import CredalApi
-
-        client = CredalApi(
-            api_key="YOUR_API_KEY",
-        )
-        client.document_catalog.upload_document_url(
-            document_url="https://docs.google.com/document/d/170NrBm0Do7gdzvr54UvyslPVWkQFOA0lgNycFmdZJQr",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"documentUrl": document_url}
-        if upload_as_user_email is not OMIT:
-            _request["uploadAsUserEmail"] = upload_as_user_email
-        if custom_metadata is not OMIT:
-            _request["customMetadata"] = custom_metadata
-        if collection_id is not OMIT:
-            _request["collectionId"] = collection_id
-        _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v0/catalog/uploadDocumentUrl"),
-            params=encode_query(
-                jsonable_encoder(
-                    request_options.get("additional_query_parameters") if request_options is not None else None
-                )
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     def upload_document_contents(
         self,
         *,
         document_name: str,
         document_contents: str,
         allowed_users_email_addresses: typing.Sequence[str],
         upload_as_user_email: str,
@@ -243,76 +151,14 @@
             return pydantic_v1.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def upload_document_file(
-        self, *, document: core.File, request_options: typing.Optional[RequestOptions] = None
-    ) -> UploadDocumentResponse:
-        """
-        Parameters
-        ----------
-        document : core.File
-            See core.File for more documentation
-
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        UploadDocumentResponse
-
-        Examples
-        --------
-        from credal.client import CredalApi
-
-        client = CredalApi(
-            api_key="YOUR_API_KEY",
-        )
-        client.document_catalog.upload_document_file()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v0/catalog/uploadDocumentFile"),
-            params=encode_query(
-                jsonable_encoder(
-                    request_options.get("additional_query_parameters") if request_options is not None else None
-                )
-            ),
-            data=jsonable_encoder(remove_none_from_dict({}))
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(remove_none_from_dict({})),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"document": document})),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     def metadata(
         self,
         *,
         sources: typing.Sequence[DocumentMetadataPatch],
         upload_as_user_email: str,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
@@ -398,105 +244,14 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDocumentCatalogClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def upload_document_url(
-        self,
-        *,
-        document_url: str,
-        upload_as_user_email: typing.Optional[str] = OMIT,
-        custom_metadata: typing.Optional[typing.Any] = OMIT,
-        collection_id: typing.Optional[str] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> UploadDocumentResponse:
-        """
-        Upload a document using its URL.
-
-        Parameters
-        ----------
-        document_url : str
-            The URL for the document you want to upload. Credal will automatically connect to source systems like Google Drive, Office 365, Confluence, etc. to fetch and upload the document contents.
-
-
-        upload_as_user_email : typing.Optional[str]
-            The user email to upload this document for. This user will be the owner of the document. User must be a collaborator on the API key.
-
-
-        custom_metadata : typing.Optional[typing.Any]
-            Optional JSON representing any custom metdata for this document
-
-
-        collection_id : typing.Optional[str]
-            If specified, document will also be added to a particular document collection
-
-
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        UploadDocumentResponse
-
-        Examples
-        --------
-        from credal.client import AsyncCredalApi
-
-        client = AsyncCredalApi(
-            api_key="YOUR_API_KEY",
-        )
-        await client.document_catalog.upload_document_url(
-            document_url="https://docs.google.com/document/d/170NrBm0Do7gdzvr54UvyslPVWkQFOA0lgNycFmdZJQr",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"documentUrl": document_url}
-        if upload_as_user_email is not OMIT:
-            _request["uploadAsUserEmail"] = upload_as_user_email
-        if custom_metadata is not OMIT:
-            _request["customMetadata"] = custom_metadata
-        if collection_id is not OMIT:
-            _request["collectionId"] = collection_id
-        _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v0/catalog/uploadDocumentUrl"),
-            params=encode_query(
-                jsonable_encoder(
-                    request_options.get("additional_query_parameters") if request_options is not None else None
-                )
-            ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
     async def upload_document_contents(
         self,
         *,
         document_name: str,
         document_contents: str,
         allowed_users_email_addresses: typing.Sequence[str],
         upload_as_user_email: str,
@@ -607,76 +362,14 @@
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UploadDocumentResponse, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def upload_document_file(
-        self, *, document: core.File, request_options: typing.Optional[RequestOptions] = None
-    ) -> UploadDocumentResponse:
-        """
-        Parameters
-        ----------
-        document : core.File
-            See core.File for more documentation
-
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        UploadDocumentResponse
-
-        Examples
-        --------
-        from credal.client import AsyncCredalApi
-
-        client = AsyncCredalApi(
-            api_key="YOUR_API_KEY",
-        )
-        await client.document_catalog.upload_document_file()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v0/catalog/uploadDocumentFile"),
-            params=encode_query(
-                jsonable_encoder(
-                    request_options.get("additional_query_parameters") if request_options is not None else None
-                )
-            ),
-            data=jsonable_encoder(remove_none_from_dict({}))
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(remove_none_from_dict({})),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            files=core.convert_file_dict_to_httpx_tuples(remove_none_from_dict({"document": document})),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
```

### Comparing `credal-0.0.1/src/credal/document_catalog/types/document_metadata_patch.py` & `credal-0.0.2/src/credal/document_catalog/types/document_metadata_patch.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/document_catalog/types/document_metadata_patch_request.py` & `credal-0.0.2/src/credal/document_catalog/types/document_metadata_patch_request.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/document_catalog/types/upload_document_response.py` & `credal-0.0.2/src/credal/document_catalog/types/upload_document_response.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/document_collections/types/__init__.py` & `credal-0.0.2/src/credal/search/types/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .create_document_collection_response import CreateDocumentCollectionResponse
-from .data_type import DataType
-from .distance_metric import DistanceMetric
-from .indexed_document import IndexedDocument
-from .list_document_collection_response import ListDocumentCollectionResponse
-from .metadata_field import MetadataField
-from .metadata_schema import MetadataSchema
+from .document_collection_search_options import DocumentCollectionSearchOptions
+from .document_collection_search_result import DocumentCollectionSearchResult
+from .operator import Operator
+from .search_document_collection_response import SearchDocumentCollectionResponse
+from .search_result_chunk import SearchResultChunk
+from .single_field_filter import SingleFieldFilter
 
 __all__ = [
-    "CreateDocumentCollectionResponse",
-    "DataType",
-    "DistanceMetric",
-    "IndexedDocument",
-    "ListDocumentCollectionResponse",
-    "MetadataField",
-    "MetadataSchema",
+    "DocumentCollectionSearchOptions",
+    "DocumentCollectionSearchResult",
+    "Operator",
+    "SearchDocumentCollectionResponse",
+    "SearchResultChunk",
+    "SingleFieldFilter",
 ]
```

### Comparing `credal-0.0.1/src/credal/document_collections/types/create_document_collection_response.py` & `credal-0.0.2/src/credal/permissions_service/types/check_resource_authorization_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
-import uuid
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
 
-class CreateDocumentCollectionResponse(pydantic_v1.BaseModel):
-    document_collection_id: uuid.UUID = pydantic_v1.Field(alias="documentCollectionId")
+class CheckResourceAuthorizationResponse(pydantic_v1.BaseModel):
+    authorized: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
@@ -22,11 +21,9 @@
         return deep_union_pydantic_dicts(
             super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
         )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `credal-0.0.1/src/credal/document_collections/types/indexed_document.py` & `credal-0.0.2/src/credal/permissions_service/types/resource_authorization_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
-import uuid
 
+from ...common.types.resource_identifier import ResourceIdentifier
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
 
-class IndexedDocument(pydantic_v1.BaseModel):
-    document_id: uuid.UUID = pydantic_v1.Field(alias="documentId")
-    metadata: typing.Dict[str, str]
+class ResourceAuthorizationResult(pydantic_v1.BaseModel):
+    resource_identifier: ResourceIdentifier = pydantic_v1.Field(alias="resourceIdentifier")
+    authorized: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/document_collections/types/list_document_collection_response.py` & `credal-0.0.2/src/credal/permissions_service/types/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .indexed_document import IndexedDocument
 
 
-class ListDocumentCollectionResponse(pydantic_v1.BaseModel):
-    documents: typing.List[IndexedDocument] = pydantic_v1.Field()
-    """
-    The list of documents in the document collection.
-    """
+class User(pydantic_v1.BaseModel):
+    email: str
+    name: typing.Optional[str] = None
+    id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/document_collections/types/metadata_field.py` & `credal-0.0.2/src/credal/permissions_service/types/resource_list_page.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...common.types.resource_identifier import ResourceIdentifier
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .data_type import DataType
 
 
-class MetadataField(pydantic_v1.BaseModel):
-    name: str
-    type: DataType
+class ResourceListPage(pydantic_v1.BaseModel):
+    resources: typing.List[ResourceIdentifier]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/document_collections/types/metadata_schema.py` & `credal-0.0.2/src/credal/permissions_service/types/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .metadata_field import MetadataField
 
 
-class MetadataSchema(pydantic_v1.BaseModel):
-    fields: typing.List[MetadataField] = pydantic_v1.Field()
-    """
-    The list of metadata fields.
-    """
+class Group(pydantic_v1.BaseModel):
+    name: str
+    id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/permissions_service/__init__.py` & `credal-0.0.2/src/credal/permissions_service/__init__.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/permissions_service/client.py` & `credal-0.0.2/src/credal/permissions_service/client.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/permissions_service/types/__init__.py` & `credal-0.0.2/src/credal/permissions_service/types/__init__.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/permissions_service/types/check_resource_authorization_response.py` & `credal-0.0.2/src/credal/search/types/single_field_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .operator import Operator
 
 
-class CheckResourceAuthorizationResponse(pydantic_v1.BaseModel):
-    authorized: bool
+class SingleFieldFilter(pydantic_v1.BaseModel):
+    field: str
+    operator: Operator
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/permissions_service/types/group.py` & `credal-0.0.2/src/credal/users/types/user_metadata_patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 
 
-class Group(pydantic_v1.BaseModel):
-    name: str
-    id: typing.Optional[str] = None
+class UserMetadataPatch(pydantic_v1.BaseModel):
+    user_email: str = pydantic_v1.Field(alias="userEmail")
+    metadata: typing.Any = pydantic_v1.Field()
+    """
+    Key-value object of metadata for user. Keys will be merged with any existing values but can also be set to `null` to effectively remove
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
@@ -22,9 +25,11 @@
         return deep_union_pydantic_dicts(
             super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
         )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `credal-0.0.1/src/credal/permissions_service/types/principal.py` & `credal-0.0.2/src/credal/permissions_service/types/principal.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/permissions_service/types/principal_list_page.py` & `credal-0.0.2/src/credal/permissions_service/types/principal_list_page.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/permissions_service/types/resource_authorization_result.py` & `credal-0.0.2/src/credal/search/types/document_collection_search_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
+import uuid
 
-from ...common.types.resource_identifier import ResourceIdentifier
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .search_result_chunk import SearchResultChunk
 
 
-class ResourceAuthorizationResult(pydantic_v1.BaseModel):
-    resource_identifier: ResourceIdentifier = pydantic_v1.Field(alias="resourceIdentifier")
-    authorized: bool
+class DocumentCollectionSearchResult(pydantic_v1.BaseModel):
+    document_id: uuid.UUID = pydantic_v1.Field(alias="documentId")
+    document_name: str = pydantic_v1.Field(alias="documentName")
+    document_metadata: typing.Dict[str, str] = pydantic_v1.Field(alias="documentMetadata")
+    chunks: typing.List[SearchResultChunk]
+    merged_contents: typing.Optional[str] = pydantic_v1.Field(alias="mergedContents", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/permissions_service/types/resource_list_page.py` & `credal-0.0.2/src/credal/search/types/search_document_collection_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
+import uuid
 
-from ...common.types.resource_identifier import ResourceIdentifier
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .document_collection_search_result import DocumentCollectionSearchResult
+from .single_field_filter import SingleFieldFilter
 
 
-class ResourceListPage(pydantic_v1.BaseModel):
-    resources: typing.List[ResourceIdentifier]
+class SearchDocumentCollectionResponse(pydantic_v1.BaseModel):
+    search_terms_used: typing.List[str] = pydantic_v1.Field(alias="searchTermsUsed")
+    structured_filters_applied: typing.List[SingleFieldFilter] = pydantic_v1.Field(alias="structuredFiltersApplied")
+    search_id: uuid.UUID = pydantic_v1.Field(alias="searchId")
+    results: typing.List[DocumentCollectionSearchResult]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
@@ -22,9 +27,11 @@
         return deep_union_pydantic_dicts(
             super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
         )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `credal-0.0.1/src/credal/search/client.py` & `credal-0.0.2/src/credal/search/client.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/search/types/document_collection_search_options.py` & `credal-0.0.2/src/credal/search/types/document_collection_search_options.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/src/credal/search/types/document_collection_search_result.py` & `credal-0.0.2/src/credal/search/types/search_result_chunk.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import datetime as dt
 import typing
 import uuid
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
-from .search_result_chunk import SearchResultChunk
 
 
-class DocumentCollectionSearchResult(pydantic_v1.BaseModel):
-    document_id: uuid.UUID = pydantic_v1.Field(alias="documentId")
-    document_name: str = pydantic_v1.Field(alias="documentName")
-    document_metadata: typing.Dict[str, str] = pydantic_v1.Field(alias="documentMetadata")
-    chunks: typing.List[SearchResultChunk]
-    merged_contents: typing.Optional[str] = pydantic_v1.Field(alias="mergedContents", default=None)
+class SearchResultChunk(pydantic_v1.BaseModel):
+    chunk_id: uuid.UUID = pydantic_v1.Field(alias="chunkId")
+    chunk_index: int = pydantic_v1.Field(alias="chunkIndex")
+    text: str
+    score: float = pydantic_v1.Field()
+    """
+    The similarity score between 0 and 1 for the search result. A higher number means the chunk is more relevant to the search query.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `credal-0.0.1/src/credal/users/client.py` & `credal-0.0.2/src/credal/users/client.py`

 * *Files identical despite different names*

### Comparing `credal-0.0.1/PKG-INFO` & `credal-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credal
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

