# Comparing `tmp/argilla_server-1.29.0.tar.gz` & `tmp/argilla_server-1.29.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argilla_server-1.29.0.tar", last modified: Thu May 30 15:56:11 2024, max compression
+gzip compressed data, was "argilla_server-1.29.0rc1.tar", last modified: Thu May 30 14:29:59 2024, max compression
```

## Comparing `argilla_server-1.29.0.tar` & `argilla_server-1.29.0rc1.tar`

### file list

```diff
@@ -1,791 +1,791 @@
--rw-r--r--   0        0        0     2974 2024-05-30 15:47:37.395383 argilla_server-1.29.0/README.md
--rw-r--r--   0        0        0     3924 2024-05-30 15:56:11.729505 argilla_server-1.29.0/pyproject.toml
--rw-r--r--   0        0        0      907 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/__init__.py
--rw-r--r--   0        0        0      695 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/__main__.py
--rw-r--r--   0        0        0     8482 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/_app.py
--rw-r--r--   0        0        0      843 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/_messages.py
--rw-r--r--   0        0        0      646 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/_version.py
--rw-r--r--   0        0        0     3206 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic.ini
--rw-r--r--   0        0        0     2986 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/env.py
--rw-r--r--   0        0        0      510 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/script.py.mako
--rw-r--r--   0        0        0     1589 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/1769ee58fbb4_create_workspaces_users_table.py
--rw-r--r--   0        0        0     1225 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/1e629a913727_fix_suggestions_type_enum_values.py
--rw-r--r--   0        0        0     1777 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/3a8e2f9b5dea_create_questions_table.py
--rw-r--r--   0        0        0     2891 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/3fc3c0839959_create_suggestions_table.py
--rw-r--r--   0        0        0     1290 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/3ff6484f8b37_add_record_metadata_column.py
--rw-r--r--   0        0        0     1578 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/74694870197c_create_users_table.py
--rw-r--r--   0        0        0     2280 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/7850ab5b42d9_create_vectors_settings_table.py
--rw-r--r--   0        0        0     2394 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/7cbcccf8b57a_create_metadata_properties_table.py
--rw-r--r--   0        0        0     1302 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/82a5a88a3fa5_create_workspaces_table.py
--rw-r--r--   0        0        0     1513 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/84f6b9ff6076_add_last_activity_at_to_datasets_table.py
--rw-r--r--   0        0        0     1544 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/8be56284dac0_create_records_table.py
--rw-r--r--   0        0        0     2750 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/8c574ada5e5f_update_enum_columns.py
--rw-r--r--   0        0        0     1722 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/ae5522b4c674_create_fields_table.py
--rw-r--r--   0        0        0     1388 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/b8458008b60e_add_allow_extra_metadata_column_to_.py
--rw-r--r--   0        0        0     1629 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/b9099dc08489_create_datasets_table.py
--rw-r--r--   0        0        0     2285 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/bda6fe24314e_create_vectors_table.py
--rw-r--r--   0        0        0     2583 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/ca7293c38970_change_suggestions_score_column_to_json.py
--rw-r--r--   0        0        0     1634 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/alembic/versions/e402e9d9245e_create_responses_table.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/errors/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/errors/v1/__init__.py
--rw-r--r--   0        0        0     1076 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/errors/v1/exception_handlers.py
--rw-r--r--   0        0        0     4134 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/routes.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/__init__.py
--rw-r--r--   0        0        0     1571 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/authentication.py
--rw-r--r--   0        0        0     6008 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/datasets.py
--rw-r--r--   0        0        0     1205 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/info.py
--rw-r--r--   0        0        0     4616 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/metrics.py
--rw-r--r--   0        0        0     3975 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/records.py
--rw-r--r--   0        0        0     4565 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/records_search.py
--rw-r--r--   0        0        0     3057 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/records_update.py
--rw-r--r--   0        0        0     4790 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/text2text.py
--rw-r--r--   0        0        0    14645 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/text_classification.py
--rw-r--r--   0        0        0     5584 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/text_classification_dataset_settings.py
--rw-r--r--   0        0        0     5674 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/token_classification.py
--rw-r--r--   0        0        0     5588 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/token_classification_dataset_settings.py
--rw-r--r--   0        0        0     4442 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/users.py
--rw-r--r--   0        0        0     4388 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/workspaces.py
--rw-r--r--   0        0        0     1710 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/helpers.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/commons/__init__.py
--rw-r--r--   0        0        0     1907 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/commons/model.py
--rw-r--r--   0        0        0     2163 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/commons/params.py
--rw-r--r--   0        0        0     2046 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/dataset_settings.py
--rw-r--r--   0        0        0     2637 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/text2text.py
--rw-r--r--   0        0        0     5074 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/text_classification.py
--rw-r--r--   0        0        0     3191 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/models/token_classification.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/validators/__init__.py
--rw-r--r--   0        0        0      974 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/validators/commons.py
--rw-r--r--   0        0        0     4343 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/validators/text_classification.py
--rw-r--r--   0        0        0     4216 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v0/validators/token_classification.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v1/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/__init__.py
--rw-r--r--   0        0        0     1407 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/authentication.py
--rw-r--r--   0        0        0     1198 2024-05-30 15:47:37.399383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/__init__.py
--rw-r--r--   0        0        0    14798 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/datasets.py
--rw-r--r--   0        0        0     2996 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/questions.py
--rw-r--r--   0        0        0    27687 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/records.py
--rw-r--r--   0        0        0     3866 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/records_bulk.py
--rw-r--r--   0        0        0     2918 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/fields.py
--rw-r--r--   0        0        0     1261 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/info.py
--rw-r--r--   0        0        0     3744 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/metadata_properties.py
--rw-r--r--   0        0        0     4109 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/oauth2.py
--rw-r--r--   0        0        0     3069 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/questions.py
--rw-r--r--   0        0        0     8457 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/records.py
--rw-r--r--   0        0        0     3806 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/responses.py
--rw-r--r--   0        0        0      925 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/settings.py
--rw-r--r--   0        0        0     2219 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/suggestions.py
--rw-r--r--   0        0        0     4271 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/users.py
--rw-r--r--   0        0        0     2706 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/vectors_settings.py
--rw-r--r--   0        0        0     7027 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/workspaces.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/bulk/__init__.py
--rw-r--r--   0        0        0    10789 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/bulk/records_bulk.py
--rw-r--r--   0        0        0      671 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/__main__.py
--rw-r--r--   0        0        0      671 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/__init__.py
--rw-r--r--   0        0        0     1045 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/__main__.py
--rw-r--r--   0        0        0     1760 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/migrate.py
--rw-r--r--   0        0        0     1388 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/revisions.py
--rw-r--r--   0        0        0      671 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/__init__.py
--rw-r--r--   0        0        0     1289 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/__main__.py
--rw-r--r--   0        0        0     5357 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/create.py
--rw-r--r--   0        0        0     2390 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/create_default.py
--rw-r--r--   0        0        0     4101 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/migrate.py
--rw-r--r--   0        0        0     1890 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/update.py
--rw-r--r--   0        0        0     1064 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/users/utils.py
--rw-r--r--   0        0        0     1058 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/database/utils.py
--rw-r--r--   0        0        0     1386 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/rich.py
--rw-r--r--   0        0        0      671 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/search_engine/__init__.py
--rw-r--r--   0        0        0      889 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/search_engine/__main__.py
--rw-r--r--   0        0        0     6068 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/search_engine/reindex.py
--rw-r--r--   0        0        0     1087 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/start.py
--rw-r--r--   0        0        0     2488 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/cli/typer_ext.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/commons/__init__.py
--rw-r--r--   0        0        0     3685 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/commons/config.py
--rw-r--r--   0        0        0      999 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/commons/models.py
--rw-r--r--   0        0        0     1203 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/constants.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/__init__.py
--rw-r--r--   0        0        0     8275 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/accounts.py
--rw-r--r--   0        0        0    43287 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/datasets.py
--rw-r--r--   0        0        0     1441 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/info.py
--rw-r--r--   0        0        0     3151 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/questions.py
--rw-r--r--   0        0        0     2320 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/records.py
--rw-r--r--   0        0        0     5200 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/search.py
--rw-r--r--   0        0        0     1459 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/contexts/settings.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/__init__.py
--rw-r--r--   0        0        0      694 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/__init__.py
--rw-r--r--   0        0        0     3625 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/base.py
--rw-r--r--   0        0        0      728 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/__init__.py
--rw-r--r--   0        0        0     5041 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/base.py
--rw-r--r--   0        0        0     4180 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/elasticsearch.py
--rw-r--r--   0        0        0     3218 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/factory.py
--rw-r--r--   0        0        0    23007 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/opensearch.py
--rw-r--r--   0        0        0    16512 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/generic_elastic.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/__init__.py
--rw-r--r--   0        0        0     1333 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/datasets.py
--rw-r--r--   0        0        0     7053 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/helpers.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/stopwords/__init__.py
--rw-r--r--   0        0        0     5834 2024-05-30 15:47:37.403383 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/stopwords/english.py
--rw-r--r--   0        0        0     1264 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/text2text.py
--rw-r--r--   0        0        0     1876 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/text_classification.py
--rw-r--r--   0        0        0     2119 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/token_classification.py
--rw-r--r--   0        0        0      865 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/__init__.py
--rw-r--r--   0        0        0     7713 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/base.py
--rw-r--r--   0        0        0     1823 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/commons.py
--rw-r--r--   0        0        0     5242 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/text_classification.py
--rw-r--r--   0        0        0     8377 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/token_classification.py
--rw-r--r--   0        0        0    12654 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/query_helpers.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/search/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/search/model.py
--rw-r--r--   0        0        0    12471 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/backend/search/query_builder.py
--rw-r--r--   0        0        0     7267 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/datasets.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/models/__init__.py
--rw-r--r--   0        0        0     3020 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/models/datasets.py
--rw-r--r--   0        0        0     9683 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/models/records.py
--rw-r--r--   0        0        0     8164 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/daos/records.py
--rw-r--r--   0        0        0     2378 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/database.py
--rw-r--r--   0        0        0     2096 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/enums.py
--rw-r--r--   0        0        0      663 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/errors/__init__.py
--rw-r--r--   0        0        0     5318 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/errors/base_errors.py
--rw-r--r--   0        0        0     3703 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/errors/error_handler.py
--rw-r--r--   0        0        0      642 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/errors/future/__init__.py
--rw-r--r--   0        0        0     1633 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/errors/future/base_errors.py
--rw-r--r--   0        0        0      812 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/errors/task_errors.py
--rw-r--r--   0        0        0     4091 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/helpers.py
--rw-r--r--   0        0        0     2284 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/logging.py
--rw-r--r--   0        0        0      938 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/models/__init__.py
--rw-r--r--   0        0        0     1420 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/models/base.py
--rw-r--r--   0        0        0    18467 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/models/database.py
--rw-r--r--   0        0        0     3178 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/models/metadata_properties.py
--rw-r--r--   0        0        0     6689 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/models/mixins.py
--rw-r--r--   0        0        0      773 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/models/suggestions.py
--rw-r--r--   0        0        0    22732 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/policies.py
--rw-r--r--   0        0        0      905 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      731 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/pydantic_v1/errors.py
--rw-r--r--   0        0        0      735 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/pydantic_v1/generics.py
--rw-r--r--   0        0        0      729 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/pydantic_v1/utils.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/__init__.py
--rw-r--r--   0        0        0     1639 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/base.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v0/__init__.py
--rw-r--r--   0        0        0     1056 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v0/authentication.py
--rw-r--r--   0        0        0     2260 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v0/datasets.py
--rw-r--r--   0        0        0     2207 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v0/users.py
--rw-r--r--   0        0        0     1079 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v0/workspaces.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/__init__.py
--rw-r--r--   0        0        0     2601 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/datasets.py
--rw-r--r--   0        0        0     2414 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/fields.py
--rw-r--r--   0        0        0      786 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/info.py
--rw-r--r--   0        0        0     5522 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/metadata_properties.py
--rw-r--r--   0        0        0      873 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/oauth2.py
--rw-r--r--   0        0        0    11234 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/questions.py
--rw-r--r--   0        0        0    10639 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/records.py
--rw-r--r--   0        0        0     1853 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/records_bulk.py
--rw-r--r--   0        0        0     5862 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/responses.py
--rw-r--r--   0        0        0     1670 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/settings.py
--rw-r--r--   0        0        0     2925 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/suggestions.py
--rw-r--r--   0        0        0     1717 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/users.py
--rw-r--r--   0        0        0     2376 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/vector_settings.py
--rw-r--r--   0        0        0      803 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/vectors.py
--rw-r--r--   0        0        0     1214 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/schemas/v1/workspaces.py
--rw-r--r--   0        0        0      949 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/search_engine/__init__.py
--rw-r--r--   0        0        0     9988 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/search_engine/base.py
--rw-r--r--   0        0        0    34423 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/search_engine/commons.py
--rw-r--r--   0        0        0     5910 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/search_engine/elasticsearch.py
--rw-r--r--   0        0        0     6186 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/search_engine/opensearch.py
--rw-r--r--   0        0        0      687 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/__init__.py
--rw-r--r--   0        0        0      791 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/__init__.py
--rw-r--r--   0        0        0     1338 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/claims.py
--rw-r--r--   0        0        0      810 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/db/__init__.py
--rw-r--r--   0        0        0     1718 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/db/api_key_backend.py
--rw-r--r--   0        0        0     1818 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/db/bearer_token_backend.py
--rw-r--r--   0        0        0     1527 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/jwt.py
--rw-r--r--   0        0        0      764 2024-05-30 15:47:37.407384 argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/__init__.py
--rw-r--r--   0        0        0     1797 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/auth_backend.py
--rw-r--r--   0        0        0     6795 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/client_provider.py
--rw-r--r--   0        0        0     3576 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/settings.py
--rw-r--r--   0        0        0     1873 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/supported_providers.py
--rw-r--r--   0        0        0     2887 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/authentication/provider.py
--rw-r--r--   0        0        0     1288 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/authentication/userinfo.py
--rw-r--r--   0        0        0     2693 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/model.py
--rw-r--r--   0        0        0     2185 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/security/settings.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/server.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/__init__.py
--rw-r--r--   0        0        0    10394 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/datasets.py
--rw-r--r--   0        0        0     2862 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/info.py
--rw-r--r--   0        0        0      702 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/metrics/__init__.py
--rw-r--r--   0        0        0     5036 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/metrics/models.py
--rw-r--r--   0        0        0     4102 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/metrics/service.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/search/__init__.py
--rw-r--r--   0        0        0     2154 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/search/model.py
--rw-r--r--   0        0        0     4929 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/search/service.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/storage/__init__.py
--rw-r--r--   0        0        0     4287 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/storage/service.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/__init__.py
--rw-r--r--   0        0        0      629 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/commons/__init__.py
--rw-r--r--   0        0        0     1284 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/commons/models.py
--rw-r--r--   0        0        0      645 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text2text/__init__.py
--rw-r--r--   0        0        0     2460 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text2text/models.py
--rw-r--r--   0        0        0     4300 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text2text/service.py
--rw-r--r--   0        0        0      654 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/__init__.py
--rw-r--r--   0        0        0     6258 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/metrics.py
--rw-r--r--   0        0        0    10345 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/model.py
--rw-r--r--   0        0        0    13450 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/service.py
--rw-r--r--   0        0        0      655 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/__init__.py
--rw-r--r--   0        0        0    15760 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/metrics.py
--rw-r--r--   0        0        0     6801 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/model.py
--rw-r--r--   0        0        0     5488 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/service.py
--rw-r--r--   0        0        0     8391 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/settings.py
--rw-r--r--   0        0        0        0 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/.nojekyll
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/200.html
--rw-r--r--   0        0        0      435 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/README.md
--rw-r--r--   0        0        0    34042 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/013b2a2.js
--rw-r--r--   0        0        0     8735 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/044f51a.js
--rw-r--r--   0        0        0    14896 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/04ee322.js
--rw-r--r--   0        0        0    18396 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/062aa1b.js
--rw-r--r--   0        0        0    24146 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/067807e.js
--rw-r--r--   0        0        0    33180 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/07d520c.js
--rw-r--r--   0        0        0     5885 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0825c42.js
--rw-r--r--   0        0        0    17327 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0860d7f.js
--rw-r--r--   0        0        0    13877 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0871234.js
--rw-r--r--   0        0        0    36431 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/089e044.js
--rw-r--r--   0        0        0   191172 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0947351.js
--rw-r--r--   0        0        0     2059 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0ddded0.js
--rw-r--r--   0        0        0    18927 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0e81119.js
--rw-r--r--   0        0        0     1305 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/0f97c02.js
--rw-r--r--   0        0        0    15499 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/10080fe.js
--rw-r--r--   0        0        0    38481 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1069132.js
--rw-r--r--   0        0        0    20403 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/118c84b.js
--rw-r--r--   0        0        0      420 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/119484b.js
--rw-r--r--   0        0        0     1297 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1200f05.js
--rw-r--r--   0        0        0    23070 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/14cc7db.js
--rw-r--r--   0        0        0    35679 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/150492b.js
--rw-r--r--   0        0        0     3236 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/17934c0.js
--rw-r--r--   0        0        0    47783 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/17e1412.js
--rw-r--r--   0        0        0    11989 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/180c687.js
--rw-r--r--   0        0        0    10073 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/18218e0.js
--rw-r--r--   0        0        0    73003 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/18ced35.js
--rw-r--r--   0        0        0     5849 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/18d4cfc.js
--rw-r--r--   0        0        0    15509 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/19065ba.js
--rw-r--r--   0        0        0    13465 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/195ef90.js
--rw-r--r--   0        0        0     5772 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/19bc22f.js
--rw-r--r--   0        0        0     7884 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1a8d6cd.js
--rw-r--r--   0        0        0     7819 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1c811c3.js
--rw-r--r--   0        0        0     9390 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1d154db.js
--rw-r--r--   0        0        0     7431 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1daf168.js
--rw-r--r--   0        0        0    13932 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/1e0fecd.js
--rw-r--r--   0        0        0    23778 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/20656e6.js
--rw-r--r--   0        0        0     7610 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/20e2acb.js
--rw-r--r--   0        0        0     9396 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/21af5f2.js
--rw-r--r--   0        0        0    26912 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/236468b.js
--rw-r--r--   0        0        0     7242 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/23d5212.js
--rw-r--r--   0        0        0     2283 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/253fe5d.js
--rw-r--r--   0        0        0    10102 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/25a65ea.js
--rw-r--r--   0        0        0    16084 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/28f0cc4.js
--rw-r--r--   0        0        0    21212 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/293afa8.js
--rw-r--r--   0        0        0     6624 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/2a02714.js
--rw-r--r--   0        0        0     7115 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/2a30bbe.js
--rw-r--r--   0        0        0      603 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/2b4bd32.js
--rw-r--r--   0        0        0    24173 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/2b6a91d.js
--rw-r--r--   0        0        0     8996 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/2bcabcb.js
--rw-r--r--   0        0        0    11010 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/2be230f.js
--rw-r--r--   0        0        0    22686 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/334cf94.js
--rw-r--r--   0        0        0     1270 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/34b0f74.js
--rw-r--r--   0        0        0    26677 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/34fb14a.js
--rw-r--r--   0        0        0     9071 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/35267f4.js
--rw-r--r--   0        0        0    16047 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3589b51.js
--rw-r--r--   0        0        0    13433 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/35c38bb.js
--rw-r--r--   0        0        0    56981 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3660432.js
--rw-r--r--   0        0        0     8689 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/37678ae.js
--rw-r--r--   0        0        0    45970 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/37a8d34.js
--rw-r--r--   0        0        0    18862 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/37e0496.js
--rw-r--r--   0        0        0     8493 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/37f0ed3.js
--rw-r--r--   0        0        0      954 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/38bfa8a.js
--rw-r--r--   0        0        0     9738 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/393e0cb.js
--rw-r--r--   0        0        0    50017 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3ae506d.js
--rw-r--r--   0        0        0    66203 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3b116b7.js
--rw-r--r--   0        0        0     9390 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3d2f697.js
--rw-r--r--   0        0        0    17751 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3e416f9.js
--rw-r--r--   0        0        0  2363254 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/3eb41c4.js
--rw-r--r--   0        0        0     1333 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/41bfc83.js
--rw-r--r--   0        0        0    15176 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4288855.js
--rw-r--r--   0        0        0    57895 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/42e48d6.js
--rw-r--r--   0        0        0    31439 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/431ac92.js
--rw-r--r--   0        0        0     8834 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/433d86e.js
--rw-r--r--   0        0        0     8742 2024-05-30 15:56:09.617513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/44da1fe.js
--rw-r--r--   0        0        0    24734 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/45c5778.js
--rw-r--r--   0        0        0    47287 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/473c94a.js
--rw-r--r--   0        0        0     8598 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/48ab383.js
--rw-r--r--   0        0        0     6545 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/48afbb8.js
--rw-r--r--   0        0        0    18358 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/48bdb55.js
--rw-r--r--   0        0        0    44536 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4943115.js
--rw-r--r--   0        0        0    18793 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/49efda7.js
--rw-r--r--   0        0        0     6746 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4a00879.js
--rw-r--r--   0        0        0   787702 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4a07ba2.js
--rw-r--r--   0        0        0     1632 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4ab08c6.js
--rw-r--r--   0        0        0    18887 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4ab2f0e.js
--rw-r--r--   0        0        0     6202 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4afa49d.js
--rw-r--r--   0        0        0     1270 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4b8c9e5.js
--rw-r--r--   0        0        0     7411 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4cb5088.js
--rw-r--r--   0        0        0     9558 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4d350f9.js
--rw-r--r--   0        0        0    20511 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4d4f708.js
--rw-r--r--   0        0        0    16735 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/4ed7f9b.js
--rw-r--r--   0        0        0     6427 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/50100f8.js
--rw-r--r--   0        0        0    20923 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5048443.js
--rw-r--r--   0        0        0     7938 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5128dee.js
--rw-r--r--   0        0        0    50936 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/516e13f.js
--rw-r--r--   0        0        0     7080 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/517a829.js
--rw-r--r--   0        0        0     5779 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5221f06.js
--rw-r--r--   0        0        0    23693 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/523b8f3.js
--rw-r--r--   0        0        0     1012 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5250978.js
--rw-r--r--   0        0        0    38665 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/52bc438.js
--rw-r--r--   0        0        0     1821 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5313688.js
--rw-r--r--   0        0        0    23973 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/53f6e15.js
--rw-r--r--   0        0        0     7742 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/55ca8de.js
--rw-r--r--   0        0        0     8439 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/56939a1.js
--rw-r--r--   0        0        0    10049 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/56e2001.js
--rw-r--r--   0        0        0      443 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5808988.js
--rw-r--r--   0        0        0      420 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5925665.js
--rw-r--r--   0        0        0   134978 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/59f135b.js
--rw-r--r--   0        0        0    19479 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5bfecac.js
--rw-r--r--   0        0        0    56247 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5c9196c.js
--rw-r--r--   0        0        0    35455 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/5fa1d20.js
--rw-r--r--   0        0        0     1603 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/603a676.js
--rw-r--r--   0        0        0    67976 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/615110d.js
--rw-r--r--   0        0        0     9380 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/62e65e8.js
--rw-r--r--   0        0        0    28588 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/63d8f21.js
--rw-r--r--   0        0        0    38103 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/65cbc28.js
--rw-r--r--   0        0        0    17525 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/67b5ce1.js
--rw-r--r--   0        0        0    22216 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/6a2bb14.js
--rw-r--r--   0        0        0     5977 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/6c3f9c9.js
--rw-r--r--   0        0        0     7377 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/6d2c5ba.js
--rw-r--r--   0        0        0    13915 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/6d6d001.js
--rw-r--r--   0        0        0     6659 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/6d915c8.js
--rw-r--r--   0        0        0     8377 2024-05-30 15:56:09.613513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/6dd33cc.js
--rw-r--r--   0        0        0   329983 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7002aba.js
--rw-r--r--   0        0        0     7460 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/70072c5.js
--rw-r--r--   0        0        0    22275 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7062e38.js
--rw-r--r--   0        0        0     1838 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/70a28c1.js
--rw-r--r--   0        0        0     6508 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/71043f0.js
--rw-r--r--   0        0        0    36399 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/711e9f4.js
--rw-r--r--   0        0        0    47944 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/71861c4.js
--rw-r--r--   0        0        0   184996 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/719d89c.js
--rw-r--r--   0        0        0    14033 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/71bff6b.js
--rw-r--r--   0        0        0    32394 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/71f1583.js
--rw-r--r--   0        0        0    17297 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/722387e.js
--rw-r--r--   0        0        0     8931 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7304342.js
--rw-r--r--   0        0        0     9329 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7308f13.js
--rw-r--r--   0        0        0     6979 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/755499f.js
--rw-r--r--   0        0        0    27264 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/76e0837.js
--rw-r--r--   0        0        0     1750 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/77d5c4e.js
--rw-r--r--   0        0        0    20692 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7810ab7.js
--rw-r--r--   0        0        0     7687 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/783d220.js
--rw-r--r--   0        0        0   164308 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/791a0d6.js
--rw-r--r--   0        0        0     6263 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/79287e2.js
--rw-r--r--   0        0        0    32328 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7a8b85c.js
--rw-r--r--   0        0        0     9524 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7aea98f.js
--rw-r--r--   0        0        0     6694 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7b71301.js
--rw-r--r--   0        0        0     6772 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7bda7b2.js
--rw-r--r--   0        0        0     9925 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7c86bca.js
--rw-r--r--   0        0        0     6029 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7d19bec.js
--rw-r--r--   0        0        0    12448 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7d95f80.js
--rw-r--r--   0        0        0     6608 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7e2d35c.js
--rw-r--r--   0        0        0     7373 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7f014bb.js
--rw-r--r--   0        0        0    35020 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/7f50bb1.js
--rw-r--r--   0        0        0     6843 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/811f3aa.js
--rw-r--r--   0        0        0     8481 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/82243c9.js
--rw-r--r--   0        0        0     1897 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/827fbc3.js
--rw-r--r--   0        0        0     1821 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/859e3a2.js
--rw-r--r--   0        0        0    32804 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/86a6498.js
--rw-r--r--   0        0        0   104201 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8753b79.js
--rw-r--r--   0        0        0     8668 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8a2c5a2.js
--rw-r--r--   0        0        0    31603 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8a9dc00.js
--rw-r--r--   0        0        0     5615 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8ac6918.js
--rw-r--r--   0        0        0     6998 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8b30d40.js
--rw-r--r--   0        0        0    16186 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8c85121.js
--rw-r--r--   0        0        0    79820 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8debb26.js
--rw-r--r--   0        0        0    15255 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/8f61c54.js
--rw-r--r--   0        0        0    15344 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9060868.js
--rw-r--r--   0        0        0     6780 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9133688.js
--rw-r--r--   0        0        0    35459 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/913ad1e.js
--rw-r--r--   0        0        0    21968 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/919299c.js
--rw-r--r--   0        0        0    39034 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/923d2e5.js
--rw-r--r--   0        0        0    11589 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/938a825.js
--rw-r--r--   0        0        0    16614 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/93ff988.js
--rw-r--r--   0        0        0    22290 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/949e7ce.js
--rw-r--r--   0        0        0     3888 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/95ab122.js
--rw-r--r--   0        0        0     5701 2024-05-30 15:56:09.609513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/95db8b3.js
--rw-r--r--   0        0        0    26510 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/961efe0.js
--rw-r--r--   0        0        0     8339 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9651160.js
--rw-r--r--   0        0        0     8169 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/96c3974.js
--rw-r--r--   0        0        0     1919 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/97cdc40.js
--rw-r--r--   0        0        0     9992 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/980752a.js
--rw-r--r--   0        0        0    41531 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/98b724f.js
--rw-r--r--   0        0        0     7772 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9959e1c.js
--rw-r--r--   0        0        0     8030 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9a6c8ed.js
--rw-r--r--   0        0        0     1921 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9b4233d.js
--rw-r--r--   0        0        0     7384 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9c2eddf.js
--rw-r--r--   0        0        0    36636 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9c66ec1.js
--rw-r--r--   0        0        0    25826 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9d7b714.js
--rw-r--r--   0        0        0     1049 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9d8ec11.js
--rw-r--r--   0        0        0     9590 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9dc9c16.js
--rw-r--r--   0        0        0     5986 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/9fb2cd3.js
--rw-r--r--   0        0        0     1726 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/LICENSES
--rw-r--r--   0        0        0     3282 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a0a7333.js
--rw-r--r--   0        0        0    63778 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a128d0a.js
--rw-r--r--   0        0        0    24710 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a233280.js
--rw-r--r--   0        0        0     8209 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a4051d7.js
--rw-r--r--   0        0        0    34002 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a61d3e4.js
--rw-r--r--   0        0        0    16602 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a63bfb6.js
--rw-r--r--   0        0        0    16740 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a757343.js
--rw-r--r--   0        0        0    25622 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a8ae09e.js
--rw-r--r--   0        0        0    33881 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a97c5b4.js
--rw-r--r--   0        0        0    64350 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/a99f76b.js
--rw-r--r--   0        0        0   421296 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/aa2a6d6.js
--rw-r--r--   0        0        0     1306 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/aa2b049.js
--rw-r--r--   0        0        0     9828 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/ad412fa.js
--rw-r--r--   0        0        0    23279 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/ade1835.js
--rw-r--r--   0        0        0     6789 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/af2be6c.js
--rw-r--r--   0        0        0   420673 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b1c7a5f.js
--rw-r--r--   0        0        0      420 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b1feae4.js
--rw-r--r--   0        0        0      931 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b21e71c.js
--rw-r--r--   0        0        0     9031 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b28cfbc.js
--rw-r--r--   0        0        0     1009 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b2f22c5.js
--rw-r--r--   0        0        0    25066 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b2fc075.js
--rw-r--r--   0        0        0   558191 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b4c1d0d.js
--rw-r--r--   0        0        0      482 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b4f53d2.js
--rw-r--r--   0        0        0    40322 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b53ca3b.js
--rw-r--r--   0        0        0     1205 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b5b4aae.js
--rw-r--r--   0        0        0   590941 2024-05-30 15:56:09.605513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b6ffaa9.js
--rw-r--r--   0        0        0     1260 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b781657.js
--rw-r--r--   0        0        0     1415 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b804ce5.js
--rw-r--r--   0        0        0    11573 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b8c421d.js
--rw-r--r--   0        0        0     1207 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/b955150.js
--rw-r--r--   0        0        0    28137 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bad085e.js
--rw-r--r--   0        0        0    28039 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bad26d7.js
--rw-r--r--   0        0        0    52299 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bd7cb12.js
--rw-r--r--   0        0        0     4508 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bdf5c09.js
--rw-r--r--   0        0        0     5403 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/beccc06.js
--rw-r--r--   0        0        0    35550 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bedb2dd.js
--rw-r--r--   0        0        0    19503 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bef1a27.js
--rw-r--r--   0        0        0    17968 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/bf6bced.js
--rw-r--r--   0        0        0      603 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c02ad86.js
--rw-r--r--   0        0        0     8439 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c26b3ec.js
--rw-r--r--   0        0        0    20780 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c380661.js
--rw-r--r--   0        0        0    39831 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c5ba452.js
--rw-r--r--   0        0        0      954 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c5dda82.js
--rw-r--r--   0        0        0     6284 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c606e8c.js
--rw-r--r--   0        0        0     8622 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c615699.js
--rw-r--r--   0        0        0     1472 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c72e4ee.js
--rw-r--r--   0        0        0     7961 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c863a84.js
--rw-r--r--   0        0        0    17385 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/c9f74e7.js
--rw-r--r--   0        0        0    23243 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/ca0d950.js
--rw-r--r--   0        0        0    56678 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cba5c90.js
--rw-r--r--   0        0        0     7474 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cc5cbbe.js
--rw-r--r--   0        0        0     8089 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cd3d6f6.js
--rw-r--r--   0        0        0     5871 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cd61b37.js
--rw-r--r--   0        0        0    68986 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cdeab7c.js
--rw-r--r--   0        0        0   624339 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cf435aa.js
--rw-r--r--   0        0        0    36311 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/cf5d4e8.js
--rw-r--r--   0        0        0   377557 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d3b25ba.js
--rw-r--r--   0        0        0    23720 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d3ec09a.js
--rw-r--r--   0        0        0   329438 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d6044c6.js
--rw-r--r--   0        0        0      603 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d8454ea.js
--rw-r--r--   0        0        0    23669 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d8c7cdd.js
--rw-r--r--   0        0        0     8996 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d95f66b.js
--rw-r--r--   0        0        0     8932 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/d9f709f.js
--rw-r--r--   0        0        0    13915 2024-05-30 15:56:09.601513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/da56dc9.js
--rw-r--r--   0        0        0    41490 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/da98642.js
--rw-r--r--   0        0        0   138125 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/dae7b34.js
--rw-r--r--   0        0        0     3066 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/de51b34.js
--rw-r--r--   0        0        0     5835 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/df05a2c.js
--rw-r--r--   0        0        0     8332 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/df0702e.js
--rw-r--r--   0        0        0    18956 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/dfb4e3d.js
--rw-r--r--   0        0        0    14414 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e1fa0db.js
--rw-r--r--   0        0        0    25241 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e208f0f.js
--rw-r--r--   0        0        0    25259 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e23db67.js
--rw-r--r--   0        0        0    54826 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e2678f8.js
--rw-r--r--   0        0        0      560 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e311004.js
--rw-r--r--   0        0        0    46483 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e31b663.js
--rw-r--r--   0        0        0    23279 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e3fe598.js
--rw-r--r--   0        0        0    15135 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e44b050.js
--rw-r--r--   0        0        0    22723 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e4c5fa4.js
--rw-r--r--   0        0        0     8487 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e4cf190.js
--rw-r--r--   0        0        0    33699 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e4f9f5b.js
--rw-r--r--   0        0        0     5670 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e63dbd4.js
--rw-r--r--   0        0        0     9319 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e7035e6.js
--rw-r--r--   0        0        0    68469 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e79118e.js
--rw-r--r--   0        0        0    16063 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e79cf5b.js
--rw-r--r--   0        0        0     8394 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e7e5f43.js
--rw-r--r--   0        0        0    18287 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e8142c4.js
--rw-r--r--   0        0        0   119788 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e8e19b2.js
--rw-r--r--   0        0        0     2284 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/e901328.js
--rw-r--r--   0        0        0    10082 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/ea525f4.js
--rw-r--r--   0        0        0     5982 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/eb1faf3.js
--rw-r--r--   0        0        0     7276 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/edd702e.js
--rw-r--r--   0        0        0    24471 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/efe6a6f.js
--rw-r--r--   0        0        0     7593 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f03fccb.js
--rw-r--r--   0        0        0    18228 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f0a6dd7.js
--rw-r--r--   0        0        0     6115 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f14f26d.js
--rw-r--r--   0        0        0   329973 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f217920.js
--rw-r--r--   0        0        0      289 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f2cf071.js
--rw-r--r--   0        0        0     5853 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f36addc.js
--rw-r--r--   0        0        0    36070 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f3b5d22.js
--rw-r--r--   0        0        0    14514 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f3eb9f7.js
--rw-r--r--   0        0        0     7613 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f3f39b2.js
--rw-r--r--   0        0        0    25350 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f409abc.js
--rw-r--r--   0        0        0    17834 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f41b1df.js
--rw-r--r--   0        0        0     9321 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f66f192.js
--rw-r--r--   0        0        0    11382 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f6c0467.js
--rw-r--r--   0        0        0    29182 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f7afca5.js
--rw-r--r--   0        0        0    33119 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f86ebc2.js
--rw-r--r--   0        0        0     9004 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/f947aa0.js
--rw-r--r--   0        0        0     8504 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fa7f8a6.js
--rw-r--r--   0        0        0     7481 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fa9e6f9.js
--rw-r--r--   0        0        0     1507 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fd39885.js
--rw-r--r--   0        0        0    14475 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fd59c1c.js
--rw-r--r--   0        0        0    86840 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fd65964.js
--rw-r--r--   0        0        0     7158 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fdf390c.js
--rw-r--r--   0        0        0    25130 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fe8b19e.js
--rw-r--r--   0        0        0    13339 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fec21cc.js
--rw-r--r--   0        0        0    67510 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fefbfff.js
--rw-r--r--   0        0        0    28116 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.3c074ae.woff2
--rw-r--r--   0        0        0    36012 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.f7cfb4c.woff
--rw-r--r--   0        0        0     5814 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/apple-touch-icon.png
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/datasets/index.html
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/datasets/useDatasetsViewModel/index.html
--rw-r--r--   0        0        0     1048 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/favicon-16x16.png
--rw-r--r--   0        0        0     1139 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/favicon.ico
--rw-r--r--   0        0        0      263 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/icons/arrow-down.svg
--rw-r--r--   0        0        0      278 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/icons/arrow-up.svg
--rw-r--r--   0        0        0     1134 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/icons/bulk-mode.svg
--rw-r--r--   0        0        0     1743 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/icons/change-height.svg
--rw-r--r--   0        0        0      201 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/icons/check.svg
--rw-r--r--   0        0        0      199 2024-05-30 15:56:09.597513 argilla_server-1.29.0/src/argilla_server/static/icons/chevron-down.svg
--rw-r--r--   0        0        0      187 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/chevron-left.svg
--rw-r--r--   0        0        0      183 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/chevron-right.svg
--rw-r--r--   0        0        0      199 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/chevron-up.svg
--rw-r--r--   0        0        0      761 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/clear.svg
--rw-r--r--   0        0        0      638 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/close.svg
--rw-r--r--   0        0        0      518 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/code.svg
--rw-r--r--   0        0        0      353 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/copy.svg
--rw-r--r--   0        0        0     2408 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/danger.svg
--rw-r--r--   0        0        0      637 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/discard.svg
--rw-r--r--   0        0        0     1372 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/draggable.svg
--rw-r--r--   0        0        0      375 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/expand-arrows.svg
--rw-r--r--   0        0        0      956 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/exploration.svg
--rw-r--r--   0        0        0      350 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/external-link.svg
--rw-r--r--   0        0        0      364 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/external.svg
--rw-r--r--   0        0        0      590 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/filter.svg
--rw-r--r--   0        0        0      382 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/focus-mode.svg
--rw-r--r--   0        0        0      643 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/hand-labeling.svg
--rw-r--r--   0        0        0      835 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/info.svg
--rw-r--r--   0        0        0      685 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/kebab.svg
--rw-r--r--   0        0        0     1021 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/link.svg
--rw-r--r--   0        0        0      548 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/log-out.svg
--rw-r--r--   0        0        0      595 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/matching.svg
--rwxr-xr-x   0        0        0      487 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/math-plus.svg
--rw-r--r--   0        0        0      585 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/meatballs.svg
--rw-r--r--   0        0        0      465 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/minimize-arrows.svg
--rw-r--r--   0        0        0     1010 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/no-matching.svg
--rw-r--r--   0        0        0      816 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/pen.svg
--rw-r--r--   0        0        0      651 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/progress.svg
--rw-r--r--   0        0        0      526 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/refresh.svg
--rw-r--r--   0        0        0      568 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/reset.svg
--rw-r--r--   0        0        0      800 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/row-last.svg
--rw-r--r--   0        0        0      805 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/search.svg
--rw-r--r--   0        0        0     4510 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/settings.svg
--rw-r--r--   0        0        0      977 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/shortcuts.svg
--rw-r--r--   0        0        0     1668 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/similarity.svg
--rw-r--r--   0        0        0      888 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/smile-sad.svg
--rw-r--r--   0        0        0      354 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/sort.svg
--rw-r--r--   0        0        0      260 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/stats.svg
--rw-r--r--   0        0        0     1131 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/suggestion.svg
--rw-r--r--   0        0        0     2187 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/support.svg
--rw-r--r--   0        0        0      451 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/time.svg
--rw-r--r--   0        0        0      809 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/trash-empty.svg
--rw-r--r--   0        0        0      630 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/unavailable.svg
--rw-r--r--   0        0        0      647 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/validate.svg
--rw-r--r--   0        0        0     1233 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/icons/weak-labeling.svg
--rw-r--r--   0        0        0    29161 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/images/help-info/explain.png
--rw-r--r--   0        0        0   121622 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/images/help-info/similarity.png
--rw-r--r--   0        0        0     3554 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/images/logo.svg
--rw-r--r--   0        0        0   346289 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/images/welcome-hf-sign-in-ss.png
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/index.html
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/sign-in/index.html
--rw-r--r--   0        0        0      426 2024-05-30 15:56:09.593513 argilla_server-1.29.0/src/argilla_server/static/site.webmanifest
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/useWelcomeHFViewModel/index.html
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/user-settings/index.html
--rw-r--r--   0        0        0     3626 2024-05-30 15:56:09.621513 argilla_server-1.29.0/src/argilla_server/static/welcome-hf-sign-in/index.html
--rw-r--r--   0        0        0     1618 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/static_rewrite.py
--rw-r--r--   0        0        0     4550 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/telemetry.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/use_cases/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/use_cases/responses/__init__.py
--rw-r--r--   0        0        0     2655 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/use_cases/responses/upsert_responses_in_bulk.py
--rw-r--r--   0        0        0     6793 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils.py
--rw-r--r--   0        0        0      730 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils/__init__.py
--rw-r--r--   0        0        0     2973 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils/_telemetry.py
--rw-r--r--   0        0        0     7709 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils/dependency.py
--rw-r--r--   0        0        0     6788 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils/params.py
--rw-r--r--   0        0        0     8486 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils/span_utils.py
--rw-r--r--   0        0        0     1377 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/utils/utils.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/__init__.py
--rw-r--r--   0        0        0     6378 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/questions.py
--rw-r--r--   0        0        0     7169 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/records.py
--rw-r--r--   0        0        0    12940 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/response_values.py
--rw-r--r--   0        0        0     3436 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/responses.py
--rw-r--r--   0        0        0     2513 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/suggestions.py
--rw-r--r--   0        0        0     1115 2024-05-30 15:47:37.411383 argilla_server-1.29.0/src/argilla_server/validators/vectors.py
--rw-r--r--   0        0        0     1116 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/__init__.py
--rw-r--r--   0        0        0     3523 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/conftest.py
--rw-r--r--   0        0        0     1106 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/database.py
--rw-r--r--   0        0        0    12180 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/factories.py
--rw-r--r--   0        0        0      906 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      735 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/pydantic_v1/generics.py
--rw-r--r--   0        0        0      729 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/pydantic_v1/utils.py
--rw-r--r--   0        0        0      622 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/test_docs.py
--rw-r--r--   0        0        0     1163 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/test_not_found_routes.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/v0/__init__.py
--rw-r--r--   0        0        0     1468 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/v0/test_authentication.py
--rw-r--r--   0        0        0    19094 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/v0/test_datasets.py
--rw-r--r--   0        0        0     2434 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/v0/test_info.py
--rw-r--r--   0        0        0    14083 2024-05-30 15:47:37.411383 argilla_server-1.29.0/tests/unit/api/v0/test_metrics.py
--rw-r--r--   0        0        0     5360 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_records_get.py
--rw-r--r--   0        0        0     9023 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_records_update.py
--rw-r--r--   0        0        0     2152 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_security_token.py
--rw-r--r--   0        0        0     9256 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_text2text.py
--rw-r--r--   0        0        0    34224 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_text_classification.py
--rw-r--r--   0        0        0    23182 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_text_classification_api_rules.py
--rw-r--r--   0        0        0    11094 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_text_classification_dataset_settings.py
--rw-r--r--   0        0        0    23310 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_token_classification.py
--rw-r--r--   0        0        0     7388 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_token_classification_dataset_settings.py
--rw-r--r--   0        0        0    16140 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_users.py
--rw-r--r--   0        0        0    15316 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v0/test_workspaces.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/authentication/__init__.py
--rw-r--r--   0        0        0     2035 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/authentication/test_create_token.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/questions/__init__.py
--rw-r--r--   0        0        0     6250 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/questions/test_create_dataset_question.py
--rw-r--r--   0        0        0     2581 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/questions/test_list_dataset_questions.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/__init__.py
--rw-r--r--   0        0        0     6715 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk.py
--rw-r--r--   0        0        0    14466 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_responses.py
--rw-r--r--   0        0        0    16789 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_suggestions.py
--rw-r--r--   0        0        0    13736 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_vectors.py
--rw-r--r--   0        0        0     9277 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/test_create_dataset_records.py
--rw-r--r--   0        0        0     7436 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/records/test_update_dataset_records.py
--rw-r--r--   0        0        0     7690 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_create_dataset_question.py
--rw-r--r--   0        0        0     1778 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_create_dataset_vector_settings.py
--rw-r--r--   0        0        0     7550 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_get_dataset_progress.py
--rw-r--r--   0        0        0     7099 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_list_dataset_records_search_suggestions_options.py
--rw-r--r--   0        0        0    24808 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_questions.py
--rw-r--r--   0        0        0    10220 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_search_current_user_dataset_records.py
--rw-r--r--   0        0        0    15677 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/datasets/test_search_dataset_records.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/info/__init__.py
--rw-r--r--   0        0        0     1288 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/info/test_get_status.py
--rw-r--r--   0        0        0     1026 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/info/test_get_version.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/questions/__init__.py
--rw-r--r--   0        0        0    10670 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/questions/test_update_question.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/records/__init__.py
--rw-r--r--   0        0        0    17476 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/records/test_create_record_response.py
--rw-r--r--   0        0        0    27129 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/records/test_upsert_suggestion.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/responses/__init__.py
--rw-r--r--   0        0        0    16388 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/responses/test_create_current_user_responses_bulk.py
--rw-r--r--   0        0        0    19671 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/responses/test_update_response.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/settings/__init__.py
--rw-r--r--   0        0        0     3926 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/settings/test_get_settings.py
--rw-r--r--   0        0        0   210934 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/test_datasets.py
--rw-r--r--   0        0        0     8602 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/test_fields.py
--rw-r--r--   0        0        0    66065 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/test_list_dataset_records.py
--rw-r--r--   0        0        0    17388 2024-05-30 15:47:37.415383 argilla_server-1.29.0/tests/unit/api/v1/test_metadata_properties.py
--rw-r--r--   0        0        0    13387 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_oauth2.py
--rw-r--r--   0        0        0    21205 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_questions.py
--rw-r--r--   0        0        0    63240 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_records.py
--rw-r--r--   0        0        0    18407 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_responses.py
--rw-r--r--   0        0        0     3533 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_suggestions.py
--rw-r--r--   0        0        0     3348 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_users.py
--rw-r--r--   0        0        0     6885 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_vectors_settings.py
--rw-r--r--   0        0        0     7867 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/test_workspaces.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/users/__init__.py
--rw-r--r--   0        0        0    10802 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/users/test_create_user.py
--rw-r--r--   0        0        0     3177 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/users/test_delete_user.py
--rw-r--r--   0        0        0     1608 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/users/test_get_current_user.py
--rw-r--r--   0        0        0     2618 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/users/test_get_user.py
--rw-r--r--   0        0        0     3225 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/users/test_list_users.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/workspaces/__init__.py
--rw-r--r--   0        0        0     4166 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_create_workspace.py
--rw-r--r--   0        0        0     5420 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_create_workspace_user.py
--rw-r--r--   0        0        0     6310 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_delete_workspace_user.py
--rw-r--r--   0        0        0     5479 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_list_workspace_users.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0      875 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/conftest.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/__init__.py
--rw-r--r--   0        0        0     1330 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/conftest.py
--rw-r--r--   0        0        0     9387 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_create.py
--rw-r--r--   0        0        0     3595 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_create_default.py
--rw-r--r--   0        0        0     6328 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_migrate.py
--rw-r--r--   0        0        0     2626 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_update.py
--rw-r--r--   0        0        0     1207 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_user_files/users.yml
--rw-r--r--   0        0        0      252 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_user_files/users_invalid_user.yml
--rw-r--r--   0        0        0      257 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_user_files/users_invalid_workspace.yml
--rw-r--r--   0        0        0      240 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/database/users/test_user_files/users_one.yml
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/search_engine/__init__.py
--rw-r--r--   0        0        0      966 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/search_engine/conftest.py
--rw-r--r--   0        0        0     1466 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/search_engine/test_reindex.py
--rw-r--r--   0        0        0     1152 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/cli/test_start.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/commons/__init__.py
--rw-r--r--   0        0        0     1311 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/commons/test_records_dao.py
--rw-r--r--   0        0        0     2708 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/commons/test_settings.py
--rw-r--r--   0        0        0     2652 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/commons/test_telemetry.py
--rw-r--r--   0        0        0     4670 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/conftest.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/contexts/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/contexts/search/__init__.py
--rw-r--r--   0        0        0     9910 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/contexts/search/test_search_records_query_validator.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/backend/__init__.py
--rw-r--r--   0        0        0     1535 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/backend/test_es_client.py
--rw-r--r--   0        0        0     4141 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/backend/test_generic_elastic_engine.py
--rw-r--r--   0        0        0     3477 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/backend/test_query_builder.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/models/__init__.py
--rw-r--r--   0        0        0     1918 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/models/test_records.py
--rw-r--r--   0        0        0     3078 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/daos/test_datasets.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/errors/__init__.py
--rw-r--r--   0        0        0     2682 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/errors/test_api_errors.py
--rw-r--r--   0        0        0      870 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/errors/test_errors.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/old_models/__init__.py
--rw-r--r--   0        0        0     3246 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/old_models/test_datasets.py
--rw-r--r--   0        0        0     4175 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/old_models/test_text2text.py
--rw-r--r--   0        0        0    12876 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/old_models/test_text_classification.py
--rw-r--r--   0        0        0    11021 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/old_models/test_token_classification.py
--rw-r--r--   0        0        0     7785 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/models/test_base.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/schemas/__init__.py
--rw-r--r--   0        0        0      974 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/schemas/test_base.py
--rw-r--r--   0        0        0     2914 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/schemas/v1/responses/test_response_value_create.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/search_engine/__init__.py
--rw-r--r--   0        0        0     1719 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/search_engine/conftest.py
--rw-r--r--   0        0        0    56309 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/search_engine/test_commons.py
--rw-r--r--   0        0        0     2658 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/search_engine/test_elastisearch.py
--rw-r--r--   0        0        0     3370 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/search_engine/test_opensearch.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/security/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.419383 argilla_server-1.29.0/tests/unit/security/authentication/__init__.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/security/authentication/oauth2/__init__.py
--rw-r--r--   0        0        0     2437 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/security/authentication/oauth2/test_settings.py
--rw-r--r--   0        0        0     3250 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/security/test_model.py
--rw-r--r--   0        0        0     1872 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/security/test_settings.py
--rw-r--r--   0        0        0     1608 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/test_app.py
--rw-r--r--   0        0        0     2180 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/test_logging.py
--rw-r--r--   0        0        0     4008 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/test_utils.py
--rw-r--r--   0        0        0      622 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     5140 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/utils/test_dependency.py
--rw-r--r--   0        0        0     5538 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/utils/test_span_utils.py
--rw-r--r--   0        0        0      606 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/validators/__init__.py
--rw-r--r--   0        0        0     5336 2024-05-30 15:47:37.423383 argilla_server-1.29.0/tests/unit/validators/test_records_bulk.py
--rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 argilla_server-1.29.0/PKG-INFO
+-rw-r--r--   0        0        0     2974 2024-05-30 14:20:53.681105 argilla_server-1.29.0rc1/README.md
+-rw-r--r--   0        0        0     3927 2024-05-30 14:29:59.549717 argilla_server-1.29.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      907 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/__main__.py
+-rw-r--r--   0        0        0     8482 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/_app.py
+-rw-r--r--   0        0        0      843 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/_messages.py
+-rw-r--r--   0        0        0      649 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/_version.py
+-rw-r--r--   0        0        0     3206 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic.ini
+-rw-r--r--   0        0        0     2986 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/env.py
+-rw-r--r--   0        0        0      510 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/script.py.mako
+-rw-r--r--   0        0        0     1589 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/1769ee58fbb4_create_workspaces_users_table.py
+-rw-r--r--   0        0        0     1225 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/1e629a913727_fix_suggestions_type_enum_values.py
+-rw-r--r--   0        0        0     1777 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/3a8e2f9b5dea_create_questions_table.py
+-rw-r--r--   0        0        0     2891 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/3fc3c0839959_create_suggestions_table.py
+-rw-r--r--   0        0        0     1290 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/3ff6484f8b37_add_record_metadata_column.py
+-rw-r--r--   0        0        0     1578 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/74694870197c_create_users_table.py
+-rw-r--r--   0        0        0     2280 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/7850ab5b42d9_create_vectors_settings_table.py
+-rw-r--r--   0        0        0     2394 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/7cbcccf8b57a_create_metadata_properties_table.py
+-rw-r--r--   0        0        0     1302 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/82a5a88a3fa5_create_workspaces_table.py
+-rw-r--r--   0        0        0     1513 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/84f6b9ff6076_add_last_activity_at_to_datasets_table.py
+-rw-r--r--   0        0        0     1544 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/8be56284dac0_create_records_table.py
+-rw-r--r--   0        0        0     2750 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/8c574ada5e5f_update_enum_columns.py
+-rw-r--r--   0        0        0     1722 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/ae5522b4c674_create_fields_table.py
+-rw-r--r--   0        0        0     1388 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/b8458008b60e_add_allow_extra_metadata_column_to_.py
+-rw-r--r--   0        0        0     1629 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/b9099dc08489_create_datasets_table.py
+-rw-r--r--   0        0        0     2285 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/bda6fe24314e_create_vectors_table.py
+-rw-r--r--   0        0        0     2583 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/ca7293c38970_change_suggestions_score_column_to_json.py
+-rw-r--r--   0        0        0     1634 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/e402e9d9245e_create_responses_table.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/errors/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/errors/v1/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/errors/v1/exception_handlers.py
+-rw-r--r--   0        0        0     4134 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/routes.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/__init__.py
+-rw-r--r--   0        0        0     1571 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/authentication.py
+-rw-r--r--   0        0        0     6008 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/datasets.py
+-rw-r--r--   0        0        0     1205 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/info.py
+-rw-r--r--   0        0        0     4616 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/metrics.py
+-rw-r--r--   0        0        0     3975 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/records.py
+-rw-r--r--   0        0        0     4565 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/records_search.py
+-rw-r--r--   0        0        0     3057 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/records_update.py
+-rw-r--r--   0        0        0     4790 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/text2text.py
+-rw-r--r--   0        0        0    14645 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/text_classification.py
+-rw-r--r--   0        0        0     5584 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/text_classification_dataset_settings.py
+-rw-r--r--   0        0        0     5674 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/token_classification.py
+-rw-r--r--   0        0        0     5588 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/token_classification_dataset_settings.py
+-rw-r--r--   0        0        0     4442 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/users.py
+-rw-r--r--   0        0        0     4388 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/workspaces.py
+-rw-r--r--   0        0        0     1710 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/helpers.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.685104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/commons/__init__.py
+-rw-r--r--   0        0        0     1907 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/commons/model.py
+-rw-r--r--   0        0        0     2163 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/commons/params.py
+-rw-r--r--   0        0        0     2046 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/dataset_settings.py
+-rw-r--r--   0        0        0     2637 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/text2text.py
+-rw-r--r--   0        0        0     5074 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/text_classification.py
+-rw-r--r--   0        0        0     3191 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/token_classification.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/__init__.py
+-rw-r--r--   0        0        0      974 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/commons.py
+-rw-r--r--   0        0        0     4343 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/text_classification.py
+-rw-r--r--   0        0        0     4216 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/token_classification.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/__init__.py
+-rw-r--r--   0        0        0     1407 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/authentication.py
+-rw-r--r--   0        0        0     1198 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/__init__.py
+-rw-r--r--   0        0        0    14798 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/datasets.py
+-rw-r--r--   0        0        0     2996 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/questions.py
+-rw-r--r--   0        0        0    27687 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/records.py
+-rw-r--r--   0        0        0     3866 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/records_bulk.py
+-rw-r--r--   0        0        0     2918 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/fields.py
+-rw-r--r--   0        0        0     1261 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/info.py
+-rw-r--r--   0        0        0     3744 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/metadata_properties.py
+-rw-r--r--   0        0        0     4109 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/oauth2.py
+-rw-r--r--   0        0        0     3069 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/questions.py
+-rw-r--r--   0        0        0     8457 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/records.py
+-rw-r--r--   0        0        0     3806 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/responses.py
+-rw-r--r--   0        0        0      925 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/settings.py
+-rw-r--r--   0        0        0     2219 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/suggestions.py
+-rw-r--r--   0        0        0     4271 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/users.py
+-rw-r--r--   0        0        0     2706 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/vectors_settings.py
+-rw-r--r--   0        0        0     7027 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/workspaces.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/bulk/__init__.py
+-rw-r--r--   0        0        0    10789 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/bulk/records_bulk.py
+-rw-r--r--   0        0        0      671 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/__main__.py
+-rw-r--r--   0        0        0      671 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/__init__.py
+-rw-r--r--   0        0        0     1045 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/__main__.py
+-rw-r--r--   0        0        0     1760 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/migrate.py
+-rw-r--r--   0        0        0     1388 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/revisions.py
+-rw-r--r--   0        0        0      671 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/__main__.py
+-rw-r--r--   0        0        0     5357 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/create.py
+-rw-r--r--   0        0        0     2390 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/create_default.py
+-rw-r--r--   0        0        0     4101 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/migrate.py
+-rw-r--r--   0        0        0     1890 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/update.py
+-rw-r--r--   0        0        0     1064 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/utils.py
+-rw-r--r--   0        0        0     1058 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/database/utils.py
+-rw-r--r--   0        0        0     1386 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/rich.py
+-rw-r--r--   0        0        0      671 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/search_engine/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/search_engine/__main__.py
+-rw-r--r--   0        0        0     6068 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/search_engine/reindex.py
+-rw-r--r--   0        0        0     1087 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/start.py
+-rw-r--r--   0        0        0     2488 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/cli/typer_ext.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/commons/__init__.py
+-rw-r--r--   0        0        0     3685 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/commons/config.py
+-rw-r--r--   0        0        0      999 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/commons/models.py
+-rw-r--r--   0        0        0     1203 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/constants.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/__init__.py
+-rw-r--r--   0        0        0     8275 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/accounts.py
+-rw-r--r--   0        0        0    43287 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/datasets.py
+-rw-r--r--   0        0        0     1441 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/info.py
+-rw-r--r--   0        0        0     3151 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/questions.py
+-rw-r--r--   0        0        0     2320 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/records.py
+-rw-r--r--   0        0        0     5200 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/search.py
+-rw-r--r--   0        0        0     1459 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/contexts/settings.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/daos/__init__.py
+-rw-r--r--   0        0        0      694 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/__init__.py
+-rw-r--r--   0        0        0     3625 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/base.py
+-rw-r--r--   0        0        0      728 2024-05-30 14:20:53.689104 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/__init__.py
+-rw-r--r--   0        0        0     5041 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/base.py
+-rw-r--r--   0        0        0     4180 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/elasticsearch.py
+-rw-r--r--   0        0        0     3218 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/factory.py
+-rw-r--r--   0        0        0    23007 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/opensearch.py
+-rw-r--r--   0        0        0    16512 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/generic_elastic.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/__init__.py
+-rw-r--r--   0        0        0     1333 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/datasets.py
+-rw-r--r--   0        0        0     7053 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/helpers.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/stopwords/__init__.py
+-rw-r--r--   0        0        0     5834 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/stopwords/english.py
+-rw-r--r--   0        0        0     1264 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/text2text.py
+-rw-r--r--   0        0        0     1876 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/text_classification.py
+-rw-r--r--   0        0        0     2119 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/token_classification.py
+-rw-r--r--   0        0        0      865 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/__init__.py
+-rw-r--r--   0        0        0     7713 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/base.py
+-rw-r--r--   0        0        0     1823 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/commons.py
+-rw-r--r--   0        0        0     5242 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/text_classification.py
+-rw-r--r--   0        0        0     8377 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/token_classification.py
+-rw-r--r--   0        0        0    12654 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/query_helpers.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/search/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/search/model.py
+-rw-r--r--   0        0        0    12471 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/backend/search/query_builder.py
+-rw-r--r--   0        0        0     7267 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/datasets.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/models/__init__.py
+-rw-r--r--   0        0        0     3020 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/models/datasets.py
+-rw-r--r--   0        0        0     9683 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/models/records.py
+-rw-r--r--   0        0        0     8164 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/daos/records.py
+-rw-r--r--   0        0        0     2378 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/database.py
+-rw-r--r--   0        0        0     2096 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/enums.py
+-rw-r--r--   0        0        0      663 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/errors/__init__.py
+-rw-r--r--   0        0        0     5318 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/errors/base_errors.py
+-rw-r--r--   0        0        0     3703 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/errors/error_handler.py
+-rw-r--r--   0        0        0      642 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/errors/future/__init__.py
+-rw-r--r--   0        0        0     1633 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/errors/future/base_errors.py
+-rw-r--r--   0        0        0      812 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/errors/task_errors.py
+-rw-r--r--   0        0        0     4091 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/helpers.py
+-rw-r--r--   0        0        0     2284 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/logging.py
+-rw-r--r--   0        0        0      938 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/models/__init__.py
+-rw-r--r--   0        0        0     1420 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/models/base.py
+-rw-r--r--   0        0        0    18467 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/models/database.py
+-rw-r--r--   0        0        0     3178 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/models/metadata_properties.py
+-rw-r--r--   0        0        0     6689 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/models/mixins.py
+-rw-r--r--   0        0        0      773 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/models/suggestions.py
+-rw-r--r--   0        0        0    22732 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/policies.py
+-rw-r--r--   0        0        0      905 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/errors.py
+-rw-r--r--   0        0        0      735 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/generics.py
+-rw-r--r--   0        0        0      729 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/utils.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/__init__.py
+-rw-r--r--   0        0        0     1639 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/base.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/__init__.py
+-rw-r--r--   0        0        0     1056 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/authentication.py
+-rw-r--r--   0        0        0     2260 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/datasets.py
+-rw-r--r--   0        0        0     2207 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/users.py
+-rw-r--r--   0        0        0     1079 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/workspaces.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     2601 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/datasets.py
+-rw-r--r--   0        0        0     2414 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/fields.py
+-rw-r--r--   0        0        0      786 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/info.py
+-rw-r--r--   0        0        0     5522 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/metadata_properties.py
+-rw-r--r--   0        0        0      873 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/oauth2.py
+-rw-r--r--   0        0        0    11234 2024-05-30 14:20:53.693105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/questions.py
+-rw-r--r--   0        0        0    10639 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/records.py
+-rw-r--r--   0        0        0     1853 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/records_bulk.py
+-rw-r--r--   0        0        0     5862 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/responses.py
+-rw-r--r--   0        0        0     1670 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/settings.py
+-rw-r--r--   0        0        0     2925 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/suggestions.py
+-rw-r--r--   0        0        0     1717 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/users.py
+-rw-r--r--   0        0        0     2376 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/vector_settings.py
+-rw-r--r--   0        0        0      803 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/vectors.py
+-rw-r--r--   0        0        0     1214 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/workspaces.py
+-rw-r--r--   0        0        0      949 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/search_engine/__init__.py
+-rw-r--r--   0        0        0     9988 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/search_engine/base.py
+-rw-r--r--   0        0        0    34423 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/search_engine/commons.py
+-rw-r--r--   0        0        0     5910 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/search_engine/elasticsearch.py
+-rw-r--r--   0        0        0     6186 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/search_engine/opensearch.py
+-rw-r--r--   0        0        0      687 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/__init__.py
+-rw-r--r--   0        0        0      791 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/__init__.py
+-rw-r--r--   0        0        0     1338 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/claims.py
+-rw-r--r--   0        0        0      810 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/db/__init__.py
+-rw-r--r--   0        0        0     1718 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/db/api_key_backend.py
+-rw-r--r--   0        0        0     1818 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/db/bearer_token_backend.py
+-rw-r--r--   0        0        0     1527 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/jwt.py
+-rw-r--r--   0        0        0      764 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/__init__.py
+-rw-r--r--   0        0        0     1797 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/auth_backend.py
+-rw-r--r--   0        0        0     6795 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/client_provider.py
+-rw-r--r--   0        0        0     3576 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/settings.py
+-rw-r--r--   0        0        0     1873 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/supported_providers.py
+-rw-r--r--   0        0        0     2887 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/provider.py
+-rw-r--r--   0        0        0     1288 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/authentication/userinfo.py
+-rw-r--r--   0        0        0     2693 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/model.py
+-rw-r--r--   0        0        0     2185 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/security/settings.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/server.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/__init__.py
+-rw-r--r--   0        0        0    10394 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/datasets.py
+-rw-r--r--   0        0        0     2862 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/info.py
+-rw-r--r--   0        0        0      702 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/metrics/__init__.py
+-rw-r--r--   0        0        0     5036 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/metrics/models.py
+-rw-r--r--   0        0        0     4102 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/metrics/service.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/search/__init__.py
+-rw-r--r--   0        0        0     2154 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/search/model.py
+-rw-r--r--   0        0        0     4929 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/search/service.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/storage/__init__.py
+-rw-r--r--   0        0        0     4287 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/storage/service.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/__init__.py
+-rw-r--r--   0        0        0      629 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/commons/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/commons/models.py
+-rw-r--r--   0        0        0      645 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text2text/__init__.py
+-rw-r--r--   0        0        0     2460 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text2text/models.py
+-rw-r--r--   0        0        0     4300 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text2text/service.py
+-rw-r--r--   0        0        0      654 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/__init__.py
+-rw-r--r--   0        0        0     6258 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/metrics.py
+-rw-r--r--   0        0        0    10345 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/model.py
+-rw-r--r--   0        0        0    13450 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/service.py
+-rw-r--r--   0        0        0      655 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/__init__.py
+-rw-r--r--   0        0        0    15760 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/metrics.py
+-rw-r--r--   0        0        0     6801 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/model.py
+-rw-r--r--   0        0        0     5488 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/service.py
+-rw-r--r--   0        0        0     8391 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/settings.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/.nojekyll
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/200.html
+-rw-r--r--   0        0        0      435 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/README.md
+-rw-r--r--   0        0        0    34042 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/013b2a2.js
+-rw-r--r--   0        0        0     8735 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/044f51a.js
+-rw-r--r--   0        0        0    14896 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/04ee322.js
+-rw-r--r--   0        0        0    18396 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/062aa1b.js
+-rw-r--r--   0        0        0    24146 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/067807e.js
+-rw-r--r--   0        0        0    33180 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/07d520c.js
+-rw-r--r--   0        0        0     5885 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0825c42.js
+-rw-r--r--   0        0        0    17327 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0860d7f.js
+-rw-r--r--   0        0        0    13877 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0871234.js
+-rw-r--r--   0        0        0    36431 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/089e044.js
+-rw-r--r--   0        0        0   191172 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0947351.js
+-rw-r--r--   0        0        0     2059 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0ddded0.js
+-rw-r--r--   0        0        0    18927 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0e81119.js
+-rw-r--r--   0        0        0     1305 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0f97c02.js
+-rw-r--r--   0        0        0    15499 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/10080fe.js
+-rw-r--r--   0        0        0    38481 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1069132.js
+-rw-r--r--   0        0        0    20403 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/118c84b.js
+-rw-r--r--   0        0        0      420 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/119484b.js
+-rw-r--r--   0        0        0     1297 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1200f05.js
+-rw-r--r--   0        0        0    23070 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/14cc7db.js
+-rw-r--r--   0        0        0    35679 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/150492b.js
+-rw-r--r--   0        0        0     3236 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/17934c0.js
+-rw-r--r--   0        0        0    47783 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/17e1412.js
+-rw-r--r--   0        0        0    11989 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/180c687.js
+-rw-r--r--   0        0        0    10073 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/18218e0.js
+-rw-r--r--   0        0        0    73003 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/18ced35.js
+-rw-r--r--   0        0        0     5849 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/18d4cfc.js
+-rw-r--r--   0        0        0    15509 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/19065ba.js
+-rw-r--r--   0        0        0    13465 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/195ef90.js
+-rw-r--r--   0        0        0     5772 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/19bc22f.js
+-rw-r--r--   0        0        0     7884 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1a8d6cd.js
+-rw-r--r--   0        0        0     7819 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1c811c3.js
+-rw-r--r--   0        0        0     9390 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1d154db.js
+-rw-r--r--   0        0        0     7431 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1daf168.js
+-rw-r--r--   0        0        0    13932 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1e0fecd.js
+-rw-r--r--   0        0        0    23778 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/20656e6.js
+-rw-r--r--   0        0        0     7610 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/20e2acb.js
+-rw-r--r--   0        0        0     9396 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/21af5f2.js
+-rw-r--r--   0        0        0    26912 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/236468b.js
+-rw-r--r--   0        0        0     7242 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/23d5212.js
+-rw-r--r--   0        0        0     2283 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/253fe5d.js
+-rw-r--r--   0        0        0    10102 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/25a65ea.js
+-rw-r--r--   0        0        0    16084 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/28f0cc4.js
+-rw-r--r--   0        0        0    21212 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/293afa8.js
+-rw-r--r--   0        0        0     6624 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2a02714.js
+-rw-r--r--   0        0        0     7115 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2a30bbe.js
+-rw-r--r--   0        0        0      603 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2b4bd32.js
+-rw-r--r--   0        0        0    24173 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2b6a91d.js
+-rw-r--r--   0        0        0     8996 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2bcabcb.js
+-rw-r--r--   0        0        0    11010 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2be230f.js
+-rw-r--r--   0        0        0    22686 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/334cf94.js
+-rw-r--r--   0        0        0     1270 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/34b0f74.js
+-rw-r--r--   0        0        0    26677 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/34fb14a.js
+-rw-r--r--   0        0        0     9071 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/35267f4.js
+-rw-r--r--   0        0        0    16047 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3589b51.js
+-rw-r--r--   0        0        0    13433 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/35c38bb.js
+-rw-r--r--   0        0        0    56981 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3660432.js
+-rw-r--r--   0        0        0     8689 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37678ae.js
+-rw-r--r--   0        0        0    45970 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37a8d34.js
+-rw-r--r--   0        0        0    18862 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37e0496.js
+-rw-r--r--   0        0        0     8493 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37f0ed3.js
+-rw-r--r--   0        0        0      954 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/38bfa8a.js
+-rw-r--r--   0        0        0     9738 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/393e0cb.js
+-rw-r--r--   0        0        0    50017 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3ae506d.js
+-rw-r--r--   0        0        0    66203 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3b116b7.js
+-rw-r--r--   0        0        0     9390 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3d2f697.js
+-rw-r--r--   0        0        0    17751 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3e416f9.js
+-rw-r--r--   0        0        0  2363254 2024-05-30 14:29:57.277733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3eb41c4.js
+-rw-r--r--   0        0        0     1333 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/41bfc83.js
+-rw-r--r--   0        0        0    15176 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4288855.js
+-rw-r--r--   0        0        0    57895 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/42e48d6.js
+-rw-r--r--   0        0        0    31439 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/431ac92.js
+-rw-r--r--   0        0        0     8834 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/433d86e.js
+-rw-r--r--   0        0        0     8742 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/44da1fe.js
+-rw-r--r--   0        0        0    24734 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/45c5778.js
+-rw-r--r--   0        0        0    47287 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/473c94a.js
+-rw-r--r--   0        0        0     8598 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/48ab383.js
+-rw-r--r--   0        0        0     6545 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/48afbb8.js
+-rw-r--r--   0        0        0    18358 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/48bdb55.js
+-rw-r--r--   0        0        0    44536 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4943115.js
+-rw-r--r--   0        0        0    18793 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/49efda7.js
+-rw-r--r--   0        0        0     6746 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4a00879.js
+-rw-r--r--   0        0        0   787702 2024-05-30 14:29:57.273733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4a07ba2.js
+-rw-r--r--   0        0        0     1632 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4ab08c6.js
+-rw-r--r--   0        0        0    18887 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4ab2f0e.js
+-rw-r--r--   0        0        0     6202 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4afa49d.js
+-rw-r--r--   0        0        0     1270 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4b8c9e5.js
+-rw-r--r--   0        0        0     7411 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4cb5088.js
+-rw-r--r--   0        0        0     9558 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4d350f9.js
+-rw-r--r--   0        0        0    20511 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4d4f708.js
+-rw-r--r--   0        0        0    16735 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4ed7f9b.js
+-rw-r--r--   0        0        0     6427 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/50100f8.js
+-rw-r--r--   0        0        0    20923 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5048443.js
+-rw-r--r--   0        0        0     7938 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5128dee.js
+-rw-r--r--   0        0        0    50936 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/516e13f.js
+-rw-r--r--   0        0        0     7080 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/517a829.js
+-rw-r--r--   0        0        0     5779 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5221f06.js
+-rw-r--r--   0        0        0    23693 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/523b8f3.js
+-rw-r--r--   0        0        0     1012 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5250978.js
+-rw-r--r--   0        0        0    38665 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/52bc438.js
+-rw-r--r--   0        0        0     1821 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5313688.js
+-rw-r--r--   0        0        0    23973 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/53f6e15.js
+-rw-r--r--   0        0        0     7742 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/55ca8de.js
+-rw-r--r--   0        0        0     8439 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/56939a1.js
+-rw-r--r--   0        0        0    10049 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/56e2001.js
+-rw-r--r--   0        0        0      443 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5808988.js
+-rw-r--r--   0        0        0      420 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5925665.js
+-rw-r--r--   0        0        0   134978 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/59f135b.js
+-rw-r--r--   0        0        0    19479 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5bfecac.js
+-rw-r--r--   0        0        0    56247 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5c9196c.js
+-rw-r--r--   0        0        0    35455 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5fa1d20.js
+-rw-r--r--   0        0        0     1603 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/603a676.js
+-rw-r--r--   0        0        0    67976 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/615110d.js
+-rw-r--r--   0        0        0     9380 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/62e65e8.js
+-rw-r--r--   0        0        0    28588 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/63d8f21.js
+-rw-r--r--   0        0        0    38103 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/65cbc28.js
+-rw-r--r--   0        0        0    17525 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/67b5ce1.js
+-rw-r--r--   0        0        0    22216 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6a2bb14.js
+-rw-r--r--   0        0        0     5977 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6c3f9c9.js
+-rw-r--r--   0        0        0     7377 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6d2c5ba.js
+-rw-r--r--   0        0        0    13915 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6d6d001.js
+-rw-r--r--   0        0        0     6659 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6d915c8.js
+-rw-r--r--   0        0        0     8377 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6dd33cc.js
+-rw-r--r--   0        0        0   329983 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7002aba.js
+-rw-r--r--   0        0        0     7460 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/70072c5.js
+-rw-r--r--   0        0        0    22275 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7062e38.js
+-rw-r--r--   0        0        0     1838 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/70a28c1.js
+-rw-r--r--   0        0        0     6508 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71043f0.js
+-rw-r--r--   0        0        0    36399 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/711e9f4.js
+-rw-r--r--   0        0        0    47944 2024-05-30 14:29:57.269733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71861c4.js
+-rw-r--r--   0        0        0   184996 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/719d89c.js
+-rw-r--r--   0        0        0    14033 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71bff6b.js
+-rw-r--r--   0        0        0    32394 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71f1583.js
+-rw-r--r--   0        0        0    17297 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/722387e.js
+-rw-r--r--   0        0        0     8931 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7304342.js
+-rw-r--r--   0        0        0     9329 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7308f13.js
+-rw-r--r--   0        0        0     6979 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/755499f.js
+-rw-r--r--   0        0        0    27264 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/76e0837.js
+-rw-r--r--   0        0        0     1750 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/77d5c4e.js
+-rw-r--r--   0        0        0    20692 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7810ab7.js
+-rw-r--r--   0        0        0     7687 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/783d220.js
+-rw-r--r--   0        0        0   164308 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/791a0d6.js
+-rw-r--r--   0        0        0     6263 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/79287e2.js
+-rw-r--r--   0        0        0    32328 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7a8b85c.js
+-rw-r--r--   0        0        0     9524 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7aea98f.js
+-rw-r--r--   0        0        0     6694 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7b71301.js
+-rw-r--r--   0        0        0     6772 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7bda7b2.js
+-rw-r--r--   0        0        0     9925 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7c86bca.js
+-rw-r--r--   0        0        0     6029 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7d19bec.js
+-rw-r--r--   0        0        0    12448 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7d95f80.js
+-rw-r--r--   0        0        0     6608 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7e2d35c.js
+-rw-r--r--   0        0        0     7373 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7f014bb.js
+-rw-r--r--   0        0        0    35020 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7f50bb1.js
+-rw-r--r--   0        0        0     6843 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/811f3aa.js
+-rw-r--r--   0        0        0     8481 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/82243c9.js
+-rw-r--r--   0        0        0     1897 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/827fbc3.js
+-rw-r--r--   0        0        0     1821 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/859e3a2.js
+-rw-r--r--   0        0        0   420673 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/85aa264.js
+-rw-r--r--   0        0        0    32804 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/86a6498.js
+-rw-r--r--   0        0        0   104201 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8753b79.js
+-rw-r--r--   0        0        0     8668 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8a2c5a2.js
+-rw-r--r--   0        0        0    31603 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8a9dc00.js
+-rw-r--r--   0        0        0     5615 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8ac6918.js
+-rw-r--r--   0        0        0     6998 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8b30d40.js
+-rw-r--r--   0        0        0    16186 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8c85121.js
+-rw-r--r--   0        0        0    79820 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8debb26.js
+-rw-r--r--   0        0        0    15255 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8f61c54.js
+-rw-r--r--   0        0        0    15344 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9060868.js
+-rw-r--r--   0        0        0     6780 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9133688.js
+-rw-r--r--   0        0        0    35459 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/913ad1e.js
+-rw-r--r--   0        0        0    21968 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/919299c.js
+-rw-r--r--   0        0        0    39034 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/923d2e5.js
+-rw-r--r--   0        0        0    11589 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/938a825.js
+-rw-r--r--   0        0        0    16614 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/93ff988.js
+-rw-r--r--   0        0        0    22290 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/949e7ce.js
+-rw-r--r--   0        0        0     3888 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/95ab122.js
+-rw-r--r--   0        0        0     5701 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/95db8b3.js
+-rw-r--r--   0        0        0    26510 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/961efe0.js
+-rw-r--r--   0        0        0     8339 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9651160.js
+-rw-r--r--   0        0        0     8169 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/96c3974.js
+-rw-r--r--   0        0        0     1919 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/97cdc40.js
+-rw-r--r--   0        0        0     9992 2024-05-30 14:29:57.265733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/980752a.js
+-rw-r--r--   0        0        0    41531 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/98b724f.js
+-rw-r--r--   0        0        0     7772 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9959e1c.js
+-rw-r--r--   0        0        0     8030 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9a6c8ed.js
+-rw-r--r--   0        0        0     1921 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9b4233d.js
+-rw-r--r--   0        0        0     7384 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9c2eddf.js
+-rw-r--r--   0        0        0    36636 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9c66ec1.js
+-rw-r--r--   0        0        0    25826 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9d7b714.js
+-rw-r--r--   0        0        0     1049 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9d8ec11.js
+-rw-r--r--   0        0        0     9590 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9dc9c16.js
+-rw-r--r--   0        0        0     5986 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9fb2cd3.js
+-rw-r--r--   0        0        0     1726 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/LICENSES
+-rw-r--r--   0        0        0     3282 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a0a7333.js
+-rw-r--r--   0        0        0    63778 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a128d0a.js
+-rw-r--r--   0        0        0    24710 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a233280.js
+-rw-r--r--   0        0        0     8209 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a4051d7.js
+-rw-r--r--   0        0        0    34002 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a61d3e4.js
+-rw-r--r--   0        0        0    16602 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a63bfb6.js
+-rw-r--r--   0        0        0    16740 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a757343.js
+-rw-r--r--   0        0        0    25622 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a8ae09e.js
+-rw-r--r--   0        0        0    33881 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a97c5b4.js
+-rw-r--r--   0        0        0    64350 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a99f76b.js
+-rw-r--r--   0        0        0   421296 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/aa2a6d6.js
+-rw-r--r--   0        0        0     1306 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/aa2b049.js
+-rw-r--r--   0        0        0     9828 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ad412fa.js
+-rw-r--r--   0        0        0    23279 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ade1835.js
+-rw-r--r--   0        0        0     6789 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/af2be6c.js
+-rw-r--r--   0        0        0      420 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b1feae4.js
+-rw-r--r--   0        0        0      931 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b21e71c.js
+-rw-r--r--   0        0        0     9031 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b28cfbc.js
+-rw-r--r--   0        0        0     1009 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b2f22c5.js
+-rw-r--r--   0        0        0    25066 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b2fc075.js
+-rw-r--r--   0        0        0   558191 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b4c1d0d.js
+-rw-r--r--   0        0        0      482 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b4f53d2.js
+-rw-r--r--   0        0        0    40322 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b53ca3b.js
+-rw-r--r--   0        0        0     1205 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b5b4aae.js
+-rw-r--r--   0        0        0   590941 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b6ffaa9.js
+-rw-r--r--   0        0        0     1260 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b781657.js
+-rw-r--r--   0        0        0     1415 2024-05-30 14:29:57.261733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b804ce5.js
+-rw-r--r--   0        0        0    11573 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b8c421d.js
+-rw-r--r--   0        0        0     1207 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b955150.js
+-rw-r--r--   0        0        0    28137 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bad085e.js
+-rw-r--r--   0        0        0    28039 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bad26d7.js
+-rw-r--r--   0        0        0    52299 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bd7cb12.js
+-rw-r--r--   0        0        0     4508 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bdf5c09.js
+-rw-r--r--   0        0        0     5403 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/beccc06.js
+-rw-r--r--   0        0        0    35550 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bedb2dd.js
+-rw-r--r--   0        0        0    19503 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bef1a27.js
+-rw-r--r--   0        0        0    17968 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bf6bced.js
+-rw-r--r--   0        0        0      603 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c02ad86.js
+-rw-r--r--   0        0        0     8439 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c26b3ec.js
+-rw-r--r--   0        0        0    20780 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c380661.js
+-rw-r--r--   0        0        0    39831 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c5ba452.js
+-rw-r--r--   0        0        0      954 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c5dda82.js
+-rw-r--r--   0        0        0     6284 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c606e8c.js
+-rw-r--r--   0        0        0     8622 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c615699.js
+-rw-r--r--   0        0        0     1472 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c72e4ee.js
+-rw-r--r--   0        0        0     7961 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c863a84.js
+-rw-r--r--   0        0        0    17385 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c9f74e7.js
+-rw-r--r--   0        0        0    23243 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ca0d950.js
+-rw-r--r--   0        0        0    56678 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cba5c90.js
+-rw-r--r--   0        0        0     7474 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cc5cbbe.js
+-rw-r--r--   0        0        0     8089 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cd3d6f6.js
+-rw-r--r--   0        0        0     5871 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cd61b37.js
+-rw-r--r--   0        0        0    68986 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cdeab7c.js
+-rw-r--r--   0        0        0   624339 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cf435aa.js
+-rw-r--r--   0        0        0    36311 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cf5d4e8.js
+-rw-r--r--   0        0        0   377557 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d3b25ba.js
+-rw-r--r--   0        0        0    23720 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d3ec09a.js
+-rw-r--r--   0        0        0   329438 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d6044c6.js
+-rw-r--r--   0        0        0      603 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d8454ea.js
+-rw-r--r--   0        0        0    23669 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d8c7cdd.js
+-rw-r--r--   0        0        0     8996 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d95f66b.js
+-rw-r--r--   0        0        0     8932 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d9f709f.js
+-rw-r--r--   0        0        0    13915 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/da56dc9.js
+-rw-r--r--   0        0        0    41490 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/da98642.js
+-rw-r--r--   0        0        0   138125 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/dae7b34.js
+-rw-r--r--   0        0        0     3066 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/de51b34.js
+-rw-r--r--   0        0        0     5835 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/df05a2c.js
+-rw-r--r--   0        0        0     8332 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/df0702e.js
+-rw-r--r--   0        0        0    18956 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/dfb4e3d.js
+-rw-r--r--   0        0        0    14414 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e1fa0db.js
+-rw-r--r--   0        0        0    25241 2024-05-30 14:29:57.257733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e208f0f.js
+-rw-r--r--   0        0        0    25259 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e23db67.js
+-rw-r--r--   0        0        0    54826 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e2678f8.js
+-rw-r--r--   0        0        0      560 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e311004.js
+-rw-r--r--   0        0        0    46483 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e31b663.js
+-rw-r--r--   0        0        0    23279 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e3fe598.js
+-rw-r--r--   0        0        0    15135 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e44b050.js
+-rw-r--r--   0        0        0    22723 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e4c5fa4.js
+-rw-r--r--   0        0        0     8487 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e4cf190.js
+-rw-r--r--   0        0        0    33699 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e4f9f5b.js
+-rw-r--r--   0        0        0     5670 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e63dbd4.js
+-rw-r--r--   0        0        0     9319 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e7035e6.js
+-rw-r--r--   0        0        0    68469 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e79118e.js
+-rw-r--r--   0        0        0    16063 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e79cf5b.js
+-rw-r--r--   0        0        0     8394 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e7e5f43.js
+-rw-r--r--   0        0        0    18287 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e8142c4.js
+-rw-r--r--   0        0        0   119788 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e8e19b2.js
+-rw-r--r--   0        0        0     2284 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e901328.js
+-rw-r--r--   0        0        0    10082 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ea525f4.js
+-rw-r--r--   0        0        0     5982 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/eb1faf3.js
+-rw-r--r--   0        0        0     7276 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/edd702e.js
+-rw-r--r--   0        0        0    24471 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/efe6a6f.js
+-rw-r--r--   0        0        0     7593 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f03fccb.js
+-rw-r--r--   0        0        0    18228 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f0a6dd7.js
+-rw-r--r--   0        0        0     6115 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f14f26d.js
+-rw-r--r--   0        0        0   329973 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f217920.js
+-rw-r--r--   0        0        0      289 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f2cf071.js
+-rw-r--r--   0        0        0     5853 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f36addc.js
+-rw-r--r--   0        0        0    36070 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f3b5d22.js
+-rw-r--r--   0        0        0    14514 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f3eb9f7.js
+-rw-r--r--   0        0        0     7613 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f3f39b2.js
+-rw-r--r--   0        0        0    25350 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f409abc.js
+-rw-r--r--   0        0        0    17834 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f41b1df.js
+-rw-r--r--   0        0        0     9321 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f66f192.js
+-rw-r--r--   0        0        0    11382 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f6c0467.js
+-rw-r--r--   0        0        0    29182 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f7afca5.js
+-rw-r--r--   0        0        0    33119 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f86ebc2.js
+-rw-r--r--   0        0        0     9004 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f947aa0.js
+-rw-r--r--   0        0        0     8504 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fa7f8a6.js
+-rw-r--r--   0        0        0     7481 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fa9e6f9.js
+-rw-r--r--   0        0        0     1507 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fd39885.js
+-rw-r--r--   0        0        0    14475 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fd59c1c.js
+-rw-r--r--   0        0        0    86840 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fd65964.js
+-rw-r--r--   0        0        0     7158 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fdf390c.js
+-rw-r--r--   0        0        0    25130 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fe8b19e.js
+-rw-r--r--   0        0        0    13339 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fec21cc.js
+-rw-r--r--   0        0        0    67510 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fefbfff.js
+-rw-r--r--   0        0        0    28116 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.3c074ae.woff2
+-rw-r--r--   0        0        0    36012 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.f7cfb4c.woff
+-rw-r--r--   0        0        0     5814 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/apple-touch-icon.png
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/datasets/index.html
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/datasets/useDatasetsViewModel/index.html
+-rw-r--r--   0        0        0     1048 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/favicon-16x16.png
+-rw-r--r--   0        0        0     1139 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/favicon.ico
+-rw-r--r--   0        0        0      263 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/arrow-down.svg
+-rw-r--r--   0        0        0      278 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/arrow-up.svg
+-rw-r--r--   0        0        0     1134 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/bulk-mode.svg
+-rw-r--r--   0        0        0     1743 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/change-height.svg
+-rw-r--r--   0        0        0      201 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/check.svg
+-rw-r--r--   0        0        0      199 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/chevron-down.svg
+-rw-r--r--   0        0        0      187 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/chevron-left.svg
+-rw-r--r--   0        0        0      183 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/chevron-right.svg
+-rw-r--r--   0        0        0      199 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/chevron-up.svg
+-rw-r--r--   0        0        0      761 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/clear.svg
+-rw-r--r--   0        0        0      638 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/close.svg
+-rw-r--r--   0        0        0      518 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/code.svg
+-rw-r--r--   0        0        0      353 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/copy.svg
+-rw-r--r--   0        0        0     2408 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/danger.svg
+-rw-r--r--   0        0        0      637 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/discard.svg
+-rw-r--r--   0        0        0     1372 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/draggable.svg
+-rw-r--r--   0        0        0      375 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/expand-arrows.svg
+-rw-r--r--   0        0        0      956 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/exploration.svg
+-rw-r--r--   0        0        0      350 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/external-link.svg
+-rw-r--r--   0        0        0      364 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/external.svg
+-rw-r--r--   0        0        0      590 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/filter.svg
+-rw-r--r--   0        0        0      382 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/focus-mode.svg
+-rw-r--r--   0        0        0      643 2024-05-30 14:29:57.253733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/hand-labeling.svg
+-rw-r--r--   0        0        0      835 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/info.svg
+-rw-r--r--   0        0        0      685 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/kebab.svg
+-rw-r--r--   0        0        0     1021 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/link.svg
+-rw-r--r--   0        0        0      548 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/log-out.svg
+-rw-r--r--   0        0        0      595 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/matching.svg
+-rwxr-xr-x   0        0        0      487 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/math-plus.svg
+-rw-r--r--   0        0        0      585 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/meatballs.svg
+-rw-r--r--   0        0        0      465 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/minimize-arrows.svg
+-rw-r--r--   0        0        0     1010 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/no-matching.svg
+-rw-r--r--   0        0        0      816 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/pen.svg
+-rw-r--r--   0        0        0      651 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/progress.svg
+-rw-r--r--   0        0        0      526 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/refresh.svg
+-rw-r--r--   0        0        0      568 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/reset.svg
+-rw-r--r--   0        0        0      800 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/row-last.svg
+-rw-r--r--   0        0        0      805 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/search.svg
+-rw-r--r--   0        0        0     4510 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/settings.svg
+-rw-r--r--   0        0        0      977 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/shortcuts.svg
+-rw-r--r--   0        0        0     1668 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/similarity.svg
+-rw-r--r--   0        0        0      888 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/smile-sad.svg
+-rw-r--r--   0        0        0      354 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/sort.svg
+-rw-r--r--   0        0        0      260 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/stats.svg
+-rw-r--r--   0        0        0     1131 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/suggestion.svg
+-rw-r--r--   0        0        0     2187 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/support.svg
+-rw-r--r--   0        0        0      451 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/time.svg
+-rw-r--r--   0        0        0      809 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/trash-empty.svg
+-rw-r--r--   0        0        0      630 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/unavailable.svg
+-rw-r--r--   0        0        0      647 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/validate.svg
+-rw-r--r--   0        0        0     1233 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/icons/weak-labeling.svg
+-rw-r--r--   0        0        0    29161 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/images/help-info/explain.png
+-rw-r--r--   0        0        0   121622 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/images/help-info/similarity.png
+-rw-r--r--   0        0        0     3554 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/images/logo.svg
+-rw-r--r--   0        0        0   346289 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/images/welcome-hf-sign-in-ss.png
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/index.html
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/sign-in/index.html
+-rw-r--r--   0        0        0      426 2024-05-30 14:29:57.249733 argilla_server-1.29.0rc1/src/argilla_server/static/site.webmanifest
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/useWelcomeHFViewModel/index.html
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/user-settings/index.html
+-rw-r--r--   0        0        0     3626 2024-05-30 14:29:57.281733 argilla_server-1.29.0rc1/src/argilla_server/static/welcome-hf-sign-in/index.html
+-rw-r--r--   0        0        0     1618 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/static_rewrite.py
+-rw-r--r--   0        0        0     4550 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/telemetry.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/use_cases/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/use_cases/responses/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/use_cases/responses/upsert_responses_in_bulk.py
+-rw-r--r--   0        0        0     6793 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/utils.py
+-rw-r--r--   0        0        0      730 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/utils/__init__.py
+-rw-r--r--   0        0        0     2973 2024-05-30 14:20:53.697105 argilla_server-1.29.0rc1/src/argilla_server/utils/_telemetry.py
+-rw-r--r--   0        0        0     7709 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/utils/dependency.py
+-rw-r--r--   0        0        0     6788 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/utils/params.py
+-rw-r--r--   0        0        0     8486 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/utils/span_utils.py
+-rw-r--r--   0        0        0     1377 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/utils/utils.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/__init__.py
+-rw-r--r--   0        0        0     6378 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/questions.py
+-rw-r--r--   0        0        0     7169 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/records.py
+-rw-r--r--   0        0        0    12940 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/response_values.py
+-rw-r--r--   0        0        0     3436 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/responses.py
+-rw-r--r--   0        0        0     2513 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/suggestions.py
+-rw-r--r--   0        0        0     1115 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/src/argilla_server/validators/vectors.py
+-rw-r--r--   0        0        0     1116 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3523 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     1106 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/database.py
+-rw-r--r--   0        0        0    12180 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/factories.py
+-rw-r--r--   0        0        0      906 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/pydantic_v1/generics.py
+-rw-r--r--   0        0        0      729 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/pydantic_v1/utils.py
+-rw-r--r--   0        0        0      622 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/test_docs.py
+-rw-r--r--   0        0        0     1163 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/test_not_found_routes.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_authentication.py
+-rw-r--r--   0        0        0    19094 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_datasets.py
+-rw-r--r--   0        0        0     2434 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_info.py
+-rw-r--r--   0        0        0    14083 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_metrics.py
+-rw-r--r--   0        0        0     5360 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_records_get.py
+-rw-r--r--   0        0        0     9023 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_records_update.py
+-rw-r--r--   0        0        0     2152 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_security_token.py
+-rw-r--r--   0        0        0     9256 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_text2text.py
+-rw-r--r--   0        0        0    34224 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_text_classification.py
+-rw-r--r--   0        0        0    23182 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_text_classification_api_rules.py
+-rw-r--r--   0        0        0    11094 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_text_classification_dataset_settings.py
+-rw-r--r--   0        0        0    23310 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_token_classification.py
+-rw-r--r--   0        0        0     7388 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_token_classification_dataset_settings.py
+-rw-r--r--   0        0        0    16140 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_users.py
+-rw-r--r--   0        0        0    15316 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v0/test_workspaces.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/authentication/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/authentication/test_create_token.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/questions/__init__.py
+-rw-r--r--   0        0        0     6250 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/questions/test_create_dataset_question.py
+-rw-r--r--   0        0        0     2581 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/questions/test_list_dataset_questions.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/__init__.py
+-rw-r--r--   0        0        0     6715 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk.py
+-rw-r--r--   0        0        0    14466 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_responses.py
+-rw-r--r--   0        0        0    16789 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_suggestions.py
+-rw-r--r--   0        0        0    13736 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_vectors.py
+-rw-r--r--   0        0        0     9277 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/test_create_dataset_records.py
+-rw-r--r--   0        0        0     7436 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/test_update_dataset_records.py
+-rw-r--r--   0        0        0     7690 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_create_dataset_question.py
+-rw-r--r--   0        0        0     1778 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_create_dataset_vector_settings.py
+-rw-r--r--   0        0        0     7550 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_get_dataset_progress.py
+-rw-r--r--   0        0        0     7099 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_list_dataset_records_search_suggestions_options.py
+-rw-r--r--   0        0        0    24808 2024-05-30 14:20:53.701104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_questions.py
+-rw-r--r--   0        0        0    10220 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_search_current_user_dataset_records.py
+-rw-r--r--   0        0        0    15677 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_search_dataset_records.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/info/__init__.py
+-rw-r--r--   0        0        0     1288 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/info/test_get_status.py
+-rw-r--r--   0        0        0     1026 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/info/test_get_version.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/questions/__init__.py
+-rw-r--r--   0        0        0    10670 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/questions/test_update_question.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/records/__init__.py
+-rw-r--r--   0        0        0    17476 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/records/test_create_record_response.py
+-rw-r--r--   0        0        0    27129 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/records/test_upsert_suggestion.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/responses/__init__.py
+-rw-r--r--   0        0        0    16388 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/responses/test_create_current_user_responses_bulk.py
+-rw-r--r--   0        0        0    19671 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/responses/test_update_response.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/settings/__init__.py
+-rw-r--r--   0        0        0     3926 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/settings/test_get_settings.py
+-rw-r--r--   0        0        0   210934 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_datasets.py
+-rw-r--r--   0        0        0     8602 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_fields.py
+-rw-r--r--   0        0        0    66065 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_list_dataset_records.py
+-rw-r--r--   0        0        0    17388 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_metadata_properties.py
+-rw-r--r--   0        0        0    13387 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_oauth2.py
+-rw-r--r--   0        0        0    21205 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_questions.py
+-rw-r--r--   0        0        0    63240 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_records.py
+-rw-r--r--   0        0        0    18407 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_responses.py
+-rw-r--r--   0        0        0     3533 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_suggestions.py
+-rw-r--r--   0        0        0     3348 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_users.py
+-rw-r--r--   0        0        0     6885 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_vectors_settings.py
+-rw-r--r--   0        0        0     7867 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/test_workspaces.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/users/__init__.py
+-rw-r--r--   0        0        0    10802 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_create_user.py
+-rw-r--r--   0        0        0     3177 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_delete_user.py
+-rw-r--r--   0        0        0     1608 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_get_current_user.py
+-rw-r--r--   0        0        0     2618 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_get_user.py
+-rw-r--r--   0        0        0     3225 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_list_users.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/__init__.py
+-rw-r--r--   0        0        0     4166 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_create_workspace.py
+-rw-r--r--   0        0        0     5420 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_create_workspace_user.py
+-rw-r--r--   0        0        0     6310 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_delete_workspace_user.py
+-rw-r--r--   0        0        0     5479 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_list_workspace_users.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/conftest.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/__init__.py
+-rw-r--r--   0        0        0     1330 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/conftest.py
+-rw-r--r--   0        0        0     9387 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_create.py
+-rw-r--r--   0        0        0     3595 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_create_default.py
+-rw-r--r--   0        0        0     6328 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_migrate.py
+-rw-r--r--   0        0        0     2626 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_update.py
+-rw-r--r--   0        0        0     1207 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_user_files/users.yml
+-rw-r--r--   0        0        0      252 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_user_files/users_invalid_user.yml
+-rw-r--r--   0        0        0      257 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_user_files/users_invalid_workspace.yml
+-rw-r--r--   0        0        0      240 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_user_files/users_one.yml
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/search_engine/__init__.py
+-rw-r--r--   0        0        0      966 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/search_engine/conftest.py
+-rw-r--r--   0        0        0     1466 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/search_engine/test_reindex.py
+-rw-r--r--   0        0        0     1152 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/cli/test_start.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/commons/__init__.py
+-rw-r--r--   0        0        0     1311 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/commons/test_records_dao.py
+-rw-r--r--   0        0        0     2708 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/commons/test_settings.py
+-rw-r--r--   0        0        0     2652 2024-05-30 14:20:53.705104 argilla_server-1.29.0rc1/tests/unit/commons/test_telemetry.py
+-rw-r--r--   0        0        0     4670 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/conftest.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/contexts/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/contexts/search/__init__.py
+-rw-r--r--   0        0        0     9910 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/contexts/search/test_search_records_query_validator.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/backend/__init__.py
+-rw-r--r--   0        0        0     1535 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/backend/test_es_client.py
+-rw-r--r--   0        0        0     4141 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/backend/test_generic_elastic_engine.py
+-rw-r--r--   0        0        0     3477 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/backend/test_query_builder.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/models/__init__.py
+-rw-r--r--   0        0        0     1918 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/models/test_records.py
+-rw-r--r--   0        0        0     3078 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/daos/test_datasets.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/errors/__init__.py
+-rw-r--r--   0        0        0     2682 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/errors/test_api_errors.py
+-rw-r--r--   0        0        0      870 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/errors/test_errors.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/old_models/__init__.py
+-rw-r--r--   0        0        0     3246 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/old_models/test_datasets.py
+-rw-r--r--   0        0        0     4175 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/old_models/test_text2text.py
+-rw-r--r--   0        0        0    12876 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/old_models/test_text_classification.py
+-rw-r--r--   0        0        0    11021 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/old_models/test_token_classification.py
+-rw-r--r--   0        0        0     7785 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/models/test_base.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/schemas/__init__.py
+-rw-r--r--   0        0        0      974 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/schemas/test_base.py
+-rw-r--r--   0        0        0     2914 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/schemas/v1/responses/test_response_value_create.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/search_engine/__init__.py
+-rw-r--r--   0        0        0     1719 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/search_engine/conftest.py
+-rw-r--r--   0        0        0    56309 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/search_engine/test_commons.py
+-rw-r--r--   0        0        0     2658 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/search_engine/test_elastisearch.py
+-rw-r--r--   0        0        0     3370 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/search_engine/test_opensearch.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/security/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/security/authentication/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/security/authentication/oauth2/__init__.py
+-rw-r--r--   0        0        0     2437 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/security/authentication/oauth2/test_settings.py
+-rw-r--r--   0        0        0     3250 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/security/test_model.py
+-rw-r--r--   0        0        0     1872 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/security/test_settings.py
+-rw-r--r--   0        0        0     1608 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/test_app.py
+-rw-r--r--   0        0        0     2180 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/test_logging.py
+-rw-r--r--   0        0        0     4008 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/test_utils.py
+-rw-r--r--   0        0        0      622 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     5140 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/utils/test_dependency.py
+-rw-r--r--   0        0        0     5538 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/utils/test_span_utils.py
+-rw-r--r--   0        0        0      606 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/validators/__init__.py
+-rw-r--r--   0        0        0     5336 2024-05-30 14:20:53.709104 argilla_server-1.29.0rc1/tests/unit/validators/test_records_bulk.py
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 argilla_server-1.29.0rc1/PKG-INFO
```

### Comparing `argilla_server-1.29.0/README.md` & `argilla_server-1.29.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/pyproject.toml` & `argilla_server-1.29.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "social-auth-core ~= 4.5.0",
     "psutil >= 5.8, <5.10",
     "segment-analytics-python == 2.2.0",
     "rich != 13.1.0",
     "typer >= 0.6.0, < 0.10.0",
     "packaging>=23.2",
 ]
