# Comparing `tmp/skibidi_orm-0.1.0.tar.gz` & `tmp/skibidi_orm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skibidi_orm-0.1.0.tar", last modified: Thu May 30 13:20:22 2024, max compression
+gzip compressed data, was "skibidi_orm-0.1.1.tar", last modified: Thu May 30 14:01:30 2024, max compression
```

## Comparing `skibidi_orm-0.1.0.tar` & `skibidi_orm-0.1.1.tar`

### file list

```diff
@@ -1,125 +1,110 @@
--rw-r--r--   0        0        0       26 2024-05-28 22:54:44.626227 skibidi_orm-0.1.0/README.md
--rw-r--r--   0        0        0      911 2024-05-30 13:20:22.511967 skibidi_orm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 22:54:44.626227 skibidi_orm-0.1.0/src/skibidi_orm/__init__.py
--rw-r--r--   0        0        0     2708 2024-05-29 13:45:39.054079 skibidi_orm-0.1.0/src/skibidi_orm/cli/run.py
--rw-r--r--   0        0        0      596 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/cli/utils.py
--rw-r--r--   0        0        0      136 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/exceptions/cli_exceptions.py
--rw-r--r--   0        0        0       93 2024-05-29 13:48:00.738913 skibidi_orm-0.1.0/src/skibidi_orm/exceptions/config_exceptions.py
--rw-r--r--   0        0        0      190 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/exceptions/constraints.py
--rw-r--r--   0        0        0      172 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/exceptions/db_mutator_exceptions.py
--rw-r--r--   0        0        0      309 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/exceptions/operations.py
--rw-r--r--   0        0        0        0 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/__init__.py
--rw-r--r--   0        0        0     1160 2024-05-30 11:51:55.102388 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/base_adapter.py
--rw-r--r--   0        0        0        0 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
--rw-r--r--   0        0        0     2031 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/constraints-old-bak.py
--rw-r--r--   0        0        0     2532 2024-05-30 12:51:45.049013 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
--rw-r--r--   0        0        0      659 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
--rw-r--r--   0        0        0      439 2024-05-29 14:59:49.438352 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/sqlite3_typing.py
--rw-r--r--   0        0        0     1303 2024-05-30 12:54:57.335198 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py
--rw-r--r--   0        0        0     1227 2024-05-30 11:38:51.368974 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/postgres_typing.py
--rw-r--r--   0        0        0     1404 2024-05-29 15:00:14.229539 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
--rw-r--r--   0        0        0      439 2024-05-29 15:00:38.730471 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
--rw-r--r--   0        0        0     3410 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/base/interfaces.py
--rw-r--r--   0        0        0     1065 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
--rw-r--r--   0        0        0     3921 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
--rw-r--r--   0        0        0     1974 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
--rw-r--r--   0        0        0     5457 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
--rw-r--r--   0        0        0     1053 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
--rw-r--r--   0        0        0     2508 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
--rw-r--r--   0        0        0     1062 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_config/base_config.py
--rw-r--r--   0        0        0     1624 2024-05-29 14:22:57.376633 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_config/postgres_config.py
--rw-r--r--   0        0        0      392 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
--rw-r--r--   0        0        0      671 2024-05-30 12:54:32.135068 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
--rw-r--r--   0        0        0     8809 2024-05-30 12:41:40.958668 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py
--rw-r--r--   0        0        0     5789 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
--rw-r--r--   0        0        0     6589 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/operations/column_operations.py
--rw-r--r--   0        0        0      280 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/operations/operation_type.py
--rw-r--r--   0        0        0     2286 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/operations/table_operations.py
--rw-r--r--   0        0        0      585 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
--rw-r--r--   0        0        0     1379 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
--rw-r--r--   0        0        0      417 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
--rw-r--r--   0        0        0     4586 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/state_manager/state_manager.py
--rw-r--r--   0        0        0     3053 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/server.py
--rw-r--r--   0        0        0      436 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      248 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
--rw-r--r--   0        0        0      339 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
--rw-r--r--   0        0        0  2063635 2024-05-28 23:30:01.555813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
--rw-r--r--   0        0        0   318663 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
--rw-r--r--   0        0        0      283 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
--rw-r--r--   0        0        0      464 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
--rw-r--r--   0        0        0     1497 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
--rw-r--r--   0        0        0      366 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
--rw-r--r--   0        0        0     1617 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
--rw-r--r--   0        0        0   134211 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       80 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
--rw-r--r--   0        0        0     1497 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
--rw-r--r--   0        0        0     4126 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
--rw-r--r--   0        0        0      926 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
--rw-r--r--   0        0        0     1038 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
--rw-r--r--   0        0        0     1337 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
--rw-r--r--   0        0        0     2121 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
--rw-r--r--   0        0        0     1377 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
--rw-r--r--   0        0        0     1322 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
--rw-r--r--   0        0        0     1730 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1835 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
--rw-r--r--   0        0        0      315 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     3835 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7295 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     1709 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
--rw-r--r--   0        0        0      772 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     1361 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
--rw-r--r--   0        0        0     1529 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
--rw-r--r--   0        0        0     1224 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
--rw-r--r--   0        0        0     1054 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
--rw-r--r--   0        0        0      945 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
--rw-r--r--   0        0        0     1140 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
--rw-r--r--   0        0        0     1726 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
--rw-r--r--   0        0        0     1595 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
--rw-r--r--   0        0        0      764 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
--rw-r--r--   0        0        0      355 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
--rw-r--r--   0        0        0      166 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
--rw-r--r--   0        0        0      790 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
--rw-r--r--   0        0        0     1409 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
--rw-r--r--   0        0        0     1173 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
--rw-r--r--   0        0        0      343 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
--rw-r--r--   0        0        0     7445 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
--rw-r--r--   0        0        0     1211 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
--rw-r--r--   0        0        0       38 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0     2143 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
--rw-r--r--   0        0        0      711 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
--rw-r--r--   0        0        0      378 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
--rw-r--r--   0        0        0      617 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
--rw-r--r--   0        0        0      784 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
--rw-r--r--   0        0        0      566 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
--rw-r--r--   0        0        0     3493 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/table_example.py
--rw-r--r--   0        0        0        0 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/tests/skibidi-orm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 22:54:44.636227 skibidi_orm-0.1.0/tests/skibidi-orm/cli/schema.py
--rw-r--r--   0        0        0     2136 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/tests/skibidi-orm/cli/test_run.py
--rw-r--r--   0        0        0        0 2024-05-29 15:29:03.376282 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/__init__.py
--rw-r--r--   0        0        0     3262 2024-05-29 17:27:48.227178 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/conftest.py
--rw-r--r--   0        0        0      617 2024-05-29 23:35:42.667393 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/constraints/test_constraints.py
--rw-r--r--   0        0        0     7289 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
--rw-r--r--   0        0        0     2619 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
--rw-r--r--   0        0        0     4974 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
--rw-r--r--   0        0        0     1594 2024-05-29 14:00:59.664833 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_config/test_config.py
--rw-r--r--   0        0        0     1590 2024-05-29 14:21:21.523846 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py
--rw-r--r--   0        0        0        0 2024-05-29 15:29:09.166268 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_inspector/__init__.py
--rw-r--r--   0        0        0     5122 2024-05-29 16:31:19.295832 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
--rw-r--r--   0        0        0    33961 2024-05-30 12:50:33.157091 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:39.057771 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_mutators/__init__.py
--rw-r--r--   0        0        0     9698 2024-05-29 16:30:44.864877 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
--rw-r--r--   0        0        0     7425 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/operations/test_operations.py
--rw-r--r--   0        0        0     7372 2024-05-30 12:43:18.032203 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/sql_data.py
--rw-r--r--   0        0        0      967 2024-05-28 23:00:31.386159 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
--rw-r--r--   0        0        0        0 2024-05-29 16:25:09.614489 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/state_manager/__init__.py
--rw-r--r--   0        0        0    16096 2024-05-29 16:30:06.833853 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
--rw-r--r--   0        0        0        0 2024-05-29 16:23:45.831815 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/__init__.py
--rw-r--r--   0        0        0     2146 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
--rw-r--r--   0        0        0      805 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
--rw-r--r--   0        0        0      736 2024-05-28 23:30:01.565813 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
--rw-r--r--   0        0        0     3281 2024-05-29 16:29:38.532942 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_routes.py
--rw-r--r--   0        0        0    17551 2024-05-29 16:29:19.491784 skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/test_module_cooperation.py
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 skibidi_orm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-28 22:54:44.626227 skibidi_orm-0.1.1/README.md
+-rw-r--r--   0        0        0      775 2024-05-30 14:01:30.070050 skibidi_orm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 22:54:44.626227 skibidi_orm-0.1.1/src/skibidi_orm/__init__.py
+-rw-r--r--   0        0        0     2653 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/cli/run.py
+-rw-r--r--   0        0        0      596 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/cli/utils.py
+-rw-r--r--   0        0        0      136 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/exceptions/cli_exceptions.py
+-rw-r--r--   0        0        0      190 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/exceptions/constraints.py
+-rw-r--r--   0        0        0      172 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/exceptions/db_mutator_exceptions.py
+-rw-r--r--   0        0        0      309 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/exceptions/operations.py
+-rw-r--r--   0        0        0        0 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/base_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
+-rw-r--r--   0        0        0     2192 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
+-rw-r--r--   0        0        0      901 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
+-rw-r--r--   0        0        0     1614 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
+-rw-r--r--   0        0        0      515 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
+-rw-r--r--   0        0        0     3410 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/base/interfaces.py
+-rw-r--r--   0        0        0     1065 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
+-rw-r--r--   0        0        0     3904 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
+-rw-r--r--   0        0        0     1974 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
+-rw-r--r--   0        0        0     5440 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
+-rw-r--r--   0        0        0     1053 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
+-rw-r--r--   0        0        0     2508 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
+-rw-r--r--   0        0        0     1062 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_config/base_config.py
+-rw-r--r--   0        0        0      192 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_config/postgres_config.py
+-rw-r--r--   0        0        0      392 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
+-rw-r--r--   0        0        0      671 2024-05-30 12:54:32.135068 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
+-rw-r--r--   0        0        0     6025 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
+-rw-r--r--   0        0        0     6589 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/operations/column_operations.py
+-rw-r--r--   0        0        0      280 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/operations/operation_type.py
+-rw-r--r--   0        0        0     2286 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/operations/table_operations.py
+-rw-r--r--   0        0        0      585 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
+-rw-r--r--   0        0        0     2173 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
+-rw-r--r--   0        0        0      694 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
+-rw-r--r--   0        0        0     5556 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/state_manager/state_manager.py
+-rw-r--r--   0        0        0     3053 2024-05-30 13:51:05.731531 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/server.py
+-rw-r--r--   0        0        0      436 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      248 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
+-rw-r--r--   0        0        0      339 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
+-rw-r--r--   0        0        0  2063635 2024-05-28 23:30:01.555813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
+-rw-r--r--   0        0        0   318663 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
+-rw-r--r--   0        0        0      283 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
+-rw-r--r--   0        0        0      464 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
+-rw-r--r--   0        0        0      366 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
+-rw-r--r--   0        0        0     1617 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
+-rw-r--r--   0        0        0   134211 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       80 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
+-rw-r--r--   0        0        0     1497 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
+-rw-r--r--   0        0        0     4126 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
+-rw-r--r--   0        0        0      926 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
+-rw-r--r--   0        0        0     1038 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1337 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
+-rw-r--r--   0        0        0     2121 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
+-rw-r--r--   0        0        0     1377 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
+-rw-r--r--   0        0        0     1322 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
+-rw-r--r--   0        0        0     1730 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1835 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
+-rw-r--r--   0        0        0      315 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     3835 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7295 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     1709 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
+-rw-r--r--   0        0        0      772 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     1361 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
+-rw-r--r--   0        0        0     1529 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
+-rw-r--r--   0        0        0     1224 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
+-rw-r--r--   0        0        0     1054 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
+-rw-r--r--   0        0        0      945 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
+-rw-r--r--   0        0        0     1140 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
+-rw-r--r--   0        0        0     1726 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
+-rw-r--r--   0        0        0     1595 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
+-rw-r--r--   0        0        0      764 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
+-rw-r--r--   0        0        0      355 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
+-rw-r--r--   0        0        0      166 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
+-rw-r--r--   0        0        0      790 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
+-rw-r--r--   0        0        0     1409 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
+-rw-r--r--   0        0        0     1173 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
+-rw-r--r--   0        0        0      343 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
+-rw-r--r--   0        0        0     7445 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
+-rw-r--r--   0        0        0     1211 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
+-rw-r--r--   0        0        0       38 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0     2143 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
+-rw-r--r--   0        0        0      711 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      378 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
+-rw-r--r--   0        0        0      617 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
+-rw-r--r--   0        0        0      784 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
+-rw-r--r--   0        0        0      566 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
+-rw-r--r--   0        0        0     3476 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/table_example.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/tests/skibidi-orm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:54:44.636227 skibidi_orm-0.1.1/tests/skibidi-orm/cli/schema.py
+-rw-r--r--   0        0        0     2136 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/tests/skibidi-orm/cli/test_run.py
+-rw-r--r--   0        0        0     1654 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/conftest.py
+-rw-r--r--   0        0        0     7281 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
+-rw-r--r--   0        0        0     2619 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
+-rw-r--r--   0        0        0     4963 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
+-rw-r--r--   0        0        0     1447 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/db_config/test_config.py
+-rw-r--r--   0        0        0     6182 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
+-rw-r--r--   0        0        0     9737 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
+-rw-r--r--   0        0        0     7425 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/operations/test_operations.py
+-rw-r--r--   0        0        0      967 2024-05-28 23:00:31.386159 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
+-rw-r--r--   0        0        0    17111 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
+-rw-r--r--   0        0        0     2146 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
+-rw-r--r--   0        0        0      805 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
+-rw-r--r--   0        0        0      736 2024-05-28 23:30:01.565813 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
+-rw-r--r--   0        0        0     4268 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_routes.py
+-rw-r--r--   0        0        0    17767 2024-05-30 13:34:55.161340 skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/test_module_cooperation.py
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 skibidi_orm-0.1.1/PKG-INFO
```

### Comparing `skibidi_orm-0.1.0/pyproject.toml` & `skibidi_orm-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [project]
 name = "SkiBiDi-ORM"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python ORM"
 authors = [
     { name = "xDepcio", email = "olek.drwal@gmail.com" },
     { name = "jedrzej-grabski", email = "jedrzej@grabski.pl" },
     { name = "mbienkowski", email = "bienkowski.maksym@gmail.com" },
 ]
 dependencies = [
     "typer>=0.11.0",
     "colorama>=0.4.6",
     "fastapi>=0.111.0",
-    "psycopg2-binary>=2.9.9",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
@@ -34,12 +33,7 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.1.1",
 ]
 
 [tool.pdm.scripts]
 tests = "pytest --verbose --color=yes --ignore ./tmp"
