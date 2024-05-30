# Comparing `tmp/cratedb-toolkit-0.0.7.tar.gz` & `tmp/cratedb-toolkit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cratedb-toolkit-0.0.7.tar", last modified: Thu Mar  7 22:23:26 2024, max compression
+gzip compressed data, was "cratedb-toolkit-0.0.8.tar", last modified: Mon Mar 11 13:07:09 2024, max compression
```

## Comparing `cratedb-toolkit-0.0.7.tar` & `cratedb-toolkit-0.0.8.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.651951 cratedb-toolkit-0.0.7/
--rw-r--r--   0 amo        (501) staff       (20)     2727 2024-03-07 18:11:43.000000 cratedb-toolkit-0.0.7/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)    32387 2023-06-26 23:58:53.000000 cratedb-toolkit-0.0.7/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      126 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     8391 2024-03-07 22:23:26.651565 cratedb-toolkit-0.0.7/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3016 2023-11-02 11:18:34.000000 cratedb-toolkit-0.0.7/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.617885 cratedb-toolkit-0.0.7/cratedb_toolkit/
--rw-r--r--   0 amo        (501) staff       (20)      402 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.620204 cratedb-toolkit-0.0.7/cratedb_toolkit/api/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/api/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1521 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/api/guide.py
--rw-r--r--   0 amo        (501) staff       (20)     4679 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/api/main.py
--rw-r--r--   0 amo        (501) staff       (20)      797 2024-01-18 18:59:49.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/cli.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.621404 cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-17 17:15:29.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1442 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/cli.py
--rw-r--r--   0 amo        (501) staff       (20)      935 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/croud.py
--rw-r--r--   0 amo        (501) staff       (20)      382 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.624354 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/
--rw-r--r--   0 amo        (501) staff       (20)       45 2024-03-07 00:41:53.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      237 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/core.py
--rw-r--r--   0 amo        (501) staff       (20)     1594 2024-03-07 15:58:40.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/kaggle.py
--rw-r--r--   0 amo        (501) staff       (20)     4047 2024-03-07 18:10:56.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/model.py
--rw-r--r--   0 amo        (501) staff       (20)       89 2024-03-07 00:41:53.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/store.py
--rw-r--r--   0 amo        (501) staff       (20)     1749 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/tutorial.py
--rw-r--r--   0 amo        (501) staff       (20)      854 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/util.py
--rw-r--r--   0 amo        (501) staff       (20)      130 2023-11-13 21:02:34.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/exception.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.625841 cratedb-toolkit-0.0.7/cratedb_toolkit/io/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-08 11:26:53.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     3327 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     7110 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/croud.py
--rw-r--r--   0 amo        (501) staff       (20)      458 2023-11-13 08:54:25.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/influxdb.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.629692 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-13 08:16:35.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     2803 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/api.py
--rw-r--r--   0 amo        (501) staff       (20)     3051 2023-11-13 08:54:25.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     3905 2023-11-15 12:10:47.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/core.py
--rw-r--r--   0 amo        (501) staff       (20)     3473 2023-11-13 08:54:25.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/export.py
--rw-r--r--   0 amo        (501) staff       (20)     5862 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/extract.py
--rw-r--r--   0 amo        (501) staff       (20)     5392 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/translate.py
--rw-r--r--   0 amo        (501) staff       (20)      611 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/util.py
--rw-r--r--   0 amo        (501) staff       (20)       81 2023-11-09 19:44:41.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/io/sql.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.630839 cratedb-toolkit-0.0.7/cratedb_toolkit/job/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-13 08:11:25.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/job/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      851 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/job/cli.py
--rw-r--r--   0 amo        (501) staff       (20)      631 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/job/croud.py
--rw-r--r--   0 amo        (501) staff       (20)     3079 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/model.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.633338 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     9419 2023-11-13 04:56:19.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     8555 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/core.py
--rw-r--r--   0 amo        (501) staff       (20)     5839 2023-11-13 04:56:14.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/model.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.634527 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/setup/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/setup/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      968 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/setup/schema.py
--rw-r--r--   0 amo        (501) staff       (20)     1569 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/setup/schema.sql
--rw-r--r--   0 amo        (501) staff       (20)     8437 2023-12-04 03:25:49.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/store.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.635912 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1106 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/delete.py
--rw-r--r--   0 amo        (501) staff       (20)     1985 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/reallocate.py
--rw-r--r--   0 amo        (501) staff       (20)     1460 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/snapshot.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.636438 cratedb-toolkit-0.0.7/cratedb_toolkit/shell/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-13 08:11:25.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/shell/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     2039 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/shell/cli.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.637764 cratedb-toolkit-0.0.7/cratedb_toolkit/sqlalchemy/
--rw-r--r--   0 amo        (501) staff       (20)      149 2023-12-31 22:15:28.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/sqlalchemy/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1141 2023-12-31 22:15:28.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/sqlalchemy/patch.py
--rw-r--r--   0 amo        (501) staff       (20)     4302 2023-11-09 19:44:41.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/sqlalchemy/polyfill.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.638367 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      760 2024-02-12 12:59:27.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/pytest.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.640924 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     3016 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/azurite.py
--rw-r--r--   0 amo        (501) staff       (20)     8224 2024-02-09 22:24:41.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/cratedb.py
--rw-r--r--   0 amo        (501) staff       (20)     2960 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/influxdb2.py
--rw-r--r--   0 amo        (501) staff       (20)     1672 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/minio.py
--rw-r--r--   0 amo        (501) staff       (20)     1534 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/mongodb.py
--rw-r--r--   0 amo        (501) staff       (20)     4758 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.644235 cratedb-toolkit-0.0.7/cratedb_toolkit/util/
--rw-r--r--   0 amo        (501) staff       (20)      194 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     2978 2024-01-18 18:59:49.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     1026 2023-12-04 03:25:49.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/common.py
--rw-r--r--   0 amo        (501) staff       (20)      273 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/cr8.py
--rw-r--r--   0 amo        (501) staff       (20)      918 2023-11-13 08:18:56.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/crash.py
--rw-r--r--   0 amo        (501) staff       (20)     5834 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/croud.py
--rw-r--r--   0 amo        (501) staff       (20)      391 2024-01-18 18:59:49.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/data.py
--rw-r--r--   0 amo        (501) staff       (20)     9479 2024-03-07 00:41:53.000000 cratedb-toolkit-0.0.7/cratedb_toolkit/util/database.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.647957 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     8391 2024-03-07 22:23:23.000000 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     2783 2024-03-07 22:23:26.000000 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-03-07 22:23:23.000000 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)      249 2024-03-07 22:23:23.000000 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      835 2024-03-07 22:23:23.000000 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       22 2024-03-07 22:23:23.000000 cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-07 22:23:26.647248 cratedb-toolkit-0.0.7/doc/
--rw-r--r--   0 amo        (501) staff       (20)     9430 2024-02-12 13:02:22.000000 cratedb-toolkit-0.0.7/doc/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)     4455 2023-11-13 08:18:56.000000 cratedb-toolkit-0.0.7/doc/bugs.md
--rw-r--r--   0 amo        (501) staff       (20)     2800 2023-11-15 05:14:14.000000 cratedb-toolkit-0.0.7/doc/notes.md
--rw-r--r--   0 amo        (501) staff       (20)    16804 2023-11-13 04:56:10.000000 cratedb-toolkit-0.0.7/doc/retention.md
--rw-r--r--   0 amo        (501) staff       (20)     1122 2024-02-09 21:10:27.000000 cratedb-toolkit-0.0.7/doc/sandbox.md
--rw-r--r--   0 amo        (501) staff       (20)     7095 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.7/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-03-07 22:23:26.652022 cratedb-toolkit-0.0.7/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:09.009547 cratedb-toolkit-0.0.8/
+-rw-r--r--   0 amo        (501) staff       (20)     2794 2024-03-11 13:06:36.000000 cratedb-toolkit-0.0.8/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)    32387 2023-06-26 23:58:53.000000 cratedb-toolkit-0.0.8/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      126 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     8451 2024-03-11 13:07:09.009082 cratedb-toolkit-0.0.8/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3016 2023-11-02 11:18:34.000000 cratedb-toolkit-0.0.8/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.972764 cratedb-toolkit-0.0.8/cratedb_toolkit/
+-rw-r--r--   0 amo        (501) staff       (20)      402 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.976216 cratedb-toolkit-0.0.8/cratedb_toolkit/api/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/api/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1521 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/api/guide.py
+-rw-r--r--   0 amo        (501) staff       (20)     4679 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/api/main.py
+-rw-r--r--   0 amo        (501) staff       (20)      797 2024-01-18 18:59:49.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/cli.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.977439 cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-17 17:15:29.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1442 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)      935 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/croud.py
+-rw-r--r--   0 amo        (501) staff       (20)      382 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.980571 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/
+-rw-r--r--   0 amo        (501) staff       (20)       45 2024-03-07 00:41:53.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      237 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     1594 2024-03-07 15:58:40.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/kaggle.py
+-rw-r--r--   0 amo        (501) staff       (20)     4170 2024-03-11 13:06:15.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/model.py
+-rw-r--r--   0 amo        (501) staff       (20)       89 2024-03-07 00:41:53.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/store.py
+-rw-r--r--   0 amo        (501) staff       (20)     1749 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/tutorial.py
+-rw-r--r--   0 amo        (501) staff       (20)      854 2024-03-07 15:41:37.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/util.py
+-rw-r--r--   0 amo        (501) staff       (20)      130 2023-11-13 21:02:34.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/exception.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.982300 cratedb-toolkit-0.0.8/cratedb_toolkit/io/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-08 11:26:53.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     3327 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     7110 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/croud.py
+-rw-r--r--   0 amo        (501) staff       (20)      458 2023-11-13 08:54:25.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/influxdb.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.985941 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-13 08:16:35.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     2803 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/api.py
+-rw-r--r--   0 amo        (501) staff       (20)     3051 2023-11-13 08:54:25.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     3905 2023-11-15 12:10:47.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     3473 2023-11-13 08:54:25.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/export.py
+-rw-r--r--   0 amo        (501) staff       (20)     5862 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/extract.py
+-rw-r--r--   0 amo        (501) staff       (20)     5392 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/translate.py
+-rw-r--r--   0 amo        (501) staff       (20)      611 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/util.py
+-rw-r--r--   0 amo        (501) staff       (20)       81 2023-11-09 19:44:41.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/io/sql.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.986992 cratedb-toolkit-0.0.8/cratedb_toolkit/job/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-13 08:11:25.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/job/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      851 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/job/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)      631 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/job/croud.py
+-rw-r--r--   0 amo        (501) staff       (20)     3079 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/model.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.989549 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     9419 2023-11-13 04:56:19.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     8555 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     5839 2023-11-13 04:56:14.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/model.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.990793 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/setup/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/setup/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      968 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/setup/schema.py
+-rw-r--r--   0 amo        (501) staff       (20)     1569 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/setup/schema.sql
+-rw-r--r--   0 amo        (501) staff       (20)     8437 2023-12-04 03:25:49.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/store.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.992273 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1106 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/delete.py
+-rw-r--r--   0 amo        (501) staff       (20)     1985 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/reallocate.py
+-rw-r--r--   0 amo        (501) staff       (20)     1460 2023-11-02 01:51:31.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/snapshot.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.992779 cratedb-toolkit-0.0.8/cratedb_toolkit/shell/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-11-13 08:11:25.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/shell/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     2039 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/shell/cli.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.994202 cratedb-toolkit-0.0.8/cratedb_toolkit/sqlalchemy/
+-rw-r--r--   0 amo        (501) staff       (20)      149 2023-12-31 22:15:28.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/sqlalchemy/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1141 2023-12-31 22:15:28.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/sqlalchemy/patch.py
+-rw-r--r--   0 amo        (501) staff       (20)     4302 2023-11-09 19:44:41.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/sqlalchemy/polyfill.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.994834 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      760 2024-02-12 12:59:27.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/pytest.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:08.997861 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     3016 2023-10-10 20:52:48.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/azurite.py
+-rw-r--r--   0 amo        (501) staff       (20)     8224 2024-02-09 22:24:41.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/cratedb.py
+-rw-r--r--   0 amo        (501) staff       (20)     2960 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/influxdb2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1672 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/minio.py
+-rw-r--r--   0 amo        (501) staff       (20)     1534 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/mongodb.py
+-rw-r--r--   0 amo        (501) staff       (20)     4758 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:09.001557 cratedb-toolkit-0.0.8/cratedb_toolkit/util/
+-rw-r--r--   0 amo        (501) staff       (20)      194 2023-11-22 01:41:59.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     2978 2024-01-18 18:59:49.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     1026 2023-12-04 03:25:49.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/common.py
+-rw-r--r--   0 amo        (501) staff       (20)      273 2023-11-13 08:54:26.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/cr8.py
+-rw-r--r--   0 amo        (501) staff       (20)      918 2023-11-13 08:18:56.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/crash.py
+-rw-r--r--   0 amo        (501) staff       (20)     5834 2024-02-06 13:52:32.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/croud.py
+-rw-r--r--   0 amo        (501) staff       (20)      391 2024-01-18 18:59:49.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/data.py
+-rw-r--r--   0 amo        (501) staff       (20)     9602 2024-03-11 13:06:15.000000 cratedb-toolkit-0.0.8/cratedb_toolkit/util/database.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:09.005096 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     8451 2024-03-11 13:07:05.000000 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     2783 2024-03-11 13:07:08.000000 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-03-11 13:07:05.000000 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)      249 2024-03-11 13:07:05.000000 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      855 2024-03-11 13:07:05.000000 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       22 2024-03-11 13:07:05.000000 cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-11 13:07:09.004615 cratedb-toolkit-0.0.8/doc/
+-rw-r--r--   0 amo        (501) staff       (20)     9430 2024-02-12 13:02:22.000000 cratedb-toolkit-0.0.8/doc/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)     4455 2023-11-13 08:18:56.000000 cratedb-toolkit-0.0.8/doc/bugs.md
+-rw-r--r--   0 amo        (501) staff       (20)     2800 2023-11-15 05:14:14.000000 cratedb-toolkit-0.0.8/doc/notes.md
+-rw-r--r--   0 amo        (501) staff       (20)    16804 2023-11-13 04:56:10.000000 cratedb-toolkit-0.0.8/doc/retention.md
+-rw-r--r--   0 amo        (501) staff       (20)     1122 2024-02-09 21:10:27.000000 cratedb-toolkit-0.0.8/doc/sandbox.md
+-rw-r--r--   0 amo        (501) staff       (20)     7145 2024-03-11 13:06:15.000000 cratedb-toolkit-0.0.8/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-03-11 13:07:09.009636 cratedb-toolkit-0.0.8/setup.cfg
```

### Comparing `cratedb-toolkit-0.0.7/CHANGES.md` & `cratedb-toolkit-0.0.8/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changes for cratedb-toolkit
 
 
 ## Unreleased
 