-version = "1.29.0"
+version = "1.29.0rc1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 postgresql = [
     "psycopg2 ~= 2.9.5",
```

### Comparing `argilla_server-1.29.0/src/argilla_server/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/__main__.py` & `argilla_server-1.29.0rc1/src/argilla_server/__main__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/_app.py` & `argilla_server-1.29.0rc1/src/argilla_server/_app.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/_messages.py` & `argilla_server-1.29.0rc1/src/argilla_server/_messages.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/_version.py` & `argilla_server-1.29.0rc1/src/argilla_server/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 # coding: utf-8
-__version__ = "1.29.0"
+__version__ = "1.29.0rc1"
```

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic.ini` & `argilla_server-1.29.0rc1/src/argilla_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/env.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/env.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/1769ee58fbb4_create_workspaces_users_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/1769ee58fbb4_create_workspaces_users_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/1e629a913727_fix_suggestions_type_enum_values.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/1e629a913727_fix_suggestions_type_enum_values.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/3a8e2f9b5dea_create_questions_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/3a8e2f9b5dea_create_questions_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/3fc3c0839959_create_suggestions_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/3fc3c0839959_create_suggestions_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/3ff6484f8b37_add_record_metadata_column.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/3ff6484f8b37_add_record_metadata_column.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/74694870197c_create_users_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/74694870197c_create_users_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/7850ab5b42d9_create_vectors_settings_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/7850ab5b42d9_create_vectors_settings_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/7cbcccf8b57a_create_metadata_properties_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/7cbcccf8b57a_create_metadata_properties_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/82a5a88a3fa5_create_workspaces_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/82a5a88a3fa5_create_workspaces_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/84f6b9ff6076_add_last_activity_at_to_datasets_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/84f6b9ff6076_add_last_activity_at_to_datasets_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/8be56284dac0_create_records_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/8be56284dac0_create_records_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/8c574ada5e5f_update_enum_columns.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/8c574ada5e5f_update_enum_columns.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/ae5522b4c674_create_fields_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/ae5522b4c674_create_fields_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/b8458008b60e_add_allow_extra_metadata_column_to_.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/b8458008b60e_add_allow_extra_metadata_column_to_.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/b9099dc08489_create_datasets_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/b9099dc08489_create_datasets_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/bda6fe24314e_create_vectors_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/bda6fe24314e_create_vectors_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/ca7293c38970_change_suggestions_score_column_to_json.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/ca7293c38970_change_suggestions_score_column_to_json.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/alembic/versions/e402e9d9245e_create_responses_table.py` & `argilla_server-1.29.0rc1/src/argilla_server/alembic/versions/e402e9d9245e_create_responses_table.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/errors/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/errors/v1/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/errors/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/errors/v1/exception_handlers.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/errors/v1/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/routes.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/routes.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/authentication.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/authentication.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/info.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/info.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/metrics.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/metrics.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/records_search.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/records_search.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/records_update.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/records_update.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/text2text.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/text2text.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/text_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/text_classification_dataset_settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/text_classification_dataset_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/token_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/token_classification_dataset_settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/token_classification_dataset_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/users.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/handlers/workspaces.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/handlers/workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/helpers.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/commons/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/commons/model.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/commons/model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/commons/params.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/commons/params.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/dataset_settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/dataset_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/text2text.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/text2text.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/text_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/models/token_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/models/token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/validators/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/validators/commons.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/commons.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/validators/text_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v0/validators/token_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v0/validators/token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/authentication.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/authentication.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/questions.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/datasets/records_bulk.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/datasets/records_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/fields.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/fields.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/info.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/info.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/metadata_properties.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/metadata_properties.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/oauth2.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/oauth2.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/questions.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/responses.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/responses.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/suggestions.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/users.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/vectors_settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/vectors_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/apis/v1/handlers/workspaces.py` & `argilla_server-1.29.0rc1/src/argilla_server/apis/v1/handlers/workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/bulk/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/bulk/records_bulk.py` & `argilla_server-1.29.0rc1/src/argilla_server/bulk/records_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/__main__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/__main__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/__main__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/migrate.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/migrate.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/revisions.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/revisions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/__main__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/__main__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/create.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/create.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/create_default.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/create_default.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/migrate.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/migrate.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/update.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/update.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/users/utils.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/users/utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/database/utils.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/database/utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/rich.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/rich.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/search_engine/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/search_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/search_engine/__main__.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/search_engine/__main__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/search_engine/reindex.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/search_engine/reindex.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/start.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/start.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/cli/typer_ext.py` & `argilla_server-1.29.0rc1/src/argilla_server/cli/typer_ext.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/commons/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/commons/config.py` & `argilla_server-1.29.0rc1/src/argilla_server/commons/config.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/commons/models.py` & `argilla_server-1.29.0rc1/src/argilla_server/commons/models.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/constants.py` & `argilla_server-1.29.0rc1/src/argilla_server/constants.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/accounts.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/accounts.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/info.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/info.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/questions.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/search.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/search.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/contexts/settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/contexts/settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/base.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/base.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/elasticsearch.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/factory.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/factory.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/client_adapters/opensearch.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/client_adapters/opensearch.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/generic_elastic.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/generic_elastic.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/helpers.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/stopwords/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/stopwords/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/stopwords/english.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/stopwords/english.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/text2text.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/text2text.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/text_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/mappings/token_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/mappings/token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/base.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/commons.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/commons.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/text_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/metrics/token_classification.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/metrics/token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/query_helpers.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/query_helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/search/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/search/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/search/model.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/search/model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/backend/search/query_builder.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/backend/search/query_builder.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/models/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/models/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/models/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/models/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/models/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/daos/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/daos/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/database.py` & `argilla_server-1.29.0rc1/src/argilla_server/database.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/enums.py` & `argilla_server-1.29.0rc1/src/argilla_server/enums.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/errors/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/errors/base_errors.py` & `argilla_server-1.29.0rc1/src/argilla_server/errors/base_errors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/errors/error_handler.py` & `argilla_server-1.29.0rc1/src/argilla_server/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/errors/future/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/errors/future/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/errors/future/base_errors.py` & `argilla_server-1.29.0rc1/src/argilla_server/errors/future/base_errors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/errors/task_errors.py` & `argilla_server-1.29.0rc1/src/argilla_server/errors/task_errors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/helpers.py` & `argilla_server-1.29.0rc1/src/argilla_server/helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/logging.py` & `argilla_server-1.29.0rc1/src/argilla_server/logging.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/models/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/models/base.py` & `argilla_server-1.29.0rc1/src/argilla_server/models/base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/models/database.py` & `argilla_server-1.29.0rc1/src/argilla_server/models/database.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/models/metadata_properties.py` & `argilla_server-1.29.0rc1/src/argilla_server/models/metadata_properties.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/models/mixins.py` & `argilla_server-1.29.0rc1/src/argilla_server/models/mixins.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/models/suggestions.py` & `argilla_server-1.29.0rc1/src/argilla_server/models/suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/policies.py` & `argilla_server-1.29.0rc1/src/argilla_server/policies.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/pydantic_v1/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/pydantic_v1/errors.py` & `argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/errors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/pydantic_v1/generics.py` & `argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/generics.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/pydantic_v1/utils.py` & `argilla_server-1.29.0rc1/src/argilla_server/pydantic_v1/utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/base.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v0/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v0/authentication.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/authentication.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v0/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v0/users.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v0/workspaces.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v0/workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/fields.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/fields.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/info.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/info.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/metadata_properties.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/metadata_properties.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/oauth2.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/oauth2.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/questions.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/records_bulk.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/records_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/responses.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/responses.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/suggestions.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/users.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/vector_settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/vector_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/vectors.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/vectors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/schemas/v1/workspaces.py` & `argilla_server-1.29.0rc1/src/argilla_server/schemas/v1/workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/search_engine/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/search_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/search_engine/base.py` & `argilla_server-1.29.0rc1/src/argilla_server/search_engine/base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/search_engine/commons.py` & `argilla_server-1.29.0rc1/src/argilla_server/search_engine/commons.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/search_engine/elasticsearch.py` & `argilla_server-1.29.0rc1/src/argilla_server/search_engine/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/search_engine/opensearch.py` & `argilla_server-1.29.0rc1/src/argilla_server/search_engine/opensearch.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/claims.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/claims.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/db/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/db/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/db/api_key_backend.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/db/api_key_backend.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/db/bearer_token_backend.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/db/bearer_token_backend.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/jwt.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/jwt.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/auth_backend.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/auth_backend.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/client_provider.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/client_provider.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/oauth2/supported_providers.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/oauth2/supported_providers.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/provider.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/provider.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/authentication/userinfo.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/authentication/userinfo.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/model.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/security/settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/security/settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/server.py` & `argilla_server-1.29.0rc1/src/argilla_server/server.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/datasets.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/info.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/info.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/metrics/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/metrics/models.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/metrics/models.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/metrics/service.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/metrics/service.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/search/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/search/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/search/model.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/search/model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/search/service.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/search/service.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/storage/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/storage/service.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/storage/service.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/commons/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/commons/models.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/commons/models.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text2text/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text2text/models.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text2text/models.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text2text/service.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text2text/service.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/metrics.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/metrics.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/model.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/text_classification/service.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/text_classification/service.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/metrics.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/metrics.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/model.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/services/tasks/token_classification/service.py` & `argilla_server-1.29.0rc1/src/argilla_server/services/tasks/token_classification/service.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/settings.py` & `argilla_server-1.29.0rc1/src/argilla_server/settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/200.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/200.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/013b2a2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/013b2a2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/044f51a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/044f51a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/04ee322.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/04ee322.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/062aa1b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/062aa1b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/067807e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/067807e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/07d520c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/07d520c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0825c42.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0825c42.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0860d7f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0860d7f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0871234.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0871234.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/089e044.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/089e044.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0947351.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0947351.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0ddded0.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0ddded0.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0e81119.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0e81119.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/0f97c02.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/0f97c02.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/10080fe.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/10080fe.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1069132.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1069132.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/118c84b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/118c84b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1200f05.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1200f05.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/14cc7db.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/14cc7db.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/150492b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/150492b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/17934c0.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/17934c0.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/17e1412.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/17e1412.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/180c687.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/180c687.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/18218e0.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/18218e0.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/18ced35.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/18ced35.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/18d4cfc.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/18d4cfc.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/19065ba.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/19065ba.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/195ef90.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/195ef90.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/19bc22f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/19bc22f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1a8d6cd.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1a8d6cd.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1c811c3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1c811c3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1d154db.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1d154db.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1daf168.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1daf168.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/1e0fecd.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/1e0fecd.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/20656e6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/20656e6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/20e2acb.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/20e2acb.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/21af5f2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/21af5f2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/236468b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/236468b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/23d5212.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/23d5212.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/253fe5d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/253fe5d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/25a65ea.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/25a65ea.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/28f0cc4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/28f0cc4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/293afa8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/293afa8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/2a02714.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2a02714.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/2a30bbe.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2a30bbe.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/2b4bd32.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2b4bd32.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/2b6a91d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2b6a91d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/2bcabcb.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2bcabcb.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/2be230f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/2be230f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/334cf94.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/334cf94.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/34b0f74.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/34b0f74.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/34fb14a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/34fb14a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/35267f4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/35267f4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3589b51.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3589b51.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/35c38bb.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/35c38bb.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3660432.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3660432.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/37678ae.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37678ae.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/37a8d34.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37a8d34.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/37e0496.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37e0496.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/37f0ed3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/37f0ed3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/38bfa8a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/38bfa8a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/393e0cb.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/393e0cb.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3ae506d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3ae506d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3b116b7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3b116b7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3d2f697.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3d2f697.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3e416f9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3e416f9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/3eb41c4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/3eb41c4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/41bfc83.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/41bfc83.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4288855.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4288855.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/42e48d6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/42e48d6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/431ac92.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/431ac92.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/433d86e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/433d86e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/44da1fe.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/44da1fe.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/45c5778.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/45c5778.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/473c94a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/473c94a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/48ab383.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/48ab383.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/48afbb8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/48afbb8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/48bdb55.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/48bdb55.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4943115.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4943115.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/49efda7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/49efda7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4a00879.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4a00879.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4a07ba2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4a07ba2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4ab08c6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4ab08c6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4ab2f0e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4ab2f0e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4afa49d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4afa49d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4b8c9e5.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4b8c9e5.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4cb5088.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4cb5088.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4d350f9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4d350f9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4d4f708.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4d4f708.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/4ed7f9b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/4ed7f9b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/50100f8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/50100f8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5048443.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5048443.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5128dee.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5128dee.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/516e13f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/516e13f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/517a829.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/517a829.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5221f06.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5221f06.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/523b8f3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/523b8f3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5250978.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5250978.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/52bc438.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/52bc438.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5313688.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5313688.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/53f6e15.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/53f6e15.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/55ca8de.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/55ca8de.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/56939a1.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/56939a1.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/56e2001.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/56e2001.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/59f135b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/59f135b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5bfecac.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5bfecac.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5c9196c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5c9196c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/5fa1d20.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/5fa1d20.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/603a676.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/603a676.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/615110d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/615110d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/62e65e8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/62e65e8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/63d8f21.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/63d8f21.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/65cbc28.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/65cbc28.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/67b5ce1.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/67b5ce1.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/6a2bb14.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6a2bb14.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/6c3f9c9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6c3f9c9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/6d2c5ba.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6d2c5ba.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/6d6d001.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6d6d001.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/6d915c8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6d915c8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/6dd33cc.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/6dd33cc.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7002aba.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7002aba.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/70072c5.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/70072c5.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7062e38.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7062e38.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/70a28c1.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/70a28c1.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/71043f0.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71043f0.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/711e9f4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/711e9f4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/71861c4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71861c4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/719d89c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/719d89c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/71bff6b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71bff6b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/71f1583.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/71f1583.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/722387e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/722387e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7304342.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7304342.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7308f13.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7308f13.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/755499f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/755499f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/76e0837.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/76e0837.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/77d5c4e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/77d5c4e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7810ab7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7810ab7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/783d220.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/783d220.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/791a0d6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/791a0d6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/79287e2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/79287e2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7a8b85c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7a8b85c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7aea98f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7aea98f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7b71301.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7b71301.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7bda7b2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7bda7b2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7c86bca.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7c86bca.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7d19bec.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7d19bec.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7d95f80.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7d95f80.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7e2d35c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7e2d35c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7f014bb.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7f014bb.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/7f50bb1.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/7f50bb1.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/811f3aa.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/811f3aa.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/82243c9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/82243c9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/827fbc3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/827fbc3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/859e3a2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/859e3a2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/86a6498.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/86a6498.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8753b79.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8753b79.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8a2c5a2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8a2c5a2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8a9dc00.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8a9dc00.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8ac6918.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8ac6918.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8b30d40.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8b30d40.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8c85121.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8c85121.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8debb26.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8debb26.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/8f61c54.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/8f61c54.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9060868.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9060868.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9133688.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9133688.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/913ad1e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/913ad1e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/919299c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/919299c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/923d2e5.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/923d2e5.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/938a825.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/938a825.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/93ff988.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/93ff988.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/949e7ce.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/949e7ce.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/95ab122.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/95ab122.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/95db8b3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/95db8b3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/961efe0.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/961efe0.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9651160.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9651160.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/96c3974.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/96c3974.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/97cdc40.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/97cdc40.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/980752a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/980752a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/98b724f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/98b724f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9959e1c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9959e1c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9a6c8ed.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9a6c8ed.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9b4233d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9b4233d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9c2eddf.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9c2eddf.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9c66ec1.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9c66ec1.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9d7b714.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9d7b714.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9d8ec11.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9d8ec11.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9dc9c16.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9dc9c16.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/9fb2cd3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/9fb2cd3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/LICENSES` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/LICENSES`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a0a7333.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a0a7333.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a128d0a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a128d0a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a233280.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a233280.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a4051d7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a4051d7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a61d3e4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a61d3e4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a63bfb6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a63bfb6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a757343.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a757343.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a8ae09e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a8ae09e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a97c5b4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a97c5b4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/a99f76b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/a99f76b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/aa2a6d6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/aa2a6d6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/aa2b049.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/aa2b049.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/ad412fa.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ad412fa.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/ade1835.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ade1835.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/af2be6c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/af2be6c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b1c7a5f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/85aa264.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9894,43 +9894,43 @@
                 return Rn
             })), a.d(o, "TokenClassificationSidebar", (function() {
                 return kn
             })), a.d(o, "TokenClassificationStats", (function() {
                 return Tn
             })), a.d(o, "BaseFeedbackErrorComponent", (function() {
                 return Ln
-            })), a.d(o, "FilterDropdown", (function() {
+            })), a.d(o, "CreateNewAction", (function() {
                 return Cn
-            })), a.d(o, "FilterScore", (function() {
+            })), a.d(o, "GlobalActions", (function() {
                 return An
-            })), a.d(o, "FilterUncoveredByRules", (function() {
+            })), a.d(o, "ValidateDiscardAction", (function() {
                 return jn
-            })), a.d(o, "FiltersArea", (function() {
+            })), a.d(o, "FilterDropdown", (function() {
                 return In
-            })), a.d(o, "FiltersList", (function() {
+            })), a.d(o, "FilterScore", (function() {
                 return En
-            })), a.d(o, "FiltersListEmpty", (function() {
+            })), a.d(o, "FilterUncoveredByRules", (function() {
                 return Nn
-            })), a.d(o, "SearchBar", (function() {
+            })), a.d(o, "FiltersArea", (function() {
                 return Fn
-            })), a.d(o, "SelectFilter", (function() {
+            })), a.d(o, "FiltersList", (function() {
                 return Dn
-            })), a.d(o, "SelectOptions", (function() {
+            })), a.d(o, "FiltersListEmpty", (function() {
                 return Pn
-            })), a.d(o, "SelectOptionsSearch", (function() {
+            })), a.d(o, "SearchBar", (function() {
                 return Bn
-            })), a.d(o, "SortFilter", (function() {
+            })), a.d(o, "SelectFilter", (function() {
                 return Mn
-            })), a.d(o, "SortList", (function() {
+            })), a.d(o, "SelectOptions", (function() {
                 return $n
-            })), a.d(o, "CreateNewAction", (function() {
+            })), a.d(o, "SelectOptionsSearch", (function() {
                 return Un
-            })), a.d(o, "GlobalActions", (function() {
+            })), a.d(o, "SortFilter", (function() {
                 return qn
-            })), a.d(o, "ValidateDiscardAction", (function() {
+            })), a.d(o, "SortList", (function() {
                 return Hn
             })), a.d(o, "DatasetSettingsIconFeedbackTaskComponent", (function() {
                 return Vn
             })), a.d(o, "HeaderFeedbackTaskComponent", (function() {
                 return zn
             })), a.d(o, "HelpInfo", (function() {
                 return Wn
@@ -10038,19 +10038,19 @@
                 return Hr
             })), a.d(o, "TextClassificationBulkAnnotationSingle", (function() {
                 return Vr
             })), a.d(o, "ClassifierAnnotationArea", (function() {
                 return zr
             })), a.d(o, "ClassifierAnnotationButton", (function() {
                 return Wr
-            })), a.d(o, "FilterSimilarity", (function() {
-                return Gr
             })), a.d(o, "BulkAnnotationComponent", (function() {
-                return Qr
+                return Gr
             })), a.d(o, "BulkAnnotationFormComponent", (function() {
+                return Qr
+            })), a.d(o, "FilterSimilarity", (function() {
                 return Yr
             })), a.d(o, "HelpInfoExplain", (function() {
                 return Kr
             })), a.d(o, "HelpInfoSimilarity", (function() {
                 return Xr
             })), a.d(o, "UserTokenComponent", (function() {
                 return Jr
@@ -11474,89 +11474,89 @@
                     }))
                 },
                 Ln = function BaseFeedbackErrorComponent() {
                     return a.e(50).then(a.bind(null, 1016)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Cn = function FilterDropdown() {
+                Cn = function CreateNewAction() {
+                    return a.e(82).then(a.bind(null, 1615)).then((function(r) {
+                        return wrapFunctional(r.default || r)
+                    }))
+                },
+                An = function GlobalActions() {
+                    return Promise.all([a.e(9), a.e(18), a.e(117)]).then(a.bind(null, 1342)).then((function(r) {
+                        return wrapFunctional(r.default || r)
+                    }))
+                },
+                jn = function ValidateDiscardAction() {
+                    return Promise.all([a.e(9), a.e(18)]).then(a.bind(null, 1439)).then((function(r) {
+                        return wrapFunctional(r.default || r)
+                    }))
+                },
+                In = function FilterDropdown() {
                     return a.e(107).then(a.bind(null, 1165)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                An = function FilterScore() {
+                En = function FilterScore() {
                     return Promise.all([a.e(28), a.e(108)]).then(a.bind(null, 1799)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                jn = function FilterUncoveredByRules() {
+                Nn = function FilterUncoveredByRules() {
                     return a.e(111).then(a.bind(null, 1800)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                In = function FiltersArea() {
+                Fn = function FiltersArea() {
                     return Promise.all([a.e(15), a.e(17), a.e(112)]).then(a.bind(null, 1341)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                En = function FiltersList() {
+                Dn = function FiltersList() {
                     return a.e(113).then(a.bind(null, 1282)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Nn = function FiltersListEmpty() {
+                Pn = function FiltersListEmpty() {
                     return a.e(114).then(a.bind(null, 1801)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Fn = function SearchBar() {
+                Bn = function SearchBar() {
                     return a.e(17).then(a.bind(null, 1437)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Dn = function SelectFilter() {
+                Mn = function SelectFilter() {
                     return a.e(181).then(a.bind(null, 1802)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Pn = function SelectOptions() {
+                $n = function SelectOptions() {
                     return a.e(182).then(a.bind(null, 1336)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Bn = function SelectOptionsSearch() {
+                Un = function SelectOptionsSearch() {
                     return a.e(183).then(a.bind(null, 1164)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Mn = function SortFilter() {
+                qn = function SortFilter() {
                     return a.e(35).then(a.bind(null, 1752)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                $n = function SortList() {
+                Hn = function SortList() {
                     return Promise.all([a.e(35), a.e(217)]).then(a.bind(null, 1803)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Un = function CreateNewAction() {
-                    return a.e(82).then(a.bind(null, 1615)).then((function(r) {
-                        return wrapFunctional(r.default || r)
-                    }))
-                },
-                qn = function GlobalActions() {
-                    return Promise.all([a.e(9), a.e(18), a.e(117)]).then(a.bind(null, 1342)).then((function(r) {
-                        return wrapFunctional(r.default || r)
-                    }))
-                },
-                Hn = function ValidateDiscardAction() {
-                    return Promise.all([a.e(9), a.e(18)]).then(a.bind(null, 1439)).then((function(r) {
-                        return wrapFunctional(r.default || r)
-                    }))
-                },
                 Vn = function DatasetSettingsIconFeedbackTaskComponent() {
                     return a.e(86).then(a.bind(null, 1430)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
                 zn = function HeaderFeedbackTaskComponent() {
                     return Promise.all([a.e(25), a.e(118)]).then(a.bind(null, 1429)).then((function(r) {
@@ -11834,26 +11834,26 @@
                     }))
                 },
                 Wr = function ClassifierAnnotationButton() {
                     return a.e(79).then(a.bind(null, 796)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Gr = function FilterSimilarity() {
-                    return a.e(109).then(a.bind(null, 1283)).then((function(r) {
+                Gr = function BulkAnnotationComponent() {
+                    return a.e(9).then(a.bind(null, 1622)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Qr = function BulkAnnotationComponent() {
-                    return a.e(9).then(a.bind(null, 1622)).then((function(r) {
+                Qr = function BulkAnnotationFormComponent() {
+                    return a.e(76).then(a.bind(null, 1623)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
-                Yr = function BulkAnnotationFormComponent() {
-                    return a.e(76).then(a.bind(null, 1623)).then((function(r) {
+                Yr = function FilterSimilarity() {
+                    return a.e(109).then(a.bind(null, 1283)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
                 },
                 Kr = function HelpInfoExplain() {
                     return a.e(120).then(a.bind(null, 1805)).then((function(r) {
                         return wrapFunctional(r.default || r)
                     }))
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b21e71c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b21e71c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b28cfbc.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b28cfbc.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b2f22c5.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b2f22c5.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b2fc075.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b2fc075.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b4c1d0d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b4c1d0d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b53ca3b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b53ca3b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b5b4aae.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b5b4aae.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b6ffaa9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b6ffaa9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b781657.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b781657.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b804ce5.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b804ce5.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b8c421d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b8c421d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/b955150.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/b955150.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bad085e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bad085e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bad26d7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bad26d7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bd7cb12.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bd7cb12.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bdf5c09.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bdf5c09.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/beccc06.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/beccc06.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bedb2dd.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bedb2dd.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bef1a27.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bef1a27.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/bf6bced.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/bf6bced.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c02ad86.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c02ad86.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c26b3ec.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c26b3ec.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c380661.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c380661.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c5ba452.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c5ba452.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c5dda82.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c5dda82.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c606e8c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c606e8c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c615699.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c615699.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c72e4ee.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c72e4ee.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c863a84.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c863a84.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/c9f74e7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/c9f74e7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/ca0d950.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ca0d950.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cba5c90.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cba5c90.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cc5cbbe.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cc5cbbe.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cd3d6f6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cd3d6f6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cd61b37.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cd61b37.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cdeab7c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cdeab7c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cf435aa.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cf435aa.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/cf5d4e8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/cf5d4e8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d3b25ba.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d3b25ba.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d3ec09a.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d3ec09a.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d6044c6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d6044c6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d8454ea.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d8454ea.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d8c7cdd.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d8c7cdd.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d95f66b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d95f66b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/d9f709f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/d9f709f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/da56dc9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/da56dc9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/da98642.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/da98642.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/dae7b34.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/dae7b34.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/de51b34.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/de51b34.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/df05a2c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/df05a2c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/df0702e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/df0702e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/dfb4e3d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/dfb4e3d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e1fa0db.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e1fa0db.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e208f0f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e208f0f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e23db67.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e23db67.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e2678f8.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e2678f8.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e311004.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e311004.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e31b663.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e31b663.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e3fe598.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e3fe598.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e44b050.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e44b050.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e4c5fa4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e4c5fa4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e4cf190.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e4cf190.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e4f9f5b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e4f9f5b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e63dbd4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e63dbd4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e7035e6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e7035e6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e79118e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e79118e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e79cf5b.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e79cf5b.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e7e5f43.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e7e5f43.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e8142c4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e8142c4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e8e19b2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e8e19b2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/e901328.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/e901328.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/ea525f4.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/ea525f4.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/eb1faf3.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/eb1faf3.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/edd702e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/edd702e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/efe6a6f.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/efe6a6f.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f03fccb.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f03fccb.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f0a6dd7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f0a6dd7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f14f26d.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f14f26d.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f217920.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f217920.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f36addc.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f36addc.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f3b5d22.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f3b5d22.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f3eb9f7.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f3eb9f7.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f3f39b2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f3f39b2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f409abc.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f409abc.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f41b1df.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f41b1df.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f66f192.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f66f192.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f6c0467.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f6c0467.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f7afca5.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f7afca5.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f86ebc2.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f86ebc2.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/f947aa0.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/f947aa0.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fa7f8a6.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fa7f8a6.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fa9e6f9.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fa9e6f9.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fd39885.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fd39885.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fd59c1c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fd59c1c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fd65964.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fd65964.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fdf390c.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fdf390c.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fe8b19e.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fe8b19e.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fec21cc.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fec21cc.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fefbfff.js` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fefbfff.js`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.3c074ae.woff2` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.3c074ae.woff2`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.f7cfb4c.woff` & `argilla_server-1.29.0rc1/src/argilla_server/static/_nuxt/fonts/raptorv2premium-bold-webfont.f7cfb4c.woff`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/apple-touch-icon.png` & `argilla_server-1.29.0rc1/src/argilla_server/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/datasets/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/datasets/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/datasets/useDatasetsViewModel/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/datasets/useDatasetsViewModel/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/favicon-16x16.png` & `argilla_server-1.29.0rc1/src/argilla_server/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/favicon-32x32.png` & `argilla_server-1.29.0rc1/src/argilla_server/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/favicon.ico` & `argilla_server-1.29.0rc1/src/argilla_server/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/bulk-mode.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/bulk-mode.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/change-height.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/change-height.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/clear.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/clear.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/close.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/close.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/code.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/code.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/danger.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/danger.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/discard.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/discard.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/draggable.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/draggable.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/exploration.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/exploration.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/filter.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/filter.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/hand-labeling.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/hand-labeling.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/info.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/info.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/kebab.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/kebab.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/link.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/link.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/log-out.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/log-out.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/matching.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/matching.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/meatballs.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/meatballs.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/no-matching.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/no-matching.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/pen.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/pen.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/progress.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/progress.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/refresh.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/reset.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/row-last.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/row-last.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/search.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/search.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/settings.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/shortcuts.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/shortcuts.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/similarity.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/similarity.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/smile-sad.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/smile-sad.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/suggestion.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/suggestion.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/support.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/support.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/trash-empty.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/trash-empty.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/unavailable.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/unavailable.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/validate.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/validate.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/icons/weak-labeling.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/icons/weak-labeling.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/images/help-info/explain.png` & `argilla_server-1.29.0rc1/src/argilla_server/static/images/help-info/explain.png`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/images/help-info/similarity.png` & `argilla_server-1.29.0rc1/src/argilla_server/static/images/help-info/similarity.png`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/images/logo.svg` & `argilla_server-1.29.0rc1/src/argilla_server/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/images/welcome-hf-sign-in-ss.png` & `argilla_server-1.29.0rc1/src/argilla_server/static/images/welcome-hf-sign-in-ss.png`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/static/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/sign-in/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/sign-in/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/useWelcomeHFViewModel/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/useWelcomeHFViewModel/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/user-settings/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/user-settings/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static/welcome-hf-sign-in/index.html` & `argilla_server-1.29.0rc1/src/argilla_server/static/welcome-hf-sign-in/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!doctype html>
 <html>
   <head>
-    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/b1c7a5f.js" as="script">
+    <meta data-n-head="1" charset="utf-8"><meta data-n-head="1" name="viewport" content="width=device-width,initial-scale=1"><meta data-n-head="1" data-hid="description" name="description" content=""><title>Argilla</title><link data-n-head="1" rel="icon" type="image/x-icon" href="favicon.ico"><link data-n-head="1" rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png"><link data-n-head="1" rel="icon" sizes="32x32" href="favicon-32x32.png"><link data-n-head="1" rel="icon" sizes="16x16" href="favicon-16x16.png"><link data-n-head="1" rel="manifest" href="site.webmanifest"><base href="@@baseUrl@@/"><link rel="preload" href="@@baseUrl@@/_nuxt/8b30d40.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/d3b25ba.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/3eb41c4.js" as="script"><link rel="preload" href="@@baseUrl@@/_nuxt/85aa264.js" as="script">
   </head>
   <body>
     <div id="__nuxt"><style>#nuxt-loading{background:#fff;visibility:hidden;opacity:0;position:absolute;left:0;right:0;top:0;bottom:0;display:flex;justify-content:center;align-items:center;flex-direction:column;animation:nuxtLoadingIn 10s ease;-webkit-animation:nuxtLoadingIn 10s ease;animation-fill-mode:forwards;overflow:hidden}@keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}@-webkit-keyframes nuxtLoadingIn{0%{visibility:hidden;opacity:0}20%{visibility:visible;opacity:0}100%{visibility:visible;opacity:1}}#nuxt-loading>div,#nuxt-loading>div:after{border-radius:50%;width:5rem;height:5rem}#nuxt-loading>div{font-size:10px;position:relative;text-indent:-9999em;border:.5rem solid #f5f5f5;border-left:.5rem solid #d3d3d3;-webkit-transform:translateZ(0);-ms-transform:translateZ(0);transform:translateZ(0);-webkit-animation:nuxtLoading 1.1s infinite linear;animation:nuxtLoading 1.1s infinite linear}#nuxt-loading.error>div{border-left:.5rem solid #ff4500;animation-duration:5s}@-webkit-keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}@keyframes nuxtLoading{0%{-webkit-transform:rotate(0);transform:rotate(0)}100%{-webkit-transform:rotate(360deg);transform:rotate(360deg)}}</style> <script>window.addEventListener("error",function(){var e=document.getElementById("nuxt-loading");e&&(e.className+=" error")})</script> <div id="nuxt-loading" aria-live="polite" role="status"><div>Loading...</div></div> </div><script>window.__NUXT__={config:{clientVersion:"1.29.0",slackCommunity:"https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g",documentationSite:"https://docs.argilla.io/",documentationSiteQuickStart:"https://docs.argilla.io/en/latest/getting_started/quickstart.html",documentationSiteSemanticSearch:"https://docs.argilla.io/en/latest/reference/webapp/features.html#semantic-search",documentationSiteLabelScheme:"https://docs.argilla.io/en/latest/guides/log_load_and_prepare_data.html#define-a-labeling-schema",documentationSiteQueryDatasets:"https://docs.argilla.io/en/latest/guides/query_datasets.html",documentationPersistentStorage:"https://docs.argilla.io/en/latest/getting_started/installation/deployments/huggingface-spaces.html#setting-up-persistent-storage",_app:{basePath:"@@baseUrl@@/",assetsPath:"@@baseUrl@@/_nuxt/",cdnURL:null}}}</script>
-  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/b1c7a5f.js"></script></body>
+  <script src="@@baseUrl@@/_nuxt/8b30d40.js"></script><script src="@@baseUrl@@/_nuxt/d3b25ba.js"></script><script src="@@baseUrl@@/_nuxt/3eb41c4.js"></script><script src="@@baseUrl@@/_nuxt/85aa264.js"></script></body>
 </html>
```

