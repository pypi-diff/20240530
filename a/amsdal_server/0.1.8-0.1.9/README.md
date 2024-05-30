# Comparing `tmp/amsdal_server-0.1.8.tar.gz` & `tmp/amsdal_server-0.1.9.tar.gz`

## Comparing `amsdal_server-0.1.8.tar` & `amsdal_server-0.1.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/.editorconfig
--rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/py.typed
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/errors.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/class_create.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/class_delete.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/class_detail.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/class_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/mixins/__init__.py
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/mixins/column_info_mixin.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/mixins/model_class_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/serializers/__init__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/serializers/class_info.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/serializers/register_class.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/services/__init__.py
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/classes/services/classes_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/__init__.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/authentication.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/depends.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/error_handlers/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/error_handlers/class_not_found.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/error_handlers/invalid_auth.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/__init__.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/logger.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/response_event.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/mixins/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/mixins/permissions_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/permissions/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/permissions/enums.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/permissions/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/base_serializer.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/column_format.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/column_response.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/fields_restriction.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/filter.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/objects_response.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/option.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/enums.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/controllers/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/controllers/liveness.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/controllers/readiness.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/serializers/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/serializers/healthcheck_result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/services/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/services/healthcheck.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/services/checkers/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/services/checkers/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/router.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/file_download.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_create.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_delete.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_detail.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_list.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_update.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/mixins/__init__.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/mixins/object_data_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/file_object.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/object_api.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/object_list_api.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/object_versions_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/router.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/controllers/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/controllers/transaction_execute.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/controllers/transaction_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/mixins/__init__.py
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/serializers/__init__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/serializers/transaction_item.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/serializers/transaction_property.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/services/__init__.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/services/transaction_api.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/apps/transactions/services/transaction_execution_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/configs/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/configs/constants.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/configs/main.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/src/amsdal_server/docs/api.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/.gitignore
--rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0    27844 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/README.md
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    57048 2020-02-02 00:00:00.000000 amsdal_server-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    41901 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/.editorconfig
+-rw-r--r--   0        0        0    62595 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/py.typed
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/errors.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/class_create.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/class_delete.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/class_detail.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/class_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/mixins/__init__.py
+-rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/mixins/column_info_mixin.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/mixins/model_class_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/serializers/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/serializers/class_info.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/serializers/register_class.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/services/__init__.py
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/classes/services/classes_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/__init__.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/authentication.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/depends.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/error_handlers/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/error_handlers/class_not_found.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/error_handlers/invalid_auth.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/__init__.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/logger.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/response_event.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/mixins/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/mixins/permissions_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/permissions/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/permissions/enums.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/permissions/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/base_serializer.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/column_format.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/column_response.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/fields_restriction.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/filter.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/objects_response.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/option.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/enums.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/controllers/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/controllers/liveness.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/controllers/readiness.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/serializers/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/serializers/healthcheck_result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/services/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/services/healthcheck.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/services/checkers/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/services/checkers/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/router.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/file_download.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_create.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_delete.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_detail.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_list.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_update.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/mixins/__init__.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/mixins/object_data_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/file_object.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/object_api.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/object_list_api.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/object_versions_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/router.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/controllers/__init__.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/controllers/transaction_execute.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/controllers/transaction_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/mixins/__init__.py
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/serializers/__init__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/serializers/transaction_item.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/serializers/transaction_property.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/services/__init__.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/services/transaction_api.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/apps/transactions/services/transaction_execution_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/configs/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/configs/constants.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/configs/main.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/src/amsdal_server/docs/api.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/.gitignore
+-rw-r--r--   0        0        0    27355 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0    27844 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/README.md
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    57048 2020-02-02 00:00:00.000000 amsdal_server-0.1.9/PKG-INFO
```

### Comparing `amsdal_server-0.1.8/.editorconfig` & `amsdal_server-0.1.9/.editorconfig`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md` & `amsdal_server-0.1.9/src/amsdal_server/Third-Party Materials - AMSDAL Dependencies - License Notices.md`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/server.py` & `amsdal_server-0.1.9/src/amsdal_server/server.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/router.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/router.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/errors.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/errors.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/class_create.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/class_create.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/controllers/class_list.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/controllers/class_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/mixins/column_info_mixin.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/mixins/column_info_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/mixins/model_class_info.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/mixins/model_class_info.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/serializers/register_class.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/serializers/register_class.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/classes/services/classes_api.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/classes/services/classes_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/authentication.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/authentication.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/depends.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/depends.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/errors.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/errors.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/error_handlers/validation_error_handler.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/logger.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/logger.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/response_event.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/response_event.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/middlewares/utils.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/middlewares/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/mixins/permissions_mixin.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/mixins/permissions_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/column_response.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/column_response.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/common/serializers/filter.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/common/serializers/filter.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/controllers/liveness.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/controllers/liveness.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/healthcheck/services/healthcheck.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/healthcheck/services/healthcheck.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/utils.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/file_download.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/file_download.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_create.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_create.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_detail.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_detail.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_list.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     include_subclasses: bool = True,
     load_references: bool = False,
     all_versions: bool = False,
     file_optimized: bool = False,
     fields_restrictions: dict[str, FieldsRestriction] = Depends(get_fields_restrictions),
     filters: list[Filter] = Depends(get_filters),
     page: int = 1,
