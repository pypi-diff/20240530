# Comparing `tmp/mds_cashbook-7.0.33.tar.gz` & `tmp/mds_cashbook-7.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook-7.0.33.tar", last modified: Sun Dec 31 09:20:51 2023, max compression
+gzip compressed data, was "mds_cashbook-7.0.34.tar", last modified: Thu May 30 10:58:25 2024, max compression
```

## Comparing `mds_cashbook-7.0.33.tar` & `mds_cashbook-7.0.34.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.114187 mds_cashbook-7.0.33/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7868 2023-12-31 09:20:51.114187 mds_cashbook-7.0.33/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5385 2023-12-31 09:19:33.000000 mds_cashbook-7.0.33/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1500 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    23181 2023-12-31 09:18:00.000000 mds_cashbook-7.0.33/book.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    25770 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/book.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5335 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/category.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/category.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/cbreport.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/cbreport.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6924 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/configuration.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/configuration.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      225 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/const.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      500 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/cron.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      501 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/cron.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1866 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/currency.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.070186 mds_cashbook-7.0.33/docs/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/docs/settings.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/group.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.070186 mds_cashbook-7.0.33/icon/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/icon/notebook1.svg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/icon.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1045 2023-12-31 09:16:55.000000 mds_cashbook-7.0.33/ir.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    43435 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/line.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    13058 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.070186 mds_cashbook-7.0.33/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    46386 2023-12-31 09:17:33.000000 mds_cashbook-7.0.33/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    43568 2023-12-31 09:17:33.000000 mds_cashbook-7.0.33/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.114187 mds_cashbook-7.0.33/mds_cashbook.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7868 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1681 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-12-31 09:20:50.000000 mds_cashbook-7.0.33/mds_cashbook.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8068 2023-12-31 09:17:33.000000 mds_cashbook-7.0.33/message.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7164 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/mixin.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     4392 2023-12-31 09:17:11.000000 mds_cashbook-7.0.33/model.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    18283 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/reconciliation.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     9672 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/reconciliation.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.074186 mds_cashbook-7.0.33/report/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/report/cashbook.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/report/reconciliation.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-12-31 09:20:51.114187 mds_cashbook-7.0.33/setup.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3830 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11193 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/splitline.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6066 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/splitline.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.090186 mds_cashbook-7.0.33/tests/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      203 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    25017 2023-12-31 09:17:33.000000 mds_cashbook-7.0.33/tests/book.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6777 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/bookingwiz.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     8328 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/category.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6679 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/config.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    74665 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/tests/line.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    32358 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/reconciliation.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    16431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/splitline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      970 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/tests/test_module.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1551 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/tests/type.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    33651 2023-12-31 09:17:50.000000 mds_cashbook-7.0.33/tests/valuestore.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      359 2023-12-31 09:19:39.000000 mds_cashbook-7.0.33/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2128 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/types.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/types.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6867 2023-12-31 09:17:23.000000 mds_cashbook-7.0.33/valuestore.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-12-31 09:20:51.110187 mds_cashbook-7.0.33/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/book_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      503 2023-12-31 09:17:41.000000 mds_cashbook-7.0.33/view/book_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      598 2023-12-31 09:17:41.000000 mds_cashbook-7.0.33/view/book_tree.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/cashbook_line_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/category_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/category_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/category_tree.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      999 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/configuration_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1048 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/enterbooking_start_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/line_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      639 2023-12-06 19:43:08.000000 mds_cashbook-7.0.33/view/line_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      650 2023-12-06 19:43:08.000000 mds_cashbook-7.0.33/view/line_recon_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/recon_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      538 2023-12-06 19:43:08.000000 mds_cashbook-7.0.33/view/recon_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/split_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      612 2023-12-06 19:43:08.000000 mds_cashbook-7.0.33/view/split_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/type_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/type_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/wizard_openline_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/view/wizard_runrepbook_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6908 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/wizard_booking.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/wizard_booking.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/wizard_openline.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/wizard_openline.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4613 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/wizard_runreport.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-12-01 19:18:18.000000 mds_cashbook-7.0.33/wizard_runreport.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7969 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     5454 2024-05-30 10:58:02.000000 mds_cashbook-7.0.34/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1500 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    23181 2024-01-03 20:03:30.000000 mds_cashbook-7.0.34/book.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    25770 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/book.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     5335 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/category.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/cbreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/cbreport.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6924 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/configuration.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/configuration.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      225 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/const.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      500 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/cron.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      501 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/cron.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1866 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/currency.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.563778 mds_cashbook-7.0.34/docs/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/docs/settings.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/group.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.563778 mds_cashbook-7.0.34/icon/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/icon/notebook1.svg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/icon.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1045 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/ir.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    43435 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/line.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    13058 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.567778 mds_cashbook-7.0.34/locale/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    46721 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/locale/de.po
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    43888 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/mds_cashbook.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7969 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1681 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     8068 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/message.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7164 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/mixin.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     4392 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/model.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    18283 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/reconciliation.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     9672 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/reconciliation.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.567778 mds_cashbook-7.0.34/report/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/report/cashbook.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/report/reconciliation.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3830 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/setup.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11193 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/splitline.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6066 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/splitline.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.575778 mds_cashbook-7.0.34/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      203 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    25017 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/book.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7013 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/tests/bookingwiz.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     8328 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6679 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/config.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    74665 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    32358 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/reconciliation.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    16431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/splitline.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      970 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/test_module.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1551 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/type.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    33651 2024-05-30 10:58:02.000000 mds_cashbook-7.0.34/tests/valuestore.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      359 2024-05-30 10:58:02.000000 mds_cashbook-7.0.34/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2128 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/types.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/types.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7138 2024-05-30 10:52:27.000000 mds_cashbook-7.0.34/valuestore.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.579778 mds_cashbook-7.0.34/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/book_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      503 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/book_list.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      598 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/book_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/cashbook_line_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/category_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/category_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/category_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      999 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/configuration_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1170 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/view/enterbooking_start_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/line_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      639 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/line_list.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      650 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/line_recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/recon_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      538 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/split_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      612 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/split_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/type_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/type_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/wizard_openline_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/wizard_runrepbook_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7324 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/wizard_booking.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_booking.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_openline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_openline.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4613 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_runreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_runreport.xml
```

### Comparing `mds_cashbook-7.0.33/PKG-INFO` & `mds_cashbook-7.0.34/mds_cashbook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mds_cashbook
-Version: 7.0.33
+Name: mds-cashbook
+Version: 7.0.34
 Summary: Tryton module to add a cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook
 Description: mds-cashbook