+## 2024/03/11 v0.0.8
+- datasets: Fix compatibility with Python 3.7
 
 ## 2024/03/07 v0.0.7
 - datasets: Fix dataset loader
 
 ## 2024/03/07 v0.0.6
 
 - Added `cratedb_toolkit.datasets` subsystem, for acquiring datasets
```

### Comparing `cratedb-toolkit-0.0.7/LICENSE` & `cratedb-toolkit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/PKG-INFO` & `cratedb-toolkit-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cratedb-toolkit
-Version: 0.0.7
+Version: 0.0.8
 Summary: CrateDB Toolkit
 Author-email: Niklas Schmidtmer <niklas@crate.io>, Marija Selakovic <marija@crate.io>, Andreas Motl <andreas.motl@crate.io>
 License: AGPL 3, EUPL 1.2
 Project-URL: changelog, https://github.com/crate-workbench/cratedb-toolkit/blob/main/CHANGES.rst
 Project-URL: documentation, https://github.com/crate-workbench/cratedb-toolkit
 Project-URL: homepage, https://github.com/crate-workbench/cratedb-toolkit
 Project-URL: repository, https://github.com/crate-workbench/cratedb-toolkit
@@ -72,14 +72,15 @@
 Requires-Dist: crash
 Requires-Dist: crate[sqlalchemy]>=0.34
 Requires-Dist: importlib-metadata; python_version <= "3.7"
 Requires-Dist: python-dotenv<2
 Requires-Dist: python-slugify<9
 Requires-Dist: sqlalchemy
 Requires-Dist: sqlparse<0.5
