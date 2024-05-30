# Comparing `tmp/castor_extractor-0.9.0.tar.gz` & `tmp/castor_extractor-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castor_extractor-0.9.0.tar", max compression
+gzip compressed data, was "castor_extractor-0.9.2.tar", max compression
```

## Comparing `castor_extractor-0.9.0.tar` & `castor_extractor-0.9.2.tar`

### file list

```diff
@@ -1,292 +1,293 @@
--rw-r--r--   0        0        0     7105 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     8254 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/LICENCE
--rw-r--r--   0        0        0     3423 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.446658 castor_extractor-0.9.0/castor_extractor/__init__.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.446658 castor_extractor-0.9.0/castor_extractor/commands/__init__.py
--rw-r--r--   0        0        0     1269 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_bigquery.py
--rw-r--r--   0        0        0     1208 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_domo.py
--rwxr-xr-x   0        0        0     1725 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_looker.py
--rwxr-xr-x   0        0        0      778 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_metabase_api.py
--rwxr-xr-x   0        0        0     1269 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_metabase_db.py
--rwxr-xr-x   0        0        0      953 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_mode.py
--rw-r--r--   0        0        0     1154 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_postgres.py
--rw-r--r--   0        0        0      875 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_powerbi.py
--rw-r--r--   0        0        0      989 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_qlik.py
--rwxr-xr-x   0        0        0     1155 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_redshift.py
--rw-r--r--   0        0        0      703 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_sigma.py
--rwxr-xr-x   0        0        0     1982 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_snowflake.py
--rwxr-xr-x   0        0        0     1415 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/extract_tableau.py
--rw-r--r--   0        0        0     2684 2023-11-22 14:41:15.303660 castor_extractor-0.9.0/castor_extractor/commands/file_check.py
--rwxr-xr-x   0        0        0     1956 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/commands/upload.py
--rw-r--r--   0        0        0      119 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/__init__.py
--rw-r--r--   0        0        0     3097 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/column.py
--rw-r--r--   0        0        0     1935 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/column_test.py
--rw-r--r--   0        0        0      289 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/constants.py
--rw-r--r--   0        0        0      536 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/enums.py
--rw-r--r--   0        0        0     6537 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/file.py
--rw-r--r--   0        0        0     2121 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/file_test.py
--rw-r--r--   0        0        0      547 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/file_test_users.csv
--rw-r--r--   0        0        0      286 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/file_test_users_valid.csv
--rw-r--r--   0        0        0       60 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/templates/__init__.py
--rw-r--r--   0        0        0     2977 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/file_checker/templates/generic_warehouse.py
--rw-r--r--   0        0        0     1197 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/logger.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.450658 castor_extractor-0.9.0/castor_extractor/transformation/__init__.py
--rw-r--r--   0        0        0       99 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/transformation/dbt/__init__.py
--rw-r--r--   0        0        0      126 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/transformation/dbt/assets.py
--rw-r--r--   0        0        0       94 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/__init__.py
--rw-r--r--   0        0        0     5508 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/client.py
--rw-r--r--   0        0        0     4030 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/client_test.py
--rw-r--r--   0        0        0      760 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/credentials.py
--rw-r--r--   0        0        0      158 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/types.py
--rw-r--r--   0        0        0       75 2023-11-22 14:41:15.304660 castor_extractor-0.9.0/castor_extractor/uploader/__init__.py
--rw-r--r--   0        0        0      718 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/uploader/constant.py
--rw-r--r--   0        0        0      878 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/uploader/env.py
--rw-r--r--   0        0        0      472 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/uploader/env_test.py
--rw-r--r--   0        0        0     3363 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/uploader/upload.py
--rw-r--r--   0        0        0      328 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/uploader/upload_test.py
--rw-r--r--   0        0        0      478 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/uploader/utils.py
--rw-r--r--   0        0        0     1013 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/__init__.py
--rw-r--r--   0        0        0      417 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/collection.py
--rw-r--r--   0        0        0       39 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/constants.py
--rw-r--r--   0        0        0      817 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/deprecate.py
--rw-r--r--   0        0        0      608 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/env.py
--rw-r--r--   0        0        0     1545 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/files.py
--rw-r--r--   0        0        0     1542 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/files_test.py
--rw-r--r--   0        0        0     4450 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/formatter.py
--rw-r--r--   0        0        0     3802 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/formatter_test.csv
--rw-r--r--   0        0        0    12527 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/formatter_test.json
--rw-r--r--   0        0        0     1542 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/formatter_test.py
--rw-r--r--   0        0        0     2081 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/json_stream_write.py
--rw-r--r--   0        0        0      265 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/load.py
--rw-r--r--   0        0        0     1987 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/object.py
--rw-r--r--   0        0        0     2487 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/object_test.py
--rw-r--r--   0        0        0     3912 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/pager.py
--rw-r--r--   0        0        0     3246 2023-11-22 14:41:15.305660 castor_extractor-0.9.0/castor_extractor/utils/pager_test.py
--rw-r--r--   0        0        0     2627 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/retry.py
--rw-r--r--   0        0        0     1650 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/retry_test.py
--rw-r--r--   0        0        0     1967 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/safe.py
--rw-r--r--   0        0        0     2160 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/safe_test.py
--rw-r--r--   0        0        0     2040 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/store.py
--rw-r--r--   0        0        0     1961 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/string.py
--rw-r--r--   0        0        0     2205 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/string_test.py
--rw-r--r--   0        0        0     1062 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/time.py
--rw-r--r--   0        0        0      168 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/time_test.py
--rw-r--r--   0        0        0      313 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/type.py
--rw-r--r--   0        0        0      150 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/uri.py
--rw-r--r--   0        0        0      259 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/uri_test.py
--rw-r--r--   0        0        0     1913 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/validation.py
--rw-r--r--   0        0        0     1181 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/validation_test.py
--rw-r--r--   0        0        0     2135 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/utils/write.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.451658 castor_extractor-0.9.0/castor_extractor/visualization/__init__.py
--rw-r--r--   0        0        0      127 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/__init__.py
--rw-r--r--   0        0        0      184 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/assets.py
--rw-r--r--   0        0        0       88 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/client/__init__.py
--rw-r--r--   0        0        0     8994 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/client/client.py
--rw-r--r--   0        0        0      583 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/client/client_test.py
--rw-r--r--   0        0        0     1148 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/client/credentials.py
--rw-r--r--   0        0        0     1812 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/client/endpoints.py
--rw-r--r--   0        0        0      565 2023-11-22 14:41:15.306660 castor_extractor-0.9.0/castor_extractor/visualization/domo/client/pagination.py
--rw-r--r--   0        0        0      233 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/domo/constants.py
--rw-r--r--   0        0        0     2567 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/domo/extract.py
--rw-r--r--   0        0        0      235 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/__init__.py
--rw-r--r--   0        0        0      181 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/__init__.py
--rw-r--r--   0        0        0    10076 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/client.py
--rw-r--r--   0        0        0     1868 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/client_test.py
--rw-r--r--   0        0        0     4126 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/constants.py
--rw-r--r--   0        0        0     3553 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/sdk.py
--rw-r--r--   0        0        0     1742 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/sdk_test.py
--rw-r--r--   0        0        0     1315 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/api/utils.py
--rw-r--r--   0        0        0      442 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/assets.py
--rw-r--r--   0        0        0      732 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/constant.py
--rw-r--r--   0        0        0     1174 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/env.py
--rw-r--r--   0        0        0     5121 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/extract.py
--rw-r--r--   0        0        0      636 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/fields.py
--rw-r--r--   0        0        0      782 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/fields_test.py
--rw-r--r--   0        0        0     3122 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/multithreading.py
--rw-r--r--   0        0        0     2564 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/looker/parameters.py
--rw-r--r--   0        0        0      125 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/__init__.py
--rw-r--r--   0        0        0     2814 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/assets.py
--rw-r--r--   0        0        0       52 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/__init__.py
--rw-r--r--   0        0        0       30 2023-11-22 14:41:15.307660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/api/__init__.py
--rw-r--r--   0        0        0     5622 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/api/client.py
--rw-r--r--   0        0        0     1348 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/api/credentials.py
--rw-r--r--   0        0        0       29 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/__init__.py
--rw-r--r--   0        0        0     4115 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/client.py
--rw-r--r--   0        0        0     1891 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/credentials.py
--rw-r--r--   0        0        0       76 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
--rw-r--r--   0        0        0       79 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
--rw-r--r--   0        0        0      419 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/card.sql
--rw-r--r--   0        0        0       42 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/collection.sql
--rw-r--r--   0        0        0      439 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
--rw-r--r--   0        0        0       52 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
--rw-r--r--   0        0        0       49 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/database.sql
--rw-r--r--   0        0        0       46 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/table.sql
--rw-r--r--   0        0        0       41 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/queries/user.sql
--rw-r--r--   0        0        0     1076 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/decryption.py
--rw-r--r--   0        0        0      590 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/decryption_test.py
--rw-r--r--   0        0        0      389 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/shared.py
--rw-r--r--   0        0        0     1006 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/errors.py
--rw-r--r--   0        0        0     1777 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/extract.py
--rw-r--r--   0        0        0       45 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/metabase/types.py
--rw-r--r--   0        0        0      117 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/mode/__init__.py
--rw-r--r--   0        0        0     1552 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/mode/assets.py
--rw-r--r--   0        0        0       27 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/mode/client/__init__.py
--rw-r--r--   0        0        0     7820 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/mode/client/client.py
--rw-r--r--   0        0        0     2087 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/mode/client/client_test.json
--rw-r--r--   0        0        0     1424 2023-11-22 14:41:15.308660 castor_extractor-0.9.0/castor_extractor/visualization/mode/client/client_test.py
--rw-r--r--   0        0        0      453 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/mode/client/constants.py
--rw-r--r--   0        0        0     1650 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/mode/client/credentials.py
--rw-r--r--   0        0        0     1495 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/mode/errors.py
--rw-r--r--   0        0        0     1559 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/mode/extract.py
--rw-r--r--   0        0        0      106 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/__init__.py
--rw-r--r--   0        0        0      504 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/assets.py
--rw-r--r--   0        0        0       62 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/__init__.py
--rw-r--r--   0        0        0     2356 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/constants.py
--rw-r--r--   0        0        0      500 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/credentials.py
--rw-r--r--   0        0        0      787 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/credentials_test.py
--rw-r--r--   0        0        0     9500 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/rest.py
--rw-r--r--   0        0        0     7343 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/rest_test.py
--rw-r--r--   0        0        0      541 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/utils.py
--rw-r--r--   0        0        0      719 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/utils_test.py
--rw-r--r--   0        0        0     1328 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/powerbi/extract.py
--rw-r--r--   0        0        0      143 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/__init__.py
--rw-r--r--   0        0        0     1634 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/assets.py
--rw-r--r--   0        0        0       94 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/__init__.py
--rw-r--r--   0        0        0      786 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/constants.py
--rw-r--r--   0        0        0       36 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/__init__.py
--rw-r--r--   0        0        0     2537 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/client.py
--rw-r--r--   0        0        0      707 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/constants.py
--rw-r--r--   0        0        0     1229 2023-11-22 14:41:15.309660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/error.py
--rw-r--r--   0        0        0     1005 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/error_test.py
--rw-r--r--   0        0        0     1411 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/json_rpc.py
--rw-r--r--   0        0        0     1304 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
--rw-r--r--   0        0        0     2032 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/websocket.py
--rw-r--r--   0        0        0     3261 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/master.py
--rw-r--r--   0        0        0     5966 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/rest.py
--rw-r--r--   0        0        0     1684 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/rest_test.py
--rw-r--r--   0        0        0       95 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/constants.py
--rw-r--r--   0        0        0     2397 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/qlik/extract.py
--rw-r--r--   0        0        0      130 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/__init__.py
--rw-r--r--   0        0        0      246 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/assets.py
--rw-r--r--   0        0        0       90 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/__init__.py
--rw-r--r--   0        0        0     6356 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/client.py
--rw-r--r--   0        0        0     1552 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/client_test.py
--rw-r--r--   0        0        0      797 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/credentials.py
--rw-r--r--   0        0        0     1157 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/endpoints.py
--rw-r--r--   0        0        0      667 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/pagination.py
--rw-r--r--   0        0        0      144 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/constants.py
--rw-r--r--   0        0        0     2678 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/sigma/extract.py
--rw-r--r--   0        0        0      114 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/__init__.py
--rw-r--r--   0        0        0      762 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/assets.py
--rw-r--r--   0        0        0       78 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/__init__.py
--rw-r--r--   0        0        0     6861 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/client.py
--rw-r--r--   0        0        0     2094 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/client_utils.py
--rw-r--r--   0        0        0     3386 2023-11-22 14:41:15.310660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/credentials.py
--rw-r--r--   0        0        0      812 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/project.py
--rw-r--r--   0        0        0     2045 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/safe_mode.py
--rw-r--r--   0        0        0      126 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/constants.py
--rw-r--r--   0        0        0       91 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/errors.py
--rw-r--r--   0        0        0     2880 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/extract.py
--rw-r--r--   0        0        0     4732 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/gql_fields.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.464658 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.464658 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/__init__.py
--rw-r--r--   0        0        0      446 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
--rw-r--r--   0        0        0      447 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
--rw-r--r--   0        0        0      450 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
--rw-r--r--   0        0        0     1018 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
--rw-r--r--   0        0        0      679 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
--rw-r--r--   0        0        0     1415 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
--rw-r--r--   0        0        0     1325 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.464658 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
--rw-r--r--   0        0        0     1922 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.464658 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
--rw-r--r--   0        0        0     1173 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
--rw-r--r--   0        0        0      419 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
--rw-r--r--   0        0        0     1779 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
--rw-r--r--   0        0        0     1401 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
--rw-r--r--   0        0        0     1499 2023-11-22 14:41:15.311660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
--rw-r--r--   0        0        0     1979 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
--rw-r--r--   0        0        0       26 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
--rw-r--r--   0        0        0      966 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/tsc_fields.py
--rw-r--r--   0        0        0      322 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/types.py
--rw-r--r--   0        0        0      427 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/visualization/tableau/usage.py
--rw-r--r--   0        0        0        0 2023-11-22 14:41:15.464658 castor_extractor-0.9.0/castor_extractor/warehouse/__init__.py
--rw-r--r--   0        0        0      366 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/__init__.py
--rw-r--r--   0        0        0     1278 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/asset.py
--rw-r--r--   0        0        0     1934 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/client.py
--rw-r--r--   0        0        0     2901 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/extract.py
--rw-r--r--   0        0        0     2632 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/query.py
--rw-r--r--   0        0        0      935 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/time_filter.py
--rw-r--r--   0        0        0      448 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/abstract/time_filter_test.py
--rw-r--r--   0        0        0      125 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/__init__.py
--rw-r--r--   0        0        0     3062 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/client.py
--rw-r--r--   0        0        0     1430 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/client_test.py
--rw-r--r--   0        0        0     2810 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/extract.py
--rw-r--r--   0        0        0       30 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/.sqlfluff
--rw-r--r--   0        0        0     1815 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/column.sql
--rw-r--r--   0        0        0     1454 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
--rw-r--r--   0        0        0      207 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/database.sql
--rw-r--r--   0        0        0      660 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/query.sql
--rw-r--r--   0        0        0      284 2023-11-22 14:41:15.312660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/schema.sql
--rw-r--r--   0        0        0     1508 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/table.sql
--rw-r--r--   0        0        0     2660 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
--rw-r--r--   0        0        0      189 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/user.sql
--rw-r--r--   0        0        0      326 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
--rw-r--r--   0        0        0     4162 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/query.py
--rw-r--r--   0        0        0      140 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/types.py
--rw-r--r--   0        0        0      125 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/__init__.py
--rw-r--r--   0        0        0      871 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/client.py
--rw-r--r--   0        0        0     2131 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/extract.py
--rw-r--r--   0        0        0       30 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/.sqlfluff
--rw-r--r--   0        0        0     1632 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/column.sql
--rw-r--r--   0        0        0      241 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/database.sql
--rw-r--r--   0        0        0      101 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/group.sql
--rw-r--r--   0        0        0      592 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/schema.sql
--rw-r--r--   0        0        0     1489 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/table.sql
--rw-r--r--   0        0        0      170 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/user.sql
--rw-r--r--   0        0        0      540 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/postgres/query.py
--rw-r--r--   0        0        0      125 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/__init__.py
--rw-r--r--   0        0        0      764 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/client.py
--rw-r--r--   0        0        0     1027 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/client_test.py
--rw-r--r--   0        0        0     2270 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/extract.py
--rw-r--r--   0        0        0       30 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/.sqlfluff
--rw-r--r--   0        0        0     7044 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/column.sql
--rw-r--r--   0        0        0      299 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/database.sql
--rw-r--r--   0        0        0      101 2023-11-22 14:41:15.313660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/group.sql
--rw-r--r--   0        0        0     3258 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/query.sql
--rw-r--r--   0        0        0      585 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/schema.sql
--rw-r--r--   0        0        0     2645 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/table.sql
--rw-r--r--   0        0        0      726 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/table_freshness.sql
--rw-r--r--   0        0        0      170 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/user.sql
--rw-r--r--   0        0        0      719 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/view_ddl.sql
--rw-r--r--   0        0        0      540 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/redshift/query.py
--rw-r--r--   0        0        0      128 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/__init__.py
--rw-r--r--   0        0        0     5152 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/client.py
--rw-r--r--   0        0        0     1435 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/client_test.py
--rw-r--r--   0        0        0     2833 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/extract.py
--rw-r--r--   0        0        0       31 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/.sqlfluff
--rw-r--r--   0        0        0     1803 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/column.sql
--rw-r--r--   0        0        0     1179 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
--rw-r--r--   0        0        0      483 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/database.sql
--rw-r--r--   0        0        0      272 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
--rw-r--r--   0        0        0      143 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
--rw-r--r--   0        0        0     1779 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/query.sql
--rw-r--r--   0        0        0       96 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/role.sql
--rw-r--r--   0        0        0      730 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/schema.sql
--rw-r--r--   0        0        0     1378 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/table.sql
--rw-r--r--   0        0        0      570 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/user.sql
--rw-r--r--   0        0        0      673 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
--rw-r--r--   0        0        0     1769 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/query.py
--rw-r--r--   0        0        0       36 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/__init__.py
--rw-r--r--   0        0        0      518 2023-11-22 14:41:15.314660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/extract.py
--rw-r--r--   0        0        0       26 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/.sqlfluff
--rw-r--r--   0        0        0     1392 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/column.sql
--rw-r--r--   0        0        0      138 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/database.sql
--rw-r--r--   0        0        0     1110 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/query.sql
--rw-r--r--   0        0        0      250 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/schema.sql
--rw-r--r--   0        0        0     1049 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/table.sql
--rw-r--r--   0        0        0       67 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/user.sql
--rw-r--r--   0        0        0      249 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/view_ddl.sql
--rw-r--r--   0        0        0     6155 2023-11-22 14:41:15.315660 castor_extractor-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5879 1970-01-01 00:00:00.000000 castor_extractor-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7255 2023-11-27 11:16:15.310237 castor_extractor-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0      303 2023-11-27 11:16:15.310237 castor_extractor-0.9.2/Dockerfile
+-rw-r--r--   0        0        0     8254 2023-11-27 11:16:15.310237 castor_extractor-0.9.2/LICENCE
+-rw-r--r--   0        0        0     3423 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.464220 castor_extractor-0.9.2/castor_extractor/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.464220 castor_extractor-0.9.2/castor_extractor/commands/__init__.py
+-rw-r--r--   0        0        0     1269 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_bigquery.py
+-rw-r--r--   0        0        0     1208 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_domo.py
+-rwxr-xr-x   0        0        0     1483 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_looker.py
+-rwxr-xr-x   0        0        0      778 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_metabase_api.py
+-rwxr-xr-x   0        0        0     1269 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_metabase_db.py
+-rwxr-xr-x   0        0        0      953 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_mode.py
+-rw-r--r--   0        0        0     1154 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_postgres.py
+-rw-r--r--   0        0        0      875 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_powerbi.py
+-rw-r--r--   0        0        0      989 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_qlik.py
+-rwxr-xr-x   0        0        0     1155 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_redshift.py
+-rw-r--r--   0        0        0      703 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_sigma.py
+-rwxr-xr-x   0        0        0     1982 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_snowflake.py
+-rwxr-xr-x   0        0        0     1415 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/extract_tableau.py
+-rw-r--r--   0        0        0     2684 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/file_check.py
+-rwxr-xr-x   0        0        0     1956 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/commands/upload.py
+-rw-r--r--   0        0        0      119 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/__init__.py
+-rw-r--r--   0        0        0     3097 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/column.py
+-rw-r--r--   0        0        0     1935 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/column_test.py
+-rw-r--r--   0        0        0      289 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/constants.py
+-rw-r--r--   0        0        0      536 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/enums.py
+-rw-r--r--   0        0        0     6537 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/file.py
+-rw-r--r--   0        0        0     2121 2023-11-27 11:16:15.311237 castor_extractor-0.9.2/castor_extractor/file_checker/file_test.py
+-rw-r--r--   0        0        0      547 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/file_checker/file_test_users.csv
+-rw-r--r--   0        0        0      286 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/file_checker/file_test_users_valid.csv
+-rw-r--r--   0        0        0       60 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/file_checker/templates/__init__.py
+-rw-r--r--   0        0        0     2977 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/file_checker/templates/generic_warehouse.py
+-rw-r--r--   0        0        0     1197 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/logger.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.465220 castor_extractor-0.9.2/castor_extractor/transformation/__init__.py
+-rw-r--r--   0        0        0       99 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/transformation/dbt/__init__.py
+-rw-r--r--   0        0        0      126 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/transformation/dbt/assets.py
+-rw-r--r--   0        0        0       94 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/__init__.py
+-rw-r--r--   0        0        0     5508 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/client.py
+-rw-r--r--   0        0        0     4030 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/client_test.py
+-rw-r--r--   0        0        0      760 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/credentials.py
+-rw-r--r--   0        0        0      158 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/types.py
+-rw-r--r--   0        0        0       75 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/__init__.py
+-rw-r--r--   0        0        0      718 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/constant.py
+-rw-r--r--   0        0        0      878 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/env.py
+-rw-r--r--   0        0        0      472 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/env_test.py
+-rw-r--r--   0        0        0     3363 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/upload.py
+-rw-r--r--   0        0        0      328 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/upload_test.py
+-rw-r--r--   0        0        0      478 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/uploader/utils.py
+-rw-r--r--   0        0        0     1013 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/utils/__init__.py
+-rw-r--r--   0        0        0      417 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/utils/collection.py
+-rw-r--r--   0        0        0       39 2023-11-27 11:16:15.312237 castor_extractor-0.9.2/castor_extractor/utils/constants.py
+-rw-r--r--   0        0        0      817 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/deprecate.py
+-rw-r--r--   0        0        0      608 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/env.py
+-rw-r--r--   0        0        0     1545 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/files.py
+-rw-r--r--   0        0        0     1542 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/files_test.py
+-rw-r--r--   0        0        0     4450 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/formatter.py
+-rw-r--r--   0        0        0     3802 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/formatter_test.csv
+-rw-r--r--   0        0        0    12527 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/formatter_test.json
+-rw-r--r--   0        0        0     1542 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/formatter_test.py
+-rw-r--r--   0        0        0     2081 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/json_stream_write.py
+-rw-r--r--   0        0        0      265 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/load.py
+-rw-r--r--   0        0        0     1987 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/object.py
+-rw-r--r--   0        0        0     2487 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/object_test.py
+-rw-r--r--   0        0        0     3912 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/pager.py
+-rw-r--r--   0        0        0     3246 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/pager_test.py
+-rw-r--r--   0        0        0     2627 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/retry.py
+-rw-r--r--   0        0        0     1650 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/retry_test.py
+-rw-r--r--   0        0        0     1967 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/safe.py
+-rw-r--r--   0        0        0     2160 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/safe_test.py
+-rw-r--r--   0        0        0     2040 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/store.py
+-rw-r--r--   0        0        0     1961 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/string.py
+-rw-r--r--   0        0        0     2205 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/string_test.py
+-rw-r--r--   0        0        0     1062 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/time.py
+-rw-r--r--   0        0        0      168 2023-11-27 11:16:15.313237 castor_extractor-0.9.2/castor_extractor/utils/time_test.py
+-rw-r--r--   0        0        0      313 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/utils/type.py
+-rw-r--r--   0        0        0      150 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/utils/uri.py
+-rw-r--r--   0        0        0      259 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/utils/uri_test.py
+-rw-r--r--   0        0        0     1913 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/utils/validation.py
+-rw-r--r--   0        0        0     1181 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/utils/validation_test.py
+-rw-r--r--   0        0        0     2135 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/utils/write.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.468219 castor_extractor-0.9.2/castor_extractor/visualization/__init__.py
+-rw-r--r--   0        0        0      127 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/__init__.py
+-rw-r--r--   0        0        0      184 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/assets.py
+-rw-r--r--   0        0        0       88 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/client/__init__.py
+-rw-r--r--   0        0        0     8994 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/client/client.py
+-rw-r--r--   0        0        0      583 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/client/client_test.py
+-rw-r--r--   0        0        0     1148 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/client/credentials.py
+-rw-r--r--   0        0        0     1812 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/client/endpoints.py
+-rw-r--r--   0        0        0      565 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/client/pagination.py
+-rw-r--r--   0        0        0      233 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/constants.py
+-rw-r--r--   0        0        0     2567 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/domo/extract.py
+-rw-r--r--   0        0        0      235 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/looker/__init__.py
+-rw-r--r--   0        0        0      181 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/__init__.py
+-rw-r--r--   0        0        0     9547 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/client.py
+-rw-r--r--   0        0        0     1868 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/client_test.py
+-rw-r--r--   0        0        0     4126 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/constants.py
+-rw-r--r--   0        0        0     3553 2023-11-27 11:16:15.314236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/sdk.py
+-rw-r--r--   0        0        0     1742 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/sdk_test.py
+-rw-r--r--   0        0        0     1315 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/api/utils.py
+-rw-r--r--   0        0        0      442 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/assets.py
+-rw-r--r--   0        0        0      694 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/constant.py
+-rw-r--r--   0        0        0     1174 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/env.py
+-rw-r--r--   0        0        0     5051 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/extract.py
+-rw-r--r--   0        0        0      636 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/fields.py
+-rw-r--r--   0        0        0      782 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/fields_test.py
+-rw-r--r--   0        0        0     3122 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/multithreading.py
+-rw-r--r--   0        0        0     2427 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/looker/parameters.py
+-rw-r--r--   0        0        0      125 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/__init__.py
+-rw-r--r--   0        0        0     2814 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/assets.py
+-rw-r--r--   0        0        0       52 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/__init__.py
+-rw-r--r--   0        0        0       30 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/api/__init__.py
+-rw-r--r--   0        0        0     5622 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/api/client.py
+-rw-r--r--   0        0        0     1348 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/api/credentials.py
+-rw-r--r--   0        0        0       29 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/__init__.py
+-rw-r--r--   0        0        0     4115 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/client.py
+-rw-r--r--   0        0        0     1891 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/credentials.py
+-rw-r--r--   0        0        0       76 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/.sqlfluff
+-rw-r--r--   0        0        0       79 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/base_url.sql
+-rw-r--r--   0        0        0      419 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/card.sql
+-rw-r--r--   0        0        0       42 2023-11-27 11:16:15.315236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/collection.sql
+-rw-r--r--   0        0        0      439 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/dashboard.sql
+-rw-r--r--   0        0        0       52 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/dashboard_cards.sql
+-rw-r--r--   0        0        0       49 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/database.sql
+-rw-r--r--   0        0        0       46 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/table.sql
+-rw-r--r--   0        0        0       41 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/queries/user.sql
+-rw-r--r--   0        0        0     1076 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/decryption.py
+-rw-r--r--   0        0        0      590 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/decryption_test.py
+-rw-r--r--   0        0        0      389 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/shared.py
+-rw-r--r--   0        0        0     1006 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/errors.py
+-rw-r--r--   0        0        0     1777 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/extract.py
+-rw-r--r--   0        0        0       45 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/metabase/types.py
+-rw-r--r--   0        0        0      117 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/__init__.py
+-rw-r--r--   0        0        0     1552 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/assets.py
+-rw-r--r--   0        0        0       27 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/client/__init__.py
+-rw-r--r--   0        0        0     7820 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/client/client.py
+-rw-r--r--   0        0        0     2087 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/client/client_test.json
+-rw-r--r--   0        0        0     1424 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/client/client_test.py
+-rw-r--r--   0        0        0      453 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/client/constants.py
+-rw-r--r--   0        0        0     1650 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/client/credentials.py
+-rw-r--r--   0        0        0     1495 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/errors.py
+-rw-r--r--   0        0        0     1559 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/mode/extract.py
+-rw-r--r--   0        0        0      106 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/__init__.py
+-rw-r--r--   0        0        0      504 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/assets.py
+-rw-r--r--   0        0        0       62 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/__init__.py
+-rw-r--r--   0        0        0     2356 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/constants.py
+-rw-r--r--   0        0        0      500 2023-11-27 11:16:15.316236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/credentials.py
+-rw-r--r--   0        0        0      787 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/credentials_test.py
+-rw-r--r--   0        0        0     9500 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/rest.py
+-rw-r--r--   0        0        0     7343 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/rest_test.py
+-rw-r--r--   0        0        0      541 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/utils.py
+-rw-r--r--   0        0        0      719 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/utils_test.py
+-rw-r--r--   0        0        0     1328 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/powerbi/extract.py
+-rw-r--r--   0        0        0      143 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/__init__.py
+-rw-r--r--   0        0        0     1634 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/assets.py
+-rw-r--r--   0        0        0       94 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/__init__.py
+-rw-r--r--   0        0        0      786 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/constants.py
+-rw-r--r--   0        0        0       36 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/__init__.py
+-rw-r--r--   0        0        0     2537 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/client.py
+-rw-r--r--   0        0        0      707 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/constants.py
+-rw-r--r--   0        0        0     1229 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/error.py
+-rw-r--r--   0        0        0     1005 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/error_test.py
+-rw-r--r--   0        0        0     1411 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/json_rpc.py
+-rw-r--r--   0        0        0     1304 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py
+-rw-r--r--   0        0        0     2032 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/websocket.py
+-rw-r--r--   0        0        0     3261 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/master.py
+-rw-r--r--   0        0        0     5966 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/rest.py
+-rw-r--r--   0        0        0     1684 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/rest_test.py
+-rw-r--r--   0        0        0       95 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/constants.py
+-rw-r--r--   0        0        0     2397 2023-11-27 11:16:15.317236 castor_extractor-0.9.2/castor_extractor/visualization/qlik/extract.py
+-rw-r--r--   0        0        0      130 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/__init__.py
+-rw-r--r--   0        0        0      246 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/assets.py
+-rw-r--r--   0        0        0       90 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/__init__.py
+-rw-r--r--   0        0        0     6356 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/client.py
+-rw-r--r--   0        0        0     1552 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/client_test.py
+-rw-r--r--   0        0        0      797 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/credentials.py
+-rw-r--r--   0        0        0     1157 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/endpoints.py
+-rw-r--r--   0        0        0      667 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/pagination.py
+-rw-r--r--   0        0        0      144 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/constants.py
+-rw-r--r--   0        0        0     2678 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/sigma/extract.py
+-rw-r--r--   0        0        0      114 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/__init__.py
+-rw-r--r--   0        0        0      762 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/assets.py
+-rw-r--r--   0        0        0       78 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/__init__.py
+-rw-r--r--   0        0        0     6861 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/client.py
+-rw-r--r--   0        0        0     2094 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/client_utils.py
+-rw-r--r--   0        0        0     3386 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/credentials.py
+-rw-r--r--   0        0        0      812 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/project.py
+-rw-r--r--   0        0        0     2045 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/safe_mode.py
+-rw-r--r--   0        0        0      126 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/constants.py
+-rw-r--r--   0        0        0       91 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/errors.py
+-rw-r--r--   0        0        0     2880 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/extract.py
+-rw-r--r--   0        0        0     4732 2023-11-27 11:16:15.318236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/gql_fields.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.476218 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.476218 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/__init__.py
+-rw-r--r--   0        0        0      446 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_1_get.json
+-rw-r--r--   0        0        0      447 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/graphql/metadata/metadata_2_get.json
+-rw-r--r--   0        0        0      450 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/auth.xml
+-rw-r--r--   0        0        0     1018 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml
+-rw-r--r--   0        0        0      679 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml
+-rw-r--r--   0        0        0     1415 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml
+-rw-r--r--   0        0        0     1325 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.477218 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/graphql/__init__.py
+-rw-r--r--   0        0        0     1922 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.477218 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/__init__.py
+-rw-r--r--   0        0        0     1173 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py
+-rw-r--r--   0        0        0      419 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/credentials_test.py
+-rw-r--r--   0        0        0     1779 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py
+-rw-r--r--   0        0        0     1401 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py
+-rw-r--r--   0        0        0     1499 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py
+-rw-r--r--   0        0        0     1979 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py
+-rw-r--r--   0        0        0       26 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/utils/env_key.py
+-rw-r--r--   0        0        0      966 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/tsc_fields.py
+-rw-r--r--   0        0        0      322 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/types.py
+-rw-r--r--   0        0        0      427 2023-11-27 11:16:15.319236 castor_extractor-0.9.2/castor_extractor/visualization/tableau/usage.py
+-rw-r--r--   0        0        0        0 2023-11-27 11:16:15.477218 castor_extractor-0.9.2/castor_extractor/warehouse/__init__.py
+-rw-r--r--   0        0        0      366 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/__init__.py
+-rw-r--r--   0        0        0     1278 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/asset.py
+-rw-r--r--   0        0        0     1934 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/client.py
+-rw-r--r--   0        0        0     2901 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/extract.py
+-rw-r--r--   0        0        0     2632 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/query.py
+-rw-r--r--   0        0        0      935 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/time_filter.py
+-rw-r--r--   0        0        0      448 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/abstract/time_filter_test.py
+-rw-r--r--   0        0        0      125 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/__init__.py
+-rw-r--r--   0        0        0     3062 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/client.py
+-rw-r--r--   0        0        0     1430 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/client_test.py
+-rw-r--r--   0        0        0     2810 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/extract.py
+-rw-r--r--   0        0        0       30 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/.sqlfluff
+-rw-r--r--   0        0        0     1815 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/column.sql
+-rw-r--r--   0        0        0     1454 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql
+-rw-r--r--   0        0        0      207 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/database.sql
+-rw-r--r--   0        0        0      660 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/query.sql
+-rw-r--r--   0        0        0      284 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/schema.sql
+-rw-r--r--   0        0        0     1508 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/table.sql
+-rw-r--r--   0        0        0     2660 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql
+-rw-r--r--   0        0        0      189 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/user.sql
+-rw-r--r--   0        0        0      326 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/view_ddl.sql
+-rw-r--r--   0        0        0     4162 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/query.py
+-rw-r--r--   0        0        0      140 2023-11-27 11:16:15.320236 castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/types.py
+-rw-r--r--   0        0        0      125 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/__init__.py
+-rw-r--r--   0        0        0      871 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/client.py
+-rw-r--r--   0        0        0     2131 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/extract.py
+-rw-r--r--   0        0        0       30 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/.sqlfluff
+-rw-r--r--   0        0        0     1632 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/column.sql
+-rw-r--r--   0        0        0      241 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/group.sql
+-rw-r--r--   0        0        0      592 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/schema.sql
+-rw-r--r--   0        0        0     1489 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/table.sql
+-rw-r--r--   0        0        0      170 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/user.sql
+-rw-r--r--   0        0        0      540 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/postgres/query.py
+-rw-r--r--   0        0        0      125 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/__init__.py
+-rw-r--r--   0        0        0      764 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/client.py
+-rw-r--r--   0        0        0     1027 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/client_test.py
+-rw-r--r--   0        0        0     2270 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/extract.py
+-rw-r--r--   0        0        0       30 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/.sqlfluff
+-rw-r--r--   0        0        0     7044 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/column.sql
+-rw-r--r--   0        0        0      299 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/database.sql
+-rw-r--r--   0        0        0      101 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/group.sql
+-rw-r--r--   0        0        0     3465 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/query.sql
+-rw-r--r--   0        0        0      585 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/schema.sql
+-rw-r--r--   0        0        0     2645 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/table.sql
+-rw-r--r--   0        0        0      726 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/table_freshness.sql
+-rw-r--r--   0        0        0      170 2023-11-27 11:16:15.321236 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/user.sql
+-rw-r--r--   0        0        0      719 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/view_ddl.sql
+-rw-r--r--   0        0        0      540 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/redshift/query.py
+-rw-r--r--   0        0        0      128 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/__init__.py
+-rw-r--r--   0        0        0     5152 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/client.py
+-rw-r--r--   0        0        0     1435 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/client_test.py
+-rw-r--r--   0        0        0     2833 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/extract.py
+-rw-r--r--   0        0        0       31 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/.sqlfluff
+-rw-r--r--   0        0        0     1803 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/column.sql
+-rw-r--r--   0        0        0     1179 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/column_lineage.sql
+-rw-r--r--   0        0        0      483 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/database.sql
+-rw-r--r--   0        0        0      272 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/grant_to_role.sql
+-rw-r--r--   0        0        0      143 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/grant_to_user.sql
+-rw-r--r--   0        0        0     1779 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/query.sql
+-rw-r--r--   0        0        0       96 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/role.sql
+-rw-r--r--   0        0        0      730 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/schema.sql
+-rw-r--r--   0        0        0     1378 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/table.sql
+-rw-r--r--   0        0        0      570 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/user.sql
+-rw-r--r--   0        0        0      673 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/view_ddl.sql
+-rw-r--r--   0        0        0     1769 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/query.py
+-rw-r--r--   0        0        0       36 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/__init__.py
+-rw-r--r--   0        0        0      518 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/extract.py
+-rw-r--r--   0        0        0       26 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/.sqlfluff
+-rw-r--r--   0        0        0     1392 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/column.sql
+-rw-r--r--   0        0        0      138 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/database.sql
+-rw-r--r--   0        0        0     1110 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/query.sql
+-rw-r--r--   0        0        0      250 2023-11-27 11:16:15.322235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/schema.sql
+-rw-r--r--   0        0        0     1049 2023-11-27 11:16:15.323235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/table.sql
+-rw-r--r--   0        0        0       67 2023-11-27 11:16:15.323235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/user.sql
+-rw-r--r--   0        0        0      249 2023-11-27 11:16:15.323235 castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/view_ddl.sql
+-rw-r--r--   0        0        0     6191 2023-11-27 11:16:15.323235 castor_extractor-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5879 1970-01-01 00:00:00.000000 castor_extractor-0.9.2/PKG-INFO
```

### Comparing `castor_extractor-0.9.0/CHANGELOG.md` & `castor_extractor-0.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 0.9.2 - 2023-11-23
+
+* Looker : remove deprecated all_looks parameter
+
+## 0.9.1 - 2023-11-22
+
+* Redshift : filter out queries exceeding 65535 char
+
 ## 0.9.0 - 2023-11-20
 
 * Snowflake : Add key-pair authentication
 
 ## 0.8.1 - 2023-11-15
 
 * Add a logging option to log to stdout
