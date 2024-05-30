# Comparing `tmp/dbt_duckdb-1.8.0.tar.gz` & `tmp/dbt_duckdb-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_duckdb-1.8.0.tar", last modified: Fri May 10 04:54:01 2024, max compression
+gzip compressed data, was "dbt_duckdb-1.8.1.tar", last modified: Thu May 30 17:45:16 2024, max compression
```

## Comparing `dbt_duckdb-1.8.0.tar` & `dbt_duckdb-1.8.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.938098 dbt_duckdb-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-05-10 04:54:01.938098 dbt_duckdb-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.926098 dbt_duckdb-1.8.0/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.926098 dbt_duckdb-1.8.0/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/adapters/duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/buenavista.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/motherduck.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/pd_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/include/duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/incremental_helper.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/snapshot_helper.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/upstream.sql
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:54:01.938098 dbt_duckdb-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.693908 dbt_duckdb-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23798 2024-05-30 17:45:16.693908 dbt_duckdb-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.685908 dbt_duckdb-1.8.1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.685908 dbt_duckdb-1.8.1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.685908 dbt_duckdb-1.8.1/dbt/adapters/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.685908 dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.689908 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/motherduck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/pd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.689908 dbt_duckdb-1.8.1/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.689908 dbt_duckdb-1.8.1/dbt/include/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.689908 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/incremental_helper.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.689908 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/snapshot_helper.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.693908 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/upstream.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/dbt/include/duckdb/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:45:16.693908 dbt_duckdb-1.8.1/dbt_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23798 2024-05-30 17:45:16.000000 dbt_duckdb-1.8.1/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 17:45:16.000000 dbt_duckdb-1.8.1/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:45:16.000000 dbt_duckdb-1.8.1/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 17:45:16.000000 dbt_duckdb-1.8.1/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 17:45:16.000000 dbt_duckdb-1.8.1/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:45:16.693908 dbt_duckdb-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-30 17:45:13.000000 dbt_duckdb-1.8.1/setup.py
```

### Comparing `dbt_duckdb-1.8.0/LICENSE` & `dbt_duckdb-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/PKG-INFO` & `dbt_duckdb-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.8.0
+Version: 1.8.1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dbt-common<2,>=1
 Requires-Dist: dbt-adapters<2,>=1
-Requires-Dist: duckdb>=0.7.0
+Requires-Dist: duckdb!=0.10.3,>=0.7.0
 Requires-Dist: dbt-core>=1.8.0
 Provides-Extra: glue
 Requires-Dist: boto3; extra == "glue"
 Requires-Dist: mypy-boto3-glue; extra == "glue"
 Provides-Extra: md
-Requires-Dist: duckdb>=0.10.2; extra == "md"
+Requires-Dist: duckdb==0.10.2; extra == "md"
 
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
 It is crazy fast and allows you to read and write data stored in CSV, JSON, and Parquet files directly, without requiring you to load
 them into the database first.
```

### Comparing `dbt_duckdb-1.8.0/README.md` & `dbt_duckdb-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/column.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/column.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/connections.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/credentials.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/__init__.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/buenavista.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/local.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/environments/local.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/impl.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/__init__.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/delta.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/delta.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/excel.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/excel.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/glue.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/glue.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/motherduck.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/motherduck.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/pd_utils.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/postgres.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/relation.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/adapters/duckdb/utils.py` & `dbt_duckdb-1.8.1/dbt/adapters/duckdb/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/adapters.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/catalog.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/columns.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/incremental_helper.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/incremental_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/external.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/table.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/persist_docs.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/seed.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/snapshot_helper.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/snapshot_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt_duckdb-1.8.1/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/dbt_duckdb.egg-info/PKG-INFO` & `dbt_duckdb-1.8.1/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.8.0
+Version: 1.8.1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dbt-common<2,>=1
 Requires-Dist: dbt-adapters<2,>=1
-Requires-Dist: duckdb>=0.7.0
+Requires-Dist: duckdb!=0.10.3,>=0.7.0
 Requires-Dist: dbt-core>=1.8.0
 Provides-Extra: glue
 Requires-Dist: boto3; extra == "glue"
 Requires-Dist: mypy-boto3-glue; extra == "glue"
 Provides-Extra: md
-Requires-Dist: duckdb>=0.10.2; extra == "md"
+Requires-Dist: duckdb==0.10.2; extra == "md"
 
 ## dbt-duckdb
 
 [DuckDB](http://duckdb.org) is an embedded database, similar to SQLite, but designed for OLAP-style analytics.
 It is crazy fast and allows you to read and write data stored in CSV, JSON, and Parquet files directly, without requiring you to load
 them into the database first.
```

### Comparing `dbt_duckdb-1.8.0/dbt_duckdb.egg-info/SOURCES.txt` & `dbt_duckdb-1.8.1/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.8.0/setup.py` & `dbt_duckdb-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     author_email="joshwills+dbt@gmail.com",
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-common>=1,<2",
         "dbt-adapters>=1,<2",
-        "duckdb>=0.7.0",
+        "duckdb>=0.7.0,!=0.10.3",
         # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
         "dbt-core>=1.8.0",
     ],
-    extras_require={"glue": ["boto3", "mypy-boto3-glue"], "md": ["duckdb>=0.10.2"]},
+    extras_require={"glue": ["boto3", "mypy-boto3-glue"], "md": ["duckdb==0.10.2"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.8",
```

