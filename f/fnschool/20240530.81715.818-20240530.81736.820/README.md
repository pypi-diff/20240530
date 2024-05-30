# Comparing `tmp/fnschool-20240530.81715.818.tar.gz` & `tmp/fnschool-20240530.81736.820.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240530.81715.818.tar", last modified: Thu May 30 09:15:23 2024, max compression
+gzip compressed data, was "fnschool-20240530.81736.820.tar", last modified: Thu May 30 09:36:25 2024, max compression
```

## Comparing `fnschool-20240530.81715.818.tar` & `fnschool-20240530.81736.820.tar`

### file list

```diff
@@ -1,93 +1,91 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.183879 fnschool-20240530.81715.818/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240530.81715.818/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-30 09:15:23.183879 fnschool-20240530.81715.818/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240530.81715.818/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240530.81715.818/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-30 09:15:23.183879 fnschool-20240530.81715.818/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.158845 fnschool-20240530.81715.818/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.165855 fnschool-20240530.81715.818/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      522 2024-05-30 09:15:18.000000 fnschool-20240530.81715.818/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5301 2024-05-29 14:52:26.000000 fnschool-20240530.81715.818/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.173865 fnschool-20240530.81715.818/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-29 14:29:30.000000 fnschool-20240530.81715.818/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240530.81715.818/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)      184 2024-05-29 14:01:36.000000 fnschool-20240530.81715.818/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240530.81715.818/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240530.81715.818/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.174867 fnschool-20240530.81715.818/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255561 2024-05-29 19:10:43.000000 fnschool-20240530.81715.818/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46634 2024-05-29 19:11:20.000000 fnschool-20240530.81715.818/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240530.81715.818/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)      616 2024-05-23 14:19:22.000000 fnschool-20240530.81715.818/src/fnschool/canteen/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240530.81715.818/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240530.81715.818/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81715.818/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81715.818/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3803 2024-05-29 14:28:29.000000 fnschool-20240530.81715.818/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      698 2024-05-30 09:11:40.000000 fnschool-20240530.81715.818/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-29 14:01:50.000000 fnschool-20240530.81715.818/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.178872 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4148 2024-05-29 14:01:50.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10384 2024-05-23 01:03:24.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-29 14:01:50.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9187 2024-05-29 14:53:23.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10136 2024-05-29 15:24:10.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9164 2024-05-29 14:40:36.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    18946 2024-05-30 05:50:14.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-29 14:01:50.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-29 14:01:57.000000 fnschool-20240530.81715.818/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81715.818/src/fnschool/canteen/workbook.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1175 2024-05-29 14:01:37.000000 fnschool-20240530.81715.818/src/fnschool/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.178872 fnschool-20240530.81715.818/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240530.81715.818/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)      624 2024-05-24 05:10:01.000000 fnschool-20240530.81715.818/src/fnschool/entry.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.180875 fnschool-20240530.81715.818/src/fnschool/exam/
--rw-rw-r--   0 larry     (1000) larry     (1000)       78 2024-05-26 16:57:37.000000 fnschool-20240530.81715.818/src/fnschool/exam/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-26 16:57:37.000000 fnschool-20240530.81715.818/src/fnschool/exam/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      614 2024-05-26 15:01:13.000000 fnschool-20240530.81715.818/src/fnschool/exam/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      190 2024-05-26 16:57:37.000000 fnschool-20240530.81715.818/src/fnschool/exam/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      151 2024-05-26 16:57:37.000000 fnschool-20240530.81715.818/src/fnschool/exam/score.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-26 17:04:31.000000 fnschool-20240530.81715.818/src/fnschool/exam/subject.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      258 2024-05-26 17:04:31.000000 fnschool-20240530.81715.818/src/fnschool/exam/teacher.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240530.81715.818/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1883 2024-05-23 14:19:22.000000 fnschool-20240530.81715.818/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.161849 fnschool-20240530.81715.818/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.159846 fnschool-20240530.81715.818/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.181877 fnschool-20240530.81715.818/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-30 09:15:18.000000 fnschool-20240530.81715.818/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.160848 fnschool-20240530.81715.818/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.181877 fnschool-20240530.81715.818/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    19754 2024-05-30 09:15:18.000000 fnschool-20240530.81715.818/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.160848 fnschool-20240530.81715.818/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.181877 fnschool-20240530.81715.818/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 09:15:18.000000 fnschool-20240530.81715.818/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.161849 fnschool-20240530.81715.818/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.182878 fnschool-20240530.81715.818/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 09:15:18.000000 fnschool-20240530.81715.818/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.161849 fnschool-20240530.81715.818/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.182878 fnschool-20240530.81715.818/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 09:15:18.000000 fnschool-20240530.81715.818/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      898 2024-05-24 05:00:49.000000 fnschool-20240530.81715.818/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240530.81715.818/src/fnschool/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5697 2024-05-30 08:51:50.000000 fnschool-20240530.81715.818/src/fnschool/user.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:15:23.182878 fnschool-20240530.81715.818/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-30 09:15:23.000000 fnschool-20240530.81715.818/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2458 2024-05-30 09:15:23.000000 fnschool-20240530.81715.818/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-30 09:15:23.000000 fnschool-20240530.81715.818/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-30 09:15:23.000000 fnschool-20240530.81715.818/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-30 09:15:23.000000 fnschool-20240530.81715.818/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-30 09:15:23.000000 fnschool-20240530.81715.818/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.566717 fnschool-20240530.81736.820/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240530.81736.820/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-30 09:36:25.566717 fnschool-20240530.81736.820/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240530.81736.820/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240530.81736.820/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-30 09:36:25.566717 fnschool-20240530.81736.820/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.540718 fnschool-20240530.81736.820/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.547718 fnschool-20240530.81736.820/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      522 2024-05-30 09:36:20.000000 fnschool-20240530.81736.820/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5301 2024-05-29 14:52:26.000000 fnschool-20240530.81736.820/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.555718 fnschool-20240530.81736.820/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-29 14:29:30.000000 fnschool-20240530.81736.820/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240530.81736.820/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)      184 2024-05-29 14:01:36.000000 fnschool-20240530.81736.820/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240530.81736.820/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240530.81736.820/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.556718 fnschool-20240530.81736.820/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255561 2024-05-29 19:10:43.000000 fnschool-20240530.81736.820/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46634 2024-05-29 19:11:20.000000 fnschool-20240530.81736.820/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240530.81736.820/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)      616 2024-05-23 14:19:22.000000 fnschool-20240530.81736.820/src/fnschool/canteen/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240530.81736.820/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240530.81736.820/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81736.820/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81736.820/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3803 2024-05-29 14:28:29.000000 fnschool-20240530.81736.820/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      698 2024-05-30 09:11:40.000000 fnschool-20240530.81736.820/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-29 14:01:50.000000 fnschool-20240530.81736.820/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.560718 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4148 2024-05-29 14:01:50.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10384 2024-05-23 01:03:24.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-29 14:01:50.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9187 2024-05-29 14:53:23.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10136 2024-05-29 15:24:10.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9164 2024-05-29 14:40:36.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18946 2024-05-30 05:50:14.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-29 14:01:50.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-29 14:01:57.000000 fnschool-20240530.81736.820/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.81736.820/src/fnschool/canteen/workbook.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1175 2024-05-29 14:01:37.000000 fnschool-20240530.81736.820/src/fnschool/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      624 2024-05-24 05:10:01.000000 fnschool-20240530.81736.820/src/fnschool/entry.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.562718 fnschool-20240530.81736.820/src/fnschool/exam/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       78 2024-05-26 16:57:37.000000 fnschool-20240530.81736.820/src/fnschool/exam/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-26 16:57:37.000000 fnschool-20240530.81736.820/src/fnschool/exam/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      614 2024-05-26 15:01:13.000000 fnschool-20240530.81736.820/src/fnschool/exam/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      190 2024-05-26 16:57:37.000000 fnschool-20240530.81736.820/src/fnschool/exam/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      151 2024-05-26 16:57:37.000000 fnschool-20240530.81736.820/src/fnschool/exam/score.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-26 17:04:31.000000 fnschool-20240530.81736.820/src/fnschool/exam/subject.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      258 2024-05-26 17:04:31.000000 fnschool-20240530.81736.820/src/fnschool/exam/teacher.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240530.81736.820/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1883 2024-05-23 14:19:22.000000 fnschool-20240530.81736.820/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.543718 fnschool-20240530.81736.820/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.542718 fnschool-20240530.81736.820/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.563718 fnschool-20240530.81736.820/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-30 09:36:20.000000 fnschool-20240530.81736.820/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.542718 fnschool-20240530.81736.820/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.563718 fnschool-20240530.81736.820/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    19678 2024-05-30 09:36:20.000000 fnschool-20240530.81736.820/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.542718 fnschool-20240530.81736.820/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.563718 fnschool-20240530.81736.820/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 09:36:20.000000 fnschool-20240530.81736.820/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.543718 fnschool-20240530.81736.820/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.564718 fnschool-20240530.81736.820/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 09:36:20.000000 fnschool-20240530.81736.820/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.543718 fnschool-20240530.81736.820/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.564718 fnschool-20240530.81736.820/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-30 09:36:20.000000 fnschool-20240530.81736.820/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      545 2024-05-30 09:28:48.000000 fnschool-20240530.81736.820/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240530.81736.820/src/fnschool/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5697 2024-05-30 08:51:50.000000 fnschool-20240530.81736.820/src/fnschool/user.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-30 09:36:25.565718 fnschool-20240530.81736.820/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-30 09:36:25.000000 fnschool-20240530.81736.820/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2427 2024-05-30 09:36:25.000000 fnschool-20240530.81736.820/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-30 09:36:25.000000 fnschool-20240530.81736.820/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-30 09:36:25.000000 fnschool-20240530.81736.820/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-30 09:36:25.000000 fnschool-20240530.81736.820/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-30 09:36:25.000000 fnschool-20240530.81736.820/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240530.81715.818/LICENSE` & `fnschool-20240530.81736.820/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/PKG-INFO` & `fnschool-20240530.81736.820/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240530.81715.818
+Version: 20240530.81736.820
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240530.81715.818/README.md` & `fnschool-20240530.81736.820/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/pyproject.toml` & `fnschool-20240530.81736.820/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/__init__.py` & `fnschool-20240530.81736.820/src/fnschool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 from fnschool.user import *
 from fnschool.config import *
 
 