```

### Comparing `castor_extractor-0.9.0/LICENCE` & `castor_extractor-0.9.2/LICENCE`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/README.md` & `castor_extractor-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_bigquery.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_bigquery.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_domo.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_domo.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_looker.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_looker.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,30 +23,23 @@
     )
     parser.add_argument(
         "--log-to-stdout",
         help="Send all log outputs to stdout instead of stderr",
         action="store_true",
     )
 
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
-        "--all-looks",
-        help="Use all_looks endpoint instead of the paginated search_looks",
-        action="store_true",
-    )
-    group.add_argument(
+    parser.add_argument(
         "--search-per-folder",
         help="Fetches Looks and Dashboards per folder",
         action="store_true",
     )
 
     args = parser.parse_args()
 
     looker.extract_all(
-        all_looks=args.all_looks,
         base_url=args.base_url,
         client_id=args.username,
         client_secret=args.password,
         log_to_stdout=args.log_to_stdout,
         output_directory=args.output,
         safe_mode=args.safe_mode,
         search_per_folder=args.search_per_folder,
```

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_metabase_api.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_metabase_api.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_metabase_db.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_metabase_db.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_mode.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_postgres.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_postgres.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_powerbi.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_powerbi.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_qlik.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_qlik.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_redshift.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_redshift.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_sigma.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_sigma.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_snowflake.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_snowflake.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/extract_tableau.py` & `castor_extractor-0.9.2/castor_extractor/commands/extract_tableau.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/file_check.py` & `castor_extractor-0.9.2/castor_extractor/commands/file_check.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/commands/upload.py` & `castor_extractor-0.9.2/castor_extractor/commands/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/column.py` & `castor_extractor-0.9.2/castor_extractor/file_checker/column.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/column_test.py` & `castor_extractor-0.9.2/castor_extractor/file_checker/column_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/enums.py` & `castor_extractor-0.9.2/castor_extractor/file_checker/enums.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/file.py` & `castor_extractor-0.9.2/castor_extractor/file_checker/file.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/file_test.py` & `castor_extractor-0.9.2/castor_extractor/file_checker/file_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/file_test_users.csv` & `castor_extractor-0.9.2/castor_extractor/file_checker/file_test_users.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/file_checker/templates/generic_warehouse.py` & `castor_extractor-0.9.2/castor_extractor/file_checker/templates/generic_warehouse.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/logger.py` & `castor_extractor-0.9.2/castor_extractor/logger.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/client.py` & `castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/client_test.py` & `castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/transformation/dbt/client/credentials.py` & `castor_extractor-0.9.2/castor_extractor/transformation/dbt/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/uploader/constant.py` & `castor_extractor-0.9.2/castor_extractor/uploader/constant.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/uploader/env.py` & `castor_extractor-0.9.2/castor_extractor/uploader/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/uploader/upload.py` & `castor_extractor-0.9.2/castor_extractor/uploader/upload.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/__init__.py` & `castor_extractor-0.9.2/castor_extractor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/deprecate.py` & `castor_extractor-0.9.2/castor_extractor/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/env.py` & `castor_extractor-0.9.2/castor_extractor/utils/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/files.py` & `castor_extractor-0.9.2/castor_extractor/utils/files.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/files_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/formatter.py` & `castor_extractor-0.9.2/castor_extractor/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/formatter_test.csv` & `castor_extractor-0.9.2/castor_extractor/utils/formatter_test.csv`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/formatter_test.json` & `castor_extractor-0.9.2/castor_extractor/utils/formatter_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/formatter_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/formatter_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/json_stream_write.py` & `castor_extractor-0.9.2/castor_extractor/utils/json_stream_write.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/object.py` & `castor_extractor-0.9.2/castor_extractor/utils/object.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/object_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/pager.py` & `castor_extractor-0.9.2/castor_extractor/utils/pager.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/pager_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/pager_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/retry.py` & `castor_extractor-0.9.2/castor_extractor/utils/retry.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/retry_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/retry_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/safe.py` & `castor_extractor-0.9.2/castor_extractor/utils/safe.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/safe_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/safe_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/store.py` & `castor_extractor-0.9.2/castor_extractor/utils/store.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/string.py` & `castor_extractor-0.9.2/castor_extractor/utils/string.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/string_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/string_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/time.py` & `castor_extractor-0.9.2/castor_extractor/utils/time.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/validation.py` & `castor_extractor-0.9.2/castor_extractor/utils/validation.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/validation_test.py` & `castor_extractor-0.9.2/castor_extractor/utils/validation_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/utils/write.py` & `castor_extractor-0.9.2/castor_extractor/utils/write.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/domo/client/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/domo/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/domo/client/client_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/domo/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/domo/client/credentials.py` & `castor_extractor-0.9.2/castor_extractor/visualization/domo/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/domo/client/endpoints.py` & `castor_extractor-0.9.2/castor_extractor/visualization/domo/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/domo/client/pagination.py` & `castor_extractor-0.9.2/castor_extractor/visualization/domo/client/pagination.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/domo/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/domo/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/api/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             )
 
         if folder_id:
             return list(_search())  # no pagination when using folder filter
 
         return Pager(_search, logger=self._logger).all(per_page=self.per_page)
 
-    def _search_looks(self, folder_id: Optional[str] = None) -> List[Look]:
+    def looks(self, folder_id: Optional[str] = None) -> List[Look]:
         """
         Fetch looks via `search_looks` using pagination. The optional folder_id
         allows restricting the search to the given folder.
         https://developers.looker.com/api/explorer/4.0/methods/Look/search_looks
         """
 
         def _search(
@@ -152,30 +152,14 @@
         """
         fetch looks via `all_looks`
         https://castor.cloud.looker.com/extensions/marketplace_extension_api_explorer::api-explorer/4.0/methods/Look/all_looks
         """
         # No pagination : see https://community.looker.com/looker-api-77/api-paging-limits-14598
         return list(self._sdk.all_looks(fields=format_fields(LOOK_FIELDS)))
 
-    def looks(
-        self,
-        all_looks_endpoint: Optional[bool] = False,
-        folder_id: Optional[str] = None,
-    ) -> List[Look]:
-        """Lists looks of the given Looker account
-
-        By default, uses the endpoint `search_looks` that allows pagination and
-        filtering on a folder.
-        If `all_looks_endpoint` parameter is set to True, it uses `all_looks` endpoint.
-        """
-        if all_looks_endpoint:
-            return self._all_looks()
-
-        return self._search_looks(folder_id)
-
     def users(self) -> List[User]:
         """Lists users of the given Looker account"""
 
         def _search(page: int, per_page: int) -> Sequence[User]:
             # HACK:
             # We use verified_looker_employee=False (filter out Looker employees)
             # Else api returns an empty list when no parameters are specified
```

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/api/client_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/api/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/api/constants.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/api/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/api/sdk.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/api/sdk.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/api/sdk_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/api/sdk_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/api/utils.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/api/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/constant.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/constant.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,10 +16,9 @@
 DEFAULT_LOOKER_THREAD_POOL_SIZE = 20
 KEY_LOOKER_THREAD_POOL_SIZE = "CASTOR_LOOKER_THREAD_POOL_SIZE"
 
 # env variables
 BASE_URL = "CASTOR_LOOKER_BASE_URL"
 CLIENT_ID = "CASTOR_LOOKER_CLIENT_ID"
 CLIENT_SECRET = "CASTOR_LOOKER_CLIENT_SECRET"  # noqa: S105