### Comparing `argilla_server-1.29.0/src/argilla_server/static_rewrite.py` & `argilla_server-1.29.0rc1/src/argilla_server/static_rewrite.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/telemetry.py` & `argilla_server-1.29.0rc1/src/argilla_server/telemetry.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/use_cases/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/use_cases/responses/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/use_cases/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/use_cases/responses/upsert_responses_in_bulk.py` & `argilla_server-1.29.0rc1/src/argilla_server/use_cases/responses/upsert_responses_in_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils/_telemetry.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils/_telemetry.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils/dependency.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils/params.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils/params.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils/span_utils.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils/span_utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/utils/utils.py` & `argilla_server-1.29.0rc1/src/argilla_server/utils/utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/__init__.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/questions.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/records.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/response_values.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/response_values.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/responses.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/responses.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/suggestions.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/src/argilla_server/validators/vectors.py` & `argilla_server-1.29.0rc1/src/argilla_server/validators/vectors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/__init__.py` & `argilla_server-1.29.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/conftest.py` & `argilla_server-1.29.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/database.py` & `argilla_server-1.29.0rc1/tests/database.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/factories.py` & `argilla_server-1.29.0rc1/tests/factories.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/pydantic_v1/__init__.py` & `argilla_server-1.29.0rc1/tests/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/pydantic_v1/generics.py` & `argilla_server-1.29.0rc1/tests/pydantic_v1/generics.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/pydantic_v1/utils.py` & `argilla_server-1.29.0rc1/tests/pydantic_v1/utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/test_docs.py` & `argilla_server-1.29.0rc1/tests/unit/api/test_docs.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/test_not_found_routes.py` & `argilla_server-1.29.0rc1/tests/unit/api/test_not_found_routes.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_authentication.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_authentication.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_datasets.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_info.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_info.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_metrics.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_metrics.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_records_get.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_records_get.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_records_update.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_records_update.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_security_token.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_security_token.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_text2text.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_text2text.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_text_classification.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_text_classification_api_rules.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_text_classification_api_rules.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_text_classification_dataset_settings.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_text_classification_dataset_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_token_classification.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_token_classification_dataset_settings.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_token_classification_dataset_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_users.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v0/test_workspaces.py` & `argilla_server-1.29.0rc1/tests/unit/api/v0/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/authentication/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/authentication/test_create_token.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/authentication/test_create_token.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/questions/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/questions/test_create_dataset_question.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/questions/test_create_dataset_question.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/questions/test_list_dataset_questions.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/questions/test_list_dataset_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_responses.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_responses.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_suggestions.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_vectors.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/records_bulk/test_dataset_records_bulk_with_vectors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/test_create_dataset_records.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/test_create_dataset_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/records/test_update_dataset_records.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/records/test_update_dataset_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_create_dataset_question.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_create_dataset_question.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_create_dataset_vector_settings.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_create_dataset_vector_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_get_dataset_progress.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_get_dataset_progress.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_list_dataset_records_search_suggestions_options.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_list_dataset_records_search_suggestions_options.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_questions.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_search_current_user_dataset_records.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_search_current_user_dataset_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/datasets/test_search_dataset_records.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/datasets/test_search_dataset_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/info/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/info/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/info/test_get_status.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/info/test_get_status.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/info/test_get_version.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/info/test_get_version.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/questions/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/questions/test_update_question.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/questions/test_update_question.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/records/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/records/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/records/test_create_record_response.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/records/test_create_record_response.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/records/test_upsert_suggestion.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/records/test_upsert_suggestion.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/responses/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/responses/test_create_current_user_responses_bulk.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/responses/test_create_current_user_responses_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/responses/test_update_response.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/responses/test_update_response.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/settings/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/settings/test_get_settings.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/settings/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_datasets.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_fields.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_fields.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_list_dataset_records.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_list_dataset_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_metadata_properties.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_metadata_properties.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_oauth2.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_questions.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_questions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_records.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_responses.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_responses.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_suggestions.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_users.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_vectors_settings.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_vectors_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/test_workspaces.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/users/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/users/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/users/test_create_user.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_create_user.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/users/test_delete_user.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_delete_user.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/users/test_get_current_user.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_get_current_user.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/users/test_get_user.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_get_user.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/users/test_list_users.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/users/test_list_users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/workspaces/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_create_workspace.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_create_workspace.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_create_workspace_user.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_create_workspace_user.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_delete_workspace_user.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_delete_workspace_user.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/api/v1/workspaces/test_list_workspace_users.py` & `argilla_server-1.29.0rc1/tests/unit/api/v1/workspaces/test_list_workspace_users.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/conftest.py` & `argilla_server-1.29.0rc1/tests/unit/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/conftest.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/test_create.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_create.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/test_create_default.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_create_default.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/test_migrate.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_migrate.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/test_update.py` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_update.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/database/users/test_user_files/users.yml` & `argilla_server-1.29.0rc1/tests/unit/cli/database/users/test_user_files/users.yml`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/search_engine/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/cli/search_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/search_engine/conftest.py` & `argilla_server-1.29.0rc1/tests/unit/cli/search_engine/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/search_engine/test_reindex.py` & `argilla_server-1.29.0rc1/tests/unit/cli/search_engine/test_reindex.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/cli/test_start.py` & `argilla_server-1.29.0rc1/tests/unit/cli/test_start.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/commons/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/commons/test_records_dao.py` & `argilla_server-1.29.0rc1/tests/unit/commons/test_records_dao.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/commons/test_settings.py` & `argilla_server-1.29.0rc1/tests/unit/commons/test_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/commons/test_telemetry.py` & `argilla_server-1.29.0rc1/tests/unit/commons/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/conftest.py` & `argilla_server-1.29.0rc1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/contexts/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/contexts/search/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/contexts/search/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/contexts/search/test_search_records_query_validator.py` & `argilla_server-1.29.0rc1/tests/unit/contexts/search/test_search_records_query_validator.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/daos/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/backend/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/daos/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/backend/test_es_client.py` & `argilla_server-1.29.0rc1/tests/unit/daos/backend/test_es_client.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/backend/test_generic_elastic_engine.py` & `argilla_server-1.29.0rc1/tests/unit/daos/backend/test_generic_elastic_engine.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/backend/test_query_builder.py` & `argilla_server-1.29.0rc1/tests/unit/daos/backend/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/models/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/daos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/models/test_records.py` & `argilla_server-1.29.0rc1/tests/unit/daos/models/test_records.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/daos/test_datasets.py` & `argilla_server-1.29.0rc1/tests/unit/daos/test_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/errors/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/errors/test_api_errors.py` & `argilla_server-1.29.0rc1/tests/unit/errors/test_api_errors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/errors/test_errors.py` & `argilla_server-1.29.0rc1/tests/unit/errors/test_errors.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/old_models/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/models/old_models/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/old_models/test_datasets.py` & `argilla_server-1.29.0rc1/tests/unit/models/old_models/test_datasets.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/old_models/test_text2text.py` & `argilla_server-1.29.0rc1/tests/unit/models/old_models/test_text2text.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/old_models/test_text_classification.py` & `argilla_server-1.29.0rc1/tests/unit/models/old_models/test_text_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/old_models/test_token_classification.py` & `argilla_server-1.29.0rc1/tests/unit/models/old_models/test_token_classification.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/models/test_base.py` & `argilla_server-1.29.0rc1/tests/unit/models/test_base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/schemas/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/schemas/test_base.py` & `argilla_server-1.29.0rc1/tests/unit/schemas/test_base.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/schemas/v1/responses/test_response_value_create.py` & `argilla_server-1.29.0rc1/tests/unit/schemas/v1/responses/test_response_value_create.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/search_engine/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/search_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/search_engine/conftest.py` & `argilla_server-1.29.0rc1/tests/unit/search_engine/conftest.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/search_engine/test_commons.py` & `argilla_server-1.29.0rc1/tests/unit/search_engine/test_commons.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/search_engine/test_elastisearch.py` & `argilla_server-1.29.0rc1/tests/unit/search_engine/test_elastisearch.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/search_engine/test_opensearch.py` & `argilla_server-1.29.0rc1/tests/unit/search_engine/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/security/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/security/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/security/authentication/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/security/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/security/authentication/oauth2/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/security/authentication/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/security/authentication/oauth2/test_settings.py` & `argilla_server-1.29.0rc1/tests/unit/security/authentication/oauth2/test_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/security/test_model.py` & `argilla_server-1.29.0rc1/tests/unit/security/test_model.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/security/test_settings.py` & `argilla_server-1.29.0rc1/tests/unit/security/test_settings.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/test_app.py` & `argilla_server-1.29.0rc1/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/test_logging.py` & `argilla_server-1.29.0rc1/tests/unit/test_logging.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/test_utils.py` & `argilla_server-1.29.0rc1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/utils/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/utils/test_dependency.py` & `argilla_server-1.29.0rc1/tests/unit/utils/test_dependency.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/utils/test_span_utils.py` & `argilla_server-1.29.0rc1/tests/unit/utils/test_span_utils.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/validators/__init__.py` & `argilla_server-1.29.0rc1/tests/unit/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/tests/unit/validators/test_records_bulk.py` & `argilla_server-1.29.0rc1/tests/unit/validators/test_records_bulk.py`

 * *Files identical despite different names*

