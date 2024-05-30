# Comparing `tmp/pfmongo-0.9.98.tar.gz` & `tmp/pfmongo-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfmongo-0.9.98.tar", last modified: Thu Jan 18 05:15:33 2024, max compression
+gzip compressed data, was "pfmongo-0.9.99.tar", last modified: Thu Jan 18 05:27:30 2024, max compression
```

## Comparing `pfmongo-0.9.98.tar` & `pfmongo-0.9.99.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.101745 pfmongo-0.9.98/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11357 2023-09-07 00:22:51.000000 pfmongo-0.9.98/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2946 2024-01-18 05:15:33.101745 pfmongo-0.9.98/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2726 2024-01-17 00:12:36.000000 pfmongo-0.9.98/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.095745 pfmongo-0.9.98/pfmongo/
--rwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)      185 2023-09-07 00:22:53.000000 pfmongo-0.9.98/pfmongo/__init__.py
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     4311 2024-01-18 05:14:30.000000 pfmongo-0.9.98/pfmongo/__main__.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.096746 pfmongo-0.9.98/pfmongo/commands/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-09-11 19:33:46.000000 pfmongo-0.9.98/pfmongo/commands/__init__.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.098745 pfmongo-0.9.98/pfmongo/commands/clop/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     4843 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/clop/add.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      868 2024-01-16 23:12:39.000000 pfmongo-0.9.98/pfmongo/commands/clop/connect.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1677 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/clop/delete.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1334 2024-01-16 23:13:22.000000 pfmongo-0.9.98/pfmongo/commands/clop/deleteCol.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1157 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/clop/get.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      979 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/clop/list.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1413 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/clop/search.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      656 2024-01-16 23:57:00.000000 pfmongo-0.9.98/pfmongo/commands/clop/showAll.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      837 2024-01-16 23:12:14.000000 pfmongo-0.9.98/pfmongo/commands/collection.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      584 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/database.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.098745 pfmongo-0.9.98/pfmongo/commands/dbop/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      814 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/dbop/connect.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1120 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/commands/dbop/deleteDB.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      606 2023-09-26 19:03:51.000000 pfmongo-0.9.98/pfmongo/commands/dbop/showAll.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      643 2024-01-16 16:52:15.000000 pfmongo-0.9.98/pfmongo/commands/document.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.100746 pfmongo-0.9.98/pfmongo/commands/fop/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-09-11 19:53:19.000000 pfmongo-0.9.98/pfmongo/commands/fop/__init__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      443 2023-09-15 02:26:53.000000 pfmongo-0.9.98/pfmongo/commands/fop/cat.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      783 2023-09-15 02:29:13.000000 pfmongo-0.9.98/pfmongo/commands/fop/cd.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      566 2023-09-17 17:31:38.000000 pfmongo-0.9.98/pfmongo/commands/fop/exp.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      589 2023-09-17 17:33:58.000000 pfmongo-0.9.98/pfmongo/commands/fop/imp.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      918 2023-09-15 02:32:29.000000 pfmongo-0.9.98/pfmongo/commands/fop/ls.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      594 2023-09-15 02:33:17.000000 pfmongo-0.9.98/pfmongo/commands/fop/mkdir.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1072 2023-09-18 23:42:47.000000 pfmongo-0.9.98/pfmongo/commands/fs.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2471 2023-09-19 13:28:09.000000 pfmongo-0.9.98/pfmongo/commands/man.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      603 2023-10-02 22:23:31.000000 pfmongo-0.9.98/pfmongo/commands/state.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.100746 pfmongo-0.9.98/pfmongo/commands/stateop/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1414 2024-01-18 03:34:10.000000 pfmongo-0.9.98/pfmongo/commands/stateop/showAll.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.100746 pfmongo-0.9.98/pfmongo/config/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      166 2023-09-07 00:22:53.000000 pfmongo-0.9.98/pfmongo/config/__init__.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1556 2024-01-12 22:20:25.000000 pfmongo-0.9.98/pfmongo/config/settings.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.100746 pfmongo-0.9.98/pfmongo/db/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    20226 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/db/pfdb.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6439 2024-01-18 05:13:33.000000 pfmongo-0.9.98/pfmongo/driver.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    30775 2024-01-16 23:15:50.000000 pfmongo-0.9.98/pfmongo/env.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.101745 pfmongo-0.9.98/pfmongo/models/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      532 2023-09-26 17:24:31.000000 pfmongo-0.9.98/pfmongo/models/dataModel.py
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5569 2024-01-12 13:56:52.000000 pfmongo-0.9.98/pfmongo/models/responseModel.py
--rwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)    24420 2024-01-12 22:37:24.000000 pfmongo-0.9.98/pfmongo/pfmongo.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.096746 pfmongo-0.9.98/pfmongo.egg-info/
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     2946 2024-01-18 05:15:33.000000 pfmongo-0.9.98/pfmongo.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1290 2024-01-18 05:15:33.000000 pfmongo-0.9.98/pfmongo.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-01-18 05:15:33.000000 pfmongo-0.9.98/pfmongo.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       50 2024-01-18 05:15:33.000000 pfmongo-0.9.98/pfmongo.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-09-13 14:02:08.000000 pfmongo-0.9.98/pfmongo.egg-info/not-zip-safe
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      115 2024-01-18 05:15:33.000000 pfmongo-0.9.98/pfmongo.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      156 2024-01-18 05:15:33.000000 pfmongo-0.9.98/pfmongo.egg-info/top_level.txt
--rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      167 2024-01-18 03:33:37.000000 pfmongo-0.9.98/requirements.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-01-18 05:15:33.101745 pfmongo-0.9.98/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2152 2024-01-18 00:19:38.000000 pfmongo-0.9.98/setup.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:15:33.101745 pfmongo-0.9.98/tests/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1650 2023-09-17 17:53:43.000000 pfmongo-0.9.98/tests/test_pfmongo.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.496887 pfmongo-0.9.99/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11357 2023-09-07 00:22:51.000000 pfmongo-0.9.99/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2946 2024-01-18 05:27:30.496887 pfmongo-0.9.99/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2726 2024-01-17 00:12:36.000000 pfmongo-0.9.99/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.491887 pfmongo-0.9.99/pfmongo/
+-rwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)      185 2023-09-07 00:22:53.000000 pfmongo-0.9.99/pfmongo/__init__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     4311 2024-01-18 05:26:38.000000 pfmongo-0.9.99/pfmongo/__main__.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.493887 pfmongo-0.9.99/pfmongo/commands/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-09-11 19:33:46.000000 pfmongo-0.9.99/pfmongo/commands/__init__.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.494887 pfmongo-0.9.99/pfmongo/commands/clop/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     4843 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/clop/add.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      868 2024-01-16 23:12:39.000000 pfmongo-0.9.99/pfmongo/commands/clop/connect.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1677 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/clop/delete.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1334 2024-01-16 23:13:22.000000 pfmongo-0.9.99/pfmongo/commands/clop/deleteCol.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1157 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/clop/get.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      979 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/clop/list.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1413 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/clop/search.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      656 2024-01-16 23:57:00.000000 pfmongo-0.9.99/pfmongo/commands/clop/showAll.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      837 2024-01-16 23:12:14.000000 pfmongo-0.9.99/pfmongo/commands/collection.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      584 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/database.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.494887 pfmongo-0.9.99/pfmongo/commands/dbop/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      814 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/dbop/connect.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1120 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/commands/dbop/deleteDB.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      606 2023-09-26 19:03:51.000000 pfmongo-0.9.99/pfmongo/commands/dbop/showAll.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      643 2024-01-16 16:52:15.000000 pfmongo-0.9.99/pfmongo/commands/document.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.495887 pfmongo-0.9.99/pfmongo/commands/fop/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        0 2023-09-11 19:53:19.000000 pfmongo-0.9.99/pfmongo/commands/fop/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      443 2023-09-15 02:26:53.000000 pfmongo-0.9.99/pfmongo/commands/fop/cat.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      783 2023-09-15 02:29:13.000000 pfmongo-0.9.99/pfmongo/commands/fop/cd.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      566 2023-09-17 17:31:38.000000 pfmongo-0.9.99/pfmongo/commands/fop/exp.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      589 2023-09-17 17:33:58.000000 pfmongo-0.9.99/pfmongo/commands/fop/imp.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      918 2023-09-15 02:32:29.000000 pfmongo-0.9.99/pfmongo/commands/fop/ls.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      594 2023-09-15 02:33:17.000000 pfmongo-0.9.99/pfmongo/commands/fop/mkdir.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1072 2023-09-18 23:42:47.000000 pfmongo-0.9.99/pfmongo/commands/fs.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2471 2023-09-19 13:28:09.000000 pfmongo-0.9.99/pfmongo/commands/man.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      603 2023-10-02 22:23:31.000000 pfmongo-0.9.99/pfmongo/commands/state.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.495887 pfmongo-0.9.99/pfmongo/commands/stateop/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1414 2024-01-18 03:34:10.000000 pfmongo-0.9.99/pfmongo/commands/stateop/showAll.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.496887 pfmongo-0.9.99/pfmongo/config/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      166 2023-09-07 00:22:53.000000 pfmongo-0.9.99/pfmongo/config/__init__.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1556 2024-01-12 22:20:25.000000 pfmongo-0.9.99/pfmongo/config/settings.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.496887 pfmongo-0.9.99/pfmongo/db/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    20226 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/db/pfdb.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     6453 2024-01-18 05:26:08.000000 pfmongo-0.9.99/pfmongo/driver.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    30775 2024-01-16 23:15:50.000000 pfmongo-0.9.99/pfmongo/env.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.496887 pfmongo-0.9.99/pfmongo/models/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      532 2023-09-26 17:24:31.000000 pfmongo-0.9.99/pfmongo/models/dataModel.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5569 2024-01-12 13:56:52.000000 pfmongo-0.9.99/pfmongo/models/responseModel.py
+-rwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)    24420 2024-01-12 22:37:24.000000 pfmongo-0.9.99/pfmongo/pfmongo.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.492887 pfmongo-0.9.99/pfmongo.egg-info/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     2946 2024-01-18 05:27:30.000000 pfmongo-0.9.99/pfmongo.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1290 2024-01-18 05:27:30.000000 pfmongo-0.9.99/pfmongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2024-01-18 05:27:30.000000 pfmongo-0.9.99/pfmongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       50 2024-01-18 05:27:30.000000 pfmongo-0.9.99/pfmongo.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-09-13 14:02:08.000000 pfmongo-0.9.99/pfmongo.egg-info/not-zip-safe
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      115 2024-01-18 05:27:30.000000 pfmongo-0.9.99/pfmongo.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      156 2024-01-18 05:27:30.000000 pfmongo-0.9.99/pfmongo.egg-info/top_level.txt
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      167 2024-01-18 03:33:37.000000 pfmongo-0.9.99/requirements.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       38 2024-01-18 05:27:30.496887 pfmongo-0.9.99/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     2152 2024-01-18 00:19:38.000000 pfmongo-0.9.99/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2024-01-18 05:27:30.496887 pfmongo-0.9.99/tests/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1650 2023-09-17 17:53:43.000000 pfmongo-0.9.99/tests/test_pfmongo.py
```

### Comparing `pfmongo-0.9.98/LICENSE` & `pfmongo-0.9.99/LICENSE`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/PKG-INFO` & `pfmongo-0.9.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfmongo
-Version: 0.9.98
+Version: 0.9.99
 Summary: A mongodb (portable) "pf" client
 Home-page: https://github.com/FNNDSC/persair
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 License-File: LICENSE
```