-ALL_LOOKS = "CASTOR_LOOKER_ALL_LOOKS"
 SEARCH_PER_FOLDER = "CASTOR_LOOKER_SEARCH_PER_FOLDER"
 LOG_TO_STDOUT = "CASTOR_LOOKER_LOG_TO_STDOUT"
```

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/env.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/env.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         timeout=timeout,
     )
     return ApiClient(credentials=credentials, safe_mode=safe_mode)
 
 
 def iterate_all_data(
     client: ApiClient,
-    all_looks: bool,
     search_per_folder: bool,
     thread_pool_size: int,
     log_to_stdout: bool,
 ) -> Union[StreamableList, Iterable[Tuple[LookerAsset, list]]]:
     """Iterate over the extracted Data From looker"""
 
     logger.info("Extracting users from Looker API")
@@ -70,15 +69,15 @@
         thread_pool_size=thread_pool_size,
         log_to_stdout=log_to_stdout,
     )
     if search_per_folder:
         looks_stream = fetcher.fetch_assets(LookerAsset.LOOKS)
         yield LookerAsset.LOOKS, StreamableList(looks_stream)
     else:
-        yield LookerAsset.LOOKS, deep_serialize(client.looks(all_looks))
+        yield LookerAsset.LOOKS, deep_serialize(client.looks())
 
     logger.info("Extracting dashboards from Looker API")
     if search_per_folder:
         dashboards_stream = fetcher.fetch_assets(LookerAsset.DASHBOARDS)
         yield LookerAsset.DASHBOARDS, StreamableList(dashboards_stream)
         dashboard_explore_names_ = fetcher.explores
     else:
@@ -140,15 +139,14 @@
         safe_mode=safe_mode,
     )
 
     ts = current_timestamp()
 
     data = iterate_all_data(
         client=client,
-        all_looks=parameters.all_looks,
         search_per_folder=parameters.search_per_folder,
         thread_pool_size=parameters.thread_pool_size,
         log_to_stdout=parameters.log_to_stdout,
     )
     for asset, data in data:
         filename = get_output_filename(asset.value, output_directory, ts)
         write_json(filename, data)
```

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/fields.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/fields_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/fields_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/multithreading.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/multithreading.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/looker/parameters.py` & `castor_extractor-0.9.2/castor_extractor/visualization/looker/parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import NamedTuple, Optional
 
 from ...utils import OUTPUT_DIR, from_env, validate_baseurl
 from .constant import (
-    ALL_LOOKS,
     BASE_URL,
     CLIENT_ID,
     CLIENT_SECRET,
     LOG_TO_STDOUT,
     SEARCH_PER_FOLDER,
 )
 from .env import thread_pool_size