@@ -158,14 +158,18 @@
         If you have hierarchical cash books, the amounts of subordinate cash books with foreign
         currency are converted  into the display currency of the parent cash book.
         
         
         Changes
         =======
         
+        *7.0.34 - 30.05.2024*
+        
+        - add: fixate of booking from booking-wizard
+        
         *7.0.33 - 31.12.2023*
         
         - remove caching
         - add worker-based precalculation of cashbook-values
         
         *7.0.32 - 06.12.2023*
```

### Comparing `mds_cashbook-7.0.33/README.rst` & `mds_cashbook-7.0.34/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -149,14 +149,18 @@
 If you have hierarchical cash books, the amounts of subordinate cash books with foreign
 currency are converted  into the display currency of the parent cash book.
 
 
 Changes
 =======
 
+*7.0.34 - 30.05.2024*
+
+- add: fixate of booking from booking-wizard
+
 *7.0.33 - 31.12.2023*
 
 - remove caching
 - add worker-based precalculation of cashbook-values
 
 *7.0.32 - 06.12.2023*
```

### Comparing `mds_cashbook-7.0.33/__init__.py` & `mds_cashbook-7.0.34/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/book.py` & `mds_cashbook-7.0.34/book.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/book.xml` & `mds_cashbook-7.0.34/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/category.py` & `mds_cashbook-7.0.34/category.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/category.xml` & `mds_cashbook-7.0.34/category.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/cbreport.py` & `mds_cashbook-7.0.34/cbreport.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/cbreport.xml` & `mds_cashbook-7.0.34/cbreport.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/configuration.py` & `mds_cashbook-7.0.34/configuration.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/configuration.xml` & `mds_cashbook-7.0.34/configuration.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/currency.py` & `mds_cashbook-7.0.34/currency.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/group.xml` & `mds_cashbook-7.0.34/group.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/icon/notebook1.svg` & `mds_cashbook-7.0.34/icon/notebook1.svg`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/ir.py` & `mds_cashbook-7.0.34/ir.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/line.py` & `mds_cashbook-7.0.34/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/line.xml` & `mds_cashbook-7.0.34/line.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/locale/de.po` & `mds_cashbook-7.0.34/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -1642,14 +1642,26 @@
 msgid "Source/Dest"
 msgstr "Quelle/Ziel"
 
 msgctxt "field:cashbook.enterbooking.start,party:"
 msgid "Party"
 msgstr "Partei"
 
+msgctxt "field:cashbook.enterbooking.start,description:"
+msgid "Description"
+msgstr "Beschreibung"
+
+msgctxt "field:cashbook.enterbooking.start,fixate:"
+msgid "Fixate"
+msgstr "Festschreiben"
+
+msgctxt "help:cashbook.enterbooking.start,fixate:"
+msgid "The booking is fixed immediately."
+msgstr "Die Buchung wird sofort festgeschrieben."
+
 
 #########################
 # cashbook.enterbooking #
 #########################
 msgctxt "model:cashbook.enterbooking,name:"
 msgid "Enter Booking"
 msgstr "Buchung eingeben"
```

