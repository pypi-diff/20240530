# Comparing `tmp/dbt-fabric-1.8.5.tar.gz` & `tmp/dbt-fabric-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.8.5.tar", last modified: Mon May 20 17:08:11 2024, max compression
+gzip compressed data, was "dbt-fabric-1.8.6.tar", last modified: Thu May 30 21:50:36 2024, max compression
```

## Comparing `dbt-fabric-1.8.5.tar` & `dbt-fabric-1.8.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.535967 dbt-fabric-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-20 17:08:11.535967 dbt-fabric-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.523968 dbt-fabric-1.8.5/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.523968 dbt-fabric-1.8.5/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.527968 dbt-fabric-1.8.5/dbt/adapters/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.527968 dbt-fabric-1.8.5/dbt/adapters/fabric/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/adapters/fabric/relation_configs/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.523968 dbt-fabric-1.8.5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.527968 dbt-fabric-1.8.5/dbt/include/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.523968 dbt-fabric-1.8.5/dbt/include/fabric/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.527968 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/show.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.523968 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.523968 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.527968 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.531967 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.531967 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.531967 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.531967 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.531967 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.531967 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/get_tables_by_pattern.sql
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/dbt/include/fabric/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:08:11.535967 dbt-fabric-1.8.5/dbt_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-20 17:08:11.000000 dbt-fabric-1.8.5/dbt_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 17:08:11.000000 dbt-fabric-1.8.5/dbt_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:08:11.000000 dbt-fabric-1.8.5/dbt_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-20 17:08:11.000000 dbt-fabric-1.8.5/dbt_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 17:08:11.000000 dbt-fabric-1.8.5/dbt_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:08:11.535967 dbt-fabric-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-20 17:07:32.000000 dbt-fabric-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.395278 dbt-fabric-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-30 21:50:36.395278 dbt-fabric-1.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.383278 dbt-fabric-1.8.6/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.383278 dbt-fabric-1.8.6/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.387278 dbt-fabric-1.8.6/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16745 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.387278 dbt-fabric-1.8.6/dbt/adapters/fabric/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/adapters/fabric/relation_configs/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.383278 dbt-fabric-1.8.6/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.387278 dbt-fabric-1.8.6/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.383278 dbt-fabric-1.8.6/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.387278 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.383278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.383278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.387278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.391278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.391278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.391278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.391278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.391278 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.391278 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/get_tables_by_pattern.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:50:36.395278 dbt-fabric-1.8.6/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-30 21:50:36.000000 dbt-fabric-1.8.6/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-30 21:50:36.000000 dbt-fabric-1.8.6/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:50:36.000000 dbt-fabric-1.8.6/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 21:50:36.000000 dbt-fabric-1.8.6/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 21:50:36.000000 dbt-fabric-1.8.6/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:50:36.395278 dbt-fabric-1.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-30 21:49:54.000000 dbt-fabric-1.8.6/setup.py
```

### Comparing `dbt-fabric-1.8.5/LICENSE` & `dbt-fabric-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/PKG-INFO` & `dbt-fabric-1.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.5
+Version: 1.8.6
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.5/README.md` & `dbt-fabric-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,20 @@
             # SQL Server named instance. In this case then port number has to be omitted.
             con_str.append(f"SERVER={credentials.host}")
         else:
             con_str.append(f"SERVER={credentials.host}")
 
         con_str.append(f"Database={credentials.database}")
 
+        #Enabling trace flag
+        if credentials.trace_flag:
+            con_str.append("SQL_ATTR_TRACE=SQL_OPT_TRACE_ON")
+        else:
+            con_str.append("SQL_ATTR_TRACE=SQL_OPT_TRACE_OFF")
+
         assert credentials.authentication is not None
 
         if "ActiveDirectory" in credentials.authentication:
             con_str.append(f"Authentication={credentials.authentication}")
 
             if credentials.authentication == "ActiveDirectoryPassword":
                 con_str.append(f"UID={{{credentials.UID}}}")
