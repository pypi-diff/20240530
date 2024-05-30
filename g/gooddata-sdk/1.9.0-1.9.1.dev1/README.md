# Comparing `tmp/gooddata-sdk-1.9.0.tar.gz` & `tmp/gooddata-sdk-1.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-sdk-1.9.0.tar", last modified: Thu Nov 16 13:24:58 2023, max compression
+gzip compressed data, was "gooddata-sdk-1.9.1.dev1.tar", last modified: Thu Dec 14 13:21:19 2023, max compression
```

## Comparing `gooddata-sdk-1.9.0.tar` & `gooddata-sdk-1.9.1.dev1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.118158 gooddata-sdk-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    39862 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-11-16 13:24:58.118158 gooddata-sdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.098158 gooddata-sdk-1.9.0/gooddata_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.102158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/catalog_service_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.102158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.102158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.102158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.102158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/responses/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/sql_column.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    25313 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/validation/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/validation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/depends_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/export/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/export/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14459 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/export/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/directive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/jwk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.106158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/entity_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/entity_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/entity_model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/entity_model/user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25067 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/content_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.110158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/data_filter_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/dataset_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/model_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    46148 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/compute/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.114158 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13732 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/compute/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16764 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/gooddata_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.102158 gooddata-sdk-1.9.0/gooddata_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-11-16 13:24:58.000000 gooddata-sdk-1.9.0/gooddata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-11-16 13:24:58.000000 gooddata-sdk-1.9.0/gooddata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 13:24:58.000000 gooddata-sdk-1.9.0/gooddata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-16 13:24:58.000000 gooddata-sdk-1.9.0/gooddata_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-16 13:24:58.000000 gooddata-sdk-1.9.0/gooddata_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 13:24:58.118158 gooddata-sdk-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:24:58.118158 gooddata-sdk-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2023-11-16 13:24:41.000000 gooddata-sdk-1.9.0/tests/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    39862 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-12-14 13:21:12.000000 gooddata-sdk-1.9.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.103675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/catalog_service_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/scan_sql_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/sql_column.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.107675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22226 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/validation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/depends_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/export/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14459 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/export/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/directive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.111675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/entity_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/entity_model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/entity_model/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25067 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/content_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/data_filter_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/dataset_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.115675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15619 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/model_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46148 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13732 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16764 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-12-14 13:21:19.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-12-14 13:21:19.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 13:21:19.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-14 13:21:19.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-14 13:21:19.000000 gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-12-14 13:21:12.000000 gooddata-sdk-1.9.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:19.119675 gooddata-sdk-1.9.1.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2023-12-14 13:20:56.000000 gooddata-sdk-1.9.1.dev1/tests/test_type_converter.py
```

### Comparing `gooddata-sdk-1.9.0/LICENSE.txt` & `gooddata-sdk-1.9.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/PKG-INFO` & `gooddata-sdk-1.9.1.dev1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: GoodData Cloud Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.9.0
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.9.1.dev1
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,20 +18,20 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-api-client~=1.9.0
+Requires-Dist: gooddata-api-client~=1.9.1.dev1
 Requires-Dist: python-dateutil>=2.5.3
 Requires-Dist: pyyaml>=5.1
-Requires-Dist: attrs==21.4.0
-Requires-Dist: cattrs==22.1.0
-Requires-Dist: brotli==1.0.9
+Requires-Dist: attrs<=23.1.0,>=21.4.0
+Requires-Dist: cattrs<=23.2.3,>=22.1.0
+Requires-Dist: brotli==1.1.0
 
 # GoodData Python SDK
 
 The `gooddata-sdk` package provides a clean and convenient Python API to interact with [GoodData](https://www.gooddata.com/).
 
 At the moment the SDK provides services to inspect and interact with the Semantic Model and consume analytics:
 * Catalog Workspaces Service
@@ -40,20 +40,20 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.9.0) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.9.1.dev1) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
--  Python 3.7 or newer
+-  Python 3.8 or newer
 
 ## Installation
 
 Run the following command to install the `gooddata-sdk` package on your system:
 
     pip install gooddata-sdk