-
-[tool.pytest.ini_options]
-markers = [
-    "slow: mark test as slow (deselect with '-m \"not slow\"')",
-]
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/cli/run.py` & `skibidi_orm-0.1.1/src/skibidi_orm/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,31 +83,28 @@
     schema_file: Union[str, None] = typer.Option(
         None, "--schema-file", "-s", help="Schema file path"
     )
 ):
     """
     Run web UI for CRUD operations on current DB.
     """
+    if schema_file is not None:
+        run_server(schema_file=schema_file)
+        return
 
     try:
-        if schema_file is None:
-            schema_file = find_schema_file()
+        schema_file = find_schema_file()
+        run_server(schema_file=schema_file)
     except MultipleSchemaFilesError:
         print(
             Fore.RED
             + "Multiple schema files found. Please specify the schema file to use: --schema-file <PATH>"
         )
         raise typer.Exit(code=1)
 
-    try:
-        run_server(schema_file=schema_file)
-    except Exception as e:
-        print(Fore.RED + f"Error: {e}")
-        raise typer.Exit(code=1)
-
 
 def main():
     app()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/cli/utils.py` & `skibidi_orm-0.1.1/src/skibidi_orm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/base_adapter.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/base_adapter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from functools import total_ordering
 from typing import Any
 
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     ColumnSpecificConstraint,
     ForeignKeyConstraint,
 )
 
 