```

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     driver: str
     host: str
     database: str
     schema: str
     UID: Optional[str] = None
     PWD: Optional[str] = None
     windows_login: Optional[bool] = False
+    trace_flag: Optional[bool] = False
     tenant_id: Optional[str] = None
     client_id: Optional[str] = None
     client_secret: Optional[str] = None
     authentication: Optional[str] = "ActiveDirectoryServicePrincipal"
     encrypt: Optional[bool] = True  # default value in MS ODBC Driver 18 as well
     trust_cert: Optional[bool] = False  # default value in MS ODBC Driver 18 as well
     retries: int = 1
@@ -32,14 +33,15 @@
         "server": "host",
         "trusted_connection": "windows_login",
         "auth": "authentication",
         "app_id": "client_id",
         "app_secret": "client_secret",
         "TrustServerCertificate": "trust_cert",
         "schema_auth": "schema_authorization",
+        "SQL_ATTR_TRACE": "trace_flag",
     }
 
     @property
     def type(self):
         return "fabric"
 
     def _connection_keys(self):
@@ -59,12 +61,13 @@
             "client_id",
             "authentication",
             "encrypt",
             "trust_cert",
             "retries",
             "login_timeout",
             "query_timeout",
+            "trace_flag",
         )
 
     @property
     def unique_field(self):
         return self.host
```

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/fabric_relation.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/fabric_relation.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/adapters/fabric/relation_configs/base.py` & `dbt-fabric-1.8.6/dbt/adapters/fabric/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/catalog.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     {% endcall %}
 
     {{ return(load_result('get_columns_in_query').table.columns | map(attribute='name') | list) }}
 {% endmacro %}
 
 {% macro fabric__alter_column_type(relation, column_name, new_column_type) %}
 