+Requires-Dist: typing-extensions<5; python_version <= "3.7"
 Provides-Extra: all
 Requires-Dist: cratedb-toolkit[cloud,datasets,influxdb,io,mongodb]; extra == "all"
 Provides-Extra: cloud
 Requires-Dist: croud==1.10.1; extra == "cloud"
 Provides-Extra: datasets
 Requires-Dist: datasets<3; extra == "datasets"
 Requires-Dist: kaggle<2; extra == "datasets"
```

### Comparing `cratedb-toolkit-0.0.7/README.md` & `cratedb-toolkit-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/api/guide.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/api/guide.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/api/main.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/api/main.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/cluster/croud.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/cluster/croud.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/kaggle.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/kaggle.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/model.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import typing as t
 
 import requests
 import sqlparse
 
 from cratedb_toolkit.util import DatabaseAdapter
 
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  # type: ignore[assignment]
+
 
 @dataclasses.dataclass
 class Dataset:
     """
     Wrapper around a dataset.
     """
 
@@ -64,15 +69,15 @@
 
     def __post_init__(self):
         self.init_sql = None
         self.db = DatabaseAdapter(dburi=self.dburi)
 
     def create(
         self,
-        if_exists: t.Literal["append", "noop", "replace"] = "noop",
+        if_exists: Literal["append", "noop", "replace"] = "noop",
         drop: bool = False,
     ):
         """
         Load dataset into CrateDB, or prepare loading, using SQL.
         """
 
         self.dataset.acquire()