-__version__ = "20240530.81715.818"
+__version__ = "20240530.81736.820"
 
 
 # The end.
```

### Comparing `fnschool-20240530.81715.818/src/fnschool/app.py` & `fnschool-20240530.81736.820/src/fnschool/app.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/bill.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/canteen.toml` & `fnschool-20240530.81736.820/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/consuming.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240530.81736.820/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240530.81736.820/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240530.81736.820/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/entry.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/food.cp.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/food.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/food_classes.toml` & `fnschool-20240530.81736.820/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/operator.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/path.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/profile.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/test.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/canteen/workbook.py` & `fnschool-20240530.81736.820/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/config.py` & `fnschool-20240530.81736.820/src/fnschool/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/entry.py` & `fnschool-20240530.81736.820/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/exam/entry.py` & `fnschool-20240530.81736.820/src/fnschool/exam/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/external.py` & `fnschool-20240530.81736.820/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/fnprint.py` & `fnschool-20240530.81736.820/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/language.py` & `fnschool-20240530.81736.820/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240530.81736.820/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-30 17:14+0800\n"
-"PO-Revision-Date: 2024-05-30 16:50+0800\n"
+"POT-Creation-Date: 2024-05-30 17:27+0800\n"
+"PO-Revision-Date: 2024-05-30 17:28+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -69,17 +69,14 @@
 
 msgid "Column \"{0}\" was not found. Exit"
 msgstr "未找到 “{0}” 列。退出。"
 
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
-msgid "Configuration file '%s' was copied to '%s'."
-msgstr "配置文件 “%s” 被复制到 “%s” 。"
-
 msgid "Configurations has been read from \"{0}\"."
 msgstr "应用配置已从 “{0}” 读取。"
 
 msgid "Consuming days of {0}:"
 msgstr "{0} 的出库日期："
 
 msgid "Consuming days:"