### Comparing `pfmongo-0.9.98/README.rst` & `pfmongo-0.9.99/README.rst`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/__main__.py` & `pfmongo-0.9.99/pfmongo/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # (c) 2023+ Fetal-Neonatal Neuroimaging & Developmental Science Center
 #                   Boston Children's Hospital
 #
 #              http://childrenshospital.org/FNNDSC/
 #                        dev@babyMRI.org
 #
 
-__version__ = "0.9.98"
+__version__ = "0.9.99"
 
 import sys
 
 from    pfmongo             import pfmongo
 from    pfmongo             import env
 from    pfmongo.commands    import fs
 from    pfmongo.pfmongo     import parser_setup, parser_interpret, parser_JSONinterpret
```

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/add.py` & `pfmongo-0.9.99/pfmongo/commands/clop/add.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/connect.py` & `pfmongo-0.9.99/pfmongo/commands/clop/connect.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/delete.py` & `pfmongo-0.9.99/pfmongo/commands/clop/delete.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/deleteCol.py` & `pfmongo-0.9.99/pfmongo/commands/clop/deleteCol.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/get.py` & `pfmongo-0.9.99/pfmongo/commands/clop/get.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/list.py` & `pfmongo-0.9.99/pfmongo/commands/clop/list.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/search.py` & `pfmongo-0.9.99/pfmongo/commands/clop/search.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/clop/showAll.py` & `pfmongo-0.9.99/pfmongo/commands/clop/showAll.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/collection.py` & `pfmongo-0.9.99/pfmongo/commands/collection.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/database.py` & `pfmongo-0.9.99/pfmongo/commands/database.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/dbop/connect.py` & `pfmongo-0.9.99/pfmongo/commands/dbop/connect.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/dbop/deleteDB.py` & `pfmongo-0.9.99/pfmongo/commands/dbop/deleteDB.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/dbop/showAll.py` & `pfmongo-0.9.99/pfmongo/commands/dbop/showAll.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/document.py` & `pfmongo-0.9.99/pfmongo/commands/document.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/fop/cd.py` & `pfmongo-0.9.99/pfmongo/commands/fop/cd.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/fop/exp.py` & `pfmongo-0.9.99/pfmongo/commands/fop/exp.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/fop/imp.py` & `pfmongo-0.9.99/pfmongo/commands/fop/imp.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/fop/ls.py` & `pfmongo-0.9.99/pfmongo/commands/fop/ls.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/fop/mkdir.py` & `pfmongo-0.9.99/pfmongo/commands/fop/mkdir.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/fs.py` & `pfmongo-0.9.99/pfmongo/commands/fs.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/man.py` & `pfmongo-0.9.99/pfmongo/commands/man.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/state.py` & `pfmongo-0.9.99/pfmongo/commands/state.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/commands/stateop/showAll.py` & `pfmongo-0.9.99/pfmongo/commands/stateop/showAll.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/config/settings.py` & `pfmongo-0.9.99/pfmongo/config/settings.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/db/pfdb.py` & `pfmongo-0.9.99/pfmongo/db/pfdb.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/driver.py` & `pfmongo-0.9.99/pfmongo/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     return run
 
 def do(
     options:Namespace,
     retType:str,
     f_syncCallBack:Optional[Callable[[MONGO], MONGO]] = None
-) -> int | pfmongo.Pfmongo:
+) -> int | responseModel.mongodbResponse:
     f = event_process(options, f_syncCallBack)
     return f(printResponse = True, returnType = retType)
 
 def run_intReturn(
     options:Namespace,
     f_syncCallBack:Optional[Callable[[MONGO], MONGO]] = None
 ) -> int:
```

### Comparing `pfmongo-0.9.98/pfmongo/env.py` & `pfmongo-0.9.99/pfmongo/env.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/models/dataModel.py` & `pfmongo-0.9.99/pfmongo/models/dataModel.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/models/responseModel.py` & `pfmongo-0.9.99/pfmongo/models/responseModel.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo/pfmongo.py` & `pfmongo-0.9.99/pfmongo/pfmongo.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/pfmongo.egg-info/PKG-INFO` & `pfmongo-0.9.99/pfmongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfmongo
-Version: 0.9.98
+Version: 0.9.99
 Summary: A mongodb (portable) "pf" client
 Home-page: https://github.com/FNNDSC/persair
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 License-File: LICENSE
```

### Comparing `pfmongo-0.9.98/pfmongo.egg-info/SOURCES.txt` & `pfmongo-0.9.99/pfmongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/setup.py` & `pfmongo-0.9.99/setup.py`

 * *Files identical despite different names*

### Comparing `pfmongo-0.9.98/tests/test_pfmongo.py` & `pfmongo-0.9.99/tests/test_pfmongo.py`

 * *Files identical despite different names*