### Comparing `mds_cashbook-7.0.33/locale/en.po` & `mds_cashbook-7.0.34/locale/en.po`

 * *Files 0% similar despite different names*

```diff
@@ -1550,14 +1550,26 @@
 msgid "Source/Dest"
 msgstr "Source/Dest"
 
 msgctxt "field:cashbook.enterbooking.start,party:"
 msgid "Party"
 msgstr "Party"
 
+msgctxt "field:cashbook.enterbooking.start,description:"
+msgid "Description"
+msgstr "Description"
+
+msgctxt "field:cashbook.enterbooking.start,fixate:"
+msgid "Fixate"
+msgstr "Fixate"
+
+msgctxt "help:cashbook.enterbooking.start,fixate:"
+msgid "The booking is fixed immediately."
+msgstr "The booking is fixed immediately."
+
 msgctxt "model:cashbook.enterbooking,name:"
 msgid "Enter Booking"
 msgstr "Enter Booking"
 
 msgctxt "wizard_button:cashbook.enterbooking,start,end:"
 msgid "Cancel"
 msgstr "Cancel"
```

### Comparing `mds_cashbook-7.0.33/mds_cashbook.egg-info/PKG-INFO` & `mds_cashbook-7.0.34/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mds-cashbook
-Version: 7.0.33
+Name: mds_cashbook
+Version: 7.0.34
 Summary: Tryton module to add a cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook
 Description: mds-cashbook
@@ -158,14 +158,18 @@
         If you have hierarchical cash books, the amounts of subordinate cash books with foreign
         currency are converted  into the display currency of the parent cash book.
         
         
         Changes
         =======
         
+        *7.0.34 - 30.05.2024*
+        
+        - add: fixate of booking from booking-wizard
+        
         *7.0.33 - 31.12.2023*
         
         - remove caching
         - add worker-based precalculation of cashbook-values
         
         *7.0.32 - 06.12.2023*
