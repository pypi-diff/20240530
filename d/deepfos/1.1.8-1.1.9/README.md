# Comparing `tmp/deepfos-1.1.8.tar.gz` & `tmp/deepfos-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfos-1.1.8.tar", last modified: Mon Sep  4 11:15:35 2023, max compression
+gzip compressed data, was "deepfos-1.1.9.tar", last modified: Mon Sep  4 11:15:46 2023, max compression
```

## Comparing `deepfos-1.1.8.tar` & `deepfos-1.1.9.tar`

### file list

```diff
@@ -1,186 +1,194 @@
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.440871 deepfos-1.1.8/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      138 2023-09-04 11:15:15.000000 deepfos-1.1.8/MANIFEST.in
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      600 2023-09-04 11:15:35.440871 deepfos-1.1.8/PKG-INFO
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      869 2023-09-04 11:15:23.000000 deepfos-1.1.8/README.md
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.422870 deepfos-1.1.8/deepfos/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      148 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    22390 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/_version.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.422870 deepfos-1.1.8/deepfos/algo/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/algo/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4974 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/algo/graph.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.424870 deepfos-1.1.8/deepfos/api/
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.424870 deepfos-1.1.8/deepfos/api/V1_1/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/api/V1_1/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3422 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/V1_1/business_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    21941 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/V1_1/dimension.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.425870 deepfos-1.1.8/deepfos/api/V1_1/models/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/api/V1_1/models/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    27844 2023-03-07 10:39:31.000000 deepfos-1.1.8/deepfos/api/V1_1/models/business_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    62934 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/api/V1_1/models/dimension.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.425870 deepfos-1.1.8/deepfos/api/V1_2/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/api/V1_2/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     9350 2023-09-04 11:14:57.000000 deepfos-1.1.8/deepfos/api/V1_2/dimension.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.425870 deepfos-1.1.8/deepfos/api/V1_2/models/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/api/V1_2/models/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    71828 2023-09-04 11:14:57.000000 deepfos-1.1.8/deepfos/api/V1_2/models/dimension.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/api/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4033 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/account.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4550 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/accounting_engines.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    23974 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/app.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6562 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/approval_process.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    32722 2023-09-04 11:15:23.000000 deepfos-1.1.8/deepfos/api/base.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5714 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/business_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3956 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/consolidation.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    10220 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/api/datatable.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2644 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/deepfos_task.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    14650 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/dimension.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     8702 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/financial_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3730 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/journal_template.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2812 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/memory_financial_model.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.428870 deepfos-1.1.8/deepfos/api/models/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)       64 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/api/models/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    11736 2023-04-13 06:45:39.000000 deepfos-1.1.8/deepfos/api/models/account.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    21041 2023-01-05 10:14:03.000000 deepfos-1.1.8/deepfos/api/models/accounting_engines.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    34219 2022-08-25 09:03:15.000000 deepfos-1.1.8/deepfos/api/models/app.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    24284 2022-08-01 09:26:10.000000 deepfos-1.1.8/deepfos/api/models/approval_process.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     7441 2023-01-05 06:56:53.000000 deepfos-1.1.8/deepfos/api/models/base.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    21580 2023-03-07 10:39:31.000000 deepfos-1.1.8/deepfos/api/models/business_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    20461 2022-01-19 02:14:35.000000 deepfos-1.1.8/deepfos/api/models/consolidation.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    11956 2022-01-19 02:14:35.000000 deepfos-1.1.8/deepfos/api/models/datatable_mysql.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    10606 2022-08-04 07:41:09.000000 deepfos-1.1.8/deepfos/api/models/deepfos_task.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    33688 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/api/models/dimension.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    48552 2023-02-02 02:05:17.000000 deepfos-1.1.8/deepfos/api/models/financial_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    22827 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/api/models/journal_template.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    13255 2022-08-29 06:42:41.000000 deepfos-1.1.8/deepfos/api/models/memory_financial_model.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3612 2022-08-11 07:36:12.000000 deepfos-1.1.8/deepfos/api/models/platform.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5121 2023-04-11 07:43:12.000000 deepfos-1.1.8/deepfos/api/models/python.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     9452 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/api/models/reconciliation_engine.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4054 2022-01-19 02:14:35.000000 deepfos-1.1.8/deepfos/api/models/reconciliation_report.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    21686 2022-08-11 07:36:12.000000 deepfos-1.1.8/deepfos/api/models/role_strategy.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5214 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/api/models/smartlist.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    27700 2023-03-02 07:17:32.000000 deepfos-1.1.8/deepfos/api/models/space.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    15192 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/api/models/system.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    11241 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/api/models/variable.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    22057 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/api/models/workflow.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6356 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/platform.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2126 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/python.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4994 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/api/reconciliation_engine.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     1737 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/reconciliation_report.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     8575 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/role_strategy.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     1786 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/smartlist.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    20148 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/space.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6453 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/system.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4231 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/api/variable.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     8062 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/api/workflow.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.439871 deepfos-1.1.8/deepfos/boost/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      174 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/boost/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)   159611 2023-04-06 04:36:08.000000 deepfos-1.1.8/deepfos/boost/jstream.c
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3035 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/boost/jstream.pyx
--rw-rw-r--   0 doc_user (10001) doc_user (10001)   150099 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/boost/pandas.c
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      927 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/boost/pandas.pyx
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2860 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/boost/py_jstream.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      693 2022-10-19 03:55:19.000000 deepfos-1.1.8/deepfos/boost/py_pandas.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2983 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/cache.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      111 2023-01-04 05:52:16.000000 deepfos-1.1.8/deepfos/config.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.428870 deepfos-1.1.8/deepfos/core/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      780 2023-09-04 11:14:57.000000 deepfos-1.1.8/deepfos/core/__init__.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.429870 deepfos-1.1.8/deepfos/core/cube/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      156 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/core/cube/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    15060 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/core/cube/_base.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      316 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/core/cube/constants.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    14802 2023-02-07 03:39:16.000000 deepfos-1.1.8/deepfos/core/cube/cube.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    21838 2023-02-07 03:39:16.000000 deepfos-1.1.8/deepfos/core/cube/formula.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    18781 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/core/cube/syscube.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      156 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/core/cube/typing.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6022 2023-02-07 06:25:21.000000 deepfos-1.1.8/deepfos/core/cube/utils.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.430870 deepfos-1.1.8/deepfos/core/dimension/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      348 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/core/dimension/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    14253 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/core/dimension/_base.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5613 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/core/dimension/dimcreator.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    16497 2023-09-04 11:13:12.000000 deepfos-1.1.8/deepfos/core/dimension/dimension.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     7957 2023-03-01 02:26:32.000000 deepfos-1.1.8/deepfos/core/dimension/dimexpr.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5349 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/core/dimension/dimmember.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      720 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/core/dimension/eledimension.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2693 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/core/dimension/filters.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6089 2023-02-07 03:39:16.000000 deepfos-1.1.8/deepfos/core/dimension/sysdimension.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.430870 deepfos-1.1.8/deepfos/core/logictable/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      190 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/core/logictable/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4830 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/core/logictable/_cache.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    20447 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/core/logictable/_operator.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    19532 2023-09-04 11:13:12.000000 deepfos-1.1.8/deepfos/core/logictable/nodemixin.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    21063 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/core/logictable/sqlcondition.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    17933 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/core/logictable/tablemodel.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.432870 deepfos-1.1.8/deepfos/db/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     1418 2023-09-04 11:14:57.000000 deepfos-1.1.8/deepfos/db/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    53960 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/db/cipher.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5831 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/clickhouse.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5358 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/db/connector.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5041 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/db/daclickhouse.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2898 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/db/dameng.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5838 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/db/damysql.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    11646 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/db/dbkits.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2824 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/deepengine.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2257 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/db/gauss.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2304 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/db/kingbase.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5482 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/mysql.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3826 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/oracle.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5950 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/postgresql.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2765 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/sqlserver.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4411 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/db/utils.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.433871 deepfos-1.1.8/deepfos/element/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     3253 2023-09-04 11:14:57.000000 deepfos-1.1.8/deepfos/element/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    14927 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/element/accounting.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6648 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/apvlprocess.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    12505 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/element/base.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    48158 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/bizmodel.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    73611 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/datatable.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    31284 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/dimension.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    15220 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/element/fact_table.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    40215 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/finmodel.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    34305 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/journal_template.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    12234 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/pyscript.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    15664 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/element/reconciliation.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     7410 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/element/rolestrategy.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    14760 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/element/smartlist.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    24334 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/element/variable.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    16668 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/element/workflow.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.434871 deepfos-1.1.8/deepfos/exceptions/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2852 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/exceptions/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2166 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/exceptions/hook.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2812 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/lazy.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.438871 deepfos-1.1.8/deepfos/lib/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/lib/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     9552 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/lib/_javaobj.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    23388 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/lib/asynchronous.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2723 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/lib/concurrency.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      867 2023-01-05 06:56:53.000000 deepfos-1.1.8/deepfos/lib/constant.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     8000 2023-09-04 11:14:48.000000 deepfos-1.1.8/deepfos/lib/decorator.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    27486 2023-09-04 11:15:23.000000 deepfos-1.1.8/deepfos/lib/deepchart.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6012 2023-09-04 11:15:32.000000 deepfos-1.1.8/deepfos/lib/deepux.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5300 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/lib/discovery.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5174 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/lib/eureka.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    24403 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/lib/filterparser.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2716 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/lib/httpcli.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2209 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/lib/jsonstreamer.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6836 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/lib/nacos.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2369 2022-01-17 05:58:38.000000 deepfos-1.1.8/deepfos/lib/patch.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6230 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/lib/redis.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     2366 2023-06-29 07:57:23.000000 deepfos-1.1.8/deepfos/lib/stopwatch.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    17585 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/lib/subtask.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    22192 2023-09-04 11:13:28.000000 deepfos-1.1.8/deepfos/lib/sysutils.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    25484 2023-09-04 11:14:39.000000 deepfos-1.1.8/deepfos/lib/utils.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     6442 2023-01-04 05:52:16.000000 deepfos-1.1.8/deepfos/local.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    19743 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/options.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     5647 2023-09-04 11:15:15.000000 deepfos-1.1.8/deepfos/translation.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.439871 deepfos-1.1.8/deepfos.egg-info/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      600 2023-09-04 11:15:35.000000 deepfos-1.1.8/deepfos.egg-info/PKG-INFO
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     4946 2023-09-04 11:15:35.000000 deepfos-1.1.8/deepfos.egg-info/SOURCES.txt
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        1 2023-09-04 11:15:35.000000 deepfos-1.1.8/deepfos.egg-info/dependency_links.txt
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        1 2022-01-17 09:11:42.000000 deepfos-1.1.8/deepfos.egg-info/not-zip-safe
--rw-rw-r--   0 doc_user (10001) doc_user (10001)      239 2023-09-04 11:15:35.000000 deepfos-1.1.8/deepfos.egg-info/requires.txt
--rw-rw-r--   0 doc_user (10001) doc_user (10001)        8 2023-09-04 11:15:35.000000 deepfos-1.1.8/deepfos.egg-info/top_level.txt
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     1075 2023-09-04 11:15:35.440871 deepfos-1.1.8/setup.cfg
--rw-rw-r--   0 doc_user (10001) doc_user (10001)     1495 2023-09-04 11:15:34.000000 deepfos-1.1.8/setup.py
-drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:35.438871 deepfos-1.1.8/tests/
--rw-rw-r--   0 doc_user (10001) doc_user (10001)       54 2023-09-04 11:14:57.000000 deepfos-1.1.8/tests/__init__.py
--rw-rw-r--   0 doc_user (10001) doc_user (10001)    78657 2023-09-04 11:15:34.000000 deepfos-1.1.8/versioneer.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.629244 deepfos-1.1.9/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      138 2023-09-04 11:15:15.000000 deepfos-1.1.9/MANIFEST.in
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      600 2023-09-04 11:15:46.630244 deepfos-1.1.9/PKG-INFO
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      869 2023-09-04 11:15:23.000000 deepfos-1.1.9/README.md
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.610244 deepfos-1.1.9/deepfos/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      148 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    22386 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/_version.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.611244 deepfos-1.1.9/deepfos/algo/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/algo/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4974 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/algo/graph.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.613244 deepfos-1.1.9/deepfos/api/
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.613244 deepfos-1.1.9/deepfos/api/V1_1/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/api/V1_1/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3422 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/V1_1/business_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    21941 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/V1_1/dimension.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.614244 deepfos-1.1.9/deepfos/api/V1_1/models/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/api/V1_1/models/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    27844 2023-03-07 10:39:31.000000 deepfos-1.1.9/deepfos/api/V1_1/models/business_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    62934 2023-09-04 11:14:39.000000 deepfos-1.1.9/deepfos/api/V1_1/models/dimension.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.614244 deepfos-1.1.9/deepfos/api/V1_2/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/api/V1_2/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     9350 2023-09-04 11:14:57.000000 deepfos-1.1.9/deepfos/api/V1_2/dimension.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.614244 deepfos-1.1.9/deepfos/api/V1_2/models/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/api/V1_2/models/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    71828 2023-09-04 11:14:57.000000 deepfos-1.1.9/deepfos/api/V1_2/models/dimension.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/api/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4033 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/account.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4550 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/accounting_engines.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    23974 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/app.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6562 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/approval_process.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    32722 2023-09-04 11:15:23.000000 deepfos-1.1.9/deepfos/api/base.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5714 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/business_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3956 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/consolidation.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    10220 2023-09-04 11:14:39.000000 deepfos-1.1.9/deepfos/api/datatable.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2644 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/deepfos_task.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      798 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/api/deepmodel.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    14650 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/dimension.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     8702 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/financial_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3503 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/api/journal_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3730 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/journal_template.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2812 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/memory_financial_model.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.617244 deepfos-1.1.9/deepfos/api/models/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)       64 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/api/models/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    11736 2023-04-13 06:45:39.000000 deepfos-1.1.9/deepfos/api/models/account.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    21041 2023-01-05 10:14:03.000000 deepfos-1.1.9/deepfos/api/models/accounting_engines.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    34219 2022-08-25 09:03:15.000000 deepfos-1.1.9/deepfos/api/models/app.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    24284 2022-08-01 09:26:10.000000 deepfos-1.1.9/deepfos/api/models/approval_process.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     7441 2023-01-05 06:56:53.000000 deepfos-1.1.9/deepfos/api/models/base.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    21580 2023-03-07 10:39:31.000000 deepfos-1.1.9/deepfos/api/models/business_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    20461 2022-01-19 02:14:35.000000 deepfos-1.1.9/deepfos/api/models/consolidation.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    11956 2022-01-19 02:14:35.000000 deepfos-1.1.9/deepfos/api/models/datatable_mysql.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    10606 2022-08-04 07:41:09.000000 deepfos-1.1.9/deepfos/api/models/deepfos_task.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3753 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/api/models/deepmodel.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    33688 2023-09-04 11:14:39.000000 deepfos-1.1.9/deepfos/api/models/dimension.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    48552 2023-02-02 02:05:17.000000 deepfos-1.1.9/deepfos/api/models/financial_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     9166 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/api/models/journal_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    22827 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/api/models/journal_template.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    13255 2022-08-29 06:42:41.000000 deepfos-1.1.9/deepfos/api/models/memory_financial_model.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3612 2022-08-11 07:36:12.000000 deepfos-1.1.9/deepfos/api/models/platform.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5121 2023-04-11 07:43:12.000000 deepfos-1.1.9/deepfos/api/models/python.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     9452 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/api/models/reconciliation_engine.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4054 2022-01-19 02:14:35.000000 deepfos-1.1.9/deepfos/api/models/reconciliation_report.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    21686 2022-08-11 07:36:12.000000 deepfos-1.1.9/deepfos/api/models/role_strategy.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5214 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/api/models/smartlist.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    27700 2023-03-02 07:17:32.000000 deepfos-1.1.9/deepfos/api/models/space.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    15192 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/api/models/system.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    11241 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/api/models/variable.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    22057 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/api/models/workflow.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6356 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/platform.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2126 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/python.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4994 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/api/reconciliation_engine.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     1737 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/reconciliation_report.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     8575 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/role_strategy.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     1786 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/smartlist.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    20148 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/space.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6453 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/system.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4231 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/api/variable.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     8062 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/api/workflow.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.629244 deepfos-1.1.9/deepfos/boost/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      174 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/boost/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)   159611 2023-04-06 04:36:08.000000 deepfos-1.1.9/deepfos/boost/jstream.c
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3035 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/boost/jstream.pyx
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)   150099 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/boost/pandas.c
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      927 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/boost/pandas.pyx
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2860 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/boost/py_jstream.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      693 2022-10-19 03:55:19.000000 deepfos-1.1.9/deepfos/boost/py_pandas.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2983 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/cache.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      111 2023-01-04 05:52:16.000000 deepfos-1.1.9/deepfos/config.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.617244 deepfos-1.1.9/deepfos/core/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      780 2023-09-04 11:14:57.000000 deepfos-1.1.9/deepfos/core/__init__.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.618244 deepfos-1.1.9/deepfos/core/cube/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      156 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/core/cube/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    15060 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/core/cube/_base.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      316 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/core/cube/constants.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    14802 2023-02-07 03:39:16.000000 deepfos-1.1.9/deepfos/core/cube/cube.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    21838 2023-02-07 03:39:16.000000 deepfos-1.1.9/deepfos/core/cube/formula.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    18781 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/core/cube/syscube.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      156 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/core/cube/typing.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6022 2023-02-07 06:25:21.000000 deepfos-1.1.9/deepfos/core/cube/utils.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.619244 deepfos-1.1.9/deepfos/core/dimension/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      348 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/core/dimension/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    14253 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/core/dimension/_base.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5613 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/core/dimension/dimcreator.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    16497 2023-09-04 11:13:12.000000 deepfos-1.1.9/deepfos/core/dimension/dimension.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     7957 2023-03-01 02:26:32.000000 deepfos-1.1.9/deepfos/core/dimension/dimexpr.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5349 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/core/dimension/dimmember.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      720 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/core/dimension/eledimension.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2693 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/core/dimension/filters.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6089 2023-02-07 03:39:16.000000 deepfos-1.1.9/deepfos/core/dimension/sysdimension.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.620244 deepfos-1.1.9/deepfos/core/logictable/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      190 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/core/logictable/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4830 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/core/logictable/_cache.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    20447 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/core/logictable/_operator.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    19532 2023-09-04 11:13:12.000000 deepfos-1.1.9/deepfos/core/logictable/nodemixin.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    21063 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/core/logictable/sqlcondition.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    17933 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/core/logictable/tablemodel.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.622244 deepfos-1.1.9/deepfos/db/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     1418 2023-09-04 11:14:57.000000 deepfos-1.1.9/deepfos/db/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    53960 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/db/cipher.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5831 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/clickhouse.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5358 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/db/connector.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5041 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/db/daclickhouse.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2898 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/db/dameng.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5838 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/db/damysql.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    11646 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/db/dbkits.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2824 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/deepengine.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3646 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/db/edb.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2257 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/db/gauss.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2304 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/db/kingbase.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5482 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/mysql.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3826 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/oracle.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5950 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/postgresql.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2765 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/sqlserver.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     4411 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/db/utils.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.625244 deepfos-1.1.9/deepfos/element/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3506 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/element/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    14927 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/element/accounting.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6648 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/apvlprocess.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    12505 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/element/base.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    48158 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/bizmodel.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    73611 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/datatable.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    23566 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/element/deepmodel.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    31284 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/dimension.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    15220 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/element/fact_table.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    40215 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/finmodel.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    25940 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/element/journal.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    34305 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/journal_template.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    12234 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/pyscript.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    15684 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/element/reconciliation.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     7410 2023-09-04 11:14:39.000000 deepfos-1.1.9/deepfos/element/rolestrategy.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    14760 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/element/smartlist.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    24334 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/element/variable.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    16668 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/element/workflow.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.625244 deepfos-1.1.9/deepfos/exceptions/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     3282 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/exceptions/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2166 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/exceptions/hook.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2812 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/lazy.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.627244 deepfos-1.1.9/deepfos/lib/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        0 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/lib/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     9552 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/lib/_javaobj.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    23388 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/lib/asynchronous.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2723 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/lib/concurrency.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      867 2023-01-05 06:56:53.000000 deepfos-1.1.9/deepfos/lib/constant.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     8000 2023-09-04 11:14:48.000000 deepfos-1.1.9/deepfos/lib/decorator.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    27486 2023-09-04 11:15:23.000000 deepfos-1.1.9/deepfos/lib/deepchart.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6012 2023-09-04 11:15:32.000000 deepfos-1.1.9/deepfos/lib/deepux.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5300 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/lib/discovery.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5174 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/lib/eureka.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    24403 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/lib/filterparser.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2716 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/lib/httpcli.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2209 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/lib/jsonstreamer.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6836 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/lib/nacos.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2369 2022-01-17 05:58:38.000000 deepfos-1.1.9/deepfos/lib/patch.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6230 2023-09-04 11:14:39.000000 deepfos-1.1.9/deepfos/lib/redis.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2171 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/lib/serutils.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     2366 2023-06-29 07:57:23.000000 deepfos-1.1.9/deepfos/lib/stopwatch.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    17585 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/lib/subtask.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    22192 2023-09-04 11:13:28.000000 deepfos-1.1.9/deepfos/lib/sysutils.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    25468 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/lib/utils.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     6442 2023-01-04 05:52:16.000000 deepfos-1.1.9/deepfos/local.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    20029 2023-09-04 11:15:41.000000 deepfos-1.1.9/deepfos/options.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5647 2023-09-04 11:15:15.000000 deepfos-1.1.9/deepfos/translation.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.628244 deepfos-1.1.9/deepfos.egg-info/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      600 2023-09-04 11:15:46.000000 deepfos-1.1.9/deepfos.egg-info/PKG-INFO
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     5182 2023-09-04 11:15:46.000000 deepfos-1.1.9/deepfos.egg-info/SOURCES.txt
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        1 2023-09-04 11:15:46.000000 deepfos-1.1.9/deepfos.egg-info/dependency_links.txt
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        1 2022-01-17 09:11:42.000000 deepfos-1.1.9/deepfos.egg-info/not-zip-safe
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)      253 2023-09-04 11:15:46.000000 deepfos-1.1.9/deepfos.egg-info/requires.txt
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)        8 2023-09-04 11:15:46.000000 deepfos-1.1.9/deepfos.egg-info/top_level.txt
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     1090 2023-09-04 11:15:46.630244 deepfos-1.1.9/setup.cfg
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)     1495 2023-09-04 11:15:45.000000 deepfos-1.1.9/setup.py
+drwxrwxr-x   0 doc_user (10001) doc_user (10001)        0 2023-09-04 11:15:46.628244 deepfos-1.1.9/tests/
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)       54 2023-09-04 11:14:57.000000 deepfos-1.1.9/tests/__init__.py
+-rw-rw-r--   0 doc_user (10001) doc_user (10001)    78254 2023-09-04 11:15:45.000000 deepfos-1.1.9/versioneer.py
```

### Comparing `deepfos-1.1.8/PKG-INFO` & `deepfos-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfos
-Version: 1.1.8
+Version: 1.1.9
 Summary: Collecions of useful and handy tools for deepfos platform
 Home-page: http://py.deepfos.com
 Author: deepfos-python-team
 Author-email: wei.wei@proinnova.com.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deepfos-1.1.8/README.md` & `deepfos-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/_version.py` & `deepfos-1.1.9/deepfos/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "pep440"
     cfg.tag_prefix = "v"
     cfg.parentdir_prefix = "deepfos-"
