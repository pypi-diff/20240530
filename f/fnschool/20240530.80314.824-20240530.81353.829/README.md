# Comparing `tmp/fnschool-20240530.80314.824.tar.gz` & `tmp/fnschool-20240530.81353.829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240530.80314.824.tar", last modified: Wed May 29 19:14:28 2024, max compression
+gzip compressed data, was "fnschool-20240530.81353.829.tar", last modified: Thu May 30 05:53:35 2024, max compression
```

## Comparing `fnschool-20240530.80314.824.tar` & `fnschool-20240530.81353.829.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.959382 fnschool-20240530.80314.824/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240530.80314.824/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-29 19:14:28.959382 fnschool-20240530.80314.824/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240530.80314.824/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240530.80314.824/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-29 19:14:28.959382 fnschool-20240530.80314.824/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.932381 fnschool-20240530.80314.824/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.939381 fnschool-20240530.80314.824/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      522 2024-05-29 19:14:24.000000 fnschool-20240530.80314.824/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5301 2024-05-29 14:52:26.000000 fnschool-20240530.80314.824/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.948382 fnschool-20240530.80314.824/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-29 14:29:30.000000 fnschool-20240530.80314.824/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240530.80314.824/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)      184 2024-05-29 14:01:36.000000 fnschool-20240530.80314.824/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240530.80314.824/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240530.80314.824/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.950382 fnschool-20240530.80314.824/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255561 2024-05-29 19:10:43.000000 fnschool-20240530.80314.824/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46634 2024-05-29 19:11:20.000000 fnschool-20240530.80314.824/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240530.80314.824/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)      616 2024-05-23 14:19:22.000000 fnschool-20240530.80314.824/src/fnschool/canteen/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240530.80314.824/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240530.80314.824/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80314.824/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80314.824/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3803 2024-05-29 14:28:29.000000 fnschool-20240530.80314.824/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      601 2024-05-29 13:55:44.000000 fnschool-20240530.80314.824/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-29 14:01:50.000000 fnschool-20240530.80314.824/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.954382 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4148 2024-05-29 14:01:50.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10384 2024-05-23 01:03:24.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-29 14:01:50.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9187 2024-05-29 14:53:23.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10136 2024-05-29 15:24:10.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9164 2024-05-29 14:40:36.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    18745 2024-05-29 14:28:30.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-29 14:01:50.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-29 14:01:57.000000 fnschool-20240530.80314.824/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80314.824/src/fnschool/canteen/workbook.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1175 2024-05-29 14:01:37.000000 fnschool-20240530.80314.824/src/fnschool/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.954382 fnschool-20240530.80314.824/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240530.80314.824/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)      624 2024-05-24 05:10:01.000000 fnschool-20240530.80314.824/src/fnschool/entry.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.956382 fnschool-20240530.80314.824/src/fnschool/exam/
--rw-rw-r--   0 larry     (1000) larry     (1000)       78 2024-05-26 16:57:37.000000 fnschool-20240530.80314.824/src/fnschool/exam/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-26 16:57:37.000000 fnschool-20240530.80314.824/src/fnschool/exam/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      614 2024-05-26 15:01:13.000000 fnschool-20240530.80314.824/src/fnschool/exam/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      190 2024-05-26 16:57:37.000000 fnschool-20240530.80314.824/src/fnschool/exam/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      151 2024-05-26 16:57:37.000000 fnschool-20240530.80314.824/src/fnschool/exam/score.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-26 17:04:31.000000 fnschool-20240530.80314.824/src/fnschool/exam/subject.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      258 2024-05-26 17:04:31.000000 fnschool-20240530.80314.824/src/fnschool/exam/teacher.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240530.80314.824/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1883 2024-05-23 14:19:22.000000 fnschool-20240530.80314.824/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.935382 fnschool-20240530.80314.824/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.934382 fnschool-20240530.80314.824/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.956382 fnschool-20240530.80314.824/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-29 19:14:24.000000 fnschool-20240530.80314.824/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.934382 fnschool-20240530.80314.824/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.957382 fnschool-20240530.80314.824/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    19661 2024-05-29 19:14:24.000000 fnschool-20240530.80314.824/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.935382 fnschool-20240530.80314.824/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.957382 fnschool-20240530.80314.824/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 19:14:24.000000 fnschool-20240530.80314.824/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.935382 fnschool-20240530.80314.824/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.957382 fnschool-20240530.80314.824/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 19:14:24.000000 fnschool-20240530.80314.824/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.935382 fnschool-20240530.80314.824/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.957382 fnschool-20240530.80314.824/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 19:14:24.000000 fnschool-20240530.80314.824/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      898 2024-05-24 05:00:49.000000 fnschool-20240530.80314.824/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240530.80314.824/src/fnschool/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5545 2024-05-29 19:13:39.000000 fnschool-20240530.80314.824/src/fnschool/user.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 19:14:28.958382 fnschool-20240530.80314.824/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-29 19:14:28.000000 fnschool-20240530.80314.824/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2458 2024-05-29 19:14:28.000000 fnschool-20240530.80314.824/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-29 19:14:28.000000 fnschool-20240530.80314.824/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-29 19:14:28.000000 fnschool-20240530.80314.824/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-29 19:14:28.000000 fnschool-20240530.80314.824/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-29 19:14:28.000000 fnschool-20240530.80314.824/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.137144 fnschool-20240530.81353.829/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240530.81353.829/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-30 05:53:35.136144 fnschool-20240530.81353.829/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240530.81353.829/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240530.81353.829/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-30 05:53:35.137144 fnschool-20240530.81353.829/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.099145 fnschool-20240530.81353.829/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.107145 fnschool-20240530.81353.829/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      522 2024-05-30 05:53:29.000000 fnschool-20240530.81353.829/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5301 2024-05-29 14:52:26.000000 fnschool-20240530.81353.829/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.116145 fnschool-20240530.81353.829/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-29 14:29:30.000000 fnschool-20240530.81353.829/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240530.81353.829/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)      184 2024-05-29 14:01:36.000000 fnschool-20240530.81353.829/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240530.81353.829/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240530.81353.829/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.123144 fnschool-20240530.81353.829/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255561 2024-05-29 19:10:43.000000 fnschool-20240530.81353.829/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46634 2024-05-29 19:11:20.000000 fnschool-20240530.81353.829/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240530.81353.829/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)      616 2024-05-23 14:19:22.000000 fnschool-20240530.81353.829/src/fnschool/canteen/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240530.81353.829/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240530.81353.829/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81353.829/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81353.829/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3803 2024-05-29 14:28:29.000000 fnschool-20240530.81353.829/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      601 2024-05-29 13:55:44.000000 fnschool-20240530.81353.829/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-29 14:01:50.000000 fnschool-20240530.81353.829/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.128144 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4148 2024-05-29 14:01:50.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10384 2024-05-23 01:03:24.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-29 14:01:50.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9187 2024-05-29 14:53:23.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10136 2024-05-29 15:24:10.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9164 2024-05-29 14:40:36.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18946 2024-05-30 05:50:14.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-29 14:01:50.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-29 14:01:57.000000 fnschool-20240530.81353.829/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81353.829/src/fnschool/canteen/workbook.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1175 2024-05-29 14:01:37.000000 fnschool-20240530.81353.829/src/fnschool/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.128144 fnschool-20240530.81353.829/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240530.81353.829/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)      624 2024-05-24 05:10:01.000000 fnschool-20240530.81353.829/src/fnschool/entry.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.133144 fnschool-20240530.81353.829/src/fnschool/exam/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       78 2024-05-26 16:57:37.000000 fnschool-20240530.81353.829/src/fnschool/exam/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-26 16:57:37.000000 fnschool-20240530.81353.829/src/fnschool/exam/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      614 2024-05-26 15:01:13.000000 fnschool-20240530.81353.829/src/fnschool/exam/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      190 2024-05-26 16:57:37.000000 fnschool-20240530.81353.829/src/fnschool/exam/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      151 2024-05-26 16:57:37.000000 fnschool-20240530.81353.829/src/fnschool/exam/score.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-26 17:04:31.000000 fnschool-20240530.81353.829/src/fnschool/exam/subject.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      258 2024-05-26 17:04:31.000000 fnschool-20240530.81353.829/src/fnschool/exam/teacher.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240530.81353.829/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1883 2024-05-23 14:19:22.000000 fnschool-20240530.81353.829/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.102145 fnschool-20240530.81353.829/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.101145 fnschool-20240530.81353.829/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.133144 fnschool-20240530.81353.829/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-30 05:53:29.000000 fnschool-20240530.81353.829/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.101145 fnschool-20240530.81353.829/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.134144 fnschool-20240530.81353.829/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    19658 2024-05-30 05:53:29.000000 fnschool-20240530.81353.829/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.102145 fnschool-20240530.81353.829/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.134144 fnschool-20240530.81353.829/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 05:53:29.000000 fnschool-20240530.81353.829/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.102145 fnschool-20240530.81353.829/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.135144 fnschool-20240530.81353.829/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 05:53:29.000000 fnschool-20240530.81353.829/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.102145 fnschool-20240530.81353.829/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.135144 fnschool-20240530.81353.829/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 05:53:29.000000 fnschool-20240530.81353.829/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      898 2024-05-24 05:00:49.000000 fnschool-20240530.81353.829/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240530.81353.829/src/fnschool/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5545 2024-05-29 19:13:39.000000 fnschool-20240530.81353.829/src/fnschool/user.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 05:53:35.136144 fnschool-20240530.81353.829/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-30 05:53:35.000000 fnschool-20240530.81353.829/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2458 2024-05-30 05:53:35.000000 fnschool-20240530.81353.829/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-30 05:53:35.000000 fnschool-20240530.81353.829/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-30 05:53:35.000000 fnschool-20240530.81353.829/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-30 05:53:35.000000 fnschool-20240530.81353.829/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-30 05:53:35.000000 fnschool-20240530.81353.829/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240530.80314.824/LICENSE` & `fnschool-20240530.81353.829/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/PKG-INFO` & `fnschool-20240530.81353.829/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240530.80314.824
+Version: 20240530.81353.829
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240530.80314.824/README.md` & `fnschool-20240530.81353.829/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/pyproject.toml` & `fnschool-20240530.81353.829/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/__init__.py` & `fnschool-20240530.81353.829/src/fnschool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 from fnschool.user import *
 from fnschool.config import *
 
 