```

### Comparing `mds_cashbook-7.0.33/mds_cashbook.egg-info/SOURCES.txt` & `mds_cashbook-7.0.34/mds_cashbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/menu.xml` & `mds_cashbook-7.0.34/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/message.xml` & `mds_cashbook-7.0.34/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/mixin.py` & `mds_cashbook-7.0.34/mixin.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/model.py` & `mds_cashbook-7.0.34/model.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/reconciliation.py` & `mds_cashbook-7.0.34/reconciliation.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/reconciliation.xml` & `mds_cashbook-7.0.34/reconciliation.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/report/cashbook.fods` & `mds_cashbook-7.0.34/report/cashbook.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/report/reconciliation.fods` & `mds_cashbook-7.0.34/report/reconciliation.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/setup.py` & `mds_cashbook-7.0.34/setup.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/splitline.py` & `mds_cashbook-7.0.34/splitline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/splitline.xml` & `mds_cashbook-7.0.34/splitline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/book.py` & `mds_cashbook-7.0.34/tests/book.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/bookingwiz.py` & `mds_cashbook-7.0.34/tests/bookingwiz.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,37 +61,39 @@
             self.assertEqual(result['view']['defaults']['bookingtype'], 'out')
             self.assertEqual(result['view']['defaults']['cashbook'], None)
             self.assertEqual(result['view']['defaults']['amount'], None)
             self.assertEqual(result['view']['defaults']['party'], None)
             self.assertEqual(result['view']['defaults']['booktransf'], None)
             self.assertEqual(result['view']['defaults']['description'], None)
             self.assertEqual(result['view']['defaults']['category'], None)
+            self.assertEqual(result['view']['defaults']['fixate'], False)
 
             self.assertEqual(len(book.lines), 0)
 
             r1 = {
                 'amount': Decimal('10.0'),
                 'cashbook': book.id,
                 'party': party.id,
                 'description': 'Test 1',
                 'category': categories[1].id,
                 'bookingtype': 'out',
-                }
+                'fixate': True}
             for x in r1.keys():
                 setattr(w_obj.start, x, r1[x])
 
             IrDate.today = MagicMock(return_value=date(2022, 5, 1))
             result = BookingWiz.execute(sess_id, {'start': r1}, 'save_')
             BookingWiz.delete(sess_id)
             IrDate.today = MagicMock(return_value=date.today())
 
             self.assertEqual(len(book.lines), 1)
             self.assertEqual(
                 book.lines[0].rec_name,
                 '05/01/2022|Exp|-10.00 usd|Test 1 [Food]')
+            self.assertEqual(book.lines[0].state, 'check')
 
     @with_transaction()
     def test_bookwiz_transfer(self):
         """ run booking-wizard to store expense
         """
         pool = Pool()
         BookingWiz = pool.get('cashbook.enterbooking', type='wizard')
@@ -143,25 +145,26 @@
             self.assertEqual(result['view']['defaults']['bookingtype'], 'out')
             self.assertEqual(result['view']['defaults']['cashbook'], None)
             self.assertEqual(result['view']['defaults']['amount'], None)
             self.assertEqual(result['view']['defaults']['party'], None)
             self.assertEqual(result['view']['defaults']['booktransf'], None)
             self.assertEqual(result['view']['defaults']['description'], None)
             self.assertEqual(result['view']['defaults']['category'], None)
+            self.assertEqual(result['view']['defaults']['fixate'], False)
 
             self.assertEqual(len(books[0].lines), 0)
             self.assertEqual(len(books[1].lines), 0)
 
             r1 = {
                 'amount': Decimal('10.0'),
                 'cashbook': books[0].id,
                 'description': 'Test 1',
                 'booktransf': books[1].id,
                 'bookingtype': 'mvout',
-                }
+                'fixate': False}
             for x in r1.keys():
                 setattr(w_obj.start, x, r1[x])
 
             IrDate.today = MagicMock(return_value=date(2022, 5, 1))
             result = BookingWiz.execute(sess_id, {'start': r1}, 'save_')
             BookingWiz.delete(sess_id)
             IrDate.today = MagicMock(return_value=date.today())