@@ -27,15 +26,14 @@
     parameter = from_env(key, allow_missing=True)
     return str(parameter).lower() == "true"
 
 
 class Parameters(NamedTuple):
     """Parameters for Looker extraction"""
 
-    all_looks: bool
     base_url: str
     client_id: str
     client_secret: str
     is_safe_mode: bool
     log_to_stdout: bool
     output_directory: str
     search_per_folder: bool
@@ -59,21 +57,19 @@
     # timeout can be set with env variable however we don't use from_env because it has a default value
     timeout = kwargs.get("timeout")
 
     is_safe_mode = kwargs.get("safe_mode", False)
     search_per_folder = kwargs.get("search_per_folder") or _bool_env_variable(
         SEARCH_PER_FOLDER,
     )
-    all_looks = kwargs.get("all_looks") or _bool_env_variable(ALL_LOOKS)
     log_to_stdout = kwargs.get("log_to_stdout") or _bool_env_variable(
         LOG_TO_STDOUT
     )
 
     return Parameters(
-        all_looks=all_looks,
         base_url=base_url,
         client_id=client_id,
         client_secret=client_secret,
         is_safe_mode=is_safe_mode,
         log_to_stdout=log_to_stdout,
         output_directory=output_directory,
         search_per_folder=search_per_folder,
```

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/assets.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/api/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/api/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/api/credentials.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/api/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/db/credentials.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/db/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/decryption.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/decryption.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/client/decryption_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/client/decryption_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/errors.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/metabase/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/metabase/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/assets.py` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/client/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/client/client_test.json` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/client/client_test.json`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/client/client_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/client/credentials.py` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/errors.py` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/errors.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/mode/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/mode/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/constants.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/credentials_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/credentials_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/rest.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/rest_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/utils.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/client/utils_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/client/utils_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/powerbi/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/powerbi/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/assets.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/constants.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/constants.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/constants.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/error.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/error.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/error_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/error_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/json_rpc.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/json_rpc.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/json_rpc_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/engine/websocket.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/engine/websocket.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/master.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/master.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/rest.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/rest.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/client/rest_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/client/rest_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/qlik/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/qlik/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/client_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/credentials.py` & `castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/endpoints.py` & `castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/sigma/client/pagination.py` & `castor_extractor-0.9.2/castor_extractor/visualization/sigma/client/pagination.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/sigma/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/sigma/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/assets.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/assets.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/client.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/client_utils.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/client_utils.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/credentials.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/credentials.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/project.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/project.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/client/safe_mode.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/client/safe_mode.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/extract.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/gql_fields.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/gql_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/project_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/user_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/view_get_usage.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/assets/rest_api/workbook_get.xml`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/graphql/paginated_object_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/auth_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/projects_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/usages_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/users_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tests/unit/rest_api/workbooks_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/visualization/tableau/tsc_fields.py` & `castor_extractor-0.9.2/castor_extractor/visualization/tableau/tsc_fields.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/abstract/asset.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/abstract/asset.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/abstract/client.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/abstract/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/abstract/extract.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/abstract/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/abstract/query.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/abstract/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/abstract/time_filter.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/abstract/time_filter.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/client.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/client_test.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/extract.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/column.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/cte/sharded.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/query.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/table.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/queries/table_with_tags.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/bigquery/query.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/bigquery/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/postgres/client.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/postgres/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/postgres/extract.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/postgres/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/column.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/schema.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/postgres/queries/table.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/postgres/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/postgres/query.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/postgres/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/client.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/client_test.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/extract.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/column.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/query.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/query.sql`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,34 @@
     FROM pg_catalog.stl_query AS q
         CROSS JOIN parameters AS p
     WHERE TRUE
         AND DATE(q.starttime) = p.day_start
         AND EXTRACT('hour' FROM q.starttime) BETWEEN p.hour_min AND p.hour_max
 ),
 