-__version__ = "20240530.80314.824"
+__version__ = "20240530.81353.829"
 
 
 # The end.
```

### Comparing `fnschool-20240530.80314.824/src/fnschool/app.py` & `fnschool-20240530.81353.829/src/fnschool/app.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/bill.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/canteen.toml` & `fnschool-20240530.81353.829/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/consuming.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240530.81353.829/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240530.81353.829/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240530.81353.829/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/entry.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/food.cp.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/food.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/food_classes.toml` & `fnschool-20240530.81353.829/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/operator.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/path.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/profile.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,24 @@
 
     def get_col(self, col):
         if not col[1]:
             col0 = [
                 (n, self.headers.index(n) + 1)
                 for n in self.headers
                 if n in col[2]
-            ][-1]
+            ]
+            if len(col0) < 1:
+                print_error(
+                    _('Column "{0}" was not found. Exit').format(col[2][0])
+                )
+                exit()
+            col0 = col0[-1]
             col[0] = col0[0]
             col[1] = col0[1]
+
         return col
 
     @property
     def col_indexes(self):
         indexes = [c[1] for c in self.cols]
         indexes = sorted(indexes)
         return indexes
```

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/test.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/canteen/workbook.py` & `fnschool-20240530.81353.829/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/config.py` & `fnschool-20240530.81353.829/src/fnschool/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/entry.py` & `fnschool-20240530.81353.829/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/exam/entry.py` & `fnschool-20240530.81353.829/src/fnschool/exam/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/external.py` & `fnschool-20240530.81353.829/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/fnprint.py` & `fnschool-20240530.81353.829/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/language.py` & `fnschool-20240530.81353.829/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240530.81353.829/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-30 03:12+0800\n"
-"PO-Revision-Date: 2024-05-30 02:54+0800\n"
+"POT-Creation-Date: 2024-05-30 13:50+0800\n"
+"PO-Revision-Date: 2024-05-30 13:50+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -63,14 +63,17 @@
 msgstr "工作表 “{0}” 的所有单元格被取消合并。"
 
 msgid ""
 "Column \"{0}\" has been updated, feel free to open new issue if some food "
 "with the wrong class ({1}). "
 msgstr "“{0}”列已添加，如果食材的大类名有错误，还请您随时提交反馈（{1}）。"
 
+msgid "Column \"{0}\" was not found. Exit"
+msgstr "未找到 “{0}” 列。退出。"
+
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
 msgid "Configuration file '%s' was copied to '%s'."
 msgstr "配置文件 “%s” 被复制到 “%s” 。"
 
 msgid "Configurations has been read from \"{0}\"."
@@ -575,17 +578,14 @@
 "for next updating."
 msgstr ""
 "您可以把 食材台账表 里面没有更新的月份的数据更新了，这些数据会被保存下来的。"
 
 msgid "Your food classes were read from \"{0}\". It will be used first."
 msgstr "您的食材大类已从 “{0}”  读取。它会被优先匹配。"
 
-msgid "Your name has been saved to \"{0}\""
-msgstr "您的名字被保存到 “{0}”。"
-
 msgid "Your name has been saved to \"{0}\"."
 msgstr "您的名字被保存到 “{0}”。"
 
 msgid "app_config"
 msgstr "应用配置"
 
 msgid "bill"
```

### Comparing `fnschool-20240530.80314.824/src/fnschool/path.py` & `fnschool-20240530.81353.829/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/test.py` & `fnschool-20240530.81353.829/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool/user.py` & `fnschool-20240530.81353.829/src/fnschool/user.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80314.824/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240530.81353.829/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240530.80314.824
+Version: 20240530.81353.829
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240530.80314.824/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240530.81353.829/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