```

### Comparing `mds_cashbook-7.0.33/tests/category.py` & `mds_cashbook-7.0.34/tests/category.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/config.py` & `mds_cashbook-7.0.34/tests/config.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/line.py` & `mds_cashbook-7.0.34/tests/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/reconciliation.py` & `mds_cashbook-7.0.34/tests/reconciliation.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/splitline.py` & `mds_cashbook-7.0.34/tests/splitline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/test_module.py` & `mds_cashbook-7.0.34/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/type.py` & `mds_cashbook-7.0.34/tests/type.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/tests/valuestore.py` & `mds_cashbook-7.0.34/tests/valuestore.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/types.py` & `mds_cashbook-7.0.34/types.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/types.xml` & `mds_cashbook-7.0.34/types.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/valuestore.py` & `mds_cashbook-7.0.34/valuestore.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         string='Value', digits=(16, Eval('valuedigits', 6)),
         depends=['valuedigits'])
     valuedigits = fields.Function(fields.Integer(
         string='Digits', readonly=True),
         'on_change_with_valuedigits')
 
     @classmethod
+    def __register__(cls, module_name):
+        super(ValueStore, cls).__register__(module_name)
+
+        # clear value-store, re-calc
+        records = cls.search([])
+        if records:
+            cls.delete(records)
+        cls.maintenance_values()
+
+    @classmethod
     def __setup__(cls):
         super(ValueStore, cls).__setup__()
         t = cls.__table__()
         cls._sql_constraints.extend([
             ('uniqu_field',
                 Unique(t, t.cashbook, t.field_name),
                 'cashbook.msg_value_exists_in_store'),
```

### Comparing `mds_cashbook-7.0.33/view/book_form.xml` & `mds_cashbook-7.0.34/view/book_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/book_tree.xml` & `mds_cashbook-7.0.34/view/book_tree.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/category_form.xml` & `mds_cashbook-7.0.34/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/configuration_form.xml` & `mds_cashbook-7.0.34/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/enterbooking_start_form.xml` & `mds_cashbook-7.0.34/view/enterbooking_start_form.xml`

 * *Files 7% similar despite different names*

#### Comparing `mds_cashbook-7.0.33/view/enterbooking_start_form.xml` & `mds_cashbook-7.0.34/view/enterbooking_start_form.xml`

```diff
@@ -17,13 +17,17 @@
       <field name="booktransf"/>
       <label name="party"/>
       <field name="party"/>
     </page>
     <page id="descr" string="Description" col="1">
       <field name="description"/>
     </page>
+    <page name="fixate" col="2">
+      <label name="fixate"/>
+      <field name="fixate"/>
+    </page>
   </notebook>
   <field name="cashbooks"/>
   <field name="currency_digits"/>
   <field name="currency"/>
   <field name="owner_cashbook"/>
 </form>
```

### Comparing `mds_cashbook-7.0.33/view/line_form.xml` & `mds_cashbook-7.0.34/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/line_list.xml` & `mds_cashbook-7.0.34/view/line_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/line_recon_list.xml` & `mds_cashbook-7.0.34/view/line_recon_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/recon_form.xml` & `mds_cashbook-7.0.34/view/recon_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/recon_list.xml` & `mds_cashbook-7.0.34/view/recon_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/split_form.xml` & `mds_cashbook-7.0.34/view/split_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/split_list.xml` & `mds_cashbook-7.0.34/view/split_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/wizard_openline_form.xml` & `mds_cashbook-7.0.34/view/wizard_openline_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/view/wizard_runrepbook_form.xml` & `mds_cashbook-7.0.34/view/wizard_runrepbook_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/wizard_booking.py` & `mds_cashbook-7.0.34/wizard_booking.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import ModelView, fields
 from trytond.wizard import Wizard, StateView, StateTransition, Button
 from trytond.pool import Pool
 from trytond.transaction import Transaction
-from trytond.pyson import Eval, Bool, If
+from trytond.pyson import Eval, Bool, If, And
 from decimal import Decimal
 from .line import sel_bookingtype
 
 sel_booktypewiz = [x for x in sel_bookingtype if not x[0] in ['spin', 'spout']]
 
 
 class EnterBookingStart(ModelView):
@@ -41,29 +41,33 @@
     bookingtype = fields.Selection(
         string='Type', required=True, selection=sel_booktypewiz)
     amount = fields.Numeric(
         string='Amount',
         depends=['currency_digits', 'bookingtype'],
         digits=(16, Eval('currency_digits', 2)), required=True,
         domain=[('amount', '>=', Decimal('0.0'))])
-    description = fields.Text(string='Description')
+    description = fields.Text(
+        string='Description', states={'required': Bool(Eval('fixate'))},
+        depends=['fixate'])
     category = fields.Many2One(
         string='Category',
         model_name='cashbook.category', depends=['bookingtype'],
         states={
             'readonly': ~Bool(Eval('bookingtype')),
             'required': Eval('bookingtype', '').in_(['in', 'out']),
             'invisible': ~Eval('bookingtype', '').in_(['in', 'out']),
         },
         domain=[
             If(
                 Eval('bookingtype', '').in_(['in', 'mvin']),
                 ('cattype', '=', 'in'),
                 ('cattype', '=', 'out'),
             )])
+    fixate = fields.Boolean(
+        string='Fixate', help='The booking is fixed immediately.')
 
     # party or cashbook as counterpart
     booktransf = fields.Many2One(
         string='Source/Dest',
         model_name='cashbook.book',
         domain=[
             ('owner.id', '=', Eval('owner_cashbook', -1)),
@@ -73,15 +77,18 @@
             'invisible': ~Eval('bookingtype', '').in_(['mvin', 'mvout']),
             'required': Eval('bookingtype', '').in_(['mvin', 'mvout']),
         }, depends=['bookingtype', 'owner_cashbook', 'cashbook'])
     party = fields.Many2One(
         string='Party', model_name='party.party',
         states={
             'invisible': ~Eval('bookingtype', '').in_(['in', 'out']),
-        }, depends=['bookingtype'])
+            'required': And(
+                Bool(Eval('fixate')),
+                Eval('bookingtype', '').in_(['in', 'out']))},
+        depends=['bookingtype', 'fixate'])
 
     @fields.depends('bookingtype', 'category')
     def on_change_bookingtype(self):
         """ clear category if not valid type
         """
         types = {
             'in': ['in', 'mvin'],
@@ -146,14 +153,15 @@
 
         book_ids = []
         for x in ['defbook', 'book1', 'book2', 'book3', 'book4', 'book5']:
             if getattr(cfg1, x, None) is not None:
                 book_ids.append(getattr(cfg1, x, None).id)
 
         result = {
+            'fixate': False,
             'cashbooks': [x.id for x in Cashbook.search([
                     ('state', '=', 'open'),
                     ('btype', '!=', None),
                     ('owner', '=', Transaction().user),
                     ('id', 'in', book_ids),
                 ])],
             'bookingtype': getattr(self.start, 'bookingtype', 'out'),
@@ -183,15 +191,17 @@
 
         if self.start.bookingtype in ['in', 'out']:
             query['category'] = self.start.category.id
             query['party'] = getattr(self.start.party, 'id', None)
         elif self.start.bookingtype in ['mvin', 'mvout']:
             query['booktransf'] = self.start.booktransf.id
 
-        Line.create([query])
+        lines = Line.create([query])
+        if self.start.fixate:
+            Line.wfcheck(lines)
         return 'end'
 
     def transition_savenext_(self):
         """ store booking & restart
         """
         self.transition_save_()
         return 'start'
```

### Comparing `mds_cashbook-7.0.33/wizard_booking.xml` & `mds_cashbook-7.0.34/wizard_booking.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/wizard_openline.py` & `mds_cashbook-7.0.34/wizard_openline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/wizard_openline.xml` & `mds_cashbook-7.0.34/wizard_openline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/wizard_runreport.py` & `mds_cashbook-7.0.34/wizard_runreport.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.33/wizard_runreport.xml` & `mds_cashbook-7.0.34/wizard_runreport.xml`

 * *Files identical despite different names*