@@ -91,15 +96,15 @@
                 self.db.prune_table(self.table, errors="ignore")
 
             if not self.dataset.init_includes_loading:
                 self.run_sql(self.init_sql)
 
     def load(
         self,
-        if_exists: t.Literal["append", "noop", "replace"] = "noop",
+        if_exists: Literal["append", "noop", "replace"] = "noop",
         drop: bool = False,
     ):
         self.create(if_exists=if_exists, drop=drop)
 
         cardinality = self.db.count_records(self.table, errors="ignore")
         has_data = cardinality > 0
```

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/tutorial.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/datasets/util.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/datasets/util.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/croud.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/croud.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/api.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/api.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/core.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/core.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/export.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/export.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/extract.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/extract.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/translate.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/translate.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/io/mongodb/util.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/io/mongodb/util.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/job/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/job/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/job/croud.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/job/croud.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/model.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/model.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/core.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/core.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/model.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/model.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/setup/schema.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/setup/schema.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/setup/schema.sql` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/setup/schema.sql`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/store.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/store.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/delete.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/delete.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/reallocate.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/reallocate.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/retention/strategy/snapshot.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/retention/strategy/snapshot.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/shell/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/shell/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/sqlalchemy/patch.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/sqlalchemy/patch.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/sqlalchemy/polyfill.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/sqlalchemy/polyfill.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/pytest.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/azurite.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/azurite.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/cratedb.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/cratedb.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/influxdb2.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/influxdb2.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/minio.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/minio.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/mongodb.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/mongodb.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/testing/testcontainers/util.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/testing/testcontainers/util.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/util/cli.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/util/cli.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/util/common.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/util/common.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/util/crash.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/util/crash.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/util/croud.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/util/croud.py`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit/util/database.py` & `cratedb-toolkit-0.0.8/cratedb_toolkit/util/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 import sqlparse
 from boltons.urlutils import URL
 from sqlalchemy.exc import ProgrammingError
 from sqlalchemy.sql.elements import AsBoolean
 
 from cratedb_toolkit.util.data import str_contains
 
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  # type: ignore[assignment]
+
 
 def run_sql(dburi: str, sql: str, records: bool = False):
     return DatabaseAdapter(dburi=dburi).run_sql(sql=sql, records=records)
 
 
 class DatabaseAdapter:
     """
@@ -70,15 +75,15 @@
 
         # Backward-compatibility.
         if len(results) == 1:
             return results[0]
         else:
             return results
 
-    def count_records(self, tablename_full: str, errors: t.Literal["raise", "ignore"] = "raise"):
+    def count_records(self, tablename_full: str, errors: Literal["raise", "ignore"] = "raise"):
         """
         Return number of records in table.
         """
         sql = f"SELECT COUNT(*) AS count FROM {tablename_full};"  # noqa: S608
         try:
             results = self.run_sql(sql=sql)
         except ProgrammingError as ex:
@@ -103,15 +108,15 @@
         """
         Run a `REFRESH TABLE ...` command.
         """
         sql = f"REFRESH TABLE {tablename_full};"  # noqa: S608
         self.run_sql(sql=sql)
         return True
 
-    def prune_table(self, tablename_full: str, errors: t.Literal["raise", "ignore"] = "raise"):
+    def prune_table(self, tablename_full: str, errors: Literal["raise", "ignore"] = "raise"):
         """
         Run a `DELETE FROM ...` command.
         """
         sql = f"DELETE FROM {tablename_full};"  # noqa: S608
         try:
             self.run_sql(sql=sql)
         except ProgrammingError as ex:
```

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/PKG-INFO` & `cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cratedb-toolkit
-Version: 0.0.7
+Version: 0.0.8
 Summary: CrateDB Toolkit
 Author-email: Niklas Schmidtmer <niklas@crate.io>, Marija Selakovic <marija@crate.io>, Andreas Motl <andreas.motl@crate.io>
 License: AGPL 3, EUPL 1.2
 Project-URL: changelog, https://github.com/crate-workbench/cratedb-toolkit/blob/main/CHANGES.rst
 Project-URL: documentation, https://github.com/crate-workbench/cratedb-toolkit
 Project-URL: homepage, https://github.com/crate-workbench/cratedb-toolkit
 Project-URL: repository, https://github.com/crate-workbench/cratedb-toolkit
@@ -72,14 +72,15 @@
 Requires-Dist: crash
 Requires-Dist: crate[sqlalchemy]>=0.34
 Requires-Dist: importlib-metadata; python_version <= "3.7"
 Requires-Dist: python-dotenv<2
 Requires-Dist: python-slugify<9
 Requires-Dist: sqlalchemy
 Requires-Dist: sqlparse<0.5
+Requires-Dist: typing-extensions<5; python_version <= "3.7"
 Provides-Extra: all
 Requires-Dist: cratedb-toolkit[cloud,datasets,influxdb,io,mongodb]; extra == "all"
 Provides-Extra: cloud
 Requires-Dist: croud==1.10.1; extra == "cloud"
 Provides-Extra: datasets
 Requires-Dist: datasets<3; extra == "datasets"
 Requires-Dist: kaggle<2; extra == "datasets"
```

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/SOURCES.txt` & `cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/cratedb_toolkit.egg-info/requires.txt` & `cratedb-toolkit-0.0.8/cratedb_toolkit.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 python-dotenv<2
 python-slugify<9
 sqlalchemy
 sqlparse<0.5
 
 [:python_version <= "3.7"]
 importlib-metadata
+typing-extensions<5
 
 [all]
 cratedb-toolkit[cloud,datasets,influxdb,io,mongodb]
 
 [cloud]
 croud==1.10.1
```

### Comparing `cratedb-toolkit-0.0.7/doc/backlog.md` & `cratedb-toolkit-0.0.8/doc/backlog.md`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/doc/bugs.md` & `cratedb-toolkit-0.0.8/doc/bugs.md`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/doc/notes.md` & `cratedb-toolkit-0.0.8/doc/notes.md`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/doc/retention.md` & `cratedb-toolkit-0.0.8/doc/retention.md`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/doc/sandbox.md` & `cratedb-toolkit-0.0.8/doc/sandbox.md`

 * *Files identical despite different names*

### Comparing `cratedb-toolkit-0.0.7/pyproject.toml` & `cratedb-toolkit-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
   "crash",
   "crate[sqlalchemy]>=0.34",
   'importlib-metadata; python_version <= "3.7"',
   "python-dotenv<2",
   "python-slugify<9",
   "sqlalchemy",
   "sqlparse<0.5",
+  'typing-extensions<5; python_version <= "3.7"',
 ]
 [project.optional-dependencies]
 all = [
   "cratedb-toolkit[cloud,datasets,influxdb,io,mongodb]",
 ]
 cloud = [
   "croud==1.10.1",
```