-@total_ordering
 @dataclass(unsafe_hash=True)
 class BaseColumn[TDataTypes]:
+    """
+    Base column class that has to be properly implemented by the database specific column class.
+    """
+
     name: str
     data_type: TDataTypes
     column_constraints: list[ColumnSpecificConstraint] = field(
         default_factory=list, hash=False
     )
 
-    def __lt__(self, other: Any):
-        if isinstance(other, BaseColumn):
-            return self.name < other.name
-        return NotImplemented
-
 
 @dataclass
 class BaseTable[TCol]:
+    """
+    Base table class that has to be properly implemented by the database specific table class.
+    """
+
     name: str
     columns: list[TCol] = field(default_factory=list)
     foreign_keys: set[ForeignKeyConstraint] = field(default_factory=set)
 
 
 class BaseAdapter(ABC):
+    """
+    Base adapter class that has to be properly implemented by the database specific adapter class.
+    """
 
     @abstractmethod
     def create_table(self, table: BaseTable[BaseColumn[Any]]):
         """Create a table in the database"""
         pass
 
     @abstractmethod
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/constraints-old-bak.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,58 @@
 import enum
 from dataclasses import dataclass, field
 
 
 class ConstraintType(enum.Enum):
     """All supported constraint types"""
 
-    NOT_NULL = enum.auto()
-    UNIQUE = enum.auto()
-    PRIMARY_KEY = enum.auto()
-    FOREIGN_KEY = enum.auto()
-    CHECK = enum.auto()
-    DEFAULT = enum.auto()
+    NOT_NULL = "NOT NULL"
+    UNIQUE = "UNIQUE"
+    PRIMARY_KEY = "PRIMARY KEY"
+    FOREIGN_KEY = "FOREIGN KEY"
+    CHECK = "CHECK"
+    DEFAULT = "DEFAULT"
 
 
 @dataclass(frozen=True)
 class Constraint(ABC):
     """Base class for all constraints"""
 
     constraint_type: ConstraintType = field(init=False)
     table_name: str
 
 
 @dataclass(frozen=True)