-    page_size: int = 10,
+    page_size: int | None = Query(default=None),
     ordering: list[str] | None = Query(default=None),
 ) -> dict[str, Any]:
     return ObjectListApi.fetch_objects(
         request.user,
         base_url=str(request.base_url),
         class_name=class_name,
         filters=filters,
```

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/controllers/object_update.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/controllers/object_update.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/mixins/object_data_mixin.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/mixins/object_data_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/file_object.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/file_object.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/object_api.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/object_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/object_list_api.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/object_list_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         include_metadata: bool = False,
         include_subclasses: bool = False,
         fields_restrictions: dict[str, FieldsRestriction] | None = None,
         load_references: bool = False,
         all_versions: bool = False,
         file_optimized: bool = False,
         page: int = 1,
-        page_size: int = 10,
+        page_size: int | None = None,
         ordering: list[str] | None = None,
     ) -> ObjectsResponse:
         model_class = cls.get_model_class_by_name(class_name)
         permissions_info = cls.get_permissions_info(model_class, user)
         class_item: Model = cls.get_class_objects_qs().get(_address__object_id=class_name).execute()
         class_meta_item: Model = cls.get_class_object_metas_qs().get(_address__object_id=class_item.object_id).execute()
 
@@ -102,15 +102,15 @@
         include_subclasses: bool = False,
         include_metadata: bool = False,
         fields_restrictions: dict[str, FieldsRestriction] | None = None,
         load_references: bool = False,
         all_versions: bool = False,
         file_optimized: bool = False,
         page: int = 1,
-        page_size: int = 10,
+        page_size: int | None = None,
         ordering: list[str] | None = None,
     ) -> tuple[list[dict[str, Any]], int]:
         result: list[dict[str, Any]] = []
         total: int = 0
         classes: list[type[ModelBase]] = [model_class]
 
         if include_subclasses:
@@ -147,17 +147,21 @@
                 )
 
             total += qs.count().execute()
 
             if ordering is None:
                 ordering = ['-_metadata__updated_at']
 
-            offset = (page - 1) * page_size
-            limit = offset + page_size
-            qs = qs.order_by(*ordering)[offset:limit]
+            qs = qs.order_by(*ordering)
+
+            if page_size is not None:
+                offset = (page - 1) * page_size
+                limit = offset + page_size
+
+                qs = qs[offset:limit]
 
             items: list[Model] = qs.execute()
 
             for item in items:
                 result.append(
                     cls.build_object_data(
                         item,
```

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/objects/services/object_versions_api.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/objects/services/object_versions_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/transactions/utils.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/transactions/utils.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/transactions/controllers/transaction_list.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/transactions/controllers/transaction_list.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/transactions/mixins/ast_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/transactions/services/transaction_api.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/transactions/services/transaction_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/apps/transactions/services/transaction_execution_api.py` & `amsdal_server-0.1.9/src/amsdal_server/apps/transactions/services/transaction_execution_api.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/configs/constants.py` & `amsdal_server-0.1.9/src/amsdal_server/configs/constants.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/configs/main.py` & `amsdal_server-0.1.9/src/amsdal_server/configs/main.py`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/src/amsdal_server/docs/api.md` & `amsdal_server-0.1.9/src/amsdal_server/docs/api.md`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/LICENSE.txt` & `amsdal_server-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/README.md` & `amsdal_server-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/pyproject.toml` & `amsdal_server-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amsdal_server-0.1.8/PKG-INFO` & `amsdal_server-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: amsdal_server
-Version: 0.1.8
+Version: 0.1.9
 Summary: Rest API server for AMSDAL framework
 Project-URL: Documentation, https://pypi.org/project/amsdal_server/#readme
 Project-URL: Issues, https://pypi.org/project/amsdal_server/
 Project-URL: Source, https://pypi.org/project/amsdal_server/
 Author-email: "A. Michael Salem" <ams@amsdal.com>
 License: AMSDAL End User License Agreement
```