```

### Comparing `gooddata-sdk-1.9.0/README.md` & `gooddata-sdk-1.9.1.dev1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.9.0) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.9.1.dev1) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
--  Python 3.7 or newer
+-  Python 3.8 or newer
 
 ## Installation
 
 Run the following command to install the `gooddata-sdk` package on your system:
 
     pip install gooddata-sdk
```

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/__init__.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from gooddata_sdk.catalog.data_source.action_model.requests.scan_model_request import CatalogScanModelRequest
 from gooddata_sdk.catalog.data_source.action_model.requests.scan_sql_request import ScanSqlRequest
 from gooddata_sdk.catalog.data_source.action_model.responses.scan_sql_response import ScanSqlResponse
 from gooddata_sdk.catalog.data_source.action_model.sql_column import SqlColumn
 from gooddata_sdk.catalog.data_source.declarative_model.data_source import (
     CatalogDeclarativeDataSource,
     CatalogDeclarativeDataSources,
-    CatalogDeclarativeTables,
 )
+from gooddata_sdk.catalog.data_source.declarative_model.physical_model.pdm import CatalogDeclarativeTables
 from gooddata_sdk.catalog.data_source.declarative_model.physical_model.table import (
     CatalogDeclarativeColumn,
     CatalogDeclarativeTable,
 )
 from gooddata_sdk.catalog.data_source.entity_model.content_objects.table import CatalogDataSourceTable
 from gooddata_sdk.catalog.data_source.entity_model.data_source import (
     CatalogDataSource,
```

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/base.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/catalog_service_base.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/catalog_service_base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/ldm_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/requests/scan_model_request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/action_model/responses/scan_sql_response.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/data_source.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/data_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import attr
 
 from gooddata_api_client.model.declarative_data_source import DeclarativeDataSource
 from gooddata_api_client.model.declarative_data_sources import DeclarativeDataSources
 from gooddata_api_client.model.test_definition_request import TestDefinitionRequest
 from gooddata_sdk.catalog.base import Base, value_in_allowed
-from gooddata_sdk.catalog.data_source.declarative_model.physical_model.pdm import CatalogDeclarativeTables
 from gooddata_sdk.catalog.entity import TokenCredentialsFromFile
 from gooddata_sdk.catalog.parameter import CatalogParameter
 from gooddata_sdk.catalog.permission.declarative_model.permission import CatalogDeclarativeDataSourcePermission
 from gooddata_sdk.utils import create_directory, read_layout_from_file, write_layout_to_file
 
 BIGQUERY_TYPE = "BIGQUERY"
 LAYOUT_DATA_SOURCES_DIR = "data_sources"
@@ -67,15 +66,14 @@
 class CatalogDeclarativeDataSource(Base):
     id: str
     name: str
     type: str = attr.field(validator=value_in_allowed)
     url: Optional[str] = None
     schema: str
     enable_caching: Optional[bool] = None