-class NotNullConstraint(Constraint):
+class ColumnSpecificConstraint(Constraint):
+    """Base class for constraints that apply to a column instead of multiple (e.g. composite foreign keys)"""
+
+    column_name: str
+
+
+@dataclass(frozen=True)
+class NotNullConstraint(ColumnSpecificConstraint):
     """Class for the NOT NULL constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.NOT_NULL)
-    column_name: str
 
 
 @dataclass(frozen=True)
-class UniqueConstraint(Constraint):
+class UniqueConstraint(ColumnSpecificConstraint):
     """Class for the UNIQUE constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.UNIQUE)
-    column_name: str
 
 
 @dataclass(frozen=True)
-class PrimaryKeyConstraint(Constraint):
+class PrimaryKeyConstraint(ColumnSpecificConstraint):
     """Class for the PRIMARY KEY constraint"""
 
     constraint_type: ConstraintType = field(
         init=False, default=ConstraintType.PRIMARY_KEY
     )
-    column_name: str
 
 
 @dataclass(frozen=True, unsafe_hash=True)
 class ForeignKeyConstraint(Constraint):
     """Class for the FOREIGN KEY constraint"""
 
     constraint_type: ConstraintType = field(
@@ -58,22 +62,20 @@
     referenced_table: str
     column_mapping: dict[str, str] = field(
         hash=False
     )  # maps the corresponding column names: {referencing_column1: referenced_column1, ...}
 
 
 @dataclass(frozen=True)
-class CheckConstraint(Constraint):
+class CheckConstraint(ColumnSpecificConstraint):
     """Class for the CHECK constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.CHECK)
-    column_name: str
     condition: str
 
 
 @dataclass(frozen=True)
-class DefaultConstraint(Constraint):
+class DefaultConstraint(ColumnSpecificConstraint):
     """Class for the DEFAULT constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.DEFAULT)
-    column_name: str
     value: str
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 
 from skibidi_orm.migration_engine.operations.column_operations import ColumnOperation
 from skibidi_orm.migration_engine.operations.table_operations import TableOperation
 
 
 # All classes need to inherit from this class if they participate in a migration
 class MigrationElement:
+    """
+    Base class for all migration elements. Every class that wants to participate in a migration should inherit from this class.
+    """
+
     adapter: BaseAdapter
     operations: list[ColumnOperation | TableOperation] = []
 
     def migrate(self, preview: bool = False):