-raw_query_text AS
-(
+query AS (
     SELECT
         q.query,
-        LISTAGG(qt.text, '') WITHIN GROUP (ORDER BY qt.sequence) AS agg_text
+        qt.text,
+        qt.sequence,
+        COUNT(*) OVER(PARTITION BY q.query) AS sequence_count
     FROM queries_deduplicated AS q
         INNER JOIN pg_catalog.stl_querytext AS qt ON q.query = qt.query
+),
+
+raw_query_text AS
+(
+    SELECT
+        q.query,
+        LISTAGG(q.text, '') WITHIN GROUP (ORDER BY q.sequence) AS agg_text
+    FROM query AS q
     WHERE TRUE
-        -- LISTAGG raises an error when total length >= 64K
-        AND qt.sequence < (65535 / 200)
+    -- LISTAGG raises an error when total length >= 65535
+    -- each sequence contains 200 char max
+        AND q.sequence_count < (65535 / 200)
     GROUP BY q.query
 ),
 
 query_text AS (
     SELECT
         query,
         CASE
@@ -55,15 +65,15 @@
         JOIN pg_catalog.pg_database AS db ON db.datname = q.database
         CROSS JOIN parameters AS p
     WHERE TRUE
         AND DATE(q.starttime) = p.day_start
         AND EXTRACT('hour' FROM q.starttime) BETWEEN p.hour_min AND p.hour_max
 ),
 
--- the DDL part is sensible to any change of JOIN and AGGREGATIOn: test in the field prior to merging
+-- the DDL part is sensible to any change of JOIN and AGGREGATION: test in the field prior to merging
 ddl_query AS (
     SELECT
         (q.xid || '-' || q.query_part_rank)::VARCHAR(256) AS query_id,
         q.query_text::VARCHAR(20000) AS query_text,
         db.oid AS database_id,
         db.datname AS database_name,
         q.process_id,
```

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/schema.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/table.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/table_freshness.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/table_freshness.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/queries/view_ddl.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/redshift/query.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/redshift/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/client.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/client.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/client_test.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/client_test.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/extract.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/column.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/column_lineage.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/column_lineage.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/query.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/schema.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/schema.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/table.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/user.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/user.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/queries/view_ddl.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/queries/view_ddl.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/snowflake/query.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/snowflake/query.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/synapse/extract.py` & `castor_extractor-0.9.2/castor_extractor/warehouse/synapse/extract.py`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/column.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/column.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/query.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/query.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/castor_extractor/warehouse/synapse/queries/table.sql` & `castor_extractor-0.9.2/castor_extractor/warehouse/synapse/queries/table.sql`

 * *Files identical despite different names*

### Comparing `castor_extractor-0.9.0/pyproject.toml` & `castor_extractor-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 
 [tool.poetry]
 name = "castor-extractor"
-version = "0.9.0"
+version = "0.9.2"
 description = "Extract your metadata assets."
 authors = ["Castor <support@castordoc.com>"]
 license = "EULA"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 readme = "README.md"
 homepage = "https://www.castordoc.com/"
 documentation = "https://docs.castordoc.com/castor-package/castor-extractor"
-include = ["README.md", "CHANGELOG.md", "LICENCE", "*/*/*/*.sql"]
+include = ["README.md", "CHANGELOG.md", "LICENCE", "*/*/*/*.sql", "Dockerfile", "DockerfileUsage.md"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 
 click = "~8.1"
 cryptography = { version = ">= 41.0.5", optional = true }
```

### Comparing `castor_extractor-0.9.0/PKG-INFO` & `castor_extractor-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castor-extractor
-Version: 0.9.0
+Version: 0.9.2
 Summary: Extract your metadata assets.
 Home-page: https://www.castordoc.com/
 License: EULA
 Author: Castor
 Author-email: support@castordoc.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