-    cfg.versionfile_source = "deepfos_1_1/_version.py"
+    cfg.versionfile_source = "deepfos/_version.py"
     cfg.verbose = False
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
```

### Comparing `deepfos-1.1.8/deepfos/algo/graph.py` & `deepfos-1.1.9/deepfos/algo/graph.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/V1_1/business_model.py` & `deepfos-1.1.9/deepfos/api/V1_1/business_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/V1_1/dimension.py` & `deepfos-1.1.9/deepfos/api/V1_1/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/V1_1/models/business_model.py` & `deepfos-1.1.9/deepfos/api/V1_1/models/business_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/V1_1/models/dimension.py` & `deepfos-1.1.9/deepfos/api/V1_1/models/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/V1_2/dimension.py` & `deepfos-1.1.9/deepfos/api/V1_2/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/V1_2/models/dimension.py` & `deepfos-1.1.9/deepfos/api/V1_2/models/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/account.py` & `deepfos-1.1.9/deepfos/api/account.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/accounting_engines.py` & `deepfos-1.1.9/deepfos/api/accounting_engines.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/app.py` & `deepfos-1.1.9/deepfos/api/app.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/approval_process.py` & `deepfos-1.1.9/deepfos/api/approval_process.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/base.py` & `deepfos-1.1.9/deepfos/api/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/business_model.py` & `deepfos-1.1.9/deepfos/api/business_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/consolidation.py` & `deepfos-1.1.9/deepfos/api/consolidation.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/datatable.py` & `deepfos-1.1.9/deepfos/api/datatable.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/deepfos_task.py` & `deepfos-1.1.9/deepfos/api/deepfos_task.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/dimension.py` & `deepfos-1.1.9/deepfos/api/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/financial_model.py` & `deepfos-1.1.9/deepfos/api/financial_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/journal_template.py` & `deepfos-1.1.9/deepfos/api/journal_template.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/memory_financial_model.py` & `deepfos-1.1.9/deepfos/api/memory_financial_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/account.py` & `deepfos-1.1.9/deepfos/api/models/account.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/accounting_engines.py` & `deepfos-1.1.9/deepfos/api/models/accounting_engines.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/app.py` & `deepfos-1.1.9/deepfos/api/models/app.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/approval_process.py` & `deepfos-1.1.9/deepfos/api/models/approval_process.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/base.py` & `deepfos-1.1.9/deepfos/api/models/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/business_model.py` & `deepfos-1.1.9/deepfos/api/models/business_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/consolidation.py` & `deepfos-1.1.9/deepfos/api/models/consolidation.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/datatable_mysql.py` & `deepfos-1.1.9/deepfos/api/models/datatable_mysql.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/deepfos_task.py` & `deepfos-1.1.9/deepfos/api/models/deepfos_task.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/dimension.py` & `deepfos-1.1.9/deepfos/api/models/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/financial_model.py` & `deepfos-1.1.9/deepfos/api/models/financial_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/journal_template.py` & `deepfos-1.1.9/deepfos/api/models/journal_template.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/memory_financial_model.py` & `deepfos-1.1.9/deepfos/api/models/memory_financial_model.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/platform.py` & `deepfos-1.1.9/deepfos/api/models/platform.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/python.py` & `deepfos-1.1.9/deepfos/api/models/python.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/reconciliation_engine.py` & `deepfos-1.1.9/deepfos/api/models/reconciliation_engine.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/reconciliation_report.py` & `deepfos-1.1.9/deepfos/api/models/reconciliation_report.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/role_strategy.py` & `deepfos-1.1.9/deepfos/api/models/role_strategy.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/smartlist.py` & `deepfos-1.1.9/deepfos/api/models/smartlist.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/space.py` & `deepfos-1.1.9/deepfos/api/models/space.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/system.py` & `deepfos-1.1.9/deepfos/api/models/system.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/variable.py` & `deepfos-1.1.9/deepfos/api/models/variable.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/models/workflow.py` & `deepfos-1.1.9/deepfos/api/models/workflow.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/platform.py` & `deepfos-1.1.9/deepfos/api/platform.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/python.py` & `deepfos-1.1.9/deepfos/api/python.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/reconciliation_engine.py` & `deepfos-1.1.9/deepfos/api/reconciliation_engine.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/reconciliation_report.py` & `deepfos-1.1.9/deepfos/api/reconciliation_report.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/role_strategy.py` & `deepfos-1.1.9/deepfos/api/role_strategy.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/smartlist.py` & `deepfos-1.1.9/deepfos/api/smartlist.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/space.py` & `deepfos-1.1.9/deepfos/api/space.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/system.py` & `deepfos-1.1.9/deepfos/api/system.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/variable.py` & `deepfos-1.1.9/deepfos/api/variable.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/api/workflow.py` & `deepfos-1.1.9/deepfos/api/workflow.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/boost/jstream.c` & `deepfos-1.1.9/deepfos/boost/jstream.c`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/boost/jstream.pyx` & `deepfos-1.1.9/deepfos/boost/jstream.pyx`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/boost/pandas.c` & `deepfos-1.1.9/deepfos/boost/pandas.c`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/boost/pandas.pyx` & `deepfos-1.1.9/deepfos/boost/pandas.pyx`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/boost/py_jstream.py` & `deepfos-1.1.9/deepfos/boost/py_jstream.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/boost/py_pandas.py` & `deepfos-1.1.9/deepfos/boost/py_pandas.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/cache.py` & `deepfos-1.1.9/deepfos/cache.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/__init__.py` & `deepfos-1.1.9/deepfos/core/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/cube/_base.py` & `deepfos-1.1.9/deepfos/core/cube/_base.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/cube/cube.py` & `deepfos-1.1.9/deepfos/core/cube/cube.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/cube/formula.py` & `deepfos-1.1.9/deepfos/core/cube/formula.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/cube/syscube.py` & `deepfos-1.1.9/deepfos/core/cube/syscube.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/cube/utils.py` & `deepfos-1.1.9/deepfos/core/cube/utils.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/_base.py` & `deepfos-1.1.9/deepfos/core/dimension/_base.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/dimcreator.py` & `deepfos-1.1.9/deepfos/core/dimension/dimcreator.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/dimension.py` & `deepfos-1.1.9/deepfos/core/dimension/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/dimexpr.py` & `deepfos-1.1.9/deepfos/core/dimension/dimexpr.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/dimmember.py` & `deepfos-1.1.9/deepfos/core/dimension/dimmember.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/eledimension.py` & `deepfos-1.1.9/deepfos/core/dimension/eledimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/filters.py` & `deepfos-1.1.9/deepfos/core/dimension/filters.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/dimension/sysdimension.py` & `deepfos-1.1.9/deepfos/core/dimension/sysdimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/logictable/_cache.py` & `deepfos-1.1.9/deepfos/core/logictable/_cache.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/logictable/_operator.py` & `deepfos-1.1.9/deepfos/core/logictable/_operator.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/logictable/nodemixin.py` & `deepfos-1.1.9/deepfos/core/logictable/nodemixin.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/logictable/sqlcondition.py` & `deepfos-1.1.9/deepfos/core/logictable/sqlcondition.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/core/logictable/tablemodel.py` & `deepfos-1.1.9/deepfos/core/logictable/tablemodel.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/__init__.py` & `deepfos-1.1.9/deepfos/db/__init__.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/cipher.py` & `deepfos-1.1.9/deepfos/db/cipher.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/clickhouse.py` & `deepfos-1.1.9/deepfos/db/clickhouse.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/connector.py` & `deepfos-1.1.9/deepfos/db/connector.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/daclickhouse.py` & `deepfos-1.1.9/deepfos/db/daclickhouse.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/dameng.py` & `deepfos-1.1.9/deepfos/db/dameng.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/damysql.py` & `deepfos-1.1.9/deepfos/db/damysql.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/dbkits.py` & `deepfos-1.1.9/deepfos/db/dbkits.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/deepengine.py` & `deepfos-1.1.9/deepfos/db/deepengine.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/gauss.py` & `deepfos-1.1.9/deepfos/db/gauss.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/kingbase.py` & `deepfos-1.1.9/deepfos/db/kingbase.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/mysql.py` & `deepfos-1.1.9/deepfos/db/mysql.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/oracle.py` & `deepfos-1.1.9/deepfos/db/oracle.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/postgresql.py` & `deepfos-1.1.9/deepfos/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/sqlserver.py` & `deepfos-1.1.9/deepfos/db/sqlserver.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/db/utils.py` & `deepfos-1.1.9/deepfos/db/utils.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/__init__.py` & `deepfos-1.1.9/deepfos/element/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     from .journal_template import (
         AsyncJournalTemplate, JournalTemplate, FullPostingParameter
     )
     from .rolestrategy import AsyncRoleStrategy, RoleStrategy
     from .smartlist import AsyncSmartList, SmartList
     from .variable import AsyncVariable, Variable
     from .workflow import AsyncWorkFlow, WorkFlow