+        """
+        This will execute the migration for all the migration elements.
+
+        """
         table = MigrationElement.__subclasses__()
 
         for cls in table:
             table_instance = cls()
             table_instance.adapter.execute_migration(preview)
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 from skibidi_orm.migration_engine.adapters.base_adapter import BaseAdapter
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import (
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.state_manager.state_manager import StateManager
 
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
 
 
 class SQLite3Adapter(BaseAdapter):
+    """
+    This is an adapter that will select the proper functionality of the whole migration engine to accommodate a SQLite3 database.
+    """
 
     tables: list[SQLite3Typing.Table]
 
     def __init__(self) -> None:
         self.tables = []
 
     def create_table(self, table: SQLite3Typing.Table):
@@ -34,11 +37,13 @@
         db_tables = self.inspector.get_tables()
 
         state_manager = StateManager[SQLite3Typing.Table](
             db_tables=db_tables,
             schema_tables=self.tables,
         )
 
-        MigrationElement.operations = state_manager.get_operations()
+        MigrationElement.operations = (
+            state_manager.get_operations_transforming_database_schema_into_class_hierarchy_schema()
+        )
 
         if not preview:
             SQLite3Executor.execute_operations(MigrationElement.operations)
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/base/interfaces.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/all.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/all.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import SQLite3Typing
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import SQLite3Typing
 from skibidi_orm.migration_engine.converters.base.interfaces import (
     ColumnOperationSQLConverter,
 )
 from skibidi_orm.migration_engine.converters.sqlite3.constraints import (
     SQLite3ConstraintConverter,
 )
 from skibidi_orm.migration_engine.operations.column_operations import (
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import SQLite3Typing
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import SQLite3Typing
 from skibidi_orm.migration_engine.converters.base.interfaces import (
     TableOperationSQLConverter,
 )
 from skibidi_orm.migration_engine.converters.sqlite3.columns import (
     SQLite3ColumnOperationConverter,
 )
 from skibidi_orm.migration_engine.converters.sqlite3.constraints import (
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_config/base_config.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_config/base_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Any, Literal, cast
 import sqlite3
 
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import (
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 import skibidi_orm.migration_engine.adapters.database_objects.constraints as c
 
 type SQLite3PragmaTableInfo = list[
     tuple[int, str, str, Literal[0, 1], Any, Literal[0, 1]]
 ]
@@ -56,23 +56,31 @@
 
     def __init__(self) -> None:
         self.config = SQLite3Config.get_instance()
 
     def get_tables(
         self,
     ) -> list[SQLite3Typing.Table]:
+        """
+        Retrieve all tables from the database.
+        """
+
         tables: list[SQLite3Typing.Table] = []
         tables_names = self.get_tables_names()
         for table_name in tables_names:
             table_columns = self.get_table_columns(table_name)
             tables.append(SQLite3Typing.Table(name=table_name, columns=table_columns))
 
         return tables
 
     def get_tables_names(self) -> list[str]:
+        """
+        Retrieve just tables names from the database.
+        """
+
         tables = self._sqlite_execute(
             "SELECT name FROM sqlite_master WHERE type='table';"
         )
         return [table[0] for table in tables]
 
     @staticmethod
     def foreign_keys_from_pragma_entries(
@@ -126,14 +134,17 @@
         )
         return constraints
 
     def get_table_columns(self, table_name: str) -> list[SQLite3Typing.Column]:
         columns: SQLite3PragmaTableInfo = self._sqlite_execute(
             f"PRAGMA table_info({table_name});"
         )
+        """
+        When given a table name, returns a list of Column objects inside it.
+        """
 
         return [
             SQLite3Typing.Column(
                 name=name,
                 data_type=cast(SQLite3Typing.DataTypes, data_type),
                 column_constraints=[
                     cast(c.ColumnSpecificConstraint, constraint)
@@ -155,15 +166,15 @@
                 ],
             )
             for _, name, data_type, notnull, _, pk in columns
         ]
 
     def _sqlite_execute(self, query: str):
         """
-        Execute a query in the SQLite3 database, rutrns its result.
+        Execute a query in the SQLite3 database, returns its result.
         """
 
         db_path = self.config.db_path
         with sqlite3.connect(db_path) as conn:
             cursor = conn.cursor()
             cursor.execute(query)
             conn.commit()
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/operations/column_operations.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/operations/column_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/operations/table_operations.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/operations/table_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,29 +4,60 @@
 from skibidi_orm.migration_engine.operations.column_operations import ColumnOperation
 from skibidi_orm.migration_engine.operations.table_operations import TableOperation
 
 from skibidi_orm.migration_engine.converters.sqlite3.all import SQLite3Converter
 
 
 class SQLite3Executor(BaseSQLExecutor):
+    """
+    Executes SQL statements and operations on a SQLite3 database.
+
+    This class provides methods to execute SQL statements and operations on a SQLite3 database.
+    It inherits from the BaseSQLExecutor class.
+
+    Methods:
+        execute_sql: Executes a single SQL statement.
+        execute_operations: Executes a list of table or column operations.
+
+    """
 
     @staticmethod
     def execute_sql(sql: str):
+        """
+        Executes a single SQL statement.
+
+        Args:
+            sql (str): The SQL statement to be executed.
+
+        Returns:
+            None
+
+        """
         sqlite_config = SQLite3Config.get_instance()
         with sqlite3.connect(sqlite_config.db_path) as conn:
             cursor = conn.cursor()
             commands = sql.split(";")
             for command in commands:
                 if not command:
                     continue
                 cursor.execute(command.strip())
             conn.commit()
 
     @staticmethod
     def execute_operations(operations: list[TableOperation | ColumnOperation]):
+        """
+        Executes a list of table or column operations.
+
+        Args:
+            operations (list[TableOperation | ColumnOperation]): The list of table or column operations to be executed.
+
+        Returns:
+            None
+
+        """
         for operation in operations:
             if isinstance(operation, TableOperation):
                 SQLite3Executor.execute_sql(
                     SQLite3Converter.convert_table_operation_to_SQL(operation)
                 )
             else:
                 SQLite3Executor.execute_sql(
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/state_manager/state_manager.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/state_manager/state_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,48 +16,70 @@
     RenameTableOperation,
 )
 
 from skibidi_orm.migration_engine.state_manager.i_state_manager import IStateManager
 
 
 class StateManager[TTable: BaseTable[BaseColumn[Any]]](IStateManager):
+    """
+    Class that will analyze the differences between the database schema and the class structure defined schema
+    when instantiated.
+
+    It can provide a list of operations needed to transform the schema of the database to be equivalent with the
+    one defined via python objects and migration files.
+    """
+
     def __init__(
         self,
         db_tables: list[TTable],
         schema_tables: list[TTable],
     ) -> None:
         self.db_tables = db_tables
         self.schema_tables = schema_tables
 
         self.serviced_tables: list[TTable] = []
 
         self.operations: list[TableOperation | ColumnOperation] = []
 
-        self.analyze_schemas()
+        self._analyze_schemas()
 
-    def analyze_schemas(self):
-        self.get_delete_tables_operations()
-        self.get_create_tables_operations()
-        self.get_delete_columns_operations()
-        self.get_create_columns_operations()
+    def _analyze_schemas(self):
+        """
+        Call helper functions to retrieve all operations needed for database transformation.
+        """
+        self._get_delete_tables_operations()
+        self._get_create_tables_operations()
+        self._get_delete_columns_operations()
+        self._get_create_columns_operations()
 
-    def get_operations(self) -> list[TableOperation | ColumnOperation]:
+    def get_operations_transforming_database_schema_into_class_hierarchy_schema(
+        self,
+    ) -> list[TableOperation | ColumnOperation]:
+        """
+        Return operations required for transforming the database calculated by the schema analysis.
+        """
         return self.operations
 
-    def get_create_tables_operations(self) -> None:
+    def _get_create_tables_operations(self) -> None:
+        """
+        Get operations concerning the creation of new tables.
+        """
 
         t_db_names = set([t.name for t in self.db_tables])
 
         for s_table in self.schema_tables:
             if s_table.name not in t_db_names:
                 if s_table not in self.serviced_tables:
                     self.operations.append(CreateTableOperation(s_table))
                     self.serviced_tables.append(s_table)
 
-    def get_delete_tables_operations(self) -> None:
+    def _get_delete_tables_operations(self) -> None:
+        """
+        Get operations concerning the deletion of tables.
+        """
 
         class TableFound(Exception):
             pass
 
         t_schema_names = set([t.name for t in self.schema_tables])
         for db_table in self.db_tables:
             try:
@@ -74,15 +96,18 @@
                             raise TableFound
                     if db_table not in self.serviced_tables:
                         self.operations.append(DeleteTableOperation(db_table))
                         self.serviced_tables.append(db_table)
             except TableFound:
                 pass
 
-    def get_create_columns_operations(self):
+    def _get_create_columns_operations(self):
+        """
+        Get operations concerning the creation of new columns.
+        """
 
         db_table_dict = {t.name: t for t in self.db_tables}
         schema_table_dict = {t.name: t for t in self.schema_tables}
 
         for s_table_name, s_table in schema_table_dict.items():
             if s_table not in self.serviced_tables:
                 if s_table_name in db_table_dict.keys():
@@ -94,15 +119,18 @@
                         if s_column not in table_db_columns:
                             self.operations.append(
                                 AddColumnOperation(
                                     db_table_dict[s_table_name], s_column
                                 )
                             )
 
-    def get_delete_columns_operations(self):
+    def _get_delete_columns_operations(self):
+        """
+        Get operations concerning the deletion of columns.
+        """
 
         db_table_dict = {t.name: t for t in self.db_tables}
         schema_table_dict = {t.name: t for t in self.schema_tables}
 
         for db_table_name, db_table in db_table_dict.items():
             if db_table not in self.serviced_tables:
                 if db_table_name in schema_table_dict.keys():
@@ -116,8 +144,8 @@
                                 DeleteColumnOperation(db_table, db_column)
                             )
 
     # def get_relations_operations(self):
     #     # TODO: implement using foreign keys
     #     for relation in self.schema_relations:
     #         if relation not in self.db_relations:
-    #             pass  # add crea
+    #             pass
```

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/server.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/server.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/src/skibidi_orm/migration_engine/table_example.py` & `skibidi_orm-0.1.1/src/skibidi_orm/migration_engine/table_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Example of how Table class and classes modeling DB schema can be implemented
 from skibidi_orm.migration_engine.adapters.base_adapter import BaseAdapter
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import (
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.adapters.sqlite3_adapter import SQLite3Adapter
 import skibidi_orm.migration_engine.adapters.database_objects.constraints as c
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/cli/test_run.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pytest import raises
 from skibidi_orm.exceptions.operations import UnsupportedOperationError
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import SQLite3Typing
-from skibidi_orm.migration_engine.converters.sqlite3.columns import SQLite3ColumnOperationConverter
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import SQLite3Typing
+from skibidi_orm.migration_engine.converters.sqlite3.columns import (
+    SQLite3ColumnOperationConverter,
+)
 from skibidi_orm.migration_engine.operations.column_operations import (
     AddColumnOperation,
     ChangeDataTypeOperation,
     DeleteColumnOperation,
     RenameColumnOperation,
 )
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pytest
 
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import SQLite3Typing
-from skibidi_orm.migration_engine.converters.sqlite3.tables import SQLite3TableOperationConverter
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import SQLite3Typing
+from skibidi_orm.migration_engine.converters.sqlite3.tables import (
+    SQLite3TableOperationConverter,
+)
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     CheckConstraint,
     Constraint,
     ConstraintType,
     ForeignKeyConstraint,
     PrimaryKeyConstraint,
     UniqueConstraint,
@@ -125,15 +127,15 @@
 def test_create_table_conversion_complex_with_constraints():
     """Create a complex table with multiple constraints"""
     operation = CreateTableOperation(complex_table_with_constraints)
     assert (
         SQLite3TableOperationConverter.convert_table_operation_to_SQL(operation)
         == "CREATE TABLE admin_users (user_id INTEGER PRIMARY KEY NOT NULL, name TEXT, "
         "email TEXT UNIQUE, active BLOB, age INTEGER, CHECK (age > 18), FOREIGN KEY (active, name) REFERENCES users ("
-           "active, name));"
+        "active, name));"
     )
 
 
 def test_delete_table_conversion():
     """Delete a simple table"""
     operation = DeleteTableOperation(simple_table_no_constraints)
     assert (
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_config/test_config.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/db_config/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,15 @@
 
 def test_should_raise_error_when_instantiating_other_config():
     """
     Should raise error when trying to instantiate other config after one has been instantiated
     """
     SQLite3Config(db_path="first_path")
     with pytest.raises(RuntimeError) as exc_info:
-        PostgresConfig(
-            db_name="db_name",
-            db_user="db_user",
-            db_password="db_password",
-            db_host="db_host",
-            db_port=5432,
-        )
+        PostgresConfig(db_path="first_path")
     assert str(exc_info.value) == "Only one instance of this class is allowed"
 
 
 def test_accessing_through_instance_method_should_throw_error_when_instance_does_not_exist():
     """
     Should raise error when trying to access instance method when instance does not exist
     """
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,34 +2,60 @@
 import pytest
 
 from skibidi_orm.exceptions.db_mutator_exceptions import AmbigiousDeleteRowError
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     NotNullConstraint,
     PrimaryKeyConstraint,
 )
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import (
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.data_mutator.base_data_mutator import (
     DeleteRowPk,
     InsertRowColumn,
 )
 from skibidi_orm.migration_engine.data_mutator.sqlite3_data_mutatorr import (
     SQLite3DataMutator,
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
-from ..sql_data import SQLite3InsertData, SQLite3TablesData
 
+sql_simple_db = [
+    """
+    CREATE TABLE users (
+        user_id INTEGER PRIMARY KEY,
+        username TEXT NOT NULL
+    );
+"""
+]
+
+sql_double_pk_db = [
+    """
+    CREATE TABLE Orders (
+        order_id INTEGER,
+        product_id INTEGER,
+        PRIMARY KEY (order_id, product_id)
+    );
+"""
+]
+
+sql_simple_insert = [
+    """
+    INSERT INTO users (user_id, username) VALUES
+    (1, 'test1'),
+    (2, 'test2'),
+    (3, 'test3')
+;
+"""
+]
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
-)
+
+@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
 def test_insert_row(make_database: str):
     SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="users",
         row=[
             InsertRowColumn(name="user_id", value=str(1)),
@@ -56,17 +82,15 @@
                     NotNullConstraint(table_name="users", column_name="username"),
                 ],
             ),
         ],
     )
 
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
-)
+@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
 def test_delete_row_one_pk(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
 
     db_seeder.insert_row(
         table_name="users",
         row=[
@@ -95,17 +119,15 @@
         cursor.execute("SELECT * FROM users")
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 0
 
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
-)
+@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
 def test_delete_row_two_pk(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -134,17 +156,15 @@
         cursor.execute("SELECT * FROM Orders")
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 0
 
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
-)
+@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
 def test_delete_row_table_two_pk_one_pk_given_ok(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -180,17 +200,15 @@
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 1
     assert data[0] == (1, 1)
 
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
-)
+@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
 def test_delete_row_table_two_pk_two_pk_given_ok(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -227,17 +245,15 @@
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 1
     assert data[0] == (1, 1)
 
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
-)
+@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
 def test_delete_row_table_two_pk_one_pk_given_ambigious(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -266,57 +282,49 @@
             pks=[
                 DeleteRowPk(name="order_id", value=str(1)),
             ],
         )
 
 
 @pytest.mark.parametrize(
-    "make_database",
-    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
-    indirect=True,
+    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
 )
 def test_raw_query(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.raw_query("SELECT * FROM users;")
     assert data == [(1, "test1"), (2, "test2"), (3, "test3")]
 
 
 @pytest.mark.parametrize(
-    "make_database",
-    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
-    indirect=True,
+    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
 )
 def test_get_rows_normal(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.get_rows("users")
     assert data == [(1, "test1"), (2, "test2"), (3, "test3")]
 
 
 @pytest.mark.parametrize(
-    "make_database",
-    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
-    indirect=True,
+    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
 )
 def test_get_rows_offset(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.get_rows("users", offset=1)
     assert data == [(2, "test2"), (3, "test3")]
     data = db_mutator.get_rows("users", offset=2)
     assert data == [(3, "test3")]
     data = db_mutator.get_rows("users", offset=3)
     assert data == []
 
 
 @pytest.mark.parametrize(
-    "make_database",
-    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
-    indirect=True,
+    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
 )
 def test_get_rows_limit(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.get_rows("users", limit=1)
     assert data == [(1, "test1")]
     data = db_mutator.get_rows("users", limit=2)
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/operations/test_operations.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/operations/test_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import (
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.adapters.sqlite3_adapter import SQLite3Adapter
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
 
 from skibidi_orm.migration_engine.adapters.database_objects import constraints as c
@@ -21,15 +21,75 @@
 )
 
 # from tmp.mock_schema import Table
 
 from pathlib import Path
 import pytest
 import sqlite3
-from ..sql_data import SQLite3TablesData
+
+sql_table_user = """
+    CREATE TABLE User (
+        user_id INTEGER PRIMARY KEY,
+        user_name TEXT NOT NULL
+    );
+"""
+sql_table_post = """
+    CREATE TABLE Post (
+        post_id INTEGER PRIMARY KEY,
+        post_name TEXT NOT NULL
+    );
+"""
+
+sql_table_comment = """
+    CREATE TABLE Comment (
+        comment_id INTEGER PRIMARY KEY,
+        comment_name TEXT NOT NULL
+    );
+"""
+
+sql_table_primary_key_not_null = """
+    CREATE TABLE table_primary_key_not_null (
+        id INTEGER PRIMARY KEY NOT NULL
+    );
+"""
+
+
+# TODO: what is this?
+# sql_schema_with_fks = [
+#     """
+#     CREATE TABLE users (
+#         user_id INTEGER PRIMARY KEY,
+#         username TEXT NOT NULL UNIQUE,
+#         email TEXT NOT NULL UNIQUE,
+#         password_hash TEXT NOT NULL,
+#         registration_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
+#     );
+# """,
+#     """
+#     CREATE TABLE posts (
+#         post_id INTEGER PRIMARY KEY,
+#         user_id INTEGER NOT NULL,
+#         title TEXT NOT NULL,
+#         content TEXT NOT NULL,
+#         post_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
+#         FOREIGN KEY (user_id) REFERENCES users(user_id)
+#     );
+# """,
+#     """
+#     CREATE TABLE comments (
+#         comment_id INTEGER PRIMARY KEY,
+#         user_idd INTEGER NOT NULL,
+#         post_id INTEGER NOT NULL,
+#         comment_text TEXT NOT NULL,
+#         comment_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
+#         FOREIGN KEY (user_idd) REFERENCES users(user_id),
+#         FOREIGN KEY (post_id) REFERENCES posts(post_id)
+#     );
+# """,
+# ]
 
 
 def execute_sqlite3_commands(db_path: str, commands: list[str]):
     """Executes the given commands in a SQLite DB living under db_path"""
     with sqlite3.connect(db_path) as conn:
         cursor = conn.cursor()
         for command in commands:
@@ -63,17 +123,15 @@
         SQLite3Executor,
         "execute_operations",
         do_nothing,  # type: ignore
     )
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
 )
 def test_rename_table_operation_needed(
     tmp_database: str, capfd: pytest.CaptureFixture[str]
 ):
     from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
         MigrationElement,
     )
@@ -126,17 +184,15 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == RenameTableOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
 )
 def test_no_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
     # TODO: refactor to avoid duplicating the setup multiple times
     class Table(MigrationElement):
 
@@ -185,17 +241,15 @@
     m = MigrationElement()
     m.migrate(preview=True)
 
     assert len(MigrationElement.operations) == 0
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
 )
 def test_create_table_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -262,23 +316,15 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == CreateTableOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [
-        [
-            SQLite3TablesData.sql_table_user,
-            SQLite3TablesData.sql_table_post,
-            SQLite3TablesData.sql_table_comment,
-        ]
-    ],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post, sql_table_comment]], indirect=True
 )
 def test_delete_table_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -328,17 +374,15 @@
     m.migrate(preview=True)
 
     assert len(MigrationElement.operations) == 1
     assert type(MigrationElement.operations[0]) == DeleteTableOperation
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
 )
 def test_create_column_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -393,17 +437,15 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == AddColumnOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
 )
 def test_delete_column_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -448,23 +490,15 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == DeleteColumnOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database",
-    [
-        [
-            SQLite3TablesData.sql_table_user,
-            SQLite3TablesData.sql_table_post,
-            SQLite3TablesData.sql_table_comment,
-        ]
-    ],
-    indirect=True,
+    "tmp_database", [[sql_table_user, sql_table_post, sql_table_comment]], indirect=True
 )
 def test_add_column_and_delete_tabe_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
     class Table(MigrationElement):
 
         def __init__(self) -> None:
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/studio/test_routes.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/studio/test_routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,22 +7,62 @@
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.studio.server import app
 import pathlib
-from ..sql_data import SQLite3TablesData
+
 
 client = TestClient(app)
 
+sql_schema_with_fks = [
+    """
+    CREATE TABLE users (
+        user_id INTEGER PRIMARY KEY,
+        username TEXT NOT NULL UNIQUE,
+        email TEXT NOT NULL UNIQUE,
+        password_hash TEXT NOT NULL,
+        registration_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
+    );
+""",
+    """
+    CREATE TABLE posts (
+        post_id INTEGER PRIMARY KEY,
+        user_id INTEGER NOT NULL,
+        title TEXT NOT NULL,
+        content TEXT NOT NULL,
+        post_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
+        FOREIGN KEY (user_id) REFERENCES users(user_id)
+    );
+""",
+    """
+    CREATE TABLE comments (
+        comment_id INTEGER PRIMARY KEY,
+        user_idd INTEGER NOT NULL,
+        post_id INTEGER NOT NULL,
+        comment_text TEXT NOT NULL,
+        comment_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
+        FOREIGN KEY (user_idd) REFERENCES users(user_id),
+        FOREIGN KEY (post_id) REFERENCES posts(post_id)
+    );
+""",
+]
+
+sql_simple_db = [
+    """
+    CREATE TABLE users (
+        user_id INTEGER PRIMARY KEY,
+        username TEXT NOT NULL UNIQUE
+    );
+"""
+]
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
-)
+
+@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
 def test_GET_db(
     monkeypatch: pytest.MonkeyPatch, tmp_path: pathlib.Path, make_database: str
 ):
     import skibidi_orm.migration_engine.studio.server  # type: ignore
 
     importlib.import_module("skibidi_orm.migration_engine.studio.server")
 
@@ -64,17 +104,15 @@
                     ],
                 }
             ]
         }
     )
 
 
-@pytest.mark.parametrize(
-    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
-)
+@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
 def test_POST_route_db_table_name_row_correct(
     monkeypatch: pytest.MonkeyPatch, make_database: str
 ):
     import skibidi_orm.migration_engine.studio.server  # type: ignore
 
     importlib.import_module("skibidi_orm.migration_engine.studio.server")
```

### Comparing `skibidi_orm-0.1.0/tests/skibidi-orm/migration_engine/test_module_cooperation.py` & `skibidi_orm-0.1.1/tests/skibidi-orm/migration_engine/test_module_cooperation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,53 @@
-from skibidi_orm.migration_engine.adapters.database_objects.sqlite3_typing import (
+from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
 from skibidi_orm.migration_engine.adapters.sqlite3_adapter import SQLite3Adapter
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
 from skibidi_orm.migration_engine.adapters.database_objects import constraints as c
-from .sql_data import SQLite3TablesData
+
+
+sql_table_user = """
+    CREATE TABLE User (
+        user_id INTEGER PRIMARY KEY,
+        user_name TEXT NOT NULL
+    );
+"""
+sql_table_post = """
+    CREATE TABLE Post (
+        post_id INTEGER PRIMARY KEY,
+        post_name TEXT NOT NULL
+    );
+"""
+
+sql_table_comment = """
+    CREATE TABLE Comment (
+        comment_id INTEGER PRIMARY KEY,
+        comment_name TEXT NOT NULL
+    );
+"""
+
+sql_table_primary_key_not_null = """
+    CREATE TABLE table_primary_key_not_null (
+        id INTEGER PRIMARY KEY NOT NULL
+    );
+"""
 
 
 def test_adding_table_to_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
+    SQLite3Executor.execute_sql(sql_table_user)
+    SQLite3Executor.execute_sql(sql_table_post)
 
     class Table(MigrationElement):
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
             if self.__class__ == Table:
@@ -94,17 +120,17 @@
     assert tables[2].columns[1].column_constraints == [
         c.NotNullConstraint("Comment", "comment_name")
     ]
 
 
 def test_removing_table_from_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_comment)
+    SQLite3Executor.execute_sql(sql_table_user)
+    SQLite3Executor.execute_sql(sql_table_post)
+    SQLite3Executor.execute_sql(sql_table_comment)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
@@ -175,16 +201,16 @@
     assert tables[1].columns[1].column_constraints == [
         c.NotNullConstraint("Post", "post_name")
     ]
 
 
 def test_add_column_to_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
+    SQLite3Executor.execute_sql(sql_table_user)
+    SQLite3Executor.execute_sql(sql_table_post)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
@@ -265,16 +291,16 @@
     assert tables[1].columns[2].column_constraints == [
         c.NotNullConstraint("Post", "post_content")
     ]
 
 
 def test_removing_column_from_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
+    SQLite3Executor.execute_sql(sql_table_user)
+    SQLite3Executor.execute_sql(sql_table_post)
 
     class Table(MigrationElement):
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
             if self.__class__ == Table:
@@ -335,16 +361,16 @@
     assert tables[1].columns[0].column_constraints == [
         c.PrimaryKeyConstraint("Post", "post_id")
     ]
 
 
 def test_renaming_table_in_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
+    SQLite3Executor.execute_sql(sql_table_user)
+    SQLite3Executor.execute_sql(sql_table_post)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
@@ -413,17 +439,17 @@
     assert tables[1].columns[1].column_constraints == [
         c.NotNullConstraint("NewNamePost", "post_name")
     ]
 
 
 def test_add_column_to_database_and_remove_table_from_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
-    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_comment)
+    SQLite3Executor.execute_sql(sql_table_user)
+    SQLite3Executor.execute_sql(sql_table_post)
+    SQLite3Executor.execute_sql(sql_table_comment)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
```