### Comparing `argilla_server-1.29.0/PKG-INFO` & `argilla_server-1.29.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argilla-server
-Version: 1.29.0
+Version: 1.29.0rc1
 Summary: Open-source tool for exploring, labeling, and monitoring data for NLP projects.
 Keywords: data-science,natural-language-processing,text-labeling,data-annotation,artificial-intelligence,knowledged-graph,developers-tools,human-in-the-loop,mlops
 Home-page: https://www.argilla.io
 Author-Email: argilla <contact@argilla.io>
 Maintainer-Email: argilla <contact@argilla.io>
 License: Apache-2.0
 Project-URL: Homepage, https://www.argilla.io
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_4hcr9avn_/tmpw5c73534_TarContainer/0/790", line 50, column 96: Levels of opening and closing headings don't match*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: argilla-server Version: 1.29.0 Summary: Open-source
-tool for exploring, labeling, and monitoring data for NLP projects. Keywords:
-data-science,natural-language-processing,text-labeling,data-
+Metadata-Version: 2.1 Name: argilla-server Version: 1.29.0rc1 Summary: Open-
+source tool for exploring, labeling, and monitoring data for NLP projects.
+Keywords: data-science,natural-language-processing,text-labeling,data-
 annotation,artificial-intelligence,knowledged-graph,developers-tools,human-in-
 the-loop,mlops Home-page: https://www.argilla.io Author-Email: argilla
 argilla.io> Maintainer-Email: argilla
 argilla.io> License: Apache-2.0 Project-URL: Homepage, https://www.argilla.io
 Project-URL: Documentation, https://docs.argilla.io Project-URL: Repository,
 https://github.com/argilla-io/argilla Requires-Python: <3.11,>=3.8 Requires-
 Dist: fastapi<1.0.0,>=0.103.1 Requires-Dist: pydantic<2.0,>=1.10.7 Requires-
```