+    from .journal import AsyncJournalModel, JournalModel
+    from .deepmodel import AsyncDeepModel, DeepModel
 
 
 lazify(
     {
         'deepfos.element.finmodel': (
             'AsyncFinancialCube', 'FinancialCube'
         ),
@@ -68,10 +70,12 @@
         'deepfos.element.smartlist': ('AsyncSmartList', 'SmartList'),
         'deepfos.element.variable': ('AsyncVariable', 'Variable'),
         'deepfos.element.workflow': ('AsyncWorkFlow', 'WorkFlow'),
         'deepfos.element.reconciliation': (
             'AsyncReconciliationEngine', 'AsyncReconciliationMsEngine',
             'ReconciliationEngine', 'ReconciliationMsEngine',
         ),
+        'deepfos.element.journal': ('AsyncJournalModel', 'JournalModel'),
+        'deepfos.element.deepmodel': ('AsyncDeepModel', 'DeepModel')
     },
     globals()
 )
```

### Comparing `deepfos-1.1.8/deepfos/element/accounting.py` & `deepfos-1.1.9/deepfos/element/accounting.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/apvlprocess.py` & `deepfos-1.1.9/deepfos/element/apvlprocess.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/base.py` & `deepfos-1.1.9/deepfos/element/base.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/bizmodel.py` & `deepfos-1.1.9/deepfos/element/bizmodel.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/datatable.py` & `deepfos-1.1.9/deepfos/element/datatable.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/dimension.py` & `deepfos-1.1.9/deepfos/element/dimension.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/fact_table.py` & `deepfos-1.1.9/deepfos/element/fact_table.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/finmodel.py` & `deepfos-1.1.9/deepfos/element/finmodel.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/journal_template.py` & `deepfos-1.1.9/deepfos/element/journal_template.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/pyscript.py` & `deepfos-1.1.9/deepfos/element/pyscript.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/reconciliation.py` & `deepfos-1.1.9/deepfos/element/reconciliation.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,15 @@
         'close_task',
         'open_task',
         'delete_task',
         'mark_by_hand',
         'cancel_by_hand',
         'cancel_matched',
     )