-    {%- set table_name= tmp_relation.include(database=False).include(schema=False)-%}
-    {%- set schema_name = tmp_relation.include(database=False).include(identifier=False) -%}
+    {%- set table_name= relation.identifier -%}
+    {%- set schema_name = relation.schema -%}
 
     {% set generate_tmp_relation_script %}
         SELECT TRIM(REPLACE(STRING_AGG(ColumnName + ' ', ',-'), '-', CHAR(10)))  AS ColumnDef
         FROM
         (
             SELECT
             CAST(c.COLUMN_NAME AS VARCHAR) AS ColumnName
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 {% macro default__information_schema_hints() %}{% endmacro %}
 {% macro fabric__information_schema_hints() %}{% endmacro %}
 
 {% macro fabric__information_schema_name(database) -%}
   information_schema
 {%- endmacro %}
 
+{% macro get_use_database_sql(database) %}
+    {{ return(adapter.dispatch('get_use_database_sql', 'dbt')(database)) }}
+{% endmacro %}
+
+{%- macro fabric__get_use_database_sql(database) -%}
+  USE [{{database}}];
+{%- endmacro -%}
+
 {% macro fabric__list_schemas(database) %}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
     select  name as [schema]
     from sys.schemas {{ information_schema_hints() }}
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
@@ -23,15 +31,15 @@
     SELECT count(*) as schema_exist FROM sys.schemas WHERE name = '{{ schema }}'
   {%- endcall %}
   {{ return(load_result('check_schema_exists').table) }}
 {% endmacro %}
 
 {% macro fabric__list_relations_without_caching(schema_relation) -%}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
-    USE [{{ schema_relation.database }}];
+    {{ get_use_database_sql(schema_relation.database) }}
     with base as (
       select
         DB_NAME() as [database],
         t.name as [name],
         SCHEMA_NAME(t.schema_id) as [schema],
         'table' as table_type
       from sys.tables as t {{ information_schema_hints() }}
@@ -47,15 +55,15 @@
     where [schema] like '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 {% macro fabric__get_relation_without_caching(schema_relation) -%}
   {% call statement('get_relation_without_caching', fetch_result=True) -%}
-    USE [{{ schema_relation.database }}];
+    {{ get_use_database_sql(schema_relation.database) }}
     with base as (
       select
         DB_NAME() as [database],
         t.name as [name],
         SCHEMA_NAME(t.schema_id) as [schema],
         'table' as table_type
       from sys.tables as t {{ information_schema_hints() }}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/relation.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/relation.sql`

 * *Files 10% similar despite different names*

```diff
@@ -2,59 +2,52 @@
     {%- set temp_identifier = base_relation.identifier ~ suffix -%}
     {%- set temp_relation = base_relation.incorporate(
                                 path={"identifier": temp_identifier}) -%}
 
     {{ return(temp_relation) }}
 {% endmacro %}
 
-{% macro fabric__drop_relation(relation) -%}
-  {% call statement('drop_relation', auto_begin=False) -%}
-    {{ fabric__drop_relation_script(relation) }}
-  {%- endcall %}
-{% endmacro %}
-
-{% macro fabric__drop_relation_script(relation) -%}
-
-    {% if relation.type == 'view' -%}
+{% macro fabric__get_drop_sql(relation) -%}
+  {% if relation.type == 'view' -%}
       {% call statement('find_references', fetch_result=true) %}
-      USE [{{ relation.database }}];
-      select
-          sch.name as schema_name,
-          obj.name as view_name
-      from sys.sql_expression_dependencies refs
-      inner join sys.objects obj
-      on refs.referencing_id = obj.object_id
-      inner join sys.schemas sch
-      on obj.schema_id = sch.schema_id
-      where refs.referenced_database_name = '{{ relation.database }}'
-      and refs.referenced_schema_name = '{{ relation.schema }}'
-      and refs.referenced_entity_name = '{{ relation.identifier }}'
-      and refs.referencing_class = 1
-      and obj.type = 'V'
+        {{ get_use_database_sql(relation.database) }}
+        select
+            sch.name as schema_name,
+            obj.name as view_name
+        from sys.sql_expression_dependencies refs
+        inner join sys.objects obj
+        on refs.referencing_id = obj.object_id
+        inner join sys.schemas sch
+        on obj.schema_id = sch.schema_id
+        where refs.referenced_database_name = '{{ relation.database }}'
+        and refs.referenced_schema_name = '{{ relation.schema }}'
+        and refs.referenced_entity_name = '{{ relation.identifier }}'
+        and refs.referencing_class = 1
+        and obj.type = 'V'
       {% endcall %}
       {% set references = load_result('find_references')['data'] %}
       {% for reference in references -%}
-      -- dropping referenced view {{ reference[0] }}.{{ reference[1] }}
-      {{ fabric__drop_relation_script(relation.incorporate(
-          type="view",
-          path={"schema": reference[0], "identifier": reference[1]})) }}
+        -- dropping referenced view {{ reference[0] }}.{{ reference[1] }}
+        {% do adapter.drop_relation
+          (api.Relation.create(
+            identifier = reference[1], schema = reference[0], database = relation.database, type='view'
+          ))%}
       {% endfor %}
     {% elif relation.type == 'table'%}
       {% set object_id_type = 'U' %}
-
     {%- else -%}
         {{ exceptions.raise_not_implemented('Invalid relation being dropped: ' ~ relation) }}
     {% endif %}
-    USE [{{ relation.database }}];
+    {{ get_use_database_sql(relation.database) }}
     EXEC('DROP {{ relation.type }} IF EXISTS {{ relation.include(database=False) }};');
 {% endmacro %}
 
 {% macro fabric__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
-     USE [{{ from_relation.database }}];
+     {{ get_use_database_sql(from_relation.database) }}
       EXEC sp_rename '{{ from_relation.schema }}.{{ from_relation.identifier }}', '{{ to_relation.identifier }}'
   {%- endcall %}
 {% endmacro %}
 
 -- DROP fabric__truncate_relation when TRUNCATE TABLE is supported
 {% macro fabric__truncate_relation(relation) -%}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     EXEC('CREATE SCHEMA [{{ relation.schema }}]')
     END
   {% endcall %}
 {% endmacro %}
 
 {% macro fabric__create_schema_with_authorization(relation, schema_authorization) -%}
   {% call statement('create_schema') -%}
-    USE [{{ relation.database }}];
+    {{ get_use_database_sql(relation.database) }}
     IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = '{{ relation.schema }}')
     BEGIN
     EXEC('CREATE SCHEMA [{{ relation.schema }}] AUTHORIZATION [{{ schema_authorization }}]')
     END
   {% endcall %}
 {% endmacro %}
 
@@ -23,14 +23,14 @@
 
   {% for row in relations_in_schema %}
     {%- set schema_relation = api.Relation.create(database=relation.database,
                                                schema=relation.schema,
                                                identifier=row[1],
                                                type=row[3]
                                                ) -%}
-    {% do drop_relation(schema_relation) %}
+    {% do adapter.drop_relation(schema_relation) %}
   {%- endfor %}
 
   {% call statement('drop_schema') -%}
       EXEC('DROP SCHEMA IF EXISTS {{ relation.schema }}')
   {% endcall %}
 {% endmacro %}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,63 @@
-
 {% materialization incremental, adapter='fabric' -%}
 
   {%- set full_refresh_mode = (should_full_refresh()) -%}
   {% set target_relation = this.incorporate(type='table') %}
-  {%- set relations_list = fabric__get_relation_without_caching(target_relation) -%}
+  {%- set relation = load_cached_relation(this) -%}
 
   {%- set existing_relation = none %}
-  {% if (relations_list|length == 1) and (relations_list[0][2] == target_relation.schema)
-        and (relations_list[0][1] ==  target_relation.identifier) and  (relations_list[0][3] ==  target_relation.type)%}
+  {% if relation.type ==  'table' %}
     {% set existing_relation = target_relation %}
-  {% elif (relations_list|length == 1) and (relations_list[0][2] == target_relation.schema)
-        and (relations_list[0][1] ==  target_relation.identifier) and  (relations_list[0][3] !=  target_relation.type) %}
-      {% set existing_relation = get_or_create_relation(relations_list[0][0], relations_list[0][2] , relations_list[0][1] , relations_list[0][3])[1] %}
+  {% elif relation.type ==  'view' %}
+    {% set existing_relation = get_or_create_relation(relation.database, relation.schema, relation.identifier, relation.type)[1] %}
   {% endif %}
 
-  {{ log("Full refresh mode" ~ full_refresh_mode)}}
-  {{ log("existing relation : "~existing_relation ~ " type  "~ existing_relation.type ~ " is view?  "~existing_relation.is_view)  }}
-  {{ log("target relation: " ~target_relation ~ " type  "~ target_relation.type ~ " is view?  "~target_relation.is_view) }}
-
   -- configs
   {%- set unique_key = config.get('unique_key') -%}
   {% set incremental_strategy = config.get('incremental_strategy') or 'default' %}
   {%- set temp_relation = make_temp_relation(target_relation)-%}
 
   {% set grant_config = config.get('grants') %}
   {%- set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') -%}
 
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
-  {% if existing_relation is none %}
+  -- naming a temp relation
+  {% set tmp_relation_view = target_relation.incorporate(path={"identifier": target_relation.identifier ~ '__dbt_tmp_vw'}, type='view')-%}
 
+  -- Fabric & Synapse adapters use temp relation because of lack of CTE support for CTE in CTAS, Insert
+  -- drop temp relation if exists
+  {% do adapter.drop_relation(tmp_relation_view) %}
+
+  {% if existing_relation is none %}
     {%- call statement('main') -%}
-      {{ fabric__create_table_as(False, target_relation, sql)}}
+      {{ get_create_table_as_sql(False, target_relation, sql)}}
     {%- endcall -%}
 
   {% elif existing_relation.is_view %}
-
     {#-- Can't overwrite a view with a table - we must drop --#}
     {{ log("Dropping relation " ~ target_relation ~ " because it is a view and this model is a table.") }}
-    {{ drop_relation_if_exists(existing_relation) }}
+    {% do adapter.drop_relation(existing_relation) %}
+
     {%- call statement('main') -%}
-      {{ fabric__create_table_as(False, target_relation, sql)}}
+      {{ get_create_table_as_sql(False, target_relation, sql)}}
     {%- endcall -%}
 
   {% elif full_refresh_mode %}
-
     {%- call statement('main') -%}
-      {{ fabric__create_table_as(False, target_relation, sql)}}
+      {{ get_create_table_as_sql(False, target_relation, sql)}}
     {%- endcall -%}
 
   {% else %}
-
     {%- call statement('create_tmp_relation') -%}
-      {{ fabric__create_table_as(True, temp_relation, sql)}}
+      {{ get_create_table_as_sql(True, temp_relation, sql)}}
     {%- endcall -%}
     {% do adapter.expand_target_column_types(
-             from_relation=temp_relation,
-             to_relation=target_relation) %}
+              from_relation=temp_relation,
+              to_relation=target_relation) %}
     {#-- Process schema changes. Returns dict of changes if successful. Use source columns for upserting/merging --#}
     {% set dest_columns = process_schema_changes(on_schema_change, temp_relation, existing_relation) %}
     {% if not dest_columns %}
       {% set dest_columns = adapter.get_columns_in_relation(existing_relation) %}
     {% endif %}
 
     {#-- Get the incremental_strategy, the macro to use for the strategy, and build the sql --#}
@@ -68,20 +65,18 @@
     {% set strategy_sql_macro_func = adapter.get_incremental_strategy_macro(context, incremental_strategy) %}
     {% set strategy_arg_dict = ({'target_relation': target_relation, 'temp_relation': temp_relation, 'unique_key': unique_key, 'dest_columns': dest_columns, 'incremental_predicates': incremental_predicates }) %}
     {%- call statement('main') -%}
       {{ strategy_sql_macro_func(strategy_arg_dict) }}
     {%- endcall -%}
   {% endif %}
 
-  {% do drop_relation_if_exists(temp_relation) %}
+  {% do adapter.drop_relation(tmp_relation_view) %}
+  {% do adapter.drop_relation(temp_relation) %}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
-
   {% set target_relation = target_relation.incorporate(type='table') %}
-
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
-
   {% do persist_docs(target_relation, model) %}
   {% do adapter.commit() %}
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/clone.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/clone.sql`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     {%- set other_existing_relation = load_cached_relation(defer_relation) -%}
     {% set can_clone_table = can_clone_table() %}
 
     {%- if other_existing_relation and other_existing_relation.type == 'table' and can_clone_table -%}
         {%- set target_relation = this.incorporate(type='table') -%}
 
         {% call statement('main') %}
-            {{ fabric__drop_relation_script(target_relation) }}
+            {% do adapter.drop_relation(target_relation) %}
             {{ create_or_replace_clone(target_relation, defer_relation) }}
         {% endcall %}
         {{ return({'relations': [target_relation]}) }}
     {%- else -%}
 
         {%- set target_relation = this.incorporate(type='view') -%}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+{% macro build_columns_constraints(relation) %}
+    {{ return(adapter.dispatch('build_columns_constraints', 'dbt')(relation)) }}
+{% endmacro %}
+
 {% macro fabric__build_columns_constraints(relation) %}
   {# loop through user_provided_columns to create DDL with data types and constraints #}
     {%- set raw_column_constraints = adapter.render_raw_columns_constraints(raw_columns=model['columns']) -%}
     (
       {% for c in raw_column_constraints -%}
         {{ c }}{{ "," if not loop.last }}
       {% endfor %}
     )
 {% endmacro %}
 
+{% macro build_model_constraints(relation) %}
+    {{ return(adapter.dispatch('build_model_constraints', 'dbt')(relation)) }}
+{% endmacro %}
+
 {% macro fabric__build_model_constraints(relation) %}
   {# loop through user_provided_columns to create DDL with data types and constraints #}
     {%- set raw_model_constraints = adapter.render_raw_model_constraints(raw_constraints=model['constraints']) -%}
     {% for c in raw_model_constraints -%}
       {% set alter_table_script %}
         alter table {{ relation.include(database=False) }} {{c}};
       {%endset%}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 {% macro fabric__create_table_as(temporary, relation, sql) -%}
 
-   {% set tmp_relation = relation.incorporate(
-   path={"identifier": relation.identifier.replace("#", "") ~ '_temp_view'},
-   type='view')-%}
-   {% do run_query(fabric__drop_relation_script(tmp_relation)) %}
+    {% set tmp_relation = relation.incorporate(path={"identifier": relation.identifier ~ '__dbt_tmp_vw'}, type='view')-%}
+    {{ get_create_view_as_sql(tmp_relation, sql) }}
 
-   {% set contract_config = config.get('contract') %}
-
-    {{ fabric__create_view_as(tmp_relation, sql) }}
+    {% set contract_config = config.get('contract') %}
     {% if contract_config.enforced %}
 
         CREATE TABLE [{{relation.database}}].[{{relation.schema}}].[{{relation.identifier}}]
-        {{ fabric__build_columns_constraints(relation) }}
+        {{ build_columns_constraints(relation) }}
         {{ get_assert_columns_equivalent(sql)  }}
-
         {% set listColumns %}
             {% for column in model['columns'] %}
                 {{ "["~column~"]" }}{{ ", " if not loop.last }}
             {% endfor %}
         {%endset%}
 
         INSERT INTO [{{relation.database}}].[{{relation.schema}}].[{{relation.identifier}}]
         ({{listColumns}}) SELECT {{listColumns}} FROM [{{tmp_relation.database}}].[{{tmp_relation.schema}}].[{{tmp_relation.identifier}}];
 
     {%- else %}
-      EXEC('CREATE TABLE [{{relation.database}}].[{{relation.schema}}].[{{relation.identifier}}] AS (SELECT * FROM [{{tmp_relation.database}}].[{{tmp_relation.schema}}].[{{tmp_relation.identifier}}]);');
+        EXEC('CREATE TABLE [{{relation.database}}].[{{relation.schema}}].[{{relation.identifier}}] AS (SELECT * FROM [{{tmp_relation.database}}].[{{tmp_relation.schema}}].[{{tmp_relation.identifier}}]);');
     {% endif %}
-
-    {{ fabric__drop_relation_script(tmp_relation) }}
-
+    {% do adapter.drop_relation(tmp_relation)%}
 {% endmacro %}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/table/table.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/table/table.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 {% materialization table, adapter='fabric' %}
 
   -- Load target relation
   {%- set target_relation = this.incorporate(type='table') %}
-  -- Load existing relation
-  {%- set relation = fabric__get_relation_without_caching(this) %}
-
-  {% set existing_relation = none %}
-  {% if (relation|length == 1) %}
-    {% set existing_relation = get_or_create_relation(relation[0][0], relation[0][2] , relation[0][1] , relation[0][3])[1] %}
-  {% endif %}
+  {%- set existing_relation = adapter.get_relation(database=this.database, schema=this.schema, identifier=this.identifier) -%}
 
   {%- set backup_relation = none %}
-  {{log("Existing Relation type is "~ existing_relation.type)}}
   {% if (existing_relation != none and existing_relation.type == "table") %}
       {%- set backup_relation = make_backup_relation(target_relation, 'table') -%}
   {% elif (existing_relation != none and existing_relation.type == "view") %}
       {%- set backup_relation = make_backup_relation(target_relation, 'view') -%}
   {% endif %}
 
   {% if (existing_relation != none) %}
     -- drop the temp relations if they exist already in the database
-    {{ drop_relation_if_exists(backup_relation) }}
+    {% do adapter.drop_relation(backup_relation) %}
     -- Rename target relation as backup relation
     {{ adapter.rename_relation(existing_relation, backup_relation) }}
   {% endif %}
 
   -- grab current tables grants config for comparision later on
   {% set grant_config = config.get('grants') %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
+  -- naming a temp relation
+  {% set tmp_relation = target_relation.incorporate(path={"identifier": target_relation.identifier ~ '__dbt_tmp_vw'}, type='view')-%}
+
+  -- Fabric & Synapse adapters use temp relation because of lack of CTE support for CTE in CTAS, Insert
+  -- drop temp relation if exists
+  {% do adapter.drop_relation(tmp_relation) %}
+
   -- build model
   {% call statement('main') -%}
     {{ get_create_table_as_sql(False, target_relation, sql) }}
   {%- endcall %}
 
+  -- drop temp relation if exists
+  {% do adapter.drop_relation(tmp_relation) %}
+
   -- cleanup
   {{ run_hooks(post_hooks, inside_transaction=True) }}
+
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
   {% do persist_docs(target_relation, model) %}
   -- `COMMIT` happens here
   {{ adapter.commit() }}
 
   {% if (backup_relation != none) %}
     -- finally, drop the foreign key references if exists
     {{ drop_fk_indexes_on_table(backup_relation) }}
     -- drop existing/backup relation after the commit
-    {{ drop_relation_if_exists(backup_relation) }}
+    {% do adapter.drop_relation(backup_relation) %}
    {% endif %}
+
   -- Add constraints including FK relation.
-  {{ fabric__build_model_constraints(target_relation) }}
+  {{ build_model_constraints(target_relation) }}
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     {{ fabric__create_view_exec(relation, sql) }}
 {% endmacro %}
 
 {% macro fabric__create_view_exec(relation, sql) -%}
 
     {%- set temp_view_sql = sql.replace("'", "''") -%}
 
-    USE [{{ relation.database }}];
+    {{ get_use_database_sql(relation.database) }}
     {% set contract_config = config.get('contract') %}
     {% if contract_config.enforced %}
         {{ get_assert_columns_equivalent(sql) }}
     {%- endif %}
 
     EXEC('create view {{ relation.include(database=False) }} as {{ temp_view_sql }};');
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/models/view/view.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/models/view/view.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 {% materialization view, adapter='fabric' -%}
 
   {%- set target_relation = this.incorporate(type='view') -%}
-  {{log("Target Relation "~target_relation)}}
-
-  {%- set relation = fabric__get_relation_without_caching(this) %}
-  {% set existing_relation = none %}
-  {% if (relation|length == 1) %}
-    {% set existing_relation = get_or_create_relation(relation[0][0], relation[0][2] , relation[0][1] , relation[0][3])[1] %}
-  {% endif %}
-  {{log("Existing Relation "~existing_relation)}}
+  {%- set existing_relation = adapter.get_relation(database=this.database, schema=this.schema, identifier=this.identifier) -%}
 
   {%- set backup_relation = none %}
-  {{log("Existing Relation type is "~ existing_relation.type)}}
   {% if (existing_relation != none and existing_relation.type == "table") %}
       {%- set backup_relation = make_backup_relation(target_relation, 'table') -%}
   {% elif (existing_relation != none and existing_relation.type == "view") %}
       {%- set backup_relation = make_backup_relation(target_relation, 'view') -%}
   {% endif %}
 
   {% if (existing_relation != none) %}
     -- drop the temp relations if they exist already in the database
-    {{ drop_relation_if_exists(backup_relation) }}
+    {% do adapter.drop_relation(backup_relation) %}
     -- Rename target relation as backup relation
     {{ adapter.rename_relation(existing_relation, backup_relation) }}
   {% endif %}
 
   {% set grant_config = config.get('grants') %}
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
@@ -39,13 +31,13 @@
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
   {{ adapter.commit() }}
   {% if (backup_relation != none) %}
-    {{ drop_relation_if_exists(backup_relation) }}
+    {% do adapter.drop_relation(backup_relation) %}
   {% endif %}
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization -%}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/helpers.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/helpers.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% macro fabric__post_snapshot(staging_relation) %}
   -- Clean up the snapshot temp table
-  {% do drop_relation(staging_relation) %}
+  {% do drop_relation_if_exists(staging_relation) %}
 {% endmacro %}
 
 --Due to Alter not being supported, have to rely on this for temporarily
 {% macro fabric__create_columns(relation, columns) %}
   {# default__ macro uses "add column"
      TSQL preferes just "add"
   #}
@@ -186,14 +186,14 @@
     select * from deletes
     {%- endif %}
 
 {%- endmacro %}
 
 {% macro build_snapshot_staging_table(strategy, temp_snapshot_relation, target_relation) %}
     {% set temp_relation = make_temp_relation(target_relation) %}
-    {% set select = fabric__snapshot_staging_table(strategy, temp_snapshot_relation, target_relation) %}
+    {% set select = snapshot_staging_table(strategy, temp_snapshot_relation, target_relation) %}
     {% call statement('build_snapshot_staging_relation') %}
-        {{ create_table_as(True, temp_relation, select) }}
+        {{ get_create_table_as_sql(True, temp_relation, select) }}
     {% endcall %}
 
     {% do return(temp_relation) %}
 {% endmacro %}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,22 @@
     EXEC('DROP VIEW IF EXISTS {{ temp_snapshot_relation.include(database=False) }};');
     EXEC('create view {{ temp_snapshot_relation.include(database=False) }} as {{ temp_snapshot_relation_sql }};');
   {% endcall %}
 
   {% if not target_relation_exists %}
 
       {% set build_sql = build_snapshot_table(strategy, temp_snapshot_relation) %}
-      {% set final_sql = create_table_as(False, target_relation, build_sql) %}
+
+      -- naming a temp relation
+      {% set tmp_relation_view = target_relation.incorporate(path={"identifier": target_relation.identifier ~ '__dbt_tmp_vw'}, type='view')-%}
+      -- Fabric & Synapse adapters use temp relation because of lack of CTE support for CTE in CTAS, Insert
+      -- drop temp relation if exists
+      {% do adapter.drop_relation(tmp_relation_view) %}
+      {% set final_sql = get_create_table_as_sql(False, target_relation, build_sql) %}
+      {% do adapter.drop_relation(tmp_relation_view) %}
 
   {% else %}
 
       {{ adapter.valid_snapshot_target(target_relation) }}
       {% set staging_table = build_snapshot_staging_table(strategy, temp_snapshot_relation, target_relation) %}
       -- this may no-op if the database does not require column expansion
       {% do adapter.expand_target_column_types(from_relation=staging_table,
@@ -71,38 +78,34 @@
 
       {% set final_sql = snapshot_merge_sql(
             target = target_relation,
             source = staging_table,
             insert_cols = quoted_source_columns
          )
       %}
-
   {% endif %}
 
   {% call statement('main') %}
       {{ final_sql }}
   {% endcall %}
 
-  fabric__drop_relation_script(temp_snapshot_relation)
-
+  {% do adapter.drop_relation(temp_snapshot_relation) %}
   {% set should_revoke = should_revoke(target_relation_exists, full_refresh_mode=False) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
 
   {% if not target_relation_exists %}
     {% do create_indexes(target_relation) %}
   {% endif %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
-
   {{ adapter.commit() }}
 
   {% if staging_table is defined %}
       {% do post_snapshot(staging_table) %}
   {% endif %}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
-
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
```

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/dbt/include/fabric/macros/materializations/tests/helpers.sql` & `dbt-fabric-1.8.6/dbt/include/fabric/macros/materializations/tests/helpers.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 {% macro fabric__get_test_sql(main_sql, fail_calc, warn_if, error_if, limit) -%}
 
+  -- Create target schema if it does not
+  USE [{{ target.database }}];
+  IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = '{{ target.schema }}')
+  BEGIN
+    EXEC('CREATE SCHEMA [{{ target.schema }}]')
+  END
+
   {% if main_sql.strip().lower().startswith('with') %}
     {% set testview %}
-      {{ config.get('schema') }}.testview_{{ range(1300, 19000) | random }}
+      {{ target.schema }}.testview_{{ range(1300, 19000) | random }}
     {% endset %}
 
     {% set sql = main_sql.replace("'", "''")%}
-
     EXEC('create view {{testview}} as {{ sql }};')
     select
       {{ "top (" ~ limit ~ ')' if limit != none }}
       {{ fail_calc }} as failures,
       case when {{ fail_calc }} {{ warn_if }}
         then 'true' else 'false' end as should_warn,
       case when {{ fail_calc }} {{ error_if }}
```

### Comparing `dbt-fabric-1.8.5/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.8.6/dbt_fabric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.5
+Version: 1.8.6
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.5/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.8.6/dbt_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.5/setup.py` & `dbt-fabric-1.8.6/setup.py`

 * *Files identical despite different names*

