# Comparing `tmp/vdk-trino-0.4.944393829.tar.gz` & `tmp/vdk-trino-0.4.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-trino-0.4.944393829.tar", last modified: Tue Jul 25 09:01:03 2023, max compression
+gzip compressed data, was "vdk-trino-0.4.948436673.tar", last modified: Fri Jul 28 09:43:57 2023, max compression
```

## Comparing `vdk-trino-0.4.944393829.tar` & `vdk-trino-0.4.948436673.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.401383 vdk-trino-0.4.944393829/
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3242 2023-07-25 09:01:03.401383 vdk-trino-0.4.944393829/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2615 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:01:03.401383 vdk-trino-0.4.944393829/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-07-25 09:00:50.000000 vdk-trino-0.4.944393829/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.397384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/
--rw-rw-rw-   0 root         (0) root         (0)     7384 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/ingest_to_trino.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/lineage_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.397384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/00-verify-valid-target.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/02-drop-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/03-drop-backup-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/04-create-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/05-insert-into-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/06-move-data-from-tmp-to-target.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.397384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/00-verify-valid-target.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/01-add-props-for-args.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/02-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/03-drop-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/04-drop-backup-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/05-create-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3940 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/06-insert-into-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/07-move-data-from-tmp-to-target.py.py
--rw-rw-rw-   0 root         (0) root         (0)     3350 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.393384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.397384 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/00-verify-valid-target.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/02-drop-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/03-drop-backup-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/04-create-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/05-insert-into-tmp-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2159 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/06-move-data-from-tmp-to-target.py
--rw-rw-rw-   0 root         (0) root         (0)     2164 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_config.py
--rw-rw-rw-   0 root         (0) root         (0)     5127 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     6046 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    10112 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.397384 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3242 2023-07-25 09:01:03.000000 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2662 2023-07-25 09:01:03.000000 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:01:03.000000 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 09:01:03.000000 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-25 09:01:03.000000 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:01:03.000000 vdk-trino-0.4.944393829/src/vdk_trino.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:03.401383 vdk-trino-0.4.944393829/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3055 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/tests/test_ingest_to_trino.py
--rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/tests/test_trino_sql.py
--rw-rw-rw-   0 root         (0) root         (0)    21703 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/tests/test_vdk_templates.py
--rw-rw-rw-   0 root         (0) root         (0)    12904 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/tests/test_vdk_trino_lineage.py
--rw-rw-rw-   0 root         (0) root         (0)     7086 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/tests/test_vdk_trino_lineage_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-07-25 09:00:45.000000 vdk-trino-0.4.944393829/tests/test_vdk_trino_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.253954 vdk-trino-0.4.948436673/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-07-28 09:43:57.253954 vdk-trino-0.4.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2615 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:57.253954 vdk-trino-0.4.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-07-28 09:43:42.000000 vdk-trino-0.4.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.249954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/
+-rw-rw-rw-   0 root         (0) root         (0)     7384 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/ingest_to_trino.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/lineage_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.249954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/00-verify-valid-target.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/02-drop-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/03-drop-backup-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/04-create-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/05-insert-into-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/06-move-data-from-tmp-to-target.py
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.249954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/00-verify-valid-target.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/01-add-props-for-args.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/02-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/03-drop-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/04-drop-backup-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/05-create-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/06-insert-into-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/07-move-data-from-tmp-to-target.py.py
+-rw-rw-rw-   0 root         (0) root         (0)     3350 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.245954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.253954 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/00-verify-valid-target.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/02-drop-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/03-drop-backup-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/04-create-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/05-insert-into-tmp-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/06-move-data-from-tmp-to-target.py
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3444 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5127 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6046 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    10112 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.253954 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-07-28 09:43:57.000000 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-28 09:43:57.000000 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:57.000000 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-28 09:43:57.000000 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-28 09:43:57.000000 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:57.000000 vdk-trino-0.4.948436673/src/vdk_trino.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:57.253954 vdk-trino-0.4.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3055 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/tests/test_ingest_to_trino.py
+-rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/tests/test_trino_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    21703 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/tests/test_vdk_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)    12904 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/tests/test_vdk_trino_lineage.py
+-rw-rw-rw-   0 root         (0) root         (0)     7086 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/tests/test_vdk_trino_lineage_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-07-28 09:43:32.000000 vdk-trino-0.4.948436673/tests/test_vdk_trino_utils.py
```

### Comparing `vdk-trino-0.4.944393829/PKG-INFO` & `vdk-trino-0.4.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-trino
-Version: 0.4.944393829
+Version: 0.4.948436673
 Summary: Versatile Data Kit SDK plugin provides support for trino database and trino transformation templates.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-trino-0.4.944393829/README.md` & `vdk-trino-0.4.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/setup.py` & `vdk-trino-0.4.948436673/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.4.944393829"
+__version__ = "0.4.948436673"
 
 setuptools.setup(
     name="vdk-trino",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for trino database and trino transformation templates.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/ingest_to_trino.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/ingest_to_trino.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/lineage_utils.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/lineage_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/00-verify-valid-target.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/00-verify-valid-target.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/06-move-data-from-tmp-to-target.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/06-move-data-from-tmp-to-target.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd1/README.md` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd1/README.md`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/00-verify-valid-target.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/00-verify-valid-target.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/01-add-props-for-args.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/01-add-props-for-args.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/06-insert-into-tmp-target.sql` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/06-insert-into-tmp-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/07-move-data-from-tmp-to-target.py.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/07-move-data-from-tmp-to-target.py.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/dimension/scd2/README.md` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/dimension/scd2/README.md`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/00-verify-valid-target.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/00-verify-valid-target.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/06-move-data-from-tmp-to-target.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/06-move-data-from-tmp-to-target.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/README.md` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/templates/load/fact/periodic_snapshot/README.md`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_config.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_config.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_connection.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_plugin.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk/plugin/trino/trino_utils.py` & `vdk-trino-0.4.948436673/src/vdk/plugin/trino/trino_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/src/vdk_trino.egg-info/PKG-INFO` & `vdk-trino-0.4.948436673/src/vdk_trino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-trino
-Version: 0.4.944393829
+Version: 0.4.948436673
 Summary: Versatile Data Kit SDK plugin provides support for trino database and trino transformation templates.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-trino-0.4.944393829/src/vdk_trino.egg-info/SOURCES.txt` & `vdk-trino-0.4.948436673/src/vdk_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/tests/test_ingest_to_trino.py` & `vdk-trino-0.4.948436673/tests/test_ingest_to_trino.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/tests/test_trino_sql.py` & `vdk-trino-0.4.948436673/tests/test_trino_sql.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/tests/test_vdk_templates.py` & `vdk-trino-0.4.948436673/tests/test_vdk_templates.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/tests/test_vdk_trino_lineage.py` & `vdk-trino-0.4.948436673/tests/test_vdk_trino_lineage.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/tests/test_vdk_trino_lineage_utils.py` & `vdk-trino-0.4.948436673/tests/test_vdk_trino_lineage_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-trino-0.4.944393829/tests/test_vdk_trino_utils.py` & `vdk-trino-0.4.948436673/tests/test_vdk_trino_utils.py`

 * *Files identical despite different names*