-    if TYPE_CHECKING:
+    if TYPE_CHECKING:  # pragma: no cover
         def execute(
             self,
             pov: Dict[str, str],
             params: AccountInfoParam = None,
             task_id: str = None,
             task_name: str = None
         ) -> int:
```

### Comparing `deepfos-1.1.8/deepfos/element/rolestrategy.py` & `deepfos-1.1.9/deepfos/element/rolestrategy.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/smartlist.py` & `deepfos-1.1.9/deepfos/element/smartlist.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/variable.py` & `deepfos-1.1.9/deepfos/element/variable.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/element/workflow.py` & `deepfos-1.1.9/deepfos/element/workflow.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/exceptions/__init__.py` & `deepfos-1.1.9/deepfos/exceptions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -123,7 +123,25 @@
     """任务并发数过高"""
 
 
 # -----------------------------------------------------------------------------
 # FinancialCube Error
 class MDXExecuteTimeout(DeepfosBaseException):
     """执行MDX任务超时"""
+
+
+# -----------------------------------------------------------------------------
+# EdgeDB Error
+class EdgeDBError(DeepfosBaseException):
+    """EdgeDB相关报错基类"""
+
+
+class NonExternalObjectNotExist(EdgeDBError):
+    """EdgeDB非外部对象不存在"""
+
+
+class ExternalObjectReadOnly(EdgeDBError):
+    """EdgeDB外部对象只可读"""
+
+
+class RequiredFieldUnfilled(EdgeDBError):
+    """Insert语句缺少必填字段"""
```

### Comparing `deepfos-1.1.8/deepfos/exceptions/hook.py` & `deepfos-1.1.9/deepfos/exceptions/hook.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lazy.py` & `deepfos-1.1.9/deepfos/lazy.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/_javaobj.py` & `deepfos-1.1.9/deepfos/lib/_javaobj.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/asynchronous.py` & `deepfos-1.1.9/deepfos/lib/asynchronous.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/concurrency.py` & `deepfos-1.1.9/deepfos/lib/concurrency.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/constant.py` & `deepfos-1.1.9/deepfos/lib/constant.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/decorator.py` & `deepfos-1.1.9/deepfos/lib/decorator.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/deepchart.py` & `deepfos-1.1.9/deepfos/lib/deepchart.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/deepux.py` & `deepfos-1.1.9/deepfos/lib/deepux.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/discovery.py` & `deepfos-1.1.9/deepfos/lib/discovery.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/eureka.py` & `deepfos-1.1.9/deepfos/lib/eureka.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/filterparser.py` & `deepfos-1.1.9/deepfos/lib/filterparser.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/httpcli.py` & `deepfos-1.1.9/deepfos/lib/httpcli.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/jsonstreamer.py` & `deepfos-1.1.9/deepfos/lib/jsonstreamer.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/nacos.py` & `deepfos-1.1.9/deepfos/lib/nacos.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/patch.py` & `deepfos-1.1.9/deepfos/lib/patch.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/redis.py` & `deepfos-1.1.9/deepfos/lib/redis.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/stopwatch.py` & `deepfos-1.1.9/deepfos/lib/stopwatch.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/subtask.py` & `deepfos-1.1.9/deepfos/lib/subtask.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/sysutils.py` & `deepfos-1.1.9/deepfos/lib/sysutils.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/lib/utils.py` & `deepfos-1.1.9/deepfos/lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 from loguru import logger
 import pandas as pd
 
 from deepfos.lib.constant import RE_DIMNAME_PARSER, ACCEPT_LANS, UNSET
 
 
 FORCE_POP = [
-    'deepfos_1_1.element.datatable',
-    'deepfos_1_1.db.mysql',
-    'deepfos_1_1.db.clickhouse',
-    'deepfos_1_1.lib.subtask',
+    'deepfos.element.datatable',
+    'deepfos.db.mysql',
+    'deepfos.db.clickhouse',
+    'deepfos.lib.subtask',
 ]
 
 # -----------------------------------------------------------------------------
 # typing
 KT = TypeVar('KT')
 VT = TypeVar('VT')