@@ -599,14 +596,17 @@
 
 msgid "canteen"
 msgstr "食堂"
 
 msgid "config"
 msgstr "配置"
 
+msgid "data_dir"
+msgstr "数据"
+
 msgid "exam"
 msgstr "测试"
 
 msgid "fnschool"
 msgstr "fnschool"
 
 msgid "food_classes"
```

### Comparing `fnschool-20240530.81715.818/src/fnschool/test.py` & `fnschool-20240530.81736.820/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool/user.py` & `fnschool-20240530.81736.820/src/fnschool/user.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.81715.818/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240530.81736.820/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240530.81715.818
+Version: 20240530.81736.820
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240530.81715.818/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240530.81736.820/src/fnschool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 src/fnschool/canteen/spreadsheet/inventory.py
 src/fnschool/canteen/spreadsheet/preconsuming.py
 src/fnschool/canteen/spreadsheet/purchasing.py
 src/fnschool/canteen/spreadsheet/purchasingsum.py
 src/fnschool/canteen/spreadsheet/unwarehousing.py
 src/fnschool/canteen/spreadsheet/unwarehousingsum.py
 src/fnschool/canteen/spreadsheet/warehousing.py
-src/fnschool/data/config0.toml
 src/fnschool/exam/__init__.py
 src/fnschool/exam/__main__.py
 src/fnschool/exam/entry.py
 src/fnschool/exam/path.py
 src/fnschool/exam/score.py
 src/fnschool/exam/subject.py
 src/fnschool/exam/teacher.py
```