-    pdm: CatalogDeclarativeTables = CatalogDeclarativeTables()
     cache_path: Optional[List[str]] = None
     username: Optional[str] = None
     parameters: Optional[List[CatalogParameter]] = None
     decoded_parameters: Optional[List[CatalogParameter]] = None
     permissions: List[CatalogDeclarativeDataSourcePermission] = attr.field(factory=list)
 
     def to_test_request(
@@ -102,34 +100,27 @@
         create_directory(data_source_folder)
         return data_source_folder
 
     def to_api(
         self, password: Optional[str] = None, token: Optional[str] = None, include_nested_structures: bool = True
     ) -> DeclarativeDataSource:
         dictionary = self._get_snake_dict()
-        if not include_nested_structures:
-            del dictionary["pdm"]
         if password is not None:
             dictionary["password"] = password
         if token is not None:
             dictionary["token"] = token
         return self.client_class().from_dict(dictionary)
 
     def store_to_disk(self, data_sources_folder: Path) -> None:
         data_source_folder = self.data_source_folder(data_sources_folder, self.id)
         file_path = data_source_folder / f"{self.id}.yaml"
         data_source_dict = self.to_api(include_nested_structures=False).to_dict(camel_case=True)
 
         write_layout_to_file(file_path, data_source_dict)
 
-        if self.pdm is not None:
-            self.pdm.store_to_disk(data_source_folder)
-
     @classmethod
     def load_from_disk(cls, data_sources_folder: Path, data_source_id: str) -> CatalogDeclarativeDataSource:
         data_source_folder = data_sources_folder / data_source_id
         data_source_file_path = data_source_folder / f"{data_source_id}.yaml"
-        pdm = CatalogDeclarativeTables.load_from_disk(data_source_folder)
         data_source_dict = read_layout_from_file(data_source_file_path)
         data_source = CatalogDeclarativeDataSource.from_dict(data_source_dict)
-        data_source.pdm = pdm
         return data_source
```

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/column.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/pdm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/declarative_model/physical_model/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/content_objects/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/entity_model/data_source.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/entity_model/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # (C) 2022 GoodData Corporation
 from __future__ import annotations
 
 import functools
 from pathlib import Path
-from typing import Any, List, Optional
-from warnings import warn
+from typing import Any, List, Optional, Tuple
 
 from gooddata_api_client.exceptions import NotFoundException
-from gooddata_api_client.model.declarative_pdm import DeclarativePdm
 from gooddata_sdk.catalog.catalog_service_base import CatalogServiceBase
-from gooddata_sdk.catalog.data_source.action_model.requests.ldm_request import CatalogGenerateLdmRequest
+from gooddata_sdk.catalog.data_source.action_model.requests.ldm_request import (
+    CatalogGenerateLdmRequest,
+    CatalogPdmLdmRequest,
+)
 from gooddata_sdk.catalog.data_source.action_model.requests.scan_model_request import CatalogScanModelRequest
 from gooddata_sdk.catalog.data_source.action_model.requests.scan_sql_request import ScanSqlRequest
 from gooddata_sdk.catalog.data_source.action_model.responses.scan_sql_response import ScanSqlResponse
 from gooddata_sdk.catalog.data_source.declarative_model.data_source import (
     BIGQUERY_TYPE,
     CatalogDeclarativeDataSource,
     CatalogDeclarativeDataSources,
@@ -251,169 +252,47 @@
 
         Returns:
             None
         """
         data_sources = self.load_declarative_data_sources(layout_root_path)
         self.put_declarative_data_sources(data_sources, credentials_path, test_data_sources)
 
-    def get_declarative_pdm(self, data_source_id: str) -> CatalogDeclarativeTables:
-        """Retrieve physical data model for a given data source.
-
-        Args:
-            data_source_id (str):
-                Data Source identification string. e.g. "demo"
-
-        Returns:
-            CatalogDeclarativeTables:
-                Physical Data Model object.
-        """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return CatalogDeclarativeTables.from_api(self._layout_api.get_pdm_layout(data_source_id).get("pdm"))
-
-    def put_declarative_pdm(self, data_source_id: str, declarative_tables: CatalogDeclarativeTables) -> None:
-        """Set physical data model for a given data source.
-
-        Args:
-            data_source_id (str):
-                Data Source identification string. e.g. "demo"
-            declarative_tables (CatalogDeclarativeTables):
-                Physical Data Model object. Can be obtained via get_declarative_pdm.
-
-        Returns:
-            None
-        """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        declarative_pdm = DeclarativePdm(pdm=declarative_tables.to_api())
-        self._layout_api.set_pdm_layout(data_source_id, declarative_pdm)
-
-    def store_declarative_pdm(self, data_source_id: str, layout_root_path: Path = Path.cwd()) -> None:
-        """Store physical data model layout in directory hierarchy for a given data source.
-
-        gooddata_layouts
-        └── organization_id
-                └── data_sources
-                        └── data_source_a
-                                └── pdm
-                                    ├── table_A.yaml
-                                    └── table_B.yaml
-
-        Args:
-            data_source_id (str):
-                Data Source identification string. e.g. "demo"
-            layout_root_path (Path, optional):
-                Path to the root of the layout directory. Defaults to Path.cwd().
-
-        Returns:
-            None
-        """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        data_source_folder = self.data_source_folder(data_source_id, layout_root_path)
-        self.get_declarative_pdm(data_source_id).store_to_disk(data_source_folder)
-
-    def load_declarative_pdm(
-        self, data_source_id: str, layout_root_path: Path = Path.cwd()
-    ) -> CatalogDeclarativeTables:
-        """Load declarative physical data model layout.
-
-        Load declarative physical data model layout, which was stored using
-        `store_declarative_pdm` for a given data source.
-
-        Args:
-            data_source_id (str):
-                Data Source identification string. e.g. "demo"
-            layout_root_path (Path, optional):
-                Path to the root of the layout directory. Defaults to Path.cwd().
-
-        Returns:
-            CatalogDeclarativeTables: Physical Data Model object.
-        """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        data_source_folder = self.data_source_folder(data_source_id, layout_root_path)
-        return CatalogDeclarativeTables.load_from_disk(data_source_folder)
-
-    def load_and_put_declarative_pdm(self, data_source_id: str, layout_root_path: Path = Path.cwd()) -> None:
-        """Loads and sets layouts stored using `store_declarative_pdm`.
-
-        This method combines load_declarative_pdm and `put_declarative_pdm` methods
-        to load and set layouts stored using `store_declarative_pdm`.
-
-        Args:
-            data_source_id (str):
-                Data Source identification string. e.g. "demo"
-            layout_root_path (Path, optional):
-                Path to the root of the layout directory. Defaults to Path.cwd().
-
-        Returns:
-            None
-        """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self.put_declarative_pdm(data_source_id, self.load_declarative_pdm(data_source_id, layout_root_path))
-
-    def store_pdm_to_disk(self, datasource_id: str, path: Path = Path.cwd()) -> None:
-        """Store the physical data model layout in the directory for a given data source.
+    @staticmethod
+    def store_pdm_to_disk(pdm: CatalogDeclarativeTables, path: Path = Path.cwd()) -> None:
+        """Store the physical data model layout in the directory.
 
         The directory structure below shows the output for the path set to Path("pdm_location").
         pdm_location
             └── pdm
                 ├── table_A.yaml
                 └── table_B.yaml
 
         Args:
-            datasource_id (str):
-                Data Source identification string. e.g. "demo"
+            pdm (CatalogDeclarativeTables):
+                Declarative PDM definition to be persisted on disk.
             path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             None
         """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self.get_declarative_pdm(datasource_id).store_to_disk(path)
+        pdm.store_to_disk(path)
 
     @staticmethod
     def load_pdm_from_disk(path: Path = Path.cwd()) -> CatalogDeclarativeTables:
         """This method is used to load pdm stored to disk using method store_pdm_to_disk.
 
         Args:
             path (Path, optional):
                 Path to the root of the layout directory. Defaults to Path.cwd().
 
         Returns:
             CatalogDeclarativeTables:
                 Physical Data Model object.
         """
-        warn(
-            _PDM_DEPRECATION_MSG,
-            DeprecationWarning,
-            stacklevel=2,
-        )
         return CatalogDeclarativeTables.load_from_disk(path)
 
     # Actions methods are listed below
 
     def generate_logical_model(
         self,
         data_source_id: str,
@@ -431,14 +310,53 @@
             CatalogDeclarativeModel:
                 Object Containing declarative Logical Data Model
         """
         return CatalogDeclarativeModel.from_api(
             self._actions_api.generate_logical_model(data_source_id, generate_ldm_request.to_api())
         )
 
+    def scan_pdm_and_generate_logical_model(
+        self,
+        data_source_id: str,
+        generate_ldm_request: CatalogGenerateLdmRequest = CatalogGenerateLdmRequest(separator="__", wdf_prefix="wdf"),
+        scan_request: CatalogScanModelRequest = CatalogScanModelRequest(),
+        report_warnings: bool = False,
+    ) -> Tuple[CatalogDeclarativeModel, CatalogScanResultPdm]:
+        """Scan data source and use returned PDM to generate logical data model. If generate_ldm_request
+        contains PDM already, PDM tables received from the scan are appended without deduplication.
+
+        Args:
+            data_source_id (str):
+                Data Source identification string. e.g. "demo"
+            generate_ldm_request (CatalogGenerateLdmRequest, optional):
+                LDM options. Defaults to CatalogGenerateLdmRequest(separator="__", wdf_prefix="wdf")
+            scan_request (CatalogScanModelRequest, optional):
+                Options for the Scan Request. Defaults to CatalogScanModelRequest().
+            report_warnings (bool, optional):
+                Switch to turn on warnings. Defaults to False.
+
+
+        Returns:
+            CatalogDeclarativeModel:
+                Object Containing declarative Logical Data Model
+            CatalogScanResultPdm:
+                An instance of CatalogScanResultPdm.
+                Containing pdm itself and a list of warnings that occurred during scanning.
+        """
+        scan_result = self.scan_data_source(data_source_id, scan_request, report_warnings)
+        if generate_ldm_request.pdm and generate_ldm_request.pdm.tables:
+            generate_ldm_request.pdm.tables.extend(scan_result.pdm.tables)
+        elif generate_ldm_request.pdm:
+            generate_ldm_request.pdm.tables = scan_result.pdm.tables
+        else:
+            generate_ldm_request.pdm = CatalogPdmLdmRequest(tables=scan_result.pdm.tables)
+        return CatalogDeclarativeModel.from_api(
+            self._actions_api.generate_logical_model(data_source_id, generate_ldm_request.to_api())
+        ), scan_result
+
     def register_upload_notification(self, data_source_id: str) -> None:
         """Invalidate cache of your computed reports to force your analytics to be recomputed.
 
         Args:
             data_source_id (str):
                 Data Source identification string. e.g. "demo"
 
@@ -477,30 +395,14 @@
         scan_result = CatalogScanResultPdm.from_api(
             self._actions_api.scan_data_source(data_source_id, scan_request.to_api())
         )
         if report_warnings:
             self.report_warnings(scan_result.warnings)
         return scan_result
 
-    def scan_and_put_pdm(
-        self, data_source_id: str, scan_request: CatalogScanModelRequest = CatalogScanModelRequest()
-    ) -> None:
-        """This method combines scan_data_source and put_declarative_pdm methods.
-
-        Args:
-            data_source_id (str):
-                Data Source identification string. e.g. "demo"
-            scan_request (CatalogScanModelRequest, optional):
-                Options for the Scan Request. Defaults to CatalogScanModelRequest().
-
-        Returns:
-            None
-        """
-        self.put_declarative_pdm(data_source_id, self.scan_data_source(data_source_id, scan_request).pdm)
-
     def scan_schemata(self, data_source_id: str) -> list[str]:
         """Returns a list of schemas that exist in the database.
 
         Can be configured in the data source entity. Data source
         managers like Dremio or Drill can work with multiple schemas
         and schema names can be injected into scan_request to filter
         out tables stored in the different schemas.
```

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/data_source/validation/data_source.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/data_source/validation/data_source.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/entity.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/entity.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/export/request.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/export/request.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/export/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/export/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/identifier.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/identifier.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/directive.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/directive.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/jwk.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/jwk.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/organization.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/organization.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/entity_model/setting.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/entity_model/setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/organization/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/organization/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_assignees.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/manage_dashboard_permissions.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/declarative_model/permission.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/declarative_model/permission.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/permission/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/permission/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/setting.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/user.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_and_user_groups.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/declarative_model/user_group.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/declarative_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/entity_model/user.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/entity_model/user.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/entity_model/user_group.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/entity_model/user_group.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/user/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/user/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/content_service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/content_service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/analytics_model/analytics_model.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/data_filter_references.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/data_filter_references.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/dataset_extension.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/dataset_extensions/dataset_extension.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/date_dataset/date_dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/logical_model/ldm.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/declarative_model/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/dataset.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/content_objects/workspace_setting.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/graph_objects/graph.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/user_data_filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/entity_model/workspace.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/entity_model/workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/model_container.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/model_container.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/catalog/workspace/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/catalog/workspace/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/client.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/compute/model/attribute.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/attribute.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/compute/model/base.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/base.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/compute/model/execution.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/execution.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/compute/model/filter.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/compute/model/metric.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/model/metric.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/compute/service.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/compute/service.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/insight.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/insight.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/sdk.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/support.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/support.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/table.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/table.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/type_converter.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/type_converter.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk/utils.py` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk.egg-info/PKG-INFO` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-sdk
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: GoodData Cloud Python SDK
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.9.0
+Project-URL: Documentation, https://www.gooddata.com/docs/python-sdk/1.9.1.dev1
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,sdk,api,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,20 +18,20 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-api-client~=1.9.0
+Requires-Dist: gooddata-api-client~=1.9.1.dev1
 Requires-Dist: python-dateutil>=2.5.3
 Requires-Dist: pyyaml>=5.1
-Requires-Dist: attrs==21.4.0
-Requires-Dist: cattrs==22.1.0
-Requires-Dist: brotli==1.0.9
+Requires-Dist: attrs<=23.1.0,>=21.4.0
+Requires-Dist: cattrs<=23.2.3,>=22.1.0
+Requires-Dist: brotli==1.1.0
 
 # GoodData Python SDK
 
 The `gooddata-sdk` package provides a clean and convenient Python API to interact with [GoodData](https://www.gooddata.com/).
 
 At the moment the SDK provides services to inspect and interact with the Semantic Model and consume analytics:
 * Catalog Workspaces Service
@@ -40,20 +40,20 @@
 * Catalog User Service
 * Catalog Permission Service
 * Catalog Organization Service
 * Insights Service
 * Compute Service
 * Table Service
 
-See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.9.0) for more details.
+See [DOCUMENTATION](https://www.gooddata.com/docs/python-sdk/1.9.1.dev1) for more details.
 
 ## Requirements
 
 -  GoodData Cloud or GoodData.CN installation
--  Python 3.7 or newer
+-  Python 3.8 or newer
 
 ## Installation
 
 Run the following command to install the `gooddata-sdk` package on your system:
 
     pip install gooddata-sdk
```

### Comparing `gooddata-sdk-1.9.0/gooddata_sdk.egg-info/SOURCES.txt` & `gooddata-sdk-1.9.1.dev1/gooddata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-sdk-1.9.0/setup.py` & `gooddata-sdk-1.9.1.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-api-client~=1.9.0",
+    "gooddata-api-client~=1.9.1.dev1",
     "python-dateutil>=2.5.3",
     "pyyaml>=5.1",
-    "attrs==21.4.0",
-    "cattrs==22.1.0",
-    "brotli==1.0.9",
+    "attrs>=21.4.0,<=23.1.0",
+    "cattrs>=22.1.0,<=23.2.3",
+    "brotli==1.1.0",
 ]
 
 setup(
     name="gooddata-sdk",
     description="GoodData Cloud Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.9.0",
+    version="1.9.1.dev1",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.8.0",
     project_urls={
-        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.9.0",
+        "Documentation": "https://www.gooddata.com/docs/python-sdk/1.9.1.dev1",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
```

### Comparing `gooddata-sdk-1.9.0/tests/test_type_converter.py` & `gooddata-sdk-1.9.1.dev1/tests/test_type_converter.py`

 * *Files identical despite different names*