```

### Comparing `deepfos-1.1.8/deepfos/local.py` & `deepfos-1.1.9/deepfos/local.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos/options.py` & `deepfos-1.1.9/deepfos/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # extra check / trigger / convertors
 def _check_number_range(number, minimum=None, maximum=None):
     if minimum is not None:
         if number < minimum:
             raise ValueError(f"Value should be greater than {minimum}")
     if maximum is not None:
         if number > maximum:
-            raise ValueError(f"Value should be less than {minimum}")
+            raise ValueError(f"Value should be less than {maximum}")
 
 
 def _reset_level(level: str):
     logger.remove()
     if level.upper() == 'DISABLED':
         return
     logger.configure(
@@ -449,14 +449,25 @@
     url = _Option('', val_type=str)
 
     def __get__(self, instance, owner) -> '_Redis':
         """defined to help ide"""
         return super().__get__(instance, owner)
 
 
+class _Edgedb(_Category):
+    __id__ = 'edgedb'
+
+    dsn = _Option('', val_type=str)
+    timeout = _Option(30, val_type=int)
+
+    def __get__(self, instance, owner) -> '_Edgedb':
+        """defined to help ide"""
+        return super().__get__(instance, owner)
+
+
 class _Boost(_Category):
     __id__ = 'boost'
 
     skip_internal_existence_check = _Option(False, val_type=bool)
 
     def __get__(self, instance, owner) -> '_Boost':
         """defined to help ide"""
@@ -496,14 +507,15 @@
     server = _Server()
     api = _API()
     redis = _Redis()
     module = _Module()
     boost = _Boost()
     discovery = _ServiceDiscovery()
     nacos = _Nacos()
+    edgedb = _Edgedb()
 
     def load_file(self, filepath):
         parser = configparser.ConfigParser()
         parser.read(filepath, encoding='utf8')
         self.load_env(parser)
 
     def load_env(self, env):
```

### Comparing `deepfos-1.1.8/deepfos/translation.py` & `deepfos-1.1.9/deepfos/translation.py`

 * *Files identical despite different names*

### Comparing `deepfos-1.1.8/deepfos.egg-info/PKG-INFO` & `deepfos-1.1.9/deepfos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfos
-Version: 1.1.8
+Version: 1.1.9
 Summary: Collecions of useful and handy tools for deepfos platform
 Home-page: http://py.deepfos.com
 Author: deepfos-python-team
 Author-email: wei.wei@proinnova.com.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deepfos-1.1.8/deepfos.egg-info/SOURCES.txt` & `deepfos-1.1.9/deepfos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 ./deepfos/api/app.py
 ./deepfos/api/approval_process.py
 ./deepfos/api/base.py
 ./deepfos/api/business_model.py
 ./deepfos/api/consolidation.py
 ./deepfos/api/datatable.py
 ./deepfos/api/deepfos_task.py
+./deepfos/api/deepmodel.py
 ./deepfos/api/dimension.py
 ./deepfos/api/financial_model.py
+./deepfos/api/journal_model.py
 ./deepfos/api/journal_template.py
 ./deepfos/api/memory_financial_model.py
 ./deepfos/api/platform.py
 ./deepfos/api/python.py
 ./deepfos/api/reconciliation_engine.py
 ./deepfos/api/reconciliation_report.py
 ./deepfos/api/role_strategy.py
@@ -53,16 +55,18 @@
 ./deepfos/api/models/app.py
 ./deepfos/api/models/approval_process.py
 ./deepfos/api/models/base.py
 ./deepfos/api/models/business_model.py
 ./deepfos/api/models/consolidation.py
 ./deepfos/api/models/datatable_mysql.py
 ./deepfos/api/models/deepfos_task.py
+./deepfos/api/models/deepmodel.py
 ./deepfos/api/models/dimension.py
 ./deepfos/api/models/financial_model.py
+./deepfos/api/models/journal_model.py
 ./deepfos/api/models/journal_template.py
 ./deepfos/api/models/memory_financial_model.py
 ./deepfos/api/models/platform.py
 ./deepfos/api/models/python.py
 ./deepfos/api/models/reconciliation_engine.py
 ./deepfos/api/models/reconciliation_report.py
 ./deepfos/api/models/role_strategy.py
@@ -103,30 +107,33 @@
 ./deepfos/db/clickhouse.py
 ./deepfos/db/connector.py
 ./deepfos/db/daclickhouse.py
 ./deepfos/db/dameng.py
 ./deepfos/db/damysql.py
 ./deepfos/db/dbkits.py
 ./deepfos/db/deepengine.py
+./deepfos/db/edb.py
 ./deepfos/db/gauss.py
 ./deepfos/db/kingbase.py
 ./deepfos/db/mysql.py
 ./deepfos/db/oracle.py
 ./deepfos/db/postgresql.py
 ./deepfos/db/sqlserver.py
 ./deepfos/db/utils.py
 ./deepfos/element/__init__.py
 ./deepfos/element/accounting.py
 ./deepfos/element/apvlprocess.py
 ./deepfos/element/base.py
 ./deepfos/element/bizmodel.py
 ./deepfos/element/datatable.py
+./deepfos/element/deepmodel.py
 ./deepfos/element/dimension.py
 ./deepfos/element/fact_table.py
 ./deepfos/element/finmodel.py
+./deepfos/element/journal.py
 ./deepfos/element/journal_template.py
 ./deepfos/element/pyscript.py
 ./deepfos/element/reconciliation.py
 ./deepfos/element/rolestrategy.py
 ./deepfos/element/smartlist.py
 ./deepfos/element/variable.py
 ./deepfos/element/workflow.py
@@ -144,14 +151,15 @@
 ./deepfos/lib/eureka.py
 ./deepfos/lib/filterparser.py
 ./deepfos/lib/httpcli.py
 ./deepfos/lib/jsonstreamer.py
 ./deepfos/lib/nacos.py
 ./deepfos/lib/patch.py
 ./deepfos/lib/redis.py
+./deepfos/lib/serutils.py
 ./deepfos/lib/stopwatch.py
 ./deepfos/lib/subtask.py
 ./deepfos/lib/sysutils.py
 ./deepfos/lib/utils.py
 ./tests/__init__.py
 deepfos/_version.py
 deepfos.egg-info/PKG-INFO
```

### Comparing `deepfos-1.1.8/setup.cfg` & `deepfos-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 	PyPika==0.48.8
 	aiomysql==0.0.22
 	clickhouse-driver==0.2.2
 	aioredis==2.0.1
 	redis==3.5.3
 	deepfos-ipc~=1.2.3
 	typing-extensions==4.5.0
+	edgedb~=1.4.0
 python_requires = 
 	>=3.8.3
 
 [options.packages.find]
 where = .
 exclude = tests*
```

### Comparing `deepfos-1.1.8/setup.py` & `deepfos-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,11 +48,11 @@
             ),
         ]
         extensions.extend(c_exts)
     return extensions
 
 
 setup(
-    version="1.1.8",
+    version="1.1.9",
     # cmdclass=versioneer.get_cmdclass(),
     ext_modules=resolve_extensions()
 )
```

### Comparing `deepfos-1.1.8/versioneer.py` & `deepfos-1.1.9/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1869,22 +1869,14 @@
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
-            with open(os.path.join(base_dir, 'setup.py'), 'r') as fp:
-                ori = fp.read()
-                new_content = ori.replace('deepfos', 'deepfos')
-
-            if new_content:
-                with open(os.path.join(base_dir, 'setup.py'), 'w') as fp:
-                    fp.write(new_content)
-            os.rename(os.path.join(base_dir, 'deepfos'), os.path.join(base_dir, 'deepfos'))
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile,
                                   self._versioneer_generated_versions)
     cmds["sdist"] = cmd_sdist
 
     return cmds
```

