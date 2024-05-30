# Comparing `tmp/mappyfile-1.0.1.tar.gz` & `tmp/mappyfile-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappyfile-1.0.1.tar", last modified: Fri Apr 26 08:39:05 2024, max compression
+gzip compressed data, was "mappyfile-1.0.2.tar", last modified: Thu May 30 15:55:43 2024, max compression
```

## Comparing `mappyfile-1.0.1.tar` & `mappyfile-1.0.2.tar`

### file list

```diff
@@ -1,115 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.693572 mappyfile-1.0.1/
--rw-rw-rw-   0        0        0     1089 2017-07-06 19:50:13.000000 mappyfile-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       78 2017-10-02 08:44:46.000000 mappyfile-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5410 2024-04-26 08:39:05.693572 mappyfile-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4546 2023-09-28 08:55:09.000000 mappyfile-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.386873 mappyfile-1.0.1/docs/
--rw-rw-rw-   0        0        0        9 2023-08-11 15:22:45.000000 mappyfile-1.0.1/docs/.gitignore
--rw-rw-rw-   0        0        0    17323 2023-10-05 06:43:32.000000 mappyfile-1.0.1/docs/HISTORY.rst
--rw-rw-rw-   0        0        0     7843 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/Makefile
--rw-rw-rw-   0        0        0     3354 2020-07-14 05:32:08.000000 mappyfile-1.0.1/docs/client.rst
--rw-rw-rw-   0        0        0     3710 2023-08-13 18:55:15.000000 mappyfile-1.0.1/docs/comments.rst
--rw-rw-rw-   0        0        0    19393 2023-08-11 15:48:40.000000 mappyfile-1.0.1/docs/conf.py
--rw-rw-rw-   0        0        0     2882 2023-09-28 07:25:03.000000 mappyfile-1.0.1/docs/development.rst
--rw-rw-rw-   0        0        0     3237 2023-08-13 18:25:58.000000 mappyfile-1.0.1/docs/editing.rst
--rw-rw-rw-   0        0        0     1655 2018-08-22 22:23:30.000000 mappyfile-1.0.1/docs/format.txt
--rw-rw-rw-   0        0        0     7176 2023-04-20 10:21:52.000000 mappyfile-1.0.1/docs/grammar.rst
--rw-rw-rw-   0        0        0    10113 2023-09-28 07:56:02.000000 mappyfile-1.0.1/docs/index.rst
--rwxrwxrwx   0        0        0     7738 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/make.bat
--rw-rw-rw-   0        0        0     6378 2023-08-11 15:31:23.000000 mappyfile-1.0.1/docs/parser.rst
--rw-rw-rw-   0        0        0    12725 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/performance.txt
--rw-rw-rw-   0        0        0     5423 2023-08-13 18:28:48.000000 mappyfile-1.0.1/docs/pretty_printing.rst
--rw-rw-rw-   0        0        0     1144 2023-08-11 14:50:51.000000 mappyfile-1.0.1/docs/python_integration.rst
--rw-rw-rw-   0        0        0       13 2024-04-25 14:10:28.000000 mappyfile-1.0.1/docs/requirements.txt
--rw-rw-rw-   0        0        0    10515 2023-08-13 18:15:54.000000 mappyfile-1.0.1/docs/rfc.rst
--rw-rw-rw-   0        0        0     1692 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/sample_dict.json
--rw-rw-rw-   0        0        0      879 2017-07-06 19:50:13.000000 mappyfile-1.0.1/docs/sample_map.txt
--rw-rw-rw-   0        0        0     2723 2023-08-11 17:41:30.000000 mappyfile-1.0.1/docs/schemas.rst
--rw-rw-rw-   0        0        0     3497 2023-08-13 18:03:47.000000 mappyfile-1.0.1/docs/testing.rst
--rw-rw-rw-   0        0        0     2268 2023-08-13 18:22:08.000000 mappyfile-1.0.1/docs/transformer.rst
--rw-rw-rw-   0        0        0      923 2018-08-22 22:23:30.000000 mappyfile-1.0.1/docs/validate.txt
--rw-rw-rw-   0        0        0     5919 2023-08-13 08:30:20.000000 mappyfile-1.0.1/docs/validation.rst
--rw-rw-rw-   0        0        0      305 2018-08-22 22:23:30.000000 mappyfile-1.0.1/docs/validation_errors.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.406803 mappyfile-1.0.1/mappyfile/
--rw-rw-rw-   0        0        0     2534 2024-03-14 12:58:45.000000 mappyfile-1.0.1/mappyfile/__init__.py
--rw-rw-rw-   0        0        0     8598 2023-08-13 12:38:53.000000 mappyfile-1.0.1/mappyfile/cli.py
--rw-rw-rw-   0        0        0     8716 2024-04-25 14:05:28.000000 mappyfile-1.0.1/mappyfile/dictutils.py
--rw-rw-rw-   0        0        0     5600 2024-01-11 16:05:39.000000 mappyfile-1.0.1/mappyfile/mapfile.lark
--rw-rw-rw-   0        0        0     5223 2023-08-13 18:01:01.000000 mappyfile-1.0.1/mappyfile/ordereddict.py
--rw-rw-rw-   0        0        0     8626 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/parser.py
--rw-rw-rw-   0        0        0    20742 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/pprint.py
--rw-rw-rw-   0        0        0        0 2023-08-14 14:48:56.000000 mappyfile-1.0.1/mappyfile/py.typed
--rw-rw-rw-   0        0        0     4021 2023-08-13 12:18:42.000000 mappyfile-1.0.1/mappyfile/quoter.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.475840 mappyfile-1.0.1/mappyfile/schemas/
--rw-rw-rw-   0        0        0     3134 2024-01-12 14:40:01.000000 mappyfile-1.0.1/mappyfile/schemas/class.json
--rw-rw-rw-   0        0        0      815 2022-02-21 21:03:48.000000 mappyfile-1.0.1/mappyfile/schemas/cluster.json
--rw-rw-rw-   0        0        0      335 2023-08-02 07:58:46.000000 mappyfile-1.0.1/mappyfile/schemas/color.json
--rw-rw-rw-   0        0        0     1140 2022-06-13 21:01:53.000000 mappyfile-1.0.1/mappyfile/schemas/composite.json
--rw-rw-rw-   0        0        0      128 2020-01-09 23:26:49.000000 mappyfile-1.0.1/mappyfile/schemas/connectionoptions.json
--rw-rw-rw-   0        0        0       51 2017-10-01 10:38:49.000000 mappyfile-1.0.1/mappyfile/schemas/debug.json
--rw-rw-rw-   0        0        0      274 2024-01-12 14:39:15.000000 mappyfile-1.0.1/mappyfile/schemas/expression.json
--rw-rw-rw-   0        0        0      103 2023-08-02 07:58:42.000000 mappyfile-1.0.1/mappyfile/schemas/extent.json
--rw-rw-rw-   0        0        0      668 2018-06-11 10:04:25.000000 mappyfile-1.0.1/mappyfile/schemas/feature.json
--rw-rw-rw-   0        0        0     1015 2022-06-13 21:01:53.000000 mappyfile-1.0.1/mappyfile/schemas/grid.json
--rw-rw-rw-   0        0        0      105 2017-09-20 14:03:32.000000 mappyfile-1.0.1/mappyfile/schemas/hex.json
--rw-rw-rw-   0        0        0      107 2017-09-20 17:48:38.000000 mappyfile-1.0.1/mappyfile/schemas/hex2.json
--rw-rw-rw-   0        0        0     1064 2019-10-06 21:14:50.000000 mappyfile-1.0.1/mappyfile/schemas/join.json
--rw-rw-rw-   0        0        0     8076 2023-08-13 10:02:15.000000 mappyfile-1.0.1/mappyfile/schemas/label.json
--rw-rw-rw-   0        0        0     7362 2023-08-13 10:24:53.000000 mappyfile-1.0.1/mappyfile/schemas/layer.json
--rw-rw-rw-   0        0        0      563 2023-04-20 10:27:46.000000 mappyfile-1.0.1/mappyfile/schemas/leader.json
--rw-rw-rw-   0        0        0     1668 2022-02-21 21:03:48.000000 mappyfile-1.0.1/mappyfile/schemas/legend.json
--rw-rw-rw-   0        0        0     3888 2023-08-13 11:04:08.000000 mappyfile-1.0.1/mappyfile/schemas/map.json
--rw-rw-rw-   0        0        0       82 2017-09-26 10:20:23.000000 mappyfile-1.0.1/mappyfile/schemas/metadata.json
--rw-rw-rw-   0        0        0       51 2017-09-24 22:00:41.000000 mappyfile-1.0.1/mappyfile/schemas/onoff.json
--rw-rw-rw-   0        0        0     1056 2022-06-13 21:01:53.000000 mappyfile-1.0.1/mappyfile/schemas/outputformat.json
--rw-rw-rw-   0        0        0      192 2018-01-16 16:42:03.000000 mappyfile-1.0.1/mappyfile/schemas/points.json
--rw-rw-rw-   0        0        0       72 2017-09-24 21:58:49.000000 mappyfile-1.0.1/mappyfile/schemas/position.json
--rw-rw-rw-   0        0        0      165 2018-02-07 23:07:41.000000 mappyfile-1.0.1/mappyfile/schemas/projection.json
--rw-rw-rw-   0        0        0      795 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/querymap.json
--rw-rw-rw-   0        0        0     1200 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/reference.json
--rw-rw-rw-   0        0        0      143 2017-09-20 14:01:00.000000 mappyfile-1.0.1/mappyfile/schemas/rgb.json
--rw-rw-rw-   0        0        0     2604 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/scalebar.json
--rw-rw-rw-   0        0        0      466 2018-06-11 10:04:25.000000 mappyfile-1.0.1/mappyfile/schemas/scaletoken.json
--rw-rw-rw-   0        0        0       96 2017-09-23 23:25:20.000000 mappyfile-1.0.1/mappyfile/schemas/sizeunits.json
--rw-rw-rw-   0        0        0     6505 2023-06-01 15:35:22.000000 mappyfile-1.0.1/mappyfile/schemas/style.json
--rw-rw-rw-   0        0        0     1620 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/symbol.json
--rw-rw-rw-   0        0        0      323 2021-12-06 13:53:21.000000 mappyfile-1.0.1/mappyfile/schemas/symbolset.json
--rw-rw-rw-   0        0        0       93 2017-10-01 10:10:15.000000 mappyfile-1.0.1/mappyfile/schemas/units.json
--rw-rw-rw-   0        0        0       82 2017-09-26 10:20:23.000000 mappyfile-1.0.1/mappyfile/schemas/validation.json
--rw-rw-rw-   0        0        0     2149 2022-02-21 21:03:49.000000 mappyfile-1.0.1/mappyfile/schemas/web.json
--rw-rw-rw-   0        0        0       52 2018-05-14 10:05:23.000000 mappyfile-1.0.1/mappyfile/schemas/yesno.json
--rw-rw-rw-   0        0        0     6275 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/tokens.py
--rw-rw-rw-   0        0        0    23783 2024-01-12 14:23:25.000000 mappyfile-1.0.1/mappyfile/transformer.py
--rw-rw-rw-   0        0        0    14610 2023-08-13 18:01:01.000000 mappyfile-1.0.1/mappyfile/utils.py
--rw-rw-rw-   0        0        0    11983 2023-08-13 18:01:01.000000 mappyfile-1.0.1/mappyfile/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.421517 mappyfile-1.0.1/mappyfile.egg-info/
--rw-rw-rw-   0        0        0     5410 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-14 09:32:10.000000 mappyfile-1.0.1/mappyfile.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       87 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 08:39:04.000000 mappyfile-1.0.1/mappyfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1002 2023-07-27 16:39:13.000000 mappyfile-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      169 2024-04-26 08:39:05.696573 mappyfile-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-09-28 08:53:25.000000 mappyfile-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:39:05.691564 mappyfile-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2017-07-06 19:50:13.000000 mappyfile-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      485 2023-09-02 14:55:20.000000 mappyfile-1.0.1/tests/test_cli.py
--rw-rw-rw-   0        0        0     8326 2023-08-01 14:59:09.000000 mappyfile-1.0.1/tests/test_comments.py
--rw-rw-rw-   0        0        0     1882 2024-01-11 21:03:52.000000 mappyfile-1.0.1/tests/test_config.py
--rw-rw-rw-   0        0        0     8512 2024-04-26 08:37:25.000000 mappyfile-1.0.1/tests/test_dictutils.py
--rw-rw-rw-   0        0        0     2579 2023-07-27 22:39:55.000000 mappyfile-1.0.1/tests/test_errors.py
--rw-rw-rw-   0        0        0    10925 2023-06-02 06:55:32.000000 mappyfile-1.0.1/tests/test_expressions.py
--rw-rw-rw-   0        0        0     3213 2023-06-02 06:55:32.000000 mappyfile-1.0.1/tests/test_includes.py
--rw-rw-rw-   0        0        0     1933 2023-08-13 10:07:02.000000 mappyfile-1.0.1/tests/test_map_collection.py
--rw-rw-rw-   0        0        0     3220 2023-08-13 10:45:27.000000 mappyfile-1.0.1/tests/test_msautotest.py
--rw-rw-rw-   0        0        0     4634 2023-06-02 06:55:33.000000 mappyfile-1.0.1/tests/test_ordereddict.py
--rw-rw-rw-   0        0        0    12135 2023-08-13 18:01:01.000000 mappyfile-1.0.1/tests/test_pprint.py
--rw-rw-rw-   0        0        0      923 2023-08-13 18:01:01.000000 mappyfile-1.0.1/tests/test_quoter.py
--rw-rw-rw-   0        0        0     4162 2023-08-13 10:00:33.000000 mappyfile-1.0.1/tests/test_sample_maps.py
--rw-rw-rw-   0        0        0    24723 2024-01-12 14:41:23.000000 mappyfile-1.0.1/tests/test_snippets.py
--rw-rw-rw-   0        0        0     2045 2023-06-02 06:55:33.000000 mappyfile-1.0.1/tests/test_symbolset.py
--rw-rw-rw-   0        0        0     8398 2023-08-13 12:59:09.000000 mappyfile-1.0.1/tests/test_transformer.py
--rw-rw-rw-   0        0        0     4262 2023-08-13 18:01:01.000000 mappyfile-1.0.1/tests/test_utils.py
--rw-rw-rw-   0        0        0    14374 2024-01-12 14:23:25.000000 mappyfile-1.0.1/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:55:43.002356 mappyfile-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-30 15:52:12.000000 mappyfile-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 15:52:12.000000 mappyfile-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-30 15:55:43.002356 mappyfile-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-30 15:52:12.000000 mappyfile-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:55:42.990356 mappyfile-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/comments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18801 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/editing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/grammar.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/performance.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/pretty_printing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/python_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/rfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/sample_dict.json
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/sample_map.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/transformer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/validate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 15:52:12.000000 mappyfile-1.0.2/docs/validation_errors.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:55:42.990356 mappyfile-1.0.2/mappyfile/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/dictutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/mapfile.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/ordereddict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/quoter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:55:42.998356 mappyfile-1.0.2/mappyfile/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/class.json
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/cluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/color.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/composite.json
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/connectionoptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/debug.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/expression.json
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/extent.json
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/hex2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/join.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/label.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/layer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/leader.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/legend.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/onoff.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/outputformat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/points.json
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/position.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/projection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/querymap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/rgb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/scalebar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/scaletoken.json
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/sizeunits.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/style.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/symbol.json
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/symbolset.json
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/units.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/validation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/web.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/schemas/yesno.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-30 15:52:12.000000 mappyfile-1.0.2/mappyfile/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:55:43.002356 mappyfile-1.0.2/mappyfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-30 15:55:42.000000 mappyfile-1.0.2/mappyfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 15:55:42.000000 mappyfile-1.0.2/mappyfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:55:42.000000 mappyfile-1.0.2/mappyfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 15:55:42.000000 mappyfile-1.0.2/mappyfile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:52:35.000000 mappyfile-1.0.2/mappyfile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 15:55:42.000000 mappyfile-1.0.2/mappyfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:55:42.000000 mappyfile-1.0.2/mappyfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-30 15:52:12.000000 mappyfile-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 15:55:43.002356 mappyfile-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-30 15:52:12.000000 mappyfile-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:55:43.002356 mappyfile-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_dictutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_map_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_msautotest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_ordereddict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_quoter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_sample_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23667 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_symbolset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-05-30 15:52:12.000000 mappyfile-1.0.2/tests/test_validation.py
```

### Comparing `mappyfile-1.0.1/PKG-INFO` & `mappyfile-1.0.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,135 @@
-Metadata-Version: 2.1
-Name: mappyfile
-Version: 1.0.1
-Summary: A pure Python MapFile parser for working with MapServer
-Home-page: http://github.com/geographika/mappyfile
-Author: Seth Girvin
-Author-email: sethg@geographika.co.uk
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Text Processing :: Linguistic
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/x-rst
-Provides-Extra: lark_cython
-License-File: LICENSE
-
-mappyfile
-=========
-
-| |Version| |Docs| |Build Status| |Coveralls| |Appveyor Build Status| |Downloads|
-
-A pure Python parser for working with `MapServer <https://mapserver.org>`_ MapFiles, built using `Lark <https://github.com/lark-parser/lark>`__.
-mappyfile is an official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_.
-
-.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/OSGeo_community_small.png
-    :align: right
-
-mappyfile is used for formatting and validation in https://app.mapserverstudio.net/, and can be tested for free on any
-of your Mapfiles. If you find mappyfile useful please consider signing up for a professional account at 
-https://mapserverstudio.net/. This will help to fund maintenance and further development of both mappyfile and MapServer.
-
-Requirements
-------------
-
-* Python 3.8 or higher
-
-Installation
-------------
-
-mappyfile is available on `PyPI <https://pypi.org/project/mappyfile/>`_ (the Python Package Index), and can be installed using pip:
-
-.. code-block:: console
-
-    pip install mappyfile
-
-This will also install its required dependencies - `Lark <https://github.com/lark-parser/lark>`__, and 
-`jsonschema <https://github.com/python-jsonschema/jsonschema>`_. 
-
-To install the optional `lark-cython <https://github.com/lark-parser/lark_cython>`_ library
-for better performance on CPython you can run the following command:
-
-.. code-block:: console
-
-    pip install mappyfile[lark_cython]
-
-mappyfile is also available on `conda <https://anaconda.org/conda-forge/mappyfile>`_. Install as
-follows:
-
-.. code-block:: console
-
-    conda install -c conda-forge mappyfile
-
-Documentation
--------------
-
-Full documentation is available at http://mappyfile.readthedocs.io/en/latest/
-
-.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/class_parsed_small.png
-
-Usage
------
-
-From within Python scripts:
-
-.. code-block:: python
-
-    import mappyfile
-
-    mapfile = mappyfile.open("./docs/examples/raster.map")
-    
-    # update the map name
-    mapfile["name"] = "MyNewMap"
-
-    new_layer_string = """
-    LAYER
-        NAME 'land'
-        TYPE POLYGON
-        DATA '../data/vector/naturalearth/ne_110m_land'
-        CLASS
-            STYLE
-                COLOR 107 208 107
-                OUTLINECOLOR 2 2 2
-                WIDTH 1
-            END
-        END
-    END
-    """
-
-    layers = mapfile["layers"]
-
-    new_layer = mappyfile.loads(new_layer_string)
-
-    layers.insert(0, new_layer) # insert the new layer at any index in the Mapfile
-
-    for l in layers:
-        print("{} {}".format(l["name"], l["type"]))
-
-    print(mappyfile.dumps(mapfile, indent=1, spacer="\t"))
-
-Three command line tools are available - ``format``, ``validate``, and ``schema``:
-
-.. code-block:: bat
-
-    mappyfile format raster.map formatted_raster.map
-    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
-    mappyfile schema mapfile-schema-8-0.json --version=8.0
-
-Authors
--------
-
-* Seth Girvin `@geographika <https://github.com/geographika>`_
-* Erez Shinan `@erezsh <https://github.com/erezsh>`_
-
-Contributors
-------------
-
-* Julien Enselme `@jenselme <https://github.com/jenselme>`_
-* Loïc Gasser `@loicgasser <https://github.com/loicgasser>`_
-* Ian Turton `@ianturton <https://github.com/ianturton>`_
-* `@thorag76 <https://github.com/thorag76>`_
-* `@DonQueso89 <https://github.com/DonQueso89>`_
-* TC Haddad `@tchaddad <https://github.com/tchaddad>`_ (Conda support)
-
-.. |Version| image:: https://img.shields.io/pypi/v/mappyfile.svg
-   :target: https://pypi.python.org/pypi/mappyfile
-
-.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
-   :target: http://mappyfile.readthedocs.io/en/latest/
-
-.. |Build Status| image:: https://github.com/geographika/mappyfile/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/geographika/mappyfile/actions/workflows/main.yml
-
-.. |Appveyor Build Status| image:: https://ci.appveyor.com/api/projects/status/mk33l07478gfytwh?svg=true
-   :target: https://ci.appveyor.com/project/SethG/mappyfile
-
-.. |Coveralls| image:: https://coveralls.io/repos/github/geographika/mappyfile/badge.svg?branch=master
-    :target: https://coveralls.io/github/geographika/mappyfile?branch=master
-
-.. |Downloads| image:: https://static.pepy.tech/badge/mappyfile
-    :target: https://www.pepy.tech/projects/mappyfile
-    
+mappyfile
+=========
+
+| |Version| |Docs| |Build Status| |Coveralls| |Appveyor Build Status| |Downloads|
+
+A pure Python parser for working with `MapServer <https://mapserver.org>`_ MapFiles, built using `Lark <https://github.com/lark-parser/lark>`__.
+mappyfile is an official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_.
+
+.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/OSGeo_community_small.png
+    :align: right
+
+mappyfile is used for formatting and validation in https://app.mapserverstudio.net/, and can be tested for free on any
+of your Mapfiles. If you find mappyfile useful please consider signing up for a professional account at 
+https://mapserverstudio.net/. This will help to fund maintenance and further development of both mappyfile and MapServer.
+
+Requirements
+------------
+
+* Python 3.8 or higher
+
+Installation
+------------
+
+mappyfile is available on `PyPI <https://pypi.org/project/mappyfile/>`_ (the Python Package Index), and can be installed using pip:
+
+.. code-block:: console
+
+    pip install mappyfile
+
+This will also install its required dependencies - `Lark <https://github.com/lark-parser/lark>`__, and 
+`jsonschema <https://github.com/python-jsonschema/jsonschema>`_. 
+
+To install the optional `lark-cython <https://github.com/lark-parser/lark_cython>`_ library
+for better performance on CPython you can run the following command:
+
+.. code-block:: console
+
+    pip install mappyfile[lark_cython]
+
+mappyfile is also available on `conda <https://anaconda.org/conda-forge/mappyfile>`_. Install as
+follows:
+
+.. code-block:: console
+
+    conda install -c conda-forge mappyfile
+
+Documentation
+-------------
+
+Full documentation is available at http://mappyfile.readthedocs.io/en/latest/
+
+.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/class_parsed_small.png
+
+Usage
+-----
+
+From within Python scripts:
+
+.. code-block:: python
+
+    import mappyfile
+
+    mapfile = mappyfile.open("./docs/examples/raster.map")
+    
+    # update the map name
+    mapfile["name"] = "MyNewMap"
+
+    new_layer_string = """
+    LAYER
+        NAME 'land'
+        TYPE POLYGON
+        DATA '../data/vector/naturalearth/ne_110m_land'
+        CLASS
+            STYLE
+                COLOR 107 208 107
+                OUTLINECOLOR 2 2 2
+                WIDTH 1
+            END
+        END
+    END
+    """
+
+    layers = mapfile["layers"]
+
+    new_layer = mappyfile.loads(new_layer_string)
+
+    layers.insert(0, new_layer) # insert the new layer at any index in the Mapfile
+
+    for l in layers:
+        print("{} {}".format(l["name"], l["type"]))
+
+    print(mappyfile.dumps(mapfile, indent=1, spacer="\t"))
+
+Three command line tools are available - ``format``, ``validate``, and ``schema``:
+
+.. code-block:: bat
+
+    mappyfile format raster.map formatted_raster.map
+    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
+    mappyfile schema mapfile-schema-8-0.json --version=8.0
+
+Authors
+-------
+
+* Seth Girvin `@geographika <https://github.com/geographika>`_
+* Erez Shinan `@erezsh <https://github.com/erezsh>`_
+
+Contributors
+------------
+
+* Julien Enselme `@jenselme <https://github.com/jenselme>`_
+* Loïc Gasser `@loicgasser <https://github.com/loicgasser>`_
+* Ian Turton `@ianturton <https://github.com/ianturton>`_
+* `@thorag76 <https://github.com/thorag76>`_
+* `@DonQueso89 <https://github.com/DonQueso89>`_
+* TC Haddad `@tchaddad <https://github.com/tchaddad>`_ (Conda support)
+
+.. |Version| image:: https://img.shields.io/pypi/v/mappyfile.svg
+   :target: https://pypi.python.org/pypi/mappyfile
+
+.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
+   :target: http://mappyfile.readthedocs.io/en/latest/
+
+.. |Build Status| image:: https://github.com/geographika/mappyfile/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/geographika/mappyfile/actions/workflows/main.yml
+
+.. |Appveyor Build Status| image:: https://ci.appveyor.com/api/projects/status/mk33l07478gfytwh?svg=true
+   :target: https://ci.appveyor.com/project/SethG/mappyfile
+
+.. |Coveralls| image:: https://coveralls.io/repos/github/geographika/mappyfile/badge.svg?branch=master
+    :target: https://coveralls.io/github/geographika/mappyfile?branch=master
+
+.. |Downloads| image:: https://static.pepy.tech/badge/mappyfile
+    :target: https://www.pepy.tech/projects/mappyfile
+
```

### Comparing `mappyfile-1.0.1/docs/HISTORY.rst` & `mappyfile-1.0.2/docs/HISTORY.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,375 +1,375 @@
-Releases
---------
-
-1.0.0 28/09/2023
-++++++++++++++++
-
-In celebration of becoming an official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_, 
-a version ``1.0.0`` release is now out!
-
-+ **Support for Python 2.7 has now been dropped.**
-  See `#166 <https://github.com/geographika/mappyfile/issues/166>`_ - Drop Python 2.7 support. The codebase has had all Python2 specific
-  code removed - see `#188 <https://github.com/geographika/mappyfile/issues/188>`_.
-
-+ **Breaking Change** - in the ``MapfileToDict`` class the parameter ``transformerClass`` has been renamed ``transformer_class``.
-  An example of how to fix this is shown below:
-
-  .. code-block:: python
-
-    from mappyfile.transformer import MapfileToDict
-    from mappyfile_colors import ColorsTransformer
-
-    m = MapfileToDict(
-        include_position=True,
-        include_comments=True,
-        # replace the following parameter
-        # transformerClass=ColorsTransformer,
-        transformer_class=ColorsTransformer,
-        conversion_type=None,
-        include_color_names=True,
-    )
-
-+ **Breaking Change** - ``LAYER`` ``DATA`` has been changed in the schema from a list to a simple string.
-
-  .. code-block:: python
-
-      layer = {
-          '__type__': 'layer',
-          // pre v1 the data clause had to be in a list
-          // 'data': ['/path/to/data']
-          // in v1 this should now be a string
-          'data': '/path/to/data'
-      }
-
-      mappyfile.dumps(layer)
-
-+ Support added for `lark_cython <https://github.com/lark-parser/lark_cython>`_ - see `#178 <https://github.com/geographika/mappyfile/issues/178>`_ - thanks @erezsh.
-  To use ``lark_cython`` is as simple as installing the option with ``pip``:
-
-  .. code-block:: bash
-
-      pip install mappyfile[lark_cython]
-
-+ All mappyfile dicts now have human readable output when displayed as a string:
-
-  .. code-block:: python
-
-    mf = mappyfile.open("./docs/examples/before.map")
-    print(mf)
-
-    # previous output
-    # DefaultOrderedDict(<class 'mappyfile.ordereddict.CaseInsensitiveOrderedDict'>, CaseInsensitiveOrderedDict([('__type__', 'map'),..
-
-    # new output
-    {
-        "__type__": "map",
-        "layers": [
-            {
-                "__type__": "layer",
-                "name": "Layer1",
-                "type": "POLYGON"
-            },
-
-+ Approach to resolving JSON references updated due to the deprecated ``jsonschema.RefResolver`` - see 
-  `this link <https://python-jsonschema.readthedocs.io/en/v4.18.4/referencing/#resolving-references-from-the-file-system>`_,
-  the associated JSONSchema `pull request <https://github.com/python-jsonschema/jsonschema/pull/1049>`_
-  and the `migration approach <https://python-jsonschema.readthedocs.io/en/stable/referencing/#migrating-from-refresolver>`_.
-
-Other improvements and fixes in the v1.0.0 release:
-
-+ `#196 <https://github.com/geographika/mappyfile/pull/196>`_ - Code base fixes for ``Prospector`` warnings
-+ `#195 <https://github.com/geographika/mappyfile/pull/195>`_ - Update test suite from latest msautotests
-+ `#194 <https://github.com/geographika/mappyfile/pull/194>`_ - Docs overhaul in preparation for v1 release
-+ `#193 <https://github.com/geographika/mappyfile/pull/193>`_ - Update to ``jsonschema`` v4 and replace deprecated ``RefResolver``
-+ `#191 <https://github.com/geographika/mappyfile/pull/191>`_ - Simplify processing of comments
-+ `#189 <https://github.com/geographika/mappyfile/pull/189>`_ - Add type hints to the code base
-+ `#153 <https://github.com/geographika/mappyfile/pull/153>`_ - Support querying items without the given key in 
-  ``utils.findunique()``- thanks @DonQueso89 for fix
-+ Schema fixes for ``grid``, ``label``, ``style``, ``leader``, add ``flatgeobuf``
-+ Code reformatted using `black <https://pypi.org/project/black/>`_
-
-Resolution of long-standing parsing issues, and all msautotest examples now pass successfully:
-
-+ `#48 <https://github.com/geographika/mappyfile/issues/48>`_ - SYMBOL ambiguity
-+ `#98 <https://github.com/geographika/mappyfile/issues/98>`_ - Unquoted attribute names fail to parse
-
-
-0.9.7 03/04/2022
-++++++++++++++++
-
-+ Fix ""ResourceWarning: unclosed"" when reading mapfile.lark in Python 3.10
-+ `#151 <https://github.com/geographika/mappyfile/pull/151>`_ - Updates for COMPOSITE blocks
-+ `#150 <https://github.com/geographika/mappyfile/issues/150>`_ - Unknown COMPOP "SOFT-LIGHT" and error with several
-   lines with COMPFILTER with validate
-
-0.9.6 29/03/2022
-++++++++++++++++
-
-+ Schema fixes for GRID LABELFORMAT and set max versions for MAP DATAPATTERN and TEMPLATEPATTERN
-+ Allow TRUE/FALSE values for OUTPUTFORMAT TRANSPARENT
-
-0.9.5 01/03/2022
-++++++++++++++++
-
-+ `#147 <https://github.com/geographika/mappyfile/pull/147>`_ - Create list objects for containers when modifying dicts
-+ `#146 <https://github.com/geographika/mappyfile/pull/146>`_ - Add COMPOSITE validation
-+ `#145 <https://github.com/geographika/mappyfile/issues/145>`_ - layers.insert fails with dict error
-+ `#144 <https://github.com/geographika/mappyfile/issues/144>`_ - Invalid value in COMPOSITE - 'compfilter'
-+ `#140 <https://github.com/geographika/mappyfile/pull/140>`_ - New feature: group complex types at the end
-
-0.9.4 22/02/2022
-++++++++++++++++
-
-+ `#137 <https://github.com/geographika/mappyfile/issues/137>`_ - Checking mapfile dict properties creates invalid empty dictionaries
-+ `#119 <https://github.com/geographika/mappyfile/issues/119>`_ - STYLE GEOMTRANSFORM 'labelcenter'
-+ `#143 <https://github.com/geographika/mappyfile/pull/143>`_ - Automate schema building
-+ `#142 <https://github.com/geographika/mappyfile/pull/142>`_ - Allow newer versions of jsonschema for py3
-+ `#141 <https://github.com/geographika/mappyfile/pull/141>`_ - Update and fix Continuous Integration
-+ `#139 <https://github.com/geographika/mappyfile/pull/139>`_ - Feature: align values in column
-+ `#138 <https://github.com/geographika/mappyfile/pull/138>`_ - Update schema based on new Mapfile validation rules
-
-0.9.3 13/12/2021
-++++++++++++++++
-
-+ Adds a new ``mappyfile.create`` function to allow creation of Mapfile objects with default values
-+ Update the Mapfile schema to include ``default`` values for keywords
-
-0.9.2 28/08/2021
-++++++++++++++++
-
-+ Add the "idw" to ``LAYER`` ``CONNECIONTYPE``
-+ Correct "minVersion" of ``LABEL`` ``EXPRESSION``
-+ Add validation to ``LEGEND`` ``LABELS``
-+ Add correct validation for ``MAP`` ``LEGEND`` and ``OUTPUTFORMAT``
-+ Add "byte" to ``OUTPUTFORMAT`` ``IMAGEMODE``
-+ Add "maxVersion" to ``WEB`` ``LOG``
-+ `#120 <https://github.com/geographika/mappyfile/issues/120>`_ - Expression list element with apostrophe throws error
-+ `#118 <https://github.com/geographika/mappyfile/issues/118>`_ - LABEL -> FONT and LABEL -> POSITION gives errors in validate when attributes are used
-
-0.9.1 23/12/2020
-++++++++++++++++
-
-+ Allow any version of lark-parser > 0.9 to be used
-+ Fixes for requirements for Python 2.7
-+ `#115 <https://github.com/geographika/mappyfile/pull/115>`_ - Fix for issue #109 (OFFSET numeric and attribute pairs)
-+ `#114 <https://github.com/geographika/mappyfile/isses/114>`_ - Style OFFSET: mixed attribute and numerical value fail to parse
-
-0.9.0 14/07/2020
-++++++++++++++++
-
-+ Schemas updated to include ``minVersion`` and ``maxVersion`` metadata to define which Mapfile keywords are valid
-  for different versions of MapServer
-+ A new ``schema`` command line tool to export Mapfile schemas for different versions of MapServer
-+ Allow Mapfile validation based on a specific version of MapServer
-+ Add better error message when incorrect dicts are passed to printer
-+ Add py38 to continuous integration testing
-+ Add command line scripts to continuous integration testing
-+ Fix ``CONNECTIONOPTIONS`` formatted output
-+ Update to lark-parser 0.9.0
-+ `#109 <https://github.com/geographika/mappyfile/pull/109>`_ - Add validation based on MapServer version
-+ `#96 <https://github.com/geographika/mappyfile/issues/96>`_ - Unquoted Unicode strings cause parsing errors
-+ `#102 <https://github.com/geographika/mappyfile/pull/102>`_ - Added support for accented-latin in unquoted strings (Issue #96) - thanks @erezsh
-+ `#97 <https://github.com/geographika/mappyfile/issues/97>`_ - Allow for negative expressions
-+ `#101 <https://github.com/geographika/mappyfile/pull/101>`_ - Fix for issue #97 (unary negation) - thanks @erezsh
-+ `#85 <https://github.com/geographika/mappyfile/issues/85>`_ - Coding of NOT logical expression
-+ `#100 <https://github.com/geographika/mappyfile/pull/100>`_ - Allowing non-bracketed NOT expression (Issue #85) - thanks @erezsh
-
-0.8.4 11/01/2020
-++++++++++++++++
-
-+ Update to lark-parser 0.7.8
-+ `#95 <https://github.com/geographika/mappyfile/pull/95>`_ - Allow Mapfile input from ``io.StringIO`` as well 
-  as from a file - thanks @ianturton for pull request
-+ `#93 <https://github.com/geographika/mappyfile/issues/93>`_ - fix to ensure Mapfiles are closed after reading
-+ `#89 <https://github.com/geographika/mappyfile/issues/89>`_ - List expressions with spaces in the attributes fail to 
-  parse - thanks @ianturton for fix
-
-0.8.3 06/10/2019
-++++++++++++++++
-
-+ Update to lark-parser 0.7.7
-+ Update to jsonref 0.2
-+ Add automated releases to GitHub using Appveyor
-+ Add automated releases to PyPI using Appveyor
-+ Add missing CLASS properties to JSON schema
-+ Additional tests for CaseInsensitiveOrderedDict and EXPRESSIONs
-+ `#37 <https://github.com/geographika/mappyfile/issues/37>`_ - LIKE not recognised in FILTER - thanks @ianturton for fix
-+ `#87 <https://github.com/geographika/mappyfile/pull/87>`_ - JSON schema add join tag- thanks @hugbe8 for fix
-
-0.8.2 29/03/2019
-++++++++++++++++
-
-+ `#74 <https://github.com/geographika/mappyfile/issues/74>`_ - Map files containing Unicode can fail in mappyfile.load with 
-  python2.7 thanks @ianturton
-+ `#73 <https://github.com/geographika/mappyfile/issues/73>`_ - Deepcopy not working (Python3 >=3.5) - thanks @guardeivid
-+ Add support for CLUSTER keyword along with schema changes and tests
-
-0.8.1 27/02/2019
-++++++++++++++++
-
-+ Fix comments on root objects in a MapFile
-+ Fix issues with duplicated METADATA keys and comments
-+ Fix ReadTheDocs build
-+ Add more sample MapFiles for testing to the project
-
-0.8.0 24/02/2019
-++++++++++++++++
-
-+ Update code to work with Lark 0.6.6 (see #71)
-+ New end_comment option for pprint - Add a comment with the block type at each closing END statement e.g. END # MAP 
-  (see request `#69 <https://github.com/geographika/mappyfile/issues/69>`_)
-+ Add ``**kwargs`` to main API to allow greater flexibility with plugins
-+ Fix DeprecationWarnings relating to Python 3.7.2 (thanks @tigerfoot for the report)
-+ Tested use with new jsonschema 3.0.0 release
-
-0.7.6 (13/10/2018)
-++++++++++++++++++
-
-+ Deprecated ``write`` function removed from the API and codebase
-+ Update OFFSET validation to allow attribute bindings - see https://github.com/mapserver/docs/pull/256
-+ `#68 <https://github.com/geographika/mappyfile/issues/68>`_ - Support pickling of DefaultOrderedDict in Python3
-+ `#67 <https://github.com/geographika/mappyfile/issues/67>`_ - Fix deprecation warnings for grammar regular expressions in Python 3.6
-+ `#65 <https://github.com/geographika/mappyfile/issues/65>`_ - Handle hexadecimal color translucence
-
-0.7.5 (14/09/2018)
-++++++++++++++++++
-
-+ Save tokens for value lists
-+ Update README and fix example code
-
-0.7.4 (07/09/2018)
-++++++++++++++++++
-
-+ Support for modulus operator
-+ Allow custom transformers to be used with kwargs
-
-0.7.3 (23/08/2018)
-++++++++++++++++++
-
-+ Two new CLI programs - ``format`` and ``validate``
-+ Update of Lark parser to 0.6.4 (fixes some validation line number issues)
-+ Improvements to validation log messages
-+ Normalise include paths
-
-0.7.2 (24/07/2018)
-++++++++++++++++++
-
-+ Update of Lark parser to 0.6.2 and associated changes - thanks @erezsh
-+ ``mappyfile.findall`` returns a list rather than a generator
-+ ``SYMBOLSET`` files now supported (both parsing and transforming)
-+ `#63 <https://github.com/geographika/mappyfile/issues/63>`_ - Set the PROJECTION value correctly for single strings
-+ `#61 <https://github.com/geographika/mappyfile/issues/61>`_ - Remove quotes in mappyfile.findall()
-
-0.7.1 (10/07/2018)
-++++++++++++++++++
-
-+ **Breaking Change** ``utils.dictfind`` renamed ``utils.findkey``
-+ new dictionary update function - allowing for easier creation of Mapfiles using YAML
-+ allow any custom hidden metadata tags of the form ``__property__`` to be used in dicts for custom processing
-+ Schema validation updates including RANGEITEM and CLUSTER
-+ Appveyor builds added
-+ `#56 <https://github.com/geographika/mappyfile/issues/56>`_ Can't parse expressions with a : in them
-+ `#54 <https://github.com/geographika/mappyfile/issues/54>`_ fix windows cwd name issue in includes - thanks @ianturton
-
-0.7.0 (04/04/2018)
-++++++++++++++++++
-
-+ Finalise validation API
-+ Finalised Mapfile comments API
-+ New ``dictfind`` function
-+ Allow non-string function parameters in expressions
-+ Use of CaseInsensitiveOrderedDict throughout transformer
-+ UTF comments
-+ JSONSchema updates and fixes
-
-0.6.2 (24/02/2018)
-++++++++++++++++++
-
-+ **Breaking Change** - the ``mappyfile.load`` method now accepts a file-like object rather than a 
-  filename to match the usage in other Python libraries. A new ``mappyfile.open`` method allows opening 
-  directly with a filename. 
-+ New preserve comments feature - *experimental*
-+ Add basic plugin system
-+ Updates to schema docs (fixes for POSITION, AUTO, and added new default values)
-+ Fix issue with comments on INCLUDE lines
-+ `#50 <https://github.com/geographika/mappyfile/issues/50>`_ Allow END keyword for GEOTRANSFORM parameter
-+ `#49 <https://github.com/geographika/mappyfile/issues/45>`_ Allow non-ASCII characters in parser
-+ `#47 <https://github.com/geographika/mappyfile/issues/47>`_ Add in missing expression operators - 
-  divide, multiply, and power. 
-
-0.6.1 (06/02/2018)
-++++++++++++++++++
-
-+ Fixes to setup.py
-
-0.6.0 (17/01/2018)
-++++++++++++++++++
-
-+ Extensive refactoring of grammar and transformer
-+ Removal of Earley grammar
-+ Whitespace ignored when parsing
-+ JSON schema fixes
-+ `#45 <https://github.com/geographika/mappyfile/issues/45>`_ Set fixed dependency ranges
-+ *Experimental* - inclusion of token positions
-+ *Experimental* - inclusion of validation comments
-
-0.5.1 (05/01/2018)
-++++++++++++++++++
-
-+ `#45 <https://github.com/geographika/mappyfile/issues/45>`_ Remove unnecessary parser keyword
-
-0.5.0 (01/11/2017)
-++++++++++++++++++
-
-+ Add in jsonschema and validation class
-+ `#44 <https://github.com/geographika/mappyfile/issues/44>`_ Includes should be relative to Mapfile
-
-0.4.3 (28/08/2017)
-++++++++++++++++++
-
-+ `#36 <https://github.com/geographika/mappyfile/pull/36>`_ Create a unique logger for mappyfile logger
-+ `#35 <https://github.com/geographika/mappyfile/pull/35>`_ Add support for missing arithmetic expressions and run flake8 within tox
-  - thanks @loicgrasser
-+ `#33 <https://github.com/geographika/mappyfile/pull/33>`_ Fix max recursion limit count - thanks @loicgrasser
-
-
-0.4.0 (18/08/2017)
-++++++++++++++++++
-
-+ Add a LALR grammar and parser, now a 8k line Mapfile is now parsed 12x faster
-+ Add a experimental validator module using jsonschema
-+ `#30 <https://github.com/geographika/mappyfile/pull/30>`_ Flake8 support - thanks @loicgrasser
-+ `#28 <https://github.com/geographika/mappyfile/pull/28>`_ Add support for relative path for nested include - thanks @loicgrasser
-+ `#25 <https://github.com/geographika/mappyfile/issues/25>`_ Expression grammar not allowing ``!``
- 
-0.3.2
-+++++
-
-+ Revert back to a single grammar, but add linebreaks before all ``END`` keywords to keep acceptable performance
-
-0.3.1
-+++++
-
-+ Add in alternative grammar that allows for no line breaks between composites, and fall back to this
-  if parsing fails (otherwise most use cases suffer a 3x performance hit)
-
-0.3.0
-+++++
-
-+ Allow multiple composites to be parsed directly (e.g. ``CLASS..END CLASS..END``)
-+ Allow direct parsing of the ``METADATA`` and ``VALIDATION`` blocks
-+ UTF-8 checks when opening a Mapfile
-+ `#23 <https://github.com/geographika/mappyfile/issues/23>`_ Alternative NE and EQ comparisons not defined
-+ `#22 <https://github.com/geographika/mappyfile/issues/22>`_ Handle AUTO Projection setting
-+ `#21 <https://github.com/geographika/mappyfile/issues/21>`_ INCLUDES throw error when no cwd set
-+ `#20 <https://github.com/geographika/mappyfile/issues/20>`_ Only the first FORMATOPTION is kept after transform
-+ `#19 <https://github.com/geographika/mappyfile/issues/19>`_ IMAGEMODE FEATURE throws parsing error
-+ `#18 <https://github.com/geographika/mappyfile/issues/18>`_ CONFIG keyword not capitalised
-
-Older Releases
-++++++++++++++
-
-+ 0.2.2 - various fixes to grammar, and allow for alternate comparison operators
-+ 0.2.1 - new ``findall`` function, see https://github.com/geographika/mappyfile/pull/12 - thanks @Jenselme
-+ 0.2.0 - switch to Lark parser
+Releases
+--------
+
+1.0.0 28/09/2023
+++++++++++++++++
+
+In celebration of becoming an official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_, 
+a version ``1.0.0`` release is now out!
+
++ **Support for Python 2.7 has now been dropped.**
+  See `#166 <https://github.com/geographika/mappyfile/issues/166>`_ - Drop Python 2.7 support. The codebase has had all Python2 specific
+  code removed - see `#188 <https://github.com/geographika/mappyfile/issues/188>`_.
+
++ **Breaking Change** - in the ``MapfileToDict`` class the parameter ``transformerClass`` has been renamed ``transformer_class``.
+  An example of how to fix this is shown below:
+
+  .. code-block:: python
+
+    from mappyfile.transformer import MapfileToDict
+    from mappyfile_colors import ColorsTransformer
+
+    m = MapfileToDict(
+        include_position=True,
+        include_comments=True,
+        # replace the following parameter
+        # transformerClass=ColorsTransformer,
+        transformer_class=ColorsTransformer,
+        conversion_type=None,
+        include_color_names=True,
+    )
+
++ **Breaking Change** - ``LAYER`` ``DATA`` has been changed in the schema from a list to a simple string.
+
+  .. code-block:: python
+
+      layer = {
+          '__type__': 'layer',
+          // pre v1 the data clause had to be in a list
+          // 'data': ['/path/to/data']
+          // in v1 this should now be a string
+          'data': '/path/to/data'
+      }
+
+      mappyfile.dumps(layer)
+
++ Support added for `lark_cython <https://github.com/lark-parser/lark_cython>`_ - see `#178 <https://github.com/geographika/mappyfile/issues/178>`_ - thanks @erezsh.
+  To use ``lark_cython`` is as simple as installing the option with ``pip``:
+
+  .. code-block:: bash
+
+      pip install mappyfile[lark_cython]
+
++ All mappyfile dicts now have human readable output when displayed as a string:
+
+  .. code-block:: python
+
+    mf = mappyfile.open("./docs/examples/before.map")
+    print(mf)
+
+    # previous output
+    # DefaultOrderedDict(<class 'mappyfile.ordereddict.CaseInsensitiveOrderedDict'>, CaseInsensitiveOrderedDict([('__type__', 'map'),..
+
+    # new output
+    {
+        "__type__": "map",
+        "layers": [
+            {
+                "__type__": "layer",
+                "name": "Layer1",
+                "type": "POLYGON"
+            },
+
++ Approach to resolving JSON references updated due to the deprecated ``jsonschema.RefResolver`` - see 
+  `this link <https://python-jsonschema.readthedocs.io/en/v4.18.4/referencing/#resolving-references-from-the-file-system>`_,
+  the associated JSONSchema `pull request <https://github.com/python-jsonschema/jsonschema/pull/1049>`_
+  and the `migration approach <https://python-jsonschema.readthedocs.io/en/stable/referencing/#migrating-from-refresolver>`_.
+
+Other improvements and fixes in the v1.0.0 release:
+
++ `#196 <https://github.com/geographika/mappyfile/pull/196>`_ - Code base fixes for ``Prospector`` warnings
++ `#195 <https://github.com/geographika/mappyfile/pull/195>`_ - Update test suite from latest msautotests
++ `#194 <https://github.com/geographika/mappyfile/pull/194>`_ - Docs overhaul in preparation for v1 release
++ `#193 <https://github.com/geographika/mappyfile/pull/193>`_ - Update to ``jsonschema`` v4 and replace deprecated ``RefResolver``
++ `#191 <https://github.com/geographika/mappyfile/pull/191>`_ - Simplify processing of comments
++ `#189 <https://github.com/geographika/mappyfile/pull/189>`_ - Add type hints to the code base
++ `#153 <https://github.com/geographika/mappyfile/pull/153>`_ - Support querying items without the given key in 
+  ``utils.findunique()``- thanks @DonQueso89 for fix
++ Schema fixes for ``grid``, ``label``, ``style``, ``leader``, add ``flatgeobuf``
++ Code reformatted using `black <https://pypi.org/project/black/>`_
+
+Resolution of long-standing parsing issues, and all msautotest examples now pass successfully:
+
++ `#48 <https://github.com/geographika/mappyfile/issues/48>`_ - SYMBOL ambiguity
++ `#98 <https://github.com/geographika/mappyfile/issues/98>`_ - Unquoted attribute names fail to parse
+
+
+0.9.7 03/04/2022
+++++++++++++++++
+
++ Fix ""ResourceWarning: unclosed"" when reading mapfile.lark in Python 3.10
++ `#151 <https://github.com/geographika/mappyfile/pull/151>`_ - Updates for COMPOSITE blocks
++ `#150 <https://github.com/geographika/mappyfile/issues/150>`_ - Unknown COMPOP "SOFT-LIGHT" and error with several
+   lines with COMPFILTER with validate
+
+0.9.6 29/03/2022
+++++++++++++++++
+
++ Schema fixes for GRID LABELFORMAT and set max versions for MAP DATAPATTERN and TEMPLATEPATTERN
++ Allow TRUE/FALSE values for OUTPUTFORMAT TRANSPARENT
+
+0.9.5 01/03/2022
+++++++++++++++++
+
++ `#147 <https://github.com/geographika/mappyfile/pull/147>`_ - Create list objects for containers when modifying dicts
++ `#146 <https://github.com/geographika/mappyfile/pull/146>`_ - Add COMPOSITE validation
++ `#145 <https://github.com/geographika/mappyfile/issues/145>`_ - layers.insert fails with dict error
++ `#144 <https://github.com/geographika/mappyfile/issues/144>`_ - Invalid value in COMPOSITE - 'compfilter'
++ `#140 <https://github.com/geographika/mappyfile/pull/140>`_ - New feature: group complex types at the end
+
+0.9.4 22/02/2022
+++++++++++++++++
+
++ `#137 <https://github.com/geographika/mappyfile/issues/137>`_ - Checking mapfile dict properties creates invalid empty dictionaries
++ `#119 <https://github.com/geographika/mappyfile/issues/119>`_ - STYLE GEOMTRANSFORM 'labelcenter'
++ `#143 <https://github.com/geographika/mappyfile/pull/143>`_ - Automate schema building
++ `#142 <https://github.com/geographika/mappyfile/pull/142>`_ - Allow newer versions of jsonschema for py3
++ `#141 <https://github.com/geographika/mappyfile/pull/141>`_ - Update and fix Continuous Integration
++ `#139 <https://github.com/geographika/mappyfile/pull/139>`_ - Feature: align values in column
++ `#138 <https://github.com/geographika/mappyfile/pull/138>`_ - Update schema based on new Mapfile validation rules
+
+0.9.3 13/12/2021
+++++++++++++++++
+
++ Adds a new ``mappyfile.create`` function to allow creation of Mapfile objects with default values
++ Update the Mapfile schema to include ``default`` values for keywords
+
+0.9.2 28/08/2021
+++++++++++++++++
+
++ Add the "idw" to ``LAYER`` ``CONNECIONTYPE``
++ Correct "minVersion" of ``LABEL`` ``EXPRESSION``
++ Add validation to ``LEGEND`` ``LABELS``
++ Add correct validation for ``MAP`` ``LEGEND`` and ``OUTPUTFORMAT``
++ Add "byte" to ``OUTPUTFORMAT`` ``IMAGEMODE``
++ Add "maxVersion" to ``WEB`` ``LOG``
++ `#120 <https://github.com/geographika/mappyfile/issues/120>`_ - Expression list element with apostrophe throws error
++ `#118 <https://github.com/geographika/mappyfile/issues/118>`_ - LABEL -> FONT and LABEL -> POSITION gives errors in validate when attributes are used
+
+0.9.1 23/12/2020
+++++++++++++++++
+
++ Allow any version of lark-parser > 0.9 to be used
++ Fixes for requirements for Python 2.7
++ `#115 <https://github.com/geographika/mappyfile/pull/115>`_ - Fix for issue #109 (OFFSET numeric and attribute pairs)
++ `#114 <https://github.com/geographika/mappyfile/isses/114>`_ - Style OFFSET: mixed attribute and numerical value fail to parse
+
+0.9.0 14/07/2020
+++++++++++++++++
+
++ Schemas updated to include ``minVersion`` and ``maxVersion`` metadata to define which Mapfile keywords are valid
+  for different versions of MapServer
++ A new ``schema`` command line tool to export Mapfile schemas for different versions of MapServer
++ Allow Mapfile validation based on a specific version of MapServer
++ Add better error message when incorrect dicts are passed to printer
++ Add py38 to continuous integration testing
++ Add command line scripts to continuous integration testing
++ Fix ``CONNECTIONOPTIONS`` formatted output
++ Update to lark-parser 0.9.0
++ `#109 <https://github.com/geographika/mappyfile/pull/109>`_ - Add validation based on MapServer version
++ `#96 <https://github.com/geographika/mappyfile/issues/96>`_ - Unquoted Unicode strings cause parsing errors
++ `#102 <https://github.com/geographika/mappyfile/pull/102>`_ - Added support for accented-latin in unquoted strings (Issue #96) - thanks @erezsh
++ `#97 <https://github.com/geographika/mappyfile/issues/97>`_ - Allow for negative expressions
++ `#101 <https://github.com/geographika/mappyfile/pull/101>`_ - Fix for issue #97 (unary negation) - thanks @erezsh
++ `#85 <https://github.com/geographika/mappyfile/issues/85>`_ - Coding of NOT logical expression
++ `#100 <https://github.com/geographika/mappyfile/pull/100>`_ - Allowing non-bracketed NOT expression (Issue #85) - thanks @erezsh
+
+0.8.4 11/01/2020
+++++++++++++++++
+
++ Update to lark-parser 0.7.8
++ `#95 <https://github.com/geographika/mappyfile/pull/95>`_ - Allow Mapfile input from ``io.StringIO`` as well 
+  as from a file - thanks @ianturton for pull request
++ `#93 <https://github.com/geographika/mappyfile/issues/93>`_ - fix to ensure Mapfiles are closed after reading
++ `#89 <https://github.com/geographika/mappyfile/issues/89>`_ - List expressions with spaces in the attributes fail to 
+  parse - thanks @ianturton for fix
+
+0.8.3 06/10/2019
+++++++++++++++++
+
++ Update to lark-parser 0.7.7
++ Update to jsonref 0.2
++ Add automated releases to GitHub using Appveyor
++ Add automated releases to PyPI using Appveyor
++ Add missing CLASS properties to JSON schema
++ Additional tests for CaseInsensitiveOrderedDict and EXPRESSIONs
++ `#37 <https://github.com/geographika/mappyfile/issues/37>`_ - LIKE not recognised in FILTER - thanks @ianturton for fix
++ `#87 <https://github.com/geographika/mappyfile/pull/87>`_ - JSON schema add join tag- thanks @hugbe8 for fix
+
+0.8.2 29/03/2019
+++++++++++++++++
+
++ `#74 <https://github.com/geographika/mappyfile/issues/74>`_ - Map files containing Unicode can fail in mappyfile.load with 
+  python2.7 thanks @ianturton
++ `#73 <https://github.com/geographika/mappyfile/issues/73>`_ - Deepcopy not working (Python3 >=3.5) - thanks @guardeivid
++ Add support for CLUSTER keyword along with schema changes and tests
+
+0.8.1 27/02/2019
+++++++++++++++++
+
++ Fix comments on root objects in a MapFile
++ Fix issues with duplicated METADATA keys and comments
++ Fix ReadTheDocs build
++ Add more sample MapFiles for testing to the project
+
+0.8.0 24/02/2019
+++++++++++++++++
+
++ Update code to work with Lark 0.6.6 (see #71)
++ New end_comment option for pprint - Add a comment with the block type at each closing END statement e.g. END # MAP 
+  (see request `#69 <https://github.com/geographika/mappyfile/issues/69>`_)
++ Add ``**kwargs`` to main API to allow greater flexibility with plugins
++ Fix DeprecationWarnings relating to Python 3.7.2 (thanks @tigerfoot for the report)
++ Tested use with new jsonschema 3.0.0 release
+
+0.7.6 (13/10/2018)
+++++++++++++++++++
+
++ Deprecated ``write`` function removed from the API and codebase
++ Update OFFSET validation to allow attribute bindings - see https://github.com/mapserver/docs/pull/256
++ `#68 <https://github.com/geographika/mappyfile/issues/68>`_ - Support pickling of DefaultOrderedDict in Python3
++ `#67 <https://github.com/geographika/mappyfile/issues/67>`_ - Fix deprecation warnings for grammar regular expressions in Python 3.6
++ `#65 <https://github.com/geographika/mappyfile/issues/65>`_ - Handle hexadecimal color translucence
+
+0.7.5 (14/09/2018)
+++++++++++++++++++
+
++ Save tokens for value lists
++ Update README and fix example code
+
+0.7.4 (07/09/2018)
+++++++++++++++++++
+
++ Support for modulus operator
++ Allow custom transformers to be used with kwargs
+
+0.7.3 (23/08/2018)
+++++++++++++++++++
+
++ Two new CLI programs - ``format`` and ``validate``
++ Update of Lark parser to 0.6.4 (fixes some validation line number issues)
++ Improvements to validation log messages
++ Normalise include paths
+
+0.7.2 (24/07/2018)
+++++++++++++++++++
+
++ Update of Lark parser to 0.6.2 and associated changes - thanks @erezsh
++ ``mappyfile.findall`` returns a list rather than a generator
++ ``SYMBOLSET`` files now supported (both parsing and transforming)
++ `#63 <https://github.com/geographika/mappyfile/issues/63>`_ - Set the PROJECTION value correctly for single strings
++ `#61 <https://github.com/geographika/mappyfile/issues/61>`_ - Remove quotes in mappyfile.findall()
+
+0.7.1 (10/07/2018)
+++++++++++++++++++
+
++ **Breaking Change** ``utils.dictfind`` renamed ``utils.findkey``
++ new dictionary update function - allowing for easier creation of Mapfiles using YAML
++ allow any custom hidden metadata tags of the form ``__property__`` to be used in dicts for custom processing
++ Schema validation updates including RANGEITEM and CLUSTER
++ Appveyor builds added
++ `#56 <https://github.com/geographika/mappyfile/issues/56>`_ Can't parse expressions with a : in them
++ `#54 <https://github.com/geographika/mappyfile/issues/54>`_ fix windows cwd name issue in includes - thanks @ianturton
+
+0.7.0 (04/04/2018)
+++++++++++++++++++
+
++ Finalise validation API
++ Finalised Mapfile comments API
++ New ``dictfind`` function
++ Allow non-string function parameters in expressions
++ Use of CaseInsensitiveOrderedDict throughout transformer
++ UTF comments
++ JSONSchema updates and fixes
+
+0.6.2 (24/02/2018)
+++++++++++++++++++
+
++ **Breaking Change** - the ``mappyfile.load`` method now accepts a file-like object rather than a 
+  filename to match the usage in other Python libraries. A new ``mappyfile.open`` method allows opening 
+  directly with a filename. 
++ New preserve comments feature - *experimental*
++ Add basic plugin system
++ Updates to schema docs (fixes for POSITION, AUTO, and added new default values)
++ Fix issue with comments on INCLUDE lines
++ `#50 <https://github.com/geographika/mappyfile/issues/50>`_ Allow END keyword for GEOTRANSFORM parameter
++ `#49 <https://github.com/geographika/mappyfile/issues/45>`_ Allow non-ASCII characters in parser
++ `#47 <https://github.com/geographika/mappyfile/issues/47>`_ Add in missing expression operators - 
+  divide, multiply, and power. 
+
+0.6.1 (06/02/2018)
+++++++++++++++++++
+
++ Fixes to setup.py
+
+0.6.0 (17/01/2018)
+++++++++++++++++++
+
++ Extensive refactoring of grammar and transformer
++ Removal of Earley grammar
++ Whitespace ignored when parsing
++ JSON schema fixes
++ `#45 <https://github.com/geographika/mappyfile/issues/45>`_ Set fixed dependency ranges
++ *Experimental* - inclusion of token positions
++ *Experimental* - inclusion of validation comments
+
+0.5.1 (05/01/2018)
+++++++++++++++++++
+
++ `#45 <https://github.com/geographika/mappyfile/issues/45>`_ Remove unnecessary parser keyword
+
+0.5.0 (01/11/2017)
+++++++++++++++++++
+
++ Add in jsonschema and validation class
++ `#44 <https://github.com/geographika/mappyfile/issues/44>`_ Includes should be relative to Mapfile
+
+0.4.3 (28/08/2017)
+++++++++++++++++++
+
++ `#36 <https://github.com/geographika/mappyfile/pull/36>`_ Create a unique logger for mappyfile logger
++ `#35 <https://github.com/geographika/mappyfile/pull/35>`_ Add support for missing arithmetic expressions and run flake8 within tox
+  - thanks @loicgrasser
++ `#33 <https://github.com/geographika/mappyfile/pull/33>`_ Fix max recursion limit count - thanks @loicgrasser
+
+
+0.4.0 (18/08/2017)
+++++++++++++++++++
+
++ Add a LALR grammar and parser, now a 8k line Mapfile is now parsed 12x faster
++ Add a experimental validator module using jsonschema
++ `#30 <https://github.com/geographika/mappyfile/pull/30>`_ Flake8 support - thanks @loicgrasser
++ `#28 <https://github.com/geographika/mappyfile/pull/28>`_ Add support for relative path for nested include - thanks @loicgrasser
++ `#25 <https://github.com/geographika/mappyfile/issues/25>`_ Expression grammar not allowing ``!``
+ 
+0.3.2
++++++
+
++ Revert back to a single grammar, but add linebreaks before all ``END`` keywords to keep acceptable performance
+
+0.3.1
++++++
+
++ Add in alternative grammar that allows for no line breaks between composites, and fall back to this
+  if parsing fails (otherwise most use cases suffer a 3x performance hit)
+
+0.3.0
++++++
+
++ Allow multiple composites to be parsed directly (e.g. ``CLASS..END CLASS..END``)
++ Allow direct parsing of the ``METADATA`` and ``VALIDATION`` blocks
++ UTF-8 checks when opening a Mapfile
++ `#23 <https://github.com/geographika/mappyfile/issues/23>`_ Alternative NE and EQ comparisons not defined
++ `#22 <https://github.com/geographika/mappyfile/issues/22>`_ Handle AUTO Projection setting
++ `#21 <https://github.com/geographika/mappyfile/issues/21>`_ INCLUDES throw error when no cwd set
++ `#20 <https://github.com/geographika/mappyfile/issues/20>`_ Only the first FORMATOPTION is kept after transform
++ `#19 <https://github.com/geographika/mappyfile/issues/19>`_ IMAGEMODE FEATURE throws parsing error
++ `#18 <https://github.com/geographika/mappyfile/issues/18>`_ CONFIG keyword not capitalised
+
+Older Releases
+++++++++++++++
+
++ 0.2.2 - various fixes to grammar, and allow for alternate comparison operators
++ 0.2.1 - new ``findall`` function, see https://github.com/geographika/mappyfile/pull/12 - thanks @Jenselme
++ 0.2.0 - switch to Lark parser
 + 0.1.0 - initial release
```

### Comparing `mappyfile-1.0.1/docs/client.rst` & `mappyfile-1.0.2/docs/client.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-.. _cli:
-
-Command-line Interface
-======================
-
-mappyfile includes two command line applications, :ref:`client-format` and :ref:`client-validate`. A command line interface (CLI), allows mappyfile 
-to be easily integrated into Continuous Integration (CI) platforms such as Travis and Appveyor, and to automate validation and formatting
-of Mapfiles. 
-
-.. _client-format:
-
-format
-------
-
-The ``format`` command can be used to apply consistent formatting and whitespace to a Mapfile, and to remove comments. 
-It has the same parameters as the :ref:`save <api-save>` function. 
-
-To format ``valid.map`` to a new ``valid_formatted.map`` file using the default formatting settings use the following syntax: 
-
-.. code-block:: bat
-
-    mappyfile format valid.map valid_formatted.map
-
-Other examples are included in the ``help`` documentation for the command, shown below. To display this at the command line run 
-the following: 
-
-.. code-block:: bat
-
-    mappyfile format --help
-
-.. literalinclude:: format.txt
-    :language: console
-
-..
-    echo run from python3 as click in Python2 doesn't pick up the correct terminal size when redirecting to a file
-    mode con:cols=250
-    mappyfile format --help > docs/format.txt
-
-.. _client-validate:
-
-validate
---------
-
-The ``validate`` command can be used to check values used in a Mapfile are valid, by comparing its contents to the Mapfile
-schema. It has the same parameters as the :ref:`validate <api-validate>` function. 
-
-mappyfile also allows validation against different versions of MapServer, for example validating Mapfiles 
-for MapServer 7.0, or for 7.6. 
-
-.. note::
-
-    When using wildcards to search for Mapfiles the Python ``glob`` module is used on Windows. This only searches subfolders
-    that are one level-deep. On Linux wildcards are typically expanded in the shell, so Mapfiles in subfolders of any depth can 
-    be validated. 
-
-If validation errors are encountered in the Mapfile they will be displayed in the console output similar to below:
-
-.. literalinclude:: validation_errors.txt
-    :language: console
-
-Example 1
-+++++++++
-
-To validate all Mapfiles in the ``ms-ogc-workshop`` folder and all subfolders:
-
-.. code-block:: bat
-
-    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
-
-Example 2
-+++++++++
-
-To validate a single Mapfile, without expanding any ``INCLUDE`` directives:
-
-.. code-block:: bat
-
-    mappyfile validate /world.map --no-expand
-
-Example 3
-+++++++++
-
-To validate a Mapfile for version 7.6 of MapServer:
-
-.. code-block:: bat
-
-    mappyfile validate /world.map --version=7.6
-
-To display the command's help text run the following: 
-
-.. code-block:: bat
-
-    mappyfile validate --help
-
-.. literalinclude:: validate.txt
-    :language: console
-
-..
-    echo run from python3 as click in Python2 doesn't pick up the correct terminal size when redirecting to a file
-    mode con:cols=200
-    mappyfile validate --help > docs/validate.txt
-    mappyfile validate C:/Temp/*.map > docs/validation_errors.txt
-
-.. _client-schema:
-
-schema
-------
-
-Save the Mapfile schema to a file. Set the version parameter to output a specific version.
-
-.. code-block:: bat
-
-    mappyfile schema --help
-
-.. literalinclude:: format.txt
+.. _cli:
+
+Command-line Interface
+======================
+
+mappyfile includes two command line applications, :ref:`client-format` and :ref:`client-validate`. A command line interface (CLI), allows mappyfile 
+to be easily integrated into Continuous Integration (CI) platforms such as Travis and Appveyor, and to automate validation and formatting
+of Mapfiles. 
+
+.. _client-format:
+
+format
+------
+
+The ``format`` command can be used to apply consistent formatting and whitespace to a Mapfile, and to remove comments. 
+It has the same parameters as the :ref:`save <api-save>` function. 
+
+To format ``valid.map`` to a new ``valid_formatted.map`` file using the default formatting settings use the following syntax: 
+
+.. code-block:: bat
+
+    mappyfile format valid.map valid_formatted.map
+
+Other examples are included in the ``help`` documentation for the command, shown below. To display this at the command line run 
+the following: 
+
+.. code-block:: bat
+
+    mappyfile format --help
+
+.. literalinclude:: format.txt
+    :language: console
+
+..
+    echo run from python3 as click in Python2 doesn't pick up the correct terminal size when redirecting to a file
+    mode con:cols=250
+    mappyfile format --help > docs/format.txt
+
+.. _client-validate:
+
+validate
+--------
+
+The ``validate`` command can be used to check values used in a Mapfile are valid, by comparing its contents to the Mapfile
+schema. It has the same parameters as the :ref:`validate <api-validate>` function. 
+
+mappyfile also allows validation against different versions of MapServer, for example validating Mapfiles 
+for MapServer 7.0, or for 7.6. 
+
+.. note::
+
+    When using wildcards to search for Mapfiles the Python ``glob`` module is used on Windows. This only searches subfolders
+    that are one level-deep. On Linux wildcards are typically expanded in the shell, so Mapfiles in subfolders of any depth can 
+    be validated. 
+
+If validation errors are encountered in the Mapfile they will be displayed in the console output similar to below:
+
+.. literalinclude:: validation_errors.txt
+    :language: console
+
+Example 1
++++++++++
+
+To validate all Mapfiles in the ``ms-ogc-workshop`` folder and all subfolders:
+
+.. code-block:: bat
+
+    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
+
+Example 2
++++++++++
+
+To validate a single Mapfile, without expanding any ``INCLUDE`` directives:
+
+.. code-block:: bat
+
+    mappyfile validate /world.map --no-expand
+
+Example 3
++++++++++
+
+To validate a Mapfile for version 7.6 of MapServer:
+
+.. code-block:: bat
+
+    mappyfile validate /world.map --version=7.6
+
+To display the command's help text run the following: 
+
+.. code-block:: bat
+
+    mappyfile validate --help
+
+.. literalinclude:: validate.txt
+    :language: console
+
+..
+    echo run from python3 as click in Python2 doesn't pick up the correct terminal size when redirecting to a file
+    mode con:cols=200
+    mappyfile validate --help > docs/validate.txt
+    mappyfile validate C:/Temp/*.map > docs/validation_errors.txt
+
+.. _client-schema:
+
+schema
+------
+
+Save the Mapfile schema to a file. Set the version parameter to output a specific version.
+
+.. code-block:: bat
+
+    mappyfile schema --help
+
+.. literalinclude:: format.txt
     :language: console
```

### Comparing `mappyfile-1.0.1/docs/comments.rst` & `mappyfile-1.0.2/docs/comments.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-Comments
-========
-
-mappyfile can remove or keep Mapfile comments. This page discusses how comments are retained when using mappyfile.
-mappyfile supports both single-line comments starting with a ``#`` and also C-style multi-line comments.
-
-In a Mapfile comments can appear anywhere. That means that in the context of a classic parser (such as lark), 
-a ``COMMENT?`` would have to be added between practically every token. This can be done automatically
-but it will slow down some parsers (like Earley), or possibly complicate others (like LALR), and 
-create a parse-tree that is much harder to process. This means it's much easier to get rid of them at the lexer.
-
-However mappyfile takes a creative approach that makes comments accessible within the tree as a "comment" attribute.
-
-The next sections descibe how comments are stored in the mappyfile Python dictionary structure, and output using
-the pretty-printer. See `test_comments.py <https://github.com/geographika/mappyfile/blob/master/tests/test_comments.py>`_
-for some sample tests.
-
-Attribute Comments
-++++++++++++++++++
-
-Comments will be associated with attribute keys, and stored in a new "__comments__" property
-at its parent level. For example a layer with two properties and two comments such as 
-below:
-
-.. code-block:: mapfile
-
-    LAYER
-        NAME 'Test' # Name comment
-        TYPE POLYGON # Type comment
-    END
-
-will be transformed into the following structure, where the attribute names are used as key in 
-the "__comments__" property:
-
-.. code-block:: json
-
-    {
-        "name": "Test", 
-        "__type__": "layer", 
-        "__comments__": {
-            "type": "Type comment", 
-            "name": "Name comment"
-        }, 
-        "type": "polygon"
-    }
-
-The location of the comment will decide which attribute it is associated with. A comment will 
-always be associated with its preceding attribute. New lines will be ignored, so the Mapfile
-below will produce the same output as above:
-
-.. code-block:: mapfile
-
-    LAYER
-        NAME 'Test' 
-        
-        # Name comment on a new line
-        TYPE POLYGON 
-        
-        # Type comment
-    END
-
-If a comment falls within the middle of an attribute value, it will be removed (even though this seems to be valid within a Mapfile):
-
-.. code-block:: mapfile
-
-        COLOR  255 #comment will be removed
-        0 0
-
-Composite Level Comments
-++++++++++++++++++++++++
-
-Any comments directly before or after a composite typename will be associated with
-the composite type. 
-
-.. code-block:: mapfile
-
-    # Layer comment
-    LAYER
-        NAME 'Test'
-    END
-
-.. code-block:: json
-
-    {
-        "name": "Test", 
-        "__type__": "layer", 
-        "__comments__": {
-            "__type__": "Layer comment"
-        }
-    }
-
-Multiple Comments
-+++++++++++++++++
-
-In both the above cases multiple comments can be stored in a list. This 
-will be the same for multiple attribute comments. 
-
-.. code-block:: mapfile
-
-    # Layer comment 1
-    # Layer comment 2
-    LAYER
-        NAME 'Test'
-    END
-
-.. code-block:: json
-
-    {
-        "name": "Test", 
-        "__type__": "layer", 
-        "__comments__": {
-            "__type__": [
-                "Layer comment 1", 
-                "Layer comment 2"
-            ]
-        }
-    }
-
-Pretty Printing
----------------
-
-How to format lists of comments?
-
-.. code-block:: mapfile
-
-    NAME "Test" # comment 1 comment 2
-
-Associate with an object - put at top of definition?
-
-.. code-block:: mapfile
-
-    # Map comment 1
-    # Map comment 2
-    MAP
-
-    END
-
-    # Layer comment
-    LAYER
-
+Comments
+========
+
+mappyfile can remove or keep Mapfile comments. This page discusses how comments are retained when using mappyfile.
+mappyfile supports both single-line comments starting with a ``#`` and also C-style multi-line comments.
+
+In a Mapfile comments can appear anywhere. That means that in the context of a classic parser (such as lark), 
+a ``COMMENT?`` would have to be added between practically every token. This can be done automatically
+but it will slow down some parsers (like Earley), or possibly complicate others (like LALR), and 
+create a parse-tree that is much harder to process. This means it's much easier to get rid of them at the lexer.
+
+However mappyfile takes a creative approach that makes comments accessible within the tree as a "comment" attribute.
+
+The next sections descibe how comments are stored in the mappyfile Python dictionary structure, and output using
+the pretty-printer. See `test_comments.py <https://github.com/geographika/mappyfile/blob/master/tests/test_comments.py>`_
+for some sample tests.
+
+Attribute Comments
+++++++++++++++++++
+
+Comments will be associated with attribute keys, and stored in a new "__comments__" property
+at its parent level. For example a layer with two properties and two comments such as 
+below:
+
+.. code-block:: mapfile
+
+    LAYER
+        NAME 'Test' # Name comment
+        TYPE POLYGON # Type comment
+    END
+
+will be transformed into the following structure, where the attribute names are used as key in 
+the "__comments__" property:
+
+.. code-block:: json
+
+    {
+        "name": "Test", 
+        "__type__": "layer", 
+        "__comments__": {
+            "type": "Type comment", 
+            "name": "Name comment"
+        }, 
+        "type": "polygon"
+    }
+
+The location of the comment will decide which attribute it is associated with. A comment will 
+always be associated with its preceding attribute. New lines will be ignored, so the Mapfile
+below will produce the same output as above:
+
+.. code-block:: mapfile
+
+    LAYER
+        NAME 'Test' 
+        
+        # Name comment on a new line
+        TYPE POLYGON 
+        
+        # Type comment
+    END
+
+If a comment falls within the middle of an attribute value, it will be removed (even though this seems to be valid within a Mapfile):
+
+.. code-block:: mapfile
+
+        COLOR  255 #comment will be removed
+        0 0
+
+Composite Level Comments
+++++++++++++++++++++++++
+
+Any comments directly before or after a composite typename will be associated with
+the composite type. 
+
+.. code-block:: mapfile
+
+    # Layer comment
+    LAYER
+        NAME 'Test'
+    END
+
+.. code-block:: json
+
+    {
+        "name": "Test", 
+        "__type__": "layer", 
+        "__comments__": {
+            "__type__": "Layer comment"
+        }
+    }
+
+Multiple Comments
++++++++++++++++++
+
+In both the above cases multiple comments can be stored in a list. This 
+will be the same for multiple attribute comments. 
+
+.. code-block:: mapfile
+
+    # Layer comment 1
+    # Layer comment 2
+    LAYER
+        NAME 'Test'
+    END
+
+.. code-block:: json
+
+    {
+        "name": "Test", 
+        "__type__": "layer", 
+        "__comments__": {
+            "__type__": [
+                "Layer comment 1", 
+                "Layer comment 2"
+            ]
+        }
+    }
+
+Pretty Printing
+---------------
+
+How to format lists of comments?
+
+.. code-block:: mapfile
+
+    NAME "Test" # comment 1 comment 2
+
+Associate with an object - put at top of definition?
+
+.. code-block:: mapfile
+
+    # Map comment 1
+    # Map comment 2
+    MAP
+
+    END
+
+    # Layer comment
+    LAYER
+
     END
```

### Comparing `mappyfile-1.0.1/docs/conf.py` & `mappyfile-1.0.2/docs/conf.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,592 +1,592 @@
-# -*- coding: utf-8 -*-
-#
-# mappyfile documentation build configuration file, created by
-# sphinx-quickstart on Fri Jan 13 00:17:15 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
-
-import mappyfile
-
-import re
-from pygments.lexer import RegexLexer, combined, include
-from pygments.token import (
-    Text,
-    Punctuation,
-    Generic,
-    Keyword,
-    Name,
-    Number,
-    String,
-    Comment,
-    Operator,
-)
-
-# -- General configuration ------------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.napoleon"]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = ".rst"
-
-# The encoding of source files.
-#
-# source_encoding = 'utf-8-sig'
-
-# The master toctree document.
-master_doc = "index"
-
-# General information about the project.
-project = "mappyfile"
-copyright = "2023, Seth Girvin"
-author = "Seth Girvin"
-
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-#
-# The short X.Y version.
-version = mappyfile.__version__
-# The full version, including alpha/beta/rc tags.
-release = mappyfile.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = "en"
-
-# There are two options for replacing |today|: either, you set today to some
-# non-false value, then it is used:
-#
-# today = ''
-#
-# Else, today_fmt is used as the format for a strftime call.
-#
-# today_fmt = '%B %d, %Y'
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
-
-# The reST default role (used for this markup: `text`) to use for all
-# documents.
-#
-# default_role = None
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-#
-# add_function_parentheses = True
-
-# If true, the current module name will be prepended to all description
-# unit titles (such as .. function::).
-#
-# add_module_names = True
-
-# If true, sectionauthor and moduleauthor directives will be shown in the
-# output. They are ignored by default.
-#
-# show_authors = False
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-# A list of ignored prefixes for module index sorting.
-# modindex_common_prefix = []
-
-# If true, keep warnings as "system message" paragraphs in the built documents.
-# keep_warnings = False
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output ----------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = "alabaster"
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom themes here, relative to this directory.
-# html_theme_path = []
-
-# The name for this set of Sphinx documents.
-# "<project> v<release> documentation" by default.
-#
-# html_title = u'mappyfile v0.1'
-
-# A shorter title for the navigation bar.  Default is the same as html_title.
-#
-# html_short_title = None
-
-# The name of an image file (relative to this directory) to place at the top
-# of the sidebar.
-#
-# html_logo = None
-
-# The name of an image file (relative to this directory) to use as a favicon of
-# the docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
-# pixels large.
-#
-# html_favicon = None
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
-
-# Add any extra paths that contain custom files (such as robots.txt or
-# .htaccess) here, relative to this directory. These files are copied
-# directly to the root of the documentation.
-#
-# html_extra_path = []
-
-# If not None, a 'Last updated on:' timestamp is inserted at every page
-# bottom, using the given strftime format.
-# The empty string is equivalent to '%b %d, %Y'.
-#
-# html_last_updated_fmt = None
-
-# If true, SmartyPants will be used to convert quotes and dashes to
-# typographically correct entities.
-#
-# html_use_smartypants = True
-
-# Custom sidebar templates, maps document names to template names.
-#
-# html_sidebars = {'**': ['globaltoc.html','searchbox.html','localtoc.html','relations.html']}
-#
-
-html_logo = "images/roll-36697_640.png"
-
-html_theme_options = {
-    # 'logo': 'images/roll-36697_640.png',
-    "page_width": "70%",
-    "github_user": "geographika",
-    "github_repo": "mappyfile",
-    "github_button": True,
-    "github_banner": False,  # currently broken see https://github.com/sphinx-doc/alabaster/issues/208
-    "github_type": "star",
-}
-
-
-# Additional templates that should be rendered to pages, maps page names to
-# template names.
-#
-# html_additional_pages = {}
-
-# If false, no module index is generated.
-#
-# html_domain_indices = True
-
-# If false, no index is generated.
-#
-# html_use_index = True
-
-# If true, the index is split into individual pages for each letter.
-#
-# html_split_index = False
-
-# If true, links to the reST sources are added to the pages.
-#
-# html_show_sourcelink = True
-
-# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#
-# html_show_sphinx = True
-
-# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#
-# html_show_copyright = True
-
-# If true, an OpenSearch description file will be output, and all pages will
-# contain a <link> tag referring to it.  The value of this option must be the
-# base URL from which the finished HTML is served.
-#
-# html_use_opensearch = ''
-
-# This is the file name suffix for HTML files (e.g. ".xhtml").
-# html_file_suffix = None
-
-# Language to be used for generating the HTML full-text search index.
-# Sphinx supports the following languages:
-#   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
-#   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr', 'zh'
-#
-# html_search_language = 'en'
-
-# A dictionary with options for the search language support, empty by default.
-# 'ja' uses this config value.
-# 'zh' user can custom change `jieba` dictionary path.
-#
-# html_search_options = {'type': 'default'}
-
-# The name of a javascript file (relative to the configuration directory) that
-# implements a search results scorer. If empty, the default will be used.
-#
-# html_search_scorer = 'scorer.js'
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = "mappyfiledoc"
-
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, "mappyfile.tex", "mappyfile Documentation", "S Girvin", "manual"),
-]
-
-# The name of an image file (relative to this directory) to place at the top of
-# the title page.
-#
-# latex_logo = None
-
-# For "manual" documents, if this is true, then toplevel headings are parts,
-# not chapters.
-#
-# latex_use_parts = False
-
-# If true, show page references after internal links.
-#
-# latex_show_pagerefs = False
-
-# If true, show URL addresses after external links.
-#
-# latex_show_urls = False
-
-# Documents to append as an appendix to all manuals.
-#
-# latex_appendices = []
-
-# It false, will not define \strong, \code, 	itleref, \crossref ... but only
-# \sphinxstrong, ..., \sphinxtitleref, ... To help avoid clash with user added
-# packages.
-#
-# latex_keep_old_macro_names = True
-
-# If false, no module index is generated.
-#
-# latex_domain_indices = True
-
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "mappyfile", "mappyfile Documentation", [author], 1)]
-
-# If true, show URL addresses after external links.
-#
-# man_show_urls = False
-
-
-# -- Options for Texinfo output -------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "mappyfile",
-        "mappyfile Documentation",
-        author,
-        "mappyfile",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
-
-# Documents to append as an appendix to all manuals.
-#
-# texinfo_appendices = []
-
-# If false, no module index is generated.
-#
-# texinfo_domain_indices = True
-
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-#
-# texinfo_show_urls = 'footnote'
-
-# If true, do not generate a @detailmenu in the "Top" node's menu.
-#
-# texinfo_no_detailmenu = False
-
-
-# -- Options for Epub output ----------------------------------------------
-
-# Bibliographic Dublin Core info.
-epub_title = project
-epub_author = author
-epub_publisher = author
-epub_copyright = copyright
-
-# The basename for the epub file. It defaults to the project name.
-# epub_basename = project
-
-# The HTML theme for the epub output. Since the default themes are not
-# optimized for small screen space, using the same theme for HTML and epub
-# output is usually not wise. This defaults to 'epub', a theme designed to save
-# visual space.
-#
-# epub_theme = 'epub'
-
-# The language of the text. It defaults to the language option
-# or 'en' if the language is not set.
-#
-# epub_language = ''
-
-# The scheme of the identifier. Typical schemes are ISBN or URL.
-# epub_scheme = ''
-
-# The unique identifier of the text. This can be a ISBN number
-# or the project homepage.
-#
-# epub_identifier = ''
-
-# A unique identification for the text.
-#
-# epub_uid = ''
-
-# A tuple containing the cover image and cover page html template filenames.
-#
-# epub_cover = ()
-
-# A sequence of (type, uri, title) tuples for the guide element of content.opf.
-#
-# epub_guide = ()
-
-# HTML files that should be inserted before the pages created by sphinx.
-# The format is a list of tuples containing the path and title.
-#
-# epub_pre_files = []
-
-# HTML files that should be inserted after the pages created by sphinx.
-# The format is a list of tuples containing the path and title.
-#
-# epub_post_files = []
-
-# A list of files that should not be packed into the epub file.
-epub_exclude_files = ["search.html"]
-
-# The depth of the table of contents in toc.ncx.
-#
-# epub_tocdepth = 3
-
-# Allow duplicate toc entries.
-#
-# epub_tocdup = True
-
-# Choose between 'default' and 'includehidden'.
-#
-# epub_tocscope = 'default'
-
-# Fix unsupported image types using the Pillow.
-#
-# epub_fix_images = False
-
-# Scale large images.
-#
-# epub_max_image_width = 0
-
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-#
-# epub_show_urls = 'inline'
-
-# If false, no index is generated.
-#
-# epub_use_index = True
-
-
-class WKTLexer(RegexLexer):
-    name = "wkt"
-    aliases = ["wkt"]
-    filenames = ["*.wkt"]
-
-    tokens = {
-        "root": [
-            (r"\s+", Text),
-            (r"[{}\[\]();,-.]+", Punctuation),
-            (r"(PROJCS)\b", Generic.Heading),
-            (r"(PARAMETER|PROJECTION|SPHEROID|DATUM|GEOGCS|AXIS)\b", Keyword),
-            (r"(PRIMEM|UNIT|TOWGS84)\b", Keyword.Constant),
-            (r"(AUTHORITY)\b", Name.Builtin),
-            (r"[$a-zA-Z_][a-zA-Z0-9_]*", Name.Other),
-            (r"[0-9][0-9]*\.[0-9]+([eE][0-9]+)?[fd]?", Number.Float),
-            (r"0x[0-9a-fA-F]+", Number.Hex),
-            (r"[0-9]+", Number.Integer),
-            (r'"(\\\\|\\"|[^"])*"', String.Double),
-            (r"'(\\\\|\\'|[^'])*'", String.Single),
-        ]
-    }
-
-
-builtins = (
-    r"(ANNOTATION|"
-    r"AUTO|BEVEL|BITMAP|BUTT|CARTOLINE|CC|CENTER|"
-    r"CHART|CIRCLE|CL|CONTOUR|CR|CSV|"
-    r"DEFAULT|DD|ELLIPSE|EMBED|FALSE|FEET|FOLLOW|"
-    r"GIANT|HATCH|HILITE|INCHES|KERNELDENSITY|KILOMETERS|LARGE|LC|"
-    r"LEFT|LINE|LL|LOCAL|LR|MEDIUM|METERS|MILES|MITER|MULTIPLE|MYGIS|MYSQL|NONE|"
-    r"NORMAL|OFF|OGR|ON|ONE-TO-ONE|ONE-TO-MANY|ORACLESPATIAL|"
-    r"PERCENTAGES|PIXMAP|PIXELS|POINT|POLYGON|POSTGIS|POSTGRESQL|"
-    r"PLUGIN|QUERY|RASTER|RIGHT|ROUND|SDE|SELECTED|SIMPLE|SINGLE|"
-    r"SMALL|SQUARE|TINY|TRIANGLE|TRUE|TRUETYPE|UC|UL|UNION|UR|UV_ANGLE|UV_MINUS_ANGLE|UV_LENGTH|UV_LENGTH_2|UVRASTER|VECTOR|"
-    r"WFS|WMS|ALPHA|"
-    r"GIF|JPEG|JPG|PNG|WBMP|SWF|PDF|GTIFF|PC256|RGB|RGBA|INT16|FLOAT32|GD|"
-    r"AGG|CAIRO|PNG8|SVG|KML|KMZ|GDAL|UTFGRID"
-    r")\b"
-)
-
-keywords = (
-    r"(ALIGN|"
-    r"ALPHACOLOR|ANCHORPOINT|ANGLE|ANTIALIAS|AUTHOR|BACKGROUNDCOLOR|BACKGROUNDSHADOWCOLOR|"
-    r"BACKGROUNDSHADOWSIZE|BANDSITEM|BROWSEFORMAT|BUFFER|CHARACTER|CLASS|CLASSITEM|"
-    r"CLASSGROUP|CLUSTER|COLOR|COLORRANGE|COMPOSITE|COMPOP|COMPFILTER|CONFIG|CONNECTION|CONNECTIONOPTIONS|CONNECTIONTYPE|DATA|DATAPATTERN|DATARANGE|DEBUG|"
-    r"DRIVER|DUMP|EMPTY|ENCODING|END|ERROR|EXPRESSION|EXTENT|EXTENSION|FEATURE|"
-    r"FILLED|FILTER|FILTERITEM|FOOTER|FONT|FONTSET|FORCE|FORMATOPTION|FROM|GAP|GEOMTRANSFORM|"
-    r"GRID|GRIDSTEP|GRATICULE|GROUP|HEADER|IMAGE|IMAGECOLOR|IMAGETYPE|IMAGEQUALITY|IMAGEPATH|"
-    r"IMAGEURL|INCLUDE|INDEX|INITIALGAP|INTERLACE|INTERVALS|JOIN|KEYIMAGE|KEYSIZE|KEYSPACING|LABEL|"
-    r"LABELCACHE|LABELFORMAT|LABELITEM|LABELMAXSCALE|LABELMAXSCALEDENOM|"
-    r"LABELMINSCALE|LABELMINSCALEDENOM|LABELREQUIRES|LATLON|LAYER|LEADER|LEGEND|"
-    r"LEGENDFORMAT|LINECAP|LINEJOIN|LINEJOINMAXSIZE|LOG|MAP|MARKER|MARKERSIZE|"
-    r"MASK|MAXARCS|MAXBOXSIZE|MAXDISTANCE|MAXFEATURES|MAXINTERVAL|MAXSCALE|MAXSCALEDENOM|MINSCALE|"
-    r"MINSCALEDENOM|MAXGEOWIDTH|MAXLENGTH|MAXSIZE|MAXSUBDIVIDE|MAXTEMPLATE|"
-    r"MAXWIDTH|METADATA|MIMETYPE|MINARCS|MINBOXSIZE|MINDISTANCE|"
-    r"MINFEATURESIZE|MININTERVAL|MINSCALE|MINSCALEDENOM|MINGEOWIDTH"
-    r"MINLENGTH|MINSIZE|MINSUBDIVIDE|MINTEMPLATE|MINWIDTH|NAME|OFFSET|OFFSITE|"
-    r"OPACITY|OUTLINECOLOR|OUTLINEWIDTH|OUTPUTFORMAT|OVERLAYBACKGROUNDCOLOR|"
-    r"OVERLAYCOLOR|OVERLAYMAXSIZE|OVERLAYMINSIZE|OVERLAYOUTLINECOLOR|"
-    r"OVERLAYSIZE|OVERLAYSYMBOL|PARTIALS|PATTERN|POINTS|POLAROFFSET|POSITION|POSTLABELCACHE|"
-    r"PRIORITY|PROCESSING|PROJECTION|QUERYFORMAT|QUERYMAP|REFERENCE|REGION|"
-    r"RELATIVETO|REQUIRES|RESOLUTION|SCALE|SCALEDENOM|SCALETOKEN|SHADOWCOLOR|SHADOWSIZE|"
-    r"SHAPEPATH|SIZE|SIZEUNITS|STATUS|STYLE|STYLEITEM|SYMBOL|SYMBOLSCALE|"
-    r"SYMBOLSCALEDENOM|SYMBOLSET|TABLE|TEMPLATE|TEMPLATEPATTERN|TEXT|"
-    r"TILEINDEX|TILEITEM|TILESRS|TITLE|TO|TOLERANCE|TOLERANCEUNITS|TRANSPARENCY|"
-    r"TRANSPARENT|TRANSFORM|TYPE|UNITS|UTFDATA|UTFITEM|WEB|WIDTH|WKT|WRAP|IMAGEMODE|VALIDATION|VALUES"
-    r")\b"
-)
-
-
-class MapFileLexer(RegexLexer):
-    name = "mapfile"
-    aliases = ["mapfile"]
-    filenames = ["*.map"]
-
-    flags = re.IGNORECASE
-    tokens = {
-        "root": [
-            (r"\s+", Text),
-            (r"\[.*?\]", Name.Other),
-            (r"[{}\[\]();,-.]+", Punctuation),
-            (r"#.*", Comment),
-            (r"(AND|OR|NOT|EQ|GT|LT|GE|LE|NE|IN|IEQ)\b", Operator.Word),
-            (r"!=|==|<=|>=|=~|&&|\|\||[-~+/*%=<>&^|./\$]", Operator),
-            ('(?:[rR]|[uU][rR]|[rR][uU])"', String, "dqs"),
-            ("(?:[rR]|[uU][rR]|[rR][uU])'", String, "sqs"),
-            (r"`([^`])*`", Number.Date),
-            ('[uU]?"', String, combined("stringescape", "dqs")),
-            ("[uU]?'", String, combined("stringescape", "sqs")),
-            #            (constants, Keyword.Constant),
-            #            (r"""[]{}:(),;[]""", Punctuation),
-            # (r'(MAP)\b', Generic.Heading),
-            (keywords, Keyword),
-            (builtins, Name.Builtin),
-            (r"[0-9][0-9]*\.[0-9]+([eE][0-9]+)?[fd]?", Number.Float),
-            (r"[0-9]+", Number.Integer),
-        ],
-        "dqs": [
-            (r'"', String, "#pop"),
-            (r'\\\\|\\"|\\\n', String.Escape),  # included here again for raw strings
-            include("strings"),
-        ],
-        "sqs": [
-            (r"'", String, "#pop"),
-            (r"\\\\|\\'|\\\n", String.Escape),  # included here again for raw strings
-            include("strings"),
-        ],
-        "tdqs": [(r'"""', String, "#pop"), include("strings"), include("nl")],
-        "tsqs": [(r"'''", String, "#pop"), include("strings"), include("nl")],
-        "strings": [
-            (
-                r"%(\([a-zA-Z0-9_]+\))?[-#0 +]*([0-9]+|[*])?(\.([0-9]+|[*]))?"
-                "[hlL]?[diouxXeEfFgGcrs%]",
-                String.Interpol,
-            ),
-            (r'[^\\\'"%\n]+', String),
-            # quotes, percents and backslashes must be parsed one at a time
-            (r'[\'"\\]', String),
-            # unhandled string formatting sign
-            (r"%", String)
-            # newlines are an error (use "nl" state)
-        ],
-        "nl": [(r"\n", String)],
-        "stringescape": [
-            (
-                r'\\([\\abfnrtv"\']|\n|N{.*?}|u[a-fA-F0-9]{4}|'
-                r"U[a-fA-F0-9]{8}|x[a-fA-F0-9]{2}|[0-7]{1,3})",
-                String.Escape,
-            )
-        ],
-    }
-
-
-def setup(app):
-    from sphinx.highlighting import lexers
-
-    lexers["wkt"] = WKTLexer()
-    lexers["mapfile"] = MapFileLexer()
+# -*- coding: utf-8 -*-
+#
+# mappyfile documentation build configuration file, created by
+# sphinx-quickstart on Fri Jan 13 00:17:15 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+#
+# import os
+# import sys
+# sys.path.insert(0, os.path.abspath('.'))
+
+import mappyfile
+
+import re
+from pygments.lexer import RegexLexer, combined, include
+from pygments.token import (
+    Text,
+    Punctuation,
+    Generic,
+    Keyword,
+    Name,
+    Number,
+    String,
+    Comment,
+    Operator,
+)
+
+# -- General configuration ------------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.napoleon"]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = ".rst"
+
+# The encoding of source files.
+#
+# source_encoding = 'utf-8-sig'
+
+# The master toctree document.
+master_doc = "index"
+
+# General information about the project.
+project = "mappyfile"
+copyright = "2023, Seth Girvin"
+author = "Seth Girvin"
+
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+#
+# The short X.Y version.
+version = mappyfile.__version__
+# The full version, including alpha/beta/rc tags.
+release = mappyfile.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = "en"
+
+# There are two options for replacing |today|: either, you set today to some
+# non-false value, then it is used:
+#
+# today = ''
+#
+# Else, today_fmt is used as the format for a strftime call.
+#
+# today_fmt = '%B %d, %Y'
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+
+# The reST default role (used for this markup: `text`) to use for all
+# documents.
+#
+# default_role = None
+
+# If true, '()' will be appended to :func: etc. cross-reference text.
+#
+# add_function_parentheses = True
+
+# If true, the current module name will be prepended to all description
+# unit titles (such as .. function::).
+#
+# add_module_names = True
+
+# If true, sectionauthor and moduleauthor directives will be shown in the
+# output. They are ignored by default.
+#
+# show_authors = False
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# A list of ignored prefixes for module index sorting.
+# modindex_common_prefix = []
+
+# If true, keep warnings as "system message" paragraphs in the built documents.
+# keep_warnings = False
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output ----------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = "alabaster"
+
+# Theme options are theme-specific and customize the look and feel of a theme
+# further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom themes here, relative to this directory.
+# html_theme_path = []
+
+# The name for this set of Sphinx documents.
+# "<project> v<release> documentation" by default.
+#
+# html_title = u'mappyfile v0.1'
+
+# A shorter title for the navigation bar.  Default is the same as html_title.
+#
+# html_short_title = None
+
+# The name of an image file (relative to this directory) to place at the top
+# of the sidebar.
+#
+# html_logo = None
+
+# The name of an image file (relative to this directory) to use as a favicon of
+# the docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
+# pixels large.
+#
+# html_favicon = None
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+# Add any extra paths that contain custom files (such as robots.txt or
+# .htaccess) here, relative to this directory. These files are copied
+# directly to the root of the documentation.
+#
+# html_extra_path = []
+
+# If not None, a 'Last updated on:' timestamp is inserted at every page
+# bottom, using the given strftime format.
+# The empty string is equivalent to '%b %d, %Y'.
+#
+# html_last_updated_fmt = None
+
+# If true, SmartyPants will be used to convert quotes and dashes to
+# typographically correct entities.
+#
+# html_use_smartypants = True
+
+# Custom sidebar templates, maps document names to template names.
+#
+# html_sidebars = {'**': ['globaltoc.html','searchbox.html','localtoc.html','relations.html']}
+#
+
+html_logo = "images/roll-36697_640.png"
+
+html_theme_options = {
+    # 'logo': 'images/roll-36697_640.png',
+    "page_width": "70%",
+    "github_user": "geographika",
+    "github_repo": "mappyfile",
+    "github_button": True,
+    "github_banner": False,  # currently broken see https://github.com/sphinx-doc/alabaster/issues/208
+    "github_type": "star",
+}
+
+
+# Additional templates that should be rendered to pages, maps page names to
+# template names.
+#
+# html_additional_pages = {}
+
+# If false, no module index is generated.
+#
+# html_domain_indices = True
+
+# If false, no index is generated.
+#
+# html_use_index = True
+
+# If true, the index is split into individual pages for each letter.
+#
+# html_split_index = False
+
+# If true, links to the reST sources are added to the pages.
+#
+# html_show_sourcelink = True
+
+# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
+#
+# html_show_sphinx = True
+
+# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
+#
+# html_show_copyright = True
+
+# If true, an OpenSearch description file will be output, and all pages will
+# contain a <link> tag referring to it.  The value of this option must be the
+# base URL from which the finished HTML is served.
+#
+# html_use_opensearch = ''
+
+# This is the file name suffix for HTML files (e.g. ".xhtml").
+# html_file_suffix = None
+
+# Language to be used for generating the HTML full-text search index.
+# Sphinx supports the following languages:
+#   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
+#   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr', 'zh'
+#
+# html_search_language = 'en'
+
+# A dictionary with options for the search language support, empty by default.
+# 'ja' uses this config value.
+# 'zh' user can custom change `jieba` dictionary path.
+#
+# html_search_options = {'type': 'default'}
+
+# The name of a javascript file (relative to the configuration directory) that
+# implements a search results scorer. If empty, the default will be used.
+#
+# html_search_scorer = 'scorer.js'
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = "mappyfiledoc"
+
+# -- Options for LaTeX output ---------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title,
+#  author, documentclass [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, "mappyfile.tex", "mappyfile Documentation", "S Girvin", "manual"),
+]
+
+# The name of an image file (relative to this directory) to place at the top of
+# the title page.
+#
+# latex_logo = None
+
+# For "manual" documents, if this is true, then toplevel headings are parts,
+# not chapters.
+#
+# latex_use_parts = False
+
+# If true, show page references after internal links.
+#
+# latex_show_pagerefs = False
+
+# If true, show URL addresses after external links.
+#
+# latex_show_urls = False
+
+# Documents to append as an appendix to all manuals.
+#
+# latex_appendices = []
+
+# It false, will not define \strong, \code, 	itleref, \crossref ... but only
+# \sphinxstrong, ..., \sphinxtitleref, ... To help avoid clash with user added
+# packages.
+#
+# latex_keep_old_macro_names = True
+
+# If false, no module index is generated.
+#
+# latex_domain_indices = True
+
+
+# -- Options for manual page output ---------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [(master_doc, "mappyfile", "mappyfile Documentation", [author], 1)]
+
+# If true, show URL addresses after external links.
+#
+# man_show_urls = False
+
+
+# -- Options for Texinfo output -------------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (
+        master_doc,
+        "mappyfile",
+        "mappyfile Documentation",
+        author,
+        "mappyfile",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
+]
+
+# Documents to append as an appendix to all manuals.
+#
+# texinfo_appendices = []
+
+# If false, no module index is generated.
+#
+# texinfo_domain_indices = True
+
+# How to display URL addresses: 'footnote', 'no', or 'inline'.
+#
+# texinfo_show_urls = 'footnote'
+
+# If true, do not generate a @detailmenu in the "Top" node's menu.
+#
+# texinfo_no_detailmenu = False
+
+
+# -- Options for Epub output ----------------------------------------------
+
+# Bibliographic Dublin Core info.
+epub_title = project
+epub_author = author
+epub_publisher = author
+epub_copyright = copyright
+
+# The basename for the epub file. It defaults to the project name.
+# epub_basename = project
+
+# The HTML theme for the epub output. Since the default themes are not
+# optimized for small screen space, using the same theme for HTML and epub
+# output is usually not wise. This defaults to 'epub', a theme designed to save
+# visual space.
+#
+# epub_theme = 'epub'
+
+# The language of the text. It defaults to the language option
+# or 'en' if the language is not set.
+#
+# epub_language = ''
+
+# The scheme of the identifier. Typical schemes are ISBN or URL.
+# epub_scheme = ''
+
+# The unique identifier of the text. This can be a ISBN number
+# or the project homepage.
+#
+# epub_identifier = ''
+
+# A unique identification for the text.
+#
+# epub_uid = ''
+
+# A tuple containing the cover image and cover page html template filenames.
+#
+# epub_cover = ()
+
+# A sequence of (type, uri, title) tuples for the guide element of content.opf.
+#
+# epub_guide = ()
+
+# HTML files that should be inserted before the pages created by sphinx.
+# The format is a list of tuples containing the path and title.
+#
+# epub_pre_files = []
+
+# HTML files that should be inserted after the pages created by sphinx.
+# The format is a list of tuples containing the path and title.
+#
+# epub_post_files = []
+
+# A list of files that should not be packed into the epub file.
+epub_exclude_files = ["search.html"]
+
+# The depth of the table of contents in toc.ncx.
+#
+# epub_tocdepth = 3
+
+# Allow duplicate toc entries.
+#
+# epub_tocdup = True
+
+# Choose between 'default' and 'includehidden'.
+#
+# epub_tocscope = 'default'
+
+# Fix unsupported image types using the Pillow.
+#
+# epub_fix_images = False
+
+# Scale large images.
+#
+# epub_max_image_width = 0
+
+# How to display URL addresses: 'footnote', 'no', or 'inline'.
+#
+# epub_show_urls = 'inline'
+
+# If false, no index is generated.
+#
+# epub_use_index = True
+
+
+class WKTLexer(RegexLexer):
+    name = "wkt"
+    aliases = ["wkt"]
+    filenames = ["*.wkt"]
+
+    tokens = {
+        "root": [
+            (r"\s+", Text),
+            (r"[{}\[\]();,-.]+", Punctuation),
+            (r"(PROJCS)\b", Generic.Heading),
+            (r"(PARAMETER|PROJECTION|SPHEROID|DATUM|GEOGCS|AXIS)\b", Keyword),
+            (r"(PRIMEM|UNIT|TOWGS84)\b", Keyword.Constant),
+            (r"(AUTHORITY)\b", Name.Builtin),
+            (r"[$a-zA-Z_][a-zA-Z0-9_]*", Name.Other),
+            (r"[0-9][0-9]*\.[0-9]+([eE][0-9]+)?[fd]?", Number.Float),
+            (r"0x[0-9a-fA-F]+", Number.Hex),
+            (r"[0-9]+", Number.Integer),
+            (r'"(\\\\|\\"|[^"])*"', String.Double),
+            (r"'(\\\\|\\'|[^'])*'", String.Single),
+        ]
+    }
+
+
+builtins = (
+    r"(ANNOTATION|"
+    r"AUTO|BEVEL|BITMAP|BUTT|CARTOLINE|CC|CENTER|"
+    r"CHART|CIRCLE|CL|CONTOUR|CR|CSV|"
+    r"DEFAULT|DD|ELLIPSE|EMBED|FALSE|FEET|FOLLOW|"
+    r"GIANT|HATCH|HILITE|INCHES|KERNELDENSITY|KILOMETERS|LARGE|LC|"
+    r"LEFT|LINE|LL|LOCAL|LR|MEDIUM|METERS|MILES|MITER|MULTIPLE|MYGIS|MYSQL|NONE|"
+    r"NORMAL|OFF|OGR|ON|ONE-TO-ONE|ONE-TO-MANY|ORACLESPATIAL|"
+    r"PERCENTAGES|PIXMAP|PIXELS|POINT|POLYGON|POSTGIS|POSTGRESQL|"
+    r"PLUGIN|QUERY|RASTER|RIGHT|ROUND|SDE|SELECTED|SIMPLE|SINGLE|"
+    r"SMALL|SQUARE|TINY|TRIANGLE|TRUE|TRUETYPE|UC|UL|UNION|UR|UV_ANGLE|UV_MINUS_ANGLE|UV_LENGTH|UV_LENGTH_2|UVRASTER|VECTOR|"
+    r"WFS|WMS|ALPHA|"
+    r"GIF|JPEG|JPG|PNG|WBMP|SWF|PDF|GTIFF|PC256|RGB|RGBA|INT16|FLOAT32|GD|"
+    r"AGG|CAIRO|PNG8|SVG|KML|KMZ|GDAL|UTFGRID"
+    r")\b"
+)
+
+keywords = (
+    r"(ALIGN|"
+    r"ALPHACOLOR|ANCHORPOINT|ANGLE|ANTIALIAS|AUTHOR|BACKGROUNDCOLOR|BACKGROUNDSHADOWCOLOR|"
+    r"BACKGROUNDSHADOWSIZE|BANDSITEM|BROWSEFORMAT|BUFFER|CHARACTER|CLASS|CLASSITEM|"
+    r"CLASSGROUP|CLUSTER|COLOR|COLORRANGE|COMPOSITE|COMPOP|COMPFILTER|CONFIG|CONNECTION|CONNECTIONOPTIONS|CONNECTIONTYPE|DATA|DATAPATTERN|DATARANGE|DEBUG|"
+    r"DRIVER|DUMP|EMPTY|ENCODING|END|ERROR|EXPRESSION|EXTENT|EXTENSION|FEATURE|"
+    r"FILLED|FILTER|FILTERITEM|FOOTER|FONT|FONTSET|FORCE|FORMATOPTION|FROM|GAP|GEOMTRANSFORM|"
+    r"GRID|GRIDSTEP|GRATICULE|GROUP|HEADER|IMAGE|IMAGECOLOR|IMAGETYPE|IMAGEQUALITY|IMAGEPATH|"
+    r"IMAGEURL|INCLUDE|INDEX|INITIALGAP|INTERLACE|INTERVALS|JOIN|KEYIMAGE|KEYSIZE|KEYSPACING|LABEL|"
+    r"LABELCACHE|LABELFORMAT|LABELITEM|LABELMAXSCALE|LABELMAXSCALEDENOM|"
+    r"LABELMINSCALE|LABELMINSCALEDENOM|LABELREQUIRES|LATLON|LAYER|LEADER|LEGEND|"
+    r"LEGENDFORMAT|LINECAP|LINEJOIN|LINEJOINMAXSIZE|LOG|MAP|MARKER|MARKERSIZE|"
+    r"MASK|MAXARCS|MAXBOXSIZE|MAXDISTANCE|MAXFEATURES|MAXINTERVAL|MAXSCALE|MAXSCALEDENOM|MINSCALE|"
+    r"MINSCALEDENOM|MAXGEOWIDTH|MAXLENGTH|MAXSIZE|MAXSUBDIVIDE|MAXTEMPLATE|"
+    r"MAXWIDTH|METADATA|MIMETYPE|MINARCS|MINBOXSIZE|MINDISTANCE|"
+    r"MINFEATURESIZE|MININTERVAL|MINSCALE|MINSCALEDENOM|MINGEOWIDTH"
+    r"MINLENGTH|MINSIZE|MINSUBDIVIDE|MINTEMPLATE|MINWIDTH|NAME|OFFSET|OFFSITE|"
+    r"OPACITY|OUTLINECOLOR|OUTLINEWIDTH|OUTPUTFORMAT|OVERLAYBACKGROUNDCOLOR|"
+    r"OVERLAYCOLOR|OVERLAYMAXSIZE|OVERLAYMINSIZE|OVERLAYOUTLINECOLOR|"
+    r"OVERLAYSIZE|OVERLAYSYMBOL|PARTIALS|PATTERN|POINTS|POLAROFFSET|POSITION|POSTLABELCACHE|"
+    r"PRIORITY|PROCESSING|PROJECTION|QUERYFORMAT|QUERYMAP|REFERENCE|REGION|"
+    r"RELATIVETO|REQUIRES|RESOLUTION|SCALE|SCALEDENOM|SCALETOKEN|SHADOWCOLOR|SHADOWSIZE|"
+    r"SHAPEPATH|SIZE|SIZEUNITS|STATUS|STYLE|STYLEITEM|SYMBOL|SYMBOLSCALE|"
+    r"SYMBOLSCALEDENOM|SYMBOLSET|TABLE|TEMPLATE|TEMPLATEPATTERN|TEXT|"
+    r"TILEINDEX|TILEITEM|TILESRS|TITLE|TO|TOLERANCE|TOLERANCEUNITS|TRANSPARENCY|"
+    r"TRANSPARENT|TRANSFORM|TYPE|UNITS|UTFDATA|UTFITEM|WEB|WIDTH|WKT|WRAP|IMAGEMODE|VALIDATION|VALUES"
+    r")\b"
+)
+
+
+class MapFileLexer(RegexLexer):
+    name = "mapfile"
+    aliases = ["mapfile"]
+    filenames = ["*.map"]
+
+    flags = re.IGNORECASE
+    tokens = {
+        "root": [
+            (r"\s+", Text),
+            (r"\[.*?\]", Name.Other),
+            (r"[{}\[\]();,-.]+", Punctuation),
+            (r"#.*", Comment),
+            (r"(AND|OR|NOT|EQ|GT|LT|GE|LE|NE|IN|IEQ)\b", Operator.Word),
+            (r"!=|==|<=|>=|=~|&&|\|\||[-~+/*%=<>&^|./\$]", Operator),
+            ('(?:[rR]|[uU][rR]|[rR][uU])"', String, "dqs"),
+            ("(?:[rR]|[uU][rR]|[rR][uU])'", String, "sqs"),
+            (r"`([^`])*`", Number.Date),
+            ('[uU]?"', String, combined("stringescape", "dqs")),
+            ("[uU]?'", String, combined("stringescape", "sqs")),
+            #            (constants, Keyword.Constant),
+            #            (r"""[]{}:(),;[]""", Punctuation),
+            # (r'(MAP)\b', Generic.Heading),
+            (keywords, Keyword),
+            (builtins, Name.Builtin),
+            (r"[0-9][0-9]*\.[0-9]+([eE][0-9]+)?[fd]?", Number.Float),
+            (r"[0-9]+", Number.Integer),
+        ],
+        "dqs": [
+            (r'"', String, "#pop"),
+            (r'\\\\|\\"|\\\n', String.Escape),  # included here again for raw strings
+            include("strings"),
+        ],
+        "sqs": [
+            (r"'", String, "#pop"),
+            (r"\\\\|\\'|\\\n", String.Escape),  # included here again for raw strings
+            include("strings"),
+        ],
+        "tdqs": [(r'"""', String, "#pop"), include("strings"), include("nl")],
+        "tsqs": [(r"'''", String, "#pop"), include("strings"), include("nl")],
+        "strings": [
+            (
+                r"%(\([a-zA-Z0-9_]+\))?[-#0 +]*([0-9]+|[*])?(\.([0-9]+|[*]))?"
+                "[hlL]?[diouxXeEfFgGcrs%]",
+                String.Interpol,
+            ),
+            (r'[^\\\'"%\n]+', String),
+            # quotes, percents and backslashes must be parsed one at a time
+            (r'[\'"\\]', String),
+            # unhandled string formatting sign
+            (r"%", String)
+            # newlines are an error (use "nl" state)
+        ],
+        "nl": [(r"\n", String)],
+        "stringescape": [
+            (
+                r'\\([\\abfnrtv"\']|\n|N{.*?}|u[a-fA-F0-9]{4}|'
+                r"U[a-fA-F0-9]{8}|x[a-fA-F0-9]{2}|[0-7]{1,3})",
+                String.Escape,
+            )
+        ],
+    }
+
+
+def setup(app):
+    from sphinx.highlighting import lexers
+
+    lexers["wkt"] = WKTLexer()
+    lexers["mapfile"] = MapFileLexer()
```

### Comparing `mappyfile-1.0.1/docs/development.rst` & `mappyfile-1.0.2/docs/development.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-Development Notes
-=================
-
-The development notes below assume a PowerShell prompt is being used on a Windows machine.
-
-Run the following before any of the following tasks (once the virtual environment itself has been built):
-
-.. code-block:: ps1
-
-    # update the following to your local paths
-    $VIRTUALENV="C:\VirtualEnvs\mappyfile3"
-    $MAPPYFILE_PATH="D:\GitHub\mappyfile"
-
-    .$VIRTUALENV\Scripts\activate.ps1
-    cd $MAPPYFILE_PATH
-
-Building the Dev Virtual Environment
-------------------------------------
-
-Run from the root of the mappyfile project folder:
-
-.. code-block:: ps1
-
-    $VIRTUALENV="C:\VirtualEnvs\mappyfile"
-    $MAPPYFILE_PATH="D:\GitHub\mappyfile"
-
-    cd "C:\Python310\Scripts"
-    .\pip install virtualenv
-    .\virtualenv $VIRTUALENV
-    .$VIRTUALENV\Scripts\activate.ps1
-    cd $MAPPYFILE_PATH
-    pip install -e .
-    pip install -r requirements-dev.txt
-    # optionally install lark_cython
-    pip install -e .[lark_cython]
-
-Testing Locally
----------------
-
-Ensure the development code has been deployed to a virtual environment as in the
-step above.
-
-Then run from the root of the mappyfile project folder:
-
-.. code-block:: ps1
-
-    pytest
-
-To see a list of which tests will run, without actually running them:
-
-.. code-block:: ps1
-
-    pytest --collect-only
-
-To run a single test file:
-
-.. code-block:: ps1
-
-    pytest tests/test_snippets.py
-
-To also include doctests:
-
-.. code-block:: ps1
-
-    pytest --doctest-modules --ignore=./docs/examples/pretty_printing.py
-
-Linting
--------
-
-.. code-block:: ps1
-
-    flake8 .
-
-Or to export to file:
-
-.. code-block:: ps1
-
-    flake8 . > D:\Temp\lint.txt
-
-Prospector
-----------
-
-.. code-block:: ps1
-
-    pip install prospector
-    prospector
-    # or just the main source code folder
-    prospector ./mappyfile
-
-Mypy
-----
-
-To run static type checking:
-
-.. code-block:: ps1
-
-    mypy mappyfile tests
-
-
-Documentation
--------------
-
-To build the Sphinx documentation:
-
-.. code-block:: ps1
-
-    sphinx-build -b html "$MAPPYFILE_PATH\docs" "$MAPPYFILE_PATH\_build"
-    # to force a rebuild of all files
-    sphinx-build -a -E -b html "$MAPPYFILE_PATH\docs" "$MAPPYFILE_PATH\_build"
-
-To run in a local browser:
-
-.. code-block:: ps1
-
-    .$VIRTUALENV\Scripts\activate.ps1
-    C:\Python310\python -m http.server --directory="$MAPPYFILE_PATH\_build" 57921
-
-    # open browser and go to http://localhost:57921
-
-To automatically rebuild docs using `watchdog <https://pypi.org/project/watchdog/>`_:
-
-.. code-block:: ps1
-
-    # run the following to automatically rebuild the project
-    # python -m pip install -U "watchdog[watchmedo]"
-    cd $MAPPYFILE_PATH
-    watchmedo shell-command --patterns="*.rst;*.txt" --recursive --command='sphinx-build -b html "./docs" "./_build"' ./docs
+Development Notes
+=================
+
+The development notes below assume a PowerShell prompt is being used on a Windows machine.
+
+Run the following before any of the following tasks (once the virtual environment itself has been built):
+
+.. code-block:: ps1
+
+    # update the following to your local paths
+    $VIRTUALENV="C:\VirtualEnvs\mappyfile3"
+    $MAPPYFILE_PATH="D:\GitHub\mappyfile"
+
+    .$VIRTUALENV\Scripts\activate.ps1
+    cd $MAPPYFILE_PATH
+
+Building the Dev Virtual Environment
+------------------------------------
+
+Run from the root of the mappyfile project folder:
+
+.. code-block:: ps1
+
+    $VIRTUALENV="C:\VirtualEnvs\mappyfile"
+    $MAPPYFILE_PATH="D:\GitHub\mappyfile"
+
+    cd "C:\Python310\Scripts"
+    .\pip install virtualenv
+    .\virtualenv $VIRTUALENV
+    .$VIRTUALENV\Scripts\activate.ps1
+    cd $MAPPYFILE_PATH
+    pip install -e .
+    pip install -r requirements-dev.txt
+    # optionally install lark_cython
+    pip install -e .[lark_cython]
+
+Testing Locally
+---------------
+
+Ensure the development code has been deployed to a virtual environment as in the
+step above.
+
+Then run from the root of the mappyfile project folder:
+
+.. code-block:: ps1
+
+    pytest
+
+To see a list of which tests will run, without actually running them:
+
+.. code-block:: ps1
+
+    pytest --collect-only
+
+To run a single test file:
+
+.. code-block:: ps1
+
+    pytest tests/test_snippets.py
+
+To also include doctests:
+
+.. code-block:: ps1
+
+    pytest --doctest-modules --ignore=./docs/examples/pretty_printing.py
+
+Linting
+-------
+
+.. code-block:: ps1
+
+    flake8 .
+
+Or to export to file:
+
+.. code-block:: ps1
+
+    flake8 . > D:\Temp\lint.txt
+
+Prospector
+----------
+
+.. code-block:: ps1
+
+    pip install prospector
+    prospector
+    # or just the main source code folder
+    prospector ./mappyfile
+
+Mypy
+----
+
+To run static type checking:
+
+.. code-block:: ps1
+
+    mypy mappyfile tests
+
+
+Documentation
+-------------
+
+To build the Sphinx documentation:
+
+.. code-block:: ps1
+
+    sphinx-build -b html "$MAPPYFILE_PATH\docs" "$MAPPYFILE_PATH\_build"
+    # to force a rebuild of all files
+    sphinx-build -a -E -b html "$MAPPYFILE_PATH\docs" "$MAPPYFILE_PATH\_build"
+
+To run in a local browser:
+
+.. code-block:: ps1
+
+    .$VIRTUALENV\Scripts\activate.ps1
+    C:\Python310\python -m http.server --directory="$MAPPYFILE_PATH\_build" 57921
+
+    # open browser and go to http://localhost:57921
+
+To automatically rebuild docs using `watchdog <https://pypi.org/project/watchdog/>`_:
+
+.. code-block:: ps1
+
+    # run the following to automatically rebuild the project
+    # python -m pip install -U "watchdog[watchmedo]"
+    cd $MAPPYFILE_PATH
+    watchmedo shell-command --patterns="*.rst;*.txt" --recursive --command='sphinx-build -b html "./docs" "./_build"' ./docs
```

### Comparing `mappyfile-1.0.1/docs/format.txt` & `mappyfile-1.0.2/docs/format.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Usage: mappyfile format [OPTIONS] INPUT_MAPFILE OUTPUT_MAPFILE
-
-  Format a the input-mapfile and save as output-mapfile. Note output-mapfile
-  will be  overwritten if it already exists.
-
-  Example of formatting a single Mapfile:
-
-      mappyfile format C:/Temp/valid.map C:/Temp/valid_formatted.map
-
-  Example of formatting a single Mapfile with single quotes and tabs for
-  indentation:
-
-      mappyfile format C:/Temp/valid.map C:/Temp/valid_formatted.map
-      --quote=\' --indent=1 --spacer=
-
-  Example of formatting a single Mapfile without expanding includes, but
-  including comments:
-
-      mappyfile format C:/Temp/valid.map C:/Temp/valid_formatted.map --no-
-      expand --comments
-
-Options:
-  --indent INTEGER            The number of spacer characters to indent
-                              structures in the Mapfile  [default: 4]
-  --spacer TEXT               The character to use for indenting structures in
-                              the Mapfile
-  --quote TEXT                The quote character to use in the Mapfile
-                              (double or single quotes). Ensure these are
-                              escaped e.g. \" or \' [default: \"]
-  --newlinechar TEXT          The character used to insert newlines in the
-                              Mapfile [default: \n]
-  --expand / --no-expand      Expand any INCLUDE directives found in the
-                              Mapfile  [default: True]
-  --comments / --no-comments  Keep Mapfile comments in the output
-                              (experimental)  [default: False]
-  --help                      Show this message and exit.
+Usage: mappyfile format [OPTIONS] INPUT_MAPFILE OUTPUT_MAPFILE
+
+  Format a the input-mapfile and save as output-mapfile. Note output-mapfile
+  will be  overwritten if it already exists.
+
+  Example of formatting a single Mapfile:
+
+      mappyfile format C:/Temp/valid.map C:/Temp/valid_formatted.map
+
+  Example of formatting a single Mapfile with single quotes and tabs for
+  indentation:
+
+      mappyfile format C:/Temp/valid.map C:/Temp/valid_formatted.map
+      --quote=\' --indent=1 --spacer=
+
+  Example of formatting a single Mapfile without expanding includes, but
+  including comments:
+
+      mappyfile format C:/Temp/valid.map C:/Temp/valid_formatted.map --no-
+      expand --comments
+
+Options:
+  --indent INTEGER            The number of spacer characters to indent
+                              structures in the Mapfile  [default: 4]
+  --spacer TEXT               The character to use for indenting structures in
+                              the Mapfile
+  --quote TEXT                The quote character to use in the Mapfile
+                              (double or single quotes). Ensure these are
+                              escaped e.g. \" or \' [default: \"]
+  --newlinechar TEXT          The character used to insert newlines in the
+                              Mapfile [default: \n]
+  --expand / --no-expand      Expand any INCLUDE directives found in the
+                              Mapfile  [default: True]
+  --comments / --no-comments  Keep Mapfile comments in the output
+                              (experimental)  [default: False]
+  --help                      Show this message and exit.
```

### Comparing `mappyfile-1.0.1/docs/grammar.rst` & `mappyfile-1.0.2/docs/grammar.rst`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-Explaining the Mapfile Grammar
-==============================
-
-For a great introduction to Lark, the general purpose parsing library used by mappyfile see the 
-`Lark reference page <https://github.com/erezsh/lark/blob/master/docs/reference.md>`_. 
-
-The full Mapfile grammar file is shown at the end of this page. The latest version can be seen `here on 
-GitHub <https://github.com/geographika/mappyfile/blob/master/mappyfile/mapfile.lark>`_. 
-
-A Simple Example
-----------------
-
-The easiest way to understand how the parser and grammar work is to go through a short example. 
-We will use the Mapfile snippet below to parse and turn into an AST (Abstract Syntax Tree). 
-
-.. code-block:: mapfile
-
-    MAP
-        NAME 'Test'
-    END
-
-This produces the following tree (click for the full-size version). 
-
-.. image:: images/tree.png
-
-The tree is stored as a Python object, shown below:
-
-.. code-block:: python
-
-    Tree(start, [Tree(composite, [Tree(composite_type, [Token(__MAP39, 'MAP')]), 
-    Tree(composite_body, [Tree(attr, [Token(UNQUOTED_STRING, 'NAME'), 
-    Tree(string, [Token(SINGLE_QUOTED_STRING, "'Test'")])])])])])
-
-This can formatted as follows:
-
-.. code-block:: bat
-
-    start
-      composite
-        composite_type	MAP
-        composite_body
-          attr
-            NAME
-            string	'Test'
-
-The grammar file contains rules and `terminals <http://www.parsifalsoft.com/gloss.html#Terminal>`_, 
-and the parser matches these to the input text to create the tree. 
-
-We will now go through all the rules matched by our example Mapfile. 
-
-The first rule ``start`` will always be at the root of the tree:
-
-.. code-block:: javascript
-
-    start: composite+
-
-The rule checks for a ``composite`` rule, followed by a plus sign, indicating one or more 
-composite types should be found in the input.
-
-Next we'll look at the ``composite`` rule:
-
-.. code-block:: javascript
-
-    composite: composite_type composite_body _END
-           | metadata
-           | validation
-
-This rule is matched by a list of options - each on its own line starting with the **|** (pipe) character. When writing or debugging a grammar
-you can comment out options to see which one matches for a particular input. 
-
-In our example the Mapfile matches the first option ``composite_type composite_body _END``, which can be broken down as follows:
-
-+ a ``composite_type`` rule (in this case ``MAP``)
-+ a ``composite_body`` rule
-+ the ``_END`` terminal (the literal string "END")
-
-As each rule creates a new branch on the tree a new ``composite`` branch is created from the ``start`` branch. 
-
-.. code-block:: javascript
-
-    !composite_type: "CLASS"i // i here is used for case insensitive matches, so CLASS, Class, or class will all be matched             
-                | "CLUSTER"i
-                | "MAP"i
-                // list cut for brevity
-
-The ``composite_type`` rule again has a list of options, but in this case consists of string literals. 
-The **!** before the rule name means the rule will keep all their terminals. 
-Without the **!** the tree would look as below - note the ``MAP`` value is missing from the ``composite_type`` branch. 
-
-.. image:: images/tree_no_terminals.png
-
-Next let's look at the ``attr`` rule:
-
-.. code-block:: javascript
-  
-    attr: attr_name value+
-
-This consists of 2 further rules. An ``attr_name`` match and one or more ``value`` rules (as noted above 
-the + denotes one or more matches). A new ``attr`` branch is added to the tree with these rules as children. 
-
-The ``attr_name`` rule is as follows:
-
-.. code-block:: javascript
-
-    attr_name: NAME | composite_type
-    
-In our example the rule is matched by the ``NAME`` terminal (the alternative is a ``composite_type``). 
-This is defined using a regular expression to match a string:
-
-.. code-block:: javascript
-
-    NAME: /[a-z_][a-z0-9_]*/i
-
-The regular expression can be explained as follows:
-
-+ ``[a-z_]`` - a single letter from a to z, or an underscore
-+ ``[a-z0-9_]`` - a single letter from a to z, a number from 0-9, or an underscore
-+ the ``*`` indicates zero to many matches
-+ the ``i`` indicates a case-insensitive search
-
-Therefore the following strings would all match: ``NAME, name, Name, NAME_, MY_NAME``, however ``'NAME', My Name, N@me`` would not. 
-
-The final rule matched in our example is the ``value`` rule. 
-
-.. code-block:: javascript
-
-    ?value: bare_string | string | int | float | expression | not_expression | attr_bind | path | regexp | runtime_var | list
-
-The **?** preceding the rule causes it to be "inlined" if it has a single child. This means a new branch isn't created for the ``value`` rule, and its
-child is added directly to the branch. The tree with "inlining" results in: 
-
-.. image:: images/tree_inlining.png
-
-And without inlining (the **?** character), the ``value`` branch appears:
-
-.. image:: images/tree_noinlining.png
-
-This example covers a large number of the rules in the grammar file, and hopefully provides a basis for understanding the more complicated rules. 
-
-Terminals
----------
-
-Terminals are displayed in uppercase in the grammar file. They are used to match tokens using string literals, regular expressions, or combinations
-of other terminals. 
-
-If the terminal is proceeded by an underscore it won't appear in the tree, for example the closing blocks of each of the composite types:
-
-.. code-block:: javascript
-
-    _END: "END"i
-
-Many of the terminals make use of regular expressions to match tokens. The site https://regex101.com/ provides useful explanations of these. 
-Remember to set the Python "Flavor" and to remove the surrounding forward slashes. 
-
-For example to get an explanation of ``COMMENT: /\#[^\n]*/`` enter ``\#[^\n]*``:
-
-.. image:: images/regex.png
-
-Some further explanations are below:
-
-.. code-block:: javascript
-
-    // check for path names e.g. /root/logs
-    PATH: /[a-z_]*[.\/][a-z0-9_\/.]+/i
-
-Miscellaneous Notes
--------------------
-
-+ Rules can be matched recursively so one of the ``composite_body`` can contain a ``_composite_item`` which can in turn be another ``composite``. This allows us to parse
-  nested composite types such as a ``CLASS`` in a ``LAYER`` in a ``MAP``.
-
-.. code-block:: javascript
-
-	composite_body: _composite_item*
-	_composite_item: (composite|attr|points|projection|metadata|pattern|validation|values) _NL+
-
-+ There are some common imported rules. These can be found at https://github.com/erezsh/lark/blob/master/lark/grammars/common.g.
-  For example:
-
-.. code-block:: javascript
-
-    %import common.INT
-
-    // this is defined in common.g as follows
-
-    DIGIT: "0".."9"
-    INT: DIGIT+
-
-Grammar File
-------------
-
-The full Mapfile grammar is shown below. 
-
-.. literalinclude:: ../mappyfile/mapfile.lark
-   :language: javascript
-
-..
-	Questions: Why bare_string and bare_string2?
-	_rule - means no function in transformer??
-
-	Ambiguities:
-
-	SYMBOL "Name" 
-
-	QUERYMAP
-		STYLE HILIYE
-
-	Style is also a composite
-
-    SCALEBAR
-        STYLE 1
-    END
+Explaining the Mapfile Grammar
+==============================
+
+For a great introduction to Lark, the general purpose parsing library used by mappyfile see the 
+`Lark reference page <https://github.com/erezsh/lark/blob/master/docs/reference.md>`_. 
+
+The full Mapfile grammar file is shown at the end of this page. The latest version can be seen `here on 
+GitHub <https://github.com/geographika/mappyfile/blob/master/mappyfile/mapfile.lark>`_. 
+
+A Simple Example
+----------------
+
+The easiest way to understand how the parser and grammar work is to go through a short example. 
+We will use the Mapfile snippet below to parse and turn into an AST (Abstract Syntax Tree). 
+
+.. code-block:: mapfile
+
+    MAP
+        NAME 'Test'
+    END
+
+This produces the following tree (click for the full-size version). 
+
+.. image:: images/tree.png
+
+The tree is stored as a Python object, shown below:
+
+.. code-block:: python
+
+    Tree(start, [Tree(composite, [Tree(composite_type, [Token(__MAP39, 'MAP')]), 
+    Tree(composite_body, [Tree(attr, [Token(UNQUOTED_STRING, 'NAME'), 
+    Tree(string, [Token(SINGLE_QUOTED_STRING, "'Test'")])])])])])
+
+This can formatted as follows:
+
+.. code-block:: bat
+
+    start
+      composite
+        composite_type	MAP
+        composite_body
+          attr
+            NAME
+            string	'Test'
+
+The grammar file contains rules and `terminals <http://www.parsifalsoft.com/gloss.html#Terminal>`_, 
+and the parser matches these to the input text to create the tree. 
+
+We will now go through all the rules matched by our example Mapfile. 
+
+The first rule ``start`` will always be at the root of the tree:
+
+.. code-block:: javascript
+
+    start: composite+
+
+The rule checks for a ``composite`` rule, followed by a plus sign, indicating one or more 
+composite types should be found in the input.
+
+Next we'll look at the ``composite`` rule:
+
+.. code-block:: javascript
+
+    composite: composite_type composite_body _END
+           | metadata
+           | validation
+
+This rule is matched by a list of options - each on its own line starting with the **|** (pipe) character. When writing or debugging a grammar
+you can comment out options to see which one matches for a particular input. 
+
+In our example the Mapfile matches the first option ``composite_type composite_body _END``, which can be broken down as follows:
+
++ a ``composite_type`` rule (in this case ``MAP``)
++ a ``composite_body`` rule
++ the ``_END`` terminal (the literal string "END")
+
+As each rule creates a new branch on the tree a new ``composite`` branch is created from the ``start`` branch. 
+
+.. code-block:: javascript
+
+    !composite_type: "CLASS"i // i here is used for case insensitive matches, so CLASS, Class, or class will all be matched             
+                | "CLUSTER"i
+                | "MAP"i
+                // list cut for brevity
+
+The ``composite_type`` rule again has a list of options, but in this case consists of string literals. 
+The **!** before the rule name means the rule will keep all their terminals. 
+Without the **!** the tree would look as below - note the ``MAP`` value is missing from the ``composite_type`` branch. 
+
+.. image:: images/tree_no_terminals.png
+
+Next let's look at the ``attr`` rule:
+
+.. code-block:: javascript
+  
+    attr: attr_name value+
+
+This consists of 2 further rules. An ``attr_name`` match and one or more ``value`` rules (as noted above 
+the + denotes one or more matches). A new ``attr`` branch is added to the tree with these rules as children. 
+
+The ``attr_name`` rule is as follows:
+
+.. code-block:: javascript
+
+    attr_name: NAME | composite_type
+    
+In our example the rule is matched by the ``NAME`` terminal (the alternative is a ``composite_type``). 
+This is defined using a regular expression to match a string:
+
+.. code-block:: javascript
+
+    NAME: /[a-z_][a-z0-9_]*/i
+
+The regular expression can be explained as follows:
+
++ ``[a-z_]`` - a single letter from a to z, or an underscore
++ ``[a-z0-9_]`` - a single letter from a to z, a number from 0-9, or an underscore
++ the ``*`` indicates zero to many matches
++ the ``i`` indicates a case-insensitive search
+
+Therefore the following strings would all match: ``NAME, name, Name, NAME_, MY_NAME``, however ``'NAME', My Name, N@me`` would not. 
+
+The final rule matched in our example is the ``value`` rule. 
+
+.. code-block:: javascript
+
+    ?value: bare_string | string | int | float | expression | not_expression | attr_bind | path | regexp | runtime_var | list
+
+The **?** preceding the rule causes it to be "inlined" if it has a single child. This means a new branch isn't created for the ``value`` rule, and its
+child is added directly to the branch. The tree with "inlining" results in: 
+
+.. image:: images/tree_inlining.png
+
+And without inlining (the **?** character), the ``value`` branch appears:
+
+.. image:: images/tree_noinlining.png
+
+This example covers a large number of the rules in the grammar file, and hopefully provides a basis for understanding the more complicated rules. 
+
+Terminals
+---------
+
+Terminals are displayed in uppercase in the grammar file. They are used to match tokens using string literals, regular expressions, or combinations
+of other terminals. 
+
+If the terminal is proceeded by an underscore it won't appear in the tree, for example the closing blocks of each of the composite types:
+
+.. code-block:: javascript
+
+    _END: "END"i
+
+Many of the terminals make use of regular expressions to match tokens. The site https://regex101.com/ provides useful explanations of these. 
+Remember to set the Python "Flavor" and to remove the surrounding forward slashes. 
+
+For example to get an explanation of ``COMMENT: /\#[^\n]*/`` enter ``\#[^\n]*``:
+
+.. image:: images/regex.png
+
+Some further explanations are below:
+
+.. code-block:: javascript
+
+    // check for path names e.g. /root/logs
+    PATH: /[a-z_]*[.\/][a-z0-9_\/.]+/i
+
+Miscellaneous Notes
+-------------------
+
++ Rules can be matched recursively so one of the ``composite_body`` can contain a ``_composite_item`` which can in turn be another ``composite``. This allows us to parse
+  nested composite types such as a ``CLASS`` in a ``LAYER`` in a ``MAP``.
+
+.. code-block:: javascript
+
+	composite_body: _composite_item*
+	_composite_item: (composite|attr|points|projection|metadata|pattern|validation|values) _NL+
+
++ There are some common imported rules. These can be found at https://github.com/erezsh/lark/blob/master/lark/grammars/common.g.
+  For example:
+
+.. code-block:: javascript
+
+    %import common.INT
+
+    // this is defined in common.g as follows
+
+    DIGIT: "0".."9"
+    INT: DIGIT+
+
+Grammar File
+------------
+
+The full Mapfile grammar is shown below. 
+
+.. literalinclude:: ../mappyfile/mapfile.lark
+   :language: javascript
+
+..
+	Questions: Why bare_string and bare_string2?
+	_rule - means no function in transformer??
+
+	Ambiguities:
+
+	SYMBOL "Name" 
+
+	QUERYMAP
+		STYLE HILIYE
+
+	Style is also a composite
+
+    SCALEBAR
+        STYLE 1
+    END
     Newlines ignored
```

### Comparing `mappyfile-1.0.1/docs/index.rst` & `mappyfile-1.0.2/docs/index.rst`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-﻿mappyfile
-=========
-
-.. image:: images/OSGeo_community.png
-    :align: right
-    :scale: 40%
-
-A Python library to create, parse, modify, and format `MapServer <https://mapserver.org/documentation.html>`_ Mapfiles. 
-
-+ Pure Python - no MapServer dependencies
-+ Open Source License (MIT)
-+ An official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_
-
-An online formatter demonstrating the libraries capabilities can be found at: https://app.mapserverstudio.net/
-
-mappyfile was first introduced in a presentation at `FOSS4G Europe 2017 <https://europe.foss4g.org/2017/Home>`_ - slides are available 
-:download:`to download here <_static/foss4ge2017_mappyfile_sgirvin.pdf>`.
-
-.. toctree::
-    :maxdepth: 2
-    :titlesonly:
-    :caption: Documentation Contents
-
-    Parsing <parser.rst>
-    Transforming <transformer.rst>
-    editing.rst
-    Pretty Printing <pretty_printing.rst>
-    comments.rst
-    validation.rst
-    schemas.rst
-    grammar.rst
-    python_integration.rst
-    client.rst
-    api/main.rst
-    testing.rst
-    development.rst
-    HISTORY.rst
-
-.. image:: images/class_parsed.png
-
-Installation
-------------
-
-mappyfile is available on `PyPI <https://pypi.org/project/mappyfile/>`_ (the Python Package Index), and can be installed using pip.
-It requires **Python 3.8** or higher.
-
-.. code-block:: console
-
-    pip install mappyfile
-
-This will also install its required dependencies - `Lark <https://github.com/lark-parser/lark>`__, and 
-`jsonschema <https://github.com/python-jsonschema/jsonschema>`_. 
-
-To install the optional `lark-cython <https://github.com/lark-parser/lark_cython>`_ library
-for better performance on CPython you can run the following command:
-
-.. code-block:: console
-
-    pip install mappyfile[lark_cython]
-
-If lark-cython is installed it will be used automatically. If it is installed and you want to disable its
-use in mappyfile you can set the ``MAPPYFILE_USE_CYTHON`` to ``False`` (or any falsy value). 
-
-.. code-block:: console
-
-    # Linux
-    export MAPPYFILE_USE_CYTHON="False"
-
-    # Windows PowerShell
-    $env:MAPPYFILE_USE_CYTHON="False"
-
-    # Windows Command Line
-    set MAPPYFILE_USE_CYTHON=False
-
-mappyfile is also available on `conda <https://anaconda.org/conda-forge/mappyfile>`_. Install as
-follows:
-
-.. code-block:: console
-
-    conda install -c conda-forge mappyfile
-
-To setup a Conda environment containing mappyfile from scratch on Windows download
-`Miniconda3 Windows 64-bit <https://conda.io/projects/conda/en/latest/user-guide/install/windows.html>`_
-and run the following commands:
-
-.. code-block:: console
-
-    conda create --name mappyfile-env
-    conda activate mappyfile-env
-
-    conda config --add channels conda-forge
-    conda config --set channel_priority strict
-    conda install mappyfile --yes
-
-    mappyfile --help
-
-Quick Start
------------
-
-This section details the basic use of the ``mappyfile`` library. To see all functionality and examples see the :ref:`mappyfile-api` documentation. 
-
-Accessing Values
-++++++++++++++++
-
-.. literalinclude:: examples/api/accessing_values_test.py
-    :language: python
-    :dedent: 4
-    :start-after: # START OF API EXAMPLE
-    :end-before: # END OF API EXAMPLE
-
-Query
-+++++
-
-.. literalinclude:: examples/api/search_test.py
-    :language: python
-    :dedent: 4
-    :start-after: # START OF API EXAMPLE
-    :end-before: # END OF API EXAMPLE
-    
-Modifying Values
-++++++++++++++++
-
-.. literalinclude:: examples/api/modifying_values_test.py
-    :language: python
-    :dedent: 4
-    :start-after: # START OF API EXAMPLE
-    :end-before: # END OF API EXAMPLE
-
-Adding Items
-++++++++++++
-
-Adding a new layer:
-
-.. literalinclude:: examples/api/adding_values_test.py
-    :language: python
-    :dedent: 4
-    :start-after: # START OF ADD LAYER EXAMPLE
-    :end-before: # END OF ADD LAYER EXAMPLE
-
-Adding a new class to a layer:
-
-.. literalinclude:: examples/api/adding_values_test.py
-    :language: python
-    :dedent: 4
-    :start-after: # START OF ADD CLASS EXAMPLE
-    :end-before: # END OF ADD CLASS EXAMPLE
-
-Three command line tools are also available - ``format``, ``validate``, and ``schema``:
-
-.. code-block:: bat
-
-    mappyfile format raster.map formatted_raster.map
-    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
-    mappyfile schema mapfile-schema-8-0.json --version=8.0
-
-What is mappyfile?
-------------------
-
-*mappyfile* takes a Mapfile as input and parses it into an `Abstract syntax tree (AST) <https://en.wikipedia.org/wiki/Abstract_syntax_tree>`_ 
-using `Lark <https://github.com/lark-parser/lark>`_ a Python parsing library. 
-mappyfile can then transform the AST into a dictionary structure, containing keys and values of dicts, and lists familiar to
-Python programmers. This structure can be edited directly. Alternatively new objects can be added by parsing further Mapfile text and 
-inserting into the dictionary structure. mappyfile also includes a "pretty printer" to export this dictionary structure back to a 
-Mapfile, with keyword formatting and indentation. 
-
-*mappyfile* assumes knowledge of the Mapfile format - a `domain specific language (DSL) <https://en.wikipedia.org/wiki/Domain-specific_language>`_ used
-by MapServer to generate map images. mappyfile is a possible alternative to using MapScript. The definitions of these (from the 
-`MapServer glossary <http://mapserver.org/el/glossary.html>`_) are shown below:
-
-+ **Mapfile** is the declarative language that MapServer uses to define data connections, 
-  map styling, templating, and server directives. Its format is XML-like and hierarchical, 
-  with closing END tags, but the format is not XML.
-
-+ **MapScript** is an alternative to the CGI application of mapserv that allows you to 
-  program the MapServer object API in many languages.
-
-The diagram below shows the different elements of mappyfile, and how they are used to modify a Mapfile:
-
-.. image:: images/mappyfile_modules.png
-
-Why?
-----
-
-* Easily generate development, staging, and production Mapfiles from the same source Mapfile
-* Create Mapfiles for different datasets from a single Mapfile
-* Create, manipulate, and test Mapfiles from within Python
-
-The current alternative to building applications with MapServer is to use MapScript. This approach has a
-number of issues that resulted in the development of mappyfile:
-
-+ MapScript needs to be compiled using SWIG and a C/C++ compiler
-+ You need to create an empty log file or MapServer won't open the map (or get ``msSetErrorFile(): General error message. 
-  Failed to open MS_ERRORFILE`` errors)
-+ MapScript is only available for Windows on PyPI
-+ It is necessary to set the working directory so that MapServer includes are found (this also applies to mappyfile, but there is no need to os.chdir
-  and change the working directory for your script or application)
-+ The MapScript API is not particularly "Pythonic"
-
-One key difference is that mappyfile only deals with text, so you cannot retrieve features or connect to databases through layers as you can with MapScript. 
-mappyfile's approach is to build a Mapfile that then uses the mapserv program to handle these requirements. This design was influenced by Sean Gillies,
-the MapScript maintainer for several years (until 2006). A couple of his last blog posts on MapScript make a strong case for working with Mapfiles rather than MapScript:  
-
-    *"Cease, or at the very least, minimize your use of MapServer's various language bindings. 
-    Instead, embrace MapServer's domain-specific language (DSL) and write more of the declarative 
-    cartographic scripts known as mapfiles. Use the mapserv (or shp2img) program to compile these 
-    scripts into images. This is the path to happiness and prosperity."*
-
-    Sean Gillies - `Stop using MapScript`_
-
-A later post listed the benefits of this approach:
-
-    *"the instructions encoded in a MapServer mapfile comprise a domain-specific language..
-    to embrace the map language is to benefit from simplicity, usability, and portability."*
-
-    Sean Gillies - `Declarative Maps`_
-
-The concept of the Mapfile as a DSL has been implemented a few times. A Python `Mapfile builder`_ written by Allan Doyle used an XML approach.
-
-More recently the Node module `node-mapserv`_ provides support for declarative mapfile programming. 
-As the author notes: 
-
-    *node-mapserv is not MapScript for Node. Instead it provides a simple declarative API for 
-    rendering mapserver mapfiles..most of what can be accomplished imperatively 
-    using mapscript can be done declaratively by custom generating new mapfiles and tweaking 
-    existing mapfiles*
-
-As an interesting footnote the MapScript "bindings" are available in several different languages thanks to `SWIG <https://en.wikipedia.org/wiki/SWIG>`_ which creates wrapper 
-code for C. SWIG was developed by `David Beazley <http://www.dabeaz.com/>`_, who then later built `PLY <http://www.dabeaz.com/ply/>`_ on which mappyfile was originally based. 
-PLY is an implementation of lex and yacc parsing tools for Python - the tools MapServer itself uses to parse Mapfiles in C. 
-
-Development Roadmap
--------------------
-
-Future development plans include:
-
-+ Setup an easy way to plug in "linters" to check various Mapfile settings and rules (e.g. configured correctly for WFS)
-+ Create a Jupyter Notebook demonstrating mappyfile usage
-+ Add a plugins page to the docs
-+ Add an example of creating Mapfiles using YAML
-+ Create a new ``prune`` function to remove redundant default settings from a Mapfile
-
-
-.. _Stop using MapScript: https://sgillies.net/2006/11/29/stop-using-mapscript.html
-.. _Declarative Maps: https://sgillies.net/2006/12/01/declarative-maps.html
-.. _Mapfile builder: https://web.archive.org/web/20090106070607/http://think.random-stuff.org/FrontPage/archive/2006/07/mapfile-builder
-.. _node-mapserv: https://www.npmjs.com/package/mapserv
+﻿mappyfile
+=========
+
+.. image:: images/OSGeo_community.png
+    :align: right
+    :scale: 40%
+
+A Python library to create, parse, modify, and format `MapServer <https://mapserver.org/documentation.html>`_ Mapfiles. 
+
++ Pure Python - no MapServer dependencies
++ Open Source License (MIT)
++ An official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_
+
+An online formatter demonstrating the libraries capabilities can be found at: https://app.mapserverstudio.net/
+
+mappyfile was first introduced in a presentation at `FOSS4G Europe 2017 <https://europe.foss4g.org/2017/Home>`_ - slides are available 
+:download:`to download here <_static/foss4ge2017_mappyfile_sgirvin.pdf>`.
+
+.. toctree::
+    :maxdepth: 2
+    :titlesonly:
+    :caption: Documentation Contents
+
+    Parsing <parser.rst>
+    Transforming <transformer.rst>
+    editing.rst
+    Pretty Printing <pretty_printing.rst>
+    comments.rst
+    validation.rst
+    schemas.rst
+    grammar.rst
+    python_integration.rst
+    client.rst
+    api/main.rst
+    testing.rst
+    development.rst
+    HISTORY.rst
+
+.. image:: images/class_parsed.png
+
+Installation
+------------
+
+mappyfile is available on `PyPI <https://pypi.org/project/mappyfile/>`_ (the Python Package Index), and can be installed using pip.
+It requires **Python 3.8** or higher.
+
+.. code-block:: console
+
+    pip install mappyfile
+
+This will also install its required dependencies - `Lark <https://github.com/lark-parser/lark>`__, and 
+`jsonschema <https://github.com/python-jsonschema/jsonschema>`_. 
+
+To install the optional `lark-cython <https://github.com/lark-parser/lark_cython>`_ library
+for better performance on CPython you can run the following command:
+
+.. code-block:: console
+
+    pip install mappyfile[lark_cython]
+
+If lark-cython is installed it will be used automatically. If it is installed and you want to disable its
+use in mappyfile you can set the ``MAPPYFILE_USE_CYTHON`` to ``False`` (or any falsy value). 
+
+.. code-block:: console
+
+    # Linux
+    export MAPPYFILE_USE_CYTHON="False"
+
+    # Windows PowerShell
+    $env:MAPPYFILE_USE_CYTHON="False"
+
+    # Windows Command Line
+    set MAPPYFILE_USE_CYTHON=False
+
+mappyfile is also available on `conda <https://anaconda.org/conda-forge/mappyfile>`_. Install as
+follows:
+
+.. code-block:: console
+
+    conda install -c conda-forge mappyfile
+
+To setup a Conda environment containing mappyfile from scratch on Windows download
+`Miniconda3 Windows 64-bit <https://conda.io/projects/conda/en/latest/user-guide/install/windows.html>`_
+and run the following commands:
+
+.. code-block:: console
+
+    conda create --name mappyfile-env
+    conda activate mappyfile-env
+
+    conda config --add channels conda-forge
+    conda config --set channel_priority strict
+    conda install mappyfile --yes
+
+    mappyfile --help
+
+Quick Start
+-----------
+
+This section details the basic use of the ``mappyfile`` library. To see all functionality and examples see the :ref:`mappyfile-api` documentation. 
+
+Accessing Values
+++++++++++++++++
+
+.. literalinclude:: examples/api/accessing_values_test.py
+    :language: python
+    :dedent: 4
+    :start-after: # START OF API EXAMPLE
+    :end-before: # END OF API EXAMPLE
+
+Query
++++++
+
+.. literalinclude:: examples/api/search_test.py
+    :language: python
+    :dedent: 4
+    :start-after: # START OF API EXAMPLE
+    :end-before: # END OF API EXAMPLE
+    
+Modifying Values
+++++++++++++++++
+
+.. literalinclude:: examples/api/modifying_values_test.py
+    :language: python
+    :dedent: 4
+    :start-after: # START OF API EXAMPLE
+    :end-before: # END OF API EXAMPLE
+
+Adding Items
+++++++++++++
+
+Adding a new layer:
+
+.. literalinclude:: examples/api/adding_values_test.py
+    :language: python
+    :dedent: 4
+    :start-after: # START OF ADD LAYER EXAMPLE
+    :end-before: # END OF ADD LAYER EXAMPLE
+
+Adding a new class to a layer:
+
+.. literalinclude:: examples/api/adding_values_test.py
+    :language: python
+    :dedent: 4
+    :start-after: # START OF ADD CLASS EXAMPLE
+    :end-before: # END OF ADD CLASS EXAMPLE
+
+Three command line tools are also available - ``format``, ``validate``, and ``schema``:
+
+.. code-block:: bat
+
+    mappyfile format raster.map formatted_raster.map
+    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
+    mappyfile schema mapfile-schema-8-0.json --version=8.0
+
+What is mappyfile?
+------------------
+
+*mappyfile* takes a Mapfile as input and parses it into an `Abstract syntax tree (AST) <https://en.wikipedia.org/wiki/Abstract_syntax_tree>`_ 
+using `Lark <https://github.com/lark-parser/lark>`_ a Python parsing library. 
+mappyfile can then transform the AST into a dictionary structure, containing keys and values of dicts, and lists familiar to
+Python programmers. This structure can be edited directly. Alternatively new objects can be added by parsing further Mapfile text and 
+inserting into the dictionary structure. mappyfile also includes a "pretty printer" to export this dictionary structure back to a 
+Mapfile, with keyword formatting and indentation. 
+
+*mappyfile* assumes knowledge of the Mapfile format - a `domain specific language (DSL) <https://en.wikipedia.org/wiki/Domain-specific_language>`_ used
+by MapServer to generate map images. mappyfile is a possible alternative to using MapScript. The definitions of these (from the 
+`MapServer glossary <http://mapserver.org/el/glossary.html>`_) are shown below:
+
++ **Mapfile** is the declarative language that MapServer uses to define data connections, 
+  map styling, templating, and server directives. Its format is XML-like and hierarchical, 
+  with closing END tags, but the format is not XML.
+
++ **MapScript** is an alternative to the CGI application of mapserv that allows you to 
+  program the MapServer object API in many languages.
+
+The diagram below shows the different elements of mappyfile, and how they are used to modify a Mapfile:
+
+.. image:: images/mappyfile_modules.png
+
+Why?
+----
+
+* Easily generate development, staging, and production Mapfiles from the same source Mapfile
+* Create Mapfiles for different datasets from a single Mapfile
+* Create, manipulate, and test Mapfiles from within Python
+
+The current alternative to building applications with MapServer is to use MapScript. This approach has a
+number of issues that resulted in the development of mappyfile:
+
++ MapScript needs to be compiled using SWIG and a C/C++ compiler
++ You need to create an empty log file or MapServer won't open the map (or get ``msSetErrorFile(): General error message. 
+  Failed to open MS_ERRORFILE`` errors)
++ MapScript is only available for Windows on PyPI
++ It is necessary to set the working directory so that MapServer includes are found (this also applies to mappyfile, but there is no need to os.chdir
+  and change the working directory for your script or application)
++ The MapScript API is not particularly "Pythonic"
+
+One key difference is that mappyfile only deals with text, so you cannot retrieve features or connect to databases through layers as you can with MapScript. 
+mappyfile's approach is to build a Mapfile that then uses the mapserv program to handle these requirements. This design was influenced by Sean Gillies,
+the MapScript maintainer for several years (until 2006). A couple of his last blog posts on MapScript make a strong case for working with Mapfiles rather than MapScript:  
+
+    *"Cease, or at the very least, minimize your use of MapServer's various language bindings. 
+    Instead, embrace MapServer's domain-specific language (DSL) and write more of the declarative 
+    cartographic scripts known as mapfiles. Use the mapserv (or shp2img) program to compile these 
+    scripts into images. This is the path to happiness and prosperity."*
+
+    Sean Gillies - `Stop using MapScript`_
+
+A later post listed the benefits of this approach:
+
+    *"the instructions encoded in a MapServer mapfile comprise a domain-specific language..
+    to embrace the map language is to benefit from simplicity, usability, and portability."*
+
+    Sean Gillies - `Declarative Maps`_
+
+The concept of the Mapfile as a DSL has been implemented a few times. A Python `Mapfile builder`_ written by Allan Doyle used an XML approach.
+
+More recently the Node module `node-mapserv`_ provides support for declarative mapfile programming. 
+As the author notes: 
+
+    *node-mapserv is not MapScript for Node. Instead it provides a simple declarative API for 
+    rendering mapserver mapfiles..most of what can be accomplished imperatively 
+    using mapscript can be done declaratively by custom generating new mapfiles and tweaking 
+    existing mapfiles*
+
+As an interesting footnote the MapScript "bindings" are available in several different languages thanks to `SWIG <https://en.wikipedia.org/wiki/SWIG>`_ which creates wrapper 
+code for C. SWIG was developed by `David Beazley <http://www.dabeaz.com/>`_, who then later built `PLY <http://www.dabeaz.com/ply/>`_ on which mappyfile was originally based. 
+PLY is an implementation of lex and yacc parsing tools for Python - the tools MapServer itself uses to parse Mapfiles in C. 
+
+Development Roadmap
+-------------------
+
+Future development plans include:
+
++ Setup an easy way to plug in "linters" to check various Mapfile settings and rules (e.g. configured correctly for WFS)
++ Create a Jupyter Notebook demonstrating mappyfile usage
++ Add a plugins page to the docs
++ Add an example of creating Mapfiles using YAML
++ Create a new ``prune`` function to remove redundant default settings from a Mapfile
+
+
+.. _Stop using MapScript: https://sgillies.net/2006/11/29/stop-using-mapscript.html
+.. _Declarative Maps: https://sgillies.net/2006/12/01/declarative-maps.html
+.. _Mapfile builder: https://web.archive.org/web/20090106070607/http://think.random-stuff.org/FrontPage/archive/2006/07/mapfile-builder
+.. _node-mapserv: https://www.npmjs.com/package/mapserv
```

### Comparing `mappyfile-1.0.1/docs/make.bat` & `mappyfile-1.0.2/docs/make.bat`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-@ECHO OFF
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set BUILDDIR=_build
-set ALLSPHINXOPTS=-d %BUILDDIR%/doctrees %SPHINXOPTS% .
-set I18NSPHINXOPTS=%SPHINXOPTS% .
-if NOT "%PAPER%" == "" (
-	set ALLSPHINXOPTS=-D latex_paper_size=%PAPER% %ALLSPHINXOPTS%
-	set I18NSPHINXOPTS=-D latex_paper_size=%PAPER% %I18NSPHINXOPTS%
-)
-
-if "%1" == "" goto help
-
-if "%1" == "help" (
-	:help
-	echo.Please use `make ^<target^>` where ^<target^> is one of
-	echo.  html       to make standalone HTML files
-	echo.  dirhtml    to make HTML files named index.html in directories
-	echo.  singlehtml to make a single large HTML file
-	echo.  pickle     to make pickle files
-	echo.  json       to make JSON files
-	echo.  htmlhelp   to make HTML files and a HTML help project
-	echo.  qthelp     to make HTML files and a qthelp project
-	echo.  devhelp    to make HTML files and a Devhelp project
-	echo.  epub       to make an epub
-	echo.  epub3      to make an epub3
-	echo.  latex      to make LaTeX files, you can set PAPER=a4 or PAPER=letter
-	echo.  text       to make text files
-	echo.  man        to make manual pages
-	echo.  texinfo    to make Texinfo files
-	echo.  gettext    to make PO message catalogs
-	echo.  changes    to make an overview over all changed/added/deprecated items
-	echo.  xml        to make Docutils-native XML files
-	echo.  pseudoxml  to make pseudoxml-XML files for display purposes
-	echo.  linkcheck  to check all external links for integrity
-	echo.  doctest    to run all doctests embedded in the documentation if enabled
-	echo.  coverage   to run coverage check of the documentation if enabled
-	echo.  dummy      to check syntax errors of document sources
-	goto end
-)
-
-if "%1" == "clean" (
-	for /d %%i in (%BUILDDIR%\*) do rmdir /q /s %%i
-	del /q /s %BUILDDIR%\*
-	goto end
-)
-
-
-REM Check if sphinx-build is available and fallback to Python version if any
-%SPHINXBUILD% 1>NUL 2>NUL
-if errorlevel 9009 goto sphinx_python
-goto sphinx_ok
-
-:sphinx_python
-
-set SPHINXBUILD=python -m sphinx.__init__
-%SPHINXBUILD% 2> nul
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
-	exit /b 1
-)
-
-:sphinx_ok
-
-
-if "%1" == "html" (
-	%SPHINXBUILD% -b html %ALLSPHINXOPTS% %BUILDDIR%/html
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The HTML pages are in %BUILDDIR%/html.
-	goto end
-)
-
-if "%1" == "dirhtml" (
-	%SPHINXBUILD% -b dirhtml %ALLSPHINXOPTS% %BUILDDIR%/dirhtml
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The HTML pages are in %BUILDDIR%/dirhtml.
-	goto end
-)
-
-if "%1" == "singlehtml" (
-	%SPHINXBUILD% -b singlehtml %ALLSPHINXOPTS% %BUILDDIR%/singlehtml
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The HTML pages are in %BUILDDIR%/singlehtml.
-	goto end
-)
-
-if "%1" == "pickle" (
-	%SPHINXBUILD% -b pickle %ALLSPHINXOPTS% %BUILDDIR%/pickle
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished; now you can process the pickle files.
-	goto end
-)
-
-if "%1" == "json" (
-	%SPHINXBUILD% -b json %ALLSPHINXOPTS% %BUILDDIR%/json
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished; now you can process the JSON files.
-	goto end
-)
-
-if "%1" == "htmlhelp" (
-	%SPHINXBUILD% -b htmlhelp %ALLSPHINXOPTS% %BUILDDIR%/htmlhelp
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished; now you can run HTML Help Workshop with the ^
-.hhp project file in %BUILDDIR%/htmlhelp.
-	goto end
-)
-
-if "%1" == "qthelp" (
-	%SPHINXBUILD% -b qthelp %ALLSPHINXOPTS% %BUILDDIR%/qthelp
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished; now you can run "qcollectiongenerator" with the ^
-.qhcp project file in %BUILDDIR%/qthelp, like this:
-	echo.^> qcollectiongenerator %BUILDDIR%\qthelp\mappyfile.qhcp
-	echo.To view the help file:
-	echo.^> assistant -collectionFile %BUILDDIR%\qthelp\mappyfile.ghc
-	goto end
-)
-
-if "%1" == "devhelp" (
-	%SPHINXBUILD% -b devhelp %ALLSPHINXOPTS% %BUILDDIR%/devhelp
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished.
-	goto end
-)
-
-if "%1" == "epub" (
-	%SPHINXBUILD% -b epub %ALLSPHINXOPTS% %BUILDDIR%/epub
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The epub file is in %BUILDDIR%/epub.
-	goto end
-)
-
-if "%1" == "epub3" (
-	%SPHINXBUILD% -b epub3 %ALLSPHINXOPTS% %BUILDDIR%/epub3
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The epub3 file is in %BUILDDIR%/epub3.
-	goto end
-)
-
-if "%1" == "latex" (
-	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished; the LaTeX files are in %BUILDDIR%/latex.
-	goto end
-)
-
-if "%1" == "latexpdf" (
-	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
-	cd %BUILDDIR%/latex
-	make all-pdf
-	cd %~dp0
-	echo.
-	echo.Build finished; the PDF files are in %BUILDDIR%/latex.
-	goto end
-)
-
-if "%1" == "latexpdfja" (
-	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
-	cd %BUILDDIR%/latex
-	make all-pdf-ja
-	cd %~dp0
-	echo.
-	echo.Build finished; the PDF files are in %BUILDDIR%/latex.
-	goto end
-)
-
-if "%1" == "text" (
-	%SPHINXBUILD% -b text %ALLSPHINXOPTS% %BUILDDIR%/text
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The text files are in %BUILDDIR%/text.
-	goto end
-)
-
-if "%1" == "man" (
-	%SPHINXBUILD% -b man %ALLSPHINXOPTS% %BUILDDIR%/man
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The manual pages are in %BUILDDIR%/man.
-	goto end
-)
-
-if "%1" == "texinfo" (
-	%SPHINXBUILD% -b texinfo %ALLSPHINXOPTS% %BUILDDIR%/texinfo
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The Texinfo files are in %BUILDDIR%/texinfo.
-	goto end
-)
-
-if "%1" == "gettext" (
-	%SPHINXBUILD% -b gettext %I18NSPHINXOPTS% %BUILDDIR%/locale
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The message catalogs are in %BUILDDIR%/locale.
-	goto end
-)
-
-if "%1" == "changes" (
-	%SPHINXBUILD% -b changes %ALLSPHINXOPTS% %BUILDDIR%/changes
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.The overview file is in %BUILDDIR%/changes.
-	goto end
-)
-
-if "%1" == "linkcheck" (
-	%SPHINXBUILD% -b linkcheck %ALLSPHINXOPTS% %BUILDDIR%/linkcheck
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Link check complete; look for any errors in the above output ^
-or in %BUILDDIR%/linkcheck/output.txt.
-	goto end
-)
-
-if "%1" == "doctest" (
-	%SPHINXBUILD% -b doctest %ALLSPHINXOPTS% %BUILDDIR%/doctest
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Testing of doctests in the sources finished, look at the ^
-results in %BUILDDIR%/doctest/output.txt.
-	goto end
-)
-
-if "%1" == "coverage" (
-	%SPHINXBUILD% -b coverage %ALLSPHINXOPTS% %BUILDDIR%/coverage
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Testing of coverage in the sources finished, look at the ^
-results in %BUILDDIR%/coverage/python.txt.
-	goto end
-)
-
-if "%1" == "xml" (
-	%SPHINXBUILD% -b xml %ALLSPHINXOPTS% %BUILDDIR%/xml
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The XML files are in %BUILDDIR%/xml.
-	goto end
-)
-
-if "%1" == "pseudoxml" (
-	%SPHINXBUILD% -b pseudoxml %ALLSPHINXOPTS% %BUILDDIR%/pseudoxml
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. The pseudo-XML files are in %BUILDDIR%/pseudoxml.
-	goto end
-)
-
-if "%1" == "dummy" (
-	%SPHINXBUILD% -b dummy %ALLSPHINXOPTS% %BUILDDIR%/dummy
-	if errorlevel 1 exit /b 1
-	echo.
-	echo.Build finished. Dummy builder generates no files.
-	goto end
-)
-
-:end
+@ECHO OFF
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set BUILDDIR=_build
+set ALLSPHINXOPTS=-d %BUILDDIR%/doctrees %SPHINXOPTS% .
+set I18NSPHINXOPTS=%SPHINXOPTS% .
+if NOT "%PAPER%" == "" (
+	set ALLSPHINXOPTS=-D latex_paper_size=%PAPER% %ALLSPHINXOPTS%
+	set I18NSPHINXOPTS=-D latex_paper_size=%PAPER% %I18NSPHINXOPTS%
+)
+
+if "%1" == "" goto help
+
+if "%1" == "help" (
+	:help
+	echo.Please use `make ^<target^>` where ^<target^> is one of
+	echo.  html       to make standalone HTML files
+	echo.  dirhtml    to make HTML files named index.html in directories
+	echo.  singlehtml to make a single large HTML file
+	echo.  pickle     to make pickle files
+	echo.  json       to make JSON files
+	echo.  htmlhelp   to make HTML files and a HTML help project
+	echo.  qthelp     to make HTML files and a qthelp project
+	echo.  devhelp    to make HTML files and a Devhelp project
+	echo.  epub       to make an epub
+	echo.  epub3      to make an epub3
+	echo.  latex      to make LaTeX files, you can set PAPER=a4 or PAPER=letter
+	echo.  text       to make text files
+	echo.  man        to make manual pages
+	echo.  texinfo    to make Texinfo files
+	echo.  gettext    to make PO message catalogs
+	echo.  changes    to make an overview over all changed/added/deprecated items
+	echo.  xml        to make Docutils-native XML files
+	echo.  pseudoxml  to make pseudoxml-XML files for display purposes
+	echo.  linkcheck  to check all external links for integrity
+	echo.  doctest    to run all doctests embedded in the documentation if enabled
+	echo.  coverage   to run coverage check of the documentation if enabled
+	echo.  dummy      to check syntax errors of document sources
+	goto end
+)
+
+if "%1" == "clean" (
+	for /d %%i in (%BUILDDIR%\*) do rmdir /q /s %%i
+	del /q /s %BUILDDIR%\*
+	goto end
+)
+
+
+REM Check if sphinx-build is available and fallback to Python version if any
+%SPHINXBUILD% 1>NUL 2>NUL
+if errorlevel 9009 goto sphinx_python
+goto sphinx_ok
+
+:sphinx_python
+
+set SPHINXBUILD=python -m sphinx.__init__
+%SPHINXBUILD% 2> nul
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.http://sphinx-doc.org/
+	exit /b 1
+)
+
+:sphinx_ok
+
+
+if "%1" == "html" (
+	%SPHINXBUILD% -b html %ALLSPHINXOPTS% %BUILDDIR%/html
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The HTML pages are in %BUILDDIR%/html.
+	goto end
+)
+
+if "%1" == "dirhtml" (
+	%SPHINXBUILD% -b dirhtml %ALLSPHINXOPTS% %BUILDDIR%/dirhtml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The HTML pages are in %BUILDDIR%/dirhtml.
+	goto end
+)
+
+if "%1" == "singlehtml" (
+	%SPHINXBUILD% -b singlehtml %ALLSPHINXOPTS% %BUILDDIR%/singlehtml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The HTML pages are in %BUILDDIR%/singlehtml.
+	goto end
+)
+
+if "%1" == "pickle" (
+	%SPHINXBUILD% -b pickle %ALLSPHINXOPTS% %BUILDDIR%/pickle
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can process the pickle files.
+	goto end
+)
+
+if "%1" == "json" (
+	%SPHINXBUILD% -b json %ALLSPHINXOPTS% %BUILDDIR%/json
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can process the JSON files.
+	goto end
+)
+
+if "%1" == "htmlhelp" (
+	%SPHINXBUILD% -b htmlhelp %ALLSPHINXOPTS% %BUILDDIR%/htmlhelp
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can run HTML Help Workshop with the ^
+.hhp project file in %BUILDDIR%/htmlhelp.
+	goto end
+)
+
+if "%1" == "qthelp" (
+	%SPHINXBUILD% -b qthelp %ALLSPHINXOPTS% %BUILDDIR%/qthelp
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; now you can run "qcollectiongenerator" with the ^
+.qhcp project file in %BUILDDIR%/qthelp, like this:
+	echo.^> qcollectiongenerator %BUILDDIR%\qthelp\mappyfile.qhcp
+	echo.To view the help file:
+	echo.^> assistant -collectionFile %BUILDDIR%\qthelp\mappyfile.ghc
+	goto end
+)
+
+if "%1" == "devhelp" (
+	%SPHINXBUILD% -b devhelp %ALLSPHINXOPTS% %BUILDDIR%/devhelp
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished.
+	goto end
+)
+
+if "%1" == "epub" (
+	%SPHINXBUILD% -b epub %ALLSPHINXOPTS% %BUILDDIR%/epub
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The epub file is in %BUILDDIR%/epub.
+	goto end
+)
+
+if "%1" == "epub3" (
+	%SPHINXBUILD% -b epub3 %ALLSPHINXOPTS% %BUILDDIR%/epub3
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The epub3 file is in %BUILDDIR%/epub3.
+	goto end
+)
+
+if "%1" == "latex" (
+	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished; the LaTeX files are in %BUILDDIR%/latex.
+	goto end
+)
+
+if "%1" == "latexpdf" (
+	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
+	cd %BUILDDIR%/latex
+	make all-pdf
+	cd %~dp0
+	echo.
+	echo.Build finished; the PDF files are in %BUILDDIR%/latex.
+	goto end
+)
+
+if "%1" == "latexpdfja" (
+	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% %BUILDDIR%/latex
+	cd %BUILDDIR%/latex
+	make all-pdf-ja
+	cd %~dp0
+	echo.
+	echo.Build finished; the PDF files are in %BUILDDIR%/latex.
+	goto end
+)
+
+if "%1" == "text" (
+	%SPHINXBUILD% -b text %ALLSPHINXOPTS% %BUILDDIR%/text
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The text files are in %BUILDDIR%/text.
+	goto end
+)
+
+if "%1" == "man" (
+	%SPHINXBUILD% -b man %ALLSPHINXOPTS% %BUILDDIR%/man
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The manual pages are in %BUILDDIR%/man.
+	goto end
+)
+
+if "%1" == "texinfo" (
+	%SPHINXBUILD% -b texinfo %ALLSPHINXOPTS% %BUILDDIR%/texinfo
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The Texinfo files are in %BUILDDIR%/texinfo.
+	goto end
+)
+
+if "%1" == "gettext" (
+	%SPHINXBUILD% -b gettext %I18NSPHINXOPTS% %BUILDDIR%/locale
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The message catalogs are in %BUILDDIR%/locale.
+	goto end
+)
+
+if "%1" == "changes" (
+	%SPHINXBUILD% -b changes %ALLSPHINXOPTS% %BUILDDIR%/changes
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.The overview file is in %BUILDDIR%/changes.
+	goto end
+)
+
+if "%1" == "linkcheck" (
+	%SPHINXBUILD% -b linkcheck %ALLSPHINXOPTS% %BUILDDIR%/linkcheck
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Link check complete; look for any errors in the above output ^
+or in %BUILDDIR%/linkcheck/output.txt.
+	goto end
+)
+
+if "%1" == "doctest" (
+	%SPHINXBUILD% -b doctest %ALLSPHINXOPTS% %BUILDDIR%/doctest
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Testing of doctests in the sources finished, look at the ^
+results in %BUILDDIR%/doctest/output.txt.
+	goto end
+)
+
+if "%1" == "coverage" (
+	%SPHINXBUILD% -b coverage %ALLSPHINXOPTS% %BUILDDIR%/coverage
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Testing of coverage in the sources finished, look at the ^
+results in %BUILDDIR%/coverage/python.txt.
+	goto end
+)
+
+if "%1" == "xml" (
+	%SPHINXBUILD% -b xml %ALLSPHINXOPTS% %BUILDDIR%/xml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The XML files are in %BUILDDIR%/xml.
+	goto end
+)
+
+if "%1" == "pseudoxml" (
+	%SPHINXBUILD% -b pseudoxml %ALLSPHINXOPTS% %BUILDDIR%/pseudoxml
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. The pseudo-XML files are in %BUILDDIR%/pseudoxml.
+	goto end
+)
+
+if "%1" == "dummy" (
+	%SPHINXBUILD% -b dummy %ALLSPHINXOPTS% %BUILDDIR%/dummy
+	if errorlevel 1 exit /b 1
+	echo.
+	echo.Build finished. Dummy builder generates no files.
+	goto end
+)
+
+:end
```

### Comparing `mappyfile-1.0.1/docs/parser.rst` & `mappyfile-1.0.2/docs/parser.rst`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-Parsing
-=======
-
-This page documents the parsing process used by mappyfile to parse Mapfiles. 
-mappyfile uses `lark <https://github.com/lark-parser/lark>`_ as the parsing engine. 
-
-MapFile Keywords
-++++++++++++++++
-
-Links to the keywords that are used within Mapfiles:
-
-+ All the tokens used by MapServer are listed in the following file: https://github.com/mapserver/mapserver/blob/main/maplexer.l
-+ Keywords are also listed at: https://mapserver.org/mapfile/index.html
-+ There is a Sphinx RegexLexer for code formatting at https://github.com/mapserver/docs/blob/main/conf.py (see bottom of file)
-
-MapFiles
-++++++++
-
-Details on the structure of the Mapfile can be found at https://mapserver.org/mapfile/#notes:
-
-+ The Mapfile is NOT case-sensitive
-+ Strings containing non-alphanumeric characters or a MapServer keyword MUST be quoted. It is recommended to put ALL strings in double-quotes.
-+ The Mapfile has a hierarchical structure, with the MAP object being the root All other objects fall under this one.
-+ Comments are designated with a #.
-+ C-style comments were added in 2017: https://github.com/mapserver/mapserver/pull/5362 - both single line (e.g. ``/* foo */``) and multi-line comments work.
-
-Hierarchy
-+++++++++
-
-A summary of all the main Mapfile components is shown below. These are directives that are in the form ``TYPE..END``. 
-
-.. image:: images/map_classes.png
-
-The ``LAYER`` type has been split out into its own diagram due to its more complex nature:
-
-.. image:: images/layer_classes.png
-
-Mapfile Notes
-+++++++++++++
-
-This section details the various declaration types found in a Mapfile. 
-
-* Quoted strings. Used for quoted property values e.g.
-
-  .. code-block:: mapfile
-
-     NAME "Layer1"
-     DATA "lakes.shp"
-
-* Non-quoted lists. E.g. a POINTS block can be defined as follows:
-
-  .. code-block:: mapfile
-  
-      POINTS
-          0 100
-          100 200
-          40 90
-      END
-
-* Quoted lists. Used for property lists that should be quoted. E.g. the PROJECTION block can be defined as follows:
-
-  .. code-block:: mapfile
-
-      PROJECTION
-          'proj=utm'
-          'ellps=GRS80'
-          'datum=NAD83'
-          'zone=15'
-          'units=m'
-          'north'
-          'no_defs'
-      END
-
-* Key-value lists:
-
-  .. code-block:: mapfile
-
-      PROCESSING "BANDS=1"
-      PROCESSING "CONTOUR_ITEM=elevation"
-      PROCESSING "CONTOUR_INTERVAL=20"
-
-* Key-double-value lists. As above but there are two strings for each directive:
-
-  .. code-block:: mapfile
-  
-        CONFIG MS_ERRORFILE "stderr"
-        CONFIG "PROJ_DEBUG" "OFF"
-        CONFIG "ON_MISSING_DATA" "IGNORE"
-
-* Composite types- container declarations which finish with the
-  keyword END. Examples:
-    
-  .. code-block:: mapfile
-
-     MAP ... END
-     LAYER ... END
-     CLASS ... END
-     STYLE ... END
-
-
-Including Files
-+++++++++++++++
-
-The parser allows for files (containing further Mapfile declarations) referenced in the Mapfile to be loaded and parsed. Notes on the ``INCLUDE`` 
-directive can be found at https://mapserver.org/mapfile/include.html:
-
-+ Includes may be nested, up to 5 deep.
-+ File locations can be given as a full path to the file, or as a path relative to the Mapfile
-+ If a string is provided to the ``parse`` method, then an optional ``root_folder`` parameter can be used
-  to work with relative paths
-
-.. code-block:: mapfile
-
-    MAP
-        NAME "include_mapfile"
-        EXTENT 0 0 500 500
-        SIZE 250 250
-
-        INCLUDE "test_include_symbols.map"
-        INCLUDE "C:\Includes\test_include_layer.map"
-    END
-
-Parsing Notes
-+++++++++++++
-
-The Mapfile has a very flexible syntax, this section points out some of those syntax features, 
-explains their significance to parsing, and detail the solution to accommodate them.
-
-Unquoted Strings
-----------------
-
-Most programming languages insist that all strings are quoted. Unquoted strings can lead to a lot of ambiguity, as it does in the Mapfile format.
-For example, in the line:
-
-.. code-block:: mapfile
-
-    TYPE LINE
-
-It is unclear to the lexer (short for "lexical analyzer" that is responsible for converting a Mapfile into tokens)
-if ``LINE`` is a command like ``TYPE``, or a string. In this case of course it's a string, but it's left to the parser to disambiguate it. This
-is not always simple process.
-
-In our parser, we simply allowed for attribute names as a value. In post-processing, we treat them the same as strings.
-
-Composite and Attribute Ambiguity
----------------------------------
-
-Two composite names - ``STYLE`` and ``SYMBOL``, are also attribute names. For example:
-
-.. code-block:: mapfile
-
-    # a style block
-    STYLE
-        OUTLINECOLOR 0 255 0 
-    END
-
-    QUERYMAP
-        # a style attribute
-        STYLE SELECTED
-        COLOR 255 0 0
-    END
-
-This above example is not a problem to parse, but it becomes very tricky when compounded by the next issue - line-breaks.
-
-Resolving the `SYMBOL ambiguity <https://github.com/geographika/mappyfile/issues/48>`_ issue required the use of an interactive LALR
-parser. See `this commit <https://github.com/geographika/mappyfile/commit/96ca51720c6275ae1979dc6391be72fa3b0c72af>`_ for details.
-
-
-Line-Break Fluidity
--------------------
-
-On its surface, the Mapfile format appears very consistent in its line-break usage. But actually, there is a lot of variance allowed. For example:
-
-.. code-block:: mapfile
-
-    STYLE  COLOR 255 0 0  END
-
-Containers can be placed completely on one line, but also partially:
-
-.. code-block:: mapfile
-
-    LAYER DEBUG 5
-    GROUP "default"
-    ...
-    END
-
-In this example, both attributes belong to ``LAYER``, but only one of them is on the same line.
-
-In this last example, we see a culmination of all 3 issues to create a high-level of ambiguity.
-It's impossible to know if ``LAYER`` here is a composite or an attribute. Only after looking much further ahead, could a smart parser figure it out.
-
-..
-    https://news.ycombinator.com/item?id=10222681
-    http://loup-vaillant.fr/tutorials/earley-parsing/what-and-why
-    http://loup-vaillant.fr/tutorials/earley-parsing/right-recursion
+Parsing
+=======
+
+This page documents the parsing process used by mappyfile to parse Mapfiles. 
+mappyfile uses `lark <https://github.com/lark-parser/lark>`_ as the parsing engine. 
+
+MapFile Keywords
+++++++++++++++++
+
+Links to the keywords that are used within Mapfiles:
+
++ All the tokens used by MapServer are listed in the following file: https://github.com/mapserver/mapserver/blob/main/maplexer.l
++ Keywords are also listed at: https://mapserver.org/mapfile/index.html
++ There is a Sphinx RegexLexer for code formatting at https://github.com/mapserver/docs/blob/main/conf.py (see bottom of file)
+
+MapFiles
+++++++++
+
+Details on the structure of the Mapfile can be found at https://mapserver.org/mapfile/#notes:
+
++ The Mapfile is NOT case-sensitive
++ Strings containing non-alphanumeric characters or a MapServer keyword MUST be quoted. It is recommended to put ALL strings in double-quotes.
++ The Mapfile has a hierarchical structure, with the MAP object being the root All other objects fall under this one.
++ Comments are designated with a #.
++ C-style comments were added in 2017: https://github.com/mapserver/mapserver/pull/5362 - both single line (e.g. ``/* foo */``) and multi-line comments work.
+
+Hierarchy
++++++++++
+
+A summary of all the main Mapfile components is shown below. These are directives that are in the form ``TYPE..END``. 
+
+.. image:: images/map_classes.png
+
+The ``LAYER`` type has been split out into its own diagram due to its more complex nature:
+
+.. image:: images/layer_classes.png
+
+Mapfile Notes
++++++++++++++
+
+This section details the various declaration types found in a Mapfile. 
+
+* Quoted strings. Used for quoted property values e.g.
+
+  .. code-block:: mapfile
+
+     NAME "Layer1"
+     DATA "lakes.shp"
+
+* Non-quoted lists. E.g. a POINTS block can be defined as follows:
+
+  .. code-block:: mapfile
+  
+      POINTS
+          0 100
+          100 200
+          40 90
+      END
+
+* Quoted lists. Used for property lists that should be quoted. E.g. the PROJECTION block can be defined as follows:
+
+  .. code-block:: mapfile
+
+      PROJECTION
+          'proj=utm'
+          'ellps=GRS80'
+          'datum=NAD83'
+          'zone=15'
+          'units=m'
+          'north'
+          'no_defs'
+      END
+
+* Key-value lists:
+
+  .. code-block:: mapfile
+
+      PROCESSING "BANDS=1"
+      PROCESSING "CONTOUR_ITEM=elevation"
+      PROCESSING "CONTOUR_INTERVAL=20"
+
+* Key-double-value lists. As above but there are two strings for each directive:
+
+  .. code-block:: mapfile
+  
+        CONFIG MS_ERRORFILE "stderr"
+        CONFIG "PROJ_DEBUG" "OFF"
+        CONFIG "ON_MISSING_DATA" "IGNORE"
+
+* Composite types- container declarations which finish with the
+  keyword END. Examples:
+    
+  .. code-block:: mapfile
+
+     MAP ... END
+     LAYER ... END
+     CLASS ... END
+     STYLE ... END
+
+
+Including Files
++++++++++++++++
+
+The parser allows for files (containing further Mapfile declarations) referenced in the Mapfile to be loaded and parsed. Notes on the ``INCLUDE`` 
+directive can be found at https://mapserver.org/mapfile/include.html:
+
++ Includes may be nested, up to 5 deep.
++ File locations can be given as a full path to the file, or as a path relative to the Mapfile
++ If a string is provided to the ``parse`` method, then an optional ``root_folder`` parameter can be used
+  to work with relative paths
+
+.. code-block:: mapfile
+
+    MAP
+        NAME "include_mapfile"
+        EXTENT 0 0 500 500
+        SIZE 250 250
+
+        INCLUDE "test_include_symbols.map"
+        INCLUDE "C:\Includes\test_include_layer.map"
+    END
+
+Parsing Notes
++++++++++++++
+
+The Mapfile has a very flexible syntax, this section points out some of those syntax features, 
+explains their significance to parsing, and detail the solution to accommodate them.
+
+Unquoted Strings
+----------------
+
+Most programming languages insist that all strings are quoted. Unquoted strings can lead to a lot of ambiguity, as it does in the Mapfile format.
+For example, in the line:
+
+.. code-block:: mapfile
+
+    TYPE LINE
+
+It is unclear to the lexer (short for "lexical analyzer" that is responsible for converting a Mapfile into tokens)
+if ``LINE`` is a command like ``TYPE``, or a string. In this case of course it's a string, but it's left to the parser to disambiguate it. This
+is not always simple process.
+
+In our parser, we simply allowed for attribute names as a value. In post-processing, we treat them the same as strings.
+
+Composite and Attribute Ambiguity
+---------------------------------
+
+Two composite names - ``STYLE`` and ``SYMBOL``, are also attribute names. For example:
+
+.. code-block:: mapfile
+
+    # a style block
+    STYLE
+        OUTLINECOLOR 0 255 0 
+    END
+
+    QUERYMAP
+        # a style attribute
+        STYLE SELECTED
+        COLOR 255 0 0
+    END
+
+This above example is not a problem to parse, but it becomes very tricky when compounded by the next issue - line-breaks.
+
+Resolving the `SYMBOL ambiguity <https://github.com/geographika/mappyfile/issues/48>`_ issue required the use of an interactive LALR
+parser. See `this commit <https://github.com/geographika/mappyfile/commit/96ca51720c6275ae1979dc6391be72fa3b0c72af>`_ for details.
+
+
+Line-Break Fluidity
+-------------------
+
+On its surface, the Mapfile format appears very consistent in its line-break usage. But actually, there is a lot of variance allowed. For example:
+
+.. code-block:: mapfile
+
+    STYLE  COLOR 255 0 0  END
+
+Containers can be placed completely on one line, but also partially:
+
+.. code-block:: mapfile
+
+    LAYER DEBUG 5
+    GROUP "default"
+    ...
+    END
+
+In this example, both attributes belong to ``LAYER``, but only one of them is on the same line.
+
+In this last example, we see a culmination of all 3 issues to create a high-level of ambiguity.
+It's impossible to know if ``LAYER`` here is a composite or an attribute. Only after looking much further ahead, could a smart parser figure it out.
+
+..
+    https://news.ycombinator.com/item?id=10222681
+    http://loup-vaillant.fr/tutorials/earley-parsing/what-and-why
+    http://loup-vaillant.fr/tutorials/earley-parsing/right-recursion
     https://www.reddit.com/r/programming/comments/3j0zfu/fast_handy_languages_an_article_about_fast_marpa/
```

### Comparing `mappyfile-1.0.1/docs/performance.txt` & `mappyfile-1.0.2/docs/performance.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-ncalls
-    for the number of calls,
-tottime
-    for the total time spent in the given function (and excluding time made in calls to sub-functions),
-percall
-    is the quotient of tottime divided by ncalls
-cumtime
-    is the total time spent in this and all subfunctions (from invocation till exit). This figure is accurate even for recursive functions.
-percall
-    is the quotient of cumtime divided by primitive calls
-
-
-With saving:
-
-         29362467 function calls (28402404 primitive calls) in 25.749 seconds
-
-   Ordered by: internal time
-
-   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
-  1203653    5.221    0.000    5.782    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:16(__init__)
-  1203653    4.313    0.000   13.905    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:46(process)
-  1173487    1.939    0.000    2.054    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:84(epsilon_closure)
-5396271/5396270    1.019    0.000    1.026    0.000 {isinstance}
-433851/66    0.822    0.000    2.814    0.043 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:323(_visit)
-  3699185    0.794    0.000    1.636    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:40(consume_nonterminal)
-  2202385    0.620    0.000    0.837    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:296(is_stree)
-      136    0.588    0.004    0.588    0.004 {method 'close' of 'file' objects}
-    29858    0.565    0.000   14.470    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:113(advance_to)
-        1    0.547    0.547    0.547    0.547 {pyodbc.connect}
-  1051897    0.496    0.000    0.496    0.000 {getattr}
- 25816/32    0.492    0.000    2.371    0.074 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:215(_format)
-   286836    0.383    0.000    0.657    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\plyplus.py:230(_flatten)
-  1202465    0.382    0.000    0.477    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:33(consume_terminal)
-        1    0.363    0.363    0.363    0.363 {method 'execute' of 'pyodbc.Cursor' objects}
-       33    0.340    0.010   15.282    0.463 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:117(feed)
-   151240    0.297    0.000    0.938    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:30(next_state)
-   426555    0.288    0.000    0.288    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
-417978/66    0.280    0.000    2.814    0.043 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\plyplus.py:224(_visit)
-    81535    0.278    0.000    0.502    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\engine_pearley.py:38(_handle_rule)
-   269252    0.232    0.000    0.443    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:129(format_value)
-   106576    0.215    0.000    0.215    0.000 {method 'format' of 'unicode' objects}
-    71735    0.199    0.000    0.531    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\lex.py:305(token)
-  1954798    0.198    0.000    0.198    0.000 {method 'append' of 'list' objects}
- 39605/66    0.158    0.000    0.507    0.008 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:342(_transform)
-   125829    0.158    0.000    0.515    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\plyplus.py:238(rule)
-       33    0.151    0.005    0.459    0.014 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\yacc.py:1001(parseopt_notrack)
-10498/5480    0.145    0.000    0.396    0.000 C:\VirtualEnvs\mappyfile\lib\sre_parse.py:395(_parse)
-
-Creating a single parser/transformer for all EAs
-
-
-         15330143 function calls (15194176 primitive calls) in 14.956 seconds
-
-   Ordered by: internal time
-
-   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
-   639550    2.745    0.000    3.047    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:16(__init__)
-   639550    2.330    0.000    7.396    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:46(process)
-   622700    1.027    0.000    1.089    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:84(epsilon_closure)
-      137    0.593    0.004    0.593    0.004 {method 'close' of 'file' objects}
-        1    0.552    0.552    0.552    0.552 {pyodbc.connect}
-2713996/2713995    0.526    0.000    0.533    0.000 {isinstance}
- 25816/32    0.499    0.000    2.399    0.075 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:215(_format)
-  2023537    0.447    0.000    0.990    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:40(consume_nonterminal)
-        1    0.316    0.316    0.316    0.316 {method 'execute' of 'pyodbc.Cursor' objects}
-    16731    0.283    0.000    7.678    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:113(advance_to)
-   382784    0.266    0.000    0.266    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
-   269252    0.237    0.000    0.453    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:129(format_value)
-   106576    0.215    0.000    0.215    0.000 {method 'format' of 'unicode' objects}
-   639481    0.208    0.000    0.261    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:33(consume_terminal)
-        1    0.189    0.189    8.132    8.132 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:117(feed)
-       35    0.157    0.004    0.738    0.021 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\yacc.py:1001(parseopt_notrack)
-    44855    0.154    0.000    0.271    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\engine_pearley.py:38(_handle_rule)
-        1    0.148    0.148   14.955   14.955 C:\build\build_map2.py:326(run)
-    51365    0.143    0.000    0.462    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\lex.py:305(token)
-   451354    0.130    0.000    0.168    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:296(is_stree)
-    83696    0.126    0.000    0.596    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:30(next_state)
-      104    0.123    0.001    0.279    0.003 C:\Python27\Lib\ConfigParser.py:464(_read)
-
-Using Lark:
-
-         30552164 function calls (30474395 primitive calls) in 24.866 seconds
-
-   Ordered by: internal time
-
-   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
-  1197450    3.687    0.000    6.412    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:35(__init__)
-  1271377    2.532    0.000    2.532    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\tree.py:6(__init__)
-   158255    2.219    0.000    5.187    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:91(add)
-    45162    1.542    0.000    7.798    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:144(predict)
-  2393212    1.140    0.000    1.528    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:56(__hash__)
-    30038    0.846    0.000   16.572    0.001 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:152(process_column)
-  1197450    0.773    0.000    3.082    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:28(__init__)
-      136    0.689    0.005    0.689    0.005 {method 'close' of 'file' objects}
- 32376/32    0.684    0.000    4.077    0.127 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:234(_format)
-  3164403    0.679    0.000    0.679    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:41(expect)
-        1    0.590    0.590    0.590    0.590 {pyodbc.connect}
-   152617    0.574    0.000    1.104    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:49(advance)
-    82978    0.561    0.000    1.777    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:148(complete)
-2480201/2480200    0.476    0.000    0.482    0.000 {isinstance}
-  1197450    0.424    0.000    0.503    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:45(is_complete)
-        1    0.361    0.361    0.361    0.361 {method 'execute' of 'pyodbc.Cursor' objects}
-  1121918    0.358    0.000    1.039    0.000 {method 'add' of 'set' objects}
-   390132    0.330    0.000    1.159    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:128(format_value)
-   152560    0.312    0.000    0.312    0.000 {method 'format' of 'unicode' objects}
-   283204    0.308    0.000    0.470    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:156(escape_quotes)
-   836381    0.230    0.000    0.230    0.000 {method 'startswith' of 'unicode' objects}
-   101189    0.215    0.000    0.215    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
-2405543/2405447    0.209    0.000    0.209    0.000 {hash}
-   283204    0.201    0.000    0.758    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:168(standardise_quotes)
-   158224    0.200    0.000    0.876    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:181(format_key)
-  2393212    0.180    0.000    0.180    0.000 {id}
-   731520    0.172    0.000    0.172    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\common.py:111(match)
-    31261    0.168    0.000    0.448    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\lexer.py:146(lex)
-   152368    0.162    0.000    2.030    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:196(format_line)
-   298661    0.159    0.000    0.180    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:72(get_news)
-  1467680    0.157    0.000    0.157    0.000 {method 'append' of 'list' objects}
-    38832    0.152    0.000    0.270    0.000 C:\Python27\Lib\collections.py:125(items)
-    38097    0.149    0.000    0.354    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parse_tree_builder.py:31(_build_ast)
-        1    0.149    0.149   24.864   24.864 C:\Users\SG\Documents\Dropbox\Projects\LgcsbPms\PmsMapServer\pmsmapserver\build\build_map2.py:326(run)
-    33996    0.134    0.000    0.134    0.000 {method 'union' of 'frozenset' objects}
-   139596    0.132    0.000    0.174    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\tree.py:64(iter_subtrees)
-    30071    0.128    0.000    0.206    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:81(__init__)
-      104    0.122    0.001    0.281    0.003 C:\Python27\Lib\ConfigParser.py:464(_read)
-
-Using mapscript:
-
-         1588964 function calls (1588944 primitive calls) in 4.107 seconds
-
-   Ordered by: internal time
-
-   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
-       32    0.584    0.018    0.584    0.018 {_mapscript.new_mapObj}
-        1    0.547    0.547    0.547    0.547 {pyodbc.connect}
-      424    0.448    0.001    1.022    0.002 C:\Python27\Lib\ConfigParser.py:464(_read)
-        1    0.370    0.370    0.370    0.370 {imp.load_module}
-       32    0.331    0.010    0.331    0.010 {_mapscript.mapObj_save}
-        1    0.311    0.311    0.311    0.311 {method 'execute' of 'pyodbc.Cursor' objects}
-       32    0.242    0.008    0.242    0.008 {_mapscript.mapObj_setConfigOption}
-   156620    0.157    0.000    0.157    0.000 C:\Python27\Lib\collections.py:71(__setitem__)
-        1    0.141    0.141    4.107    4.107 C:\LgcsbPms\PmsMapServer\pmsmapserver\build\build_map.py:296(run)
-   151736    0.113    0.000    0.113    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
-        1    0.083    0.083    0.083    0.083 {method 'fetchall' of 'pyodbc.Cursor' objects}
-        1    0.071    0.071    1.014    1.014 .\pmsmapserver\build\engineering_areas.py:64(create_classes)
-    97205    0.067    0.000    0.067    0.000 {method 'readline' of 'file' objects}
-    80415    0.037    0.000    0.037    0.000 {method 'split' of 'str' objects}
-     6156    0.032    0.000    0.052    0.000 C:\Python27\Lib\collections.py:50(__init__)
-        1    0.030    0.030    0.418    0.418 .\mappyscript\common.py:35(setup)
-      821    0.028    0.000    0.028    0.000 {nt.stat}
-     5732    0.027    0.000    0.039    0.000 C:\Python27\Lib\collections.py:125(items)
-    88463    0.026    0.000    0.026    0.000 {method 'group' of '_sre.SRE_Match' objects}
-   152510    0.022    0.000    0.022    0.000 {method 'lower' of 'str' objects}
-      445    0.022    0.000    0.022    0.000 {open}
-   169783    0.021    0.000    0.021    0.000 {method 'str
-
-
+ncalls
+    for the number of calls,
+tottime
+    for the total time spent in the given function (and excluding time made in calls to sub-functions),
+percall
+    is the quotient of tottime divided by ncalls
+cumtime
+    is the total time spent in this and all subfunctions (from invocation till exit). This figure is accurate even for recursive functions.
+percall
+    is the quotient of cumtime divided by primitive calls
+
+
+With saving:
+
+         29362467 function calls (28402404 primitive calls) in 25.749 seconds
+
+   Ordered by: internal time
+
+   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
+  1203653    5.221    0.000    5.782    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:16(__init__)
+  1203653    4.313    0.000   13.905    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:46(process)
+  1173487    1.939    0.000    2.054    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:84(epsilon_closure)
+5396271/5396270    1.019    0.000    1.026    0.000 {isinstance}
+433851/66    0.822    0.000    2.814    0.043 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:323(_visit)
+  3699185    0.794    0.000    1.636    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:40(consume_nonterminal)
+  2202385    0.620    0.000    0.837    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:296(is_stree)
+      136    0.588    0.004    0.588    0.004 {method 'close' of 'file' objects}
+    29858    0.565    0.000   14.470    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:113(advance_to)
+        1    0.547    0.547    0.547    0.547 {pyodbc.connect}
+  1051897    0.496    0.000    0.496    0.000 {getattr}
+ 25816/32    0.492    0.000    2.371    0.074 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:215(_format)
+   286836    0.383    0.000    0.657    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\plyplus.py:230(_flatten)
+  1202465    0.382    0.000    0.477    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:33(consume_terminal)
+        1    0.363    0.363    0.363    0.363 {method 'execute' of 'pyodbc.Cursor' objects}
+       33    0.340    0.010   15.282    0.463 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:117(feed)
+   151240    0.297    0.000    0.938    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:30(next_state)
+   426555    0.288    0.000    0.288    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
+417978/66    0.280    0.000    2.814    0.043 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\plyplus.py:224(_visit)
+    81535    0.278    0.000    0.502    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\engine_pearley.py:38(_handle_rule)
+   269252    0.232    0.000    0.443    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:129(format_value)
+   106576    0.215    0.000    0.215    0.000 {method 'format' of 'unicode' objects}
+    71735    0.199    0.000    0.531    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\lex.py:305(token)
+  1954798    0.198    0.000    0.198    0.000 {method 'append' of 'list' objects}
+ 39605/66    0.158    0.000    0.507    0.008 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:342(_transform)
+   125829    0.158    0.000    0.515    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\plyplus.py:238(rule)
+       33    0.151    0.005    0.459    0.014 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\yacc.py:1001(parseopt_notrack)
+10498/5480    0.145    0.000    0.396    0.000 C:\VirtualEnvs\mappyfile\lib\sre_parse.py:395(_parse)
+
+Creating a single parser/transformer for all EAs
+
+
+         15330143 function calls (15194176 primitive calls) in 14.956 seconds
+
+   Ordered by: internal time
+
+   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
+   639550    2.745    0.000    3.047    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:16(__init__)
+   639550    2.330    0.000    7.396    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:46(process)
+   622700    1.027    0.000    1.089    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:84(epsilon_closure)
+      137    0.593    0.004    0.593    0.004 {method 'close' of 'file' objects}
+        1    0.552    0.552    0.552    0.552 {pyodbc.connect}
+2713996/2713995    0.526    0.000    0.533    0.000 {isinstance}
+ 25816/32    0.499    0.000    2.399    0.075 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:215(_format)
+  2023537    0.447    0.000    0.990    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:40(consume_nonterminal)
+        1    0.316    0.316    0.316    0.316 {method 'execute' of 'pyodbc.Cursor' objects}
+    16731    0.283    0.000    7.678    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:113(advance_to)
+   382784    0.266    0.000    0.266    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
+   269252    0.237    0.000    0.453    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:129(format_value)
+   106576    0.215    0.000    0.215    0.000 {method 'format' of 'unicode' objects}
+   639481    0.208    0.000    0.261    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:33(consume_terminal)
+        1    0.189    0.189    8.132    8.132 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:117(feed)
+       35    0.157    0.004    0.738    0.021 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\yacc.py:1001(parseopt_notrack)
+    44855    0.154    0.000    0.271    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\engine_pearley.py:38(_handle_rule)
+        1    0.148    0.148   14.955   14.955 C:\build\build_map2.py:326(run)
+    51365    0.143    0.000    0.462    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\ply\lex.py:305(token)
+   451354    0.130    0.000    0.168    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\strees.py:296(is_stree)
+    83696    0.126    0.000    0.596    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\plyplus\pearley.py:30(next_state)
+      104    0.123    0.001    0.279    0.003 C:\Python27\Lib\ConfigParser.py:464(_read)
+
+Using Lark:
+
+         30552164 function calls (30474395 primitive calls) in 24.866 seconds
+
+   Ordered by: internal time
+
+   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
+  1197450    3.687    0.000    6.412    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:35(__init__)
+  1271377    2.532    0.000    2.532    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\tree.py:6(__init__)
+   158255    2.219    0.000    5.187    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:91(add)
+    45162    1.542    0.000    7.798    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:144(predict)
+  2393212    1.140    0.000    1.528    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:56(__hash__)
+    30038    0.846    0.000   16.572    0.001 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:152(process_column)
+  1197450    0.773    0.000    3.082    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:28(__init__)
+      136    0.689    0.005    0.689    0.005 {method 'close' of 'file' objects}
+ 32376/32    0.684    0.000    4.077    0.127 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:234(_format)
+  3164403    0.679    0.000    0.679    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:41(expect)
+        1    0.590    0.590    0.590    0.590 {pyodbc.connect}
+   152617    0.574    0.000    1.104    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:49(advance)
+    82978    0.561    0.000    1.777    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:148(complete)
+2480201/2480200    0.476    0.000    0.482    0.000 {isinstance}
+  1197450    0.424    0.000    0.503    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:45(is_complete)
+        1    0.361    0.361    0.361    0.361 {method 'execute' of 'pyodbc.Cursor' objects}
+  1121918    0.358    0.000    1.039    0.000 {method 'add' of 'set' objects}
+   390132    0.330    0.000    1.159    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:128(format_value)
+   152560    0.312    0.000    0.312    0.000 {method 'format' of 'unicode' objects}
+   283204    0.308    0.000    0.470    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:156(escape_quotes)
+   836381    0.230    0.000    0.230    0.000 {method 'startswith' of 'unicode' objects}
+   101189    0.215    0.000    0.215    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
+2405543/2405447    0.209    0.000    0.209    0.000 {hash}
+   283204    0.201    0.000    0.758    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:168(standardise_quotes)
+   158224    0.200    0.000    0.876    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:181(format_key)
+  2393212    0.180    0.000    0.180    0.000 {id}
+   731520    0.172    0.000    0.172    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\common.py:111(match)
+    31261    0.168    0.000    0.448    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\lexer.py:146(lex)
+   152368    0.162    0.000    2.030    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\mappyfile\pprint.py:196(format_line)
+   298661    0.159    0.000    0.180    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:72(get_news)
+  1467680    0.157    0.000    0.157    0.000 {method 'append' of 'list' objects}
+    38832    0.152    0.000    0.270    0.000 C:\Python27\Lib\collections.py:125(items)
+    38097    0.149    0.000    0.354    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parse_tree_builder.py:31(_build_ast)
+        1    0.149    0.149   24.864   24.864 C:\Users\SG\Documents\Dropbox\Projects\LgcsbPms\PmsMapServer\pmsmapserver\build\build_map2.py:326(run)
+    33996    0.134    0.000    0.134    0.000 {method 'union' of 'frozenset' objects}
+   139596    0.132    0.000    0.174    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\tree.py:64(iter_subtrees)
+    30071    0.128    0.000    0.206    0.000 C:\VirtualEnvs\mappyfile\lib\site-packages\lark\parsers\earley.py:81(__init__)
+      104    0.122    0.001    0.281    0.003 C:\Python27\Lib\ConfigParser.py:464(_read)
+
+Using mapscript:
+
+         1588964 function calls (1588944 primitive calls) in 4.107 seconds
+
+   Ordered by: internal time
+
+   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
+       32    0.584    0.018    0.584    0.018 {_mapscript.new_mapObj}
+        1    0.547    0.547    0.547    0.547 {pyodbc.connect}
+      424    0.448    0.001    1.022    0.002 C:\Python27\Lib\ConfigParser.py:464(_read)
+        1    0.370    0.370    0.370    0.370 {imp.load_module}
+       32    0.331    0.010    0.331    0.010 {_mapscript.mapObj_save}
+        1    0.311    0.311    0.311    0.311 {method 'execute' of 'pyodbc.Cursor' objects}
+       32    0.242    0.008    0.242    0.008 {_mapscript.mapObj_setConfigOption}
+   156620    0.157    0.000    0.157    0.000 C:\Python27\Lib\collections.py:71(__setitem__)
+        1    0.141    0.141    4.107    4.107 C:\LgcsbPms\PmsMapServer\pmsmapserver\build\build_map.py:296(run)
+   151736    0.113    0.000    0.113    0.000 {method 'match' of '_sre.SRE_Pattern' objects}
+        1    0.083    0.083    0.083    0.083 {method 'fetchall' of 'pyodbc.Cursor' objects}
+        1    0.071    0.071    1.014    1.014 .\pmsmapserver\build\engineering_areas.py:64(create_classes)
+    97205    0.067    0.000    0.067    0.000 {method 'readline' of 'file' objects}
+    80415    0.037    0.000    0.037    0.000 {method 'split' of 'str' objects}
+     6156    0.032    0.000    0.052    0.000 C:\Python27\Lib\collections.py:50(__init__)
+        1    0.030    0.030    0.418    0.418 .\mappyscript\common.py:35(setup)
+      821    0.028    0.000    0.028    0.000 {nt.stat}
+     5732    0.027    0.000    0.039    0.000 C:\Python27\Lib\collections.py:125(items)
+    88463    0.026    0.000    0.026    0.000 {method 'group' of '_sre.SRE_Match' objects}
+   152510    0.022    0.000    0.022    0.000 {method 'lower' of 'str' objects}
+      445    0.022    0.000    0.022    0.000 {open}
+   169783    0.021    0.000    0.021    0.000 {method 'str
+
+
```

### Comparing `mappyfile-1.0.1/docs/pretty_printing.rst` & `mappyfile-1.0.2/docs/pretty_printing.rst`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-.. _pretty-printing:
-    
-Pretty Printing
-===============
-
-mappyfile can be used to "pretty print" or format Mapfiles. This can be used to standardise a Mapfile with inconsistent formatting. For example:
-
-.. literalinclude:: examples/before.map
-   :language: mapfile
-
-Can be converted using mappyfile to a nicely formatted version using the code below:
-
-.. literalinclude:: examples/pretty_printing.py
-   :language: python
-
-The result:
-
-.. literalinclude:: examples/after.map
-   :language: mapfile
-
-Formatting of Mapfiles can be applied using the high-level mappyfile API - see :ref:`mapfile-reader-writer-api`, 
-or using the command-line :ref:`client-format`. 
-
-Please try the online interactive demo at https://app.mapserverstudio.net/ to experiment with the various formatting options in mappyfile. 
-Documentation for MapServer Studio formatting can be found `here <https://mapserverstudio.net/help/formatting.html>`_.
-
-Options
--------
-
-The formatting of the Mapfile output can be configured with several options:
-
-+ **spacer** - the character to use for indenting structures in the Mapfile. Typically spaces or tab characters (``\\t``)
-+ **indent** - can be used to set the number of ``spacer`` characters to indent structures in the Mapfile
-+ **quote** - the quote character to use in the Mapfile (double or single quotes)
-+ **newlinechar** - the character used to insert newlines in the Mapfile
-+ **end_comment** - add a comment with the block type at each closing END statement e.g. END # MAP
-+ **align_values** - aligns the values in the same column for better readability. The column is multiple of indent and determined by the longest key
-+ **separate_complex_types** - groups composites (complex mapserver definitions with "END") together at the end. Keeps the given order except 
-  that all simple key-value pairs appear before composites.
-
-.. warning::
-
-    When standardising quotes be careful that no quotes chosen for formatting are found within string values. 
-    For example large ``DATA`` blocks of SQL may contain single quotes which would then create an invalid Mapfile. 
-
-Examples
---------
-
-The following example loads a Mapfile from a string, and then dumps it back out as a string. A single tab is used for indenting 
-blocks of the Mapfile: 
-
-.. code-block:: python
-
-    s = '''MAP NAME "TEST" END'''
-    d = mappyfile.loads(s)
-    output = mappyfile.dumps(d, indent=1, spacer="\t")
-    print(output)
-
-This example adds the block type to its closing ``END`` tag:
-
-.. code-block:: python
-
-    s = '''MAP NAME "TEST" LAYER NAME "Layer1" END END'''
-    d = mappyfile.loads(s)
-    output = mappyfile.dumps(d, end_comment=True)
-    print(output)
-
-Output:
-
-.. code-block:: mapfile
-
-    MAP
-        NAME "TEST"
-        LAYER
-            NAME "Layer1"
-        END # LAYER
-    END # MAP
-
-This example surrounds all attributes with single quotes, and writes the Mapfile directly to disk:
-
-.. code-block:: python
-
-    import tempfile
-    s = '''MAP NAME "TEST" LAYER NAME "Layer1" END END'''
-    d = mappyfile.loads(s)
-    output_file = os.path.join(tempfile.mkdtemp(), 'test_mapfile.map')
-    mappyfile.save(d, output_file)
-
-This example left-aligns all the key values of an object:
-
-.. code-block:: python
-
-    s = '''MAP NAME "MyMap"
-        OUTPUTFORMAT
-        NAME "png"
-        DRIVER AGG/PNG
-        MIMETYPE "image/png"
-        IMAGEMODE RGB
-        EXTENSION "png"
-        FORMATOPTION "GAMMA=0.75"
-        END
-        END'''
-    d = mappyfile.loads(s)
-    output = mappyfile.dumps(d, align_values=True)
-    print(output)
-
-Output:
-
-.. code-block:: mapfile
-
-    MAP
-        NAME    "MyMap"
-        OUTPUTFORMAT
-            NAME            "png"
-            DRIVER          "AGG/PNG"
-            MIMETYPE        "image/png"
-            IMAGEMODE       RGB
-            EXTENSION       "png"
-            FORMATOPTION    "GAMMA=0.75"
-        END
-    END
-
-This example moves all the simple key/value pairs of an object to the start of a declaration,
-and the complex types to the end:
-
-.. code-block:: python
-
-    s = '''MAP
-    WEB
-        METADATA
-            "wms_enable_request"            "*"
-            "wms_feature_info_mime_type"    "text/html"
-        END
-    END
-    EXTENT  -180 -90 180 90    
-    OUTPUTFORMAT
-        NAME            "png"
-        DRIVER          "AGG/PNG"
-        MIMETYPE        "image/png"
-        IMAGEMODE       RGB
-        EXTENSION       "png"
-    END
-    NAME    "MyMap"
-    END'''
-    d = mappyfile.loads(s)
-    output = mappyfile.dumps(d, separate_complex_types=True)
-    print(output)
-
-Output:
-
-.. code-block:: mapfile
-
-    MAP
-        EXTENT -180 -90 180 90
-        NAME "MyMap"
-        WEB
-            METADATA
-                "wms_enable_request" "*"
-                "wms_feature_info_mime_type" "text/html"
-            END
-        END
-        OUTPUTFORMAT
-            NAME "png"
-            DRIVER "AGG/PNG"
-            MIMETYPE "image/png"
-            IMAGEMODE RGB
-            EXTENSION "png"
-        END
-    END
-
-This example writes a Mapfile to an open file object using the ``dump`` function:
-
-.. code-block:: python
-
-    s = """MAP NAME "TEST" END"""
-    d = mappyfile.loads(s)
-    with tempfile.NamedTemporaryFile(mode="w+", delete=False) as fp:
-        mappyfile.dump(d, fp)
+.. _pretty-printing:
+    
+Pretty Printing
+===============
+
+mappyfile can be used to "pretty print" or format Mapfiles. This can be used to standardise a Mapfile with inconsistent formatting. For example:
+
+.. literalinclude:: examples/before.map
+   :language: mapfile
+
+Can be converted using mappyfile to a nicely formatted version using the code below:
+
+.. literalinclude:: examples/pretty_printing.py
+   :language: python
+
+The result:
+
+.. literalinclude:: examples/after.map
+   :language: mapfile
+
+Formatting of Mapfiles can be applied using the high-level mappyfile API - see :ref:`mapfile-reader-writer-api`, 
+or using the command-line :ref:`client-format`. 
+
+Please try the online interactive demo at https://app.mapserverstudio.net/ to experiment with the various formatting options in mappyfile. 
+Documentation for MapServer Studio formatting can be found `here <https://mapserverstudio.net/help/formatting.html>`_.
+
+Options
+-------
+
+The formatting of the Mapfile output can be configured with several options:
+
++ **spacer** - the character to use for indenting structures in the Mapfile. Typically spaces or tab characters (``\\t``)
++ **indent** - can be used to set the number of ``spacer`` characters to indent structures in the Mapfile
++ **quote** - the quote character to use in the Mapfile (double or single quotes)
++ **newlinechar** - the character used to insert newlines in the Mapfile
++ **end_comment** - add a comment with the block type at each closing END statement e.g. END # MAP
++ **align_values** - aligns the values in the same column for better readability. The column is multiple of indent and determined by the longest key
++ **separate_complex_types** - groups composites (complex mapserver definitions with "END") together at the end. Keeps the given order except 
+  that all simple key-value pairs appear before composites.
+
+.. warning::
+
+    When standardising quotes be careful that no quotes chosen for formatting are found within string values. 
+    For example large ``DATA`` blocks of SQL may contain single quotes which would then create an invalid Mapfile. 
+
+Examples
+--------
+
+The following example loads a Mapfile from a string, and then dumps it back out as a string. A single tab is used for indenting 
+blocks of the Mapfile: 
+
+.. code-block:: python
+
+    s = '''MAP NAME "TEST" END'''
+    d = mappyfile.loads(s)
+    output = mappyfile.dumps(d, indent=1, spacer="\t")
+    print(output)
+
+This example adds the block type to its closing ``END`` tag:
+
+.. code-block:: python
+
+    s = '''MAP NAME "TEST" LAYER NAME "Layer1" END END'''
+    d = mappyfile.loads(s)
+    output = mappyfile.dumps(d, end_comment=True)
+    print(output)
+
+Output:
+
+.. code-block:: mapfile
+
+    MAP
+        NAME "TEST"
+        LAYER
+            NAME "Layer1"
+        END # LAYER
+    END # MAP
+
+This example surrounds all attributes with single quotes, and writes the Mapfile directly to disk:
+
+.. code-block:: python
+
+    import tempfile
+    s = '''MAP NAME "TEST" LAYER NAME "Layer1" END END'''
+    d = mappyfile.loads(s)
+    output_file = os.path.join(tempfile.mkdtemp(), 'test_mapfile.map')
+    mappyfile.save(d, output_file)
+
+This example left-aligns all the key values of an object:
+
+.. code-block:: python
+
+    s = '''MAP NAME "MyMap"
+        OUTPUTFORMAT
+        NAME "png"
+        DRIVER AGG/PNG
+        MIMETYPE "image/png"
+        IMAGEMODE RGB
+        EXTENSION "png"
+        FORMATOPTION "GAMMA=0.75"
+        END
+        END'''
+    d = mappyfile.loads(s)
+    output = mappyfile.dumps(d, align_values=True)
+    print(output)
+
+Output:
+
+.. code-block:: mapfile
+
+    MAP
+        NAME    "MyMap"
+        OUTPUTFORMAT
+            NAME            "png"
+            DRIVER          "AGG/PNG"
+            MIMETYPE        "image/png"
+            IMAGEMODE       RGB
+            EXTENSION       "png"
+            FORMATOPTION    "GAMMA=0.75"
+        END
+    END
+
+This example moves all the simple key/value pairs of an object to the start of a declaration,
+and the complex types to the end:
+
+.. code-block:: python
+
+    s = '''MAP
+    WEB
+        METADATA
+            "wms_enable_request"            "*"
+            "wms_feature_info_mime_type"    "text/html"
+        END
+    END
+    EXTENT  -180 -90 180 90    
+    OUTPUTFORMAT
+        NAME            "png"
+        DRIVER          "AGG/PNG"
+        MIMETYPE        "image/png"
+        IMAGEMODE       RGB
+        EXTENSION       "png"
+    END
+    NAME    "MyMap"
+    END'''
+    d = mappyfile.loads(s)
+    output = mappyfile.dumps(d, separate_complex_types=True)
+    print(output)
+
+Output:
+
+.. code-block:: mapfile
+
+    MAP
+        EXTENT -180 -90 180 90
+        NAME "MyMap"
+        WEB
+            METADATA
+                "wms_enable_request" "*"
+                "wms_feature_info_mime_type" "text/html"
+            END
+        END
+        OUTPUTFORMAT
+            NAME "png"
+            DRIVER "AGG/PNG"
+            MIMETYPE "image/png"
+            IMAGEMODE RGB
+            EXTENSION "png"
+        END
+    END
+
+This example writes a Mapfile to an open file object using the ``dump`` function:
+
+.. code-block:: python
+
+    s = """MAP NAME "TEST" END"""
+    d = mappyfile.loads(s)
+    with tempfile.NamedTemporaryFile(mode="w+", delete=False) as fp:
+        mappyfile.dump(d, fp)
```

### Comparing `mappyfile-1.0.1/docs/python_integration.rst` & `mappyfile-1.0.2/docs/python_integration.rst`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Integrating with Python
-=======================
-
-This page gives some examples of integrating mappyfile into Python based work flows. 
-
-Displaying Geometry
--------------------
-
-The examples below recreates the sample images used in the `Shapely documentation <https://pypi.python.org/pypi/Shapely>`_.
-
-See :download:`geometry.py <examples/geometry/geometry.py>` and :download:`geometry.map <examples/geometry/geometry.map>`. 
-
-.. image:: images/shapely.jpg
-
-.. code-block:: python
-
-    mapfile["size"] = [600, 600]
-
-Dilated
-+++++++
-
-.. literalinclude:: examples/geometry/geometry.py
-   :pyobject: dilation
-
-.. image:: images/dilated.png
-    :scale: 80%
-
-Eroded
-++++++
-
-.. literalinclude:: examples/geometry/geometry.py
-   :pyobject: erosion
-
-.. image:: images/erosion.png
-    :scale: 80%
-
-Animated Buffers
-----------------
-
-.. image:: images/animation.gif
-
-See :download:`animated_buffer.py <examples/animation/animated_buffer.py>` and :download:`animated_buffer.map <examples/animation/animated_buffer.map>`. 
-
-..
-    Colormaps http://matplotlib.org/cmocean/
+Integrating with Python
+=======================
+
+This page gives some examples of integrating mappyfile into Python based work flows. 
+
+Displaying Geometry
+-------------------
+
+The examples below recreates the sample images used in the `Shapely documentation <https://pypi.python.org/pypi/Shapely>`_.
+
+See :download:`geometry.py <examples/geometry/geometry.py>` and :download:`geometry.map <examples/geometry/geometry.map>`. 
+
+.. image:: images/shapely.jpg
+
+.. code-block:: python
+
+    mapfile["size"] = [600, 600]
+
+Dilated
++++++++
+
+.. literalinclude:: examples/geometry/geometry.py
+   :pyobject: dilation
+
+.. image:: images/dilated.png
+    :scale: 80%
+
+Eroded
+++++++
+
+.. literalinclude:: examples/geometry/geometry.py
+   :pyobject: erosion
+
+.. image:: images/erosion.png
+    :scale: 80%
+
+Animated Buffers
+----------------
+
+.. image:: images/animation.gif
+
+See :download:`animated_buffer.py <examples/animation/animated_buffer.py>` and :download:`animated_buffer.map <examples/animation/animated_buffer.map>`. 
+
+..
+    Colormaps http://matplotlib.org/cmocean/
     https://pypi.python.org/pypi/colour
```

### Comparing `mappyfile-1.0.1/docs/rfc.rst` & `mappyfile-1.0.2/docs/rfc.rst`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-:orphan:
-
-.. _rfc123:
-
-=========================================================================
-MS RFC 123: Mapfile JSON Schema
-=========================================================================
-
-:Date:  2023/08
-:Author: Seth Girvin
-:Contact: sethg@geographika.co.uk
-:Status: Proposed
-:Version: MapServer 8.4
-
-1. Introduction and Background
-==============================
-
-Writing Mapfiles is often done by hand, and errors only become apparent when a
-map is generated from its Mapfile. This proposal recommends defining a JSON 
-schema for the full Mapfile syntax to allow for validation of a Mapfile. 
-Validating a Mapfile against a schema has the following advantages:
-
-+ warn of incorrect keywords
-+ warn of an invalid structure
-+ more comprehensive and consistent documentation
-+ warnings of deprecated keywords
-+ a parseable definition of the Mapfile language allowing the creation of Mapfile-related syntaxes
-  for the Ace Editor, Pygments, VIM etc. 
-
-In addition it is proposed metadata for each attribute is added recording
-which version of MapServer introduced a keyword, and if it has been deprecated the 
-last version it was valid. 
-
-A similar proposal was made in 2009 to introduce an XML schema for Mapfiles - 
-see RFC 51. 
-
-Storing the full Mapfile syntax in a machine-parseable format opens up other possibilities
-such as automating the generation of the Mapfile syntax documentation. 
-
-mappyfile nested dictionary structure. independent of this. Any language could be
-used to create a Mapfile JSON object for validation. Printing functionality would also 
-need to be created to convert the structure back to a Mapfile - however this step is
-much easier than the initial parsing of the Mapfile and transformation to a dictionary 
-structure. Along with the Python example in mappyfile, a JavaScript port of the pretty-printer
-class should be fairly straight-forward. 
-
-language independent
-
-mappyfile. Web and JavaScript. 
-JavaScript example. 
-
-A first pass at a JSON Schema definition for each MapServer class has been attempted
-and can be seen at TO ADD. These need to be throroughly reviewed prior to adding to 
-the MapServer repository. 
-
-UIs come and go but the Mapfile remains!
-
-2. Implementation Details
-=========================
-
-JSON4 schema. 
-
-New properties and object definitions will only be added to the schema, however no
-properties will be removed, only marked as deprecated to allow validation for different versions
-of MapServer. 
-
-This approach will also mean the schema itself won't need to be versioned
-TODO is this correct?
-Metadata deprecated property would require custom checks. 
-
-
-2.1 Schema Files
-----------------
-
-Each of the Mapfile classes - that is structures defined in the ``TYPE...END``
-blocks, will have its own JSON Schema file. For example
-a ``LAYER`` object is stored in a `layer.json <TODO ADD GITHUB LINK>`_ file. 
-
-For certain attributes that are used in different locations in a Mapfile these
-will be split out into their own schema to enable easier reuse e.g. ``EXTENT`` 
-values, ``ON`` and ``OFF`` settings, and ``COLOR`` properties. 
-
-A Python script can be provided and run as a pre-release step to the documentation builds 
-that will do the following:
-
-+ Merge the long-form documentation and JSON Schema into single documentation pages
-+ Merge all the individual JSON Schema files into a single-file for easier
-  distribution with a link to this file added to the MapServer documentation. This 
-  merged file can also be used by the latest mappyfile distribution. 
-
-2.2 Mapfile Classes
--------------------
-
-Each Mapfile class will start with the standard JSON Schema properties:
-
-.. code-block:: json
-
-    {
-        "type": "object",
-        "required": [ "type" ],
-        "additionalProperties": false,
-        "properties": {
-        }
-    }
-
-If MapServer requires any of the properties to be set, then these properties 
-are listed in ``required`` property of the object. For example without a ``LAYER`` 
-missing a ``TYPE`` property will throw an error in MapServer. 
-
-The ``additionalProperties`` property defines whether or not the object can 
-have properties not listed in the schema. In the majority of cases this will be 
-set to ``false``, as any keywords not listed in the schema will be invalid. 
-
-In cases where arbitrary keywords can be set such as ``METADATA`` and ``VALIDATION``
-objects the ``additionalProperties`` will be set to ``true``. When any values are allowed
-the JSON Schema definition is left open as follows:
-
-.. code-block:: json
-
-    {
-      "type": "object",
-      "properties": {
-      },
-      "additionalProperties": true
-    }
-
-If there is a known set of values these will be listed, along with the option to arbitrarily
-add more, e.g. the ``CONFIG`` settings:
-
-.. code-block:: json
-
-    {
-        "config": {
-          "type": "object",
-          "properties": {
-            "CGI_CONTEXT_URL": { "type": "string" },
-            "MS_ENCRYPTION_KEY": { "type": "string" },
-            "ON_MISSING_DATA": {
-              "type": "string",
-              "enum": [ "FAIL", "LOG", "IGNORE" ]
-            },
-          },
-          "additionalProperties": true
-         }
-     }
-
-If any of the properties in a class are themselves classes then they will be 
-referenced using the ``$ref`` property pointing to the relevant .json file. For example
-a ``LAYER`` can contain a ``METADATA`` object. This schema is referenced as
-follows:
-
-.. code-block:: json
-
-    {
-        "metadata": {
-          "$ref": "metadata.json"
-        }
-    }
-
-+ TODO add "include":  "string"
-+ Can't include   "required": [ "type" ] in layer as this could be in an include
-+ "__position__"
-
-2.3 Arrays of Mapfile Classes
------------------------------
-
-Several Mapfile classes can be repeated within their parent class, for 
-example a ``LAYER`` can have many ``CLASS`` objects, or several ``FEATURE``
-objects. In these cases the property name will be set to the plural, and will
-be of type ``array``:
-
-.. code-block:: json
-
-    {
-        "features": {
-          "type": "array",
-          "items": {
-            "$ref": "feature.json"
-          }
-        }
-    }
-
-In most cases this will be simply be adding an "s" e.g. feature(s), layer(s). 
-In the case where the property already ends with an "s", then "es" will be used,
-e.g. class(es). 
-
-2.4 Property Definitions
-------------------------
-
-Most property definitions are self-explanatory, for example a ``MAP`` can have
-an ``ANGLE`` property, and a ``LEGEND`` can have a ``STATUS`` property. 
-These are of type ``numeric``, ``string``, and ``enumeration`` respectively. 
-
-.. code-block:: json
-
-    {
-        "angle": {
-          "type": "number"
-        },
-        "imagetype": {
-          "type": "string"
-        },
-        "status": {
-          "type": "string",
-          "enum": [ "on", "off", "embed" ]
-        }
-    }
-
-Other properties are more complicated. For example the ``COLOR`` property is used
-in several locations in the Mapfile. This can accept either an RGBA value, or an
-HTML color code. 
-
-.. code-block:: json
-
-    {
-      "oneOf": [
-        {
-          "type": "array",
-          "items": {
-            "type": "number",
-            "minimum": 0,
-            "maximum": 255
-          },
-          "minItems": 3,
-          "maxItems": 3
-        },
-        {
-          "pattern": "^#([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$",
-          "example": "#aa33cc",
-          "type": "string"
-        }
-      ]
-    }
-
-
-2.5 Property Metadata
----------------------
-
-The recommended approach to storing metadata in a JSON schema is in 
-a ``metadata`` attribute TODO ADD LINK. Metadata will only be added for attributes which 
-have been deprecated or recently introduced in to the Mapfile syntax. Recent is defined here 
-as if it is still currently mentioned in the documentation. 
-
-For example the ``LABELMAXSCALE`` attribute on a ``LAYER`` object was deprecated
-in MapServer version 5.0 (according to the documentation). Without digging into the 
-source code history the version the attribute was introduced is unknown. In this case the
-``minVersion`` will be set to 0. 
-
-.. code-block:: json
-
-    {
-        "labelmaxscale": {
-          "type": "number",
-          "metadata": {
-            "deprecated": true,
-            "minVersion": 0,
-            "maxVersion": 5.0
-          }
-        }
-    }
-
-Another standard JSON Schema property that will be used occastionally in the
-schema is the ``example`` property TODO ADD LINK. This will primarily be used 
-to document examples of valid values to list in the MapServer documentation. 
-For example one of the valid values for a ``COLOR`` property is an HTML color code. 
-An example value is listed in the property definition. 
-
-.. code-block:: json
-
-    {
-        "pattern": "^#([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$",
-        "example": "#aa33cc",
-        "type": "string"
-    }
-
-3. Documentation Changes
-========================
-
-Currently the MapServer Mapfile syntax is documented in restructured text (RST). 
-
-The `jsonschema2rst <https://github.com/inspirehep/jsonschema2rst>`_ project converts a 
-JSON schema into RST. 
-
-It is proposed that the current document's structure is modified to make it easier to comnbine
-the existing long-form documentation, with the JSON Schema details, and removing any
-duplication between the two. 
-
-It is important the long-form text can be easily edited and examples added, so this approach
-aims to enhance the hand-written documentation rather than replace it. 
-
-This would avoid issues such as https://github.com/mapserver/mapserver/issues/5748
-
-4. Online Validator
-===================
-
-JavaScript-based validator?
-Select version. Default to latest (7.2). 
-
-5. Implementation Details
-=========================
-
-5.1 Affected files
-------------------
-
-+ no code files will require modifications
-+ all documentation in the ``/mapfile`` folder could gradually be restructured
-  to allow the insertion of property definitions from the JSON Schema
-
-5.2 Tracking Issue
-------------------
-
-TBD
-
-6. Discussion
-=============
-
-+ Multipoints
-+ Use of __type__ attributes?
-+ Are there any other attribute or type metadata values that could / should
-  be stored?
-
-7. Voting History
-=================
-
+:orphan:
+
+.. _rfc123:
+
+=========================================================================
+MS RFC 123: Mapfile JSON Schema
+=========================================================================
+
+:Date:  2023/08
+:Author: Seth Girvin
+:Contact: sethg@geographika.co.uk
+:Status: Proposed
+:Version: MapServer 8.4
+
+1. Introduction and Background
+==============================
+
+Writing Mapfiles is often done by hand, and errors only become apparent when a
+map is generated from its Mapfile. This proposal recommends defining a JSON 
+schema for the full Mapfile syntax to allow for validation of a Mapfile. 
+Validating a Mapfile against a schema has the following advantages:
+
++ warn of incorrect keywords
++ warn of an invalid structure
++ more comprehensive and consistent documentation
++ warnings of deprecated keywords
++ a parseable definition of the Mapfile language allowing the creation of Mapfile-related syntaxes
+  for the Ace Editor, Pygments, VIM etc. 
+
+In addition it is proposed metadata for each attribute is added recording
+which version of MapServer introduced a keyword, and if it has been deprecated the 
+last version it was valid. 
+
+A similar proposal was made in 2009 to introduce an XML schema for Mapfiles - 
+see RFC 51. 
+
+Storing the full Mapfile syntax in a machine-parseable format opens up other possibilities
+such as automating the generation of the Mapfile syntax documentation. 
+
+mappyfile nested dictionary structure. independent of this. Any language could be
+used to create a Mapfile JSON object for validation. Printing functionality would also 
+need to be created to convert the structure back to a Mapfile - however this step is
+much easier than the initial parsing of the Mapfile and transformation to a dictionary 
+structure. Along with the Python example in mappyfile, a JavaScript port of the pretty-printer
+class should be fairly straight-forward. 
+
+language independent
+
+mappyfile. Web and JavaScript. 
+JavaScript example. 
+
+A first pass at a JSON Schema definition for each MapServer class has been attempted
+and can be seen at TO ADD. These need to be throroughly reviewed prior to adding to 
+the MapServer repository. 
+
+UIs come and go but the Mapfile remains!
+
+2. Implementation Details
+=========================
+
+JSON4 schema. 
+
+New properties and object definitions will only be added to the schema, however no
+properties will be removed, only marked as deprecated to allow validation for different versions
+of MapServer. 
+
+This approach will also mean the schema itself won't need to be versioned
+TODO is this correct?
+Metadata deprecated property would require custom checks. 
+
+
+2.1 Schema Files
+----------------
+
+Each of the Mapfile classes - that is structures defined in the ``TYPE...END``
+blocks, will have its own JSON Schema file. For example
+a ``LAYER`` object is stored in a `layer.json <TODO ADD GITHUB LINK>`_ file. 
+
+For certain attributes that are used in different locations in a Mapfile these
+will be split out into their own schema to enable easier reuse e.g. ``EXTENT`` 
+values, ``ON`` and ``OFF`` settings, and ``COLOR`` properties. 
+
+A Python script can be provided and run as a pre-release step to the documentation builds 
+that will do the following:
+
++ Merge the long-form documentation and JSON Schema into single documentation pages
++ Merge all the individual JSON Schema files into a single-file for easier
+  distribution with a link to this file added to the MapServer documentation. This 
+  merged file can also be used by the latest mappyfile distribution. 
+
+2.2 Mapfile Classes
+-------------------
+
+Each Mapfile class will start with the standard JSON Schema properties:
+
+.. code-block:: json
+
+    {
+        "type": "object",
+        "required": [ "type" ],
+        "additionalProperties": false,
+        "properties": {
+        }
+    }
+
+If MapServer requires any of the properties to be set, then these properties 
+are listed in ``required`` property of the object. For example without a ``LAYER`` 
+missing a ``TYPE`` property will throw an error in MapServer. 
+
+The ``additionalProperties`` property defines whether or not the object can 
+have properties not listed in the schema. In the majority of cases this will be 
+set to ``false``, as any keywords not listed in the schema will be invalid. 
+
+In cases where arbitrary keywords can be set such as ``METADATA`` and ``VALIDATION``
+objects the ``additionalProperties`` will be set to ``true``. When any values are allowed
+the JSON Schema definition is left open as follows:
+
+.. code-block:: json
+
+    {
+      "type": "object",
+      "properties": {
+      },
+      "additionalProperties": true
+    }
+
+If there is a known set of values these will be listed, along with the option to arbitrarily
+add more, e.g. the ``CONFIG`` settings:
+
+.. code-block:: json
+
+    {
+        "config": {
+          "type": "object",
+          "properties": {
+            "CGI_CONTEXT_URL": { "type": "string" },
+            "MS_ENCRYPTION_KEY": { "type": "string" },
+            "ON_MISSING_DATA": {
+              "type": "string",
+              "enum": [ "FAIL", "LOG", "IGNORE" ]
+            },
+          },
+          "additionalProperties": true
+         }
+     }
+
+If any of the properties in a class are themselves classes then they will be 
+referenced using the ``$ref`` property pointing to the relevant .json file. For example
+a ``LAYER`` can contain a ``METADATA`` object. This schema is referenced as
+follows:
+
+.. code-block:: json
+
+    {
+        "metadata": {
+          "$ref": "metadata.json"
+        }
+    }
+
++ TODO add "include":  "string"
++ Can't include   "required": [ "type" ] in layer as this could be in an include
++ "__position__"
+
+2.3 Arrays of Mapfile Classes
+-----------------------------
+
+Several Mapfile classes can be repeated within their parent class, for 
+example a ``LAYER`` can have many ``CLASS`` objects, or several ``FEATURE``
+objects. In these cases the property name will be set to the plural, and will
+be of type ``array``:
+
+.. code-block:: json
+
+    {
+        "features": {
+          "type": "array",
+          "items": {
+            "$ref": "feature.json"
+          }
+        }
+    }
+
+In most cases this will be simply be adding an "s" e.g. feature(s), layer(s). 
+In the case where the property already ends with an "s", then "es" will be used,
+e.g. class(es). 
+
+2.4 Property Definitions
+------------------------
+
+Most property definitions are self-explanatory, for example a ``MAP`` can have
+an ``ANGLE`` property, and a ``LEGEND`` can have a ``STATUS`` property. 
+These are of type ``numeric``, ``string``, and ``enumeration`` respectively. 
+
+.. code-block:: json
+
+    {
+        "angle": {
+          "type": "number"
+        },
+        "imagetype": {
+          "type": "string"
+        },
+        "status": {
+          "type": "string",
+          "enum": [ "on", "off", "embed" ]
+        }
+    }
+
+Other properties are more complicated. For example the ``COLOR`` property is used
+in several locations in the Mapfile. This can accept either an RGBA value, or an
+HTML color code. 
+
+.. code-block:: json
+
+    {
+      "oneOf": [
+        {
+          "type": "array",
+          "items": {
+            "type": "number",
+            "minimum": 0,
+            "maximum": 255
+          },
+          "minItems": 3,
+          "maxItems": 3
+        },
+        {
+          "pattern": "^#([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$",
+          "example": "#aa33cc",
+          "type": "string"
+        }
+      ]
+    }
+
+
+2.5 Property Metadata
+---------------------
+
+The recommended approach to storing metadata in a JSON schema is in 
+a ``metadata`` attribute TODO ADD LINK. Metadata will only be added for attributes which 
+have been deprecated or recently introduced in to the Mapfile syntax. Recent is defined here 
+as if it is still currently mentioned in the documentation. 
+
+For example the ``LABELMAXSCALE`` attribute on a ``LAYER`` object was deprecated
+in MapServer version 5.0 (according to the documentation). Without digging into the 
+source code history the version the attribute was introduced is unknown. In this case the
+``minVersion`` will be set to 0. 
+
+.. code-block:: json
+
+    {
+        "labelmaxscale": {
+          "type": "number",
+          "metadata": {
+            "deprecated": true,
+            "minVersion": 0,
+            "maxVersion": 5.0
+          }
+        }
+    }
+
+Another standard JSON Schema property that will be used occastionally in the
+schema is the ``example`` property TODO ADD LINK. This will primarily be used 
+to document examples of valid values to list in the MapServer documentation. 
+For example one of the valid values for a ``COLOR`` property is an HTML color code. 
+An example value is listed in the property definition. 
+
+.. code-block:: json
+
+    {
+        "pattern": "^#([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$",
+        "example": "#aa33cc",
+        "type": "string"
+    }
+
+3. Documentation Changes
+========================
+
+Currently the MapServer Mapfile syntax is documented in restructured text (RST). 
+
+The `jsonschema2rst <https://github.com/inspirehep/jsonschema2rst>`_ project converts a 
+JSON schema into RST. 
+
+It is proposed that the current document's structure is modified to make it easier to comnbine
+the existing long-form documentation, with the JSON Schema details, and removing any
+duplication between the two. 
+
+It is important the long-form text can be easily edited and examples added, so this approach
+aims to enhance the hand-written documentation rather than replace it. 
+
+This would avoid issues such as https://github.com/mapserver/mapserver/issues/5748
+
+4. Online Validator
+===================
+
+JavaScript-based validator?
+Select version. Default to latest (7.2). 
+
+5. Implementation Details
+=========================
+
+5.1 Affected files
+------------------
+
++ no code files will require modifications
++ all documentation in the ``/mapfile`` folder could gradually be restructured
+  to allow the insertion of property definitions from the JSON Schema
+
+5.2 Tracking Issue
+------------------
+
+TBD
+
+6. Discussion
+=============
+
++ Multipoints
++ Use of __type__ attributes?
++ Are there any other attribute or type metadata values that could / should
+  be stored?
+
+7. Voting History
+=================
+
```

### Comparing `mappyfile-1.0.1/docs/schemas.rst` & `mappyfile-1.0.2/docs/schemas.rst`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-.. _mapfile-schema:
-
-Mapfile Schema
-==============
-
-The full Mapfile schema can be downloaded directly from this link - :download:`mapfile-latest.json <schemas/mapfile-latest.json>`. 
-The schema stores ``minVersion`` and ``maxVersion`` properties in a ``metadata`` object for each keyword. This allow Mapfiles to be validated against
-older or newer releases of MapServer to see if they are still valid. 
-
-Other versions available online are:
-
-+ :download:`mapfile-schema-8-0.json <schemas/mapfile-schema-8-0.json>`
-+ :download:`mapfile-schema-7-6.json <schemas/mapfile-schema-7-6.json>`
-
-The Mapfile schema shown below is planned to be proposed as an official Mapfile language schema, subject to voting by the MapServer
-PSC (Project Steering Committee). Further details on the schema are outlined in the draft RFC (Request for Comment) at :ref:`rfc123`. 
-
-Exporting the Schema
-++++++++++++++++++++
-
-The schema can be exported to a file via the command-line using the following syntax:
-
-.. code-block:: ps1
-
-    # exports to mapfile-schema-8-0.json
-    mappyfile schema mapfile-schema-8-0.json --version=8.0
-
-The schema can be exported using Python, as shown in the example below:
-
-.. code-block:: python
-
-    import json
-    from mappyfile.validator import Validator
-
-    validator = Validator()
-    jsn = validator.get_versioned_schema(version=8.0)
-    print(json.dumps(jsn, indent=4))
-
-Creating a Mappyfile Object with Defaults
-+++++++++++++++++++++++++++++++++++++++++
-
-If MapServer uses default values for an object, the `create` function can be used to create
-a new object using these defaults. For example to output a `MAP` object with default settings
-run the following code:
-
-.. code-block:: python
-
-    import mappyfile
-
-    m = mappyfile.create("map", version=8.0)
-    print(m)
-    mappyfile.dumps(m)
-
-This outputs the following:
-
-.. code-block:: mapfile
-
-    MAP
-        ANGLE 0
-        DEBUG 0
-        DEFRESOLUTION 72
-        IMAGETYPE "png"
-        MAXSIZE 4096
-        NAME "MS"
-        RESOLUTION 72
-        SIZE -1 -1
-    END
-
-Notes
------
-
-``enum`` is used to check attribute keywords, and output them without quotes by the pretty printer. The ``CLUSTER`` ``REGION`` keyword
-is a fixed list, but has to be a string and output in quotes, therefore the following construct is used:
-
-.. code-block:: json
-
-    "type": "string",
-    "pattern": "^rectangle$"
-
-..
-    For docs: https://github.com/inspirehep/jsonschema2rst
-    Could have different schema for different purposes, e.g. a valid WMS schema. 
+.. _mapfile-schema:
+
+Mapfile Schema
+==============
+
+The full Mapfile schema can be downloaded directly from this link - :download:`mapfile-latest.json <schemas/mapfile-latest.json>`. 
+The schema stores ``minVersion`` and ``maxVersion`` properties in a ``metadata`` object for each keyword. This allow Mapfiles to be validated against
+older or newer releases of MapServer to see if they are still valid. 
+
+Other versions available online are:
+
++ :download:`mapfile-schema-8-0.json <schemas/mapfile-schema-8-0.json>`
++ :download:`mapfile-schema-7-6.json <schemas/mapfile-schema-7-6.json>`
+
+The Mapfile schema shown below is planned to be proposed as an official Mapfile language schema, subject to voting by the MapServer
+PSC (Project Steering Committee). Further details on the schema are outlined in the draft RFC (Request for Comment) at :ref:`rfc123`. 
+
+Exporting the Schema
+++++++++++++++++++++
+
+The schema can be exported to a file via the command-line using the following syntax:
+
+.. code-block:: ps1
+
+    # exports to mapfile-schema-8-0.json
+    mappyfile schema mapfile-schema-8-0.json --version=8.0
+
+The schema can be exported using Python, as shown in the example below:
+
+.. code-block:: python
+
+    import json
+    from mappyfile.validator import Validator
+
+    validator = Validator()
+    jsn = validator.get_versioned_schema(version=8.0)
+    print(json.dumps(jsn, indent=4))
+
+Creating a Mappyfile Object with Defaults
++++++++++++++++++++++++++++++++++++++++++
+
+If MapServer uses default values for an object, the `create` function can be used to create
+a new object using these defaults. For example to output a `MAP` object with default settings
+run the following code:
+
+.. code-block:: python
+
+    import mappyfile
+
+    m = mappyfile.create("map", version=8.0)
+    print(m)
+    mappyfile.dumps(m)
+
+This outputs the following:
+
+.. code-block:: mapfile
+
+    MAP
+        ANGLE 0
+        DEBUG 0
+        DEFRESOLUTION 72
+        IMAGETYPE "png"
+        MAXSIZE 4096
+        NAME "MS"
+        RESOLUTION 72
+        SIZE -1 -1
+    END
+
+Notes
+-----
+
+``enum`` is used to check attribute keywords, and output them without quotes by the pretty printer. The ``CLUSTER`` ``REGION`` keyword
+is a fixed list, but has to be a string and output in quotes, therefore the following construct is used:
+
+.. code-block:: json
+
+    "type": "string",
+    "pattern": "^rectangle$"
+
+..
+    For docs: https://github.com/inspirehep/jsonschema2rst
+    Could have different schema for different purposes, e.g. a valid WMS schema. 
     Nested schemas are in the Draft 4 spec only - https://spacetelescope.github.io/understanding-json-schema/structuring.html
```

### Comparing `mappyfile-1.0.1/docs/testing.rst` & `mappyfile-1.0.2/docs/testing.rst`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-.. _testing:
-
-Testing mappyfile
-=================
-
-There are two main objectives to testing mappyfile. 
-
-#. Check that mappyfile can parse all the test Mapfiles in the test suite. 
-#. Check that mappyfile can parse the Mapfile, pretty print it to a new file, run the tests on the new file, and check that the output is the same
-   as the original. 
-
-The Mapfiles won't be identical as comments will be stripped, and whitespace will change. They should however produce the same results. 
-MapServer has a full set of regression tests - `msautotest <https://mapserver.org/development/tests/autotest.html>`_
-that includes 100s of Mapfiles. For example:
-
-+ https://github.com/mapserver/mapserver/tree/main/msautotest/misc
-+ https://github.com/mapserver/mapserver/tree/main/msautotest/wxs
-+ https://github.com/mapserver/mapserver/tree/main/msautotest/renderers
-+ https://github.com/mapserver/mapserver/tree/main/msautotest/gdal
-
-These have been downloaded and added to the ``/tests/sample_maps`` folder and are tested as part of the automated pytest test suite. 
-Includes are not currently included - extension names of include files differ - sometimes ``.map`` and sometimes ``.include``. In addition they are sometimes
-stored in an ``includes`` folder, and sometimes in a ``data`` folder. These includes are currently added to an ``ignore_list`` in the
-`test_sample_maps.py <https://github.com/geographika/mappyfile/blob/master/tests/test_sample_maps.py>`_ test file.
-
-A second test file `test_msautotest.py <https://github.com/geographika/mappyfile/blob/master/tests/test_msautotest.py>`_ can be pointed to
-a clone of the MapServer repository, and parses them, writes them to a new file, and then parses the new output. This is a good check that
-the mappyfile pretty-print output remains valid. 
-
-Running the Test Suite
-----------------------
-
-The test suite can be run to check that the mappyfile outputs not only pass the mappyfile parsing and validation steps, but also
-pass being loaded by MapServer and run as part of msautotest. The steps below can be run on Windows using PowerShell.
-Note however that due to image output differences between Windows and the expected reference images generated by Linux there will be lots
-of failures.
-
-.. code-block:: ps1
-
-    $MSAUTOTEST_ROOT="D:\GitHub\mapserver\msautotest"
-    C:\Python310\Scripts\virtualenv C:\VirtualEnvs\msautotest
-    C:\VirtualEnvs\msautotest\Scripts\activate.ps1
-    pip install lxml
-    pip install future
-    pip install pytest
-
-    $env:PATH="C:\MapServer\bin;$env:PATH"
-    $env:MAPSERVER_CONFIG_FILE="C:\MapServer\apps\mapserver.conf"
-
-    cd $MSAUTOTEST_ROOT
-    python python pymod/xmlvalidate.py -download_ogc_schemas
-
-    cd $MSAUTOTEST_ROOT\gdal
-    new-item -itemtype symboliclink -path . -name SCHEMAS_OPENGIS_NET -value $MSAUTOTEST_ROOT\SCHEMAS_OPENGIS_NET
-    # can add -v for verbose output to the command below
-    python.exe run_test.py
-
-    cd $MSAUTOTEST_ROOT\misc
-    new-item -itemtype symboliclink -path . -name SCHEMAS_OPENGIS_NET -value $MSAUTOTEST_ROOT\SCHEMAS_OPENGIS_NET
-    python.exe run_test.py
-
-    # now run on mappyfile generated Mapfiles - error count should match
-    # switch to the copied output folder defined in test_msautotest.py
-    cd D:\GitHub\mapserver\msautotest_mappyfile\misc
-    new-item -itemtype symboliclink -path . -name SCHEMAS_OPENGIS_NET -value $MSAUTOTEST_ROOT\SCHEMAS_OPENGIS_NET
-    python.exe run_test.py
-
+.. _testing:
+
+Testing mappyfile
+=================
+
+There are two main objectives to testing mappyfile. 
+
+#. Check that mappyfile can parse all the test Mapfiles in the test suite. 
+#. Check that mappyfile can parse the Mapfile, pretty print it to a new file, run the tests on the new file, and check that the output is the same
+   as the original. 
+
+The Mapfiles won't be identical as comments will be stripped, and whitespace will change. They should however produce the same results. 
+MapServer has a full set of regression tests - `msautotest <https://mapserver.org/development/tests/autotest.html>`_
+that includes 100s of Mapfiles. For example:
+
++ https://github.com/mapserver/mapserver/tree/main/msautotest/misc
++ https://github.com/mapserver/mapserver/tree/main/msautotest/wxs
++ https://github.com/mapserver/mapserver/tree/main/msautotest/renderers
++ https://github.com/mapserver/mapserver/tree/main/msautotest/gdal
+
+These have been downloaded and added to the ``/tests/sample_maps`` folder and are tested as part of the automated pytest test suite. 
+Includes are not currently included - extension names of include files differ - sometimes ``.map`` and sometimes ``.include``. In addition they are sometimes
+stored in an ``includes`` folder, and sometimes in a ``data`` folder. These includes are currently added to an ``ignore_list`` in the
+`test_sample_maps.py <https://github.com/geographika/mappyfile/blob/master/tests/test_sample_maps.py>`_ test file.
+
+A second test file `test_msautotest.py <https://github.com/geographika/mappyfile/blob/master/tests/test_msautotest.py>`_ can be pointed to
+a clone of the MapServer repository, and parses them, writes them to a new file, and then parses the new output. This is a good check that
+the mappyfile pretty-print output remains valid. 
+
+Running the Test Suite
+----------------------
+
+The test suite can be run to check that the mappyfile outputs not only pass the mappyfile parsing and validation steps, but also
+pass being loaded by MapServer and run as part of msautotest. The steps below can be run on Windows using PowerShell.
+Note however that due to image output differences between Windows and the expected reference images generated by Linux there will be lots
+of failures.
+
+.. code-block:: ps1
+
+    $MSAUTOTEST_ROOT="D:\GitHub\mapserver\msautotest"
+    C:\Python310\Scripts\virtualenv C:\VirtualEnvs\msautotest
+    C:\VirtualEnvs\msautotest\Scripts\activate.ps1
+    pip install lxml
+    pip install future
+    pip install pytest
+
+    $env:PATH="C:\MapServer\bin;$env:PATH"
+    $env:MAPSERVER_CONFIG_FILE="C:\MapServer\apps\mapserver.conf"
+
+    cd $MSAUTOTEST_ROOT
+    python python pymod/xmlvalidate.py -download_ogc_schemas
+
+    cd $MSAUTOTEST_ROOT\gdal
+    new-item -itemtype symboliclink -path . -name SCHEMAS_OPENGIS_NET -value $MSAUTOTEST_ROOT\SCHEMAS_OPENGIS_NET
+    # can add -v for verbose output to the command below
+    python.exe run_test.py
+
+    cd $MSAUTOTEST_ROOT\misc
+    new-item -itemtype symboliclink -path . -name SCHEMAS_OPENGIS_NET -value $MSAUTOTEST_ROOT\SCHEMAS_OPENGIS_NET
+    python.exe run_test.py
+
+    # now run on mappyfile generated Mapfiles - error count should match
+    # switch to the copied output folder defined in test_msautotest.py
+    cd D:\GitHub\mapserver\msautotest_mappyfile\misc
+    new-item -itemtype symboliclink -path . -name SCHEMAS_OPENGIS_NET -value $MSAUTOTEST_ROOT\SCHEMAS_OPENGIS_NET
+    python.exe run_test.py
+
```

### Comparing `mappyfile-1.0.1/docs/transformer.rst` & `mappyfile-1.0.2/docs/transformer.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-.. _transformer:
-
-Transforming
-============
-
-mappyfile parses a Mapfile and turns it into a Abstract Syntax Tree (AST). The mappyfile
-`transformer class <https://github.com/geographika/mappyfile/blob/master/mappyfile/transformer.py>`_ then turns this tree into a Python dictionary. 
-Using a dictionary provides the Python developer with a familiar data structure that can be used to edit the Mapfile further - see :ref:`editing`.
-
-For example taking the Mapfile below:
-
-.. literalinclude:: examples/after.map
-   :language: mapfile
-
-The following code can be used to see the dictionary structure (represented here as a JSON object):
-
-.. literalinclude:: examples/sample_json.py
-   :language: python
-
-Output:
-
-.. literalinclude:: examples/sample.json
-   :language: json
-
-Some notes on the above:
-
-+ Objects that can have multiple instances (for example ``LAYER`` and ``CLASS`` in a Mapfile will be stored in lists (order is important).
-+ Most objects have a set of key/value pairs. ``PROJECTION`` however is treated as a list 
-  (see http://www.mapserver.org/mapfile/projection.html).
-+ Some keys are already quoted e.g. in the ``METADATA`` object items such as "wms_enable_request" are strings rather than keywords.
-+ Some keys are duplicated within an object. E.g.
-
-  .. code-block:: mapfile
-  
-        PROCESSING "BANDS=1"
-        PROCESSING "CONTOUR_ITEM=elevation"
-        PROCESSING "CONTOUR_INTERVAL=20"
-        
-  These are turned into lists:
-    
-  .. code-block:: json
-  
-    "processing": [
-        "'BANDS=1'", 
-        "'CONTOUR_ITEM=elevation'", 
-        "'CONTOUR_INTERVAL=20'"
-    ], 
-  
-
-Python dictionaries map closely to JSON data structures, which means the Mapfile dictionary 
-structure can be formalised into a JSONSchema. See :ref:`mapfile-schema` for more details, and also the draft MapServer
-proposal :ref:`rfc123`.
-
-Mappyfile Additions
--------------------
-
-In order to ensure that no information is lost when inputting and outputting a Mapfile,
-mappyfile makes use of hidden properties to store additional data. This data is
-not outputted as part of the pretty-print. For example a hidden property is used to store objects of the 
-same type e.g. ``LAYER``, ``CLASS``, and ``STYLE``.
+.. _transformer:
+
+Transforming
+============
+
+mappyfile parses a Mapfile and turns it into a Abstract Syntax Tree (AST). The mappyfile
+`transformer class <https://github.com/geographika/mappyfile/blob/master/mappyfile/transformer.py>`_ then turns this tree into a Python dictionary. 
+Using a dictionary provides the Python developer with a familiar data structure that can be used to edit the Mapfile further - see :ref:`editing`.
+
+For example taking the Mapfile below:
+
+.. literalinclude:: examples/after.map
+   :language: mapfile
+
+The following code can be used to see the dictionary structure (represented here as a JSON object):
+
+.. literalinclude:: examples/sample_json.py
+   :language: python
+
+Output:
+
+.. literalinclude:: examples/sample.json
+   :language: json
+
+Some notes on the above:
+
++ Objects that can have multiple instances (for example ``LAYER`` and ``CLASS`` in a Mapfile will be stored in lists (order is important).
++ Most objects have a set of key/value pairs. ``PROJECTION`` however is treated as a list 
+  (see http://www.mapserver.org/mapfile/projection.html).
++ Some keys are already quoted e.g. in the ``METADATA`` object items such as "wms_enable_request" are strings rather than keywords.
++ Some keys are duplicated within an object. E.g.
+
+  .. code-block:: mapfile
+  
+        PROCESSING "BANDS=1"
+        PROCESSING "CONTOUR_ITEM=elevation"
+        PROCESSING "CONTOUR_INTERVAL=20"
+        
+  These are turned into lists:
+    
+  .. code-block:: json
+  
+    "processing": [
+        "'BANDS=1'", 
+        "'CONTOUR_ITEM=elevation'", 
+        "'CONTOUR_INTERVAL=20'"
+    ], 
+  
+
+Python dictionaries map closely to JSON data structures, which means the Mapfile dictionary 
+structure can be formalised into a JSONSchema. See :ref:`mapfile-schema` for more details, and also the draft MapServer
+proposal :ref:`rfc123`.
+
+Mappyfile Additions
+-------------------
+
+In order to ensure that no information is lost when inputting and outputting a Mapfile,
+mappyfile makes use of hidden properties to store additional data. This data is
+not outputted as part of the pretty-print. For example a hidden property is used to store objects of the 
+same type e.g. ``LAYER``, ``CLASS``, and ``STYLE``.
```

### Comparing `mappyfile-1.0.1/docs/validate.txt` & `mappyfile-1.0.2/docs/validate.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Usage: mappyfile validate [OPTIONS] [MAPFILES]...
-
-  Validate Mapfile(s) against the Mapfile schema
-
-  The MAPFILES argument is a list of paths, either to individual Mapfiles,
-  or a folders containing Mapfiles.  Wildcards are supported (natively on
-  Linux, and up to one level deep on Windows). Validation errors are
-  reported to the console. The program returns the error count - this will
-  be 0 if no validation errors are encountered.
-
-  Example of validating a single Mapfile:
-
-      mappyfile validate C:/Temp/valid.map
-
-  Example of validating two folders containing Mapfiles, without expanding
-  INCLUDES:
-
-      mappyfile validate C:/Temp/*.map
-      D:/GitHub/mappyfile/tests/mapfiles/*.map --no-expand
-
-Options:
-  --expand / --no-expand  Expand any INCLUDE directives found in the Mapfile
-                          [default: True]
-  --help                  Show this message and exit.
+Usage: mappyfile validate [OPTIONS] [MAPFILES]...
+
+  Validate Mapfile(s) against the Mapfile schema
+
+  The MAPFILES argument is a list of paths, either to individual Mapfiles,
+  or a folders containing Mapfiles.  Wildcards are supported (natively on
+  Linux, and up to one level deep on Windows). Validation errors are
+  reported to the console. The program returns the error count - this will
+  be 0 if no validation errors are encountered.
+
+  Example of validating a single Mapfile:
+
+      mappyfile validate C:/Temp/valid.map
+
+  Example of validating two folders containing Mapfiles, without expanding
+  INCLUDES:
+
+      mappyfile validate C:/Temp/*.map
+      D:/GitHub/mappyfile/tests/mapfiles/*.map --no-expand
+
+Options:
+  --expand / --no-expand  Expand any INCLUDE directives found in the Mapfile
+                          [default: True]
+  --help                  Show this message and exit.
```

### Comparing `mappyfile-1.0.1/docs/validation.rst` & `mappyfile-1.0.2/docs/validation.rst`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-.. _validation-docs:
-
-Validation
-==========
-
-A key part of the mappyfile library is to validate Mapfiles - checking that options for various keywords are valid. In order to achieve this
-a full definition of the Mapfile language has been encoded in a JSON file - see :ref:`mapfile-schema`.
-
-`jsonschema <https://pypi.python.org/pypi/jsonschema>`_ is used to validate a Mapfile by converting the transformed dictionary to JSON. 
-For details on creating JSON schemas see the excellent documentation `here <https://spacetelescope.github.io/understanding-json-schema/>`_. 
-
-`python-fastjsonschema <https://github.com/horejsek/python-fastjsonschema>`_ was also considered, but this does now allow multiple validation
-errors to be output - only the first error encountered - see `this link <https://github.com/horejsek/python-fastjsonschema/issues/36>`_. 
-
-What is Validated?
-------------------
-
-Each of the Mapfile keywords has a limited set of allowed values. For example a `UNIT`` setting for a ``LAYER`` must be one of the strings 
-in the list below:
-
-.. code-block:: json
-
-    {
-    "units": {
-        "enum": [
-            "dd", 
-            "feet", 
-            "inches", 
-            "kilometers", 
-            "meters", 
-            "miles", 
-            "nauticalmiles", 
-            "percentages", 
-            "pixels"
-        ]
-    }
-    }
-
-If the Mapfile contains a value not in this list then an error will be raised. 
-
-For settings such as ``COLOR`` either RGB values or hex codes are allowed. This is accounted for in the schema using the ``oneOf``
-property:
-
-.. code-block:: json
-
-    {
-    "color": {
-        "oneOf": [
-            {
-                "minItems": 3, 
-                "items": {
-                    "minimum": -1, 
-                    "type": "number", 
-                    "maximum": 255
-                }, 
-                "type": "array", 
-                "maxItems": 3
-            }, 
-            {
-                "pattern": "^#([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$", 
-                "type": "string", 
-                "example": "#aa33cc"
-            }
-        ]
-    }
-    }
-
-How to Validate
----------------
-
-Mapfile validation can either be run using the :ref:`cli`, or directly in Python code:
-
-.. code-block:: python
-
-    s = """MAP
-        NAME "sample"
-        LAYER
-            NAME "test"
-            STATUS DEFAULT
-            DATA "SELECT GEOM
-            FROM
-            TABLE"
-            TYPE LINEX
-        END
-    END"""
-
-    d = mappyfile.loads(s, include_position=True)
-    v = Validator()
-    errors = v.validate(d, add_comments=True, version=7.6)
-    for e in errors:
-        print(e)
-
-Outputs the following:
-
-.. code-block:: python
-
-    {'column': 9, 'message': 'ERROR: Invalid value in TYPE', 'line': 9, 'error': "u'linex' is not one of [u'chart', u'circle', u'line', u'point', u'polygon', u'raster', u'query', u'annotation']"}
-
-The ``include_position`` parameter can be set to ``True`` when loading a Mapfile (or Mapfile snippet), so that any validation errors
-include line positions. 
-
-The optional ``version`` parameter can be used to validate the Mapfile against a specific 
-version of MapServer. 
-
-..
-    If a ``$ref`` is used then all other properties are ignored. 
-
-        You will always use $ref as the only key in an object: any other keys you put 
-        there will be ignored by the validator.
-
-    See https://json-schema.org/understanding-json-schema/structuring.html#reuse
-
-    .. code-block:: json
-
-        "color": {
-          "allOf": [
-            {
-              "$ref": "color.json"
-            }
-          ],
-          "metadata": {
-            "deprecated": true,
-            "maxVersion": 7.6
-          }
-        },
-
-
-..
-    Some keywords when missing will raise errors when trying to generate a map, for example if a ``MAP`` has no ``SIZE``:
-
-    .. code-block:: bat
-
-        msDrawMap(): Image handling error. Unable to initialize image. <br>
-        msPrepareImage(): General error message. Image dimensions not specified. <br>
-
-    However this parameter can be set from the command line, so the ``MAP`` may not actually be invalid. This is similar for ``EXTENT``:
-
-    .. code-block:: bat
-
-        shp2img -m test.map -i png -o test.png -s 200 200
-        msDrawMap(): Image handling error. Unable to initialize image. <br>
-        msCalculateScale(): General error message. Invalid image extent, minx=-1.000000, miny=-1.000000, maxx=-1.000000, maxy=-1.000000
-
-    Would need to use:
-
-    .. code-block:: bat
-
-        shp2img -m test.map -i png -o test.png -s 200 200 -e 0 0 5 5
-
-    Whilst keywords are not case-sensitive, some attributes are, for example ``STATUS "on"`` is not valid:
-
-    .. code-block:: bat
-
-        getSymbol(): Symbol definition error. Parsing error near (on):(line 3) <br>
-
-    For non-case-sensitive attributes may need to enforce lower case on all keywords prior to validation to avoid having to make ``enum`` lists of "ON","on","On" etc. 
-
-    ``CONFIG`` keywords (see http://mapserver.org/mapfile/map.html) have many MapServer and GDAL options, so won't validate these. 
-
-    Alert deprecated keywords? This appears to be a suggested feature of JSON Schema, see https://github.com/json-schema-org/json-schema-spec/pull/173. 
-
-..
-    Examples of snippets and validating against sub-schemas
-
-    additionalProperties true to allow for metadata such as __position__
-
-    Any named symmbols which do not exist cause mappyscript to crash
-    SIZE when using POLYGON and no SYMBOL - crash
-
-..
-    Check that layer, map, and group names are unique or get wrong legends etc.
-
-    Only layers of TYPE POINT are supported for a layer with CLUSTER set
+.. _validation-docs:
+
+Validation
+==========
+
+A key part of the mappyfile library is to validate Mapfiles - checking that options for various keywords are valid. In order to achieve this
+a full definition of the Mapfile language has been encoded in a JSON file - see :ref:`mapfile-schema`.
+
+`jsonschema <https://pypi.python.org/pypi/jsonschema>`_ is used to validate a Mapfile by converting the transformed dictionary to JSON. 
+For details on creating JSON schemas see the excellent documentation `here <https://spacetelescope.github.io/understanding-json-schema/>`_. 
+
+`python-fastjsonschema <https://github.com/horejsek/python-fastjsonschema>`_ was also considered, but this does now allow multiple validation
+errors to be output - only the first error encountered - see `this link <https://github.com/horejsek/python-fastjsonschema/issues/36>`_. 
+
+What is Validated?
+------------------
+
+Each of the Mapfile keywords has a limited set of allowed values. For example a `UNIT`` setting for a ``LAYER`` must be one of the strings 
+in the list below:
+
+.. code-block:: json
+
+    {
+    "units": {
+        "enum": [
+            "dd", 
+            "feet", 
+            "inches", 
+            "kilometers", 
+            "meters", 
+            "miles", 
+            "nauticalmiles", 
+            "percentages", 
+            "pixels"
+        ]
+    }
+    }
+
+If the Mapfile contains a value not in this list then an error will be raised. 
+
+For settings such as ``COLOR`` either RGB values or hex codes are allowed. This is accounted for in the schema using the ``oneOf``
+property:
+
+.. code-block:: json
+
+    {
+    "color": {
+        "oneOf": [
+            {
+                "minItems": 3, 
+                "items": {
+                    "minimum": -1, 
+                    "type": "number", 
+                    "maximum": 255
+                }, 
+                "type": "array", 
+                "maxItems": 3
+            }, 
+            {
+                "pattern": "^#([a-fA-F0-9]{6}|[a-fA-F0-9]{3})$", 
+                "type": "string", 
+                "example": "#aa33cc"
+            }
+        ]
+    }
+    }
+
+How to Validate
+---------------
+
+Mapfile validation can either be run using the :ref:`cli`, or directly in Python code:
+
+.. code-block:: python
+
+    s = """MAP
+        NAME "sample"
+        LAYER
+            NAME "test"
+            STATUS DEFAULT
+            DATA "SELECT GEOM
+            FROM
+            TABLE"
+            TYPE LINEX
+        END
+    END"""
+
+    d = mappyfile.loads(s, include_position=True)
+    v = Validator()
+    errors = v.validate(d, add_comments=True, version=7.6)
+    for e in errors:
+        print(e)
+
+Outputs the following:
+
+.. code-block:: python
+
+    {'column': 9, 'message': 'ERROR: Invalid value in TYPE', 'line': 9, 'error': "u'linex' is not one of [u'chart', u'circle', u'line', u'point', u'polygon', u'raster', u'query', u'annotation']"}
+
+The ``include_position`` parameter can be set to ``True`` when loading a Mapfile (or Mapfile snippet), so that any validation errors
+include line positions. 
+
+The optional ``version`` parameter can be used to validate the Mapfile against a specific 
+version of MapServer. 
+
+..
+    If a ``$ref`` is used then all other properties are ignored. 
+
+        You will always use $ref as the only key in an object: any other keys you put 
+        there will be ignored by the validator.
+
+    See https://json-schema.org/understanding-json-schema/structuring.html#reuse
+
+    .. code-block:: json
+
+        "color": {
+          "allOf": [
+            {
+              "$ref": "color.json"
+            }
+          ],
+          "metadata": {
+            "deprecated": true,
+            "maxVersion": 7.6
+          }
+        },
+
+
+..
+    Some keywords when missing will raise errors when trying to generate a map, for example if a ``MAP`` has no ``SIZE``:
+
+    .. code-block:: bat
+
+        msDrawMap(): Image handling error. Unable to initialize image. <br>
+        msPrepareImage(): General error message. Image dimensions not specified. <br>
+
+    However this parameter can be set from the command line, so the ``MAP`` may not actually be invalid. This is similar for ``EXTENT``:
+
+    .. code-block:: bat
+
+        shp2img -m test.map -i png -o test.png -s 200 200
+        msDrawMap(): Image handling error. Unable to initialize image. <br>
+        msCalculateScale(): General error message. Invalid image extent, minx=-1.000000, miny=-1.000000, maxx=-1.000000, maxy=-1.000000
+
+    Would need to use:
+
+    .. code-block:: bat
+
+        shp2img -m test.map -i png -o test.png -s 200 200 -e 0 0 5 5
+
+    Whilst keywords are not case-sensitive, some attributes are, for example ``STATUS "on"`` is not valid:
+
+    .. code-block:: bat
+
+        getSymbol(): Symbol definition error. Parsing error near (on):(line 3) <br>
+
+    For non-case-sensitive attributes may need to enforce lower case on all keywords prior to validation to avoid having to make ``enum`` lists of "ON","on","On" etc. 
+
+    ``CONFIG`` keywords (see http://mapserver.org/mapfile/map.html) have many MapServer and GDAL options, so won't validate these. 
+
+    Alert deprecated keywords? This appears to be a suggested feature of JSON Schema, see https://github.com/json-schema-org/json-schema-spec/pull/173. 
+
+..
+    Examples of snippets and validating against sub-schemas
+
+    additionalProperties true to allow for metadata such as __position__
+
+    Any named symmbols which do not exist cause mappyscript to crash
+    SIZE when using POLYGON and no SYMBOL - crash
+
+..
+    Check that layer, map, and group names are unique or get wrong legends etc.
+
+    Only layers of TYPE POINT are supported for a layer with CLUSTER set
     "enum": [ "ellipse", "rectangle" ] - if add these they are converted to strings without quotes
```

### Comparing `mappyfile-1.0.1/mappyfile/__init__.py` & `mappyfile-1.0.2/mappyfile/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# =================================================================
-#
-# Authors: Seth Girvin
-#
-# Copyright (c) 2020 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-import logging
-import importlib.metadata
-from logging import NullHandler
-import sys
-from types import ModuleType
-
-# allow high-level functions to be accessed directly from the mappyfile module
-# pylint: disable=redefined-builtin
-from mappyfile.utils import (
-    open,
-    create,
-    load,
-    loads,
-    dumps,
-    dump,
-    save,
-    validate,
-)
-from mappyfile.dictutils import (
-    find,
-    findall,
-    findkey,
-    findunique,
-    update,
-    dict_move_to_end,
-)
-
-__version__ = "1.0.1"
-
-__all__ = [
-    "open",
-    "load",
-    "loads",
-    "find",
-    "findall",
-    "findunique",
-    "dumps",
-    "dump",
-    "save",
-    "findkey",
-    "update",
-    "validate",
-    "create",
-    "dict_move_to_end",
-]
-
-
-module = ModuleType("mappyfile.plugins")
-sys.modules["mappyfile.plugins"] = module
-
-if sys.version_info >= (3, 10):
-    plugins = importlib.metadata.entry_points(group="mappyfile.plugins")
-else:
-    plugins = importlib.metadata.entry_points().get("mappyfile.plugins", [])
-
-for plugin in plugins:
-    setattr(module, plugin.name, plugin.load())
-
-# Set default logging handler to avoid "No handler found" warnings.
-logging.getLogger("mappyfile").addHandler(NullHandler())
+# =================================================================
+#
+# Authors: Seth Girvin
+#
+# Copyright (c) 2020 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+import logging
+import importlib.metadata
+from logging import NullHandler
+import sys
+from types import ModuleType
+
+# allow high-level functions to be accessed directly from the mappyfile module
+# pylint: disable=redefined-builtin
+from mappyfile.utils import (
+    open,
+    create,
+    load,
+    loads,
+    dumps,
+    dump,
+    save,
+    validate,
+)
+from mappyfile.dictutils import (
+    find,
+    findall,
+    findkey,
+    findunique,
+    update,
+    dict_move_to_end,
+)
+
+__version__ = "1.0.2"
+
+__all__ = [
+    "open",
+    "load",
+    "loads",
+    "find",
+    "findall",
+    "findunique",
+    "dumps",
+    "dump",
+    "save",
+    "findkey",
+    "update",
+    "validate",
+    "create",
+    "dict_move_to_end",
+]
+
+
+module = ModuleType("mappyfile.plugins")
+sys.modules["mappyfile.plugins"] = module
+
+if sys.version_info >= (3, 10):
+    plugins = importlib.metadata.entry_points(group="mappyfile.plugins")
+else:
+    plugins = importlib.metadata.entry_points().get("mappyfile.plugins", [])
+
+for plugin in plugins:
+    setattr(module, plugin.name, plugin.load())
+
+# Set default logging handler to avoid "No handler found" warnings.
+logging.getLogger("mappyfile").addHandler(NullHandler())
```

### Comparing `mappyfile-1.0.1/mappyfile/dictutils.py` & `mappyfile-1.0.2/mappyfile/dictutils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,320 +1,320 @@
-# =================================================================
-#
-# Authors: Seth Girvin
-#
-# Copyright (c) 2023 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-from __future__ import annotations
-from typing import Any
-from itertools import zip_longest
-
-
-def find(lst: list[dict], key: str, value: Any) -> dict | None:
-    """
-    Find an item in a list of dicts using a key and a value
-
-    Parameters
-    ----------
-
-    list: list
-        A list of composite dictionaries e.g. ``layers``, ``classes``
-    key: string
-        The key name to search each dictionary in the list
-    key: value
-        The value to search for
-
-    Returns
-    -------
-
-    dict
-        The first composite dictionary object with a key that matches the value
-
-    Example
-    -------
-
-    To find the ``LAYER`` in a list of layers with ``NAME`` set to ``Layer2``::
-
-        s = '''
-        MAP
-            LAYER
-                NAME "Layer1"
-                TYPE POLYGON
-            END
-            LAYER
-                NAME "Layer2"
-                TYPE POLYGON
-                CLASS
-                    NAME "Class1"
-                    COLOR 0 0 -8
-                END
-            END
-        END
-        '''
-
-        d = mappyfile.loads(s)
-        cmp = mappyfile.find(d["layers"], "name", "Layer2")
-        assert cmp["name"] == "Layer2"
-    """
-    return next((item for item in lst if item[key.lower()] == value), None)
-
-
-def findall(lst: list[dict], key: str, value: Any) -> list[dict]:
-    """
-    Find all items in lst where key matches value.
-    For example find all ``LAYER`` s in a ``MAP`` where ``GROUP`` equals ``VALUE``
-
-    Parameters
-    ----------
-
-    list: list
-        A list of composite dictionaries e.g. ``layers``, ``classes``
-    key: string
-        The key name to search each dictionary in the list
-    key: value
-        The value to search for
-
-    Returns
-    -------
-
-    list
-        A Python list containing the matching composite dictionaries
-
-    Example
-    -------
-
-    To find all ``LAYER`` s with ``GROUP`` set to ``test``::
-
-        s = '''
-        MAP
-            LAYER
-                NAME "Layer1"
-                TYPE POLYGON
-                GROUP "test"
-            END
-            LAYER
-                NAME "Layer2"
-                TYPE POLYGON
-                GROUP "test1"
-            END
-            LAYER
-                NAME "Layer3"
-                TYPE POLYGON
-                GROUP "test2"
-            END
-            LAYER
-                NAME "Layer4"
-                TYPE POLYGON
-                GROUP "test"
-            END
-        END
-        '''
-
-        d = mappyfile.loads(s)
-        layers = mappyfile.findall(d["layers"], "group", "test")
-        assert len(layers) == 2
-    """
-    return [item for item in lst if item[key.lower()] and item[key.lower()] in value]
-
-
-def findunique(lst, key):
-    """
-    Find all unique key values for items in lst. If no
-    items with the key are found an empty list is returned.
-
-    Parameters
-    ----------
-
-    lst: list
-         A list of composite dictionaries e.g. ``layers``, ``classes``
-    key: string
-        The key name to search each dictionary in the list
-
-    Returns
-    -------
-
-    list
-        A sorted Python list of unique keys in the list
-
-    Example
-    -------
-
-    To find all ``GROUP`` values for ``CLASS`` in a ``LAYER``::
-
-        s = '''
-        LAYER
-            CLASS
-                GROUP "group1"
-                NAME "Class1"
-                COLOR 0 0 0
-            END
-            CLASS
-                GROUP "group2"
-                NAME "Class2"
-                COLOR 0 0 0
-            END
-            CLASS
-                GROUP "group1"
-                NAME "Class3"
-                COLOR 0 0 0
-            END
-        END
-        '''
-
-        d = mappyfile.loads(s)
-        groups = mappyfile.findunique(d["classes"], "group")
-        assert groups == ["group1", "group2"]
-    """
-    return sorted(
-        set((item.get(key.lower(), None) for item in lst))
-        - {
-            None,
-        }
-    )
-
-
-def findkey(d: dict, *keys: list[Any]) -> dict:
-    """
-    Get a value from a dictionary based on a list of keys and/or list indexes.
-
-    Parameters
-    ----------
-
-    d: dict
-        A Python dictionary
-    keys: list
-        A list of key names, or list indexes
-
-    Returns
-    -------
-
-    dict
-        The composite dictionary object at the path specified by the keys
-
-    Example
-    -------
-
-    To return the value of the first class of the first layer in a Mapfile::
-
-        s = '''
-        MAP
-            LAYER
-                NAME "Layer1"
-                TYPE POLYGON
-                CLASS
-                    NAME "Class1"
-                    COLOR 0 0 255
-                END
-            END
-        END
-        '''
-
-        d = mappyfile.loads(s)
-
-        pth = ["layers", 0, "classes", 0]
-        cls1 = mappyfile.findkey(d, *pth)
-        assert cls1["name"] == "Class1"
-    """
-    if keys:
-        keys_list = list(keys)
-        search_key = keys_list.pop(0)
-        return findkey(d[search_key], *keys_list)
-
-    return d
-
-
-def update(d1: dict, d2: dict, overwrite: bool = True) -> dict:
-    """
-    Update dict d1 with properties from d2
-
-    Note
-    ----
-
-    Allows deletion of objects with a special ``__delete__`` key
-    For any list of dicts new items can be added when updating
-
-    Parameters
-    ----------
-
-    d1: dict
-        A Python dictionary
-    d2: dict
-        A Python dictionary that will be used to update any keys with the same name in d1
-    overwrite: boolean
-        If a key already exists in the dictionary should its value be overwritten
-
-    Returns
-    -------
-
-    dict
-        The updated dictionary
-
-    """
-    none_type = type(None)
-
-    if d2.get("__delete__", False):
-        return {}
-
-    for k, v in d2.items():
-        if isinstance(v, dict):
-            if v.get("__delete__", False):
-                # allow a __delete__ property to be set to delete objects
-                del d1[k]
-            else:
-                d1[k] = update(d1.get(k, {}), v, overwrite)
-        elif isinstance(v, (tuple, list)) and all(
-            isinstance(li, (none_type, dict)) for li in v  # type: ignore
-        ):
-            # a list of dicts and/or none_type
-            orig_list = d1.get(k, [])
-            new_list = []
-            pairs = list(zip_longest(orig_list, v, fillvalue=None))
-            for orig_item, new_item in pairs:
-                if orig_item is None:
-                    orig_item = (
-                        {}
-                    )  # can't use {} for fillvalue as only one dict created/modified!
-                if new_item is None:
-                    new_item = {}
-
-                if new_item.get("__delete__", False):
-                    d = None  # orig_list.remove(orig_item) # remove the item to delete
-                else:
-                    d = update(orig_item, new_item, overwrite)
-
-                if d is not None:
-                    new_list.append(d)
-            d1[k] = new_list
-        else:
-            if k in d1 and v == "__delete__":
-                del d1[k]
-            else:
-                if overwrite is True or k not in d1:
-                    d1[k] = v
-    return d1
-
-
-def dict_move_to_end(ordered_dict, key):
-    ordered_dict.move_to_end(key)
+# =================================================================
+#
+# Authors: Seth Girvin
+#
+# Copyright (c) 2023 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+from __future__ import annotations
+from typing import Any
+from itertools import zip_longest
+
+
+def find(lst: list[dict], key: str, value: Any) -> dict | None:
+    """
+    Find an item in a list of dicts using a key and a value
+
+    Parameters
+    ----------
+
+    list: list
+        A list of composite dictionaries e.g. ``layers``, ``classes``
+    key: string
+        The key name to search each dictionary in the list
+    key: value
+        The value to search for
+
+    Returns
+    -------
+
+    dict
+        The first composite dictionary object with a key that matches the value
+
+    Example
+    -------
+
+    To find the ``LAYER`` in a list of layers with ``NAME`` set to ``Layer2``::
+
+        s = '''
+        MAP
+            LAYER
+                NAME "Layer1"
+                TYPE POLYGON
+            END
+            LAYER
+                NAME "Layer2"
+                TYPE POLYGON
+                CLASS
+                    NAME "Class1"
+                    COLOR 0 0 -8
+                END
+            END
+        END
+        '''
+
+        d = mappyfile.loads(s)
+        cmp = mappyfile.find(d["layers"], "name", "Layer2")
+        assert cmp["name"] == "Layer2"
+    """
+    return next((item for item in lst if item[key.lower()] == value), None)
+
+
+def findall(lst: list[dict], key: str, value: Any) -> list[dict]:
+    """
+    Find all items in lst where key matches value.
+    For example find all ``LAYER`` s in a ``MAP`` where ``GROUP`` equals ``VALUE``
+
+    Parameters
+    ----------
+
+    list: list
+        A list of composite dictionaries e.g. ``layers``, ``classes``
+    key: string
+        The key name to search each dictionary in the list
+    key: value
+        The value to search for
+
+    Returns
+    -------
+
+    list
+        A Python list containing the matching composite dictionaries
+
+    Example
+    -------
+
+    To find all ``LAYER`` s with ``GROUP`` set to ``test``::
+
+        s = '''
+        MAP
+            LAYER
+                NAME "Layer1"
+                TYPE POLYGON
+                GROUP "test"
+            END
+            LAYER
+                NAME "Layer2"
+                TYPE POLYGON
+                GROUP "test1"
+            END
+            LAYER
+                NAME "Layer3"
+                TYPE POLYGON
+                GROUP "test2"
+            END
+            LAYER
+                NAME "Layer4"
+                TYPE POLYGON
+                GROUP "test"
+            END
+        END
+        '''
+
+        d = mappyfile.loads(s)
+        layers = mappyfile.findall(d["layers"], "group", "test")
+        assert len(layers) == 2
+    """
+    return [item for item in lst if item[key.lower()] and item[key.lower()] in value]
+
+
+def findunique(lst, key):
+    """
+    Find all unique key values for items in lst. If no
+    items with the key are found an empty list is returned.
+
+    Parameters
+    ----------
+
+    lst: list
+         A list of composite dictionaries e.g. ``layers``, ``classes``
+    key: string
+        The key name to search each dictionary in the list
+
+    Returns
+    -------
+
+    list
+        A sorted Python list of unique keys in the list
+
+    Example
+    -------
+
+    To find all ``GROUP`` values for ``CLASS`` in a ``LAYER``::
+
+        s = '''
+        LAYER
+            CLASS
+                GROUP "group1"
+                NAME "Class1"
+                COLOR 0 0 0
+            END
+            CLASS
+                GROUP "group2"
+                NAME "Class2"
+                COLOR 0 0 0
+            END
+            CLASS
+                GROUP "group1"
+                NAME "Class3"
+                COLOR 0 0 0
+            END
+        END
+        '''
+
+        d = mappyfile.loads(s)
+        groups = mappyfile.findunique(d["classes"], "group")
+        assert groups == ["group1", "group2"]
+    """
+    return sorted(
+        set((item.get(key.lower(), None) for item in lst))
+        - {
+            None,
+        }
+    )
+
+
+def findkey(d: dict, *keys: list[Any]) -> dict:
+    """
+    Get a value from a dictionary based on a list of keys and/or list indexes.
+
+    Parameters
+    ----------
+
+    d: dict
+        A Python dictionary
+    keys: list
+        A list of key names, or list indexes
+
+    Returns
+    -------
+
+    dict
+        The composite dictionary object at the path specified by the keys
+
+    Example
+    -------
+
+    To return the value of the first class of the first layer in a Mapfile::
+
+        s = '''
+        MAP
+            LAYER
+                NAME "Layer1"
+                TYPE POLYGON
+                CLASS
+                    NAME "Class1"
+                    COLOR 0 0 255
+                END
+            END
+        END
+        '''
+
+        d = mappyfile.loads(s)
+
+        pth = ["layers", 0, "classes", 0]
+        cls1 = mappyfile.findkey(d, *pth)
+        assert cls1["name"] == "Class1"
+    """
+    if keys:
+        keys_list = list(keys)
+        search_key = keys_list.pop(0)
+        return findkey(d[search_key], *keys_list)
+
+    return d
+
+
+def update(d1: dict, d2: dict, overwrite: bool = True) -> dict:
+    """
+    Update dict d1 with properties from d2
+
+    Note
+    ----
+
+    Allows deletion of objects with a special ``__delete__`` key
+    For any list of dicts new items can be added when updating
+
+    Parameters
+    ----------
+
+    d1: dict
+        A Python dictionary
+    d2: dict
+        A Python dictionary that will be used to update any keys with the same name in d1
+    overwrite: boolean
+        If a key already exists in the dictionary should its value be overwritten
+
+    Returns
+    -------
+
+    dict
+        The updated dictionary
+
+    """
+    none_type = type(None)
+
+    if d2.get("__delete__", False):
+        return {}
+
+    for k, v in d2.items():
+        if isinstance(v, dict):
+            if v.get("__delete__", False):
+                # allow a __delete__ property to be set to delete objects
+                del d1[k]
+            else:
+                d1[k] = update(d1.get(k, {}), v, overwrite)
+        elif isinstance(v, (tuple, list)) and all(
+            isinstance(li, (none_type, dict)) for li in v  # type: ignore
+        ):
+            # a list of dicts and/or none_type
+            orig_list = d1.get(k, [])
+            new_list = []
+            pairs = list(zip_longest(orig_list, v, fillvalue=None))
+            for orig_item, new_item in pairs:
+                if orig_item is None:
+                    orig_item = (
+                        {}
+                    )  # can't use {} for fillvalue as only one dict created/modified!
+                if new_item is None:
+                    new_item = {}
+
+                if new_item.get("__delete__", False):
+                    d = None  # orig_list.remove(orig_item) # remove the item to delete
+                else:
+                    d = update(orig_item, new_item, overwrite)
+
+                if d is not None:
+                    new_list.append(d)
+            d1[k] = new_list
+        else:
+            if k in d1 and v == "__delete__":
+                del d1[k]
+            else:
+                if overwrite is True or k not in d1:
+                    d1[k] = v
+    return d1
+
+
+def dict_move_to_end(ordered_dict, key):
+    ordered_dict.move_to_end(key)
```

### Comparing `mappyfile-1.0.1/mappyfile/mapfile.lark` & `mappyfile-1.0.2/mappyfile/mapfile.lark`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-// =================================================================
-// 
-// Authors: Erez Shinan, Seth Girvin
-// 
-// Copyright (c) 2020 Seth Girvin
-// 
-// Permission is hereby granted, free of charge, to any person
-// obtaining a copy of this software and associated documentation
-// files (the "Software"), to deal in the Software without
-// restriction, including without limitation the rights to use,
-// copy, modify, merge, publish, distribute, sublicense, and/or sell
-// copies of the Software, and to permit persons to whom the
-// Software is furnished to do so, subject to the following
-// conditions:
-// 
-// The above copyright notice and this permission notice shall be
-// included in all copies or substantial portions of the Software.
-// 
-// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-// EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-// OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-// NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-// HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-// WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-// FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-// OTHER DEALINGS IN THE SOFTWARE.
-// 
-// =================================================================
-
-start: "SYMBOLSET"i composite_body _END   -> symbolset
-     | composite+
-
-composite: composite_type composite_body _END
-       | metadata
-       | validation
-       | connectionoptions
-
-composite_body: _composite_item*
-_composite_item: (composite|attr|points|projection|pattern|values|config)
-
-!projection: "PROJECTION"i (string*|AUTO) _END
-!config: "CONFIG"i (string | UNQUOTED_STRING) (string | UNQUOTED_STRING)
-
-!points: "POINTS"i num_pair* _END
-!pattern: "PATTERN"i num_pair* _END
-
-!values: "VALUES"i string_pair* _END
-!metadata: "METADATA"i string_pair* _END
-!validation: "VALIDATION"i string_pair* _END
-!connectionoptions: "CONNECTIONOPTIONS"i string_pair* _END
-
-attr: (UNQUOTED_STRING | composite_type) (value | UNQUOTED_STRING | UNQUOTED_STRING_VALUE)
-%declare UNQUOTED_STRING_VALUE  // generated using the interactive parser. See issues #48, #98
-
-?value: string | int | float | expression | not_expression | attr_bind | path
-| regexp | runtime_var | list | NULL | true | false | extent | rgb | hexcolor
-| colorrange | hexcolorrange | num_pair | attr_bind_pair | attr_mixed_pair | _attr_keyword
-
-int: SIGNED_INT
-int_pair: int int
-rgb: int int int
-colorrange: int int int int int int
-hexcolorrange: hexcolor hexcolor
-hexcolor: DOUBLE_QUOTED_HEXCOLOR | SINGLE_QUOTED_HEXCOLOR
-
-extent: (int|float) (int|float) (int|float) (int|float) 
-
-!_attr_keyword: "AUTO"i | "HILITE"i | "SELECTED"i 
-
-string: DOUBLE_QUOTED_STRING | SINGLE_QUOTED_STRING | ESCAPED_STRING
-string_pair: (string|UNQUOTED_STRING) (string|UNQUOTED_STRING)
-
-attr_bind_pair: attr_bind attr_bind
-attr_mixed_pair: attr_bind (int|float) | (int|float) attr_bind
-float: SIGNED_FLOAT
-float_pair: float float
-path: PATH
-regexp: REGEXP1 | REGEXP2
-runtime_var: RUNTIME_VAR
-list: "{" (value | UNQUOTED_STRING_SPACE) ("," (value | UNQUOTED_STRING_SPACE))* "}"
-
-num_pair: (int|float) (int|float)
-
-attr_bind: "[" UNQUOTED_STRING "]"
-
-not_expression: ("!"|"NOT"i) comparison
-expression: "(" or_test ")"
-?or_test : (or_test ("OR"i|"||"))? and_test
-?and_test : (and_test ("AND"i|"&&"))? comparison
-?comparison: (comparison compare_op)? sum
-!compare_op: ">=" | "<" | "=*" | "==" | "=" | "!=" | "~" | "~*" | ">" | "%"
-| "<=" | "IN"i | "NE"i | "EQ"i | "LE"i | "LT"i | "GE"i | "GT"i | "LIKE"i
-
-?sum: product
-    | sum "+" product -> add
-    | sum "-" product -> sub
-
-?product: unary_expr
-    | product "*" unary_expr -> mul
-    | product "/" unary_expr -> div
-    | product "^" unary_expr -> power
-
-?unary_expr: atom
-    | "-" unary_expr -> neg
-    | "+" unary_expr
-
-?atom: (func_call | value)
-// ?multiply: (multiply "*")? (func_call | value)
-
-func_call: UNQUOTED_STRING "(" func_params ")"
-func_params: value ("," value)*
-
-!true: "TRUE"i
-!false: "FALSE"i
-
-!composite_type: "CLASS"i
-            | "CLUSTER"i
-            | "COMPOSITE"i
-            | "FEATURE"i
-            | "GRID"i
-            | "JOIN"i
-            | "LABEL"i
-            | "LAYER"i
-            | "LEADER"i
-            | "LEGEND"i
-            | "MAP"i
-            | "OUTPUTFORMAT"i
-            | "QUERYMAP"i
-            | "REFERENCE"i
-            | "SCALEBAR"i
-            | "SCALETOKEN"i
-            | "STYLE"i
-            | "WEB"i
-            | "SYMBOL"i
-
-AUTO: "AUTO"i
-PATH: /([a-z0-9_]*\.*\/|[a-z0-9_]+[.\/])[a-z0-9_\/\.-]+/i
-
-// rules allow optional alphachannel
-DOUBLE_QUOTED_HEXCOLOR.2: /\"#(?:[0-9a-fA-F]{3}){1,2}([0-9a-fA-F]{2})?\"/
-SINGLE_QUOTED_HEXCOLOR.2: /'#(?:[0-9a-fA-F]{3}){1,2}([0-9a-fA-F]{2})?'/
-
-NULL: "NULL"i
-
-SIGNED_FLOAT: ["-"|"+"] FLOAT
-SIGNED_INT: ["-"|"+"] INT
-
-INT: /[0-9]+(?![_a-zA-Z])/
-
-%import common.FLOAT
-
-// UNQUOTED_STRING: /[a-z_][a-z0-9_\-]*/i
-UNQUOTED_STRING: /[a-z0-9_\xc0-\xff\-:]+/i
-UNQUOTED_STRING_SPACE: /[a-z0-9\xc0-\xff_\-: ']+/i
-DOUBLE_QUOTED_STRING: "\"" ("\\\""|/[^"]/)* "\"" "i"?
-SINGLE_QUOTED_STRING: "'" ("\\'"|/[^']/)* "'" "i"?
-ESCAPED_STRING: /`.*?`i?/
-//KEYWORD: /[a-z]+/i
-
-//UNQUOTED_NUMERIC_STRING: /[a-z_][a-z0-9_\-]*/i
-
-REGEXP1.2: /\/.*?\/i?/
-REGEXP2: /\\\\.*?\\\\i?/
-
-RUNTIME_VAR: /%.*?%/
-
-COMMENT: /\#[^\n]*/
-CCOMMENT.3: /\/[*].*?[*]\//s
-
-_END: "END"i
-
-WS: /[ \t\f]+/
-_NL: /[\r\n]+/
-
-%ignore COMMENT
-%ignore CCOMMENT
-%ignore WS
-%ignore _NL
+// =================================================================
+// 
+// Authors: Erez Shinan, Seth Girvin
+// 
+// Copyright (c) 2020 Seth Girvin
+// 
+// Permission is hereby granted, free of charge, to any person
+// obtaining a copy of this software and associated documentation
+// files (the "Software"), to deal in the Software without
+// restriction, including without limitation the rights to use,
+// copy, modify, merge, publish, distribute, sublicense, and/or sell
+// copies of the Software, and to permit persons to whom the
+// Software is furnished to do so, subject to the following
+// conditions:
+// 
+// The above copyright notice and this permission notice shall be
+// included in all copies or substantial portions of the Software.
+// 
+// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+// EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+// OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+// NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+// HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+// WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+// FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+// OTHER DEALINGS IN THE SOFTWARE.
+// 
+// =================================================================
+
+start: "SYMBOLSET"i composite_body _END   -> symbolset
+     | composite+
+
+composite: composite_type composite_body _END
+       | metadata
+       | validation
+       | connectionoptions
+
+composite_body: _composite_item*
+_composite_item: (composite|attr|points|projection|pattern|values|config)
+
+!projection: "PROJECTION"i (string*|AUTO) _END
+!config: "CONFIG"i (string | UNQUOTED_STRING) (string | UNQUOTED_STRING)
+
+!points: "POINTS"i num_pair* _END
+!pattern: "PATTERN"i num_pair* _END
+
+!values: "VALUES"i string_pair* _END
+!metadata: "METADATA"i string_pair* _END
+!validation: "VALIDATION"i string_pair* _END
+!connectionoptions: "CONNECTIONOPTIONS"i string_pair* _END
+
+attr: (UNQUOTED_STRING | composite_type) (value | UNQUOTED_STRING | UNQUOTED_STRING_VALUE)
+%declare UNQUOTED_STRING_VALUE  // generated using the interactive parser. See issues #48, #98
+
+?value: string | int | float | expression | not_expression | attr_bind | path
+| regexp | runtime_var | list | NULL | true | false | extent | rgb | hexcolor
+| colorrange | hexcolorrange | num_pair | attr_bind_pair | attr_mixed_pair | _attr_keyword
+
+int: SIGNED_INT
+int_pair: int int
+rgb: int int int
+colorrange: int int int int int int
+hexcolorrange: hexcolor hexcolor
+hexcolor: DOUBLE_QUOTED_HEXCOLOR | SINGLE_QUOTED_HEXCOLOR
+
+extent: (int|float) (int|float) (int|float) (int|float) 
+
+!_attr_keyword: "AUTO"i | "HILITE"i | "SELECTED"i 
+
+string: DOUBLE_QUOTED_STRING | SINGLE_QUOTED_STRING | ESCAPED_STRING
+string_pair: (string|UNQUOTED_STRING) (string|UNQUOTED_STRING)
+
+attr_bind_pair: attr_bind attr_bind
+attr_mixed_pair: attr_bind (int|float) | (int|float) attr_bind
+float: SIGNED_FLOAT
+float_pair: float float
+path: PATH
+regexp: REGEXP1 | REGEXP2
+runtime_var: RUNTIME_VAR
+list: "{" (value | UNQUOTED_STRING_SPACE) ("," (value | UNQUOTED_STRING_SPACE))* "}"
+
+num_pair: (int|float) (int|float)
+
+attr_bind: "[" UNQUOTED_STRING "]"
+
+not_expression: ("!"|"NOT"i) comparison
+expression: "(" or_test ")"
+?or_test : (or_test ("OR"i|"||"))? and_test
+?and_test : (and_test ("AND"i|"&&"))? comparison
+?comparison: (comparison compare_op)? sum
+!compare_op: ">=" | "<" | "=*" | "==" | "=" | "!=" | "~" | "~*" | ">" | "%"
+| "<=" | "IN"i | "NE"i | "EQ"i | "LE"i | "LT"i | "GE"i | "GT"i | "LIKE"i
+
+?sum: product
+    | sum "+" product -> add
+    | sum "-" product -> sub
+
+?product: unary_expr
+    | product "*" unary_expr -> mul
+    | product "/" unary_expr -> div
+    | product "^" unary_expr -> power
+
+?unary_expr: atom
+    | "-" unary_expr -> neg
+    | "+" unary_expr
+
+?atom: (func_call | value)
+// ?multiply: (multiply "*")? (func_call | value)
+
+func_call: UNQUOTED_STRING "(" func_params ")"
+func_params: value ("," value)*
+
+!true: "TRUE"i
+!false: "FALSE"i
+
+!composite_type: "CLASS"i
+            | "CLUSTER"i
+            | "COMPOSITE"i
+            | "FEATURE"i
+            | "GRID"i
+            | "JOIN"i
+            | "LABEL"i
+            | "LAYER"i
+            | "LEADER"i
+            | "LEGEND"i
+            | "MAP"i
+            | "OUTPUTFORMAT"i
+            | "QUERYMAP"i
+            | "REFERENCE"i
+            | "SCALEBAR"i
+            | "SCALETOKEN"i
+            | "STYLE"i
+            | "WEB"i
+            | "SYMBOL"i
+
+AUTO: "AUTO"i
+PATH: /([a-z0-9_]*\.*\/|[a-z0-9_]+[.\/])[a-z0-9_\/\.-]+/i
+
+// rules allow optional alphachannel
+DOUBLE_QUOTED_HEXCOLOR.2: /\"#(?:[0-9a-fA-F]{3}){1,2}([0-9a-fA-F]{2})?\"/
+SINGLE_QUOTED_HEXCOLOR.2: /'#(?:[0-9a-fA-F]{3}){1,2}([0-9a-fA-F]{2})?'/
+
+NULL: "NULL"i
+
+SIGNED_FLOAT: ["-"|"+"] FLOAT
+SIGNED_INT: ["-"|"+"] INT
+
+INT: /[0-9]+(?![_a-zA-Z])/
+
+%import common.FLOAT
+
+// UNQUOTED_STRING: /[a-z_][a-z0-9_\-]*/i
+UNQUOTED_STRING: /[a-z0-9_\xc0-\xff\-:]+/i
+UNQUOTED_STRING_SPACE: /[a-z0-9\xc0-\xff_\-: ']+/i
+DOUBLE_QUOTED_STRING: "\"" ("\\\""|/[^"]/)* "\"" "i"?
+SINGLE_QUOTED_STRING: "'" ("\\'"|/[^']/)* "'" "i"?
+ESCAPED_STRING: /`.*?`i?/
+//KEYWORD: /[a-z]+/i
+
+//UNQUOTED_NUMERIC_STRING: /[a-z_][a-z0-9_\-]*/i
+
+REGEXP1.2: /\/.*?\/i?/
+REGEXP2: /\\\\.*?\\\\i?/
+
+RUNTIME_VAR: /%.*?%/
+
+COMMENT: /\#[^\n]*/
+CCOMMENT.3: /\/[*].*?[*]\//s
+
+_END: "END"i
+
+WS: /[ \t\f]+/
+_NL: /[\r\n]+/
+
+%ignore COMMENT
+%ignore CCOMMENT
+%ignore WS
+%ignore _NL
```

### Comparing `mappyfile-1.0.1/mappyfile/ordereddict.py` & `mappyfile-1.0.2/mappyfile/ordereddict.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-# =================================================================
-#
-# Authors: Seth Girvin
-#          Jason Kirtland [1]
-#          Zach Kelling [2]
-#          m000 [3],[4]
-#
-# [1] http://code.activestate.com/recipes/523034-emulate-collectionsdefaultdict/
-# [2] http://stackoverflow.com/a/6190500/562769
-# [3] https://stackoverflow.com/users/277172/m000
-# [4] https://stackoverflow.com/a/32888599/179520
-#
-# Copyright (c) 2020 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-from collections import OrderedDict
-import copy
-from mappyfile.tokens import OBJECT_LIST_KEYS
-import json
-
-
-class DefaultOrderedDict(OrderedDict):
-    """
-    Used for storing components
-    Source: http://stackoverflow.com/a/6190500/562769
-    Based on: http://code.activestate.com/recipes/523034-emulate-collectionsdefaultdict/
-    """
-
-    # pylint: disable=keyword-arg-before-vararg
-    def __init__(self, default_factory=None, *args, **kwargs):
-        if default_factory is not None and not callable(default_factory):
-            raise TypeError("First argument must be callable")
-
-        OrderedDict.__init__(self, *args, **kwargs)
-        self.default_factory = default_factory
-
-    def __getitem__(self, key):
-        key = key.lower()  # all keys should be lower-case to make editing easier
-
-        try:
-            return OrderedDict.__getitem__(self, key)
-        except KeyError:
-            return self.__missing__(key)
-
-    def __missing__(self, key):
-        if self.default_factory is None:
-            raise KeyError(key)
-
-        if key in OBJECT_LIST_KEYS:
-            # create empty lists for keys of object lists such as "layers"
-            self[key] = value = []
-        else:
-            self[key] = value = self.default_factory()
-        return value
-
-    def __reduce__(self):
-        if self.default_factory is None:
-            args: tuple = tuple()
-        else:
-            args = (self.default_factory,)
-        return type(self), args, None, None, iter(self.items())
-
-    def copy(self):
-        return copy.copy(self)
-
-    def __copy__(self):
-        return type(self)(self.default_factory, self)
-
-    def __deepcopy__(self, memo):
-        return type(self)(self.default_factory, copy.deepcopy(list(self.items())))
-
-    def __repr__(self):
-        """
-        Return a human-readable version of the dict contents
-        """
-        return json.dumps(self, indent=4)  # sort_keys=True
-
-
-class CaseInsensitiveOrderedDict(DefaultOrderedDict):
-    """
-    Based on: https://stackoverflow.com/a/32888599/179520
-    """
-
-    @classmethod
-    def _k(cls, key):
-        return key.lower() if isinstance(key, str) else key
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._convert_keys()
-
-    def __getitem__(self, key):
-        return super().__getitem__(self.__class__._k(key))
-
-    def __setitem__(self, key, value):
-        super().__setitem__(self.__class__._k(key), value)
-
-    def __delitem__(self, key):
-        return super().__delitem__(self.__class__._k(key))
-
-    def __contains__(self, key):
-        return super().__contains__(self.__class__._k(key))
-
-    def has_key(self, key):
-        return key in self
-
-    def pop(self, key, *args, **kwargs):
-        # pylint: disable=protected-access
-        return super().pop(self.__class__._k(key), *args, **kwargs)
-
-    def get(self, key, *args, **kwargs):
-        # pylint: disable=protected-access
-        return super().get(self.__class__._k(key), *args, **kwargs)
-
-    def setdefault(self, key, *args, **kwargs):
-        # pylint: disable=protected-access
-        return super().setdefault(self.__class__._k(key), *args, **kwargs)
-
-    def update(self, e=None, **f):
-        if e is not None:
-            super().update(self.__class__(CaseInsensitiveOrderedDict, e))
-        super().update(self.__class__(CaseInsensitiveOrderedDict, **f))
-
-    def _convert_keys(self):
-        for k in list(self.keys()):
-            v = super().pop(k)
-            self[k] = v
+# =================================================================
+#
+# Authors: Seth Girvin
+#          Jason Kirtland [1]
+#          Zach Kelling [2]
+#          m000 [3],[4]
+#
+# [1] http://code.activestate.com/recipes/523034-emulate-collectionsdefaultdict/
+# [2] http://stackoverflow.com/a/6190500/562769
+# [3] https://stackoverflow.com/users/277172/m000
+# [4] https://stackoverflow.com/a/32888599/179520
+#
+# Copyright (c) 2020 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+from collections import OrderedDict
+import copy
+from mappyfile.tokens import OBJECT_LIST_KEYS
+import json
+
+
+class DefaultOrderedDict(OrderedDict):
+    """
+    Used for storing components
+    Source: http://stackoverflow.com/a/6190500/562769
+    Based on: http://code.activestate.com/recipes/523034-emulate-collectionsdefaultdict/
+    """
+
+    # pylint: disable=keyword-arg-before-vararg
+    def __init__(self, default_factory=None, *args, **kwargs):
+        if default_factory is not None and not callable(default_factory):
+            raise TypeError("First argument must be callable")
+
+        OrderedDict.__init__(self, *args, **kwargs)
+        self.default_factory = default_factory
+
+    def __getitem__(self, key):
+        key = key.lower()  # all keys should be lower-case to make editing easier
+
+        try:
+            return OrderedDict.__getitem__(self, key)
+        except KeyError:
+            return self.__missing__(key)
+
+    def __missing__(self, key):
+        if self.default_factory is None:
+            raise KeyError(key)
+
+        if key in OBJECT_LIST_KEYS:
+            # create empty lists for keys of object lists such as "layers"
+            self[key] = value = []
+        else:
+            self[key] = value = self.default_factory()
+        return value
+
+    def __reduce__(self):
+        if self.default_factory is None:
+            args: tuple = tuple()
+        else:
+            args = (self.default_factory,)
+        return type(self), args, None, None, iter(self.items())
+
+    def copy(self):
+        return copy.copy(self)
+
+    def __copy__(self):
+        return type(self)(self.default_factory, self)
+
+    def __deepcopy__(self, memo):
+        return type(self)(self.default_factory, copy.deepcopy(list(self.items())))
+
+    def __repr__(self):
+        """
+        Return a human-readable version of the dict contents
+        """
+        return json.dumps(self, indent=4)  # sort_keys=True
+
+
+class CaseInsensitiveOrderedDict(DefaultOrderedDict):
+    """
+    Based on: https://stackoverflow.com/a/32888599/179520
+    """
+
+    @classmethod
+    def _k(cls, key):
+        return key.lower() if isinstance(key, str) else key
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._convert_keys()
+
+    def __getitem__(self, key):
+        return super().__getitem__(self.__class__._k(key))
+
+    def __setitem__(self, key, value):
+        super().__setitem__(self.__class__._k(key), value)
+
+    def __delitem__(self, key):
+        return super().__delitem__(self.__class__._k(key))
+
+    def __contains__(self, key):
+        return super().__contains__(self.__class__._k(key))
+
+    def has_key(self, key):
+        return key in self
+
+    def pop(self, key, *args, **kwargs):
+        # pylint: disable=protected-access
+        return super().pop(self.__class__._k(key), *args, **kwargs)
+
+    def get(self, key, *args, **kwargs):
+        # pylint: disable=protected-access
+        return super().get(self.__class__._k(key), *args, **kwargs)
+
+    def setdefault(self, key, *args, **kwargs):
+        # pylint: disable=protected-access
+        return super().setdefault(self.__class__._k(key), *args, **kwargs)
+
+    def update(self, e=None, **f):
+        if e is not None:
+            super().update(self.__class__(CaseInsensitiveOrderedDict, e))
+        super().update(self.__class__(CaseInsensitiveOrderedDict, **f))
+
+    def _convert_keys(self):
+        for k in list(self.keys()):
+            v = super().pop(k)
+            self[k] = v
```

### Comparing `mappyfile-1.0.1/mappyfile/parser.py` & `mappyfile-1.0.2/mappyfile/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,242 +1,245 @@
-# =================================================================
-#
-# Authors: Seth Girvin, Erez Shinan
-#
-# Copyright (c) 2020 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-from __future__ import annotations
-import os
-import logging
-from io import open
-from lark import Lark, ParseError, Tree, UnexpectedInput
-from typing import Any, IO
-
-
-log = logging.getLogger("mappyfile")
-
-
-def string_to_boolean(string_value: str):
-    return string_value.lower() not in ("false", "no", "0", "off")
-
-
-use_cython = string_to_boolean(os.environ.get("MAPPYFILE_USE_CYTHON", "True"))
-lark_cython = None
-
-if use_cython:
-    try:
-        import lark_cython  # type: ignore
-    except ImportError:
-        pass
-
-
-SYMBOL_ATTRIBUTES = {
-    "ANCHORPOINT",
-    "ANTIALIAS",
-    "FILLED",
-    "FONT",
-    "IMAGE",
-    "NAME",
-    "COLOR",
-    "TYPE",
-    "CHARACTER",
-    "POINTS",
-    "TRANSPARENT",
-}
-
-
-class Parser:
-    def __init__(self, expand_includes: bool = True, include_comments: bool = False):
-        self.expand_includes = expand_includes
-        self.include_comments = include_comments
-        self._comments: list[Any] = []
-        self.lalr = self._create_lalr_parser()
-
-    def _create_lalr_parser(self) -> Any:
-        extra_args = {}
-
-        if lark_cython:
-            extra_args["_plugins"] = lark_cython.plugins
-
-        if self.include_comments:
-            callbacks = {
-                "COMMENT": self._comments.append,
-                "CCOMMENT": self._comments.append,
-            }
-            extra_args.update(
-                {"propagate_positions": True, "lexer_callbacks": callbacks}
-            )
-
-        return Lark.open("mapfile.lark", rel_to=__file__, parser="lalr", **extra_args)
-
-    def _get_include_filename(self, line: str) -> str:
-        if "#" in line:
-            # remove any comments on the same line
-            line = line.split("#")[0]
-
-        include_pairs = line.split()
-        if len(include_pairs) > 2:
-            log.warning(
-                "Multiple include files have been found on the same line. "
-                "Only the first will be used. "
-            )
-        inc_file_path = include_pairs[1]
-
-        return inc_file_path.strip("'").strip('"')
-
-    def load_includes(
-        self, text: str, fn: (str | None) = None, _nested_includes: int = 0
-    ) -> str:
-        # Per default use working directory of the process
-        if fn is None:
-            fn = os.getcwd() + os.sep
-
-        lines = text.split("\n")
-        includes = {}
-        for idx, l in enumerate(lines):
-            if l.strip().lower().startswith("include"):
-                if _nested_includes == 5:
-                    raise ValueError("Maximum nested include exceeded! (MaxNested=5)")
-
-                inc_file_path = self._get_include_filename(l)
-
-                if not os.path.isabs(inc_file_path):
-                    inc_file_path = os.path.abspath(
-                        os.path.join(os.path.dirname(fn), inc_file_path)
-                    )
-                try:
-                    include_text = self.open_file(inc_file_path)
-                except IOError as ex:
-                    log.warning(
-                        "Include file '%s' not found in '%s'", inc_file_path, fn
-                    )
-                    raise ex
-                # recursively load any further includes
-                includes[idx] = self.load_includes(
-                    include_text, fn=fn, _nested_includes=_nested_includes + 1
-                )
-
-        for idx, txt in includes.items():
-            lines.pop(idx)  # remove the original include
-            lines.insert(idx, txt)
-        return "\n".join(lines)
-
-    def _assign_comments(self, _tree: Any) -> None:
-        for node in _tree.children:
-            if not isinstance(node, Tree):
-                continue
-
-            if not hasattr(node.meta, "line"):
-                continue
-
-            line = node.meta.line
-
-            # when we encounter a new type that can have associated comments
-            # assign all comments up to that point in the Mapfile to the node
-            # for metadata we want to assign comments to the string_pair
-            if node.data in ("composite", "attr", "projection", "string_pair"):
-                # for projection blocks capture any comments within the block
-
-                if node.data in ("projection"):
-                    line = node.meta.end_line
-                line_numbers = list(sorted(self.comments_dict.keys()))
-                comments = []
-
-                for line_number in line_numbers:
-                    if line_number <= line:
-                        comments.append(self.comments_dict.pop(line_number))
-
-                if comments:
-                    node.meta.comments = comments  # type: ignore
-
-            if isinstance(node, Tree):
-                self._assign_comments(node)
-
-    def load(self, fp: IO[str]) -> Any:
-        text = fp.read()
-        if hasattr(fp, "name"):
-            fn = (
-                fp.name
-            )  # name is a read-only attribute and may not be present on all file-like objects.
-        else:
-            fn = None
-        return self.parse(text, fn)
-
-    def open_file(self, fn: str):
-        try:
-            with open(fn, "r", encoding="utf-8") as f:
-                return f.read()
-        except UnicodeDecodeError as ex:
-            log.debug(ex)
-            log.error(
-                "Please check the encoding for %s. All Mapfiles should be in utf-8 format.",
-                fn,
-            )
-            raise
-
-    def parse_file(self, fn: str) -> Any:
-        text = self.open_file(fn)
-        return self.parse(text, fn=fn)
-
-    def parse(self, text: str, fn: (str | None) = None) -> Any:
-        """
-        Parse the Mapfile
-        """
-
-        if self.expand_includes:
-            text = self.load_includes(text, fn=fn)
-
-        try:
-            self._comments[:] = []  # clear any comments from a previous parse
-            ip = self.lalr.parse_interactive(text)
-            for t in ip.iter_parse():
-                if t.type == "UNQUOTED_STRING":
-                    # Unquoted strings after SYMBOL can only be values, not attributes
-                    if (
-                        ip.parser_state.value_stack[-1] == "SYMBOL"
-                        and t.value.upper() not in SYMBOL_ATTRIBUTES
-                    ):
-                        t.type = "UNQUOTED_STRING_VALUE"
-                elif t.type == "GRID":
-                    # Unquoted 'GRID' coming after NAME is always a value, not a composite type
-                    if ip.parser_state.value_stack[-1] == "NAME":
-                        t.type = "UNQUOTED_STRING_VALUE"
-
-            tree = ip.resume_parse()
-            if self.include_comments:
-                self.comments_dict = {}
-                # create a dictionary using line numbers as keys, and comments as values
-                for c in self._comments:
-                    self.comments_dict[c.line] = c.value.strip()
-                self._assign_comments(tree)
-
-            return tree
-        except (ParseError, UnexpectedInput) as ex:
-            if fn:
-                log.error("Parsing of %s unsuccessful", fn)
-            else:
-                log.error("Parsing of Mapfile unsuccessful")
-            log.info(ex)
-            raise
+# =================================================================
+#
+# Authors: Seth Girvin, Erez Shinan
+#
+# Copyright (c) 2020 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+from __future__ import annotations
+import os
+import logging
+from io import open
+from lark import Lark, ParseError, Tree, UnexpectedInput
+from typing import Any, IO
+
+
+log = logging.getLogger("mappyfile")
+
+
+def string_to_boolean(string_value: str):
+    return string_value.lower() not in ("false", "no", "0", "off")
+
+
+use_cython = string_to_boolean(os.environ.get("MAPPYFILE_USE_CYTHON", "True"))
+lark_cython = None
+
+if use_cython:
+    try:
+        import lark_cython  # type: ignore
+    except ImportError:
+        pass
+
+
+SYMBOL_ATTRIBUTES = {
+    "ANCHORPOINT",
+    "ANTIALIAS",
+    "FILLED",
+    "FONT",
+    "IMAGE",
+    "NAME",
+    "COLOR",
+    "TYPE",
+    "CHARACTER",
+    "POINTS",
+    "TRANSPARENT",
+}
+
+
+class Parser:
+    def __init__(
+        self, expand_includes: bool = True, include_comments: bool = False, **kwargs
+    ):
+        self.expand_includes = expand_includes
+        self.include_comments = include_comments
+        self._comments: list[Any] = []
+        self.lalr = self._create_lalr_parser()
+        self.kwargs = kwargs
+
+    def _create_lalr_parser(self) -> Any:
+        extra_args = {}
+
+        if lark_cython:
+            extra_args["_plugins"] = lark_cython.plugins
+
+        if self.include_comments:
+            callbacks = {
+                "COMMENT": self._comments.append,
+                "CCOMMENT": self._comments.append,
+            }
+            extra_args.update(
+                {"propagate_positions": True, "lexer_callbacks": callbacks}
+            )
+
+        return Lark.open("mapfile.lark", rel_to=__file__, parser="lalr", **extra_args)
+
+    def _get_include_filename(self, line: str) -> str:
+        if "#" in line:
+            # remove any comments on the same line
+            line = line.split("#")[0]
+
+        include_pairs = line.split()
+        if len(include_pairs) > 2:
+            log.warning(
+                "Multiple include files have been found on the same line. "
+                "Only the first will be used. "
+            )
+        inc_file_path = include_pairs[1]
+
+        return inc_file_path.strip("'").strip('"')
+
+    def load_includes(
+        self, text: str, fn: str | None = None, _nested_includes: int = 0
+    ) -> str:
+        # Per default use working directory of the process
+        if fn is None:
+            fn = os.getcwd() + os.sep
+
+        lines = text.split("\n")
+        includes = {}
+        for idx, l in enumerate(lines):
+            if l.strip().lower().startswith("include"):
+                if _nested_includes == 5:
+                    raise ValueError("Maximum nested include exceeded! (MaxNested=5)")
+
+                inc_file_path = self._get_include_filename(l)
+
+                if not os.path.isabs(inc_file_path):
+                    inc_file_path = os.path.abspath(
+                        os.path.join(os.path.dirname(fn), inc_file_path)
+                    )
+                try:
+                    include_text = self.open_file(inc_file_path)
+                except IOError as ex:
+                    log.warning(
+                        "Include file '%s' not found in '%s'", inc_file_path, fn
+                    )
+                    raise ex
+                # recursively load any further includes
+                includes[idx] = self.load_includes(
+                    include_text, fn=fn, _nested_includes=_nested_includes + 1
+                )
+
+        for idx, txt in includes.items():
+            lines.pop(idx)  # remove the original include
+            lines.insert(idx, txt)
+        return "\n".join(lines)
+
+    def _assign_comments(self, _tree: Any) -> None:
+        for node in _tree.children:
+            if not isinstance(node, Tree):
+                continue
+
+            if not hasattr(node.meta, "line"):
+                continue
+
+            line = node.meta.line
+
+            # when we encounter a new type that can have associated comments
+            # assign all comments up to that point in the Mapfile to the node
+            # for metadata we want to assign comments to the string_pair
+            if node.data in ("composite", "attr", "projection", "string_pair"):
+                # for projection blocks capture any comments within the block
+
+                if node.data in ("projection"):
+                    line = node.meta.end_line
+                line_numbers = list(sorted(self.comments_dict.keys()))
+                comments = []
+
+                for line_number in line_numbers:
+                    if line_number <= line:
+                        comments.append(self.comments_dict.pop(line_number))
+
+                if comments:
+                    node.meta.comments = comments  # type: ignore
+
+            if isinstance(node, Tree):
+                self._assign_comments(node)
+
+    def load(self, fp: IO[str]) -> Any:
+        text = fp.read()
+        if hasattr(fp, "name"):
+            fn = (
+                fp.name
+            )  # name is a read-only attribute and may not be present on all file-like objects.
+        else:
+            fn = None
+        return self.parse(text, fn)
+
+    def open_file(self, fn: str):
+        try:
+            with open(fn, "r", encoding="utf-8") as f:
+                return f.read()
+        except UnicodeDecodeError as ex:
+            log.debug(ex)
+            log.error(
+                "Please check the encoding for %s. All Mapfiles should be in utf-8 format.",
+                fn,
+            )
+            raise
+
+    def parse_file(self, fn: str) -> Any:
+        text = self.open_file(fn)
+        return self.parse(text, fn=fn)
+
+    def parse(self, text: str, fn: str | None = None) -> Any:
+        """
+        Parse the Mapfile
+        """
+
+        if self.expand_includes:
+            text = self.load_includes(text, fn=fn)
+
+        try:
+            self._comments[:] = []  # clear any comments from a previous parse
+            ip = self.lalr.parse_interactive(text)
+            for t in ip.iter_parse():
+                if t.type == "UNQUOTED_STRING":
+                    # Unquoted strings after SYMBOL can only be values, not attributes
+                    if (
+                        ip.parser_state.value_stack[-1] == "SYMBOL"
+                        and t.value.upper() not in SYMBOL_ATTRIBUTES
+                    ):
+                        t.type = "UNQUOTED_STRING_VALUE"
+                elif t.type == "GRID":
+                    # Unquoted 'GRID' coming after NAME is always a value, not a composite type
+                    if ip.parser_state.value_stack[-1] == "NAME":
+                        t.type = "UNQUOTED_STRING_VALUE"
+
+            tree = ip.resume_parse()
+            if self.include_comments:
+                self.comments_dict = {}
+                # create a dictionary using line numbers as keys, and comments as values
+                for c in self._comments:
+                    self.comments_dict[c.line] = c.value.strip()
+                self._assign_comments(tree)
+
+            return tree
+        except (ParseError, UnexpectedInput) as ex:
+            if fn:
+                log.error("Parsing of %s unsuccessful", fn)
+            else:
+                log.error("Parsing of Mapfile unsuccessful")
+            log.info(ex)
+            raise
```

### Comparing `mappyfile-1.0.1/mappyfile/pprint.py` & `mappyfile-1.0.2/mappyfile/pprint.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,575 +1,575 @@
-# =================================================================
-#
-# Authors: Seth Girvin
-#
-# Copyright (c) 2020 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-from __future__ import annotations
-import logging
-import numbers
-from mappyfile.tokens import (
-    COMPOSITE_NAMES,
-    SINGLETON_COMPOSITE_NAMES,
-    REPEATED_KEYS,
-    COMPLEX_TYPES,
-    OBJECT_LIST_KEYS,
-)
-from mappyfile.validator import Validator
-from mappyfile.quoter import Quoter
-from mappyfile import dictutils
-from typing import Any
-
-
-log = logging.getLogger("mappyfile")
-
-
-# pylint: disable=too-many-arguments
-class PrettyPrinter:
-    def __init__(
-        self,
-        indent: int = 4,
-        spacer: str = " ",
-        quote: str = '"',
-        newlinechar: str = "\n",
-        end_comment: bool = False,
-        align_values: bool = False,
-        separate_complex_types: bool = False,
-    ):
-        """
-        Option use "\t" for spacer with an indent of 1
-        """
-
-        assert quote in ("'", '"')
-
-        self.indent = indent
-        self.spacer = spacer * self.indent
-        self.quoter = Quoter(quote)
-        self.newlinechar = newlinechar
-        self.end_comment = end_comment
-        self.end = "END"
-        self.validator = Validator()
-        self.align_values = align_values
-        self.separate_complex_types = separate_complex_types
-
-    def __is_metadata(self, key: str) -> bool:
-        """
-        Check to see if the property is hidden metadata
-        e.g. "__type__", "__comments__", "__position__"
-        """
-        if key.startswith("__") and key.endswith("__"):
-            return True
-
-        return False
-
-    def compute_aligned_max_indent(self, max_key_length: int) -> int:
-        """
-        Computes the indentation as a multiple of self.indent for aligning
-        values at the same column based on the maximum key length.
-        Example:
-        key         value1
-        longkey     value2
-        longestkey  value3 <-- column at 12, indent of 4, determined by "longestkey"
-        """
-        indent = max(1, self.indent)
-        return int((int(max_key_length / indent) + 1) * indent)
-
-    def compute_max_key_length(self, composite: dict) -> int:
-        """
-        Computes the maximum length of all keys (non-recursive) in the passed
-        composite.
-        """
-        length = 0
-
-        ignore_list = (
-            "metadata",
-            "validation",
-            "values",
-            "connectionoptions",
-            "pattern",
-            "projection",
-            "points",
-            "config",
-        )
-
-        for attr, value in composite.items():
-            attr_length = len(attr)
-            if (
-                not self.__is_metadata(attr)
-                and attr not in ignore_list
-                and not self.is_hidden_container(attr, value)
-                and not self.is_composite(value)
-            ):
-                length = max(length, attr_length)
-
-        return length
-
-    def separate_complex(self, composite: dict, level: int) -> None:
-        if not self.separate_complex_types:
-            return
-        for key in list(composite.keys()):
-            if self.is_complex_type(composite, key, level):
-                dictutils.dict_move_to_end(composite, key)
-
-    def whitespace(self, level: int, indent: int) -> str:
-        return self.spacer * (level + indent)
-
-    def add_start_line(self, key: str, level: int) -> str:
-        return self.whitespace(level, 1) + key.upper()
-
-    def add_end_line(self, level: int, indent: int, key: str) -> str:
-        end_line = self.whitespace(level, indent) + self.end
-        if self.end_comment:
-            end_line = f"{end_line} # {key.upper()}"
-        return end_line
-
-    def __format_line(
-        self, spacer: str, key: str, value: Any, aligned_max_indent: int = 0
-    ) -> str:
-        if (aligned_max_indent is None) or (aligned_max_indent == 0):
-            aligned_max_indent = len(key) + 1
-        indent = " " * (aligned_max_indent - len(key))
-        tmpl = "{spacer}{key}{indent}{value}"
-        d = {"spacer": spacer, "key": key, "value": value, "indent": indent}
-        return tmpl.format(**d)
-
-    def process_key_dict(self, key: str, d: dict, level: int) -> list[str]:
-        """
-        Process key value dicts e.g. METADATA "key" "value"
-        """
-
-        # add any composite level comments
-        comments = d.get("__comments__", {})
-        lines: list[str] = []
-        self._add_type_comment(level, comments, lines)
-
-        lines += [self.add_start_line(key, level)]
-        lines += self.process_dict(d, level, comments)
-        lines.append(self.add_end_line(level, 1, key))
-
-        return lines
-
-    def process_dict(self, d: dict, level: int, comments: dict) -> list[str]:
-        """
-        Process keys and values within a block
-        """
-        lines = []
-
-        aligned_max_indent = 0
-        if self.align_values:
-            max_key_length = self.compute_max_key_length(d) + 2  # add length of quotes
-            aligned_max_indent = self.compute_aligned_max_indent(max_key_length)
-
-        for k, v in d.items():
-            if not self.__is_metadata(k):
-                qk = self.quoter.add_quotes(k)
-                qv = self.quoter.add_quotes(v)
-                line = self.__format_line(
-                    self.whitespace(level, 2), qk, qv, aligned_max_indent
-                )
-                line += self.process_attribute_comment(comments, k)
-                lines.append(line)
-
-        return lines
-
-    def process_config_dict(self, d: dict, level: int) -> list[str]:
-        """
-        Process the CONFIG block
-        """
-        lines = []
-        for k, v in d.items():
-            cfg_val = self.quoter.add_quotes(k.upper())
-            k = f"CONFIG {cfg_val}"
-            v = self.quoter.add_quotes(v)
-            lines.append(self.__format_line(self.whitespace(level, 1), k, v))
-        return lines
-
-    def process_repeated_list(
-        self, key: str, lst: list[str], level: int, aligned_max_indent: int = 1
-    ) -> list[str]:
-        """
-        Process blocks of repeated keys e.g. FORMATOPTION
-        """
-        lines = []
-
-        for v in lst:
-            k = key.upper()
-            v = self.quoter.add_quotes(v)
-            lines.append(
-                self.__format_line(self.whitespace(level, 1), k, v, aligned_max_indent)
-            )
-
-        return lines
-
-    def process_projection(
-        self, key, lst: (str | list[str]), level: int, projection_comments: str
-    ) -> list[str]:
-        lines = [self.add_start_line(key, level)]
-
-        whitespace = self.whitespace(level, 2)
-
-        if projection_comments:
-            lines.append(f"{whitespace}{projection_comments.strip()}")
-
-        if self.quoter.is_string(lst):
-            val = self.quoter.add_quotes(str(lst))
-            # the value has been manually set to a single string projection
-            lines.append(f"{whitespace}{val}")
-        elif len(lst) == 1 and lst[0].upper() == "AUTO":
-            lines.append(f"{whitespace}AUTO")
-        else:
-            for v in lst:
-                v = self.quoter.add_quotes(v)
-                lines.append(f"{whitespace}{v}")
-
-        lines.append(self.add_end_line(level, 1, key))
-        return lines
-
-    def format_pair_list(self, key: str, pair_list: list[Any], level: int) -> list[str]:
-        """
-        Process lists of pairs (e.g. PATTERN block)
-        """
-
-        lines = [self.add_start_line(key, level)]
-
-        list_spacer = self.spacer * (level + 2)
-        pairs = [f"{list_spacer}{p[0]} {p[1]}" for p in pair_list]
-        lines += pairs
-
-        lines.append(self.add_end_line(level, 1, key))
-
-        return lines
-
-    def format_repeated_pair_list(
-        self, key: str, root_list: list[Any], level: int
-    ) -> list[str]:
-        """
-        Process (possibly) repeated lists of pairs e.g. POINTs blocks
-        """
-
-        lines = []
-
-        def depth(iterable):
-            return isinstance(iterable, (tuple, list)) and max(map(depth, iterable)) + 1
-
-        if depth(root_list) == 2:
-            # single set of points only
-            root_list = [root_list]
-
-        for pair_list in root_list:
-            lines += self.format_pair_list(key, pair_list, level)
-
-        return lines
-
-    def is_composite(self, val: Any) -> bool:
-        if isinstance(val, dict) and "__type__" in val:
-            return True
-        return False
-
-    def is_complex_type(self, composite: dict, key: str, level: int) -> bool:
-        # symbol needs special treatment
-        if key == "symbol" and level > 0:
-            return False
-        return (
-            key in COMPLEX_TYPES
-            or self.is_composite(key)
-            or self.is_hidden_container(key, composite[key])
-        )
-
-    def is_hidden_container(self, key: str, val: Any) -> bool:
-        """
-        The key is not one of the Mapfile keywords, and its
-        values are a list
-        """
-
-        if key in OBJECT_LIST_KEYS and isinstance(val, list):
-            return True
-        return False
-
-    def pprint(self, composites: (dict | list[dict])) -> str:
-        """
-        Print out a nicely indented Mapfile
-        """
-
-        # if only a single composite is used then cast to list
-        # and allow for multiple root composites
-
-        if composites and not isinstance(composites, list):
-            composites = [composites]
-
-        lines = []
-
-        for composite in composites:
-            type_ = composite["__type__"]
-            if type_ in ("metadata", "validation", "connectionoptions"):
-                # types are being parsed directly, and not as an attr of a parent
-                lines += self.process_key_dict(type_, composite, level=0)
-            else:
-                lines += self._format(composite)
-
-        result = str(self.newlinechar.join(lines))
-        return result
-
-    def get_attribute_properties(self, type_: str, attr: str) -> dict:
-        jsn_schema = self.validator.get_expanded_schema(type_)
-        props = jsn_schema["properties"]
-
-        # check if a value needs to be quoted or not, by referring to the JSON schema
-
-        try:
-            attr_props = props[attr]
-        except KeyError as ex:
-            log.error(
-                "The key '%s' was not found in the JSON schema for '%s'", attr, type_
-            )
-            log.error(ex)
-            return {}
-
-        return attr_props
-
-    def is_expression(self, option):
-        return "description" in option and (option["description"] == "expression")
-
-    def check_options_list(self, options_list, value):
-        for option in options_list:
-            if "enum" in option and value.lower() in option["enum"]:
-                if value.lower() == "end":
-                    # in GEOTRANSFORM "end" is an attribute value
-                    return self.quoter.add_quotes(value)
-                return value.upper()
-
-            if self.is_expression(option):
-                if value.endswith("'i") or value.endswith('"i'):
-                    return value
-
-        if self.quoter.in_slashes(value):
-            return value
-
-        return self.quoter.add_quotes(value)
-
-    def format_value(self, attr: str, attr_props, value: Any) -> Any:
-        """
-        TODO - refactor and add more specific tests (particularly for expressions)
-        """
-        if isinstance(value, bool):
-            return str(value).upper()
-
-        if any(i in ["enum"] for i in attr_props):
-            if isinstance(value, dict) and not value:
-                raise ValueError(
-                    f"The property {attr} has an empty dictionary as a value"
-                )
-
-            if not isinstance(value, numbers.Number):
-                if attr == "compop":
-                    return self.quoter.add_quotes(str(value))
-                return str(value).upper()  # value is from a set list, no need for quote
-
-            return value
-
-        if (
-            "type" in attr_props and attr_props["type"] == "string"
-        ):  # and "enum" not in attr_props
-            # check schemas for expressions and handle accordingly
-            if self.is_expression(attr_props) and self.quoter.in_slashes(value):
-                return value
-            if self.is_expression(attr_props) and (
-                value.endswith("'i") or value.endswith('"i')
-            ):
-                # for case insensitive regex
-                return value
-
-            return self.quoter.add_quotes(value)
-
-        # expressions can be one of a string or an expression in brackets
-        if any(
-            i in ["oneOf", "anyOf"] for i in attr_props
-        ):  # and check that type string is in list
-            if "oneOf" in attr_props:
-                options_list = attr_props["oneOf"]
-            else:
-                options_list = attr_props["anyOf"]
-            if self.quoter.is_string(value):
-                if self.quoter.in_parenthesis(value):
-                    pass
-                elif attr == "expression" and self.quoter.in_braces(value):
-                    # don't add quotes to list expressions such as {val1, val2}
-                    pass
-                elif attr != "text" and self.quoter.in_brackets(value):
-                    # TEXT expressions are often "[field1]-[field2]" so need to leave quotes for these
-                    pass
-                elif value.startswith("NOT ") and self.quoter.in_parenthesis(value[4:]):
-                    value = f"NOT {value[4:]}"
-                else:
-                    value = self.check_options_list(options_list, value)
-
-        if isinstance(value, list):
-            new_values = []
-
-            for v in value:
-                if not isinstance(v, numbers.Number) and attr not in [
-                    "offset",
-                    "polaroffset",
-                ]:
-                    # don't add quotes to list of attributes for offset / polaroffset
-                    v = self.quoter.add_quotes(v)
-                new_values.append(v)
-
-            value = " ".join(list(map(str, new_values)))
-        else:
-            value = self.quoter.escape_quotes(value)
-
-        return value
-
-    # pylint: disable=too-many-arguments
-    def process_attribute(
-        self, type_: str, attr: str, value: Any, level: int, aligned_max_indent: int = 1
-    ) -> str:
-        """
-        Process one of the main composite types (see the type_ value)
-        """
-
-        attr_props = self.get_attribute_properties(type_, attr)
-        value = self.format_value(attr, attr_props, value)
-        line = self.__format_line(
-            self.whitespace(level, 1), attr.upper(), value, aligned_max_indent
-        )
-        return line
-
-    def format_comment(self, spacer: str, value: str) -> str:
-        return f"{spacer}{value}"
-
-    def process_composite_comment(self, level: int, comments: dict, key: str) -> str:
-        """
-        Process comments for composites such as MAP, LAYER etc.
-        """
-        if key not in comments:
-            comment = ""
-        else:
-            value = comments[key]
-            spacer = self.whitespace(level, 0)
-
-            if isinstance(value, list):
-                comment_list = [self.format_comment(spacer, v) for v in value]
-                comment = self.newlinechar.join(comment_list)
-            else:
-                comment = self.format_comment(spacer, value)
-
-        return comment
-
-    def process_attribute_comment(self, comments: dict, key: str) -> str:
-        if key not in comments:
-            comment = ""
-        else:
-            value = comments[key]
-            spacer = " "
-
-            # for multiple comments associated with an attribute
-            # simply join them together as a single string
-            if isinstance(value, list):
-                value = " ".join(value)
-
-            comment = self.format_comment(spacer, value)
-
-        return comment
-
-    def _add_type_comment(self, level: int, comments: dict, lines: list[str]) -> None:
-        comment = self.process_composite_comment(level, comments, "__type__")
-
-        if comment:
-            lines.append(str(comment))
-
-    def _format(self, composite: dict, level: int = 0) -> list[str]:
-        lines: list[str] = []
-        type_ = ""
-
-        # get any comments associated with the composite
-        comments = composite.get("__comments__", {})
-
-        if isinstance(composite, dict) and "__type__" in composite:
-            type_ = composite["__type__"]
-            assert type_ in COMPOSITE_NAMES.union(SINGLETON_COMPOSITE_NAMES)
-            is_hidden = False
-            self._add_type_comment(level, comments, lines)
-            s = self.whitespace(level, 0) + type_.upper()
-            lines.append(s)
-
-        aligned_max_indent = 0
-        if self.align_values:
-            max_key_length = self.compute_max_key_length(composite)
-            aligned_max_indent = self.compute_aligned_max_indent(max_key_length)
-
-        self.separate_complex(composite, level)
-
-        for attr, value in composite.items():
-            if self.__is_metadata(attr):
-                # skip hidden attributes
-                continue
-
-            if self.is_hidden_container(attr, value):
-                # now recursively print all the items in the container
-                for v in value:
-                    lines += self._format(v, level + 1)
-            elif attr == "pattern":
-                lines += self.format_pair_list(attr, value, level)
-            elif attr in ("metadata", "validation", "values", "connectionoptions"):
-                # metadata and values are also composites
-                # but will be processed here
-                lines += self.process_key_dict(attr, value, level)
-
-            elif attr == "projection":
-                projection_comments = self.process_attribute_comment(comments, attr)
-                lines += self.process_projection(
-                    attr, value, level, projection_comments
-                )
-            elif attr in REPEATED_KEYS:
-                lines += self.process_repeated_list(
-                    attr, value, level, aligned_max_indent
-                )
-            elif attr == "points":
-                lines += self.format_repeated_pair_list(attr, value, level)
-            elif attr == "config":
-                lines += self.process_config_dict(value, level)
-            elif self.is_composite(value):
-                lines += self._format(
-                    value, level + 1
-                )  # recursively add the child class
-            else:
-                # standard key value pair
-                if not type_:
-                    raise UnboundLocalError(
-                        "The Mapfile object is missing a __type__ attribute"
-                    )
-                line = self.process_attribute(
-                    type_, attr, value, level, aligned_max_indent
-                )
-                line += self.process_attribute_comment(comments, attr)
-                lines.append(line)
-
-        if not is_hidden:
-            # close the container block with an END
-            lines.append(self.add_end_line(level, 0, type_))
-
-        return lines
+# =================================================================
+#
+# Authors: Seth Girvin
+#
+# Copyright (c) 2020 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+from __future__ import annotations
+import logging
+import numbers
+from mappyfile.tokens import (
+    COMPOSITE_NAMES,
+    SINGLETON_COMPOSITE_NAMES,
+    REPEATED_KEYS,
+    COMPLEX_TYPES,
+    OBJECT_LIST_KEYS,
+)
+from mappyfile.validator import Validator
+from mappyfile.quoter import Quoter
+from mappyfile import dictutils
+from typing import Any
+
+
+log = logging.getLogger("mappyfile")
+
+
+# pylint: disable=too-many-arguments
+class PrettyPrinter:
+    def __init__(
+        self,
+        indent: int = 4,
+        spacer: str = " ",
+        quote: str = '"',
+        newlinechar: str = "\n",
+        end_comment: bool = False,
+        align_values: bool = False,
+        separate_complex_types: bool = False,
+    ):
+        """
+        Option use "\t" for spacer with an indent of 1
+        """
+
+        assert quote in ("'", '"')
+
+        self.indent = indent
+        self.spacer = spacer * self.indent
+        self.quoter = Quoter(quote)
+        self.newlinechar = newlinechar
+        self.end_comment = end_comment
+        self.end = "END"
+        self.validator = Validator()
+        self.align_values = align_values
+        self.separate_complex_types = separate_complex_types
+
+    def __is_metadata(self, key: str) -> bool:
+        """
+        Check to see if the property is hidden metadata
+        e.g. "__type__", "__comments__", "__position__"
+        """
+        if key.startswith("__") and key.endswith("__"):
+            return True
+
+        return False
+
+    def compute_aligned_max_indent(self, max_key_length: int) -> int:
+        """
+        Computes the indentation as a multiple of self.indent for aligning
+        values at the same column based on the maximum key length.
+        Example:
+        key         value1
+        longkey     value2
+        longestkey  value3 <-- column at 12, indent of 4, determined by "longestkey"
+        """
+        indent = max(1, self.indent)
+        return int((int(max_key_length / indent) + 1) * indent)
+
+    def compute_max_key_length(self, composite: dict) -> int:
+        """
+        Computes the maximum length of all keys (non-recursive) in the passed
+        composite.
+        """
+        length = 0
+
+        ignore_list = (
+            "metadata",
+            "validation",
+            "values",
+            "connectionoptions",
+            "pattern",
+            "projection",
+            "points",
+            "config",
+        )
+
+        for attr, value in composite.items():
+            attr_length = len(attr)
+            if (
+                not self.__is_metadata(attr)
+                and attr not in ignore_list
+                and not self.is_hidden_container(attr, value)
+                and not self.is_composite(value)
+            ):
+                length = max(length, attr_length)
+
+        return length
+
+    def separate_complex(self, composite: dict, level: int) -> None:
+        if not self.separate_complex_types:
+            return
+        for key in list(composite.keys()):
+            if self.is_complex_type(composite, key, level):
+                dictutils.dict_move_to_end(composite, key)
+
+    def whitespace(self, level: int, indent: int) -> str:
+        return self.spacer * (level + indent)
+
+    def add_start_line(self, key: str, level: int) -> str:
+        return self.whitespace(level, 1) + key.upper()
+
+    def add_end_line(self, level: int, indent: int, key: str) -> str:
+        end_line = self.whitespace(level, indent) + self.end
+        if self.end_comment:
+            end_line = f"{end_line} # {key.upper()}"
+        return end_line
+
+    def __format_line(
+        self, spacer: str, key: str, value: Any, aligned_max_indent: int = 0
+    ) -> str:
+        if (aligned_max_indent is None) or (aligned_max_indent == 0):
+            aligned_max_indent = len(key) + 1
+        indent = " " * (aligned_max_indent - len(key))
+        tmpl = "{spacer}{key}{indent}{value}"
+        d = {"spacer": spacer, "key": key, "value": value, "indent": indent}
+        return tmpl.format(**d)
+
+    def process_key_dict(self, key: str, d: dict, level: int) -> list[str]:
+        """
+        Process key value dicts e.g. METADATA "key" "value"
+        """
+
+        # add any composite level comments
+        comments = d.get("__comments__", {})
+        lines: list[str] = []
+        self._add_type_comment(level, comments, lines)
+
+        lines += [self.add_start_line(key, level)]
+        lines += self.process_dict(d, level, comments)
+        lines.append(self.add_end_line(level, 1, key))
+
+        return lines
+
+    def process_dict(self, d: dict, level: int, comments: dict) -> list[str]:
+        """
+        Process keys and values within a block
+        """
+        lines = []
+
+        aligned_max_indent = 0
+        if self.align_values:
+            max_key_length = self.compute_max_key_length(d) + 2  # add length of quotes
+            aligned_max_indent = self.compute_aligned_max_indent(max_key_length)
+
+        for k, v in d.items():
+            if not self.__is_metadata(k):
+                qk = self.quoter.add_quotes(k)
+                qv = self.quoter.add_quotes(v)
+                line = self.__format_line(
+                    self.whitespace(level, 2), qk, qv, aligned_max_indent
+                )
+                line += self.process_attribute_comment(comments, k)
+                lines.append(line)
+
+        return lines
+
+    def process_config_dict(self, d: dict, level: int) -> list[str]:
+        """
+        Process the CONFIG block
+        """
+        lines = []
+        for k, v in d.items():
+            cfg_val = self.quoter.add_quotes(k.upper())
+            k = f"CONFIG {cfg_val}"
+            v = self.quoter.add_quotes(v)
+            lines.append(self.__format_line(self.whitespace(level, 1), k, v))
+        return lines
+
+    def process_repeated_list(
+        self, key: str, lst: list[str], level: int, aligned_max_indent: int = 1
+    ) -> list[str]:
+        """
+        Process blocks of repeated keys e.g. FORMATOPTION
+        """
+        lines = []
+
+        for v in lst:
+            k = key.upper()
+            v = self.quoter.add_quotes(v)
+            lines.append(
+                self.__format_line(self.whitespace(level, 1), k, v, aligned_max_indent)
+            )
+
+        return lines
+
+    def process_projection(
+        self, key, lst: (str | list[str]), level: int, projection_comments: str
+    ) -> list[str]:
+        lines = [self.add_start_line(key, level)]
+
+        whitespace = self.whitespace(level, 2)
+
+        if projection_comments:
+            lines.append(f"{whitespace}{projection_comments.strip()}")
+
+        if self.quoter.is_string(lst):
+            val = self.quoter.add_quotes(str(lst))
+            # the value has been manually set to a single string projection
+            lines.append(f"{whitespace}{val}")
+        elif len(lst) == 1 and lst[0].upper() == "AUTO":
+            lines.append(f"{whitespace}AUTO")
+        else:
+            for v in lst:
+                v = self.quoter.add_quotes(v)
+                lines.append(f"{whitespace}{v}")
+
+        lines.append(self.add_end_line(level, 1, key))
+        return lines
+
+    def format_pair_list(self, key: str, pair_list: list[Any], level: int) -> list[str]:
+        """
+        Process lists of pairs (e.g. PATTERN block)
+        """
+
+        lines = [self.add_start_line(key, level)]
+
+        list_spacer = self.spacer * (level + 2)
+        pairs = [f"{list_spacer}{p[0]} {p[1]}" for p in pair_list]
+        lines += pairs
+
+        lines.append(self.add_end_line(level, 1, key))
+
+        return lines
+
+    def format_repeated_pair_list(
+        self, key: str, root_list: list[Any], level: int
+    ) -> list[str]:
+        """
+        Process (possibly) repeated lists of pairs e.g. POINTs blocks
+        """
+
+        lines = []
+
+        def depth(iterable):
+            return isinstance(iterable, (tuple, list)) and max(map(depth, iterable)) + 1
+
+        if depth(root_list) == 2:
+            # single set of points only
+            root_list = [root_list]
+
+        for pair_list in root_list:
+            lines += self.format_pair_list(key, pair_list, level)
+
+        return lines
+
+    def is_composite(self, val: Any) -> bool:
+        if isinstance(val, dict) and "__type__" in val:
+            return True
+        return False
+
+    def is_complex_type(self, composite: dict, key: str, level: int) -> bool:
+        # symbol needs special treatment
+        if key == "symbol" and level > 0:
+            return False
+        return (
+            key in COMPLEX_TYPES
+            or self.is_composite(key)
+            or self.is_hidden_container(key, composite[key])
+        )
+
+    def is_hidden_container(self, key: str, val: Any) -> bool:
+        """
+        The key is not one of the Mapfile keywords, and its
+        values are a list
+        """
+
+        if key in OBJECT_LIST_KEYS and isinstance(val, list):
+            return True
+        return False
+
+    def pprint(self, composites: (dict | list[dict])) -> str:
+        """
+        Print out a nicely indented Mapfile
+        """
+
+        # if only a single composite is used then cast to list
+        # and allow for multiple root composites
+
+        if composites and not isinstance(composites, list):
+            composites = [composites]
+
+        lines = []
+
+        for composite in composites:
+            type_ = composite["__type__"]
+            if type_ in ("metadata", "validation", "connectionoptions"):
+                # types are being parsed directly, and not as an attr of a parent
+                lines += self.process_key_dict(type_, composite, level=0)
+            else:
+                lines += self._format(composite)
+
+        result = str(self.newlinechar.join(lines))
+        return result
+
+    def get_attribute_properties(self, type_: str, attr: str) -> dict:
+        jsn_schema = self.validator.get_expanded_schema(type_)
+        props = jsn_schema["properties"]
+
+        # check if a value needs to be quoted or not, by referring to the JSON schema
+
+        try:
+            attr_props = props[attr]
+        except KeyError as ex:
+            log.error(
+                "The key '%s' was not found in the JSON schema for '%s'", attr, type_
+            )
+            log.error(ex)
+            return {}
+
+        return attr_props
+
+    def is_expression(self, option):
+        return "description" in option and (option["description"] == "expression")
+
+    def check_options_list(self, options_list, value):
+        for option in options_list:
+            if "enum" in option and value.lower() in option["enum"]:
+                if value.lower() == "end":
+                    # in GEOTRANSFORM "end" is an attribute value
+                    return self.quoter.add_quotes(value)
+                return value.upper()
+
+            if self.is_expression(option):
+                if value.endswith("'i") or value.endswith('"i'):
+                    return value
+
+        if self.quoter.in_slashes(value):
+            return value
+
+        return self.quoter.add_quotes(value)
+
+    def format_value(self, attr: str, attr_props, value: Any) -> Any:
+        """
+        TODO - refactor and add more specific tests (particularly for expressions)
+        """
+        if isinstance(value, bool):
+            return str(value).upper()
+
+        if any(i in ["enum"] for i in attr_props):
+            if isinstance(value, dict) and not value:
+                raise ValueError(
+                    f"The property {attr} has an empty dictionary as a value"
+                )
+
+            if not isinstance(value, numbers.Number):
+                if attr == "compop":
+                    return self.quoter.add_quotes(str(value))
+                return str(value).upper()  # value is from a set list, no need for quote
+
+            return value
+
+        if (
+            "type" in attr_props and attr_props["type"] == "string"
+        ):  # and "enum" not in attr_props
+            # check schemas for expressions and handle accordingly
+            if self.is_expression(attr_props) and self.quoter.in_slashes(value):
+                return value
+            if self.is_expression(attr_props) and (
+                value.endswith("'i") or value.endswith('"i')
+            ):
+                # for case insensitive regex
+                return value
+
+            return self.quoter.add_quotes(value)
+
+        # expressions can be one of a string or an expression in brackets
+        if any(
+            i in ["oneOf", "anyOf"] for i in attr_props
+        ):  # and check that type string is in list
+            if "oneOf" in attr_props:
+                options_list = attr_props["oneOf"]
+            else:
+                options_list = attr_props["anyOf"]
+            if self.quoter.is_string(value):
+                if self.quoter.in_parenthesis(value):
+                    pass
+                elif attr == "expression" and self.quoter.in_braces(value):
+                    # don't add quotes to list expressions such as {val1, val2}
+                    pass
+                elif attr != "text" and self.quoter.in_brackets(value):
+                    # TEXT expressions are often "[field1]-[field2]" so need to leave quotes for these
+                    pass
+                elif value.startswith("NOT ") and self.quoter.in_parenthesis(value[4:]):
+                    value = f"NOT {value[4:]}"
+                else:
+                    value = self.check_options_list(options_list, value)
+
+        if isinstance(value, list):
+            new_values = []
+
+            for v in value:
+                if not isinstance(v, numbers.Number) and attr not in [
+                    "offset",
+                    "polaroffset",
+                ]:
+                    # don't add quotes to list of attributes for offset / polaroffset
+                    v = self.quoter.add_quotes(v)
+                new_values.append(v)
+
+            value = " ".join(list(map(str, new_values)))
+        else:
+            value = self.quoter.escape_quotes(value)
+
+        return value
+
+    # pylint: disable=too-many-arguments
+    def process_attribute(
+        self, type_: str, attr: str, value: Any, level: int, aligned_max_indent: int = 1
+    ) -> str:
+        """
+        Process one of the main composite types (see the type_ value)
+        """
+
+        attr_props = self.get_attribute_properties(type_, attr)
+        value = self.format_value(attr, attr_props, value)
+        line = self.__format_line(
+            self.whitespace(level, 1), attr.upper(), value, aligned_max_indent
+        )
+        return line
+
+    def format_comment(self, spacer: str, value: str) -> str:
+        return f"{spacer}{value}"
+
+    def process_composite_comment(self, level: int, comments: dict, key: str) -> str:
+        """
+        Process comments for composites such as MAP, LAYER etc.
+        """
+        if key not in comments:
+            comment = ""
+        else:
+            value = comments[key]
+            spacer = self.whitespace(level, 0)
+
+            if isinstance(value, list):
+                comment_list = [self.format_comment(spacer, v) for v in value]
+                comment = self.newlinechar.join(comment_list)
+            else:
+                comment = self.format_comment(spacer, value)
+
+        return comment
+
+    def process_attribute_comment(self, comments: dict, key: str) -> str:
+        if key not in comments:
+            comment = ""
+        else:
+            value = comments[key]
+            spacer = " "
+
+            # for multiple comments associated with an attribute
+            # simply join them together as a single string
+            if isinstance(value, list):
+                value = " ".join(value)
+
+            comment = self.format_comment(spacer, value)
+
+        return comment
+
+    def _add_type_comment(self, level: int, comments: dict, lines: list[str]) -> None:
+        comment = self.process_composite_comment(level, comments, "__type__")
+
+        if comment:
+            lines.append(str(comment))
+
+    def _format(self, composite: dict, level: int = 0) -> list[str]:
+        lines: list[str] = []
+        type_ = ""
+
+        # get any comments associated with the composite
+        comments = composite.get("__comments__", {})
+
+        if isinstance(composite, dict) and "__type__" in composite:
+            type_ = composite["__type__"]
+            assert type_ in COMPOSITE_NAMES.union(SINGLETON_COMPOSITE_NAMES)
+            is_hidden = False
+            self._add_type_comment(level, comments, lines)
+            s = self.whitespace(level, 0) + type_.upper()
+            lines.append(s)
+
+        aligned_max_indent = 0
+        if self.align_values:
+            max_key_length = self.compute_max_key_length(composite)
+            aligned_max_indent = self.compute_aligned_max_indent(max_key_length)
+
+        self.separate_complex(composite, level)
+
+        for attr, value in composite.items():
+            if self.__is_metadata(attr):
+                # skip hidden attributes
+                continue
+
+            if self.is_hidden_container(attr, value):
+                # now recursively print all the items in the container
+                for v in value:
+                    lines += self._format(v, level + 1)
+            elif attr == "pattern":
+                lines += self.format_pair_list(attr, value, level)
+            elif attr in ("metadata", "validation", "values", "connectionoptions"):
+                # metadata and values are also composites
+                # but will be processed here
+                lines += self.process_key_dict(attr, value, level)
+
+            elif attr == "projection":
+                projection_comments = self.process_attribute_comment(comments, attr)
+                lines += self.process_projection(
+                    attr, value, level, projection_comments
+                )
+            elif attr in REPEATED_KEYS:
+                lines += self.process_repeated_list(
+                    attr, value, level, aligned_max_indent
+                )
+            elif attr == "points":
+                lines += self.format_repeated_pair_list(attr, value, level)
+            elif attr == "config":
+                lines += self.process_config_dict(value, level)
+            elif self.is_composite(value):
+                lines += self._format(
+                    value, level + 1
+                )  # recursively add the child class
+            else:
+                # standard key value pair
+                if not type_:
+                    raise UnboundLocalError(
+                        "The Mapfile object is missing a __type__ attribute"
+                    )
+                line = self.process_attribute(
+                    type_, attr, value, level, aligned_max_indent
+                )
+                line += self.process_attribute_comment(comments, attr)
+                lines.append(line)
+
+        if not is_hidden:
+            # close the container block with an END
+            lines.append(self.add_end_line(level, 0, type_))
+
+        return lines
```

### Comparing `mappyfile-1.0.1/mappyfile/quoter.py` & `mappyfile-1.0.2/mappyfile/quoter.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# =================================================================
-#
-# Authors: Seth Girvin
-#
-# Copyright (c) 2023 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-from __future__ import annotations
-import logging
-from typing import Any
-
-
-log = logging.getLogger("mappyfile")
-
-
-class Quoter:
-    """
-    A class to handle adding and standardising quotes around strings
-    """
-
-    def __init__(self, quote: str = '"'):
-        assert quote in ("'", '"')
-
-        self.quote = quote
-
-        if self.quote == "'":
-            self.altquote = '"'
-        else:
-            self.altquote = "'"
-
-    def add_quotes(self, val: str) -> str:
-        return self._add_quotes(val, self.quote)
-
-    def add_altquotes(self, val: str) -> str:
-        return self._add_quotes(val, self.altquote)
-
-    def _add_quotes(self, val: str, quote: str) -> str:
-        return f"{quote}{val}{quote}"
-
-    def in_quotes(self, val: str) -> bool:
-        return self._in_quotes(val, self.quote) or self._in_quotes(val, self.altquote)
-
-    def _in_quotes(self, val: str, char: str):
-        return val.startswith(char) and val.endswith(char)
-
-    def escape_quotes(self, val: Any) -> Any:
-        """
-        Escape any quotes in a value
-        """
-        if self.is_string(val) and self._in_quotes(val, self.quote):
-            # make sure any previously escaped quotes are not re-escaped
-            middle = self.remove_quotes(val).replace("\\" + self.quote, self.quote)
-            middle = middle.replace(self.quote, "\\" + self.quote)
-            val = self.add_quotes(middle)
-
-        return val
-
-    def is_string(self, val: Any) -> bool:
-        return isinstance(val, str)
-
-    def remove_quotes(self, val: Any) -> Any:
-        if isinstance(val, list):
-            return list(map(self.remove_quotes, val))
-
-        if not self.is_string(val):
-            return val
-
-        if self.in_quotes(val):
-            return val[1:-1]
-
-        return val
-
-    def in_brackets(self, val: str) -> bool:
-        val = val.strip()
-        return val.startswith("[") and val.endswith("]")
-
-    def in_parenthesis(self, val: str) -> bool:
-        val = val.strip()
-        return val.startswith("(") and val.endswith(")")
-
-    def in_braces(self, val: str) -> bool:
-        val = val.strip()
-        return val.startswith("{") and val.endswith("}")
-
-    def in_slashes(self, val: str) -> bool:
-        val = val.strip()
-        return self._in_quotes(val, "/")
-
-    def standardise_quotes(self, val: str) -> str:
-        """
-        Change the quotes used to wrap a value to the pprint default
-        E.g. "val" to 'val' or 'val' to "val"
-        """
-        if self._in_quotes(val, self.altquote):
-            middle = self.remove_quotes(val)
-            val = self.add_quotes(middle)
-
-        return self.escape_quotes(val)
+# =================================================================
+#
+# Authors: Seth Girvin
+#
+# Copyright (c) 2023 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+from __future__ import annotations
+import logging
+from typing import Any
+
+
+log = logging.getLogger("mappyfile")
+
+
+class Quoter:
+    """
+    A class to handle adding and standardising quotes around strings
+    """
+
+    def __init__(self, quote: str = '"'):
+        assert quote in ("'", '"')
+
+        self.quote = quote
+
+        if self.quote == "'":
+            self.altquote = '"'
+        else:
+            self.altquote = "'"
+
+    def add_quotes(self, val: str) -> str:
+        return self._add_quotes(val, self.quote)
+
+    def add_altquotes(self, val: str) -> str:
+        return self._add_quotes(val, self.altquote)
+
+    def _add_quotes(self, val: str, quote: str) -> str:
+        return f"{quote}{val}{quote}"
+
+    def in_quotes(self, val: str) -> bool:
+        return self._in_quotes(val, self.quote) or self._in_quotes(val, self.altquote)
+
+    def _in_quotes(self, val: str, char: str):
+        return val.startswith(char) and val.endswith(char)
+
+    def escape_quotes(self, val: Any) -> Any:
+        """
+        Escape any quotes in a value
+        """
+        if self.is_string(val) and self._in_quotes(val, self.quote):
+            # make sure any previously escaped quotes are not re-escaped
+            middle = self.remove_quotes(val).replace("\\" + self.quote, self.quote)
+            middle = middle.replace(self.quote, "\\" + self.quote)
+            val = self.add_quotes(middle)
+
+        return val
+
+    def is_string(self, val: Any) -> bool:
+        return isinstance(val, str)
+
+    def remove_quotes(self, val: Any) -> Any:
+        if isinstance(val, list):
+            return list(map(self.remove_quotes, val))
+
+        if not self.is_string(val):
+            return val
+
+        if self.in_quotes(val):
+            return val[1:-1]
+
+        return val
+
+    def in_brackets(self, val: str) -> bool:
+        val = val.strip()
+        return val.startswith("[") and val.endswith("]")
+
+    def in_parenthesis(self, val: str) -> bool:
+        val = val.strip()
+        return val.startswith("(") and val.endswith(")")
+
+    def in_braces(self, val: str) -> bool:
+        val = val.strip()
+        return val.startswith("{") and val.endswith("}")
+
+    def in_slashes(self, val: str) -> bool:
+        val = val.strip()
+        return self._in_quotes(val, "/")
+
+    def standardise_quotes(self, val: str) -> str:
+        """
+        Change the quotes used to wrap a value to the pprint default
+        E.g. "val" to 'val' or 'val' to "val"
+        """
+        if self._in_quotes(val, self.altquote):
+            middle = self.remove_quotes(val)
+            val = self.add_quotes(middle)
+
+        return self.escape_quotes(val)
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/feature.json` & `mappyfile-1.0.2/mappyfile/schemas/feature.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2270 726f 7065 7274 6965 7322  ..  "properties"
-00000080: 3a20 7b0d 0a20 2020 2022 5f5f 7479 7065  : {..    "__type
-00000090: 5f5f 223a 207b 0d0a 2020 2020 2020 2265  __": {..      "e
-000000a0: 6e75 6d22 3a20 5b20 2266 6561 7475 7265  num": [ "feature
-000000b0: 2220 5d0d 0a20 2020 207d 2c0d 0a20 2020  " ]..    },..   
-000000c0: 2022 696e 636c 7564 6522 3a20 7b0d 0a20   "include": {.. 
-000000d0: 2020 2020 2022 7479 7065 223a 2022 6172       "type": "ar
-000000e0: 7261 7922 2c0d 0a20 2020 2020 2022 6974  ray",..      "it
-000000f0: 656d 7322 3a20 7b0d 0a20 2020 2020 2020  ems": {..       
-00000100: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-00000110: 220d 0a20 2020 2020 207d 0d0a 2020 2020  "..      }..    
-00000120: 7d2c 0d0a 2020 2020 2270 6f69 6e74 7322  },..    "points"
-00000130: 3a20 7b0d 0a20 2020 2020 2022 6f6e 654f  : {..      "oneO
-00000140: 6622 3a20 5b0d 0a20 2020 2020 2020 207b  f": [..        {
-00000150: 0d0a 2020 2020 2020 2020 2020 2274 7970  ..          "typ
-00000160: 6522 3a20 2261 7272 6179 222c 0d0a 2020  e": "array",..  
-00000170: 2020 2020 2020 2020 2269 7465 6d73 223a          "items":
-00000180: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000190: 2224 7265 6622 3a20 2270 6f69 6e74 732e  "$ref": "points.
-000001a0: 6a73 6f6e 220d 0a20 2020 2020 2020 2020  json"..         
-000001b0: 207d 0d0a 2020 2020 2020 2020 7d2c 0d0a   }..        },..
-000001c0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000001d0: 2020 2020 2022 2472 6566 223a 2022 706f       "$ref": "po
-000001e0: 696e 7473 2e6a 736f 6e22 0d0a 2020 2020  ints.json"..    
-000001f0: 2020 2020 7d0d 0a20 2020 2020 205d 0d0a      }..      ]..
-00000200: 2020 2020 7d2c 0d0a 2020 2020 2269 7465      },..    "ite
-00000210: 6d73 223a 207b 0d0a 2020 2020 2020 2274  ms": {..      "t
-00000220: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
-00000230: 2020 2020 7d2c 0d0a 2020 2020 2274 6578      },..    "tex
-00000240: 7422 3a20 7b0d 0a20 2020 2020 2022 7479  t": {..      "ty
-00000250: 7065 223a 2022 7374 7269 6e67 220d 0a20  pe": "string".. 
-00000260: 2020 207d 2c0d 0a20 2020 2022 776b 7422     },..    "wkt"
-00000270: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000280: 223a 2022 7374 7269 6e67 220d 0a20 2020  ": "string"..   
-00000290: 207d 0d0a 2020 7d0d 0a7d 0d0a             }..  }..}..
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2270  $": {}.  },.  "p
+00000070: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00000080: 2020 225f 5f74 7970 655f 5f22 3a20 7b0a    "__type__": {.
+00000090: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000000a0: 2266 6561 7475 7265 2220 5d0a 2020 2020  "feature" ].    
+000000b0: 7d2c 0a20 2020 2022 696e 636c 7564 6522  },.    "include"
+000000c0: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+000000d0: 3a20 2261 7272 6179 222c 0a20 2020 2020  : "array",.     
+000000e0: 2022 6974 656d 7322 3a20 7b0a 2020 2020   "items": {.    
+000000f0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00000100: 696e 6722 0a20 2020 2020 207d 0a20 2020  ing".      }.   
+00000110: 207d 2c0a 2020 2020 2270 6f69 6e74 7322   },.    "points"
+00000120: 3a20 7b0a 2020 2020 2020 226f 6e65 4f66  : {.      "oneOf
+00000130: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+00000140: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000150: 2022 6172 7261 7922 2c0a 2020 2020 2020   "array",.      
+00000160: 2020 2020 2269 7465 6d73 223a 207b 0a20      "items": {. 
+00000170: 2020 2020 2020 2020 2020 2022 2472 6566             "$ref
+00000180: 223a 2022 706f 696e 7473 2e6a 736f 6e22  ": "points.json"
+00000190: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
+000001a0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000001b0: 7b0a 2020 2020 2020 2020 2020 2224 7265  {.          "$re
+000001c0: 6622 3a20 2270 6f69 6e74 732e 6a73 6f6e  f": "points.json
+000001d0: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
+000001e0: 2020 5d0a 2020 2020 7d2c 0a20 2020 2022    ].    },.    "
+000001f0: 6974 656d 7322 3a20 7b0a 2020 2020 2020  items": {.      
+00000200: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00000210: 0a20 2020 207d 2c0a 2020 2020 2274 6578  .    },.    "tex
+00000220: 7422 3a20 7b0a 2020 2020 2020 2274 7970  t": {.      "typ
+00000230: 6522 3a20 2273 7472 696e 6722 0a20 2020  e": "string".   
+00000240: 207d 2c0a 2020 2020 2277 6b74 223a 207b   },.    "wkt": {
+00000250: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+00000260: 7374 7269 6e67 220a 2020 2020 7d0a 2020  string".    }.  
+00000270: 7d0a 7d0a                                }.}.
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/join.json` & `mappyfile-1.0.2/mappyfile/schemas/join.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2270 726f 7065 7274 6965 7322  ..  "properties"
-00000080: 3a20 7b0d 0a20 2020 2022 5f5f 7479 7065  : {..    "__type
-00000090: 5f5f 223a 207b 0d0a 2020 2020 2020 2265  __": {..      "e
-000000a0: 6e75 6d22 3a20 5b20 226a 6f69 6e22 205d  num": [ "join" ]
-000000b0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2269  ..    },..    "i
-000000c0: 6e63 6c75 6465 223a 207b 0d0a 2020 2020  nclude": {..    
-000000d0: 2020 2274 7970 6522 3a20 2261 7272 6179    "type": "array
-000000e0: 222c 0d0a 2020 2020 2020 2269 7465 6d73  ",..      "items
-000000f0: 223a 207b 0d0a 2020 2020 2020 2020 2274  ": {..        "t
-00000100: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
-00000110: 2020 2020 2020 7d0d 0a20 2020 207d 2c0d        }..    },.
-00000120: 0a20 2020 2022 636f 6e6e 6563 7469 6f6e  .    "connection
-00000130: 223a 207b 0d0a 2020 2020 2020 2274 7970  ": {..      "typ
-00000140: 6522 3a20 2273 7472 696e 6722 0d0a 2020  e": "string"..  
-00000150: 2020 7d2c 0d0a 2020 2020 2266 6f6f 7465    },..    "foote
-00000160: 7222 3a20 7b0d 0a20 2020 2020 2022 7479  r": {..      "ty
-00000170: 7065 223a 2022 7374 7269 6e67 222c 0d0a  pe": "string",..
-00000180: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00000190: 6f6e 223a 2022 6669 6c65 6e61 6d65 220d  on": "filename".
-000001a0: 0a20 2020 207d 2c0d 0a20 2020 2022 6672  .    },..    "fr
-000001b0: 6f6d 223a 207b 0d0a 2020 2020 2020 2274  om": {..      "t
-000001c0: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
-000001d0: 2020 2020 7d2c 0d0a 2020 2020 2268 6561      },..    "hea
-000001e0: 6465 7222 3a20 7b0d 0a20 2020 2020 2022  der": {..      "
-000001f0: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
-00000200: 0d0a 2020 2020 2020 2264 6573 6372 6970  ..      "descrip
-00000210: 7469 6f6e 223a 2022 6669 6c65 6e61 6d65  tion": "filename
-00000220: 220d 0a20 2020 207d 2c0d 0a20 2020 2022  "..    },..    "
-00000230: 6e61 6d65 223a 207b 0d0a 2020 2020 2020  name": {..      
-00000240: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00000250: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2274  ..    },..    "t
-00000260: 6162 6c65 223a 207b 0d0a 2020 2020 2020  able": {..      
-00000270: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00000280: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2274  ..    },..    "t
-00000290: 656d 706c 6174 6522 3a20 7b0d 0a20 2020  emplate": {..   
-000002a0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
-000002b0: 6e67 222c 0d0a 2020 2020 2020 2264 6573  ng",..      "des
-000002c0: 6372 6970 7469 6f6e 223a 2022 6669 6c65  cription": "file
-000002d0: 6e61 6d65 220d 0a20 2020 207d 2c0d 0a20  name"..    },.. 
-000002e0: 2020 2022 746f 223a 207b 0d0a 2020 2020     "to": {..    
-000002f0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00000300: 6722 0d0a 2020 2020 7d2c 0d0a 2020 2020  g"..    },..    
-00000310: 2274 7970 6522 3a20 7b0d 0a20 2020 2020  "type": {..     
-00000320: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-00000330: 222c 0d0a 2020 2020 2020 2265 6e75 6d22  ",..      "enum"
-00000340: 3a20 5b20 226f 6e65 2d74 6f2d 6f6e 6522  : [ "one-to-one"
-00000350: 2c20 226f 6e65 2d74 6f2d 6d61 6e79 2220  , "one-to-many" 
-00000360: 5d2c 0d0a 2020 2020 2020 2261 6464 6974  ],..      "addit
-00000370: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000380: 3a20 6661 6c73 650d 0a20 2020 207d 2c0d  : false..    },.
-00000390: 0a20 2020 2022 636f 6e6e 6563 7469 6f6e  .    "connection
-000003a0: 7479 7065 223a 207b 0d0a 2020 2020 2020  type": {..      
-000003b0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-000003c0: 2c0d 0a20 2020 2020 2022 656e 756d 223a  ,..      "enum":
-000003d0: 205b 2022 6373 7622 2c20 226d 7973 716c   [ "csv", "mysql
-000003e0: 222c 2022 706f 7374 6772 6573 716c 2220  ", "postgresql" 
-000003f0: 5d2c 0d0a 2020 2020 2020 2261 6464 6974  ],..      "addit
-00000400: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000410: 3a20 6661 6c73 650d 0a20 2020 207d 0d0a  : false..    }..
-00000420: 2020 7d0d 0a7d 0d0a                        }..}..
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2270  $": {}.  },.  "p
+00000070: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00000080: 2020 225f 5f74 7970 655f 5f22 3a20 7b0a    "__type__": {.
+00000090: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000000a0: 226a 6f69 6e22 205d 0a20 2020 207d 2c0a  "join" ].    },.
+000000b0: 2020 2020 2269 6e63 6c75 6465 223a 207b      "include": {
+000000c0: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+000000d0: 6172 7261 7922 2c0a 2020 2020 2020 2269  array",.      "i
+000000e0: 7465 6d73 223a 207b 0a20 2020 2020 2020  tems": {.       
+000000f0: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+00000100: 220a 2020 2020 2020 7d0a 2020 2020 7d2c  ".      }.    },
+00000110: 0a20 2020 2022 636f 6e6e 6563 7469 6f6e  .    "connection
+00000120: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000130: 223a 2022 7374 7269 6e67 220a 2020 2020  ": "string".    
+00000140: 7d2c 0a20 2020 2022 666f 6f74 6572 223a  },.    "footer":
+00000150: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00000160: 2022 7374 7269 6e67 222c 0a20 2020 2020   "string",.     
+00000170: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00000180: 2266 696c 656e 616d 6522 0a20 2020 207d  "filename".    }
+00000190: 2c0a 2020 2020 2266 726f 6d22 3a20 7b0a  ,.    "from": {.
+000001a0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+000001b0: 7472 696e 6722 0a20 2020 207d 2c0a 2020  tring".    },.  
+000001c0: 2020 2268 6561 6465 7222 3a20 7b0a 2020    "header": {.  
+000001d0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+000001e0: 696e 6722 2c0a 2020 2020 2020 2264 6573  ing",.      "des
+000001f0: 6372 6970 7469 6f6e 223a 2022 6669 6c65  cription": "file
+00000200: 6e61 6d65 220a 2020 2020 7d2c 0a20 2020  name".    },.   
+00000210: 2022 6e61 6d65 223a 207b 0a20 2020 2020   "name": {.     
+00000220: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+00000230: 220a 2020 2020 7d2c 0a20 2020 2022 7461  ".    },.    "ta
+00000240: 626c 6522 3a20 7b0a 2020 2020 2020 2274  ble": {.      "t
+00000250: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
+00000260: 2020 207d 2c0a 2020 2020 2274 656d 706c     },.    "templ
+00000270: 6174 6522 3a20 7b0a 2020 2020 2020 2274  ate": {.      "t
+00000280: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+00000290: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000002a0: 6f6e 223a 2022 6669 6c65 6e61 6d65 220a  on": "filename".
+000002b0: 2020 2020 7d2c 0a20 2020 2022 746f 223a      },.    "to":
+000002c0: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+000002d0: 2022 7374 7269 6e67 220a 2020 2020 7d2c   "string".    },
+000002e0: 0a20 2020 2022 7479 7065 223a 207b 0a20  .    "type": {. 
+000002f0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00000300: 7269 6e67 222c 0a20 2020 2020 2022 656e  ring",.      "en
+00000310: 756d 223a 205b 2022 6f6e 652d 746f 2d6f  um": [ "one-to-o
+00000320: 6e65 222c 2022 6f6e 652d 746f 2d6d 616e  ne", "one-to-man
+00000330: 7922 205d 2c0a 2020 2020 2020 2261 6464  y" ],.      "add
+00000340: 6974 696f 6e61 6c50 726f 7065 7274 6965  itionalPropertie
+00000350: 7322 3a20 6661 6c73 650a 2020 2020 7d2c  s": false.    },
+00000360: 0a20 2020 2022 636f 6e6e 6563 7469 6f6e  .    "connection
+00000370: 7479 7065 223a 207b 0a20 2020 2020 2022  type": {.      "
+00000380: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
+00000390: 0a20 2020 2020 2022 656e 756d 223a 205b  .      "enum": [
+000003a0: 2022 6373 7622 2c20 226d 7973 716c 222c   "csv", "mysql",
+000003b0: 2022 706f 7374 6772 6573 716c 2220 5d2c   "postgresql" ],
+000003c0: 0a20 2020 2020 2022 6164 6469 7469 6f6e  .      "addition
+000003d0: 616c 5072 6f70 6572 7469 6573 223a 2066  alProperties": f
+000003e0: 616c 7365 0a20 2020 207d 0a20 207d 0a7d  alse.    }.  }.}
+000003f0: 0a                                       .
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/label.json` & `mappyfile-1.0.2/mappyfile/schemas/label.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,505 +1,480 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2270 726f 7065 7274 6965 7322  ..  "properties"
-00000080: 3a20 7b0d 0a20 2020 2022 5f5f 7479 7065  : {..    "__type
-00000090: 5f5f 223a 207b 0d0a 2020 2020 2020 2265  __": {..      "e
-000000a0: 6e75 6d22 3a20 5b20 226c 6162 656c 2220  num": [ "label" 
-000000b0: 5d0d 0a20 2020 207d 2c0d 0a20 2020 2022  ]..    },..    "
-000000c0: 696e 636c 7564 6522 3a20 7b0d 0a20 2020  include": {..   
-000000d0: 2020 2022 7479 7065 223a 2022 6172 7261     "type": "arra
-000000e0: 7922 2c0d 0a20 2020 2020 2022 6974 656d  y",..      "item
-000000f0: 7322 3a20 7b0d 0a20 2020 2020 2020 2022  s": {..        "
-00000100: 7479 7065 223a 2022 7374 7269 6e67 220d  type": "string".
-00000110: 0a20 2020 2020 207d 0d0a 2020 2020 7d2c  .      }..    },
-00000120: 0d0a 2020 2020 2261 6c69 676e 223a 207b  ..    "align": {
-00000130: 0d0a 2020 2020 2020 226f 6e65 4f66 223a  ..      "oneOf":
-00000140: 205b 0d0a 2020 2020 2020 2020 7b0d 0a20   [..        {.. 
-00000150: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000160: 2022 7374 7269 6e67 222c 0d0a 2020 2020   "string",..    
-00000170: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
-00000180: 226c 6566 7422 2c20 2263 656e 7465 7222  "left", "center"
-00000190: 2c20 2272 6967 6874 2220 5d2c 0d0a 2020  , "right" ],..  
-000001a0: 2020 2020 2020 2020 2261 6464 6974 696f          "additio
-000001b0: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
-000001c0: 6661 6c73 650d 0a20 2020 2020 2020 207d  false..        }
-000001d0: 2c0d 0a20 2020 2020 2020 207b 0d0a 2020  ,..        {..  
-000001e0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-000001f0: 2273 7472 696e 6722 2c0d 0a20 2020 2020  "string",..     
-00000200: 2020 2020 2022 7061 7474 6572 6e22 3a20       "pattern": 
-00000210: 225e 5c5c 5b28 2e2a 3f29 5c5c 5d24 222c  "^\\[(.*?)\\]$",
-00000220: 0d0a 2020 2020 2020 2020 2020 2264 6573  ..          "des
-00000230: 6372 6970 7469 6f6e 223a 2022 6174 7472  cription": "attr
-00000240: 6962 7574 6522 0d0a 2020 2020 2020 2020  ibute"..        
-00000250: 7d0d 0a20 2020 2020 205d 2c0d 0a20 2020  }..      ],..   
-00000260: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00000270: 0d0a 2020 2020 2020 2020 226d 696e 5665  ..        "minVe
-00000280: 7273 696f 6e22 3a20 352e 340d 0a20 2020  rsion": 5.4..   
-00000290: 2020 207d 0d0a 2020 2020 7d2c 0d0a 2020     }..    },..  
-000002a0: 2020 2261 6e67 6c65 223a 207b 0d0a 2020    "angle": {..  
-000002b0: 2020 2020 2264 6566 6175 6c74 223a 2030      "default": 0
-000002c0: 2c0d 0a20 2020 2020 2022 6f6e 654f 6622  ,..      "oneOf"
-000002d0: 3a20 5b0d 0a20 2020 2020 2020 207b 0d0a  : [..        {..
-000002e0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000002f0: 3a20 2273 7472 696e 6722 2c0d 0a20 2020  : "string",..   
-00000300: 2020 2020 2020 2022 656e 756d 223a 205b         "enum": [
-00000310: 2022 6175 746f 222c 2022 6175 746f 3222   "auto", "auto2"
-00000320: 2c20 2266 6f6c 6c6f 7722 205d 2c0d 0a20  , "follow" ],.. 
-00000330: 2020 2020 2020 2020 2022 6164 6469 7469           "additi
-00000340: 6f6e 616c 5072 6f70 6572 7469 6573 223a  onalProperties":
-00000350: 2066 616c 7365 0d0a 2020 2020 2020 2020   false..        
-00000360: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000370: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000380: 2022 6e75 6d62 6572 222c 0d0a 2020 2020   "number",..    
-00000390: 2020 2020 2020 226d 696e 696d 756d 223a        "minimum":
-000003a0: 202d 3336 302c 0d0a 2020 2020 2020 2020   -360,..        
-000003b0: 2020 226d 6178 696d 756d 223a 2033 3630    "maximum": 360
-000003c0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000003d0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-000003e0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
-000003f0: 6e67 222c 0d0a 2020 2020 2020 2020 2020  ng",..          
-00000400: 2270 6174 7465 726e 223a 2022 5e5c 5c5b  "pattern": "^\\[
-00000410: 282e 2a3f 295c 5c5d 2422 2c0d 0a20 2020  (.*?)\\]$",..   
-00000420: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000430: 696f 6e22 3a20 2261 7474 7269 6275 7465  ion": "attribute
-00000440: 222c 0d0a 2020 2020 2020 2020 2020 226d  ",..          "m
-00000450: 6574 6164 6174 6122 3a20 7b0d 0a20 2020  etadata": {..   
-00000460: 2020 2020 2020 2020 2022 6d69 6e56 6572           "minVer
-00000470: 7369 6f6e 223a 2035 2e30 0d0a 2020 2020  sion": 5.0..    
-00000480: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-00000490: 207d 0d0a 2020 2020 2020 5d0d 0a20 2020   }..      ]..   
-000004a0: 207d 2c0d 0a20 2020 2022 616e 7469 616c   },..    "antial
-000004b0: 6961 7322 3a20 7b0d 0a20 2020 2020 2022  ias": {..      "
-000004c0: 7479 7065 223a 2022 626f 6f6c 6561 6e22  type": "boolean"
-000004d0: 2c0d 0a20 2020 2020 2022 6465 6661 756c  ,..      "defaul
-000004e0: 7422 3a20 6661 6c73 650d 0a20 2020 207d  t": false..    }
-000004f0: 2c0d 0a20 2020 2022 6261 636b 6772 6f75  ,..    "backgrou
-00000500: 6e64 636f 6c6f 7222 3a20 7b0d 0a20 2020  ndcolor": {..   
-00000510: 2020 2022 616c 6c4f 6622 3a20 5b0d 0a20     "allOf": [.. 
-00000520: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00000530: 2020 2020 2224 7265 6622 3a20 2263 6f6c      "$ref": "col
-00000540: 6f72 2e6a 736f 6e22 0d0a 2020 2020 2020  or.json"..      
-00000550: 2020 7d0d 0a20 2020 2020 205d 2c0d 0a20    }..      ],.. 
-00000560: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
-00000570: 207b 0d0a 2020 2020 2020 2020 226d 6178   {..        "max
-00000580: 5665 7273 696f 6e22 3a20 362e 300d 0a20  Version": 6.0.. 
-00000590: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-000005a0: 2020 2020 2262 6163 6b67 726f 756e 6473      "backgrounds
-000005b0: 6861 646f 7763 6f6c 6f72 223a 207b 0d0a  hadowcolor": {..
-000005c0: 2020 2020 2020 2261 6c6c 4f66 223a 205b        "allOf": [
-000005d0: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-000005e0: 2020 2020 2020 2022 2472 6566 223a 2022         "$ref": "
-000005f0: 636f 6c6f 722e 6a73 6f6e 220d 0a20 2020  color.json"..   
-00000600: 2020 2020 207d 0d0a 2020 2020 2020 5d2c       }..      ],
-00000610: 0d0a 2020 2020 2020 226d 6574 6164 6174  ..      "metadat
-00000620: 6122 3a20 7b0d 0a20 2020 2020 2020 2022  a": {..        "
-00000630: 6d61 7856 6572 7369 6f6e 223a 2036 2e30  maxVersion": 6.0
-00000640: 0d0a 2020 2020 2020 7d0d 0a20 2020 207d  ..      }..    }
-00000650: 2c0d 0a20 2020 2022 6261 636b 6772 6f75  ,..    "backgrou
-00000660: 6e64 7368 6164 6f77 7369 7a65 223a 207b  ndshadowsize": {
-00000670: 0d0a 2020 2020 2020 2264 6566 6175 6c74  ..      "default
-00000680: 223a 2066 616c 7365 2c0d 0a20 2020 2020  ": false,..     
-00000690: 2022 616c 6c4f 6622 3a20 5b0d 0a20 2020   "allOf": [..   
-000006a0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-000006b0: 2020 2224 7265 6622 3a20 2270 6f69 6e74    "$ref": "point
-000006c0: 732e 6a73 6f6e 220d 0a20 2020 2020 2020  s.json"..       
-000006d0: 207d 0d0a 2020 2020 2020 5d2c 0d0a 2020   }..      ],..  
-000006e0: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-000006f0: 7b0d 0a20 2020 2020 2020 2022 6d61 7856  {..        "maxV
-00000700: 6572 7369 6f6e 223a 2036 2e30 0d0a 2020  ersion": 6.0..  
-00000710: 2020 2020 7d0d 0a20 2020 207d 2c0d 0a20      }..    },.. 
-00000720: 2020 2022 6275 6666 6572 223a 207b 0d0a     "buffer": {..
-00000730: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
-00000740: 6e74 6567 6572 222c 0d0a 2020 2020 2020  nteger",..      
-00000750: 2264 6566 6175 6c74 223a 2030 0d0a 2020  "default": 0..  
-00000760: 2020 7d2c 0d0a 2020 2020 2263 6f6c 6f72    },..    "color
-00000770: 223a 207b 0d0a 2020 2020 2020 226f 6e65  ": {..      "one
-00000780: 4f66 223a 205b 0d0a 2020 2020 2020 2020  Of": [..        
-00000790: 7b20 2224 7265 6622 3a20 2263 6f6c 6f72  { "$ref": "color
-000007a0: 2e6a 736f 6e22 207d 2c0d 0a20 2020 2020  .json" },..     
-000007b0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000007c0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-000007d0: 2c0d 0a20 2020 2020 2020 2020 2022 7061  ,..          "pa
-000007e0: 7474 6572 6e22 3a20 225e 5c5c 5b28 2e2a  ttern": "^\\[(.*
-000007f0: 3f29 5c5c 5d24 222c 0d0a 2020 2020 2020  ?)\\]$",..      
-00000800: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000810: 223a 2022 6174 7472 6962 7574 6522 2c0d  ": "attribute",.
-00000820: 0a20 2020 2020 2020 2020 2022 6d65 7461  .          "meta
-00000830: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000840: 2020 2020 2020 226d 696e 5665 7273 696f        "minVersio
-00000850: 6e22 3a20 352e 300d 0a20 2020 2020 2020  n": 5.0..       
-00000860: 2020 207d 0d0a 2020 2020 2020 2020 7d0d     }..        }.
-00000870: 0a20 2020 2020 205d 0d0a 2020 2020 7d2c  .      ]..    },
-00000880: 0d0a 2020 2020 2265 6e63 6f64 696e 6722  ..    "encoding"
-00000890: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-000008a0: 223a 2022 7374 7269 6e67 222c 0d0a 2020  ": "string",..  
-000008b0: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-000008c0: 7b0d 0a20 2020 2020 2020 2022 6d61 7856  {..        "maxV
-000008d0: 6572 7369 6f6e 223a 2037 2e36 0d0a 2020  ersion": 7.6..  
-000008e0: 2020 2020 7d0d 0a20 2020 207d 2c0d 0a20      }..    },.. 
-000008f0: 2020 2022 6578 7072 6573 7369 6f6e 223a     "expression":
-00000900: 207b 0d0a 2020 2020 2020 2261 6c6c 4f66   {..      "allOf
-00000910: 223a 205b 0d0a 2020 2020 2020 2020 7b0d  ": [..        {.
-00000920: 0a20 2020 2020 2020 2020 2022 2472 6566  .          "$ref
-00000930: 223a 2022 6578 7072 6573 7369 6f6e 2e6a  ": "expression.j
-00000940: 736f 6e22 0d0a 2020 2020 2020 2020 7d0d  son"..        }.
-00000950: 0a20 2020 2020 205d 2c0d 0a20 2020 2020  .      ],..     
-00000960: 2022 6d65 7461 6461 7461 223a 207b 0d0a   "metadata": {..
-00000970: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
-00000980: 696f 6e22 3a20 362e 320d 0a20 2020 2020  ion": 6.2..     
-00000990: 207d 0d0a 2020 2020 7d2c 0d0a 2020 2020   }..    },..    
-000009a0: 2266 6f6e 7422 3a20 7b0d 0a20 2020 2020  "font": {..     
-000009b0: 2022 616e 794f 6622 3a20 5b0d 0a20 2020   "anyOf": [..   
-000009c0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-000009d0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-000009e0: 6722 2c0d 0a20 2020 2020 2020 2020 2022  g",..          "
-000009f0: 7061 7474 6572 6e22 3a20 225e 5c5c 5b28  pattern": "^\\[(
-00000a00: 2e2a 3f29 5c5c 5d24 222c 0d0a 2020 2020  .*?)\\]$",..    
-00000a10: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00000a20: 6f6e 223a 2022 6174 7472 6962 7574 6522  on": "attribute"
-00000a30: 2c0d 0a20 2020 2020 2020 2020 2022 6d65  ,..          "me
-00000a40: 7461 6461 7461 223a 207b 0d0a 2020 2020  tadata": {..    
-00000a50: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
-00000a60: 696f 6e22 3a20 352e 360d 0a20 2020 2020  ion": 5.6..     
-00000a70: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000a80: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-00000a90: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000aa0: 2022 7374 7269 6e67 220d 0a20 2020 2020   "string"..     
-00000ab0: 2020 207d 0d0a 2020 2020 2020 5d0d 0a20     }..      ].. 
-00000ac0: 2020 207d 2c0d 0a20 2020 2022 666f 7263     },..    "forc
-00000ad0: 6522 3a20 7b0d 0a20 2020 2020 2022 6465  e": {..      "de
-00000ae0: 6661 756c 7422 3a20 6661 6c73 652c 0d0a  fault": false,..
-00000af0: 2020 2020 2020 226f 6e65 4f66 223a 205b        "oneOf": [
-00000b00: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00000b10: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000b20: 626f 6f6c 6561 6e22 0d0a 2020 2020 2020  boolean"..      
-00000b30: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-00000b40: 0a20 2020 2020 2020 2020 2022 656e 756d  .          "enum
-00000b50: 223a 205b 2022 6772 6f75 7022 205d 2c0d  ": [ "group" ],.
-00000b60: 0a20 2020 2020 2020 2020 2022 6d65 7461  .          "meta
-00000b70: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000b80: 2020 2020 2020 226d 696e 5665 7273 696f        "minVersio
-00000b90: 6e22 3a20 362e 320d 0a20 2020 2020 2020  n": 6.2..       
-00000ba0: 2020 207d 0d0a 2020 2020 2020 2020 7d0d     }..        }.
-00000bb0: 0a20 2020 2020 205d 0d0a 2020 2020 7d2c  .      ]..    },
-00000bc0: 0d0a 2020 2020 226d 6178 6c65 6e67 7468  ..    "maxlength
-00000bd0: 223a 207b 0d0a 2020 2020 2020 2274 7970  ": {..      "typ
-00000be0: 6522 3a20 2269 6e74 6567 6572 222c 0d0a  e": "integer",..
-00000bf0: 2020 2020 2020 2265 7863 6c75 7369 7665        "exclusive
-00000c00: 4d69 6e69 6d75 6d22 3a20 302c 0d0a 2020  Minimum": 0,..  
-00000c10: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-00000c20: 7b0d 0a20 2020 2020 2020 2022 6d69 6e56  {..        "minV
-00000c30: 6572 7369 6f6e 223a 2035 2e34 0d0a 2020  ersion": 5.4..  
-00000c40: 2020 2020 7d0d 0a20 2020 207d 2c0d 0a20      }..    },.. 
-00000c50: 2020 2022 6d61 786f 7665 726c 6170 616e     "maxoverlapan
-00000c60: 676c 6522 3a20 7b0d 0a20 2020 2020 2022  gle": {..      "
-00000c70: 6465 6661 756c 7422 3a20 3232 2e35 2c0d  default": 22.5,.
-00000c80: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-00000c90: 6e75 6d62 6572 222c 0d0a 2020 2020 2020  number",..      
-00000ca0: 226d 696e 696d 756d 223a 2030 2c0d 0a20  "minimum": 0,.. 
-00000cb0: 2020 2020 2022 6d61 7869 6d75 6d22 3a20       "maximum": 
-00000cc0: 3336 302c 0d0a 2020 2020 2020 226d 6574  360,..      "met
-00000cd0: 6164 6174 6122 3a20 7b0d 0a20 2020 2020  adata": {..     
-00000ce0: 2020 2022 6d69 6e56 6572 7369 6f6e 223a     "minVersion":
-00000cf0: 2036 2e30 0d0a 2020 2020 2020 7d0d 0a20   6.0..      }.. 
-00000d00: 2020 207d 2c0d 0a20 2020 2022 6d61 7873     },..    "maxs
-00000d10: 6361 6c65 6465 6e6f 6d22 3a20 7b0d 0a20  caledenom": {.. 
-00000d20: 2020 2020 2022 7479 7065 223a 2022 6e75       "type": "nu
-00000d30: 6d62 6572 222c 0d0a 2020 2020 2020 226d  mber",..      "m
-00000d40: 696e 696d 756d 223a 2030 2c0d 0a20 2020  inimum": 0,..   
-00000d50: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00000d60: 0d0a 2020 2020 2020 2020 226d 696e 5665  ..        "minVe
-00000d70: 7273 696f 6e22 3a20 352e 340d 0a20 2020  rsion": 5.4..   
-00000d80: 2020 207d 0d0a 2020 2020 7d2c 0d0a 2020     }..    },..  
-00000d90: 2020 226d 6178 7369 7a65 223a 207b 0d0a    "maxsize": {..
-00000da0: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
-00000db0: 6e74 6567 6572 222c 0d0a 2020 2020 2020  nteger",..      
-00000dc0: 2264 6566 6175 6c74 223a 2032 3536 2c0d  "default": 256,.
-00000dd0: 0a20 2020 2020 2022 6578 636c 7573 6976  .      "exclusiv
-00000de0: 654d 696e 696d 756d 223a 2030 0d0a 2020  eMinimum": 0..  
-00000df0: 2020 7d2c 0d0a 2020 2020 226d 696e 6469    },..    "mindi
-00000e00: 7374 616e 6365 223a 207b 0d0a 2020 2020  stance": {..    
-00000e10: 2020 2274 7970 6522 3a20 2269 6e74 6567    "type": "integ
-00000e20: 6572 222c 0d0a 2020 2020 2020 2265 7863  er",..      "exc
-00000e30: 6c75 7369 7665 4d69 6e69 6d75 6d22 3a20  lusiveMinimum": 
-00000e40: 300d 0a20 2020 207d 2c0d 0a20 2020 2022  0..    },..    "
-00000e50: 6d69 6e66 6561 7475 7265 7369 7a65 223a  minfeaturesize":
-00000e60: 207b 0d0a 2020 2020 2020 226f 6e65 4f66   {..      "oneOf
-00000e70: 223a 205b 0d0a 2020 2020 2020 2020 7b20  ": [..        { 
-00000e80: 2265 6e75 6d22 3a20 5b20 2261 7574 6f22  "enum": [ "auto"
-00000e90: 205d 207d 2c0d 0a20 2020 2020 2020 207b   ] },..        {
-00000ea0: 0d0a 2020 2020 2020 2020 2020 2274 7970  ..          "typ
-00000eb0: 6522 3a20 2269 6e74 6567 6572 222c 0d0a  e": "integer",..
-00000ec0: 2020 2020 2020 2020 2020 2265 7863 6c75            "exclu
-00000ed0: 7369 7665 4d69 6e69 6d75 6d22 3a20 300d  siveMinimum": 0.
-00000ee0: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-00000ef0: 2020 5d0d 0a20 2020 207d 2c0d 0a20 2020    ]..    },..   
-00000f00: 2022 6d69 6e73 6361 6c65 6465 6e6f 6d22   "minscaledenom"
-00000f10: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000f20: 223a 2022 6e75 6d62 6572 222c 0d0a 2020  ": "number",..  
-00000f30: 2020 2020 226d 696e 696d 756d 223a 2030      "minimum": 0
-00000f40: 2c0d 0a20 2020 2020 2022 6d65 7461 6461  ,..      "metada
-00000f50: 7461 223a 207b 0d0a 2020 2020 2020 2020  ta": {..        
-00000f60: 226d 696e 5665 7273 696f 6e22 3a20 352e  "minVersion": 5.
-00000f70: 340d 0a20 2020 2020 207d 0d0a 2020 2020  4..      }..    
-00000f80: 7d2c 0d0a 2020 2020 226d 696e 7369 7a65  },..    "minsize
-00000f90: 223a 207b 0d0a 2020 2020 2020 2274 7970  ": {..      "typ
-00000fa0: 6522 3a20 2269 6e74 6567 6572 222c 0d0a  e": "integer",..
-00000fb0: 2020 2020 2020 2265 7863 6c75 7369 7665        "exclusive
-00000fc0: 4d69 6e69 6d75 6d22 3a20 302c 0d0a 2020  Minimum": 0,..  
-00000fd0: 2020 2020 2264 6566 6175 6c74 223a 2034      "default": 4
-00000fe0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 226f  ..    },..    "o
-00000ff0: 6666 7365 7422 3a20 7b0d 0a20 2020 2020  ffset": {..     
-00001000: 2022 6465 6661 756c 7422 3a20 5b20 302c   "default": [ 0,
-00001010: 2030 205d 2c0d 0a20 2020 2020 2022 6f6e   0 ],..      "on
-00001020: 654f 6622 3a20 5b0d 0a20 2020 2020 2020  eOf": [..       
-00001030: 207b 0d0a 2020 2020 2020 2020 2020 2274   {..          "t
-00001040: 7970 6522 3a20 2261 7272 6179 222c 0d0a  ype": "array",..
-00001050: 2020 2020 2020 2020 2020 2269 7465 6d73            "items
-00001060: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00001070: 2020 2274 7970 6522 3a20 226e 756d 6265    "type": "numbe
-00001080: 7222 0d0a 2020 2020 2020 2020 2020 7d2c  r"..          },
-00001090: 0d0a 2020 2020 2020 2020 2020 226d 696e  ..          "min
-000010a0: 4974 656d 7322 3a20 322c 0d0a 2020 2020  Items": 2,..    
-000010b0: 2020 2020 2020 226d 6178 4974 656d 7322        "maxItems"
-000010c0: 3a20 320d 0a20 2020 2020 2020 207d 2c0d  : 2..        },.
-000010d0: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
-000010e0: 2020 2020 2020 2274 7970 6522 3a20 2261        "type": "a
-000010f0: 7272 6179 222c 0d0a 2020 2020 2020 2020  rray",..        
-00001100: 2020 2269 7465 6d73 223a 207b 0d0a 2020    "items": {..  
-00001110: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001120: 3a20 2273 7472 696e 6722 2c0d 0a20 2020  : "string",..   
-00001130: 2020 2020 2020 2020 2022 7061 7474 6572           "patter
-00001140: 6e22 3a20 225e 5c5c 5b28 2e2a 3f29 5c5c  n": "^\\[(.*?)\\
-00001150: 5d24 222c 0d0a 2020 2020 2020 2020 2020  ]$",..          
-00001160: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00001170: 2022 6174 7472 6962 7574 6522 0d0a 2020   "attribute"..  
-00001180: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00001190: 2020 2020 2020 226d 696e 4974 656d 7322        "minItems"
-000011a0: 3a20 322c 0d0a 2020 2020 2020 2020 2020  : 2,..          
-000011b0: 226d 6178 4974 656d 7322 3a20 322c 0d0a  "maxItems": 2,..
-000011c0: 2020 2020 2020 2020 2020 226d 6574 6164            "metad
-000011d0: 6174 6122 3a20 7b0d 0a20 2020 2020 2020  ata": {..       
-000011e0: 2020 2020 2022 6d69 6e56 6572 7369 6f6e       "minVersion
-000011f0: 223a 2037 2e36 0d0a 2020 2020 2020 2020  ": 7.6..        
-00001200: 2020 7d0d 0a20 2020 2020 2020 207d 0d0a    }..        }..
-00001210: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
-00001220: 0a20 2020 2022 6f75 746c 696e 6563 6f6c  .    "outlinecol
-00001230: 6f72 223a 207b 0d0a 2020 2020 2020 226f  or": {..      "o
-00001240: 6e65 4f66 223a 205b 0d0a 2020 2020 2020  neOf": [..      
-00001250: 2020 7b20 2224 7265 6622 3a20 2263 6f6c    { "$ref": "col
-00001260: 6f72 2e6a 736f 6e22 207d 2c0d 0a20 2020  or.json" },..   
-00001270: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00001280: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00001290: 6722 2c0d 0a20 2020 2020 2020 2020 2022  g",..          "
-000012a0: 7061 7474 6572 6e22 3a20 225e 5c5c 5b28  pattern": "^\\[(
-000012b0: 2e2a 3f29 5c5c 5d24 222c 0d0a 2020 2020  .*?)\\]$",..    
-000012c0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000012d0: 6f6e 223a 2022 6174 7472 6962 7574 6522  on": "attribute"
-000012e0: 2c0d 0a20 2020 2020 2020 2020 2022 6d65  ,..          "me
-000012f0: 7461 6461 7461 223a 207b 0d0a 2020 2020  tadata": {..    
-00001300: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
-00001310: 696f 6e22 3a20 352e 300d 0a20 2020 2020  ion": 5.0..     
-00001320: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00001330: 7d0d 0a20 2020 2020 205d 0d0a 2020 2020  }..      ]..    
-00001340: 7d2c 0d0a 2020 2020 226f 7574 6c69 6e65  },..    "outline
-00001350: 7769 6474 6822 3a20 7b0d 0a20 2020 2020  width": {..     
-00001360: 2022 7479 7065 223a 2022 696e 7465 6765   "type": "intege
-00001370: 7222 2c0d 0a20 2020 2020 2022 6578 636c  r",..      "excl
-00001380: 7573 6976 654d 696e 696d 756d 223a 2030  usiveMinimum": 0
-00001390: 2c0d 0a20 2020 2020 2022 6465 6661 756c  ,..      "defaul
-000013a0: 7422 3a20 310d 0a20 2020 207d 2c0d 0a20  t": 1..    },.. 
-000013b0: 2020 2022 7061 7274 6961 6c73 223a 207b     "partials": {
-000013c0: 0d0a 2020 2020 2020 2274 7970 6522 3a20  ..      "type": 
-000013d0: 2262 6f6f 6c65 616e 222c 0d0a 2020 2020  "boolean",..    
-000013e0: 2020 2264 6566 6175 6c74 223a 2066 616c    "default": fal
-000013f0: 7365 0d0a 2020 2020 7d2c 0d0a 2020 2020  se..    },..    
-00001400: 2270 6f73 6974 696f 6e22 3a20 7b0d 0a20  "position": {.. 
-00001410: 2020 2020 2022 6465 6661 756c 7422 3a20       "default": 
-00001420: 2263 6322 2c0d 0a20 2020 2020 2022 6f6e  "cc",..      "on
-00001430: 654f 6622 3a20 5b0d 0a20 2020 2020 2020  eOf": [..       
-00001440: 207b 2022 656e 756d 223a 205b 2022 6175   { "enum": [ "au
-00001450: 746f 2220 5d20 7d2c 0d0a 2020 2020 2020  to" ] },..      
-00001460: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
-00001470: 2472 6566 223a 2022 706f 7369 7469 6f6e  $ref": "position
-00001480: 2e6a 736f 6e22 0d0a 2020 2020 2020 2020  .json"..        
-00001490: 7d2c 0d0a 2020 2020 2020 2020 7b0d 0a20  },..        {.. 
-000014a0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000014b0: 2022 7374 7269 6e67 222c 0d0a 2020 2020   "string",..    
-000014c0: 2020 2020 2020 2270 6174 7465 726e 223a        "pattern":
-000014d0: 2022 5e5c 5c5b 282e 2a3f 295c 5c5d 2422   "^\\[(.*?)\\]$"
-000014e0: 2c0d 0a20 2020 2020 2020 2020 2022 6465  ,..          "de
-000014f0: 7363 7269 7074 696f 6e22 3a20 2261 7474  scription": "att
-00001500: 7269 6275 7465 220d 0a20 2020 2020 2020  ribute"..       
-00001510: 207d 0d0a 2020 2020 2020 5d0d 0a20 2020   }..      ]..   
-00001520: 207d 2c0d 0a20 2020 2022 7072 696f 7269   },..    "priori
-00001530: 7479 223a 207b 0d0a 2020 2020 2020 2264  ty": {..      "d
-00001540: 6566 6175 6c74 223a 2031 2c0d 0a20 2020  efault": 1,..   
-00001550: 2020 2022 6d69 6e69 6d75 6d22 3a20 312c     "minimum": 1,
-00001560: 0d0a 2020 2020 2020 226d 6178 696d 756d  ..      "maximum
-00001570: 223a 2031 302c 0d0a 2020 2020 2020 2261  ": 10,..      "a
-00001580: 6e79 4f66 223a 205b 0d0a 2020 2020 2020  nyOf": [..      
-00001590: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
-000015a0: 7479 7065 223a 2022 696e 7465 6765 7222  type": "integer"
-000015b0: 0d0a 2020 2020 2020 2020 7d2c 0d0a 2020  ..        },..  
-000015c0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-000015d0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
-000015e0: 6e67 222c 0d0a 2020 2020 2020 2020 2020  ng",..          
-000015f0: 2270 6174 7465 726e 223a 2022 5e5c 5c5b  "pattern": "^\\[
-00001600: 282e 2a3f 295c 5c5d 2422 2c0d 0a20 2020  (.*?)\\]$",..   
-00001610: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00001620: 696f 6e22 3a20 2261 7474 7269 6275 7465  ion": "attribute
-00001630: 220d 0a20 2020 2020 2020 207d 2c0d 0a20  "..        },.. 
-00001640: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00001650: 2020 2020 2261 6c6c 4f66 223a 205b 0d0a      "allOf": [..
-00001660: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00001670: 2020 2020 2020 2020 2020 2020 2022 2472               "$r
-00001680: 6566 223a 2022 6578 7072 6573 7369 6f6e  ef": "expression
-00001690: 2e6a 736f 6e22 0d0a 2020 2020 2020 2020  .json"..        
-000016a0: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
-000016b0: 205d 2c0d 0a20 2020 2020 2020 2020 2022   ],..          "
-000016c0: 6d65 7461 6461 7461 223a 207b 0d0a 2020  metadata": {..  
-000016d0: 2020 2020 2020 2020 2020 226d 696e 5665            "minVe
-000016e0: 7273 696f 6e22 3a20 382e 320d 0a20 2020  rsion": 8.2..   
-000016f0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00001700: 2020 7d0d 0a20 2020 2020 205d 2c0d 0a20    }..      ],.. 
-00001710: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
-00001720: 207b 0d0a 2020 2020 2020 2020 226d 696e   {..        "min
-00001730: 5665 7273 696f 6e22 3a20 352e 300d 0a20  Version": 5.0.. 
-00001740: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-00001750: 2020 2020 2272 6570 6561 7464 6973 7461      "repeatdista
-00001760: 6e63 6522 3a20 7b0d 0a20 2020 2020 2022  nce": {..      "
-00001770: 7479 7065 223a 2022 696e 7465 6765 7222  type": "integer"
-00001780: 2c0d 0a20 2020 2020 2022 6465 6661 756c  ,..      "defaul
-00001790: 7422 3a20 302c 0d0a 2020 2020 2020 2265  t": 0,..      "e
-000017a0: 7863 6c75 7369 7665 4d69 6e69 6d75 6d22  xclusiveMinimum"
-000017b0: 3a20 302c 0d0a 2020 2020 2020 226d 6574  : 0,..      "met
-000017c0: 6164 6174 6122 3a20 7b0d 0a20 2020 2020  adata": {..     
-000017d0: 2020 2022 6d69 6e56 6572 7369 6f6e 223a     "minVersion":
-000017e0: 2035 2e36 0d0a 2020 2020 2020 7d0d 0a20   5.6..      }.. 
-000017f0: 2020 207d 2c0d 0a20 2020 2022 7368 6164     },..    "shad
-00001800: 6f77 636f 6c6f 7222 3a20 7b0d 0a20 2020  owcolor": {..   
-00001810: 2020 2022 2472 6566 223a 2022 636f 6c6f     "$ref": "colo
-00001820: 722e 6a73 6f6e 220d 0a20 2020 207d 2c0d  r.json"..    },.
-00001830: 0a20 2020 2022 7368 6164 6f77 7369 7a65  .    "shadowsize
-00001840: 223a 207b 0d0a 2020 2020 2020 2264 6566  ": {..      "def
-00001850: 6175 6c74 223a 205b 2031 2c20 3120 5d2c  ault": [ 1, 1 ],
-00001860: 0d0a 2020 2020 2020 226f 6e65 4f66 223a  ..      "oneOf":
-00001870: 205b 0d0a 2020 2020 2020 2020 7b0d 0a20   [..        {.. 
-00001880: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00001890: 2022 6172 7261 7922 2c0d 0a20 2020 2020   "array",..     
-000018a0: 2020 2020 2022 6974 656d 7322 3a20 7b0d       "items": {.
-000018b0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-000018c0: 7065 223a 2022 696e 7465 6765 7222 0d0a  pe": "integer"..
-000018d0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
-000018e0: 2020 2020 2020 2020 226d 696e 4974 656d          "minItem
-000018f0: 7322 3a20 322c 0d0a 2020 2020 2020 2020  s": 2,..        
-00001900: 2020 226d 6178 4974 656d 7322 3a20 320d    "maxItems": 2.
-00001910: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00001920: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-00001930: 2020 2274 7970 6522 3a20 2261 7272 6179    "type": "array
-00001940: 222c 0d0a 2020 2020 2020 2020 2020 2269  ",..          "i
-00001950: 7465 6d73 223a 205b 0d0a 2020 2020 2020  tems": [..      
-00001960: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00001970: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00001980: 696e 7465 6765 7222 0d0a 2020 2020 2020  integer"..      
-00001990: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-000019a0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-000019b0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000019c0: 7374 7269 6e67 222c 0d0a 2020 2020 2020  string",..      
-000019d0: 2020 2020 2020 2020 2270 6174 7465 726e          "pattern
-000019e0: 223a 2022 5e5c 5c5b 282e 2a3f 295c 5c5d  ": "^\\[(.*?)\\]
-000019f0: 2422 2c0d 0a20 2020 2020 2020 2020 2020  $",..           
-00001a00: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00001a10: 3a20 2261 7474 7269 6275 7465 220d 0a20  : "attribute".. 
-00001a20: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00001a30: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00001a40: 2020 2020 2020 226d 696e 4974 656d 7322        "minItems"
-00001a50: 3a20 322c 0d0a 2020 2020 2020 2020 2020  : 2,..          
-00001a60: 226d 6178 4974 656d 7322 3a20 322c 0d0a  "maxItems": 2,..
-00001a70: 2020 2020 2020 2020 2020 226d 6574 6164            "metad
-00001a80: 6174 6122 3a20 7b0d 0a20 2020 2020 2020  ata": {..       
-00001a90: 2020 2020 2022 6d69 6e56 6572 7369 6f6e       "minVersion
-00001aa0: 223a 2036 2e30 0d0a 2020 2020 2020 2020  ": 6.0..        
-00001ab0: 2020 7d0d 0a20 2020 2020 2020 207d 0d0a    }..        }..
-00001ac0: 2020 2020 2020 5d0d 0a20 2020 207d 2c0d        ]..    },.
-00001ad0: 0a20 2020 2022 7369 7a65 223a 207b 0d0a  .    "size": {..
-00001ae0: 2020 2020 2020 2264 6566 6175 6c74 223a        "default":
-00001af0: 2031 302c 0d0a 2020 2020 2020 2265 7863   10,..      "exc
-00001b00: 6c75 7369 7665 4d69 6e69 6d75 6d22 3a20  lusiveMinimum": 
-00001b10: 312c 0d0a 2020 2020 2020 2261 6e79 4f66  1,..      "anyOf
-00001b20: 223a 205b 0d0a 2020 2020 2020 2020 7b0d  ": [..        {.
-00001b30: 0a20 2020 2020 2020 2020 2022 7479 7065  .          "type
-00001b40: 223a 2022 696e 7465 6765 7222 0d0a 2020  ": "integer"..  
-00001b50: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
-00001b60: 2020 7b0d 0a20 2020 2020 2020 2020 2022    {..          "
-00001b70: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
-00001b80: 0d0a 2020 2020 2020 2020 2020 2265 6e75  ..          "enu
-00001b90: 6d22 3a20 5b20 2274 696e 7922 2c20 2273  m": [ "tiny", "s
-00001ba0: 6d61 6c6c 222c 2022 6d65 6469 756d 222c  mall", "medium",
-00001bb0: 2022 6c61 7267 6522 2c20 2267 6961 6e74   "large", "giant
-00001bc0: 2220 5d2c 0d0a 2020 2020 2020 2020 2020  " ],..          
-00001bd0: 2261 6464 6974 696f 6e61 6c50 726f 7065  "additionalPrope
-00001be0: 7274 6965 7322 3a20 6661 6c73 650d 0a20  rties": false.. 
-00001bf0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00001c00: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00001c10: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00001c20: 2c0d 0a20 2020 2020 2020 2020 2022 7061  ,..          "pa
-00001c30: 7474 6572 6e22 3a20 225e 5c5c 5b28 2e2a  ttern": "^\\[(.*
-00001c40: 3f29 5c5c 5d24 222c 0d0a 2020 2020 2020  ?)\\]$",..      
-00001c50: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00001c60: 223a 2022 6174 7472 6962 7574 6522 2c0d  ": "attribute",.
-00001c70: 0a20 2020 2020 2020 2020 2022 6d65 7461  .          "meta
-00001c80: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00001c90: 2020 2020 2020 226d 696e 5665 7273 696f        "minVersio
-00001ca0: 6e22 3a20 352e 300d 0a20 2020 2020 2020  n": 5.0..       
-00001cb0: 2020 207d 0d0a 2020 2020 2020 2020 7d2c     }..        },
-00001cc0: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00001cd0: 2020 2020 2020 2022 616c 6c4f 6622 3a20         "allOf": 
-00001ce0: 5b0d 0a20 2020 2020 2020 2020 2020 207b  [..            {
-00001cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001d00: 2224 7265 6622 3a20 2265 7870 7265 7373  "$ref": "express
-00001d10: 696f 6e2e 6a73 6f6e 220d 0a20 2020 2020  ion.json"..     
-00001d20: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00001d30: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
-00001d40: 2020 226d 6574 6164 6174 6122 3a20 7b0d    "metadata": {.
-00001d50: 0a20 2020 2020 2020 2020 2020 2022 6d69  .            "mi
-00001d60: 6e56 6572 7369 6f6e 223a 2037 2e36 0d0a  nVersion": 7.6..
-00001d70: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00001d80: 2020 2020 207d 0d0a 2020 2020 2020 5d0d       }..      ].
-00001d90: 0a20 2020 207d 2c0d 0a20 2020 2022 7374  .    },..    "st
-00001da0: 796c 6573 223a 207b 0d0a 2020 2020 2020  yles": {..      
-00001db0: 2274 7970 6522 3a20 2261 7272 6179 222c  "type": "array",
-00001dc0: 0d0a 2020 2020 2020 2269 7465 6d73 223a  ..      "items":
-00001dd0: 207b 0d0a 2020 2020 2020 2020 2224 7265   {..        "$re
-00001de0: 6622 3a20 2273 7479 6c65 2e6a 736f 6e22  f": "style.json"
-00001df0: 0d0a 2020 2020 2020 7d0d 0a20 2020 207d  ..      }..    }
-00001e00: 2c0d 0a20 2020 2022 7465 7874 223a 207b  ,..    "text": {
-00001e10: 0d0a 2020 2020 2020 226f 6e65 4f66 223a  ..      "oneOf":
-00001e20: 205b 0d0a 2020 2020 2020 2020 7b0d 0a20   [..        {.. 
-00001e30: 2020 2020 2020 2020 2022 2472 6566 223a           "$ref":
-00001e40: 2022 6578 7072 6573 7369 6f6e 2e6a 736f   "expression.jso
-00001e50: 6e22 0d0a 2020 2020 2020 2020 7d0d 0a20  n"..        }.. 
-00001e60: 2020 2020 205d 2c0d 0a20 2020 2020 2022       ],..      "
-00001e70: 6d65 7461 6461 7461 223a 207b 0d0a 2020  metadata": {..  
-00001e80: 2020 2020 2020 226d 696e 5665 7273 696f        "minVersio
-00001e90: 6e22 3a20 362e 320d 0a20 2020 2020 207d  n": 6.2..      }
-00001ea0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2274  ..    },..    "t
-00001eb0: 7970 6522 3a20 7b0d 0a20 2020 2020 2022  ype": {..      "
-00001ec0: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
-00001ed0: 0d0a 2020 2020 2020 2265 6e75 6d22 3a20  ..      "enum": 
-00001ee0: 5b20 2262 6974 6d61 7022 2c20 2274 7275  [ "bitmap", "tru
-00001ef0: 6574 7970 6522 205d 2c0d 0a20 2020 2020  etype" ],..     
-00001f00: 2022 6164 6469 7469 6f6e 616c 5072 6f70   "additionalProp
-00001f10: 6572 7469 6573 223a 2066 616c 7365 0d0a  erties": false..
-00001f20: 2020 2020 7d2c 0d0a 2020 2020 2277 7261      },..    "wra
-00001f30: 7022 3a20 7b0d 0a20 2020 2020 2022 7479  p": {..      "ty
-00001f40: 7065 223a 2022 7374 7269 6e67 222c 0d0a  pe": "string",..
-00001f50: 2020 2020 2020 226d 696e 4c65 6e67 7468        "minLength
-00001f60: 223a 2031 2c0d 0a20 2020 2020 2022 6d61  ": 1,..      "ma
-00001f70: 784c 656e 6774 6822 3a20 310d 0a20 2020  xLength": 1..   
-00001f80: 207d 0d0a 2020 7d0d 0a7d 0d0a             }..  }..}..
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2270  $": {}.  },.  "p
+00000070: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00000080: 2020 225f 5f74 7970 655f 5f22 3a20 7b0a    "__type__": {.
+00000090: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000000a0: 226c 6162 656c 2220 5d0a 2020 2020 7d2c  "label" ].    },
+000000b0: 0a20 2020 2022 696e 636c 7564 6522 3a20  .    "include": 
+000000c0: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+000000d0: 2261 7272 6179 222c 0a20 2020 2020 2022  "array",.      "
+000000e0: 6974 656d 7322 3a20 7b0a 2020 2020 2020  items": {.      
+000000f0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00000100: 6722 0a20 2020 2020 207d 0a20 2020 207d  g".      }.    }
+00000110: 2c0a 2020 2020 2261 6c69 676e 223a 207b  ,.    "align": {
+00000120: 0a20 2020 2020 2022 6f6e 654f 6622 3a20  .      "oneOf": 
+00000130: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+00000140: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+00000150: 7472 696e 6722 2c0a 2020 2020 2020 2020  tring",.        
+00000160: 2020 2265 6e75 6d22 3a20 5b20 226c 6566    "enum": [ "lef
+00000170: 7422 2c20 2263 656e 7465 7222 2c20 2272  t", "center", "r
+00000180: 6967 6874 2220 5d2c 0a20 2020 2020 2020  ight" ],.       
+00000190: 2020 2022 6164 6469 7469 6f6e 616c 5072     "additionalPr
+000001a0: 6f70 6572 7469 6573 223a 2066 616c 7365  operties": false
+000001b0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000001c0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000001d0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+000001e0: 2c0a 2020 2020 2020 2020 2020 2270 6174  ,.          "pat
+000001f0: 7465 726e 223a 2022 5e5c 5c5b 282e 2a3f  tern": "^\\[(.*?
+00000200: 295c 5c5d 2422 2c0a 2020 2020 2020 2020  )\\]$",.        
+00000210: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00000220: 2022 6174 7472 6962 7574 6522 0a20 2020   "attribute".   
+00000230: 2020 2020 207d 0a20 2020 2020 205d 2c0a       }.      ],.
+00000240: 2020 2020 2020 226d 6574 6164 6174 6122        "metadata"
+00000250: 3a20 7b0a 2020 2020 2020 2020 226d 696e  : {.        "min
+00000260: 5665 7273 696f 6e22 3a20 352e 340a 2020  Version": 5.4.  
+00000270: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
+00000280: 2022 616e 676c 6522 3a20 7b0a 2020 2020   "angle": {.    
+00000290: 2020 2264 6566 6175 6c74 223a 2030 2c0a    "default": 0,.
+000002a0: 2020 2020 2020 226f 6e65 4f66 223a 205b        "oneOf": [
+000002b0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+000002c0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+000002d0: 7269 6e67 222c 0a20 2020 2020 2020 2020  ring",.         
+000002e0: 2022 656e 756d 223a 205b 2022 6175 746f   "enum": [ "auto
+000002f0: 222c 2022 6175 746f 3222 2c20 2266 6f6c  ", "auto2", "fol
+00000300: 6c6f 7722 205d 2c0a 2020 2020 2020 2020  low" ],.        
+00000310: 2020 2261 6464 6974 696f 6e61 6c50 726f    "additionalPro
+00000320: 7065 7274 6965 7322 3a20 6661 6c73 650a  perties": false.
+00000330: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000340: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00000350: 7479 7065 223a 2022 6e75 6d62 6572 222c  type": "number",
+00000360: 0a20 2020 2020 2020 2020 2022 6d69 6e69  .          "mini
+00000370: 6d75 6d22 3a20 2d33 3630 2c0a 2020 2020  mum": -360,.    
+00000380: 2020 2020 2020 226d 6178 696d 756d 223a        "maximum":
+00000390: 2033 3630 0a20 2020 2020 2020 207d 2c0a   360.        },.
+000003a0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000003b0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+000003c0: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
+000003d0: 2270 6174 7465 726e 223a 2022 5e5c 5c5b  "pattern": "^\\[
+000003e0: 282e 2a3f 295c 5c5d 2422 2c0a 2020 2020  (.*?)\\]$",.    
+000003f0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000400: 6f6e 223a 2022 6174 7472 6962 7574 6522  on": "attribute"
+00000410: 2c0a 2020 2020 2020 2020 2020 226d 6574  ,.          "met
+00000420: 6164 6174 6122 3a20 7b0a 2020 2020 2020  adata": {.      
+00000430: 2020 2020 2020 226d 696e 5665 7273 696f        "minVersio
+00000440: 6e22 3a20 352e 300a 2020 2020 2020 2020  n": 5.0.        
+00000450: 2020 7d0a 2020 2020 2020 2020 7d0a 2020    }.        }.  
+00000460: 2020 2020 5d0a 2020 2020 7d2c 0a20 2020      ].    },.   
+00000470: 2022 616e 7469 616c 6961 7322 3a20 7b0a   "antialias": {.
+00000480: 2020 2020 2020 2274 7970 6522 3a20 2262        "type": "b
+00000490: 6f6f 6c65 616e 222c 0a20 2020 2020 2022  oolean",.      "
+000004a0: 6465 6661 756c 7422 3a20 6661 6c73 650a  default": false.
+000004b0: 2020 2020 7d2c 0a20 2020 2022 6261 636b      },.    "back
+000004c0: 6772 6f75 6e64 636f 6c6f 7222 3a20 7b0a  groundcolor": {.
+000004d0: 2020 2020 2020 2261 6c6c 4f66 223a 205b        "allOf": [
+000004e0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+000004f0: 2020 2020 2022 2472 6566 223a 2022 636f       "$ref": "co
+00000500: 6c6f 722e 6a73 6f6e 220a 2020 2020 2020  lor.json".      
+00000510: 2020 7d0a 2020 2020 2020 5d2c 0a20 2020    }.      ],.   
+00000520: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
+00000530: 0a20 2020 2020 2020 2022 6d61 7856 6572  .        "maxVer
+00000540: 7369 6f6e 223a 2036 2e30 0a20 2020 2020  sion": 6.0.     
+00000550: 207d 0a20 2020 207d 2c0a 2020 2020 2262   }.    },.    "b
+00000560: 6163 6b67 726f 756e 6473 6861 646f 7763  ackgroundshadowc
+00000570: 6f6c 6f72 223a 207b 0a20 2020 2020 2022  olor": {.      "
+00000580: 616c 6c4f 6622 3a20 5b0a 2020 2020 2020  allOf": [.      
+00000590: 2020 7b0a 2020 2020 2020 2020 2020 2224    {.          "$
+000005a0: 7265 6622 3a20 2263 6f6c 6f72 2e6a 736f  ref": "color.jso
+000005b0: 6e22 0a20 2020 2020 2020 207d 0a20 2020  n".        }.   
+000005c0: 2020 205d 2c0a 2020 2020 2020 226d 6574     ],.      "met
+000005d0: 6164 6174 6122 3a20 7b0a 2020 2020 2020  adata": {.      
+000005e0: 2020 226d 6178 5665 7273 696f 6e22 3a20    "maxVersion": 
+000005f0: 362e 300a 2020 2020 2020 7d0a 2020 2020  6.0.      }.    
+00000600: 7d2c 0a20 2020 2022 6261 636b 6772 6f75  },.    "backgrou
+00000610: 6e64 7368 6164 6f77 7369 7a65 223a 207b  ndshadowsize": {
+00000620: 0a20 2020 2020 2022 6465 6661 756c 7422  .      "default"
+00000630: 3a20 6661 6c73 652c 0a20 2020 2020 2022  : false,.      "
+00000640: 616c 6c4f 6622 3a20 5b0a 2020 2020 2020  allOf": [.      
+00000650: 2020 7b0a 2020 2020 2020 2020 2020 2224    {.          "$
+00000660: 7265 6622 3a20 2270 6f69 6e74 732e 6a73  ref": "points.js
+00000670: 6f6e 220a 2020 2020 2020 2020 7d0a 2020  on".        }.  
+00000680: 2020 2020 5d2c 0a20 2020 2020 2022 6d65      ],.      "me
+00000690: 7461 6461 7461 223a 207b 0a20 2020 2020  tadata": {.     
+000006a0: 2020 2022 6d61 7856 6572 7369 6f6e 223a     "maxVersion":
+000006b0: 2036 2e30 0a20 2020 2020 207d 0a20 2020   6.0.      }.   
+000006c0: 207d 2c0a 2020 2020 2262 7566 6665 7222   },.    "buffer"
+000006d0: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+000006e0: 3a20 2269 6e74 6567 6572 222c 0a20 2020  : "integer",.   
+000006f0: 2020 2022 6465 6661 756c 7422 3a20 300a     "default": 0.
+00000700: 2020 2020 7d2c 0a20 2020 2022 636f 6c6f      },.    "colo
+00000710: 7222 3a20 7b0a 2020 2020 2020 226f 6e65  r": {.      "one
+00000720: 4f66 223a 205b 0a20 2020 2020 2020 207b  Of": [.        {
+00000730: 2022 2472 6566 223a 2022 636f 6c6f 722e   "$ref": "color.
+00000740: 6a73 6f6e 2220 7d2c 0a20 2020 2020 2020  json" },.       
+00000750: 207b 0a20 2020 2020 2020 2020 2022 7479   {.          "ty
+00000760: 7065 223a 2022 7374 7269 6e67 222c 0a20  pe": "string",. 
+00000770: 2020 2020 2020 2020 2022 7061 7474 6572           "patter
+00000780: 6e22 3a20 225e 5c5c 5b28 2e2a 3f29 5c5c  n": "^\\[(.*?)\\
+00000790: 5d24 222c 0a20 2020 2020 2020 2020 2022  ]$",.          "
+000007a0: 6465 7363 7269 7074 696f 6e22 3a20 2261  description": "a
+000007b0: 7474 7269 6275 7465 222c 0a20 2020 2020  ttribute",.     
+000007c0: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
+000007d0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000007e0: 6d69 6e56 6572 7369 6f6e 223a 2035 2e30  minVersion": 5.0
+000007f0: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
+00000800: 2020 2020 207d 0a20 2020 2020 205d 0a20       }.      ]. 
+00000810: 2020 207d 2c0a 2020 2020 2265 6e63 6f64     },.    "encod
+00000820: 696e 6722 3a20 7b0a 2020 2020 2020 2274  ing": {.      "t
+00000830: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+00000840: 2020 2020 2020 226d 6574 6164 6174 6122        "metadata"
+00000850: 3a20 7b0a 2020 2020 2020 2020 226d 6178  : {.        "max
+00000860: 5665 7273 696f 6e22 3a20 372e 360a 2020  Version": 7.6.  
+00000870: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
+00000880: 2022 6578 7072 6573 7369 6f6e 223a 207b   "expression": {
+00000890: 0a20 2020 2020 2022 616c 6c4f 6622 3a20  .      "allOf": 
+000008a0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+000008b0: 2020 2020 2020 2224 7265 6622 3a20 2265        "$ref": "e
+000008c0: 7870 7265 7373 696f 6e2e 6a73 6f6e 220a  xpression.json".
+000008d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000008e0: 5d2c 0a20 2020 2020 2022 6d65 7461 6461  ],.      "metada
+000008f0: 7461 223a 207b 0a20 2020 2020 2020 2022  ta": {.        "
+00000900: 6d69 6e56 6572 7369 6f6e 223a 2036 2e32  minVersion": 6.2
+00000910: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
+00000920: 2020 2020 2266 6f6e 7422 3a20 7b0a 2020      "font": {.  
+00000930: 2020 2020 2261 6e79 4f66 223a 205b 0a20      "anyOf": [. 
+00000940: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000950: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+00000960: 6e67 222c 0a20 2020 2020 2020 2020 2022  ng",.          "
+00000970: 7061 7474 6572 6e22 3a20 225e 5c5c 5b28  pattern": "^\\[(
+00000980: 2e2a 3f29 5c5c 5d24 222c 0a20 2020 2020  .*?)\\]$",.     
+00000990: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000009a0: 6e22 3a20 2261 7474 7269 6275 7465 222c  n": "attribute",
+000009b0: 0a20 2020 2020 2020 2020 2022 6d65 7461  .          "meta
+000009c0: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
+000009d0: 2020 2020 2022 6d69 6e56 6572 7369 6f6e       "minVersion
+000009e0: 223a 2035 2e36 0a20 2020 2020 2020 2020  ": 5.6.         
+000009f0: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00000a00: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000a10: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00000a20: 6722 0a20 2020 2020 2020 207d 0a20 2020  g".        }.   
+00000a30: 2020 205d 0a20 2020 207d 2c0a 2020 2020     ].    },.    
+00000a40: 2266 6f72 6365 223a 207b 0a20 2020 2020  "force": {.     
+00000a50: 2022 6465 6661 756c 7422 3a20 6661 6c73   "default": fals
+00000a60: 652c 0a20 2020 2020 2022 6f6e 654f 6622  e,.      "oneOf"
+00000a70: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+00000a80: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000a90: 2262 6f6f 6c65 616e 220a 2020 2020 2020  "boolean".      
+00000aa0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00000ab0: 2020 2020 2020 2020 2022 656e 756d 223a           "enum":
+00000ac0: 205b 2022 6772 6f75 7022 205d 2c0a 2020   [ "group" ],.  
+00000ad0: 2020 2020 2020 2020 226d 6574 6164 6174          "metadat
+00000ae0: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00000af0: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
+00000b00: 362e 320a 2020 2020 2020 2020 2020 7d0a  6.2.          }.
+00000b10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000b20: 5d0a 2020 2020 7d2c 0a20 2020 2022 6d61  ].    },.    "ma
+00000b30: 786c 656e 6774 6822 3a20 7b0a 2020 2020  xlength": {.    
+00000b40: 2020 2274 7970 6522 3a20 2269 6e74 6567    "type": "integ
+00000b50: 6572 222c 0a20 2020 2020 2022 6578 636c  er",.      "excl
+00000b60: 7573 6976 654d 696e 696d 756d 223a 2030  usiveMinimum": 0
+00000b70: 2c0a 2020 2020 2020 226d 6574 6164 6174  ,.      "metadat
+00000b80: 6122 3a20 7b0a 2020 2020 2020 2020 226d  a": {.        "m
+00000b90: 696e 5665 7273 696f 6e22 3a20 352e 340a  inVersion": 5.4.
+00000ba0: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000bb0: 2020 2022 6d61 786f 7665 726c 6170 616e     "maxoverlapan
+00000bc0: 676c 6522 3a20 7b0a 2020 2020 2020 2264  gle": {.      "d
+00000bd0: 6566 6175 6c74 223a 2032 322e 352c 0a20  efault": 22.5,. 
+00000be0: 2020 2020 2022 7479 7065 223a 2022 6e75       "type": "nu
+00000bf0: 6d62 6572 222c 0a20 2020 2020 2022 6d69  mber",.      "mi
+00000c00: 6e69 6d75 6d22 3a20 302c 0a20 2020 2020  nimum": 0,.     
+00000c10: 2022 6d61 7869 6d75 6d22 3a20 3336 302c   "maximum": 360,
+00000c20: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
+00000c30: 223a 207b 0a20 2020 2020 2020 2022 6d69  ": {.        "mi
+00000c40: 6e56 6572 7369 6f6e 223a 2036 2e30 0a20  nVersion": 6.0. 
+00000c50: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00000c60: 2020 226d 6178 7363 616c 6564 656e 6f6d    "maxscaledenom
+00000c70: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000c80: 223a 2022 6e75 6d62 6572 222c 0a20 2020  ": "number",.   
+00000c90: 2020 2022 6d69 6e69 6d75 6d22 3a20 302c     "minimum": 0,
+00000ca0: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
+00000cb0: 223a 207b 0a20 2020 2020 2020 2022 6d69  ": {.        "mi
+00000cc0: 6e56 6572 7369 6f6e 223a 2035 2e34 0a20  nVersion": 5.4. 
+00000cd0: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00000ce0: 2020 226d 6178 7369 7a65 223a 207b 0a20    "maxsize": {. 
+00000cf0: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
+00000d00: 7465 6765 7222 2c0a 2020 2020 2020 2264  teger",.      "d
+00000d10: 6566 6175 6c74 223a 2032 3536 2c0a 2020  efault": 256,.  
+00000d20: 2020 2020 2265 7863 6c75 7369 7665 4d69      "exclusiveMi
+00000d30: 6e69 6d75 6d22 3a20 300a 2020 2020 7d2c  nimum": 0.    },
+00000d40: 0a20 2020 2022 6d69 6e64 6973 7461 6e63  .    "mindistanc
+00000d50: 6522 3a20 7b0a 2020 2020 2020 2274 7970  e": {.      "typ
+00000d60: 6522 3a20 2269 6e74 6567 6572 222c 0a20  e": "integer",. 
+00000d70: 2020 2020 2022 6578 636c 7573 6976 654d       "exclusiveM
+00000d80: 696e 696d 756d 223a 2030 0a20 2020 207d  inimum": 0.    }
+00000d90: 2c0a 2020 2020 226d 696e 6665 6174 7572  ,.    "minfeatur
+00000da0: 6573 697a 6522 3a20 7b0a 2020 2020 2020  esize": {.      
+00000db0: 226f 6e65 4f66 223a 205b 0a20 2020 2020  "oneOf": [.     
+00000dc0: 2020 207b 2022 656e 756d 223a 205b 2022     { "enum": [ "
+00000dd0: 6175 746f 2220 5d20 7d2c 0a20 2020 2020  auto" ] },.     
+00000de0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00000df0: 7479 7065 223a 2022 696e 7465 6765 7222  type": "integer"
+00000e00: 2c0a 2020 2020 2020 2020 2020 2265 7863  ,.          "exc
+00000e10: 6c75 7369 7665 4d69 6e69 6d75 6d22 3a20  lusiveMinimum": 
+00000e20: 300a 2020 2020 2020 2020 7d0a 2020 2020  0.        }.    
+00000e30: 2020 5d0a 2020 2020 7d2c 0a20 2020 2022    ].    },.    "
+00000e40: 6d69 6e73 6361 6c65 6465 6e6f 6d22 3a20  minscaledenom": 
+00000e50: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+00000e60: 226e 756d 6265 7222 2c0a 2020 2020 2020  "number",.      
+00000e70: 226d 696e 696d 756d 223a 2030 2c0a 2020  "minimum": 0,.  
+00000e80: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
+00000e90: 7b0a 2020 2020 2020 2020 226d 696e 5665  {.        "minVe
+00000ea0: 7273 696f 6e22 3a20 352e 340a 2020 2020  rsion": 5.4.    
+00000eb0: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
+00000ec0: 6d69 6e73 697a 6522 3a20 7b0a 2020 2020  minsize": {.    
+00000ed0: 2020 2274 7970 6522 3a20 2269 6e74 6567    "type": "integ
+00000ee0: 6572 222c 0a20 2020 2020 2022 6578 636c  er",.      "excl
+00000ef0: 7573 6976 654d 696e 696d 756d 223a 2030  usiveMinimum": 0
+00000f00: 2c0a 2020 2020 2020 2264 6566 6175 6c74  ,.      "default
+00000f10: 223a 2034 0a20 2020 207d 2c0a 2020 2020  ": 4.    },.    
+00000f20: 226f 6666 7365 7422 3a20 7b0a 2020 2020  "offset": {.    
+00000f30: 2020 2264 6566 6175 6c74 223a 205b 2030    "default": [ 0
+00000f40: 2c20 3020 5d2c 0a20 2020 2020 2022 6f6e  , 0 ],.      "on
+00000f50: 654f 6622 3a20 5b0a 2020 2020 2020 2020  eOf": [.        
+00000f60: 7b0a 2020 2020 2020 2020 2020 2274 7970  {.          "typ
+00000f70: 6522 3a20 2261 7272 6179 222c 0a20 2020  e": "array",.   
+00000f80: 2020 2020 2020 2022 6974 656d 7322 3a20         "items": 
+00000f90: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
+00000fa0: 7970 6522 3a20 226e 756d 6265 7222 0a20  ype": "number". 
+00000fb0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000fc0: 2020 2020 2020 226d 696e 4974 656d 7322        "minItems"
+00000fd0: 3a20 322c 0a20 2020 2020 2020 2020 2022  : 2,.          "
+00000fe0: 6d61 7849 7465 6d73 223a 2032 0a20 2020  maxItems": 2.   
+00000ff0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001000: 7b0a 2020 2020 2020 2020 2020 2274 7970  {.          "typ
+00001010: 6522 3a20 2261 7272 6179 222c 0a20 2020  e": "array",.   
+00001020: 2020 2020 2020 2022 6974 656d 7322 3a20         "items": 
+00001030: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
+00001040: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+00001050: 2020 2020 2020 2020 2020 2020 2270 6174              "pat
+00001060: 7465 726e 223a 2022 5e5c 5c5b 282e 2a3f  tern": "^\\[(.*?
+00001070: 295c 5c5d 2422 2c0a 2020 2020 2020 2020  )\\]$",.        
+00001080: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00001090: 223a 2022 6174 7472 6962 7574 6522 0a20  ": "attribute". 
+000010a0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000010b0: 2020 2020 2020 226d 696e 4974 656d 7322        "minItems"
+000010c0: 3a20 322c 0a20 2020 2020 2020 2020 2022  : 2,.          "
+000010d0: 6d61 7849 7465 6d73 223a 2032 2c0a 2020  maxItems": 2,.  
+000010e0: 2020 2020 2020 2020 226d 6574 6164 6174          "metadat
+000010f0: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00001100: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
+00001110: 372e 360a 2020 2020 2020 2020 2020 7d0a  7.6.          }.
+00001120: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001130: 5d0a 2020 2020 7d2c 0a20 2020 2022 6f75  ].    },.    "ou
+00001140: 746c 696e 6563 6f6c 6f72 223a 207b 0a20  tlinecolor": {. 
+00001150: 2020 2020 2022 6f6e 654f 6622 3a20 5b0a       "oneOf": [.
+00001160: 2020 2020 2020 2020 7b20 2224 7265 6622          { "$ref"
+00001170: 3a20 2263 6f6c 6f72 2e6a 736f 6e22 207d  : "color.json" }
+00001180: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00001190: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+000011a0: 7472 696e 6722 2c0a 2020 2020 2020 2020  tring",.        
+000011b0: 2020 2270 6174 7465 726e 223a 2022 5e5c    "pattern": "^\
+000011c0: 5c5b 282e 2a3f 295c 5c5d 2422 2c0a 2020  \[(.*?)\\]$",.  
+000011d0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000011e0: 7469 6f6e 223a 2022 6174 7472 6962 7574  tion": "attribut
+000011f0: 6522 2c0a 2020 2020 2020 2020 2020 226d  e",.          "m
+00001200: 6574 6164 6174 6122 3a20 7b0a 2020 2020  etadata": {.    
+00001210: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+00001220: 696f 6e22 3a20 352e 300a 2020 2020 2020  ion": 5.0.      
+00001230: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00001240: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
+00001250: 2020 2022 6f75 746c 696e 6577 6964 7468     "outlinewidth
+00001260: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00001270: 223a 2022 696e 7465 6765 7222 2c0a 2020  ": "integer",.  
+00001280: 2020 2020 2265 7863 6c75 7369 7665 4d69      "exclusiveMi
+00001290: 6e69 6d75 6d22 3a20 302c 0a20 2020 2020  nimum": 0,.     
+000012a0: 2022 6465 6661 756c 7422 3a20 310a 2020   "default": 1.  
+000012b0: 2020 7d2c 0a20 2020 2022 7061 7274 6961    },.    "partia
+000012c0: 6c73 223a 207b 0a20 2020 2020 2022 7479  ls": {.      "ty
+000012d0: 7065 223a 2022 626f 6f6c 6561 6e22 2c0a  pe": "boolean",.
+000012e0: 2020 2020 2020 2264 6566 6175 6c74 223a        "default":
+000012f0: 2066 616c 7365 0a20 2020 207d 2c0a 2020   false.    },.  
+00001300: 2020 2270 6f73 6974 696f 6e22 3a20 7b0a    "position": {.
+00001310: 2020 2020 2020 2264 6566 6175 6c74 223a        "default":
+00001320: 2022 6363 222c 0a20 2020 2020 2022 6f6e   "cc",.      "on
+00001330: 654f 6622 3a20 5b0a 2020 2020 2020 2020  eOf": [.        
+00001340: 7b20 2265 6e75 6d22 3a20 5b20 2261 7574  { "enum": [ "aut
+00001350: 6f22 205d 207d 2c0a 2020 2020 2020 2020  o" ] },.        
+00001360: 7b0a 2020 2020 2020 2020 2020 2224 7265  {.          "$re
+00001370: 6622 3a20 2270 6f73 6974 696f 6e2e 6a73  f": "position.js
+00001380: 6f6e 220a 2020 2020 2020 2020 7d2c 0a20  on".        },. 
+00001390: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000013a0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+000013b0: 6e67 222c 0a20 2020 2020 2020 2020 2022  ng",.          "
+000013c0: 7061 7474 6572 6e22 3a20 225e 5c5c 5b28  pattern": "^\\[(
+000013d0: 2e2a 3f29 5c5c 5d24 222c 0a20 2020 2020  .*?)\\]$",.     
+000013e0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000013f0: 6e22 3a20 2261 7474 7269 6275 7465 220a  n": "attribute".
+00001400: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001410: 5d0a 2020 2020 7d2c 0a20 2020 2022 7072  ].    },.    "pr
+00001420: 696f 7269 7479 223a 207b 0a20 2020 2020  iority": {.     
+00001430: 2022 6465 6661 756c 7422 3a20 312c 0a20   "default": 1,. 
+00001440: 2020 2020 2022 6d69 6e69 6d75 6d22 3a20       "minimum": 
+00001450: 312c 0a20 2020 2020 2022 6d61 7869 6d75  1,.      "maximu
+00001460: 6d22 3a20 3130 2c0a 2020 2020 2020 2261  m": 10,.      "a
+00001470: 6e79 4f66 223a 205b 0a20 2020 2020 2020  nyOf": [.       
+00001480: 207b 0a20 2020 2020 2020 2020 2022 7479   {.          "ty
+00001490: 7065 223a 2022 696e 7465 6765 7222 0a20  pe": "integer". 
+000014a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000014b0: 2020 7b0a 2020 2020 2020 2020 2020 2274    {.          "t
+000014c0: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+000014d0: 2020 2020 2020 2020 2020 2270 6174 7465            "patte
+000014e0: 726e 223a 2022 5e5c 5c5b 282e 2a3f 295c  rn": "^\\[(.*?)\
+000014f0: 5c5d 2422 2c0a 2020 2020 2020 2020 2020  \]$",.          
+00001500: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00001510: 6174 7472 6962 7574 6522 0a20 2020 2020  attribute".     
+00001520: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00001530: 2020 2020 2020 2020 2020 2261 6c6c 4f66            "allOf
+00001540: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00001550: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001560: 2022 2472 6566 223a 2022 6578 7072 6573   "$ref": "expres
+00001570: 7369 6f6e 2e6a 736f 6e22 0a20 2020 2020  sion.json".     
+00001580: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001590: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+000015a0: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
+000015b0: 2020 2020 2020 2020 2020 226d 696e 5665            "minVe
+000015c0: 7273 696f 6e22 3a20 382e 320a 2020 2020  rsion": 8.2.    
+000015d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000015e0: 7d0a 2020 2020 2020 5d2c 0a20 2020 2020  }.      ],.     
+000015f0: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
+00001600: 2020 2020 2020 2022 6d69 6e56 6572 7369         "minVersi
+00001610: 6f6e 223a 2035 2e30 0a20 2020 2020 207d  on": 5.0.      }
+00001620: 0a20 2020 207d 2c0a 2020 2020 2272 6570  .    },.    "rep
+00001630: 6561 7464 6973 7461 6e63 6522 3a20 7b0a  eatdistance": {.
+00001640: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
+00001650: 6e74 6567 6572 222c 0a20 2020 2020 2022  nteger",.      "
+00001660: 6465 6661 756c 7422 3a20 302c 0a20 2020  default": 0,.   
+00001670: 2020 2022 6578 636c 7573 6976 654d 696e     "exclusiveMin
+00001680: 696d 756d 223a 2030 2c0a 2020 2020 2020  imum": 0,.      
+00001690: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
+000016a0: 2020 2020 2020 226d 696e 5665 7273 696f        "minVersio
+000016b0: 6e22 3a20 352e 360a 2020 2020 2020 7d0a  n": 5.6.      }.
+000016c0: 2020 2020 7d2c 0a20 2020 2022 7368 6164      },.    "shad
+000016d0: 6f77 636f 6c6f 7222 3a20 7b0a 2020 2020  owcolor": {.    
+000016e0: 2020 2224 7265 6622 3a20 2263 6f6c 6f72    "$ref": "color
+000016f0: 2e6a 736f 6e22 0a20 2020 207d 2c0a 2020  .json".    },.  
+00001700: 2020 2273 6861 646f 7773 697a 6522 3a20    "shadowsize": 
+00001710: 7b0a 2020 2020 2020 2264 6566 6175 6c74  {.      "default
+00001720: 223a 205b 2031 2c20 3120 5d2c 0a20 2020  ": [ 1, 1 ],.   
+00001730: 2020 2022 6f6e 654f 6622 3a20 5b0a 2020     "oneOf": [.  
+00001740: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001750: 2020 2274 7970 6522 3a20 2261 7272 6179    "type": "array
+00001760: 222c 0a20 2020 2020 2020 2020 2022 6974  ",.          "it
+00001770: 656d 7322 3a20 7b0a 2020 2020 2020 2020  ems": {.        
+00001780: 2020 2020 2274 7970 6522 3a20 2269 6e74      "type": "int
+00001790: 6567 6572 220a 2020 2020 2020 2020 2020  eger".          
+000017a0: 7d2c 0a20 2020 2020 2020 2020 2022 6d69  },.          "mi
+000017b0: 6e49 7465 6d73 223a 2032 2c0a 2020 2020  nItems": 2,.    
+000017c0: 2020 2020 2020 226d 6178 4974 656d 7322        "maxItems"
+000017d0: 3a20 320a 2020 2020 2020 2020 7d2c 0a20  : 2.        },. 
+000017e0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000017f0: 2020 2022 7479 7065 223a 2022 6172 7261     "type": "arra
+00001800: 7922 2c0a 2020 2020 2020 2020 2020 2269  y",.          "i
+00001810: 7465 6d73 223a 205b 0a20 2020 2020 2020  tems": [.       
+00001820: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001830: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
+00001840: 7465 6765 7222 0a20 2020 2020 2020 2020  teger".         
+00001850: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00001860: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00001870: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00001880: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
+00001890: 2020 2270 6174 7465 726e 223a 2022 5e5c    "pattern": "^\
+000018a0: 5c5b 282e 2a3f 295c 5c5d 2422 2c0a 2020  \[(.*?)\\]$",.  
+000018b0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+000018c0: 6372 6970 7469 6f6e 223a 2022 6174 7472  cription": "attr
+000018d0: 6962 7574 6522 0a20 2020 2020 2020 2020  ibute".         
+000018e0: 2020 207d 0a20 2020 2020 2020 2020 205d     }.          ]
+000018f0: 2c0a 2020 2020 2020 2020 2020 226d 696e  ,.          "min
+00001900: 4974 656d 7322 3a20 322c 0a20 2020 2020  Items": 2,.     
+00001910: 2020 2020 2022 6d61 7849 7465 6d73 223a       "maxItems":
+00001920: 2032 2c0a 2020 2020 2020 2020 2020 226d   2,.          "m
+00001930: 6574 6164 6174 6122 3a20 7b0a 2020 2020  etadata": {.    
+00001940: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+00001950: 696f 6e22 3a20 362e 300a 2020 2020 2020  ion": 6.0.      
+00001960: 2020 2020 7d0a 2020 2020 2020 2020 7d0a      }.        }.
+00001970: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
+00001980: 2020 2022 7369 7a65 223a 207b 0a20 2020     "size": {.   
+00001990: 2020 2022 6465 6661 756c 7422 3a20 3130     "default": 10
+000019a0: 2c0a 2020 2020 2020 2265 7863 6c75 7369  ,.      "exclusi
+000019b0: 7665 4d69 6e69 6d75 6d22 3a20 312c 0a20  veMinimum": 1,. 
+000019c0: 2020 2020 2022 616e 794f 6622 3a20 5b0a       "anyOf": [.
+000019d0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000019e0: 2020 2020 2274 7970 6522 3a20 2269 6e74      "type": "int
+000019f0: 6567 6572 220a 2020 2020 2020 2020 7d2c  eger".        },
+00001a00: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00001a10: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00001a20: 7269 6e67 222c 0a20 2020 2020 2020 2020  ring",.         
+00001a30: 2022 656e 756d 223a 205b 2022 7469 6e79   "enum": [ "tiny
+00001a40: 222c 2022 736d 616c 6c22 2c20 226d 6564  ", "small", "med
+00001a50: 6975 6d22 2c20 226c 6172 6765 222c 2022  ium", "large", "
+00001a60: 6769 616e 7422 205d 2c0a 2020 2020 2020  giant" ],.      
+00001a70: 2020 2020 2261 6464 6974 696f 6e61 6c50      "additionalP
+00001a80: 726f 7065 7274 6965 7322 3a20 6661 6c73  roperties": fals
+00001a90: 650a 2020 2020 2020 2020 7d2c 0a20 2020  e.        },.   
+00001aa0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001ab0: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+00001ac0: 222c 0a20 2020 2020 2020 2020 2022 7061  ",.          "pa
+00001ad0: 7474 6572 6e22 3a20 225e 5c5c 5b28 2e2a  ttern": "^\\[(.*
+00001ae0: 3f29 5c5c 5d24 222c 0a20 2020 2020 2020  ?)\\]$",.       
+00001af0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00001b00: 3a20 2261 7474 7269 6275 7465 222c 0a20  : "attribute",. 
+00001b10: 2020 2020 2020 2020 2022 6d65 7461 6461           "metada
+00001b20: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00001b30: 2020 2022 6d69 6e56 6572 7369 6f6e 223a     "minVersion":
+00001b40: 2035 2e30 0a20 2020 2020 2020 2020 207d   5.0.          }
+00001b50: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00001b60: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00001b70: 2261 6c6c 4f66 223a 205b 0a20 2020 2020  "allOf": [.     
+00001b80: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001b90: 2020 2020 2020 2022 2472 6566 223a 2022         "$ref": "
+00001ba0: 6578 7072 6573 7369 6f6e 2e6a 736f 6e22  expression.json"
+00001bb0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00001bc0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00001bd0: 2020 2020 2020 226d 6574 6164 6174 6122        "metadata"
+00001be0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001bf0: 226d 696e 5665 7273 696f 6e22 3a20 372e  "minVersion": 7.
+00001c00: 360a 2020 2020 2020 2020 2020 7d0a 2020  6.          }.  
+00001c10: 2020 2020 2020 7d0a 2020 2020 2020 5d0a        }.      ].
+00001c20: 2020 2020 7d2c 0a20 2020 2022 7374 796c      },.    "styl
+00001c30: 6573 223a 207b 0a20 2020 2020 2022 7479  es": {.      "ty
+00001c40: 7065 223a 2022 6172 7261 7922 2c0a 2020  pe": "array",.  
+00001c50: 2020 2020 2269 7465 6d73 223a 207b 0a20      "items": {. 
+00001c60: 2020 2020 2020 2022 2472 6566 223a 2022         "$ref": "
+00001c70: 7374 796c 652e 6a73 6f6e 220a 2020 2020  style.json".    
+00001c80: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
+00001c90: 7465 7874 223a 207b 0a20 2020 2020 2022  text": {.      "
+00001ca0: 6f6e 654f 6622 3a20 5b0a 2020 2020 2020  oneOf": [.      
+00001cb0: 2020 7b0a 2020 2020 2020 2020 2020 2224    {.          "$
+00001cc0: 7265 6622 3a20 2265 7870 7265 7373 696f  ref": "expressio
+00001cd0: 6e2e 6a73 6f6e 220a 2020 2020 2020 2020  n.json".        
+00001ce0: 7d0a 2020 2020 2020 5d2c 0a20 2020 2020  }.      ],.     
+00001cf0: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
+00001d00: 2020 2020 2020 2022 6d69 6e56 6572 7369         "minVersi
+00001d10: 6f6e 223a 2036 2e32 0a20 2020 2020 207d  on": 6.2.      }
+00001d20: 0a20 2020 207d 2c0a 2020 2020 2274 7970  .    },.    "typ
+00001d30: 6522 3a20 7b0a 2020 2020 2020 2274 7970  e": {.      "typ
+00001d40: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
+00001d50: 2020 2020 2265 6e75 6d22 3a20 5b20 2262      "enum": [ "b
+00001d60: 6974 6d61 7022 2c20 2274 7275 6574 7970  itmap", "truetyp
+00001d70: 6522 205d 2c0a 2020 2020 2020 2261 6464  e" ],.      "add
+00001d80: 6974 696f 6e61 6c50 726f 7065 7274 6965  itionalPropertie
+00001d90: 7322 3a20 6661 6c73 650a 2020 2020 7d2c  s": false.    },
+00001da0: 0a20 2020 2022 7772 6170 223a 207b 0a20  .    "wrap": {. 
+00001db0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00001dc0: 7269 6e67 222c 0a20 2020 2020 2022 6d69  ring",.      "mi
+00001dd0: 6e4c 656e 6774 6822 3a20 312c 0a20 2020  nLength": 1,.   
+00001de0: 2020 2022 6d61 784c 656e 6774 6822 3a20     "maxLength": 
+00001df0: 310a 2020 2020 7d0a 2020 7d0a 7d0a       1.    }.  }.}.
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/layer.json` & `mappyfile-1.0.2/mappyfile/schemas/layer.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 25% similar despite different names*

```diff
@@ -1,461 +1,437 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2272 6571 7569 7265 6422 3a20  ..  "required": 
-00000080: 5b20 2274 7970 6522 205d 2c0d 0a20 2022  [ "type" ],..  "
-00000090: 7072 6f70 6572 7469 6573 223a 207b 0d0a  properties": {..
-000000a0: 2020 2020 225f 5f74 7970 655f 5f22 3a20      "__type__": 
-000000b0: 7b0d 0a20 2020 2020 2022 656e 756d 223a  {..      "enum":
-000000c0: 205b 2022 6c61 7965 7222 205d 0d0a 2020   [ "layer" ]..  
-000000d0: 2020 7d2c 0d0a 2020 2020 225f 5f63 6f6d    },..    "__com
-000000e0: 6d65 6e74 735f 5f22 3a20 7b0d 0a20 2020  ments__": {..   
-000000f0: 2020 2022 7479 7065 223a 2022 6f62 6a65     "type": "obje
-00000100: 6374 220d 0a20 2020 207d 2c0d 0a20 2020  ct"..    },..   
-00000110: 2022 5f5f 706f 7369 7469 6f6e 5f5f 223a   "__position__":
-00000120: 207b 0d0a 2020 2020 2020 2274 7970 6522   {..      "type"
-00000130: 3a20 226f 626a 6563 7422 0d0a 2020 2020  : "object"..    
-00000140: 7d2c 0d0a 2020 2020 2269 6e63 6c75 6465  },..    "include
-00000150: 223a 207b 0d0a 2020 2020 2020 2274 7970  ": {..      "typ
-00000160: 6522 3a20 2261 7272 6179 222c 0d0a 2020  e": "array",..  
-00000170: 2020 2020 2269 7465 6d73 223a 207b 0d0a      "items": {..
-00000180: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00000190: 2273 7472 696e 6722 0d0a 2020 2020 2020  "string"..      
-000001a0: 7d0d 0a20 2020 207d 2c0d 0a20 2020 2022  }..    },..    "
-000001b0: 636c 6173 7365 7322 3a20 7b0d 0a20 2020  classes": {..   
-000001c0: 2020 2022 7479 7065 223a 2022 6172 7261     "type": "arra
-000001d0: 7922 2c0d 0a20 2020 2020 2022 6974 656d  y",..      "item
-000001e0: 7322 3a20 7b0d 0a20 2020 2020 2020 2022  s": {..        "
-000001f0: 2472 6566 223a 2022 636c 6173 732e 6a73  $ref": "class.js
-00000200: 6f6e 220d 0a20 2020 2020 207d 0d0a 2020  on"..      }..  
-00000210: 2020 7d2c 0d0a 2020 2020 2263 6c61 7373    },..    "class
-00000220: 6772 6f75 7022 3a20 7b0d 0a20 2020 2020  group": {..     
-00000230: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-00000240: 220d 0a20 2020 207d 2c0d 0a20 2020 2022  "..    },..    "
-00000250: 636c 6173 7369 7465 6d22 3a20 7b0d 0a20  classitem": {.. 
-00000260: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
-00000270: 7269 6e67 220d 0a20 2020 207d 2c0d 0a20  ring"..    },.. 
-00000280: 2020 2022 636c 7573 7465 7222 3a20 7b0d     "cluster": {.
-00000290: 0a20 2020 2020 2022 616c 6c4f 6622 3a20  .      "allOf": 
-000002a0: 5b0d 0a20 2020 2020 2020 207b 0d0a 2020  [..        {..  
-000002b0: 2020 2020 2020 2020 2224 7265 6622 3a20          "$ref": 
-000002c0: 2263 6c75 7374 6572 2e6a 736f 6e22 0d0a  "cluster.json"..
-000002d0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-000002e0: 205d 2c0d 0a20 2020 2020 2022 6d65 7461   ],..      "meta
-000002f0: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000300: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
-00000310: 362e 300d 0a20 2020 2020 207d 0d0a 2020  6.0..      }..  
-00000320: 2020 7d2c 0d0a 2020 2020 2263 6f6d 706f    },..    "compo
-00000330: 7369 7465 7322 3a20 7b0d 0a20 2020 2020  sites": {..     
-00000340: 2022 7479 7065 223a 2022 6172 7261 7922   "type": "array"
-00000350: 2c0d 0a20 2020 2020 2022 6974 656d 7322  ,..      "items"
-00000360: 3a20 7b0d 0a20 2020 2020 2020 2022 2472  : {..        "$r
-00000370: 6566 223a 2022 636f 6d70 6f73 6974 652e  ef": "composite.
-00000380: 6a73 6f6e 220d 0a20 2020 2020 207d 2c0d  json"..      },.
-00000390: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
-000003a0: 223a 207b 0d0a 2020 2020 2020 2020 226d  ": {..        "m
-000003b0: 696e 5665 7273 696f 6e22 3a20 372e 300d  inVersion": 7.0.
-000003c0: 0a20 2020 2020 207d 0d0a 2020 2020 7d2c  .      }..    },
-000003d0: 0d0a 2020 2020 2263 6f6e 6e65 6374 696f  ..    "connectio
-000003e0: 6e22 3a20 7b0d 0a20 2020 2020 2022 7479  n": {..      "ty
-000003f0: 7065 223a 2022 7374 7269 6e67 220d 0a20  pe": "string".. 
-00000400: 2020 207d 2c0d 0a20 2020 2022 636f 6e6e     },..    "conn
-00000410: 6563 7469 6f6e 6f70 7469 6f6e 7322 3a20  ectionoptions": 
-00000420: 7b0d 0a20 2020 2020 2022 616c 6c4f 6622  {..      "allOf"
-00000430: 3a20 5b0d 0a20 2020 2020 2020 207b 0d0a  : [..        {..
-00000440: 2020 2020 2020 2020 2020 2224 7265 6622            "$ref"
-00000450: 3a20 2263 6f6e 6e65 6374 696f 6e6f 7074  : "connectionopt
-00000460: 696f 6e73 2e6a 736f 6e22 0d0a 2020 2020  ions.json"..    
-00000470: 2020 2020 7d0d 0a20 2020 2020 205d 2c0d      }..      ],.
-00000480: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
-00000490: 223a 207b 0d0a 2020 2020 2020 2020 226d  ": {..        "m
-000004a0: 696e 5665 7273 696f 6e22 3a20 372e 360d  inVersion": 7.6.
-000004b0: 0a20 2020 2020 207d 0d0a 2020 2020 7d2c  .      }..    },
-000004c0: 0d0a 2020 2020 2263 6f6e 6e65 6374 696f  ..    "connectio
-000004d0: 6e74 7970 6522 3a20 7b0d 0a20 2020 2020  ntype": {..     
-000004e0: 2022 656e 756d 223a 205b 2022 636f 6e74   "enum": [ "cont
-000004f0: 6f75 7222 2c20 226b 6572 6e65 6c64 656e  our", "kernelden
-00000500: 7369 7479 222c 2022 6964 7722 2c20 226c  sity", "idw", "l
-00000510: 6f63 616c 222c 2022 6f67 7222 2c20 226f  ocal", "ogr", "o
-00000520: 7261 636c 6573 7061 7469 616c 222c 2022  raclespatial", "
-00000530: 706c 7567 696e 222c 2022 706f 7374 6769  plugin", "postgi
-00000540: 7322 2c20 2273 6465 222c 2022 756e 696f  s", "sde", "unio
-00000550: 6e22 2c20 2275 7672 6173 7465 7222 2c20  n", "uvraster", 
-00000560: 2277 6673 222c 2022 776d 7322 2c20 226d  "wfs", "wms", "m
-00000570: 7967 6973 222c 2022 666c 6174 6765 6f62  ygis", "flatgeob
-00000580: 7566 2220 5d0d 0a20 2020 207d 2c0d 0a20  uf" ]..    },.. 
-00000590: 2020 2022 6461 7461 223a 207b 0d0a 2020     "data": {..  
-000005a0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
-000005b0: 696e 6722 0d0a 2020 2020 7d2c 0d0a 2020  ing"..    },..  
-000005c0: 2020 2264 6562 7567 223a 207b 0d0a 2020    "debug": {..  
-000005d0: 2020 2020 2261 6c6c 4f66 223a 205b 0d0a      "allOf": [..
-000005e0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000005f0: 2020 2020 2022 2472 6566 223a 2022 6465       "$ref": "de
-00000600: 6275 672e 6a73 6f6e 220d 0a20 2020 2020  bug.json"..     
-00000610: 2020 207d 0d0a 2020 2020 2020 5d2c 0d0a     }..      ],..
-00000620: 2020 2020 2020 226d 6574 6164 6174 6122        "metadata"
-00000630: 3a20 7b0d 0a20 2020 2020 2020 2022 6d69  : {..        "mi
-00000640: 6e56 6572 7369 6f6e 223a 2035 2e30 0d0a  nVersion": 5.0..
-00000650: 2020 2020 2020 7d0d 0a20 2020 207d 2c0d        }..    },.
-00000660: 0a20 2020 2022 6475 6d70 223a 207b 0d0a  .    "dump": {..
-00000670: 2020 2020 2020 226f 6e65 4f66 223a 205b        "oneOf": [
-00000680: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00000690: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000006a0: 626f 6f6c 6561 6e22 0d0a 2020 2020 2020  boolean"..      
-000006b0: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
-000006c0: 0a20 2020 2020 2020 2020 2022 2472 6566  .          "$ref
-000006d0: 223a 2022 6f6e 6f66 662e 6a73 6f6e 220d  ": "onoff.json".
-000006e0: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-000006f0: 2020 5d2c 0d0a 2020 2020 2020 226d 6574    ],..      "met
-00000700: 6164 6174 6122 3a20 7b0d 0a20 2020 2020  adata": {..     
-00000710: 2020 2022 6d61 7856 6572 7369 6f6e 223a     "maxVersion":
-00000720: 2037 2e36 0d0a 2020 2020 2020 7d0d 0a20   7.6..      }.. 
-00000730: 2020 207d 2c0d 0a20 2020 2022 656e 636f     },..    "enco
-00000740: 6469 6e67 223a 207b 0d0a 2020 2020 2020  ding": {..      
-00000750: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00000760: 2c0d 0a20 2020 2020 2022 6d65 7461 6461  ,..      "metada
-00000770: 7461 223a 207b 0d0a 2020 2020 2020 2020  ta": {..        
-00000780: 226d 696e 5665 7273 696f 6e22 3a20 372e  "minVersion": 7.
-00000790: 300d 0a20 2020 2020 207d 0d0a 2020 2020  0..      }..    
-000007a0: 7d2c 0d0a 2020 2020 2265 7874 656e 7422  },..    "extent"
-000007b0: 3a20 7b0d 0a20 2020 2020 2022 2472 6566  : {..      "$ref
-000007c0: 223a 2022 6578 7465 6e74 2e6a 736f 6e22  ": "extent.json"
-000007d0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2266  ..    },..    "f
-000007e0: 6561 7475 7265 7322 3a20 7b0d 0a20 2020  eatures": {..   
-000007f0: 2020 2022 7479 7065 223a 2022 6172 7261     "type": "arra
-00000800: 7922 2c0d 0a20 2020 2020 2022 6974 656d  y",..      "item
-00000810: 7322 3a20 7b0d 0a20 2020 2020 2020 2022  s": {..        "
-00000820: 2472 6566 223a 2022 6665 6174 7572 652e  $ref": "feature.
-00000830: 6a73 6f6e 220d 0a20 2020 2020 207d 0d0a  json"..      }..
-00000840: 2020 2020 7d2c 0d0a 2020 2020 2266 696c      },..    "fil
-00000850: 7465 7222 3a20 7b0d 0a20 2020 2020 2022  ter": {..      "
-00000860: 2472 6566 223a 2022 6578 7072 6573 7369  $ref": "expressi
-00000870: 6f6e 2e6a 736f 6e22 0d0a 2020 2020 7d2c  on.json"..    },
-00000880: 0d0a 2020 2020 2266 696c 7465 7269 7465  ..    "filterite
-00000890: 6d22 3a20 7b0d 0a20 2020 2020 2022 7479  m": {..      "ty
-000008a0: 7065 223a 2022 7374 7269 6e67 220d 0a20  pe": "string".. 
-000008b0: 2020 207d 2c0d 0a20 2020 2022 666f 6f74     },..    "foot
-000008c0: 6572 223a 207b 0d0a 2020 2020 2020 2274  er": {..      "t
-000008d0: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
-000008e0: 2020 2020 7d2c 0d0a 2020 2020 2267 656f      },..    "geo
-000008f0: 6d74 7261 6e73 666f 726d 223a 207b 0d0a  mtransform": {..
-00000900: 2020 2020 2020 2261 6e79 4f66 223a 205b        "anyOf": [
-00000910: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00000920: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000930: 7374 7269 6e67 220d 0a20 2020 2020 2020  string"..       
-00000940: 207d 2c0d 0a20 2020 2020 2020 207b 0d0a   },..        {..
-00000950: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000960: 3a20 2273 7472 696e 6722 2c0d 0a20 2020  : "string",..   
-00000970: 2020 2020 2020 2022 7061 7474 6572 6e22         "pattern"
-00000980: 3a20 225e 5c5c 2828 2e2a 3f29 5c5c 2924  : "^\\((.*?)\\)$
-00000990: 220d 0a20 2020 2020 2020 207d 0d0a 2020  "..        }..  
-000009a0: 2020 2020 5d2c 0d0a 2020 2020 2020 226d      ],..      "m
-000009b0: 6574 6164 6174 6122 3a20 7b0d 0a20 2020  etadata": {..   
-000009c0: 2020 2020 2022 6d69 6e56 6572 7369 6f6e       "minVersion
-000009d0: 223a 2036 2e34 0d0a 2020 2020 2020 7d0d  ": 6.4..      }.
-000009e0: 0a20 2020 207d 2c0d 0a20 2020 2022 6772  .    },..    "gr
-000009f0: 6964 223a 207b 0d0a 2020 2020 2020 2224  id": {..      "$
-00000a00: 7265 6622 3a20 2267 7269 642e 6a73 6f6e  ref": "grid.json
-00000a10: 220d 0a20 2020 207d 2c0d 0a20 2020 2022  "..    },..    "
-00000a20: 6772 6f75 7022 3a20 7b0d 0a20 2020 2020  group": {..     
-00000a30: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-00000a40: 220d 0a20 2020 207d 2c0d 0a20 2020 2022  "..    },..    "
-00000a50: 6865 6164 6572 223a 207b 0d0a 2020 2020  header": {..    
-00000a60: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00000a70: 6722 0d0a 2020 2020 7d2c 0d0a 2020 2020  g"..    },..    
-00000a80: 226a 6f69 6e73 223a 207b 0d0a 2020 2020  "joins": {..    
-00000a90: 2020 2274 7970 6522 3a20 2261 7272 6179    "type": "array
-00000aa0: 222c 0d0a 2020 2020 2020 2269 7465 6d73  ",..      "items
-00000ab0: 223a 207b 0d0a 2020 2020 2020 2020 2224  ": {..        "$
-00000ac0: 7265 6622 3a20 226a 6f69 6e2e 6a73 6f6e  ref": "join.json
-00000ad0: 220d 0a20 2020 2020 207d 0d0a 2020 2020  "..      }..    
-00000ae0: 7d2c 0d0a 2020 2020 226c 6162 656c 616e  },..    "labelan
-00000af0: 676c 6569 7465 6d22 3a20 7b0d 0a20 2020  gleitem": {..   
-00000b00: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
-00000b10: 6e67 222c 0d0a 2020 2020 2020 226d 6574  ng",..      "met
-00000b20: 6164 6174 6122 3a20 7b0d 0a20 2020 2020  adata": {..     
-00000b30: 2020 2022 6d61 7856 6572 7369 6f6e 223a     "maxVersion":
-00000b40: 2035 2e36 0d0a 2020 2020 2020 7d0d 0a20   5.6..      }.. 
-00000b50: 2020 207d 2c0d 0a20 2020 2022 6c61 6265     },..    "labe
-00000b60: 6c63 6163 6865 223a 207b 0d0a 2020 2020  lcache": {..    
-00000b70: 2020 2224 7265 6622 3a20 226f 6e6f 6666    "$ref": "onoff
-00000b80: 2e6a 736f 6e22 0d0a 2020 2020 7d2c 0d0a  .json"..    },..
-00000b90: 2020 2020 226c 6162 656c 6974 656d 223a      "labelitem":
-00000ba0: 207b 0d0a 2020 2020 2020 2274 7970 6522   {..      "type"
-00000bb0: 3a20 2273 7472 696e 6722 0d0a 2020 2020  : "string"..    
-00000bc0: 7d2c 0d0a 2020 2020 226c 6162 656c 6d61  },..    "labelma
-00000bd0: 7873 6361 6c65 223a 207b 0d0a 2020 2020  xscale": {..    
-00000be0: 2020 2274 7970 6522 3a20 226e 756d 6265    "type": "numbe
-00000bf0: 7222 2c0d 0a20 2020 2020 2022 6d65 7461  r",..      "meta
-00000c00: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000c10: 2020 226d 6178 5665 7273 696f 6e22 3a20    "maxVersion": 
-00000c20: 352e 300d 0a20 2020 2020 207d 0d0a 2020  5.0..      }..  
-00000c30: 2020 7d2c 0d0a 2020 2020 226c 6162 656c    },..    "label
-00000c40: 6d69 6e73 6361 6c65 223a 207b 0d0a 2020  minscale": {..  
-00000c50: 2020 2020 2274 7970 6522 3a20 226e 756d      "type": "num
-00000c60: 6265 7222 2c0d 0a20 2020 2020 2022 6d65  ber",..      "me
-00000c70: 7461 6461 7461 223a 207b 0d0a 2020 2020  tadata": {..    
-00000c80: 2020 2020 226d 6178 5665 7273 696f 6e22      "maxVersion"
-00000c90: 3a20 352e 300d 0a20 2020 2020 207d 0d0a  : 5.0..      }..
-00000ca0: 2020 2020 7d2c 0d0a 2020 2020 226c 6162      },..    "lab
-00000cb0: 656c 6d61 7873 6361 6c65 6465 6e6f 6d22  elmaxscaledenom"
-00000cc0: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000cd0: 223a 2022 6e75 6d62 6572 222c 0d0a 2020  ": "number",..  
-00000ce0: 2020 2020 226d 696e 696d 756d 223a 2030      "minimum": 0
-00000cf0: 2c0d 0a20 2020 2020 2022 6d65 7461 6461  ,..      "metada
-00000d00: 7461 223a 207b 0d0a 2020 2020 2020 2020  ta": {..        
-00000d10: 226d 696e 5665 7273 696f 6e22 3a20 352e  "minVersion": 5.
-00000d20: 300d 0a20 2020 2020 207d 0d0a 2020 2020  0..      }..    
-00000d30: 7d2c 0d0a 2020 2020 226c 6162 656c 6d69  },..    "labelmi
-00000d40: 6e73 6361 6c65 6465 6e6f 6d22 3a20 7b0d  nscaledenom": {.
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2272  $": {}.  },.  "r
+00000070: 6571 7569 7265 6422 3a20 5b20 2274 7970  equired": [ "typ
+00000080: 6522 205d 2c0a 2020 2270 726f 7065 7274  e" ],.  "propert
+00000090: 6965 7322 3a20 7b0a 2020 2020 225f 5f74  ies": {.    "__t
+000000a0: 7970 655f 5f22 3a20 7b0a 2020 2020 2020  ype__": {.      
+000000b0: 2265 6e75 6d22 3a20 5b20 226c 6179 6572  "enum": [ "layer
+000000c0: 2220 5d0a 2020 2020 7d2c 0a20 2020 2022  " ].    },.    "
+000000d0: 5f5f 636f 6d6d 656e 7473 5f5f 223a 207b  __comments__": {
+000000e0: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+000000f0: 6f62 6a65 6374 220a 2020 2020 7d2c 0a20  object".    },. 
+00000100: 2020 2022 5f5f 706f 7369 7469 6f6e 5f5f     "__position__
+00000110: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000120: 223a 2022 6f62 6a65 6374 220a 2020 2020  ": "object".    
+00000130: 7d2c 0a20 2020 2022 696e 636c 7564 6522  },.    "include"
+00000140: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+00000150: 3a20 2261 7272 6179 222c 0a20 2020 2020  : "array",.     
+00000160: 2022 6974 656d 7322 3a20 7b0a 2020 2020   "items": {.    
+00000170: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00000180: 696e 6722 0a20 2020 2020 207d 0a20 2020  ing".      }.   
+00000190: 207d 2c0a 2020 2020 2263 6c61 7373 6573   },.    "classes
+000001a0: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+000001b0: 223a 2022 6172 7261 7922 2c0a 2020 2020  ": "array",.    
+000001c0: 2020 2269 7465 6d73 223a 207b 0a20 2020    "items": {.   
+000001d0: 2020 2020 2022 2472 6566 223a 2022 636c       "$ref": "cl
+000001e0: 6173 732e 6a73 6f6e 220a 2020 2020 2020  ass.json".      
+000001f0: 7d0a 2020 2020 7d2c 0a20 2020 2022 636c  }.    },.    "cl
+00000200: 6173 7367 726f 7570 223a 207b 0a20 2020  assgroup": {.   
+00000210: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+00000220: 6e67 220a 2020 2020 7d2c 0a20 2020 2022  ng".    },.    "
+00000230: 636c 6173 7369 7465 6d22 3a20 7b0a 2020  classitem": {.  
+00000240: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00000250: 696e 6722 0a20 2020 207d 2c0a 2020 2020  ing".    },.    
+00000260: 2263 6c75 7374 6572 223a 207b 0a20 2020  "cluster": {.   
+00000270: 2020 2022 616c 6c4f 6622 3a20 5b0a 2020     "allOf": [.  
+00000280: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000290: 2020 2224 7265 6622 3a20 2263 6c75 7374    "$ref": "clust
+000002a0: 6572 2e6a 736f 6e22 0a20 2020 2020 2020  er.json".       
+000002b0: 207d 0a20 2020 2020 205d 2c0a 2020 2020   }.      ],.    
+000002c0: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
+000002d0: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+000002e0: 696f 6e22 3a20 362e 300a 2020 2020 2020  ion": 6.0.      
+000002f0: 7d0a 2020 2020 7d2c 0a20 2020 2022 636f  }.    },.    "co
+00000300: 6d70 6f73 6974 6573 223a 207b 0a20 2020  mposites": {.   
+00000310: 2020 2022 7479 7065 223a 2022 6172 7261     "type": "arra
+00000320: 7922 2c0a 2020 2020 2020 2269 7465 6d73  y",.      "items
+00000330: 223a 207b 0a20 2020 2020 2020 2022 2472  ": {.        "$r
+00000340: 6566 223a 2022 636f 6d70 6f73 6974 652e  ef": "composite.
+00000350: 6a73 6f6e 220a 2020 2020 2020 7d2c 0a20  json".      },. 
+00000360: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
+00000370: 207b 0a20 2020 2020 2020 2022 6d69 6e56   {.        "minV
+00000380: 6572 7369 6f6e 223a 2037 2e30 0a20 2020  ersion": 7.0.   
+00000390: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+000003a0: 2263 6f6e 6e65 6374 696f 6e22 3a20 7b0a  "connection": {.
+000003b0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+000003c0: 7472 696e 6722 0a20 2020 207d 2c0a 2020  tring".    },.  
+000003d0: 2020 2263 6f6e 6e65 6374 696f 6e6f 7074    "connectionopt
+000003e0: 696f 6e73 223a 207b 0a20 2020 2020 2022  ions": {.      "
+000003f0: 616c 6c4f 6622 3a20 5b0a 2020 2020 2020  allOf": [.      
+00000400: 2020 7b0a 2020 2020 2020 2020 2020 2224    {.          "$
+00000410: 7265 6622 3a20 2263 6f6e 6e65 6374 696f  ref": "connectio
+00000420: 6e6f 7074 696f 6e73 2e6a 736f 6e22 0a20  noptions.json". 
+00000430: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00000440: 2c0a 2020 2020 2020 226d 6574 6164 6174  ,.      "metadat
+00000450: 6122 3a20 7b0a 2020 2020 2020 2020 226d  a": {.        "m
+00000460: 696e 5665 7273 696f 6e22 3a20 372e 360a  inVersion": 7.6.
+00000470: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000480: 2020 2022 636f 6e6e 6563 7469 6f6e 7479     "connectionty
+00000490: 7065 223a 207b 0a20 2020 2020 2022 656e  pe": {.      "en
+000004a0: 756d 223a 205b 2022 636f 6e74 6f75 7222  um": [ "contour"
+000004b0: 2c20 226b 6572 6e65 6c64 656e 7369 7479  , "kerneldensity
+000004c0: 222c 2022 6964 7722 2c20 226c 6f63 616c  ", "idw", "local
+000004d0: 222c 2022 6f67 7222 2c20 226f 7261 636c  ", "ogr", "oracl
+000004e0: 6573 7061 7469 616c 222c 2022 706c 7567  espatial", "plug
+000004f0: 696e 222c 2022 706f 7374 6769 7322 2c20  in", "postgis", 
+00000500: 2273 6465 222c 2022 756e 696f 6e22 2c20  "sde", "union", 
+00000510: 2275 7672 6173 7465 7222 2c20 2277 6673  "uvraster", "wfs
+00000520: 222c 2022 776d 7322 2c20 226d 7967 6973  ", "wms", "mygis
+00000530: 222c 2022 666c 6174 6765 6f62 7566 2220  ", "flatgeobuf" 
+00000540: 5d0a 2020 2020 7d2c 0a20 2020 2022 6461  ].    },.    "da
+00000550: 7461 223a 207b 0a20 2020 2020 2022 7479  ta": {.      "ty
+00000560: 7065 223a 2022 7374 7269 6e67 220a 2020  pe": "string".  
+00000570: 2020 7d2c 0a20 2020 2022 6465 6275 6722    },.    "debug"
+00000580: 3a20 7b0a 2020 2020 2020 2261 6c6c 4f66  : {.      "allOf
+00000590: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+000005a0: 2020 2020 2020 2020 2022 2472 6566 223a           "$ref":
+000005b0: 2022 6465 6275 672e 6a73 6f6e 220a 2020   "debug.json".  
+000005c0: 2020 2020 2020 7d0a 2020 2020 2020 5d2c        }.      ],
+000005d0: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
+000005e0: 223a 207b 0a20 2020 2020 2020 2022 6d69  ": {.        "mi
+000005f0: 6e56 6572 7369 6f6e 223a 2035 2e30 0a20  nVersion": 5.0. 
+00000600: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00000610: 2020 2264 756d 7022 3a20 7b0a 2020 2020    "dump": {.    
+00000620: 2020 226f 6e65 4f66 223a 205b 0a20 2020    "oneOf": [.   
+00000630: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000640: 2022 7479 7065 223a 2022 626f 6f6c 6561   "type": "boolea
+00000650: 6e22 0a20 2020 2020 2020 207d 2c0a 2020  n".        },.  
+00000660: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000670: 2020 2224 7265 6622 3a20 226f 6e6f 6666    "$ref": "onoff
+00000680: 2e6a 736f 6e22 0a20 2020 2020 2020 207d  .json".        }
+00000690: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
+000006a0: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
+000006b0: 2020 2020 2020 226d 6178 5665 7273 696f        "maxVersio
+000006c0: 6e22 3a20 372e 360a 2020 2020 2020 7d0a  n": 7.6.      }.
+000006d0: 2020 2020 7d2c 0a20 2020 2022 656e 636f      },.    "enco
+000006e0: 6469 6e67 223a 207b 0a20 2020 2020 2022  ding": {.      "
+000006f0: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
+00000700: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
+00000710: 223a 207b 0a20 2020 2020 2020 2022 6d69  ": {.        "mi
+00000720: 6e56 6572 7369 6f6e 223a 2037 2e30 0a20  nVersion": 7.0. 
+00000730: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00000740: 2020 2265 7874 656e 7422 3a20 7b0a 2020    "extent": {.  
+00000750: 2020 2020 2224 7265 6622 3a20 2265 7874      "$ref": "ext
+00000760: 656e 742e 6a73 6f6e 220a 2020 2020 7d2c  ent.json".    },
+00000770: 0a20 2020 2022 6665 6174 7572 6573 223a  .    "features":
+00000780: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00000790: 2022 6172 7261 7922 2c0a 2020 2020 2020   "array",.      
+000007a0: 2269 7465 6d73 223a 207b 0a20 2020 2020  "items": {.     
+000007b0: 2020 2022 2472 6566 223a 2022 6665 6174     "$ref": "feat
+000007c0: 7572 652e 6a73 6f6e 220a 2020 2020 2020  ure.json".      
+000007d0: 7d0a 2020 2020 7d2c 0a20 2020 2022 6669  }.    },.    "fi
+000007e0: 6c74 6572 223a 207b 0a20 2020 2020 2022  lter": {.      "
+000007f0: 2472 6566 223a 2022 6578 7072 6573 7369  $ref": "expressi
+00000800: 6f6e 2e6a 736f 6e22 0a20 2020 207d 2c0a  on.json".    },.
+00000810: 2020 2020 2266 696c 7465 7269 7465 6d22      "filteritem"
+00000820: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+00000830: 3a20 2273 7472 696e 6722 0a20 2020 207d  : "string".    }
+00000840: 2c0a 2020 2020 2266 6f6f 7465 7222 3a20  ,.    "footer": 
+00000850: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+00000860: 2273 7472 696e 6722 0a20 2020 207d 2c0a  "string".    },.
+00000870: 2020 2020 2267 656f 6d74 7261 6e73 666f      "geomtransfo
+00000880: 726d 223a 207b 0a20 2020 2020 2022 616e  rm": {.      "an
+00000890: 794f 6622 3a20 5b0a 2020 2020 2020 2020  yOf": [.        
+000008a0: 7b0a 2020 2020 2020 2020 2020 2274 7970  {.          "typ
+000008b0: 6522 3a20 2273 7472 696e 6722 0a20 2020  e": "string".   
+000008c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000008d0: 7b0a 2020 2020 2020 2020 2020 2274 7970  {.          "typ
+000008e0: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
+000008f0: 2020 2020 2020 2020 2270 6174 7465 726e          "pattern
+00000900: 223a 2022 5e5c 5c28 282e 2a3f 295c 5c29  ": "^\\((.*?)\\)
+00000910: 2422 0a20 2020 2020 2020 207d 0a20 2020  $".        }.   
+00000920: 2020 205d 2c0a 2020 2020 2020 226d 6574     ],.      "met
+00000930: 6164 6174 6122 3a20 7b0a 2020 2020 2020  adata": {.      
+00000940: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
+00000950: 362e 340a 2020 2020 2020 7d0a 2020 2020  6.4.      }.    
+00000960: 7d2c 0a20 2020 2022 6772 6964 223a 207b  },.    "grid": {
+00000970: 0a20 2020 2020 2022 2472 6566 223a 2022  .      "$ref": "
+00000980: 6772 6964 2e6a 736f 6e22 0a20 2020 207d  grid.json".    }
+00000990: 2c0a 2020 2020 2267 726f 7570 223a 207b  ,.    "group": {
+000009a0: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+000009b0: 7374 7269 6e67 220a 2020 2020 7d2c 0a20  string".    },. 
+000009c0: 2020 2022 6865 6164 6572 223a 207b 0a20     "header": {. 
+000009d0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+000009e0: 7269 6e67 220a 2020 2020 7d2c 0a20 2020  ring".    },.   
+000009f0: 2022 6a6f 696e 7322 3a20 7b0a 2020 2020   "joins": {.    
+00000a00: 2020 2274 7970 6522 3a20 2261 7272 6179    "type": "array
+00000a10: 222c 0a20 2020 2020 2022 6974 656d 7322  ",.      "items"
+00000a20: 3a20 7b0a 2020 2020 2020 2020 2224 7265  : {.        "$re
+00000a30: 6622 3a20 226a 6f69 6e2e 6a73 6f6e 220a  f": "join.json".
+00000a40: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000a50: 2020 2022 6c61 6265 6c61 6e67 6c65 6974     "labelangleit
+00000a60: 656d 223a 207b 0a20 2020 2020 2022 7479  em": {.      "ty
+00000a70: 7065 223a 2022 7374 7269 6e67 222c 0a20  pe": "string",. 
+00000a80: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
+00000a90: 207b 0a20 2020 2020 2020 2022 6d61 7856   {.        "maxV
+00000aa0: 6572 7369 6f6e 223a 2035 2e36 0a20 2020  ersion": 5.6.   
+00000ab0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+00000ac0: 226c 6162 656c 6361 6368 6522 3a20 7b0a  "labelcache": {.
+00000ad0: 2020 2020 2020 2224 7265 6622 3a20 226f        "$ref": "o
+00000ae0: 6e6f 6666 2e6a 736f 6e22 0a20 2020 207d  noff.json".    }
+00000af0: 2c0a 2020 2020 226c 6162 656c 6974 656d  ,.    "labelitem
+00000b00: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000b10: 223a 2022 7374 7269 6e67 220a 2020 2020  ": "string".    
+00000b20: 7d2c 0a20 2020 2022 6c61 6265 6c6d 6178  },.    "labelmax
+00000b30: 7363 616c 6522 3a20 7b0a 2020 2020 2020  scale": {.      
+00000b40: 2274 7970 6522 3a20 226e 756d 6265 7222  "type": "number"
+00000b50: 2c0a 2020 2020 2020 226d 6574 6164 6174  ,.      "metadat
+00000b60: 6122 3a20 7b0a 2020 2020 2020 2020 226d  a": {.        "m
+00000b70: 6178 5665 7273 696f 6e22 3a20 352e 300a  axVersion": 5.0.
+00000b80: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000b90: 2020 2022 6c61 6265 6c6d 696e 7363 616c     "labelminscal
+00000ba0: 6522 3a20 7b0a 2020 2020 2020 2274 7970  e": {.      "typ
+00000bb0: 6522 3a20 226e 756d 6265 7222 2c0a 2020  e": "number",.  
+00000bc0: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
+00000bd0: 7b0a 2020 2020 2020 2020 226d 6178 5665  {.        "maxVe
+00000be0: 7273 696f 6e22 3a20 352e 300a 2020 2020  rsion": 5.0.    
+00000bf0: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
+00000c00: 6c61 6265 6c6d 6178 7363 616c 6564 656e  labelmaxscaleden
+00000c10: 6f6d 223a 207b 0a20 2020 2020 2022 7479  om": {.      "ty
+00000c20: 7065 223a 2022 6e75 6d62 6572 222c 0a20  pe": "number",. 
+00000c30: 2020 2020 2022 6d69 6e69 6d75 6d22 3a20       "minimum": 
+00000c40: 302c 0a20 2020 2020 2022 6d65 7461 6461  0,.      "metada
+00000c50: 7461 223a 207b 0a20 2020 2020 2020 2022  ta": {.        "
+00000c60: 6d69 6e56 6572 7369 6f6e 223a 2035 2e30  minVersion": 5.0
+00000c70: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
+00000c80: 2020 2020 226c 6162 656c 6d69 6e73 6361      "labelminsca
+00000c90: 6c65 6465 6e6f 6d22 3a20 7b0a 2020 2020  ledenom": {.    
+00000ca0: 2020 2274 7970 6522 3a20 226e 756d 6265    "type": "numbe
+00000cb0: 7222 2c0a 2020 2020 2020 226d 696e 696d  r",.      "minim
+00000cc0: 756d 223a 2030 2c0a 2020 2020 2020 226d  um": 0,.      "m
+00000cd0: 6574 6164 6174 6122 3a20 7b0a 2020 2020  etadata": {.    
+00000ce0: 2020 2020 226d 696e 5665 7273 696f 6e22      "minVersion"
+00000cf0: 3a20 352e 300a 2020 2020 2020 7d0a 2020  : 5.0.      }.  
+00000d00: 2020 7d2c 0a20 2020 2022 6c61 6265 6c72    },.    "labelr
+00000d10: 6571 7569 7265 7322 3a20 7b0a 2020 2020  equires": {.    
+00000d20: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00000d30: 6722 0a20 2020 207d 2c0a 2020 2020 226c  g".    },.    "l
+00000d40: 6162 656c 7369 7a65 6974 656d 223a 207b  abelsizeitem": {
 00000d50: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-00000d60: 6e75 6d62 6572 222c 0d0a 2020 2020 2020  number",..      
-00000d70: 226d 696e 696d 756d 223a 2030 2c0d 0a20  "minimum": 0,.. 
-00000d80: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
-00000d90: 207b 0d0a 2020 2020 2020 2020 226d 696e   {..        "min
-00000da0: 5665 7273 696f 6e22 3a20 352e 300d 0a20  Version": 5.0.. 
-00000db0: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-00000dc0: 2020 2020 226c 6162 656c 7265 7175 6972      "labelrequir
-00000dd0: 6573 223a 207b 0d0a 2020 2020 2020 2274  es": {..      "t
-00000de0: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
-00000df0: 2020 2020 7d2c 0d0a 2020 2020 226c 6162      },..    "lab
-00000e00: 656c 7369 7a65 6974 656d 223a 207b 0d0a  elsizeitem": {..
-00000e10: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
-00000e20: 7472 696e 6722 2c0d 0a20 2020 2020 2022  tring",..      "
-00000e30: 6d65 7461 6461 7461 223a 207b 0d0a 2020  metadata": {..  
-00000e40: 2020 2020 2020 226d 6178 5665 7273 696f        "maxVersio
-00000e50: 6e22 3a20 352e 300d 0a20 2020 2020 207d  n": 5.0..      }
-00000e60: 0d0a 2020 2020 7d2c 0d0a 2020 2020 226d  ..    },..    "m
-00000e70: 6173 6b22 3a20 7b0d 0a20 2020 2020 2022  ask": {..      "
-00000e80: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
-00000e90: 0d0a 2020 2020 2020 226d 6574 6164 6174  ..      "metadat
-00000ea0: 6122 3a20 7b0d 0a20 2020 2020 2020 2022  a": {..        "
-00000eb0: 6d69 6e56 6572 7369 6f6e 223a 2036 2e32  minVersion": 6.2
-00000ec0: 0d0a 2020 2020 2020 7d0d 0a20 2020 207d  ..      }..    }
-00000ed0: 2c0d 0a20 2020 2022 6d61 7866 6561 7475  ,..    "maxfeatu
-00000ee0: 7265 7322 3a20 7b0d 0a20 2020 2020 2022  res": {..      "
-00000ef0: 7479 7065 223a 2022 696e 7465 6765 7222  type": "integer"
-00000f00: 2c0d 0a20 2020 2020 2022 6578 636c 7573  ,..      "exclus
-00000f10: 6976 654d 696e 696d 756d 223a 2030 0d0a  iveMinimum": 0..
-00000f20: 2020 2020 7d2c 0d0a 2020 2020 226d 6178      },..    "max
-00000f30: 6765 6f77 6964 7468 223a 207b 0d0a 2020  geowidth": {..  
-00000f40: 2020 2020 2274 7970 6522 3a20 226e 756d      "type": "num
-00000f50: 6265 7222 2c0d 0a20 2020 2020 2022 6578  ber",..      "ex
-00000f60: 636c 7573 6976 654d 696e 696d 756d 223a  clusiveMinimum":
-00000f70: 2030 2c0d 0a20 2020 2020 2022 6d65 7461   0,..      "meta
-00000f80: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000f90: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
-00000fa0: 352e 340d 0a20 2020 2020 207d 0d0a 2020  5.4..      }..  
-00000fb0: 2020 7d2c 0d0a 2020 2020 226d 6178 7363    },..    "maxsc
-00000fc0: 616c 6564 656e 6f6d 223a 207b 0d0a 2020  aledenom": {..  
-00000fd0: 2020 2020 2274 7970 6522 3a20 226e 756d      "type": "num
-00000fe0: 6265 7222 2c0d 0a20 2020 2020 2022 6d69  ber",..      "mi
-00000ff0: 6e69 6d75 6d22 3a20 302c 0d0a 2020 2020  nimum": 0,..    
-00001000: 2020 226d 6574 6164 6174 6122 3a20 7b0d    "metadata": {.
-00001010: 0a20 2020 2020 2020 2022 6d69 6e56 6572  .        "minVer
-00001020: 7369 6f6e 223a 2035 2e30 0d0a 2020 2020  sion": 5.0..    
-00001030: 2020 7d0d 0a20 2020 207d 2c0d 0a20 2020    }..    },..   
-00001040: 2022 6d61 7873 6361 6c65 223a 207b 0d0a   "maxscale": {..
-00001050: 2020 2020 2020 2274 7970 6522 3a20 226e        "type": "n
-00001060: 756d 6265 7222 2c0d 0a20 2020 2020 2022  umber",..      "
-00001070: 6d65 7461 6461 7461 223a 207b 0d0a 2020  metadata": {..  
-00001080: 2020 2020 2020 226d 6178 5665 7273 696f        "maxVersio
-00001090: 6e22 3a20 352e 300d 0a20 2020 2020 207d  n": 5.0..      }
-000010a0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 226d  ..    },..    "m
-000010b0: 6574 6164 6174 6122 3a20 7b0d 0a20 2020  etadata": {..   
-000010c0: 2020 2022 2472 6566 223a 2022 6d65 7461     "$ref": "meta
-000010d0: 6461 7461 2e6a 736f 6e22 0d0a 2020 2020  data.json"..    
-000010e0: 7d2c 0d0a 2020 2020 226d 696e 6665 6174  },..    "minfeat
-000010f0: 7572 6573 697a 6522 3a20 7b0d 0a20 2020  uresize": {..   
-00001100: 2020 2022 7479 7065 223a 2022 6e75 6d62     "type": "numb
-00001110: 6572 222c 0d0a 2020 2020 2020 2265 7863  er",..      "exc
-00001120: 6c75 7369 7665 4d69 6e69 6d75 6d22 3a20  lusiveMinimum": 
-00001130: 300d 0a20 2020 207d 2c0d 0a20 2020 2022  0..    },..    "
-00001140: 6d69 6e67 656f 7769 6474 6822 3a20 7b0d  mingeowidth": {.
-00001150: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-00001160: 6e75 6d62 6572 222c 0d0a 2020 2020 2020  number",..      
-00001170: 2265 7863 6c75 7369 7665 4d69 6e69 6d75  "exclusiveMinimu
-00001180: 6d22 3a20 302c 0d0a 2020 2020 2020 226d  m": 0,..      "m
-00001190: 6574 6164 6174 6122 3a20 7b0d 0a20 2020  etadata": {..   
-000011a0: 2020 2020 2022 6d69 6e56 6572 7369 6f6e       "minVersion
-000011b0: 223a 2035 2e34 0d0a 2020 2020 2020 7d0d  ": 5.4..      }.
-000011c0: 0a20 2020 207d 2c0d 0a20 2020 2022 6d69  .    },..    "mi
-000011d0: 6e73 6361 6c65 6465 6e6f 6d22 3a20 7b0d  nscaledenom": {.
-000011e0: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-000011f0: 6e75 6d62 6572 222c 0d0a 2020 2020 2020  number",..      
-00001200: 226d 696e 696d 756d 223a 2030 2c0d 0a20  "minimum": 0,.. 
-00001210: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
-00001220: 207b 0d0a 2020 2020 2020 2020 226d 696e   {..        "min
-00001230: 5665 7273 696f 6e22 3a20 352e 300d 0a20  Version": 5.0.. 
-00001240: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-00001250: 2020 2020 226d 696e 7363 616c 6522 3a20      "minscale": 
-00001260: 7b0d 0a20 2020 2020 2022 7479 7065 223a  {..      "type":
-00001270: 2022 6e75 6d62 6572 222c 0d0a 2020 2020   "number",..    
-00001280: 2020 226d 6574 6164 6174 6122 3a20 7b0d    "metadata": {.
-00001290: 0a20 2020 2020 2020 2022 6d61 7856 6572  .        "maxVer
-000012a0: 7369 6f6e 223a 2035 2e30 0d0a 2020 2020  sion": 5.0..    
-000012b0: 2020 7d0d 0a20 2020 207d 2c0d 0a20 2020    }..    },..   
-000012c0: 2022 6e61 6d65 223a 207b 0d0a 2020 2020   "name": {..    
-000012d0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-000012e0: 6722 0d0a 2020 2020 7d2c 0d0a 2020 2020  g"..    },..    
-000012f0: 226f 6666 7369 7465 223a 207b 0d0a 2020  "offsite": {..  
-00001300: 2020 2020 2224 7265 6622 3a20 2263 6f6c      "$ref": "col
-00001310: 6f72 2e6a 736f 6e22 0d0a 2020 2020 7d2c  or.json"..    },
-00001320: 0d0a 2020 2020 226f 7061 6369 7479 223a  ..    "opacity":
-00001330: 207b 0d0a 2020 2020 2020 2274 7970 6522   {..      "type"
-00001340: 3a20 2269 6e74 6567 6572 222c 0d0a 2020  : "integer",..  
-00001350: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-00001360: 7b0d 0a20 2020 2020 2020 2022 6d61 7856  {..        "maxV
-00001370: 6572 7369 6f6e 223a 2037 2e36 0d0a 2020  ersion": 7.6..  
-00001380: 2020 2020 7d0d 0a20 2020 207d 2c0d 0a20      }..    },.. 
-00001390: 2020 2022 706c 7567 696e 223a 207b 0d0a     "plugin": {..
-000013a0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
-000013b0: 7472 696e 6722 0d0a 2020 2020 7d2c 0d0a  tring"..    },..
-000013c0: 2020 2020 2270 6f73 746c 6162 656c 6361      "postlabelca
-000013d0: 6368 6522 3a20 7b0d 0a20 2020 2020 2022  che": {..      "
-000013e0: 7479 7065 223a 2022 626f 6f6c 6561 6e22  type": "boolean"
-000013f0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2270  ..    },..    "p
-00001400: 726f 6365 7373 696e 6722 3a20 7b0d 0a20  rocessing": {.. 
-00001410: 2020 2020 2022 7479 7065 223a 2022 6172       "type": "ar
-00001420: 7261 7922 2c0d 0a20 2020 2020 2022 6974  ray",..      "it
-00001430: 656d 7322 3a20 7b0d 0a20 2020 2020 2020  ems": {..       
-00001440: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-00001450: 220d 0a20 2020 2020 207d 0d0a 2020 2020  "..      }..    
-00001460: 7d2c 0d0a 2020 2020 2270 726f 6a65 6374  },..    "project
-00001470: 696f 6e22 3a20 7b0d 0a20 2020 2020 2022  ion": {..      "
-00001480: 2472 6566 223a 2022 7072 6f6a 6563 7469  $ref": "projecti
-00001490: 6f6e 2e6a 736f 6e22 0d0a 2020 2020 7d2c  on.json"..    },
-000014a0: 0d0a 2020 2020 2272 6571 7569 7265 7322  ..    "requires"
-000014b0: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-000014c0: 223a 2022 7374 7269 6e67 220d 0a20 2020  ": "string"..   
-000014d0: 207d 2c0d 0a20 2020 2022 7363 616c 6574   },..    "scalet
-000014e0: 6f6b 656e 7322 3a20 7b0d 0a20 2020 2020  okens": {..     
-000014f0: 2022 7479 7065 223a 2022 6172 7261 7922   "type": "array"
-00001500: 2c0d 0a20 2020 2020 2022 6974 656d 7322  ,..      "items"
-00001510: 3a20 7b0d 0a20 2020 2020 2020 2022 2472  : {..        "$r
-00001520: 6566 223a 2022 7363 616c 6574 6f6b 656e  ef": "scaletoken
-00001530: 2e6a 736f 6e22 0d0a 2020 2020 2020 7d2c  .json"..      },
-00001540: 0d0a 2020 2020 2020 226d 6574 6164 6174  ..      "metadat
-00001550: 6122 3a20 7b0d 0a20 2020 2020 2020 2022  a": {..        "
-00001560: 6d69 6e56 6572 7369 6f6e 223a 2036 2e34  minVersion": 6.4
-00001570: 0d0a 2020 2020 2020 7d0d 0a20 2020 207d  ..      }..    }
-00001580: 2c0d 0a20 2020 2022 7369 7a65 756e 6974  ,..    "sizeunit
-00001590: 7322 3a20 7b0d 0a20 2020 2020 2022 656e  s": {..      "en
-000015a0: 756d 223a 205b 2022 6665 6574 222c 2022  um": [ "feet", "
-000015b0: 696e 6368 6573 222c 2022 6b69 6c6f 6d65  inches", "kilome
-000015c0: 7465 7273 222c 2022 6d65 7465 7273 222c  ters", "meters",
-000015d0: 2022 6d69 6c65 7322 2c20 226e 6175 7469   "miles", "nauti
-000015e0: 6361 6c6d 696c 6573 222c 2022 7069 7865  calmiles", "pixe
-000015f0: 6c73 2220 5d0d 0a20 2020 207d 2c0d 0a20  ls" ]..    },.. 
-00001600: 2020 2022 7374 6174 7573 223a 207b 0d0a     "status": {..
-00001610: 2020 2020 2020 2264 6566 6175 6c74 223a        "default":
-00001620: 2022 6f66 6622 2c0d 0a20 2020 2020 2022   "off",..      "
-00001630: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
-00001640: 0d0a 2020 2020 2020 2265 6e75 6d22 3a20  ..      "enum": 
-00001650: 5b20 226f 6e22 2c20 226f 6666 222c 2022  [ "on", "off", "
-00001660: 6465 6661 756c 7422 205d 0d0a 2020 2020  default" ]..    
-00001670: 7d2c 0d0a 2020 2020 2273 7479 6c65 6974  },..    "styleit
-00001680: 656d 223a 207b 0d0a 2020 2020 2020 2274  em": {..      "t
-00001690: 7970 6522 3a20 2273 7472 696e 6722 0d0a  ype": "string"..
-000016a0: 2020 2020 7d2c 0d0a 2020 2020 2273 796d      },..    "sym
-000016b0: 626f 6c73 6361 6c65 6465 6e6f 6d22 3a20  bolscaledenom": 
-000016c0: 7b0d 0a20 2020 2020 2022 7479 7065 223a  {..      "type":
-000016d0: 2022 6e75 6d62 6572 222c 0d0a 2020 2020   "number",..    
-000016e0: 2020 226d 696e 696d 756d 223a 2031 2c0d    "minimum": 1,.
-000016f0: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
-00001700: 223a 207b 0d0a 2020 2020 2020 2020 226d  ": {..        "m
-00001710: 696e 5665 7273 696f 6e22 3a20 352e 300d  inVersion": 5.0.
-00001720: 0a20 2020 2020 207d 0d0a 2020 2020 7d2c  .      }..    },
-00001730: 0d0a 2020 2020 2274 656d 706c 6174 6522  ..    "template"
-00001740: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00001750: 223a 2022 7374 7269 6e67 220d 0a20 2020  ": "string"..   
-00001760: 207d 2c0d 0a20 2020 2022 7469 6c65 696e   },..    "tilein
-00001770: 6465 7822 3a20 7b0d 0a20 2020 2020 2022  dex": {..      "
-00001780: 7479 7065 223a 2022 7374 7269 6e67 220d  type": "string".
-00001790: 0a20 2020 207d 2c0d 0a20 2020 2022 7469  .    },..    "ti
-000017a0: 6c65 6974 656d 223a 207b 0d0a 2020 2020  leitem": {..    
-000017b0: 2020 2264 6566 6175 6c74 223a 2022 6c6f    "default": "lo
-000017c0: 6361 7469 6f6e 222c 0d0a 2020 2020 2020  cation",..      
-000017d0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-000017e0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2274  ..    },..    "t
-000017f0: 696c 6573 7273 223a 207b 0d0a 2020 2020  ilesrs": {..    
-00001800: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00001810: 6722 0d0a 2020 2020 7d2c 0d0a 2020 2020  g"..    },..    
-00001820: 2274 6f6c 6572 616e 6365 223a 207b 0d0a  "tolerance": {..
-00001830: 2020 2020 2020 2274 7970 6522 3a20 226e        "type": "n
-00001840: 756d 6265 7222 2c0d 0a20 2020 2020 2022  umber",..      "
-00001850: 6578 636c 7573 6976 654d 696e 696d 756d  exclusiveMinimum
-00001860: 223a 2030 0d0a 2020 2020 7d2c 0d0a 2020  ": 0..    },..  
-00001870: 2020 2274 6f6c 6572 616e 6365 756e 6974    "toleranceunit
-00001880: 7322 3a20 7b0d 0a20 2020 2020 2022 656e  s": {..      "en
-00001890: 756d 223a 205b 2022 7069 7865 6c73 222c  um": [ "pixels",
-000018a0: 2022 6665 6574 222c 2022 696e 6368 6573   "feet", "inches
-000018b0: 222c 2022 6b69 6c6f 6d65 7465 7273 222c  ", "kilometers",
-000018c0: 2022 6d65 7465 7273 222c 2022 6d69 6c65   "meters", "mile
-000018d0: 7322 2c20 226e 6175 7469 6361 6c6d 696c  s", "nauticalmil
-000018e0: 6573 222c 2022 6464 2220 5d0d 0a20 2020  es", "dd" ]..   
-000018f0: 207d 2c0d 0a20 2020 2022 7472 616e 7370   },..    "transp
-00001900: 6172 656e 6379 223a 207b 0d0a 2020 2020  arency": {..    
-00001910: 2020 226f 6e65 4f66 223a 205b 0d0a 2020    "oneOf": [..  
-00001920: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00001930: 2020 2022 7479 7065 223a 2022 696e 7465     "type": "inte
-00001940: 6765 7222 0d0a 2020 2020 2020 2020 7d2c  ger"..        },
-00001950: 0d0a 2020 2020 2020 2020 7b0d 0a20 2020  ..        {..   
-00001960: 2020 2020 2020 2022 656e 756d 223a 205b         "enum": [
-00001970: 2022 616c 7068 6122 205d 0d0a 2020 2020   "alpha" ]..    
-00001980: 2020 2020 7d0d 0a20 2020 2020 205d 2c0d      }..      ],.
-00001990: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
-000019a0: 223a 207b 0d0a 2020 2020 2020 2020 226d  ": {..        "m
-000019b0: 6178 5665 7273 696f 6e22 3a20 372e 360d  axVersion": 7.6.
-000019c0: 0a20 2020 2020 207d 0d0a 2020 2020 7d2c  .      }..    },
-000019d0: 0d0a 2020 2020 2274 7261 6e73 666f 726d  ..    "transform
-000019e0: 223a 207b 0d0a 2020 2020 2020 226f 6e65  ": {..      "one
-000019f0: 4f66 223a 205b 0d0a 2020 2020 2020 2020  Of": [..        
-00001a00: 7b0d 0a20 2020 2020 2020 2020 2022 7479  {..          "ty
-00001a10: 7065 223a 2022 626f 6f6c 6561 6e22 0d0a  pe": "boolean"..
-00001a20: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00001a30: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00001a40: 2022 2472 6566 223a 2022 706f 7369 7469   "$ref": "positi
-00001a50: 6f6e 2e6a 736f 6e22 0d0a 2020 2020 2020  on.json"..      
-00001a60: 2020 7d0d 0a20 2020 2020 205d 0d0a 2020    }..      ]..  
-00001a70: 2020 7d2c 0d0a 2020 2020 2274 7970 6522    },..    "type"
-00001a80: 3a20 7b0d 0a20 2020 2020 2022 656e 756d  : {..      "enum
-00001a90: 223a 205b 2022 6368 6172 7422 2c20 2263  ": [ "chart", "c
-00001aa0: 6972 636c 6522 2c20 226c 696e 6522 2c20  ircle", "line", 
-00001ab0: 2270 6f69 6e74 222c 2022 706f 6c79 676f  "point", "polygo
-00001ac0: 6e22 2c20 2272 6173 7465 7222 2c20 2271  n", "raster", "q
-00001ad0: 7565 7279 222c 2022 616e 6e6f 7461 7469  uery", "annotati
-00001ae0: 6f6e 222c 2022 7469 6c65 696e 6465 7822  on", "tileindex"
-00001af0: 205d 0d0a 2020 2020 7d2c 0d0a 2020 2020   ]..    },..    
-00001b00: 2275 6e69 7473 223a 207b 0d0a 2020 2020  "units": {..    
-00001b10: 2020 2264 6566 6175 6c74 223a 2022 6d65    "default": "me
-00001b20: 7465 7273 222c 0d0a 2020 2020 2020 2265  ters",..      "e
-00001b30: 6e75 6d22 3a20 5b20 2264 6422 2c20 2266  num": [ "dd", "f
-00001b40: 6565 7422 2c20 2269 6e63 6865 7322 2c20  eet", "inches", 
-00001b50: 226b 696c 6f6d 6574 6572 7322 2c20 226d  "kilometers", "m
-00001b60: 6574 6572 7322 2c20 226d 696c 6573 222c  eters", "miles",
-00001b70: 2022 6e61 7574 6963 616c 6d69 6c65 7322   "nauticalmiles"
-00001b80: 2c20 2270 6572 6365 6e74 6167 6573 222c  , "percentages",
-00001b90: 2022 7069 7865 6c73 2220 5d0d 0a20 2020   "pixels" ]..   
-00001ba0: 207d 2c0d 0a20 2020 2022 7574 6664 6174   },..    "utfdat
-00001bb0: 6122 3a20 7b0d 0a20 2020 2020 2022 7479  a": {..      "ty
-00001bc0: 7065 223a 2022 7374 7269 6e67 222c 0d0a  pe": "string",..
-00001bd0: 2020 2020 2020 226d 6574 6164 6174 6122        "metadata"
-00001be0: 3a20 7b0d 0a20 2020 2020 2020 2022 6d69  : {..        "mi
-00001bf0: 6e56 6572 7369 6f6e 223a 2037 2e30 0d0a  nVersion": 7.0..
-00001c00: 2020 2020 2020 7d0d 0a20 2020 207d 2c0d        }..    },.
-00001c10: 0a20 2020 2022 7574 6669 7465 6d22 3a20  .    "utfitem": 
-00001c20: 7b0d 0a20 2020 2020 2022 7479 7065 223a  {..      "type":
-00001c30: 2022 7374 7269 6e67 222c 0d0a 2020 2020   "string",..    
-00001c40: 2020 226d 6574 6164 6174 6122 3a20 7b0d    "metadata": {.
-00001c50: 0a20 2020 2020 2020 2022 6d69 6e56 6572  .        "minVer
-00001c60: 7369 6f6e 223a 2037 2e30 0d0a 2020 2020  sion": 7.0..    
-00001c70: 2020 7d0d 0a20 2020 207d 2c0d 0a20 2020    }..    },..   
-00001c80: 2022 7661 6c69 6461 7469 6f6e 223a 207b   "validation": {
-00001c90: 0d0a 2020 2020 2020 2224 7265 6622 3a20  ..      "$ref": 
-00001ca0: 2276 616c 6964 6174 696f 6e2e 6a73 6f6e  "validation.json
-00001cb0: 220d 0a20 2020 207d 0d0a 2020 7d0d 0a7d  "..    }..  }..}
-00001cc0: 0d0a                                     ..
+00000d60: 7374 7269 6e67 222c 0a20 2020 2020 2022  string",.      "
+00000d70: 6d65 7461 6461 7461 223a 207b 0a20 2020  metadata": {.   
+00000d80: 2020 2020 2022 6d61 7856 6572 7369 6f6e       "maxVersion
+00000d90: 223a 2035 2e30 0a20 2020 2020 207d 0a20  ": 5.0.      }. 
+00000da0: 2020 207d 2c0a 2020 2020 226d 6173 6b22     },.    "mask"
+00000db0: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+00000dc0: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
+00000dd0: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
+00000de0: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+00000df0: 696f 6e22 3a20 362e 320a 2020 2020 2020  ion": 6.2.      
+00000e00: 7d0a 2020 2020 7d2c 0a20 2020 2022 6d61  }.    },.    "ma
+00000e10: 7866 6561 7475 7265 7322 3a20 7b0a 2020  xfeatures": {.  
+00000e20: 2020 2020 2274 7970 6522 3a20 2269 6e74      "type": "int
+00000e30: 6567 6572 222c 0a20 2020 2020 2022 6578  eger",.      "ex
+00000e40: 636c 7573 6976 654d 696e 696d 756d 223a  clusiveMinimum":
+00000e50: 2030 0a20 2020 207d 2c0a 2020 2020 226d   0.    },.    "m
+00000e60: 6178 6765 6f77 6964 7468 223a 207b 0a20  axgeowidth": {. 
+00000e70: 2020 2020 2022 7479 7065 223a 2022 6e75       "type": "nu
+00000e80: 6d62 6572 222c 0a20 2020 2020 2022 6578  mber",.      "ex
+00000e90: 636c 7573 6976 654d 696e 696d 756d 223a  clusiveMinimum":
+00000ea0: 2030 2c0a 2020 2020 2020 226d 6574 6164   0,.      "metad
+00000eb0: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+00000ec0: 226d 696e 5665 7273 696f 6e22 3a20 352e  "minVersion": 5.
+00000ed0: 340a 2020 2020 2020 7d0a 2020 2020 7d2c  4.      }.    },
+00000ee0: 0a20 2020 2022 6d61 7873 6361 6c65 6465  .    "maxscalede
+00000ef0: 6e6f 6d22 3a20 7b0a 2020 2020 2020 2274  nom": {.      "t
+00000f00: 7970 6522 3a20 226e 756d 6265 7222 2c0a  ype": "number",.
+00000f10: 2020 2020 2020 226d 696e 696d 756d 223a        "minimum":
+00000f20: 2030 2c0a 2020 2020 2020 226d 6574 6164   0,.      "metad
+00000f30: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+00000f40: 226d 696e 5665 7273 696f 6e22 3a20 352e  "minVersion": 5.
+00000f50: 300a 2020 2020 2020 7d0a 2020 2020 7d2c  0.      }.    },
+00000f60: 0a20 2020 2022 6d61 7873 6361 6c65 223a  .    "maxscale":
+00000f70: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00000f80: 2022 6e75 6d62 6572 222c 0a20 2020 2020   "number",.     
+00000f90: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
+00000fa0: 2020 2020 2020 2022 6d61 7856 6572 7369         "maxVersi
+00000fb0: 6f6e 223a 2035 2e30 0a20 2020 2020 207d  on": 5.0.      }
+00000fc0: 0a20 2020 207d 2c0a 2020 2020 226d 6574  .    },.    "met
+00000fd0: 6164 6174 6122 3a20 7b0a 2020 2020 2020  adata": {.      
+00000fe0: 2224 7265 6622 3a20 226d 6574 6164 6174  "$ref": "metadat
+00000ff0: 612e 6a73 6f6e 220a 2020 2020 7d2c 0a20  a.json".    },. 
+00001000: 2020 2022 6d69 6e66 6561 7475 7265 7369     "minfeaturesi
+00001010: 7a65 223a 207b 0a20 2020 2020 2022 7479  ze": {.      "ty
+00001020: 7065 223a 2022 6e75 6d62 6572 222c 0a20  pe": "number",. 
+00001030: 2020 2020 2022 6578 636c 7573 6976 654d       "exclusiveM
+00001040: 696e 696d 756d 223a 2030 0a20 2020 207d  inimum": 0.    }
+00001050: 2c0a 2020 2020 226d 696e 6765 6f77 6964  ,.    "mingeowid
+00001060: 7468 223a 207b 0a20 2020 2020 2022 7479  th": {.      "ty
+00001070: 7065 223a 2022 6e75 6d62 6572 222c 0a20  pe": "number",. 
+00001080: 2020 2020 2022 6578 636c 7573 6976 654d       "exclusiveM
+00001090: 696e 696d 756d 223a 2030 2c0a 2020 2020  inimum": 0,.    
+000010a0: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
+000010b0: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+000010c0: 696f 6e22 3a20 352e 340a 2020 2020 2020  ion": 5.4.      
+000010d0: 7d0a 2020 2020 7d2c 0a20 2020 2022 6d69  }.    },.    "mi
+000010e0: 6e73 6361 6c65 6465 6e6f 6d22 3a20 7b0a  nscaledenom": {.
+000010f0: 2020 2020 2020 2274 7970 6522 3a20 226e        "type": "n
+00001100: 756d 6265 7222 2c0a 2020 2020 2020 226d  umber",.      "m
+00001110: 696e 696d 756d 223a 2030 2c0a 2020 2020  inimum": 0,.    
+00001120: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
+00001130: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+00001140: 696f 6e22 3a20 352e 300a 2020 2020 2020  ion": 5.0.      
+00001150: 7d0a 2020 2020 7d2c 0a20 2020 2022 6d69  }.    },.    "mi
+00001160: 6e73 6361 6c65 223a 207b 0a20 2020 2020  nscale": {.     
+00001170: 2022 7479 7065 223a 2022 6e75 6d62 6572   "type": "number
+00001180: 222c 0a20 2020 2020 2022 6d65 7461 6461  ",.      "metada
+00001190: 7461 223a 207b 0a20 2020 2020 2020 2022  ta": {.        "
+000011a0: 6d61 7856 6572 7369 6f6e 223a 2035 2e30  maxVersion": 5.0
+000011b0: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
+000011c0: 2020 2020 226e 616d 6522 3a20 7b0a 2020      "name": {.  
+000011d0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+000011e0: 696e 6722 0a20 2020 207d 2c0a 2020 2020  ing".    },.    
+000011f0: 226f 6666 7369 7465 223a 207b 0a20 2020  "offsite": {.   
+00001200: 2020 2022 2472 6566 223a 2022 636f 6c6f     "$ref": "colo
+00001210: 722e 6a73 6f6e 220a 2020 2020 7d2c 0a20  r.json".    },. 
+00001220: 2020 2022 6f70 6163 6974 7922 3a20 7b0a     "opacity": {.
+00001230: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
+00001240: 6e74 6567 6572 222c 0a20 2020 2020 2022  nteger",.      "
+00001250: 6d65 7461 6461 7461 223a 207b 0a20 2020  metadata": {.   
+00001260: 2020 2020 2022 6d61 7856 6572 7369 6f6e       "maxVersion
+00001270: 223a 2037 2e36 0a20 2020 2020 207d 0a20  ": 7.6.      }. 
+00001280: 2020 207d 2c0a 2020 2020 2270 6c75 6769     },.    "plugi
+00001290: 6e22 3a20 7b0a 2020 2020 2020 2274 7970  n": {.      "typ
+000012a0: 6522 3a20 2273 7472 696e 6722 0a20 2020  e": "string".   
+000012b0: 207d 2c0a 2020 2020 2270 6f73 746c 6162   },.    "postlab
+000012c0: 656c 6361 6368 6522 3a20 7b0a 2020 2020  elcache": {.    
+000012d0: 2020 2274 7970 6522 3a20 2262 6f6f 6c65    "type": "boole
+000012e0: 616e 220a 2020 2020 7d2c 0a20 2020 2022  an".    },.    "
+000012f0: 7072 6f63 6573 7369 6e67 223a 207b 0a20  processing": {. 
+00001300: 2020 2020 2022 7479 7065 223a 2022 6172       "type": "ar
+00001310: 7261 7922 2c0a 2020 2020 2020 2269 7465  ray",.      "ite
+00001320: 6d73 223a 207b 0a20 2020 2020 2020 2022  ms": {.        "
+00001330: 7479 7065 223a 2022 7374 7269 6e67 220a  type": "string".
+00001340: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00001350: 2020 2022 7072 6f6a 6563 7469 6f6e 223a     "projection":
+00001360: 207b 0a20 2020 2020 2022 2472 6566 223a   {.      "$ref":
+00001370: 2022 7072 6f6a 6563 7469 6f6e 2e6a 736f   "projection.jso
+00001380: 6e22 0a20 2020 207d 2c0a 2020 2020 2272  n".    },.    "r
+00001390: 6571 7569 7265 7322 3a20 7b0a 2020 2020  equires": {.    
+000013a0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+000013b0: 6722 0a20 2020 207d 2c0a 2020 2020 2273  g".    },.    "s
+000013c0: 6361 6c65 746f 6b65 6e73 223a 207b 0a20  caletokens": {. 
+000013d0: 2020 2020 2022 7479 7065 223a 2022 6172       "type": "ar
+000013e0: 7261 7922 2c0a 2020 2020 2020 2269 7465  ray",.      "ite
+000013f0: 6d73 223a 207b 0a20 2020 2020 2020 2022  ms": {.        "
+00001400: 2472 6566 223a 2022 7363 616c 6574 6f6b  $ref": "scaletok
+00001410: 656e 2e6a 736f 6e22 0a20 2020 2020 207d  en.json".      }
+00001420: 2c0a 2020 2020 2020 226d 6574 6164 6174  ,.      "metadat
+00001430: 6122 3a20 7b0a 2020 2020 2020 2020 226d  a": {.        "m
+00001440: 696e 5665 7273 696f 6e22 3a20 362e 340a  inVersion": 6.4.
+00001450: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00001460: 2020 2022 7369 7a65 756e 6974 7322 3a20     "sizeunits": 
+00001470: 7b0a 2020 2020 2020 2265 6e75 6d22 3a20  {.      "enum": 
+00001480: 5b20 2266 6565 7422 2c20 2269 6e63 6865  [ "feet", "inche
+00001490: 7322 2c20 226b 696c 6f6d 6574 6572 7322  s", "kilometers"
+000014a0: 2c20 226d 6574 6572 7322 2c20 226d 696c  , "meters", "mil
+000014b0: 6573 222c 2022 6e61 7574 6963 616c 6d69  es", "nauticalmi
+000014c0: 6c65 7322 2c20 2270 6978 656c 7322 205d  les", "pixels" ]
+000014d0: 0a20 2020 207d 2c0a 2020 2020 2273 7461  .    },.    "sta
+000014e0: 7475 7322 3a20 7b0a 2020 2020 2020 2264  tus": {.      "d
+000014f0: 6566 6175 6c74 223a 2022 6f66 6622 2c0a  efault": "off",.
+00001500: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+00001510: 7472 696e 6722 2c0a 2020 2020 2020 2265  tring",.      "e
+00001520: 6e75 6d22 3a20 5b20 226f 6e22 2c20 226f  num": [ "on", "o
+00001530: 6666 222c 2022 6465 6661 756c 7422 205d  ff", "default" ]
+00001540: 0a20 2020 207d 2c0a 2020 2020 2273 7479  .    },.    "sty
+00001550: 6c65 6974 656d 223a 207b 0a20 2020 2020  leitem": {.     
+00001560: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+00001570: 220a 2020 2020 7d2c 0a20 2020 2022 7379  ".    },.    "sy
+00001580: 6d62 6f6c 7363 616c 6564 656e 6f6d 223a  mbolscaledenom":
+00001590: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+000015a0: 2022 6e75 6d62 6572 222c 0a20 2020 2020   "number",.     
+000015b0: 2022 6d69 6e69 6d75 6d22 3a20 312c 0a20   "minimum": 1,. 
+000015c0: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
+000015d0: 207b 0a20 2020 2020 2020 2022 6d69 6e56   {.        "minV
+000015e0: 6572 7369 6f6e 223a 2035 2e30 0a20 2020  ersion": 5.0.   
+000015f0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+00001600: 2274 656d 706c 6174 6522 3a20 7b0a 2020  "template": {.  
+00001610: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00001620: 696e 6722 0a20 2020 207d 2c0a 2020 2020  ing".    },.    
+00001630: 2274 696c 6569 6e64 6578 223a 207b 0a20  "tileindex": {. 
+00001640: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00001650: 7269 6e67 220a 2020 2020 7d2c 0a20 2020  ring".    },.   
+00001660: 2022 7469 6c65 6974 656d 223a 207b 0a20   "tileitem": {. 
+00001670: 2020 2020 2022 6465 6661 756c 7422 3a20       "default": 
+00001680: 226c 6f63 6174 696f 6e22 2c0a 2020 2020  "location",.    
+00001690: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+000016a0: 6722 0a20 2020 207d 2c0a 2020 2020 2274  g".    },.    "t
+000016b0: 696c 6573 7273 223a 207b 0a20 2020 2020  ilesrs": {.     
+000016c0: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+000016d0: 220a 2020 2020 7d2c 0a20 2020 2022 746f  ".    },.    "to
+000016e0: 6c65 7261 6e63 6522 3a20 7b0a 2020 2020  lerance": {.    
+000016f0: 2020 2274 7970 6522 3a20 226e 756d 6265    "type": "numbe
+00001700: 7222 2c0a 2020 2020 2020 2265 7863 6c75  r",.      "exclu
+00001710: 7369 7665 4d69 6e69 6d75 6d22 3a20 300a  siveMinimum": 0.
+00001720: 2020 2020 7d2c 0a20 2020 2022 746f 6c65      },.    "tole
+00001730: 7261 6e63 6575 6e69 7473 223a 207b 0a20  ranceunits": {. 
+00001740: 2020 2020 2022 656e 756d 223a 205b 2022       "enum": [ "
+00001750: 7069 7865 6c73 222c 2022 6665 6574 222c  pixels", "feet",
+00001760: 2022 696e 6368 6573 222c 2022 6b69 6c6f   "inches", "kilo
+00001770: 6d65 7465 7273 222c 2022 6d65 7465 7273  meters", "meters
+00001780: 222c 2022 6d69 6c65 7322 2c20 226e 6175  ", "miles", "nau
+00001790: 7469 6361 6c6d 696c 6573 222c 2022 6464  ticalmiles", "dd
+000017a0: 2220 5d0a 2020 2020 7d2c 0a20 2020 2022  " ].    },.    "
+000017b0: 7472 616e 7370 6172 656e 6379 223a 207b  transparency": {
+000017c0: 0a20 2020 2020 2022 6f6e 654f 6622 3a20  .      "oneOf": 
+000017d0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+000017e0: 2020 2020 2020 2274 7970 6522 3a20 2269        "type": "i
+000017f0: 6e74 6567 6572 220a 2020 2020 2020 2020  nteger".        
+00001800: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00001810: 2020 2020 2020 2022 656e 756d 223a 205b         "enum": [
+00001820: 2022 616c 7068 6122 205d 0a20 2020 2020   "alpha" ].     
+00001830: 2020 207d 0a20 2020 2020 205d 2c0a 2020     }.      ],.  
+00001840: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
+00001850: 7b0a 2020 2020 2020 2020 226d 6178 5665  {.        "maxVe
+00001860: 7273 696f 6e22 3a20 372e 360a 2020 2020  rsion": 7.6.    
+00001870: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
+00001880: 7472 616e 7366 6f72 6d22 3a20 7b0a 2020  transform": {.  
+00001890: 2020 2020 226f 6e65 4f66 223a 205b 0a20      "oneOf": [. 
+000018a0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000018b0: 2020 2022 7479 7065 223a 2022 626f 6f6c     "type": "bool
+000018c0: 6561 6e22 0a20 2020 2020 2020 207d 2c0a  ean".        },.
+000018d0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000018e0: 2020 2020 2224 7265 6622 3a20 2270 6f73      "$ref": "pos
+000018f0: 6974 696f 6e2e 6a73 6f6e 220a 2020 2020  ition.json".    
+00001900: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
+00001910: 2020 7d2c 0a20 2020 2022 7479 7065 223a    },.    "type":
+00001920: 207b 0a20 2020 2020 2022 656e 756d 223a   {.      "enum":
+00001930: 205b 2022 6368 6172 7422 2c20 2263 6972   [ "chart", "cir
+00001940: 636c 6522 2c20 226c 696e 6522 2c20 2270  cle", "line", "p
+00001950: 6f69 6e74 222c 2022 706f 6c79 676f 6e22  oint", "polygon"
+00001960: 2c20 2272 6173 7465 7222 2c20 2271 7565  , "raster", "que
+00001970: 7279 222c 2022 616e 6e6f 7461 7469 6f6e  ry", "annotation
+00001980: 222c 2022 7469 6c65 696e 6465 7822 205d  ", "tileindex" ]
+00001990: 0a20 2020 207d 2c0a 2020 2020 2275 6e69  .    },.    "uni
+000019a0: 7473 223a 207b 0a20 2020 2020 2022 6465  ts": {.      "de
+000019b0: 6661 756c 7422 3a20 226d 6574 6572 7322  fault": "meters"
+000019c0: 2c0a 2020 2020 2020 2265 6e75 6d22 3a20  ,.      "enum": 
+000019d0: 5b20 2264 6422 2c20 2266 6565 7422 2c20  [ "dd", "feet", 
+000019e0: 2269 6e63 6865 7322 2c20 226b 696c 6f6d  "inches", "kilom
+000019f0: 6574 6572 7322 2c20 226d 6574 6572 7322  eters", "meters"
+00001a00: 2c20 226d 696c 6573 222c 2022 6e61 7574  , "miles", "naut
+00001a10: 6963 616c 6d69 6c65 7322 2c20 2270 6572  icalmiles", "per
+00001a20: 6365 6e74 6167 6573 222c 2022 7069 7865  centages", "pixe
+00001a30: 6c73 2220 5d0a 2020 2020 7d2c 0a20 2020  ls" ].    },.   
+00001a40: 2022 7574 6664 6174 6122 3a20 7b0a 2020   "utfdata": {.  
+00001a50: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+00001a60: 696e 6722 2c0a 2020 2020 2020 226d 6574  ing",.      "met
+00001a70: 6164 6174 6122 3a20 7b0a 2020 2020 2020  adata": {.      
+00001a80: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
+00001a90: 372e 300a 2020 2020 2020 7d0a 2020 2020  7.0.      }.    
+00001aa0: 7d2c 0a20 2020 2022 7574 6669 7465 6d22  },.    "utfitem"
+00001ab0: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+00001ac0: 3a20 2273 7472 696e 6722 2c0a 2020 2020  : "string",.    
+00001ad0: 2020 226d 6574 6164 6174 6122 3a20 7b0a    "metadata": {.
+00001ae0: 2020 2020 2020 2020 226d 696e 5665 7273          "minVers
+00001af0: 696f 6e22 3a20 372e 300a 2020 2020 2020  ion": 7.0.      
+00001b00: 7d0a 2020 2020 7d2c 0a20 2020 2022 7661  }.    },.    "va
+00001b10: 6c69 6461 7469 6f6e 223a 207b 0a20 2020  lidation": {.   
+00001b20: 2020 2022 2472 6566 223a 2022 7661 6c69     "$ref": "vali
+00001b30: 6461 7469 6f6e 2e6a 736f 6e22 0a20 2020  dation.json".   
+00001b40: 207d 0a20 207d 0a7d 0a                    }.  }.}.
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/leader.json` & `mappyfile-1.0.2/mappyfile/schemas/leader.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2270 726f 7065 7274 6965 7322  ..  "properties"
-00000080: 3a20 7b0d 0a20 2020 2022 5f5f 7479 7065  : {..    "__type
-00000090: 5f5f 223a 207b 0d0a 2020 2020 2020 2265  __": {..      "e
-000000a0: 6e75 6d22 3a20 5b20 226c 6561 6465 7222  num": [ "leader"
-000000b0: 205d 0d0a 2020 2020 7d2c 0d0a 2020 2020   ]..    },..    
-000000c0: 2269 6e63 6c75 6465 223a 207b 0d0a 2020  "include": {..  
-000000d0: 2020 2020 2274 7970 6522 3a20 2261 7272      "type": "arr
-000000e0: 6179 222c 0d0a 2020 2020 2020 2269 7465  ay",..      "ite
-000000f0: 6d73 223a 207b 0d0a 2020 2020 2020 2020  ms": {..        
-00000100: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00000110: 0d0a 2020 2020 2020 7d0d 0a20 2020 207d  ..      }..    }
-00000120: 2c0d 0a20 2020 2022 6772 6964 7374 6570  ,..    "gridstep
-00000130: 223a 207b 0d0a 2020 2020 2020 2274 7970  ": {..      "typ
-00000140: 6522 3a20 2269 6e74 6567 6572 222c 0d0a  e": "integer",..
-00000150: 2020 2020 2020 2265 7863 6c75 7369 7665        "exclusive
-00000160: 4d69 6e69 6d75 6d22 3a20 300d 0a20 2020  Minimum": 0..   
-00000170: 207d 2c0d 0a20 2020 2022 6d61 7864 6973   },..    "maxdis
-00000180: 7461 6e63 6522 3a20 7b0d 0a20 2020 2020  tance": {..     
-00000190: 2022 7479 7065 223a 2022 696e 7465 6765   "type": "intege
-000001a0: 7222 0d0a 2020 2020 7d2c 0d0a 2020 2020  r"..    },..    
-000001b0: 2273 7479 6c65 7322 3a20 7b0d 0a20 2020  "styles": {..   
-000001c0: 2020 2022 7479 7065 223a 2022 6172 7261     "type": "arra
-000001d0: 7922 2c0d 0a20 2020 2020 2022 6d69 6e49  y",..      "minI
-000001e0: 7465 6d73 223a 2031 2c0d 0a20 2020 2020  tems": 1,..     
-000001f0: 2022 6974 656d 7322 3a20 7b0d 0a20 2020   "items": {..   
-00000200: 2020 2020 2022 2472 6566 223a 2022 7374       "$ref": "st
-00000210: 796c 652e 6a73 6f6e 220d 0a20 2020 2020  yle.json"..     
-00000220: 207d 0d0a 2020 2020 7d0d 0a20 207d 0d0a   }..    }..  }..
-00000230: 7d0d 0a                                  }..
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2270  $": {}.  },.  "p
+00000070: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00000080: 2020 225f 5f74 7970 655f 5f22 3a20 7b0a    "__type__": {.
+00000090: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000000a0: 226c 6561 6465 7222 205d 0a20 2020 207d  "leader" ].    }
+000000b0: 2c0a 2020 2020 2269 6e63 6c75 6465 223a  ,.    "include":
+000000c0: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+000000d0: 2022 6172 7261 7922 2c0a 2020 2020 2020   "array",.      
+000000e0: 2269 7465 6d73 223a 207b 0a20 2020 2020  "items": {.     
+000000f0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+00000100: 6e67 220a 2020 2020 2020 7d0a 2020 2020  ng".      }.    
+00000110: 7d2c 0a20 2020 2022 6772 6964 7374 6570  },.    "gridstep
+00000120: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000130: 223a 2022 696e 7465 6765 7222 2c0a 2020  ": "integer",.  
+00000140: 2020 2020 2265 7863 6c75 7369 7665 4d69      "exclusiveMi
+00000150: 6e69 6d75 6d22 3a20 300a 2020 2020 7d2c  nimum": 0.    },
+00000160: 0a20 2020 2022 6d61 7864 6973 7461 6e63  .    "maxdistanc
+00000170: 6522 3a20 7b0a 2020 2020 2020 2274 7970  e": {.      "typ
+00000180: 6522 3a20 2269 6e74 6567 6572 220a 2020  e": "integer".  
+00000190: 2020 7d2c 0a20 2020 2022 7374 796c 6573    },.    "styles
+000001a0: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+000001b0: 223a 2022 6172 7261 7922 2c0a 2020 2020  ": "array",.    
+000001c0: 2020 226d 696e 4974 656d 7322 3a20 312c    "minItems": 1,
+000001d0: 0a20 2020 2020 2022 6974 656d 7322 3a20  .      "items": 
+000001e0: 7b0a 2020 2020 2020 2020 2224 7265 6622  {.        "$ref"
+000001f0: 3a20 2273 7479 6c65 2e6a 736f 6e22 0a20  : "style.json". 
+00000200: 2020 2020 207d 0a20 2020 207d 0a20 207d       }.    }.  }
+00000210: 0a7d 0a                                  .}.
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/querymap.json` & `mappyfile-1.0.2/mappyfile/schemas/querymap.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2270 726f 7065 7274 6965 7322  ..  "properties"
-00000080: 3a20 7b0d 0a20 2020 2022 5f5f 7479 7065  : {..    "__type
-00000090: 5f5f 223a 207b 0d0a 2020 2020 2020 2265  __": {..      "e
-000000a0: 6e75 6d22 3a20 5b20 2271 7565 7279 6d61  num": [ "queryma
-000000b0: 7022 205d 0d0a 2020 2020 7d2c 0d0a 2020  p" ]..    },..  
-000000c0: 2020 2269 6e63 6c75 6465 223a 207b 0d0a    "include": {..
-000000d0: 2020 2020 2020 2274 7970 6522 3a20 2261        "type": "a
-000000e0: 7272 6179 222c 0d0a 2020 2020 2020 2269  rray",..      "i
-000000f0: 7465 6d73 223a 207b 0d0a 2020 2020 2020  tems": {..      
-00000100: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
-00000110: 6722 0d0a 2020 2020 2020 7d0d 0a20 2020  g"..      }..   
-00000120: 207d 2c0d 0a20 2020 2022 636f 6c6f 7222   },..    "color"
-00000130: 3a20 7b0d 0a20 2020 2020 2022 2472 6566  : {..      "$ref
-00000140: 223a 2022 636f 6c6f 722e 6a73 6f6e 220d  ": "color.json".
-00000150: 0a20 2020 207d 2c0d 0a20 2020 2022 7369  .    },..    "si
-00000160: 7a65 223a 207b 0d0a 2020 2020 2020 2264  ze": {..      "d
-00000170: 6566 6175 6c74 223a 205b 202d 312c 202d  efault": [ -1, -
-00000180: 3120 5d2c 0d0a 2020 2020 2020 2274 7970  1 ],..      "typ
-00000190: 6522 3a20 2261 7272 6179 222c 0d0a 2020  e": "array",..  
-000001a0: 2020 2020 2269 7465 6d73 223a 207b 0d0a      "items": {..
-000001b0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-000001c0: 2269 6e74 6567 6572 222c 0d0a 2020 2020  "integer",..    
-000001d0: 2020 2020 226d 696e 696d 756d 223a 2020      "minimum":  
-000001e0: 2d31 0d0a 2020 2020 2020 7d2c 0d0a 2020  -1..      },..  
-000001f0: 2020 2020 226d 696e 4974 656d 7322 3a20      "minItems": 
-00000200: 322c 0d0a 2020 2020 2020 226d 6178 4974  2,..      "maxIt
-00000210: 656d 7322 3a20 320d 0a20 2020 207d 2c0d  ems": 2..    },.
-00000220: 0a20 2020 2022 7374 6174 7573 223a 207b  .    "status": {
-00000230: 0d0a 2020 2020 2020 2264 6566 6175 6c74  ..      "default
-00000240: 223a 2022 6f66 6622 2c0d 0a20 2020 2020  ": "off",..     
-00000250: 2022 2472 6566 223a 2022 6f6e 6f66 662e   "$ref": "onoff.
-00000260: 6a73 6f6e 220d 0a20 2020 207d 2c0d 0a20  json"..    },.. 
-00000270: 2020 2022 7374 796c 6522 3a20 7b0d 0a20     "style": {.. 
-00000280: 2020 2020 2022 6465 6661 756c 7422 3a20       "default": 
-00000290: 2268 696c 6974 6522 2c0d 0a20 2020 2020  "hilite",..     
-000002a0: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-000002b0: 222c 0d0a 2020 2020 2020 2265 6e75 6d22  ",..      "enum"
-000002c0: 3a20 5b20 226e 6f72 6d61 6c22 2c20 2268  : [ "normal", "h
-000002d0: 696c 6974 6522 2c20 2273 656c 6563 7465  ilite", "selecte
-000002e0: 6422 205d 2c0d 0a20 2020 2020 2022 6164  d" ],..      "ad
-000002f0: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
-00000300: 6573 223a 2066 616c 7365 0d0a 2020 2020  es": false..    
-00000310: 7d0d 0a20 207d 0d0a 7d0d 0a              }..  }..}..
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2270  $": {}.  },.  "p
+00000070: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00000080: 2020 225f 5f74 7970 655f 5f22 3a20 7b0a    "__type__": {.
+00000090: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000000a0: 2271 7565 7279 6d61 7022 205d 0a20 2020  "querymap" ].   
+000000b0: 207d 2c0a 2020 2020 2269 6e63 6c75 6465   },.    "include
+000000c0: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+000000d0: 223a 2022 6172 7261 7922 2c0a 2020 2020  ": "array",.    
+000000e0: 2020 2269 7465 6d73 223a 207b 0a20 2020    "items": {.   
+000000f0: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00000100: 7269 6e67 220a 2020 2020 2020 7d0a 2020  ring".      }.  
+00000110: 2020 7d2c 0a20 2020 2022 636f 6c6f 7222    },.    "color"
+00000120: 3a20 7b0a 2020 2020 2020 2224 7265 6622  : {.      "$ref"
+00000130: 3a20 2263 6f6c 6f72 2e6a 736f 6e22 0a20  : "color.json". 
+00000140: 2020 207d 2c0a 2020 2020 2273 697a 6522     },.    "size"
+00000150: 3a20 7b0a 2020 2020 2020 2264 6566 6175  : {.      "defau
+00000160: 6c74 223a 205b 202d 312c 202d 3120 5d2c  lt": [ -1, -1 ],
+00000170: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+00000180: 6172 7261 7922 2c0a 2020 2020 2020 2269  array",.      "i
+00000190: 7465 6d73 223a 207b 0a20 2020 2020 2020  tems": {.       
+000001a0: 2022 7479 7065 223a 2022 696e 7465 6765   "type": "intege
+000001b0: 7222 2c0a 2020 2020 2020 2020 226d 696e  r",.        "min
+000001c0: 696d 756d 223a 2020 2d31 0a20 2020 2020  imum":  -1.     
+000001d0: 207d 2c0a 2020 2020 2020 226d 696e 4974   },.      "minIt
+000001e0: 656d 7322 3a20 322c 0a20 2020 2020 2022  ems": 2,.      "
+000001f0: 6d61 7849 7465 6d73 223a 2032 0a20 2020  maxItems": 2.   
+00000200: 207d 2c0a 2020 2020 2273 7461 7475 7322   },.    "status"
+00000210: 3a20 7b0a 2020 2020 2020 2264 6566 6175  : {.      "defau
+00000220: 6c74 223a 2022 6f66 6622 2c0a 2020 2020  lt": "off",.    
+00000230: 2020 2224 7265 6622 3a20 226f 6e6f 6666    "$ref": "onoff
+00000240: 2e6a 736f 6e22 0a20 2020 207d 2c0a 2020  .json".    },.  
+00000250: 2020 2273 7479 6c65 223a 207b 0a20 2020    "style": {.   
+00000260: 2020 2022 6465 6661 756c 7422 3a20 2268     "default": "h
+00000270: 696c 6974 6522 2c0a 2020 2020 2020 2274  ilite",.      "t
+00000280: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+00000290: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000002a0: 226e 6f72 6d61 6c22 2c20 2268 696c 6974  "normal", "hilit
+000002b0: 6522 2c20 2273 656c 6563 7465 6422 205d  e", "selected" ]
+000002c0: 2c0a 2020 2020 2020 2261 6464 6974 696f  ,.      "additio
+000002d0: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+000002e0: 6661 6c73 650a 2020 2020 7d0a 2020 7d0a  false.    }.  }.
+000002f0: 7d0a                                     }.
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/reference.json` & `mappyfile-1.0.2/mappyfile/schemas/symbol.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8892045454545454%*

 * *Differences: {"'properties'": "{'__type__': {'enum': ['symbol']}, 'image': {delete: ['description']}, "*

 * *                 "'anchorpoint': OrderedDict([('type', 'array'), ('default', [0.5, 0.5]), "*

 * *                 "('items', [OrderedDict([('type', 'number'), ('minimum', 0), ('maximum', 1)])]), "*

 * *                 "('minItems', 2), ('maxItems', 2), ('metadata', OrderedDict([('minVersion', "*

 * *                 "6.2)]))]), 'antialias': OrderedDict([('type', 'boolean'), ('default', False), "*

 * *                 "('metadata', Order […]*

```diff
@@ -2,67 +2,96 @@
     "additionalProperties": false,
     "patternProperties": {
         "^__[a-z]+__$": {}
     },
     "properties": {
         "__type__": {
             "enum": [
-                "reference"
+                "symbol"
             ]
         },
-        "color": {
-            "$ref": "color.json"
-        },
-        "extent": {
-            "$ref": "extent.json"
-        },
-        "image": {
-            "description": "filename",
-            "type": "string"
-        },
-        "include": {
-            "items": {
-                "type": "string"
+        "anchorpoint": {
+            "default": [
+                0.5,
+                0.5
+            ],
+            "items": [
+                {
+                    "maximum": 1,
+                    "minimum": 0,
+                    "type": "number"
+                }
+            ],
+            "maxItems": 2,
+            "metadata": {
+                "minVersion": 6.2
             },
+            "minItems": 2,
             "type": "array"
         },
-        "marker": {
+        "antialias": {
+            "default": false,
+            "metadata": {
+                "maxVersion": 7.6
+            },
+            "type": "boolean"
+        },
+        "backgroundcolor": {
+            "$ref": "color.json"
+        },
+        "character": {
             "oneOf": [
                 {
-                    "minimum": 0,
-                    "type": "integer"
+                    "maxLength": 1,
+                    "minLength": 1,
+                    "type": "string"
                 },
                 {
+                    "example": "&#10140;",
+                    "pattern": "^&#[0-9]+;$",
                     "type": "string"
                 }
             ]
         },
-        "markersize": {
-            "exclusiveMinimum": 0,
-            "type": "integer"
-        },
-        "maxboxsize": {
-            "exclusiveMinimum": 0,
-            "type": "integer"
+        "filled": {
+            "default": false,
+            "type": "boolean"
         },
-        "minboxsize": {
-            "exclusiveMinimum": 0,
-            "type": "integer"
+        "font": {
+            "type": "string"
         },
-        "outlinecolor": {
-            "$ref": "color.json"
+        "image": {
+            "type": "string"
         },
-        "size": {
+        "include": {
             "items": {
-                "minimum": 5,
-                "type": "integer"
+                "type": "string"
             },
-            "maxItems": 2,
-            "minItems": 2,
             "type": "array"
         },
-        "status": {
-            "$ref": "onoff.json"
+        "name": {
+            "type": "string"
+        },
+        "points": {
+            "$ref": "points.json"
+        },
+        "transparent": {
+            "maximum": 255,
+            "metadata": {
+                "maxVersion": 7.6
+            },
+            "minimum": 0,
+            "type": "integer"
+        },
+        "type": {
+            "enum": [
+                "ellipse",
+                "hatch",
+                "pixmap",
+                "svg",
+                "truetype",
+                "vector"
+            ]
         }
     },
     "type": "object"
 }
```

### Comparing `mappyfile-1.0.1/mappyfile/schemas/web.json` & `mappyfile-1.0.2/mappyfile/schemas/web.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,128 @@
-00000000: 7b0d 0a20 2022 7479 7065 223a 2022 6f62  {..  "type": "ob
-00000010: 6a65 6374 222c 0d0a 2020 2261 6464 6974  ject",..  "addit
-00000020: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-00000030: 3a20 6661 6c73 652c 0d0a 2020 2270 6174  : false,..  "pat
-00000040: 7465 726e 5072 6f70 6572 7469 6573 223a  ternProperties":
-00000050: 207b 0d0a 2020 2020 225e 5f5f 5b61 2d7a   {..    "^__[a-z
-00000060: 5d2b 5f5f 2422 3a20 7b7d 0d0a 2020 7d2c  ]+__$": {}..  },
-00000070: 0d0a 2020 2270 726f 7065 7274 6965 7322  ..  "properties"
-00000080: 3a20 7b0d 0a20 2020 2022 5f5f 7479 7065  : {..    "__type
-00000090: 5f5f 223a 207b 0d0a 2020 2020 2020 2265  __": {..      "e
-000000a0: 6e75 6d22 3a20 5b20 2277 6562 2220 5d0d  num": [ "web" ].
-000000b0: 0a20 2020 207d 2c0d 0a20 2020 2022 696e  .    },..    "in
-000000c0: 636c 7564 6522 3a20 7b0d 0a20 2020 2020  clude": {..     
-000000d0: 2022 7479 7065 223a 2022 6172 7261 7922   "type": "array"
-000000e0: 2c0d 0a20 2020 2020 2022 6974 656d 7322  ,..      "items"
-000000f0: 3a20 7b0d 0a20 2020 2020 2020 2022 7479  : {..        "ty
-00000100: 7065 223a 2022 7374 7269 6e67 220d 0a20  pe": "string".. 
-00000110: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-00000120: 2020 2020 2262 726f 7773 6566 6f72 6d61      "browseforma
-00000130: 7422 3a20 7b0d 0a20 2020 2020 2022 7479  t": {..      "ty
-00000140: 7065 223a 2022 7374 7269 6e67 222c 0d0a  pe": "string",..
-00000150: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00000160: 6f6e 223a 2022 6d69 6d65 2d74 7970 6522  on": "mime-type"
-00000170: 2c0d 0a20 2020 2020 2022 6d65 7461 6461  ,..      "metada
-00000180: 7461 223a 207b 0d0a 2020 2020 2020 2020  ta": {..        
-00000190: 226d 696e 5665 7273 696f 6e22 3a20 342e  "minVersion": 4.
-000001a0: 380d 0a20 2020 2020 207d 0d0a 2020 2020  8..      }..    
-000001b0: 7d2c 0d0a 2020 2020 2265 6d70 7479 223a  },..    "empty":
-000001c0: 207b 0d0a 2020 2020 2020 2274 7970 6522   {..      "type"
-000001d0: 3a20 2273 7472 696e 6722 0d0a 2020 2020  : "string"..    
-000001e0: 7d2c 0d0a 2020 2020 2265 7272 6f72 223a  },..    "error":
-000001f0: 207b 0d0a 2020 2020 2020 2274 7970 6522   {..      "type"
-00000200: 3a20 2273 7472 696e 6722 0d0a 2020 2020  : "string"..    
-00000210: 7d2c 0d0a 2020 2020 2266 6f6f 7465 7222  },..    "footer"
-00000220: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000230: 223a 2022 7374 7269 6e67 222c 0d0a 2020  ": "string",..  
-00000240: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000250: 223a 2022 6669 6c65 6e61 6d65 220d 0a20  ": "filename".. 
-00000260: 2020 207d 2c0d 0a20 2020 2022 6865 6164     },..    "head
-00000270: 6572 223a 207b 0d0a 2020 2020 2020 2274  er": {..      "t
-00000280: 7970 6522 3a20 2273 7472 696e 6722 2c0d  ype": "string",.
-00000290: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
-000002a0: 696f 6e22 3a20 2266 696c 656e 616d 6522  ion": "filename"
-000002b0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2269  ..    },..    "i
-000002c0: 6d61 6765 7061 7468 223a 207b 0d0a 2020  magepath": {..  
-000002d0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
-000002e0: 696e 6722 2c0d 0a20 2020 2020 2022 6465  ing",..      "de
-000002f0: 7363 7269 7074 696f 6e22 3a20 2270 6174  scription": "pat
-00000300: 6822 0d0a 2020 2020 7d2c 0d0a 2020 2020  h"..    },..    
-00000310: 2269 6d61 6765 7572 6c22 3a20 7b0d 0a20  "imageurl": {.. 
-00000320: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
-00000330: 7269 6e67 222c 0d0a 2020 2020 2020 2264  ring",..      "d
-00000340: 6573 6372 6970 7469 6f6e 223a 2022 7572  escription": "ur
-00000350: 6c22 0d0a 2020 2020 7d2c 0d0a 2020 2020  l"..    },..    
-00000360: 226c 6567 656e 6466 6f72 6d61 7422 3a20  "legendformat": 
-00000370: 7b0d 0a20 2020 2020 2022 7479 7065 223a  {..      "type":
-00000380: 2022 7374 7269 6e67 222c 0d0a 2020 2020   "string",..    
-00000390: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000003a0: 2022 6d69 6d65 2d74 7970 6522 2c0d 0a20   "mime-type",.. 
-000003b0: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
-000003c0: 207b 0d0a 2020 2020 2020 2020 226d 696e   {..        "min
-000003d0: 5665 7273 696f 6e22 3a20 342e 380d 0a20  Version": 4.8.. 
-000003e0: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-000003f0: 2020 2020 226c 6f67 223a 207b 0d0a 2020      "log": {..  
-00000400: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
-00000410: 696e 6722 2c0d 0a20 2020 2020 2022 6465  ing",..      "de
-00000420: 7363 7269 7074 696f 6e22 3a20 2266 696c  scription": "fil
-00000430: 656e 616d 6522 2c0d 0a20 2020 2020 2022  ename",..      "
-00000440: 6d65 7461 6461 7461 223a 207b 0d0a 2020  metadata": {..  
-00000450: 2020 2020 2020 226d 6178 5665 7273 696f        "maxVersio
-00000460: 6e22 3a20 382e 300d 0a20 2020 2020 207d  n": 8.0..      }
-00000470: 0d0a 2020 2020 7d2c 0d0a 2020 2020 226d  ..    },..    "m
-00000480: 6178 7363 616c 6564 656e 6f6d 223a 207b  axscaledenom": {
-00000490: 0d0a 2020 2020 2020 2274 7970 6522 3a20  ..      "type": 
-000004a0: 226e 756d 6265 7222 2c0d 0a20 2020 2020  "number",..     
-000004b0: 2022 6d69 6e69 6d75 6d22 3a20 2030 2c0d   "minimum":  0,.
-000004c0: 0a20 2020 2020 2022 6d65 7461 6461 7461  .      "metadata
-000004d0: 223a 207b 0d0a 2020 2020 2020 2020 226d  ": {..        "m
-000004e0: 696e 5665 7273 696f 6e22 3a20 352e 300d  inVersion": 5.0.
-000004f0: 0a20 2020 2020 207d 0d0a 2020 2020 7d2c  .      }..    },
-00000500: 0d0a 2020 2020 226d 6178 7363 616c 6522  ..    "maxscale"
-00000510: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000520: 223a 2022 6e75 6d62 6572 222c 0d0a 2020  ": "number",..  
-00000530: 2020 2020 226d 6574 6164 6174 6122 3a20      "metadata": 
-00000540: 7b0d 0a20 2020 2020 2020 2022 6d61 7856  {..        "maxV
-00000550: 6572 7369 6f6e 223a 2037 2e36 0d0a 2020  ersion": 7.6..  
-00000560: 2020 2020 7d0d 0a20 2020 207d 2c0d 0a20      }..    },.. 
-00000570: 2020 2022 6d61 7874 656d 706c 6174 6522     "maxtemplate"
-00000580: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000590: 223a 2022 7374 7269 6e67 220d 0a20 2020  ": "string"..   
-000005a0: 207d 2c0d 0a20 2020 2022 6d65 7461 6461   },..    "metada
-000005b0: 7461 223a 207b 0d0a 2020 2020 2020 2224  ta": {..      "$
-000005c0: 7265 6622 3a20 226d 6574 6164 6174 612e  ref": "metadata.
-000005d0: 6a73 6f6e 220d 0a20 2020 207d 2c0d 0a20  json"..    },.. 
-000005e0: 2020 2022 6d69 6e73 6361 6c65 6465 6e6f     "minscaledeno
-000005f0: 6d22 3a20 7b0d 0a20 2020 2020 2022 7479  m": {..      "ty
-00000600: 7065 223a 2022 6e75 6d62 6572 222c 0d0a  pe": "number",..
-00000610: 2020 2020 2020 226d 696e 696d 756d 223a        "minimum":
-00000620: 2030 2c0d 0a20 2020 2020 2022 6d65 7461   0,..      "meta
-00000630: 6461 7461 223a 207b 0d0a 2020 2020 2020  data": {..      
-00000640: 2020 226d 696e 5665 7273 696f 6e22 3a20    "minVersion": 
-00000650: 352e 300d 0a20 2020 2020 207d 0d0a 2020  5.0..      }..  
-00000660: 2020 7d2c 0d0a 2020 2020 226d 696e 7363    },..    "minsc
-00000670: 616c 6522 3a20 7b0d 0a20 2020 2020 2022  ale": {..      "
-00000680: 7479 7065 223a 2022 6e75 6d62 6572 222c  type": "number",
-00000690: 0d0a 2020 2020 2020 226d 6574 6164 6174  ..      "metadat
-000006a0: 6122 3a20 7b0d 0a20 2020 2020 2020 2022  a": {..        "
-000006b0: 6d61 7856 6572 7369 6f6e 223a 2037 2e36  maxVersion": 7.6
-000006c0: 0d0a 2020 2020 2020 7d0d 0a20 2020 207d  ..      }..    }
-000006d0: 2c0d 0a20 2020 2022 6d69 6e74 656d 706c  ,..    "mintempl
-000006e0: 6174 6522 3a20 7b0d 0a20 2020 2020 2022  ate": {..      "
-000006f0: 7479 7065 223a 2022 7374 7269 6e67 220d  type": "string".
-00000700: 0a20 2020 207d 2c0d 0a20 2020 2022 7175  .    },..    "qu
-00000710: 6572 7966 6f72 6d61 7422 3a20 7b0d 0a20  eryformat": {.. 
-00000720: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
-00000730: 7269 6e67 222c 0d0a 2020 2020 2020 2264  ring",..      "d
-00000740: 6573 6372 6970 7469 6f6e 223a 2022 6d69  escription": "mi
-00000750: 6d65 2d74 7970 6522 0d0a 2020 2020 7d2c  me-type"..    },
-00000760: 0d0a 2020 2020 2274 656d 706c 6174 6522  ..    "template"
-00000770: 3a20 7b0d 0a20 2020 2020 2022 7479 7065  : {..      "type
-00000780: 223a 2022 7374 7269 6e67 220d 0a20 2020  ": "string"..   
-00000790: 207d 2c0d 0a20 2020 2022 7465 6d70 7061   },..    "temppa
-000007a0: 7468 223a 207b 0d0a 2020 2020 2020 2274  th": {..      "t
-000007b0: 7970 6522 3a20 2273 7472 696e 6722 2c0d  ype": "string",.
-000007c0: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
-000007d0: 696f 6e22 3a20 2270 6174 6822 2c0d 0a20  ion": "path",.. 
-000007e0: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
-000007f0: 207b 0d0a 2020 2020 2020 2020 226d 696e   {..        "min
-00000800: 5665 7273 696f 6e22 3a20 362e 300d 0a20  Version": 6.0.. 
-00000810: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
-00000820: 2020 2020 2276 616c 6964 6174 696f 6e22      "validation"
-00000830: 3a20 7b0d 0a20 2020 2020 2022 2472 6566  : {..      "$ref
-00000840: 223a 2022 7661 6c69 6461 7469 6f6e 2e6a  ": "validation.j
-00000850: 736f 6e22 0d0a 2020 2020 7d0d 0a20 207d  son"..    }..  }
-00000860: 0d0a 7d0d 0a                             ..}..
+00000000: 7b0a 2020 2274 7970 6522 3a20 226f 626a  {.  "type": "obj
+00000010: 6563 7422 2c0a 2020 2261 6464 6974 696f  ect",.  "additio
+00000020: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
+00000030: 6661 6c73 652c 0a20 2022 7061 7474 6572  false,.  "patter
+00000040: 6e50 726f 7065 7274 6965 7322 3a20 7b0a  nProperties": {.
+00000050: 2020 2020 225e 5f5f 5b61 2d7a 5d2b 5f5f      "^__[a-z]+__
+00000060: 2422 3a20 7b7d 0a20 207d 2c0a 2020 2270  $": {}.  },.  "p
+00000070: 726f 7065 7274 6965 7322 3a20 7b0a 2020  roperties": {.  
+00000080: 2020 225f 5f74 7970 655f 5f22 3a20 7b0a    "__type__": {.
+00000090: 2020 2020 2020 2265 6e75 6d22 3a20 5b20        "enum": [ 
+000000a0: 2277 6562 2220 5d0a 2020 2020 7d2c 0a20  "web" ].    },. 
+000000b0: 2020 2022 696e 636c 7564 6522 3a20 7b0a     "include": {.
+000000c0: 2020 2020 2020 2274 7970 6522 3a20 2261        "type": "a
+000000d0: 7272 6179 222c 0a20 2020 2020 2022 6974  rray",.      "it
+000000e0: 656d 7322 3a20 7b0a 2020 2020 2020 2020  ems": {.        
+000000f0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00000100: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
+00000110: 2020 2020 2262 726f 7773 6566 6f72 6d61      "browseforma
+00000120: 7422 3a20 7b0a 2020 2020 2020 2274 7970  t": {.      "typ
+00000130: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
+00000140: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000150: 223a 2022 6d69 6d65 2d74 7970 6522 2c0a  ": "mime-type",.
+00000160: 2020 2020 2020 226d 6574 6164 6174 6122        "metadata"
+00000170: 3a20 7b0a 2020 2020 2020 2020 226d 696e  : {.        "min
+00000180: 5665 7273 696f 6e22 3a20 342e 380a 2020  Version": 4.8.  
+00000190: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
+000001a0: 2022 656d 7074 7922 3a20 7b0a 2020 2020   "empty": {.    
+000001b0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+000001c0: 6722 0a20 2020 207d 2c0a 2020 2020 2265  g".    },.    "e
+000001d0: 7272 6f72 223a 207b 0a20 2020 2020 2022  rror": {.      "
+000001e0: 7479 7065 223a 2022 7374 7269 6e67 220a  type": "string".
+000001f0: 2020 2020 7d2c 0a20 2020 2022 666f 6f74      },.    "foot
+00000200: 6572 223a 207b 0a20 2020 2020 2022 7479  er": {.      "ty
+00000210: 7065 223a 2022 7374 7269 6e67 222c 0a20  pe": "string",. 
+00000220: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00000230: 6e22 3a20 2266 696c 656e 616d 6522 0a20  n": "filename". 
+00000240: 2020 207d 2c0a 2020 2020 2268 6561 6465     },.    "heade
+00000250: 7222 3a20 7b0a 2020 2020 2020 2274 7970  r": {.      "typ
+00000260: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
+00000270: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000280: 223a 2022 6669 6c65 6e61 6d65 220a 2020  ": "filename".  
+00000290: 2020 7d2c 0a20 2020 2022 696d 6167 6570    },.    "imagep
+000002a0: 6174 6822 3a20 7b0a 2020 2020 2020 2274  ath": {.      "t
+000002b0: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+000002c0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000002d0: 6f6e 223a 2022 7061 7468 220a 2020 2020  on": "path".    
+000002e0: 7d2c 0a20 2020 2022 696d 6167 6575 726c  },.    "imageurl
+000002f0: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000300: 223a 2022 7374 7269 6e67 222c 0a20 2020  ": "string",.   
+00000310: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000320: 3a20 2275 726c 220a 2020 2020 7d2c 0a20  : "url".    },. 
+00000330: 2020 2022 6c65 6765 6e64 666f 726d 6174     "legendformat
+00000340: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00000350: 223a 2022 7374 7269 6e67 222c 0a20 2020  ": "string",.   
+00000360: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000370: 3a20 226d 696d 652d 7479 7065 222c 0a20  : "mime-type",. 
+00000380: 2020 2020 2022 6d65 7461 6461 7461 223a       "metadata":
+00000390: 207b 0a20 2020 2020 2020 2022 6d69 6e56   {.        "minV
+000003a0: 6572 7369 6f6e 223a 2034 2e38 0a20 2020  ersion": 4.8.   
+000003b0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
+000003c0: 226c 6f67 223a 207b 0a20 2020 2020 2022  "log": {.      "
+000003d0: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
+000003e0: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
+000003f0: 696f 6e22 3a20 2266 696c 656e 616d 6522  ion": "filename"
+00000400: 2c0a 2020 2020 2020 226d 6574 6164 6174  ,.      "metadat
+00000410: 6122 3a20 7b0a 2020 2020 2020 2020 226d  a": {.        "m
+00000420: 6178 5665 7273 696f 6e22 3a20 382e 300a  axVersion": 8.0.
+00000430: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000440: 2020 2022 6d61 7873 6361 6c65 6465 6e6f     "maxscaledeno
+00000450: 6d22 3a20 7b0a 2020 2020 2020 2274 7970  m": {.      "typ
+00000460: 6522 3a20 226e 756d 6265 7222 2c0a 2020  e": "number",.  
+00000470: 2020 2020 226d 696e 696d 756d 223a 2020      "minimum":  
+00000480: 302c 0a20 2020 2020 2022 6d65 7461 6461  0,.      "metada
+00000490: 7461 223a 207b 0a20 2020 2020 2020 2022  ta": {.        "
+000004a0: 6d69 6e56 6572 7369 6f6e 223a 2035 2e30  minVersion": 5.0
+000004b0: 0a20 2020 2020 207d 0a20 2020 207d 2c0a  .      }.    },.
+000004c0: 2020 2020 226d 6178 7363 616c 6522 3a20      "maxscale": 
+000004d0: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+000004e0: 226e 756d 6265 7222 2c0a 2020 2020 2020  "number",.      
+000004f0: 226d 6574 6164 6174 6122 3a20 7b0a 2020  "metadata": {.  
+00000500: 2020 2020 2020 226d 6178 5665 7273 696f        "maxVersio
+00000510: 6e22 3a20 372e 360a 2020 2020 2020 7d0a  n": 7.6.      }.
+00000520: 2020 2020 7d2c 0a20 2020 2022 6d61 7874      },.    "maxt
+00000530: 656d 706c 6174 6522 3a20 7b0a 2020 2020  emplate": {.    
+00000540: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00000550: 6722 0a20 2020 207d 2c0a 2020 2020 226d  g".    },.    "m
+00000560: 6574 6164 6174 6122 3a20 7b0a 2020 2020  etadata": {.    
+00000570: 2020 2224 7265 6622 3a20 226d 6574 6164    "$ref": "metad
+00000580: 6174 612e 6a73 6f6e 220a 2020 2020 7d2c  ata.json".    },
+00000590: 0a20 2020 2022 6d69 6e73 6361 6c65 6465  .    "minscalede
+000005a0: 6e6f 6d22 3a20 7b0a 2020 2020 2020 2274  nom": {.      "t
+000005b0: 7970 6522 3a20 226e 756d 6265 7222 2c0a  ype": "number",.
+000005c0: 2020 2020 2020 226d 696e 696d 756d 223a        "minimum":
+000005d0: 2030 2c0a 2020 2020 2020 226d 6574 6164   0,.      "metad
+000005e0: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+000005f0: 226d 696e 5665 7273 696f 6e22 3a20 352e  "minVersion": 5.
+00000600: 300a 2020 2020 2020 7d0a 2020 2020 7d2c  0.      }.    },
+00000610: 0a20 2020 2022 6d69 6e73 6361 6c65 223a  .    "minscale":
+00000620: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00000630: 2022 6e75 6d62 6572 222c 0a20 2020 2020   "number",.     
+00000640: 2022 6d65 7461 6461 7461 223a 207b 0a20   "metadata": {. 
+00000650: 2020 2020 2020 2022 6d61 7856 6572 7369         "maxVersi
+00000660: 6f6e 223a 2037 2e36 0a20 2020 2020 207d  on": 7.6.      }
+00000670: 0a20 2020 207d 2c0a 2020 2020 226d 696e  .    },.    "min
+00000680: 7465 6d70 6c61 7465 223a 207b 0a20 2020  template": {.   
+00000690: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+000006a0: 6e67 220a 2020 2020 7d2c 0a20 2020 2022  ng".    },.    "
+000006b0: 7175 6572 7966 6f72 6d61 7422 3a20 7b0a  queryformat": {.
+000006c0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+000006d0: 7472 696e 6722 2c0a 2020 2020 2020 2264  tring",.      "d
+000006e0: 6573 6372 6970 7469 6f6e 223a 2022 6d69  escription": "mi
+000006f0: 6d65 2d74 7970 6522 0a20 2020 207d 2c0a  me-type".    },.
+00000700: 2020 2020 2274 656d 706c 6174 6522 3a20      "template": 
+00000710: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+00000720: 2273 7472 696e 6722 0a20 2020 207d 2c0a  "string".    },.
+00000730: 2020 2020 2274 656d 7070 6174 6822 3a20      "temppath": 
+00000740: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+00000750: 2273 7472 696e 6722 2c0a 2020 2020 2020  "string",.      
+00000760: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00000770: 7061 7468 222c 0a20 2020 2020 2022 6d65  path",.      "me
+00000780: 7461 6461 7461 223a 207b 0a20 2020 2020  tadata": {.     
+00000790: 2020 2022 6d69 6e56 6572 7369 6f6e 223a     "minVersion":
+000007a0: 2036 2e30 0a20 2020 2020 207d 0a20 2020   6.0.      }.   
+000007b0: 207d 2c0a 2020 2020 2276 616c 6964 6174   },.    "validat
+000007c0: 696f 6e22 3a20 7b0a 2020 2020 2020 2224  ion": {.      "$
+000007d0: 7265 6622 3a20 2276 616c 6964 6174 696f  ref": "validatio
+000007e0: 6e2e 6a73 6f6e 220a 2020 2020 7d0a 2020  n.json".    }.  
+000007f0: 7d0a 7d0a                                }.}.
```

### Comparing `mappyfile-1.0.1/mappyfile/transformer.py` & `mappyfile-1.0.2/mappyfile/transformer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,774 +1,774 @@
-# =================================================================
-#
-# Authors: Erez Shinan, Seth Girvin
-#
-# Copyright (c) 2020 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-"""
-Module to transform an AST (Abstract Syntax Tree) to a
-Python dict structure
-"""
-
-from __future__ import annotations
-import logging
-from collections import OrderedDict
-from lark import Tree
-from lark.visitors import Transformer_InPlace, Transformer, v_args
-from lark.lexer import Token
-from .parser import lark_cython
-from typing import Any
-from mappyfile.tokens import SINGLETON_COMPOSITE_NAMES, REPEATED_KEYS
-from mappyfile.ordereddict import CaseInsensitiveOrderedDict
-from mappyfile.quoter import Quoter
-
-
-if lark_cython:
-    TOKEN_TYPES = (Token, lark_cython.Token)
-
-    def update_token_value(t, value):
-        return Token.new_borrow_pos(t.type, value, t)
-
-else:
-    TOKEN_TYPES = Token  # type: ignore
-
-    def update_token_value(t, value):
-        t.value = value
-        return t
-
-
-log = logging.getLogger("mappyfile")
-
-
-class MapfileTransformer(Transformer):
-    def __init__(self, include_position: bool = False, include_comments: bool = False):
-        self.quoter = Quoter()
-        self.include_position = include_position
-        self.include_comments = include_comments
-
-    def key_name(self, token) -> str:
-        return token.value.lower()
-
-    def start(self, composites):
-        """
-        Parses a MapServer Mapfile
-        Parsing of partial Mapfiles or lists of composites is also possible
-        """
-
-        # only return a list when there are multiple root composites (e.g.
-        # several CLASSes)
-        if len(composites) == 1:
-            return composites[0]
-
-        return composites
-
-    def flatten(self, values: list[Any]) -> list[Any]:
-        flat_list = []
-
-        for v in values:
-            if isinstance(v, TOKEN_TYPES):
-                flat_list.append(v)
-            elif isinstance(v, list):
-                flat_list += v
-            elif isinstance(v, tuple):
-                flat_list += v
-            elif isinstance(v, dict):
-                assert "__tokens__" in v
-                flat_list += v["__tokens__"]
-            else:
-                raise ValueError("Attribute value type not supported", v)
-
-        return flat_list
-
-    def plural(self, s: str) -> str:
-        if s.endswith("s"):
-            return s + "es"
-
-        return s + "s"
-
-    def create_position_dict(self, key_token, values) -> dict:
-        line, column = key_token.line, key_token.column
-        d = OrderedDict()
-        d["line"] = line
-        d["column"] = column
-
-        if values:
-            flat_list = self.flatten(values)
-            value_positions = [(v.line, v.column) for v in flat_list]
-            d["values"] = value_positions
-
-        return d
-
-    def get_single_key(self, d: dict):
-        keys = list(d.keys())  # convert to list for py3
-        assert len(keys) == 1
-        return keys[0]
-
-    def composite_body(self, t):
-        return t
-
-    def composite_type(self, t):
-        return t
-
-    def _process_composite_config(
-        self,
-        composite_dict: dict,
-        attribute_dict: dict,
-        position_dict: (dict | None),
-        pos: int,
-    ):
-        key_name = "config"
-
-        # there may be several config dicts - one for each setting
-        if key_name not in composite_dict:
-            # create an initial OrderedDict
-            composite_dict[key_name] = CaseInsensitiveOrderedDict(
-                CaseInsensitiveOrderedDict
-            )
-        # populate the existing config dict
-        cfg_dict = composite_dict[key_name]
-        cfg_dict.update(attribute_dict[key_name])
-
-        if position_dict is not None:
-            if key_name not in position_dict:
-                position_dict[key_name] = OrderedDict()
-
-            subkey_name = self.get_single_key(attribute_dict[key_name])
-            position_dict[key_name][subkey_name] = pos
-
-    def _process_composite_points(
-        self,
-        composite_dict: dict,
-        attribute_dict: dict,
-        position_dict: (dict | None),
-        pos: int,
-    ):
-        key_name = "points"
-
-        if key_name not in composite_dict:
-            composite_dict[key_name] = attribute_dict[key_name]
-        else:
-            # if points are already in a feature then
-            # allow for multipart features in a nested list
-            existing_points = composite_dict[key_name]
-
-            if calculate_depth(existing_points) == 2:
-                composite_dict[key_name] = [existing_points]
-
-            if key_name not in composite_dict:
-                composite_dict[key_name] = []
-            composite_dict[key_name].append(attribute_dict[key_name])
-
-        if position_dict is not None:
-            if key_name not in position_dict:
-                position_dict[key_name] = pos
-            else:
-                existing_pos = position_dict[key_name]
-                if isinstance(existing_pos, dict):
-                    position_dict[key_name] = [existing_pos]
-                position_dict[key_name].append(pos)
-
-    def composite(self, t):
-        """
-        Handle the composite types e.g. CLASS..END
-        t is a list in the form [[Token(__LAYER36, 'LAYER')], [OrderedDict([...])]]
-
-        """
-        if len(t) == 1:
-            return t[0]  # metadata and values - already processed
-
-        key_token = t[0][0]
-        attribute_dicts = t[1]
-
-        if not isinstance(attribute_dicts, list):
-            # always handle a list of attributes
-            attribute_dicts = [attribute_dicts]
-
-        key_name = self.key_name(key_token)
-        composite_dict = CaseInsensitiveOrderedDict(CaseInsensitiveOrderedDict)
-        composite_dict["__type__"] = key_name
-
-        if self.include_position:
-            position_dict = self.create_position_dict(key_token, None)
-            composite_dict["__position__"] = position_dict
-        else:
-            position_dict = None
-
-        if self.include_comments:
-            comments_dict = composite_dict["__comments__"] = OrderedDict()
-
-        for d in attribute_dicts:
-            keys = d.keys()
-            if "__type__" in keys:
-                k = d["__type__"]
-                if k in SINGLETON_COMPOSITE_NAMES:
-                    composite_dict[k] = d
-                else:
-                    plural_key = self.plural(k)
-                    if plural_key not in composite_dict:
-                        composite_dict[plural_key] = []
-
-                    composite_dict[plural_key].append(d)
-            else:
-                #  simple attribute
-                pos = d.pop("__position__")
-                d.pop(
-                    "__tokens__", None
-                )  # tokens are no longer needed now we have the positions
-                comments = d.pop("__comments__", None)
-
-                key_name = self.get_single_key(d)
-
-                if key_name == "config":
-                    self._process_composite_config(
-                        composite_dict, d, position_dict, pos
-                    )
-                elif key_name == "points":
-                    self._process_composite_points(
-                        composite_dict, d, position_dict, pos
-                    )
-                elif key_name in REPEATED_KEYS:
-                    if key_name not in composite_dict:
-                        composite_dict[key_name] = []
-
-                    composite_dict[key_name].append(d[key_name])
-
-                    if position_dict:
-                        if key_name not in position_dict:
-                            position_dict[key_name] = []
-                        position_dict[key_name].append(pos)
-                else:
-                    assert len(d.items()) == 1
-                    if position_dict:
-                        # hoist position details to composite
-                        position_dict[key_name] = pos
-                    if self.include_comments and comments:
-                        # hoist comments to composite
-                        comments_dict[key_name] = comments
-
-                    composite_dict[key_name] = d[key_name]
-
-        return composite_dict
-
-    def clean_string(self, val: str) -> str:
-        return self.quoter.remove_quotes(val)
-
-    def attr_name(self, tokens) -> str:
-        t = tokens[0]
-        if not isinstance(t, TOKEN_TYPES):
-            #  handle ambiguities
-            t = t[0]
-            assert t.value.lower() in ("symbol", "style")
-
-        return t
-
-    def attr(self, tokens) -> dict:
-        key_token = tokens[0]
-
-        if isinstance(key_token, (list, tuple)):
-            key_token = key_token[0]
-            assert self.key_name(key_token) in ("style", "symbol"), self.key_name(
-                key_token
-            )
-
-        key_name = self.key_name(key_token)
-        value_tokens = tokens[1:]
-
-        if isinstance(value_tokens[0], (list, tuple)):
-            # for any multi-part attributes they will be lists or tuples
-            # e.g. int_pair, rgb etc.
-            assert len(value_tokens) == 1
-            value_tokens = value_tokens[0]
-
-        pd = self.create_position_dict(key_token, value_tokens)
-        d: dict = OrderedDict()
-        d["__position__"] = pd
-
-        if len(value_tokens) > 1:
-            if key_name == "config":
-                assert len(value_tokens) == 2
-                values = {value_tokens[0].value: value_tokens[1].value}
-            else:
-                # list of values
-                values = [v.value for v in value_tokens]  # type: ignore
-                d["__tokens__"] = [key_token] + list(value_tokens)
-        else:
-            # single value
-            value_token = value_tokens[0]
-            # store the original tokens so they can be processed
-            # differently for METADATA, VALIDATION, and VALUES
-            d["__tokens__"] = [key_token, value_token]
-            values = value_token.value
-
-            if self.quoter.is_string(values):
-                values = self.clean_string(values)  # type: ignore
-
-        d[key_name] = values
-
-        return d
-
-    def check_composite_tokens(self, name: str, tokens) -> tuple[str, list[Any]]:
-        """
-        Return the key and contents of a KEY..END block
-        for PATTERN, POINTS, and PROJECTION
-        """
-        assert len(tokens) >= 2
-        key = tokens[0]
-
-        assert key.value.lower() == name
-        assert tokens[-1].value.lower() == "end"
-
-        if len(tokens) == 2:
-            body = []  # empty TYPE..END block
-        else:
-            body = tokens[1:-1]
-
-        body_tokens = []
-
-        for t in body:
-            if isinstance(t, dict):
-                body_tokens.append(t["__tokens__"])
-            else:
-                body_tokens.append(t)
-        return key, body_tokens
-
-    def process_value_pairs(self, tokens, type_) -> dict:
-        """
-        Metadata, Values, and Validation blocks can either
-        have string pairs or attributes
-        Attributes will already be processed
-        """
-        key, body = self.check_composite_tokens(type_, tokens)
-        key_name = self.key_name(key)
-
-        d = CaseInsensitiveOrderedDict(CaseInsensitiveOrderedDict)
-
-        for t in body:
-            k = self.clean_string(t[0].value).lower()
-            v = self.clean_string(t[1].value)
-
-            if k in d.keys():
-                log.warning(
-                    "A duplicate key (%s) was found in %s. Only the last value (%s) will be used. ",
-                    k,
-                    type_,
-                    v,
-                )
-
-            d[k] = v
-
-        if self.include_position:
-            pd = self.create_position_dict(key, body)
-            d["__position__"] = pd
-
-        d["__type__"] = key_name
-
-        # return the token as well as the processed dict so the
-        # composites function works the same way
-        return d
-
-    def connectionoptions(self, tokens):
-        """
-        Create a dict for the connectionoptions items
-        """
-
-        return self.process_value_pairs(tokens, "connectionoptions")
-
-    def metadata(self, tokens):
-        """
-        Create a dict for the metadata items
-        """
-
-        return self.process_value_pairs(tokens, "metadata")
-
-    def values(self, tokens):
-        """
-        Create a dict for the values items
-        """
-
-        return self.process_value_pairs(tokens, "values")
-
-    def config(self, t):
-        # process this as a separate rule
-        assert len(t) == 3
-        key = t[1].value.lower()  # store all subkeys in lowercase
-        value = t[2].value
-        t[1].value = self.clean_string(key)
-        t[2].value = self.clean_string(value)
-        return self.attr(t)
-
-    def validation(self, tokens):
-        """
-        Create a dict for the validation items
-        """
-        return self.process_value_pairs(tokens, "validation")
-
-    def projection(self, tokens):
-        _, body = self.check_composite_tokens("projection", tokens)
-        projection_strings = [self.clean_string(v.value) for v in body]
-
-        key_token = tokens[0]
-        value_token = tokens[1]  # take the first string as the default token
-        value_token = update_token_value(value_token, projection_strings)
-        tokens = (key_token, value_token)
-
-        return self.attr(tokens)
-
-    def process_pair_lists(self, key_name, tokens):
-        _, body = self.check_composite_tokens(key_name, tokens)
-        pairs = [(v[0].value, v[1].value) for v in body]
-
-        key_token = tokens[0]
-        value_token = tokens[1][0]  # take the first numeric value pair as the token
-        value_token.value = pairs  # set its value to all values
-        tokens = (key_token, value_token)
-
-        return self.attr(tokens)
-
-    def points(self, tokens):
-        return self.process_pair_lists("points", tokens)
-
-    def pattern(self, tokens):
-        return self.process_pair_lists("pattern", tokens)
-
-    # for expressions
-
-    def comparison(self, t):
-        assert len(t) == 3
-        parts = [str(p.value) for p in t]
-        v = " ".join(parts)
-
-        v = f"( {v} )"
-        t[0].value = v
-        return t[0]
-
-    def and_test(self, t):
-        assert len(t) == 2
-        t[0].value = f"( {t[0].value} AND {t[1].value} )"
-        return t[0]
-
-    def or_test(self, t):
-        assert len(t) == 2
-        t[0].value = f"( {t[0].value} OR {t[1].value} )"
-        return t[0]
-
-    def compare_op(self, t):
-        v = t[0]
-        return v
-
-    def not_expression(self, t):
-        v = t[0]
-        v.value = f"NOT {v.value}"
-        return v
-
-    def expression(self, t):
-        exp = " ".join(
-            [str(v.value) for v in t]
-        )  # convert to string for boolean expressions e.g. (true)
-
-        if not self.quoter.in_parenthesis(exp):
-            t[0].value = f"({exp})"
-
-        return t[0]
-
-    def add(self, t):
-        assert len(t) == 2
-        t[0].value = f"{t[0].value} + {t[1].value}"
-        return t[0]
-
-    def sub(self, t):
-        assert len(t) == 2
-        t[0].value = f"{t[0].value} - {t[1].value}"
-        return t[0]
-
-    def div(self, t):
-        assert len(t) == 2
-        t[0].value = f"{t[0].value} / {t[1].value}"
-        return t[0]
-
-    def mul(self, t):
-        assert len(t) == 2
-        t[0].value = f"{t[0].value} * {t[1].value}"
-        return t[0]
-
-    def power(self, t):
-        assert len(t) == 2
-        t[0].value = f"{t[0].value} ^ {t[1].value}"
-        return t[0]
-
-    def neg(self, t):
-        assert len(t) == 1
-        t[0].value = f"-{t[0].value}"
-        return t[0]
-
-    def runtime_var(self, t):
-        v = t[0]
-        return v
-
-    def regexp(self, t):
-        """
-        E.g. regexp(u'/^[0-9]*$/')
-        """
-        v = t[0]
-        return v
-
-    # for functions
-
-    def func_call(self, t):
-        """
-        For function calls e.g. TEXT (tostring([area],"%.2f"))
-        """
-        func, params = t
-        func_name = func.value
-        func.value = f"({func_name}({params}))"
-        return func
-
-    def func_params(self, t):
-        params = ",".join(str(v.value) for v in t)
-        return params
-
-    def attr_bind(self, t):
-        assert len(t) == 1
-        t = t[0]
-        t.value = f"[{t.value}]"
-        return t
-
-    def extent(self, t):
-        assert len(t) == 4
-        return t
-
-    def color(self, t):
-        pass
-
-    def value(self, t):
-        return t
-
-    # basic types
-
-    def true(self, t):
-        v = t[0]
-        return update_token_value(v, True)
-
-    def false(self, t):
-        v = t[0]
-        return update_token_value(v, False)
-
-    def int(self, t):
-        v = t[0]
-        return update_token_value(v, int(v.value))
-
-    def float(self, t):
-        v = t[0]
-        return update_token_value(v, float(v.value))
-
-    def bare_string(self, t):
-        return t[0]
-
-    def name(self, t):
-        v = t[0]
-        return v
-
-    def string(self, t):
-        v = t[0]
-        return v
-
-    def path(self, t):
-        return t[0]
-
-    def string_pair(self, t):
-        a, b = t
-        return [a, b]
-
-    def rgb(self, t):
-        r, g, b = t
-        return r, g, b
-
-    def attr_bind_pair(self, t):
-        assert len(t) == 2
-        return t
-
-    def attr_mixed_pair(self, t):
-        assert len(t) == 2
-        return t
-
-    def colorrange(self, t):
-        assert len(t) == 6
-        return t
-
-    def hexcolorrange(self, t):
-        assert len(t) == 2
-        return t
-
-    def hexcolor(self, t):
-        t[0].value = self.clean_string(t[0].value).lower()
-        return t[0]
-
-    def num_pair(self, t):
-        a, b = t
-        return a, b
-
-    def int_pair(self, t):
-        a, b = t
-        return a, b
-
-    def list(self, t):
-        # http://www.mapserver.org/mapfile/expressions.html#list-expressions
-        v = t[0]
-        list_values = ",".join([str(s) for s in t])
-        v.value = "{%s}" % list_values
-        return v
-
-
-class CommentsTransformer(Transformer_InPlace):
-    """
-    This is an additional transformer that is used to go through
-    all the nodes and take any of the custom node.meta.comment properties
-    and add these value to the node's corresponding dictionary
-    """
-
-    def __init__(self, mapfile_todict):
-        self._mapfile_todict = mapfile_todict
-
-    def get_comments(self, meta):
-        all_comments = []
-
-        if hasattr(meta, "comments"):
-            all_comments += meta.comments
-
-        return all_comments
-
-    def add_metadata_comments(self, d, metadata):
-        """
-        Any duplicate keys will be replaced with the last duplicate along with comments
-        """
-
-        if len(metadata) > 2:
-            string_pairs = metadata[1:-1]  # get all metadata pairs
-            for sp in string_pairs:
-                # get the raw metadata key
-
-                if isinstance(sp.children[0], TOKEN_TYPES):
-                    token = sp.children[0]
-                    assert token.type == "UNQUOTED_STRING"
-                    key = token.value
-                else:
-                    # quoted string (double or single)
-                    token = sp.children[0].children[0]
-                    key = token.value
-
-                # clean it to match the dict key
-                key = self._mapfile_todict.clean_string(key).lower()
-                assert key in d.keys()
-                key_comments = self.get_comments(sp.meta)
-                d["__comments__"][key] = key_comments
-
-        return d
-
-    @v_args(tree=True)
-    def _save_attr_comments(self, tree):
-        d = self._mapfile_todict.transform(tree)
-        d["__comments__"] = self.get_comments(tree.meta)
-        return d
-
-    @v_args(tree=True)
-    def _save_composite_comments(self, tree):
-        d = self._mapfile_todict.transform(tree)
-
-        # composites such as METADATA will not have had a comments
-        # dict created yet
-        if "__comments__" not in d:
-            d["__comments__"] = OrderedDict()
-
-        comments = self.get_comments(tree.meta)
-        if comments:
-            d["__comments__"]["__type__"] = comments
-
-        if d["__type__"] == "metadata":
-            md = tree.children[0].children
-            self.add_metadata_comments(d, md)
-
-        return d
-
-    @v_args(tree=True)
-    def _save_projection_comments(self, tree):
-        d = self._mapfile_todict.transform(tree)
-        comments = self.get_comments(tree.meta)
-        if comments:
-            d["__comments__"] = comments
-
-        return d
-
-    # below we assign callbacks to process comments for each of the following types
-    attr = _save_attr_comments
-    projection = _save_projection_comments
-    composite = _save_composite_comments
-
-
-class MapfileToDict:
-    def __init__(
-        self,
-        include_position=False,
-        include_comments=False,
-        transformer_class=MapfileTransformer,
-        **kwargs,
-    ):
-        self.include_position = include_position
-        self.include_comments = include_comments
-        self.transformer_class = transformer_class
-        self.kwargs = kwargs
-
-    def transform(self, tree):
-        tree = Canonize().transform(tree)
-
-        self.mapfile_transformer = self.transformer_class(
-            include_position=self.include_position,
-            include_comments=self.include_comments,
-            **self.kwargs,
-        )
-
-        if self.include_comments:
-            comments_transformer = CommentsTransformer(self.mapfile_transformer)
-            tree = comments_transformer.transform(tree)
-
-        return self.mapfile_transformer.transform(tree)
-
-
-class Canonize(Transformer_InPlace):
-    @v_args(tree=True)
-    def symbolset(self, tree):
-        composite_type = Tree("composite_type", [Token("symbolset", "symbolset")])
-
-        tree.data = "composite"
-        tree.children.insert(0, composite_type)
-        return tree
-
-
-def calculate_depth(iterable):
-    """
-    A helper function to get the max length + 1 in a list of lists
-    """
-    return (
-        isinstance(iterable, (tuple, list)) and max(map(calculate_depth, iterable)) + 1
-    )
+# =================================================================
+#
+# Authors: Erez Shinan, Seth Girvin
+#
+# Copyright (c) 2020 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+"""
+Module to transform an AST (Abstract Syntax Tree) to a
+Python dict structure
+"""
+
+from __future__ import annotations
+import logging
+from collections import OrderedDict
+from lark import Tree
+from lark.visitors import Transformer_InPlace, Transformer, v_args
+from lark.lexer import Token
+from .parser import lark_cython
+from typing import Any
+from mappyfile.tokens import SINGLETON_COMPOSITE_NAMES, REPEATED_KEYS
+from mappyfile.ordereddict import CaseInsensitiveOrderedDict
+from mappyfile.quoter import Quoter
+
+
+if lark_cython:
+    TOKEN_TYPES = (Token, lark_cython.Token)
+
+    def update_token_value(t, value):
+        return Token.new_borrow_pos(t.type, value, t)
+
+else:
+    TOKEN_TYPES = Token  # type: ignore
+
+    def update_token_value(t, value):
+        t.value = value
+        return t
+
+
+log = logging.getLogger("mappyfile")
+
+
+class MapfileTransformer(Transformer):
+    def __init__(self, include_position: bool = False, include_comments: bool = False):
+        self.quoter = Quoter()
+        self.include_position = include_position
+        self.include_comments = include_comments
+
+    def key_name(self, token) -> str:
+        return token.value.lower()
+
+    def start(self, composites):
+        """
+        Parses a MapServer Mapfile
+        Parsing of partial Mapfiles or lists of composites is also possible
+        """
+
+        # only return a list when there are multiple root composites (e.g.
+        # several CLASSes)
+        if len(composites) == 1:
+            return composites[0]
+
+        return composites
+
+    def flatten(self, values: list[Any]) -> list[Any]:
+        flat_list = []
+
+        for v in values:
+            if isinstance(v, TOKEN_TYPES):
+                flat_list.append(v)
+            elif isinstance(v, list):
+                flat_list += v
+            elif isinstance(v, tuple):
+                flat_list += v
+            elif isinstance(v, dict):
+                assert "__tokens__" in v
+                flat_list += v["__tokens__"]
+            else:
+                raise ValueError("Attribute value type not supported", v)
+
+        return flat_list
+
+    def plural(self, s: str) -> str:
+        if s.endswith("s"):
+            return s + "es"
+
+        return s + "s"
+
+    def create_position_dict(self, key_token, values) -> dict:
+        line, column = key_token.line, key_token.column
+        d = OrderedDict()
+        d["line"] = line
+        d["column"] = column
+
+        if values:
+            flat_list = self.flatten(values)
+            value_positions = [(v.line, v.column) for v in flat_list]
+            d["values"] = value_positions
+
+        return d
+
+    def get_single_key(self, d: dict):
+        keys = list(d.keys())  # convert to list for py3
+        assert len(keys) == 1
+        return keys[0]
+
+    def composite_body(self, t):
+        return t
+
+    def composite_type(self, t):
+        return t
+
+    def _process_composite_config(
+        self,
+        composite_dict: dict,
+        attribute_dict: dict,
+        position_dict: (dict | None),
+        pos: int,
+    ):
+        key_name = "config"
+
+        # there may be several config dicts - one for each setting
+        if key_name not in composite_dict:
+            # create an initial OrderedDict
+            composite_dict[key_name] = CaseInsensitiveOrderedDict(
+                CaseInsensitiveOrderedDict
+            )
+        # populate the existing config dict
+        cfg_dict = composite_dict[key_name]
+        cfg_dict.update(attribute_dict[key_name])
+
+        if position_dict is not None:
+            if key_name not in position_dict:
+                position_dict[key_name] = OrderedDict()
+
+            subkey_name = self.get_single_key(attribute_dict[key_name])
+            position_dict[key_name][subkey_name] = pos
+
+    def _process_composite_points(
+        self,
+        composite_dict: dict,
+        attribute_dict: dict,
+        position_dict: (dict | None),
+        pos: int,
+    ):
+        key_name = "points"
+
+        if key_name not in composite_dict:
+            composite_dict[key_name] = attribute_dict[key_name]
+        else:
+            # if points are already in a feature then
+            # allow for multipart features in a nested list
+            existing_points = composite_dict[key_name]
+
+            if calculate_depth(existing_points) == 2:
+                composite_dict[key_name] = [existing_points]
+
+            if key_name not in composite_dict:
+                composite_dict[key_name] = []
+            composite_dict[key_name].append(attribute_dict[key_name])
+
+        if position_dict is not None:
+            if key_name not in position_dict:
+                position_dict[key_name] = pos
+            else:
+                existing_pos = position_dict[key_name]
+                if isinstance(existing_pos, dict):
+                    position_dict[key_name] = [existing_pos]
+                position_dict[key_name].append(pos)
+
+    def composite(self, t):
+        """
+        Handle the composite types e.g. CLASS..END
+        t is a list in the form [[Token(__LAYER36, 'LAYER')], [OrderedDict([...])]]
+
+        """
+        if len(t) == 1:
+            return t[0]  # metadata and values - already processed
+
+        key_token = t[0][0]
+        attribute_dicts = t[1]
+
+        if not isinstance(attribute_dicts, list):
+            # always handle a list of attributes
+            attribute_dicts = [attribute_dicts]
+
+        key_name = self.key_name(key_token)
+        composite_dict = CaseInsensitiveOrderedDict(CaseInsensitiveOrderedDict)
+        composite_dict["__type__"] = key_name
+
+        if self.include_position:
+            position_dict = self.create_position_dict(key_token, None)
+            composite_dict["__position__"] = position_dict
+        else:
+            position_dict = None
+
+        if self.include_comments:
+            comments_dict = composite_dict["__comments__"] = OrderedDict()
+
+        for d in attribute_dicts:
+            keys = d.keys()
+            if "__type__" in keys:
+                k = d["__type__"]
+                if k in SINGLETON_COMPOSITE_NAMES:
+                    composite_dict[k] = d
+                else:
+                    plural_key = self.plural(k)
+                    if plural_key not in composite_dict:
+                        composite_dict[plural_key] = []
+
+                    composite_dict[plural_key].append(d)
+            else:
+                #  simple attribute
+                pos = d.pop("__position__")
+                d.pop(
+                    "__tokens__", None
+                )  # tokens are no longer needed now we have the positions
+                comments = d.pop("__comments__", None)
+
+                key_name = self.get_single_key(d)
+
+                if key_name == "config":
+                    self._process_composite_config(
+                        composite_dict, d, position_dict, pos
+                    )
+                elif key_name == "points":
+                    self._process_composite_points(
+                        composite_dict, d, position_dict, pos
+                    )
+                elif key_name in REPEATED_KEYS:
+                    if key_name not in composite_dict:
+                        composite_dict[key_name] = []
+
+                    composite_dict[key_name].append(d[key_name])
+
+                    if position_dict:
+                        if key_name not in position_dict:
+                            position_dict[key_name] = []
+                        position_dict[key_name].append(pos)
+                else:
+                    assert len(d.items()) == 1
+                    if position_dict:
+                        # hoist position details to composite
+                        position_dict[key_name] = pos
+                    if self.include_comments and comments:
+                        # hoist comments to composite
+                        comments_dict[key_name] = comments
+
+                    composite_dict[key_name] = d[key_name]
+
+        return composite_dict
+
+    def clean_string(self, val: str) -> str:
+        return self.quoter.remove_quotes(val)
+
+    def attr_name(self, tokens) -> str:
+        t = tokens[0]
+        if not isinstance(t, TOKEN_TYPES):
+            #  handle ambiguities
+            t = t[0]
+            assert t.value.lower() in ("symbol", "style")
+
+        return t
+
+    def attr(self, tokens) -> dict:
+        key_token = tokens[0]
+
+        if isinstance(key_token, (list, tuple)):
+            key_token = key_token[0]
+            assert self.key_name(key_token) in ("style", "symbol"), self.key_name(
+                key_token
+            )
+
+        key_name = self.key_name(key_token)
+        value_tokens = tokens[1:]
+
+        if isinstance(value_tokens[0], (list, tuple)):
+            # for any multi-part attributes they will be lists or tuples
+            # e.g. int_pair, rgb etc.
+            assert len(value_tokens) == 1
+            value_tokens = value_tokens[0]
+
+        pd = self.create_position_dict(key_token, value_tokens)
+        d: dict = OrderedDict()
+        d["__position__"] = pd
+
+        if len(value_tokens) > 1:
+            if key_name == "config":
+                assert len(value_tokens) == 2
+                values = {value_tokens[0].value: value_tokens[1].value}
+            else:
+                # list of values
+                values = [v.value for v in value_tokens]  # type: ignore
+                d["__tokens__"] = [key_token] + list(value_tokens)
+        else:
+            # single value
+            value_token = value_tokens[0]
+            # store the original tokens so they can be processed
+            # differently for METADATA, VALIDATION, and VALUES
+            d["__tokens__"] = [key_token, value_token]
+            values = value_token.value
+
+            if self.quoter.is_string(values):
+                values = self.clean_string(values)  # type: ignore
+
+        d[key_name] = values
+
+        return d
+
+    def check_composite_tokens(self, name: str, tokens) -> tuple[str, list[Any]]:
+        """
+        Return the key and contents of a KEY..END block
+        for PATTERN, POINTS, and PROJECTION
+        """
+        assert len(tokens) >= 2
+        key = tokens[0]
+
+        assert key.value.lower() == name
+        assert tokens[-1].value.lower() == "end"
+
+        if len(tokens) == 2:
+            body = []  # empty TYPE..END block
+        else:
+            body = tokens[1:-1]
+
+        body_tokens = []
+
+        for t in body:
+            if isinstance(t, dict):
+                body_tokens.append(t["__tokens__"])
+            else:
+                body_tokens.append(t)
+        return key, body_tokens
+
+    def process_value_pairs(self, tokens, type_) -> dict:
+        """
+        Metadata, Values, and Validation blocks can either
+        have string pairs or attributes
+        Attributes will already be processed
+        """
+        key, body = self.check_composite_tokens(type_, tokens)
+        key_name = self.key_name(key)
+
+        d = CaseInsensitiveOrderedDict(CaseInsensitiveOrderedDict)
+
+        for t in body:
+            k = self.clean_string(t[0].value).lower()
+            v = self.clean_string(t[1].value)
+
+            if k in d.keys():
+                log.warning(
+                    "A duplicate key (%s) was found in %s. Only the last value (%s) will be used. ",
+                    k,
+                    type_,
+                    v,
+                )
+
+            d[k] = v
+
+        if self.include_position:
+            pd = self.create_position_dict(key, body)
+            d["__position__"] = pd
+
+        d["__type__"] = key_name
+
+        # return the token as well as the processed dict so the
+        # composites function works the same way
+        return d
+
+    def connectionoptions(self, tokens):
+        """
+        Create a dict for the connectionoptions items
+        """
+
+        return self.process_value_pairs(tokens, "connectionoptions")
+
+    def metadata(self, tokens):
+        """
+        Create a dict for the metadata items
+        """
+
+        return self.process_value_pairs(tokens, "metadata")
+
+    def values(self, tokens):
+        """
+        Create a dict for the values items
+        """
+
+        return self.process_value_pairs(tokens, "values")
+
+    def config(self, t):
+        # process this as a separate rule
+        assert len(t) == 3
+        key = t[1].value.lower()  # store all subkeys in lowercase
+        value = t[2].value
+        t[1].value = self.clean_string(key)
+        t[2].value = self.clean_string(value)
+        return self.attr(t)
+
+    def validation(self, tokens):
+        """
+        Create a dict for the validation items
+        """
+        return self.process_value_pairs(tokens, "validation")
+
+    def projection(self, tokens):
+        _, body = self.check_composite_tokens("projection", tokens)
+        projection_strings = [self.clean_string(v.value) for v in body]
+
+        key_token = tokens[0]
+        value_token = tokens[1]  # take the first string as the default token
+        value_token = update_token_value(value_token, projection_strings)
+        tokens = (key_token, value_token)
+
+        return self.attr(tokens)
+
+    def process_pair_lists(self, key_name, tokens):
+        _, body = self.check_composite_tokens(key_name, tokens)
+        pairs = [(v[0].value, v[1].value) for v in body]
+
+        key_token = tokens[0]
+        value_token = tokens[1][0]  # take the first numeric value pair as the token
+        value_token.value = pairs  # set its value to all values
+        tokens = (key_token, value_token)
+
+        return self.attr(tokens)
+
+    def points(self, tokens):
+        return self.process_pair_lists("points", tokens)
+
+    def pattern(self, tokens):
+        return self.process_pair_lists("pattern", tokens)
+
+    # for expressions
+
+    def comparison(self, t):
+        assert len(t) == 3
+        parts = [str(p.value) for p in t]
+        v = " ".join(parts)
+
+        v = f"( {v} )"
+        t[0].value = v
+        return t[0]
+
+    def and_test(self, t):
+        assert len(t) == 2
+        t[0].value = f"( {t[0].value} AND {t[1].value} )"
+        return t[0]
+
+    def or_test(self, t):
+        assert len(t) == 2
+        t[0].value = f"( {t[0].value} OR {t[1].value} )"
+        return t[0]
+
+    def compare_op(self, t):
+        v = t[0]
+        return v
+
+    def not_expression(self, t):
+        v = t[0]
+        v.value = f"NOT {v.value}"
+        return v
+
+    def expression(self, t):
+        exp = " ".join(
+            [str(v.value) for v in t]
+        )  # convert to string for boolean expressions e.g. (true)
+
+        if not self.quoter.in_parenthesis(exp):
+            t[0].value = f"({exp})"
+
+        return t[0]
+
+    def add(self, t):
+        assert len(t) == 2
+        t[0].value = f"{t[0].value} + {t[1].value}"
+        return t[0]
+
+    def sub(self, t):
+        assert len(t) == 2
+        t[0].value = f"{t[0].value} - {t[1].value}"
+        return t[0]
+
+    def div(self, t):
+        assert len(t) == 2
+        t[0].value = f"{t[0].value} / {t[1].value}"
+        return t[0]
+
+    def mul(self, t):
+        assert len(t) == 2
+        t[0].value = f"{t[0].value} * {t[1].value}"
+        return t[0]
+
+    def power(self, t):
+        assert len(t) == 2
+        t[0].value = f"{t[0].value} ^ {t[1].value}"
+        return t[0]
+
+    def neg(self, t):
+        assert len(t) == 1
+        t[0].value = f"-{t[0].value}"
+        return t[0]
+
+    def runtime_var(self, t):
+        v = t[0]
+        return v
+
+    def regexp(self, t):
+        """
+        E.g. regexp(u'/^[0-9]*$/')
+        """
+        v = t[0]
+        return v
+
+    # for functions
+
+    def func_call(self, t):
+        """
+        For function calls e.g. TEXT (tostring([area],"%.2f"))
+        """
+        func, params = t
+        func_name = func.value
+        func.value = f"({func_name}({params}))"
+        return func
+
+    def func_params(self, t):
+        params = ",".join(str(v.value) for v in t)
+        return params
+
+    def attr_bind(self, t):
+        assert len(t) == 1
+        t = t[0]
+        t.value = f"[{t.value}]"
+        return t
+
+    def extent(self, t):
+        assert len(t) == 4
+        return t
+
+    def color(self, t):
+        pass
+
+    def value(self, t):
+        return t
+
+    # basic types
+
+    def true(self, t):
+        v = t[0]
+        return update_token_value(v, True)
+
+    def false(self, t):
+        v = t[0]
+        return update_token_value(v, False)
+
+    def int(self, t):
+        v = t[0]
+        return update_token_value(v, int(v.value))
+
+    def float(self, t):
+        v = t[0]
+        return update_token_value(v, float(v.value))
+
+    def bare_string(self, t):
+        return t[0]
+
+    def name(self, t):
+        v = t[0]
+        return v
+
+    def string(self, t):
+        v = t[0]
+        return v
+
+    def path(self, t):
+        return t[0]
+
+    def string_pair(self, t):
+        a, b = t
+        return [a, b]
+
+    def rgb(self, t):
+        r, g, b = t
+        return r, g, b
+
+    def attr_bind_pair(self, t):
+        assert len(t) == 2
+        return t
+
+    def attr_mixed_pair(self, t):
+        assert len(t) == 2
+        return t
+
+    def colorrange(self, t):
+        assert len(t) == 6
+        return t
+
+    def hexcolorrange(self, t):
+        assert len(t) == 2
+        return t
+
+    def hexcolor(self, t):
+        t[0].value = self.clean_string(t[0].value).lower()
+        return t[0]
+
+    def num_pair(self, t):
+        a, b = t
+        return a, b
+
+    def int_pair(self, t):
+        a, b = t
+        return a, b
+
+    def list(self, t):
+        # http://www.mapserver.org/mapfile/expressions.html#list-expressions
+        v = t[0]
+        list_values = ",".join([str(s) for s in t])
+        v.value = "{%s}" % list_values
+        return v
+
+
+class CommentsTransformer(Transformer_InPlace):
+    """
+    This is an additional transformer that is used to go through
+    all the nodes and take any of the custom node.meta.comment properties
+    and add these value to the node's corresponding dictionary
+    """
+
+    def __init__(self, mapfile_todict):
+        self._mapfile_todict = mapfile_todict
+
+    def get_comments(self, meta):
+        all_comments = []
+
+        if hasattr(meta, "comments"):
+            all_comments += meta.comments
+
+        return all_comments
+
+    def add_metadata_comments(self, d, metadata):
+        """
+        Any duplicate keys will be replaced with the last duplicate along with comments
+        """
+
+        if len(metadata) > 2:
+            string_pairs = metadata[1:-1]  # get all metadata pairs
+            for sp in string_pairs:
+                # get the raw metadata key
+
+                if isinstance(sp.children[0], TOKEN_TYPES):
+                    token = sp.children[0]
+                    assert token.type == "UNQUOTED_STRING"
+                    key = token.value
+                else:
+                    # quoted string (double or single)
+                    token = sp.children[0].children[0]
+                    key = token.value
+
+                # clean it to match the dict key
+                key = self._mapfile_todict.clean_string(key).lower()
+                assert key in d.keys()
+                key_comments = self.get_comments(sp.meta)
+                d["__comments__"][key] = key_comments
+
+        return d
+
+    @v_args(tree=True)
+    def _save_attr_comments(self, tree):
+        d = self._mapfile_todict.transform(tree)
+        d["__comments__"] = self.get_comments(tree.meta)
+        return d
+
+    @v_args(tree=True)
+    def _save_composite_comments(self, tree):
+        d = self._mapfile_todict.transform(tree)
+
+        # composites such as METADATA will not have had a comments
+        # dict created yet
+        if "__comments__" not in d:
+            d["__comments__"] = OrderedDict()
+
+        comments = self.get_comments(tree.meta)
+        if comments:
+            d["__comments__"]["__type__"] = comments
+
+        if d["__type__"] == "metadata":
+            md = tree.children[0].children
+            self.add_metadata_comments(d, md)
+
+        return d
+
+    @v_args(tree=True)
+    def _save_projection_comments(self, tree):
+        d = self._mapfile_todict.transform(tree)
+        comments = self.get_comments(tree.meta)
+        if comments:
+            d["__comments__"] = comments
+
+        return d
+
+    # below we assign callbacks to process comments for each of the following types
+    attr = _save_attr_comments
+    projection = _save_projection_comments
+    composite = _save_composite_comments
+
+
+class MapfileToDict:
+    def __init__(
+        self,
+        include_position=False,
+        include_comments=False,
+        transformer_class=MapfileTransformer,
+        **kwargs,
+    ):
+        self.include_position = include_position
+        self.include_comments = include_comments
+        self.transformer_class = transformer_class
+        self.kwargs = kwargs
+
+    def transform(self, tree):
+        tree = Canonize().transform(tree)
+
+        self.mapfile_transformer = self.transformer_class(
+            include_position=self.include_position,
+            include_comments=self.include_comments,
+            **self.kwargs,
+        )
+
+        if self.include_comments:
+            comments_transformer = CommentsTransformer(self.mapfile_transformer)
+            tree = comments_transformer.transform(tree)
+
+        return self.mapfile_transformer.transform(tree)
+
+
+class Canonize(Transformer_InPlace):
+    @v_args(tree=True)
+    def symbolset(self, tree):
+        composite_type = Tree("composite_type", [Token("symbolset", "symbolset")])
+
+        tree.data = "composite"
+        tree.children.insert(0, composite_type)
+        return tree
+
+
+def calculate_depth(iterable):
+    """
+    A helper function to get the max length + 1 in a list of lists
+    """
+    return (
+        isinstance(iterable, (tuple, list)) and max(map(calculate_depth, iterable)) + 1
+    )
```

### Comparing `mappyfile-1.0.1/mappyfile/utils.py` & `mappyfile-1.0.2/mappyfile/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,515 +1,515 @@
-# =================================================================
-#
-# Authors: Seth Girvin
-#
-# Copyright (c) 2021 Seth Girvin
-#
-# Permission is hereby granted, free of charge, to any person
-# obtaining a copy of this software and associated documentation
-# files (the "Software"), to deal in the Software without
-# restriction, including without limitation the rights to use,
-# copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the
-# Software is furnished to do so, subject to the following
-# conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
-# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-# OTHER DEALINGS IN THE SOFTWARE.
-#
-# =================================================================
-
-from __future__ import annotations
-import codecs
-import warnings
-import functools
-from mappyfile.ordereddict import DefaultOrderedDict
-from mappyfile.parser import Parser
-from mappyfile.transformer import MapfileToDict
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.validator import Validator
-from typing import IO
-
-
-def deprecated(func):
-    """
-    From https://stackoverflow.com/questions/2536307/how-do-i-deprecate-python-functions/30253848#30253848
-    This is a decorator which can be used to mark functions
-    as deprecated. It will result in a warning being emitted
-    when the function is used.
-    """
-
-    @functools.wraps(func)
-    def new_func(*args, **kwargs):
-        warnings.simplefilter("always", DeprecationWarning)  # turn off filter
-        warnings.warn(
-            f"Call to deprecated function {func.__name__}.",
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-        warnings.simplefilter("default", DeprecationWarning)  # reset filter
-        return func(*args, **kwargs)
-
-    return new_func
-
-
-# pylint: disable=redefined-builtin
-def open(
-    fn: str,
-    expand_includes: bool = True,
-    include_comments: bool = False,
-    include_position: bool = False,
-    **kwargs,
-) -> dict:
-    """
-    Load a Mapfile from the supplied filename into a Python dictionary.
-
-    Parameters
-    ----------
-
-    fn: string
-        The path to the Mapfile, or partial Mapfile
-    expand_includes: boolean
-        Load any ``INCLUDE`` files in the MapFile
-    include_comments: boolean
-         Include or discard comment strings from the Mapfile - *experimental*
-    include_position: boolean
-         Include the position of the Mapfile tokens in the output
-
-    Returns
-    -------
-
-    dict
-        A Python dictionary representing the Mapfile in the mappyfile format
-
-    Example
-    -------
-
-    To open a Mapfile from a filename and return it as a dictionary object::
-
-        d = mappyfile.open('mymap.map')
-
-    Notes
-    -----
-
-    Partial Mapfiles can also be opened, for example a file containing a ``LAYER`` object.
-
-    """
-    p = Parser(
-        expand_includes=expand_includes, include_comments=include_comments, **kwargs
-    )
-    ast = p.parse_file(fn)
-    m = MapfileToDict(
-        include_position=include_position, include_comments=include_comments, **kwargs
-    )
-    d = m.transform(ast)
-    return d
-
-
-def load(
-    fp: IO[str],
-    expand_includes: bool = True,
-    include_position: bool = False,
-    include_comments: bool = False,
-    **kwargs,
-) -> dict:
-    """
-    Load a Mapfile from an open file or file-like object.
-
-    Parameters
-    ----------
-
-    fp: file
-        A file-like object - as with all Mapfiles this should be encoded in "utf-8"
-    expand_includes: boolean
-        Load any ``INCLUDE`` files in the MapFile
-    include_comments: boolean
-         Include or discard comment strings from the Mapfile - *experimental*
-    include_position: boolean
-         Include the position of the Mapfile tokens in the output
-
-    Returns
-    -------
-
-    dict
-        A Python dictionary representing the Mapfile in the mappyfile format
-
-    Example
-    -------
-
-    To open a Mapfile from a file and return it as a dictionary object::
-
-        with open('mymap.map') as fp:
-            d = mappyfile.load(fp)
-
-    Notes
-    -----
-
-    Partial Mapfiles can also be opened, for example a file containing a ``LAYER`` object.
-    """
-    p = Parser(
-        expand_includes=expand_includes, include_comments=include_comments, **kwargs
-    )
-    ast = p.load(fp)
-    m = MapfileToDict(
-        include_position=include_position, include_comments=include_comments, **kwargs
-    )
-    d = m.transform(ast)
-    return d
-
-
-def loads(
-    s: str,
-    expand_includes: bool = True,
-    include_position: bool = False,
-    include_comments: bool = False,
-    **kwargs,
-) -> dict:
-    """
-    Load a Mapfile from a string
-
-    Parameters
-    ----------
-
-    s: string
-        The Mapfile, or partial Mapfile, text
-    expand_includes: boolean
-        Load any ``INCLUDE`` files in the MapFile
-    include_comments: boolean
-         Include or discard comment strings from the Mapfile - *experimental*
-    include_position: boolean
-         Include the position of the Mapfile tokens in the output
-
-    Returns
-    -------
-
-    dict
-        A Python dictionary representing the Mapfile in the mappyfile format
-
-    Example
-    -------
-
-    To open a Mapfile from a string and return it as a dictionary object::
-
-        s = '''MAP NAME "TEST" END'''
-
-        d = mappyfile.loads(s)
-        assert d["name"] == "TEST"
-
-    """
-    p = Parser(
-        expand_includes=expand_includes, include_comments=include_comments, **kwargs
-    )
-    ast = p.parse(s)
-    m = MapfileToDict(
-        include_position=include_position, include_comments=include_comments, **kwargs
-    )
-    d = m.transform(ast)
-    return d
-
-
-# pylint: disable=too-many-arguments
-def dump(
-    d: dict,
-    fp: IO[str],
-    indent: int = 4,
-    spacer: str = " ",
-    quote: str = '"',
-    newlinechar: str = "\n",
-    end_comment: bool = False,
-    align_values: bool = False,
-    separate_complex_types: bool = False,
-):
-    """
-    Write d (the Mapfile dictionary) as a formatted stream to fp
-
-    Parameters
-    ----------
-
-    d: dict
-        A Python dictionary based on the the mappyfile schema
-    fp: file
-        A file-like object
-    indent: int
-        The number of ``spacer`` characters to indent structures in the Mapfile
-    spacer: string
-        The character to use for indenting structures in the Mapfile. Typically
-        spaces or tab characters (``\\t``)
-    quote: string
-        The quote character to use in the Mapfile (double or single quotes)
-    newlinechar: string
-        The character used to insert newlines in the Mapfile
-    end_comment: bool
-        Add a comment with the block type at each closing END
-        statement e.g. END # MAP
-    align_values: bool
-        Aligns the values in the same column for better readability. The column is
-        multiple of indent and determined by the longest key
-    separate_complex_types: bool
-        Groups composites (complex mapserver definitions with "END") together at the end.
-        Keeps the given order except that all simple key-value pairs appear before composites.
-
-    Example
-    -------
-
-    To open a Mapfile from a string, and then dump it back out to an open file,
-    using 2 spaces for indentation, and single-quotes for properties::
-
-        s = '''MAP NAME "TEST" END'''
-
-        d = mappyfile.loads(s)
-        with open(fn, "w") as f:
-            mappyfile.dump(d, f, indent=2, quote="'")
-
-    """
-    map_string = _pprint(
-        d,
-        indent,
-        spacer,
-        quote,
-        newlinechar,
-        end_comment,
-        align_values,
-        separate_complex_types,
-    )
-    fp.write(map_string)
-
-
-# pylint: disable=too-many-arguments
-def save(
-    d: dict,
-    output_file: str,
-    indent: int = 4,
-    spacer: str = " ",
-    quote: str = '"',
-    newlinechar: str = "\n",
-    end_comment: bool = False,
-    align_values: bool = False,
-    separate_complex_types: bool = False,
-) -> str:
-    """
-    Write a dictionary to an output Mapfile on disk
-
-    Parameters
-    ----------
-
-    d: dict
-        A Python dictionary based on the the mappyfile schema
-    output_file: string
-        The output filename
-    indent: int
-        The number of ``spacer`` characters to indent structures in the Mapfile
-    spacer: string
-        The character to use for indenting structures in the Mapfile. Typically
-        spaces or tab characters (``\\t``)
-    quote: string
-        The quote character to use in the Mapfile (double or single quotes)
-    newlinechar: string
-        The character used to insert newlines in the Mapfile
-    end_comment: bool
-        Add a comment with the block type at each closing END
-        statement e.g. END # MAP
-    align_values: bool
-        Aligns the values in the same column for better readability. The column is
-        multiple of indent and determined by the longest key.
-    separate_complex_types: bool
-        Groups composites (complex mapserver definitions with "END") together at the end.
-        Keeps the given order except that all simple key-value pairs appear before composites.
-
-    Returns
-    -------
-
-    string
-          The output_file passed into the function
-
-    Example
-    -------
-
-    To open a Mapfile from a string, and then save it to a file::
-
-        s = '''MAP NAME "TEST" END'''
-
-        d = mappyfile.loads(s)
-        fn = "C:/Data/mymap.map"
-        mappyfile.save(d, fn)
-    """
-    map_string = _pprint(
-        d,
-        indent,
-        spacer,
-        quote,
-        newlinechar,
-        end_comment,
-        align_values,
-        separate_complex_types,
-    )
-    _save(output_file, map_string)
-    return output_file
-
-
-# pylint: disable=too-many-arguments
-def dumps(
-    d: dict,
-    indent: int = 4,
-    spacer: str = " ",
-    quote: str = '"',
-    newlinechar: str = "\n",
-    end_comment: bool = False,
-    align_values: bool = False,
-    separate_complex_types: bool = False,
-    **kwargs,
-) -> str:
-    """
-    Output a Mapfile dictionary as a string
-
-    Parameters
-    ----------
-
-    d: dict
-        A Python dictionary based on the the mappyfile schema
-    indent: int
-        The number of ``spacer`` characters to indent structures in the Mapfile
-    spacer: string
-        The character to use for indenting structures in the Mapfile. Typically
-        spaces or tab characters (``\\t``)
-    quote: string
-        The quote character to use in the Mapfile (double or single quotes)
-    newlinechar: string
-        The character used to insert newlines in the Mapfile
-    end_comment: bool
-        Add a comment with the block type at each closing END
-        statement e.g. END # MAP
-    align_values: bool
-        Aligns the values in the same column for better readability. The column is
-        multiple of indent and determined by the longest key
-    separate_complex_types: bool
-        Groups composites (complex mapserver definitions with "END") together at the end.
-        Keeps the given order except that all simple key-value pairs appear before composites.
-
-    Returns
-    -------
-
-    string
-          The Mapfile as a string
-
-    Example
-    -------
-
-    To open a Mapfile from a string, and then print it back out
-    as a string using tabs::
-
-        s = '''MAP NAME "TEST" END'''
-
-        d = mappyfile.loads(s)
-        print(mappyfile.dumps(d, indent=1, spacer="\\t"))
-    """
-    return _pprint(
-        d,
-        indent,
-        spacer,
-        quote,
-        newlinechar,
-        end_comment,
-        align_values,
-        separate_complex_types,
-        **kwargs,
-    )
-
-
-def validate(d: dict, version: (float | None) = None) -> list:
-    """
-    Validate a mappyfile dictionary by using the Mapfile schema.
-    An optional version number can be used to specify a specific
-    a Mapfile is valid for a specific MapServer version.
-
-    Parameters
-    ----------
-
-     d: dict
-        A Python dictionary based on the the mappyfile schema
-    version: float
-        The MapServer version number used to validate the Mapfile
-
-    Returns
-    -------
-
-    list
-        A list containing validation errors
-
-    """
-    v = Validator()
-    return v.validate(d, version=version)
-
-
-def _save(output_file: str, string: str) -> None:
-    with codecs.open(output_file, "w", encoding="utf-8") as f:
-        f.write(string)
-
-
-def _pprint(
-    d: dict,
-    indent: int,
-    spacer: str,
-    quote: str,
-    newlinechar: str,
-    end_comment: bool,
-    align_values: bool,
-    separate_complex_types: bool,
-    **kwargs,
-) -> str:
-    pp = PrettyPrinter(
-        indent=indent,
-        spacer=spacer,
-        quote=quote,
-        newlinechar=newlinechar,
-        end_comment=end_comment,
-        align_values=align_values,
-        separate_complex_types=separate_complex_types,
-        **kwargs,
-    )
-    return pp.pprint(d)
-
-
-def create(type: str, version=None) -> dict:
-    """
-    Create a new mappyfile object, using MapServer defaults (if any).
-
-    Parameters
-    ----------
-
-    s: type
-        The mappyfile type to be stored in the __type__ property
-
-    Returns
-    -------
-
-    dict
-        A Python dictionary representing the Mapfile object in the mappyfile format
-    """
-
-    # get the schema for this type
-
-    v = Validator()
-    try:
-        schema = v.get_versioned_schema(version=version, schema_name=type)
-    except IOError as exc:
-        raise SyntaxError("The mappyfile type '{type}' does not exist!") from exc
-
-    d = DefaultOrderedDict()
-    d["__type__"] = type
-
-    properties = sorted(schema["properties"].items())
-
-    for key, value in properties:
-        if "default" in value:
-            d[key] = value["default"]
-
-    return d
+# =================================================================
+#
+# Authors: Seth Girvin
+#
+# Copyright (c) 2021 Seth Girvin
+#
+# Permission is hereby granted, free of charge, to any person
+# obtaining a copy of this software and associated documentation
+# files (the "Software"), to deal in the Software without
+# restriction, including without limitation the rights to use,
+# copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the
+# Software is furnished to do so, subject to the following
+# conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
+# OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
+# HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+# WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+# FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+# OTHER DEALINGS IN THE SOFTWARE.
+#
+# =================================================================
+
+from __future__ import annotations
+import codecs
+import warnings
+import functools
+from mappyfile.ordereddict import DefaultOrderedDict
+from mappyfile.parser import Parser
+from mappyfile.transformer import MapfileToDict
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.validator import Validator
+from typing import IO
+
+
+def deprecated(func):
+    """
+    From https://stackoverflow.com/questions/2536307/how-do-i-deprecate-python-functions/30253848#30253848
+    This is a decorator which can be used to mark functions
+    as deprecated. It will result in a warning being emitted
+    when the function is used.
+    """
+
+    @functools.wraps(func)
+    def new_func(*args, **kwargs):
+        warnings.simplefilter("always", DeprecationWarning)  # turn off filter
+        warnings.warn(
+            f"Call to deprecated function {func.__name__}.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+        warnings.simplefilter("default", DeprecationWarning)  # reset filter
+        return func(*args, **kwargs)
+
+    return new_func
+
+
+# pylint: disable=redefined-builtin
+def open(
+    fn: str,
+    expand_includes: bool = True,
+    include_comments: bool = False,
+    include_position: bool = False,
+    **kwargs,
+) -> dict:
+    """
+    Load a Mapfile from the supplied filename into a Python dictionary.
+
+    Parameters
+    ----------
+
+    fn: string
+        The path to the Mapfile, or partial Mapfile
+    expand_includes: boolean
+        Load any ``INCLUDE`` files in the MapFile
+    include_comments: boolean
+         Include or discard comment strings from the Mapfile - *experimental*
+    include_position: boolean
+         Include the position of the Mapfile tokens in the output
+
+    Returns
+    -------
+
+    dict
+        A Python dictionary representing the Mapfile in the mappyfile format
+
+    Example
+    -------
+
+    To open a Mapfile from a filename and return it as a dictionary object::
+
+        d = mappyfile.open('mymap.map')
+
+    Notes
+    -----
+
+    Partial Mapfiles can also be opened, for example a file containing a ``LAYER`` object.
+
+    """
+    p = Parser(
+        expand_includes=expand_includes, include_comments=include_comments, **kwargs
+    )
+    ast = p.parse_file(fn)
+    m = MapfileToDict(
+        include_position=include_position, include_comments=include_comments, **kwargs
+    )
+    d = m.transform(ast)
+    return d
+
+
+def load(
+    fp: IO[str],
+    expand_includes: bool = True,
+    include_position: bool = False,
+    include_comments: bool = False,
+    **kwargs,
+) -> dict:
+    """
+    Load a Mapfile from an open file or file-like object.
+
+    Parameters
+    ----------
+
+    fp: file
+        A file-like object - as with all Mapfiles this should be encoded in "utf-8"
+    expand_includes: boolean
+        Load any ``INCLUDE`` files in the MapFile
+    include_comments: boolean
+         Include or discard comment strings from the Mapfile - *experimental*
+    include_position: boolean
+         Include the position of the Mapfile tokens in the output
+
+    Returns
+    -------
+
+    dict
+        A Python dictionary representing the Mapfile in the mappyfile format
+
+    Example
+    -------
+
+    To open a Mapfile from a file and return it as a dictionary object::
+
+        with open('mymap.map') as fp:
+            d = mappyfile.load(fp)
+
+    Notes
+    -----
+
+    Partial Mapfiles can also be opened, for example a file containing a ``LAYER`` object.
+    """
+    p = Parser(
+        expand_includes=expand_includes, include_comments=include_comments, **kwargs
+    )
+    ast = p.load(fp)
+    m = MapfileToDict(
+        include_position=include_position, include_comments=include_comments, **kwargs
+    )
+    d = m.transform(ast)
+    return d
+
+
+def loads(
+    s: str,
+    expand_includes: bool = True,
+    include_position: bool = False,
+    include_comments: bool = False,
+    **kwargs,
+) -> dict:
+    """
+    Load a Mapfile from a string
+
+    Parameters
+    ----------
+
+    s: string
+        The Mapfile, or partial Mapfile, text
+    expand_includes: boolean
+        Load any ``INCLUDE`` files in the MapFile
+    include_comments: boolean
+         Include or discard comment strings from the Mapfile - *experimental*
+    include_position: boolean
+         Include the position of the Mapfile tokens in the output
+
+    Returns
+    -------
+
+    dict
+        A Python dictionary representing the Mapfile in the mappyfile format
+
+    Example
+    -------
+
+    To open a Mapfile from a string and return it as a dictionary object::
+
+        s = '''MAP NAME "TEST" END'''
+
+        d = mappyfile.loads(s)
+        assert d["name"] == "TEST"
+
+    """
+    p = Parser(
+        expand_includes=expand_includes, include_comments=include_comments, **kwargs
+    )
+    ast = p.parse(s)
+    m = MapfileToDict(
+        include_position=include_position, include_comments=include_comments, **kwargs
+    )
+    d = m.transform(ast)
+    return d
+
+
+# pylint: disable=too-many-arguments
+def dump(
+    d: dict,
+    fp: IO[str],
+    indent: int = 4,
+    spacer: str = " ",
+    quote: str = '"',
+    newlinechar: str = "\n",
+    end_comment: bool = False,
+    align_values: bool = False,
+    separate_complex_types: bool = False,
+):
+    """
+    Write d (the Mapfile dictionary) as a formatted stream to fp
+
+    Parameters
+    ----------
+
+    d: dict
+        A Python dictionary based on the the mappyfile schema
+    fp: file
+        A file-like object
+    indent: int
+        The number of ``spacer`` characters to indent structures in the Mapfile
+    spacer: string
+        The character to use for indenting structures in the Mapfile. Typically
+        spaces or tab characters (``\\t``)
+    quote: string
+        The quote character to use in the Mapfile (double or single quotes)
+    newlinechar: string
+        The character used to insert newlines in the Mapfile
+    end_comment: bool
+        Add a comment with the block type at each closing END
+        statement e.g. END # MAP
+    align_values: bool
+        Aligns the values in the same column for better readability. The column is
+        multiple of indent and determined by the longest key
+    separate_complex_types: bool
+        Groups composites (complex mapserver definitions with "END") together at the end.
+        Keeps the given order except that all simple key-value pairs appear before composites.
+
+    Example
+    -------
+
+    To open a Mapfile from a string, and then dump it back out to an open file,
+    using 2 spaces for indentation, and single-quotes for properties::
+
+        s = '''MAP NAME "TEST" END'''
+
+        d = mappyfile.loads(s)
+        with open(fn, "w") as f:
+            mappyfile.dump(d, f, indent=2, quote="'")
+
+    """
+    map_string = _pprint(
+        d,
+        indent,
+        spacer,
+        quote,
+        newlinechar,
+        end_comment,
+        align_values,
+        separate_complex_types,
+    )
+    fp.write(map_string)
+
+
+# pylint: disable=too-many-arguments
+def save(
+    d: dict,
+    output_file: str,
+    indent: int = 4,
+    spacer: str = " ",
+    quote: str = '"',
+    newlinechar: str = "\n",
+    end_comment: bool = False,
+    align_values: bool = False,
+    separate_complex_types: bool = False,
+) -> str:
+    """
+    Write a dictionary to an output Mapfile on disk
+
+    Parameters
+    ----------
+
+    d: dict
+        A Python dictionary based on the the mappyfile schema
+    output_file: string
+        The output filename
+    indent: int
+        The number of ``spacer`` characters to indent structures in the Mapfile
+    spacer: string
+        The character to use for indenting structures in the Mapfile. Typically
+        spaces or tab characters (``\\t``)
+    quote: string
+        The quote character to use in the Mapfile (double or single quotes)
+    newlinechar: string
+        The character used to insert newlines in the Mapfile
+    end_comment: bool
+        Add a comment with the block type at each closing END
+        statement e.g. END # MAP
+    align_values: bool
+        Aligns the values in the same column for better readability. The column is
+        multiple of indent and determined by the longest key.
+    separate_complex_types: bool
+        Groups composites (complex mapserver definitions with "END") together at the end.
+        Keeps the given order except that all simple key-value pairs appear before composites.
+
+    Returns
+    -------
+
+    string
+          The output_file passed into the function
+
+    Example
+    -------
+
+    To open a Mapfile from a string, and then save it to a file::
+
+        s = '''MAP NAME "TEST" END'''
+
+        d = mappyfile.loads(s)
+        fn = "C:/Data/mymap.map"
+        mappyfile.save(d, fn)
+    """
+    map_string = _pprint(
+        d,
+        indent,
+        spacer,
+        quote,
+        newlinechar,
+        end_comment,
+        align_values,
+        separate_complex_types,
+    )
+    _save(output_file, map_string)
+    return output_file
+
+
+# pylint: disable=too-many-arguments
+def dumps(
+    d: dict,
+    indent: int = 4,
+    spacer: str = " ",
+    quote: str = '"',
+    newlinechar: str = "\n",
+    end_comment: bool = False,
+    align_values: bool = False,
+    separate_complex_types: bool = False,
+    **kwargs,
+) -> str:
+    """
+    Output a Mapfile dictionary as a string
+
+    Parameters
+    ----------
+
+    d: dict
+        A Python dictionary based on the the mappyfile schema
+    indent: int
+        The number of ``spacer`` characters to indent structures in the Mapfile
+    spacer: string
+        The character to use for indenting structures in the Mapfile. Typically
+        spaces or tab characters (``\\t``)
+    quote: string
+        The quote character to use in the Mapfile (double or single quotes)
+    newlinechar: string
+        The character used to insert newlines in the Mapfile
+    end_comment: bool
+        Add a comment with the block type at each closing END
+        statement e.g. END # MAP
+    align_values: bool
+        Aligns the values in the same column for better readability. The column is
+        multiple of indent and determined by the longest key
+    separate_complex_types: bool
+        Groups composites (complex mapserver definitions with "END") together at the end.
+        Keeps the given order except that all simple key-value pairs appear before composites.
+
+    Returns
+    -------
+
+    string
+          The Mapfile as a string
+
+    Example
+    -------
+
+    To open a Mapfile from a string, and then print it back out
+    as a string using tabs::
+
+        s = '''MAP NAME "TEST" END'''
+
+        d = mappyfile.loads(s)
+        print(mappyfile.dumps(d, indent=1, spacer="\\t"))
+    """
+    return _pprint(
+        d,
+        indent,
+        spacer,
+        quote,
+        newlinechar,
+        end_comment,
+        align_values,
+        separate_complex_types,
+        **kwargs,
+    )
+
+
+def validate(d: dict, version: (float | None) = None) -> list:
+    """
+    Validate a mappyfile dictionary by using the Mapfile schema.
+    An optional version number can be used to specify a specific
+    a Mapfile is valid for a specific MapServer version.
+
+    Parameters
+    ----------
+
+     d: dict
+        A Python dictionary based on the the mappyfile schema
+    version: float
+        The MapServer version number used to validate the Mapfile
+
+    Returns
+    -------
+
+    list
+        A list containing validation errors
+
+    """
+    v = Validator()
+    return v.validate(d, version=version)
+
+
+def _save(output_file: str, string: str) -> None:
+    with codecs.open(output_file, "w", encoding="utf-8") as f:
+        f.write(string)
+
+
+def _pprint(
+    d: dict,
+    indent: int,
+    spacer: str,
+    quote: str,
+    newlinechar: str,
+    end_comment: bool,
+    align_values: bool,
+    separate_complex_types: bool,
+    **kwargs,
+) -> str:
+    pp = PrettyPrinter(
+        indent=indent,
+        spacer=spacer,
+        quote=quote,
+        newlinechar=newlinechar,
+        end_comment=end_comment,
+        align_values=align_values,
+        separate_complex_types=separate_complex_types,
+        **kwargs,
+    )
+    return pp.pprint(d)
+
+
+def create(type: str, version=None) -> dict:
+    """
+    Create a new mappyfile object, using MapServer defaults (if any).
+
+    Parameters
+    ----------
+
+    s: type
+        The mappyfile type to be stored in the __type__ property
+
+    Returns
+    -------
+
+    dict
+        A Python dictionary representing the Mapfile object in the mappyfile format
+    """
+
+    # get the schema for this type
+
+    v = Validator()
+    try:
+        schema = v.get_versioned_schema(version=version, schema_name=type)
+    except IOError as exc:
+        raise SyntaxError("The mappyfile type '{type}' does not exist!") from exc
+
+    d = DefaultOrderedDict()
+    d["__type__"] = type
+
+    properties = sorted(schema["properties"].items())
+
+    for key, value in properties:
+        if "default" in value:
+            d[key] = value["default"]
+
+    return d
```

### Comparing `mappyfile-1.0.1/mappyfile.egg-info/PKG-INFO` & `mappyfile-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,157 +1,162 @@
-Metadata-Version: 2.1
-Name: mappyfile
-Version: 1.0.1
-Summary: A pure Python MapFile parser for working with MapServer
-Home-page: http://github.com/geographika/mappyfile
-Author: Seth Girvin
-Author-email: sethg@geographika.co.uk
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Text Processing :: Linguistic
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/x-rst
-Provides-Extra: lark_cython
-License-File: LICENSE
-
-mappyfile
-=========
-
-| |Version| |Docs| |Build Status| |Coveralls| |Appveyor Build Status| |Downloads|
-
-A pure Python parser for working with `MapServer <https://mapserver.org>`_ MapFiles, built using `Lark <https://github.com/lark-parser/lark>`__.
-mappyfile is an official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_.
-
-.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/OSGeo_community_small.png
-    :align: right
-
-mappyfile is used for formatting and validation in https://app.mapserverstudio.net/, and can be tested for free on any
-of your Mapfiles. If you find mappyfile useful please consider signing up for a professional account at 
-https://mapserverstudio.net/. This will help to fund maintenance and further development of both mappyfile and MapServer.
-
-Requirements
-------------
-
-* Python 3.8 or higher
-
-Installation
-------------
-
-mappyfile is available on `PyPI <https://pypi.org/project/mappyfile/>`_ (the Python Package Index), and can be installed using pip:
-
-.. code-block:: console
-
-    pip install mappyfile
-
-This will also install its required dependencies - `Lark <https://github.com/lark-parser/lark>`__, and 
-`jsonschema <https://github.com/python-jsonschema/jsonschema>`_. 
-
-To install the optional `lark-cython <https://github.com/lark-parser/lark_cython>`_ library
-for better performance on CPython you can run the following command:
-
-.. code-block:: console
-
-    pip install mappyfile[lark_cython]
-
-mappyfile is also available on `conda <https://anaconda.org/conda-forge/mappyfile>`_. Install as
-follows:
-
-.. code-block:: console
-
-    conda install -c conda-forge mappyfile
-
-Documentation
--------------
-
-Full documentation is available at http://mappyfile.readthedocs.io/en/latest/
-
-.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/class_parsed_small.png
-
-Usage
------
-
-From within Python scripts:
-
-.. code-block:: python
-
-    import mappyfile
-
-    mapfile = mappyfile.open("./docs/examples/raster.map")
-    
-    # update the map name
-    mapfile["name"] = "MyNewMap"
-
-    new_layer_string = """
-    LAYER
-        NAME 'land'
-        TYPE POLYGON
-        DATA '../data/vector/naturalearth/ne_110m_land'
-        CLASS
-            STYLE
-                COLOR 107 208 107
-                OUTLINECOLOR 2 2 2
-                WIDTH 1
-            END
-        END
-    END
-    """
-
-    layers = mapfile["layers"]
-
-    new_layer = mappyfile.loads(new_layer_string)
-
-    layers.insert(0, new_layer) # insert the new layer at any index in the Mapfile
-
-    for l in layers:
-        print("{} {}".format(l["name"], l["type"]))
-
-    print(mappyfile.dumps(mapfile, indent=1, spacer="\t"))
-
-Three command line tools are available - ``format``, ``validate``, and ``schema``:
-
-.. code-block:: bat
-
-    mappyfile format raster.map formatted_raster.map
-    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
-    mappyfile schema mapfile-schema-8-0.json --version=8.0
-
-Authors
--------
-
-* Seth Girvin `@geographika <https://github.com/geographika>`_
-* Erez Shinan `@erezsh <https://github.com/erezsh>`_
-
-Contributors
-------------
-
-* Julien Enselme `@jenselme <https://github.com/jenselme>`_
-* Loïc Gasser `@loicgasser <https://github.com/loicgasser>`_
-* Ian Turton `@ianturton <https://github.com/ianturton>`_
-* `@thorag76 <https://github.com/thorag76>`_
-* `@DonQueso89 <https://github.com/DonQueso89>`_
-* TC Haddad `@tchaddad <https://github.com/tchaddad>`_ (Conda support)
-
-.. |Version| image:: https://img.shields.io/pypi/v/mappyfile.svg
-   :target: https://pypi.python.org/pypi/mappyfile
-
-.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
-   :target: http://mappyfile.readthedocs.io/en/latest/
-
-.. |Build Status| image:: https://github.com/geographika/mappyfile/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/geographika/mappyfile/actions/workflows/main.yml
-
-.. |Appveyor Build Status| image:: https://ci.appveyor.com/api/projects/status/mk33l07478gfytwh?svg=true
-   :target: https://ci.appveyor.com/project/SethG/mappyfile
-
-.. |Coveralls| image:: https://coveralls.io/repos/github/geographika/mappyfile/badge.svg?branch=master
-    :target: https://coveralls.io/github/geographika/mappyfile?branch=master
-
-.. |Downloads| image:: https://static.pepy.tech/badge/mappyfile
-    :target: https://www.pepy.tech/projects/mappyfile
-    
+Metadata-Version: 2.1
+Name: mappyfile
+Version: 1.0.2
+Summary: A pure Python MapFile parser for working with MapServer
+Home-page: http://github.com/geographika/mappyfile
+Author: Seth Girvin
+Author-email: sethg@geographika.co.uk
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: lark>=1.1.5
+Requires-Dist: jsonschema>=4.18.0
+Requires-Dist: jsonref==1.1.0
+Requires-Dist: click
+Provides-Extra: lark-cython
+Requires-Dist: lark_cython>=0.0.14; extra == "lark-cython"
+
+mappyfile
+=========
+
+| |Version| |Docs| |Build Status| |Coveralls| |Appveyor Build Status| |Downloads|
+
+A pure Python parser for working with `MapServer <https://mapserver.org>`_ MapFiles, built using `Lark <https://github.com/lark-parser/lark>`__.
+mappyfile is an official `OSGeo Community Project <https://www.osgeo.org/projects/mappyfile/>`_.
+
+.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/OSGeo_community_small.png
+    :align: right
+
+mappyfile is used for formatting and validation in https://app.mapserverstudio.net/, and can be tested for free on any
+of your Mapfiles. If you find mappyfile useful please consider signing up for a professional account at 
+https://mapserverstudio.net/. This will help to fund maintenance and further development of both mappyfile and MapServer.
+
+Requirements
+------------
+
+* Python 3.8 or higher
+
+Installation
+------------
+
+mappyfile is available on `PyPI <https://pypi.org/project/mappyfile/>`_ (the Python Package Index), and can be installed using pip:
+
+.. code-block:: console
+
+    pip install mappyfile
+
+This will also install its required dependencies - `Lark <https://github.com/lark-parser/lark>`__, and 
+`jsonschema <https://github.com/python-jsonschema/jsonschema>`_. 
+
+To install the optional `lark-cython <https://github.com/lark-parser/lark_cython>`_ library
+for better performance on CPython you can run the following command:
+
+.. code-block:: console
+
+    pip install mappyfile[lark_cython]
+
+mappyfile is also available on `conda <https://anaconda.org/conda-forge/mappyfile>`_. Install as
+follows:
+
+.. code-block:: console
+
+    conda install -c conda-forge mappyfile
+
+Documentation
+-------------
+
+Full documentation is available at http://mappyfile.readthedocs.io/en/latest/
+
+.. image:: https://raw.githubusercontent.com/geographika/mappyfile/master/docs/images/class_parsed_small.png
+
+Usage
+-----
+
+From within Python scripts:
+
+.. code-block:: python
+
+    import mappyfile
+
+    mapfile = mappyfile.open("./docs/examples/raster.map")
+    
+    # update the map name
+    mapfile["name"] = "MyNewMap"
+
+    new_layer_string = """
+    LAYER
+        NAME 'land'
+        TYPE POLYGON
+        DATA '../data/vector/naturalearth/ne_110m_land'
+        CLASS
+            STYLE
+                COLOR 107 208 107
+                OUTLINECOLOR 2 2 2
+                WIDTH 1
+            END
+        END
+    END
+    """
+
+    layers = mapfile["layers"]
+
+    new_layer = mappyfile.loads(new_layer_string)
+
+    layers.insert(0, new_layer) # insert the new layer at any index in the Mapfile
+
+    for l in layers:
+        print("{} {}".format(l["name"], l["type"]))
+
+    print(mappyfile.dumps(mapfile, indent=1, spacer="\t"))
+
+Three command line tools are available - ``format``, ``validate``, and ``schema``:
+
+.. code-block:: bat
+
+    mappyfile format raster.map formatted_raster.map
+    mappyfile validate D:\ms-ogc-workshop\ms4w\apps\ms-ogc-workshop\**\*.map
+    mappyfile schema mapfile-schema-8-0.json --version=8.0
+
+Authors
+-------
+
+* Seth Girvin `@geographika <https://github.com/geographika>`_
+* Erez Shinan `@erezsh <https://github.com/erezsh>`_
+
+Contributors
+------------
+
+* Julien Enselme `@jenselme <https://github.com/jenselme>`_
+* Loïc Gasser `@loicgasser <https://github.com/loicgasser>`_
+* Ian Turton `@ianturton <https://github.com/ianturton>`_
+* `@thorag76 <https://github.com/thorag76>`_
+* `@DonQueso89 <https://github.com/DonQueso89>`_
+* TC Haddad `@tchaddad <https://github.com/tchaddad>`_ (Conda support)
+
+.. |Version| image:: https://img.shields.io/pypi/v/mappyfile.svg
+   :target: https://pypi.python.org/pypi/mappyfile
+
+.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat
+   :target: http://mappyfile.readthedocs.io/en/latest/
+
+.. |Build Status| image:: https://github.com/geographika/mappyfile/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/geographika/mappyfile/actions/workflows/main.yml
+
+.. |Appveyor Build Status| image:: https://ci.appveyor.com/api/projects/status/mk33l07478gfytwh?svg=true
+   :target: https://ci.appveyor.com/project/SethG/mappyfile
+
+.. |Coveralls| image:: https://coveralls.io/repos/github/geographika/mappyfile/badge.svg?branch=master
+    :target: https://coveralls.io/github/geographika/mappyfile?branch=master
+
+.. |Downloads| image:: https://static.pepy.tech/badge/mappyfile
+    :target: https://www.pepy.tech/projects/mappyfile
+
```

### Comparing `mappyfile-1.0.1/mappyfile.egg-info/SOURCES.txt` & `mappyfile-1.0.2/mappyfile.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 mappyfile/schemas/units.json
 mappyfile/schemas/validation.json
 mappyfile/schemas/web.json
 mappyfile/schemas/yesno.json
 tests/__init__.py
 tests/test_cli.py
 tests/test_comments.py
-tests/test_config.py
 tests/test_dictutils.py
 tests/test_errors.py
 tests/test_expressions.py
 tests/test_includes.py
 tests/test_map_collection.py
 tests/test_msautotest.py
 tests/test_ordereddict.py
```

### Comparing `mappyfile-1.0.1/pyproject.toml` & `mappyfile-1.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# black only uses the pyproject.toml so add settings here
-[tool.black]
-exclude = 'tests/mapfiles'
-
-[tool.mypy]
-exclude = [
-    'tests/mapfiles'
-]
-
-[[tool.mypy.overrides]]
-module = [
-    'jsonref',
-    'glob2',
-    'lark_cython',
-    'PIL',
-    'shapely.geometry'
-]
-ignore_missing_imports = true
-
-# Flake8 does not currently support pyproject.toml
-# without an additional dependency
-# see https://pypi.org/project/Flake8-pyproject/
-
-# [tool.flake8]
-# max-line-length = 160
-# extend-ignore = ['E203','W503']
-# exclude = [
-#     'build',
-#     'dist',
-#     'misc',
-#     'tests/mapfiles',
-#     'docs/_build']
-
-[tool.pytest.ini_options]
-testpaths = [
-    'tests',
-    'docs/examples',
-]
-# there is no ignore ini setting in pytest, but we can add command line options with addopts
-addopts  = ['--ignore=tests/mapfiles']
-# can remove the following as https://github.com/lark-parser/lark/pull/1285 has been merged
+# black only uses the pyproject.toml so add settings here
+[tool.black]
+exclude = 'tests/mapfiles'
+
+[tool.mypy]
+exclude = [
+    'tests/mapfiles'
+]
+
+[[tool.mypy.overrides]]
+module = [
+    'jsonref',
+    'glob2',
+    'lark_cython',
+    'PIL',
+    'shapely.geometry'
+]
+ignore_missing_imports = true
+
+# Flake8 does not currently support pyproject.toml
+# without an additional dependency
+# see https://pypi.org/project/Flake8-pyproject/
+
+# [tool.flake8]
+# max-line-length = 160
+# extend-ignore = ['E203','W503']
+# exclude = [
+#     'build',
+#     'dist',
+#     'misc',
+#     'tests/mapfiles',
+#     'docs/_build']
+
+[tool.pytest.ini_options]
+testpaths = [
+    'tests',
+    'docs/examples',
+]
+# there is no ignore ini setting in pytest, but we can add command line options with addopts
+addopts  = ['--ignore=tests/mapfiles']
+# can remove the following as https://github.com/lark-parser/lark/pull/1285 has been merged
 filterwarnings = 'ignore::DeprecationWarning:lark.*'
```

### Comparing `mappyfile-1.0.1/tests/test_comments.py` & `mappyfile-1.0.2/tests/test_comments.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-import collections
-import json
-import logging
-import pytest
-import mappyfile
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-from mappyfile.parser import Parser
-from typing import Any
-
-
-def test_comment():
-    d: dict[str, Any] = collections.OrderedDict()
-    d["name"] = "Test"
-    d["__type__"] = "layer"
-    d["__comments__"] = {"name": "# Test comment"}
-    print(json.dumps(d, indent=4))
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    exp = """LAYER
-NAME 'Test' # Test comment
-END"""
-    print(s)
-    assert s == exp
-
-
-def test_double_comment():
-    d: dict[str, Any] = collections.OrderedDict()
-    d["name"] = "Test"
-    d["__type__"] = "layer"
-    d["__comments__"] = {"name": "# Name comment", "type": "# Type comment"}
-
-    d["type"] = "polygon"
-
-    print(json.dumps(d, indent=4))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    exp = """LAYER
-NAME 'Test' # Name comment
-TYPE POLYGON # Type comment
-END"""
-    print(s)
-    assert s == exp
-
-
-def test_header_comment():
-    """
-    __type__ is used as the key for any object-level comments
-    """
-    d: dict[str, Any] = collections.OrderedDict()
-    d["name"] = "Test"
-    d["__type__"] = "layer"
-    d["__comments__"] = {"__type__": "# Layer comment"}
-
-    print(json.dumps(d, indent=4))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    print(s)
-    exp = """# Layer comment
-LAYER
-NAME 'Test'
-END"""
-    assert s == exp
-
-
-def test_header_list_comments():
-    """
-    __type__ is used as the key for any object-level comments
-    """
-    d: dict[str, Any] = collections.OrderedDict()
-    d["name"] = "Test"
-    d["__type__"] = "layer"
-    d["__comments__"] = {"__type__": ["# Layer comment 1", "# Layer comment 2"]}
-    print(json.dumps(d, indent=4))
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    exp = """# Layer comment 1
-# Layer comment 2
-LAYER
-NAME 'Test'
-END"""
-    assert s == exp
-
-
-def test_example_comment_dict():
-    d = {
-        "__type__": "map",
-        "__comments__": {"__type__": ["# Map comment 1", "# Map comment 2"]},
-        "name": "Test",
-        "layers": [
-            {
-                "__type__": "layer",
-                "__comments__": {
-                    "__type__": "# Layer comment",
-                    "type": ["# This is a polygon!", "# Another comment"],
-                },
-                "type": "POLYGON",
-            }
-        ],
-    }
-    pp = PrettyPrinter(indent=4, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    print(s)
-
-
-def test_header_comment2():
-    s = """
-    # Map comment 1
-    # Map comment 2
-    MAP
-        # comment 2
-        NAME "Test" # name comment
-        # post name comment
-    END"""
-
-    p = Parser(include_comments=True)
-    ast = p.parse(s)
-    print(p._comments)
-    print(ast.pretty())
-    m = MapfileToDict(include_position=True, include_comments=True)
-    d = m.transform(ast)
-    print(json.dumps(d, indent=4))
-
-    pp = PrettyPrinter(indent=4, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    print(s)
-
-
-def test_comment_parsing():
-    s = """
-    # Map comment 1
-    # Map comment 2
-    MAP
-    NAME 'Test' # Name comment
-    # Layer comment
-    LAYER
-    TYPE POLYGON # This is a polygon!
-    END
-    END"""
-
-    p = Parser(include_comments=True)
-    m = MapfileToDict(include_position=False, include_comments=True)
-    ast = p.parse(s)
-    print(p._comments)
-    assert len(p._comments) == 5
-    print(ast.pretty())
-    d = m.transform(ast)  # transform the rest
-    print(json.dumps(d, indent=4))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    print(s)
-
-
-def test_metadata_comment():
-    txt = """MAP
-    # metadata comment
-    # on two lines
-    METADATA
-        # another comment
-        'wms_title' 'Test simple wms' # prop comment
-    END
-    END"""
-    d = mappyfile.loads(txt, include_comments=True, include_position=False)
-    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
-    expected = """MAP
-# metadata comment
-# on two lines
-METADATA
-'wms_title' 'Test simple wms' # another comment # prop comment
-END
-END"""
-    assert s == expected
-
-
-def test_projection_comment():
-    txt = """MAP
-    PROJECTION # block comment
-        "init=epsg:3857" # inline comment
-    END
-    NAME "test"
-    # header comment
-    LAYER
-        NAME "test" # attr comment
-    END
-END"""
-
-    d = mappyfile.loads(txt, include_comments=True, include_position=False)
-    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
-    expected = """MAP
-PROJECTION
-# block comment # inline comment
-'init=epsg:3857'
-END
-NAME 'test'
-# header comment
-LAYER
-NAME 'test' # attr comment
-END
-END"""
-
-    assert s == expected
-
-
-def test_metadata_duplicated_key_comment():
-    txt = """METADATA
-        'wms_title' 'Title1' # title1
-        'wms_title' 'Title2' # title2
-END"""
-    d = mappyfile.loads(txt, include_comments=True, include_position=False)
-    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
-    expected = """METADATA
-'wms_title' 'Title2' # title2
-END"""
-
-    assert s == expected
-
-
-def test_metadata_mixed_case_comment():
-    txt = """
-    METADATA
-        'wms_TITLE' 'Title1' # title1
-    END
-    """
-
-    d = mappyfile.loads(txt, include_comments=True, include_position=False)
-    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
-    expected = """METADATA
-'wms_title' 'Title1' # title1
-END"""
-
-    assert s == expected
-
-
-def test_metadata_unquoted_comment():
-    txt = """
-    METADATA
-      WMS_TITLE "Minor Civil Divisions" # comment
-    END
-    """
-
-    d = mappyfile.loads(txt, include_comments=True, include_position=False)
-    s = mappyfile.dumps(d, indent=0, quote='"', newlinechar="\n")
-    expected = """METADATA
-"wms_title" "Minor Civil Divisions" # comment
-END"""
-
-    assert s == expected
-
-
-def test_cstyle_comment():
-    s = """
-    MAP
-        /*
-        C-style comment 1
-        */
-        NAME "Test"
-    END
-    """
-    d = mappyfile.loads(s, include_comments=True, include_position=False)
-    p = Parser(include_comments=True)
-    m = MapfileToDict(include_position=False, include_comments=True)
-    ast = p.parse(s)
-    print(p._comments)
-    print(ast.pretty())
-    d = m.transform(ast)  # transform the rest
-    print(json.dumps(d, indent=4))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    print(s)
-    assert len(p._comments) == 1
-
-
-def test_cstyle_comment_start():
-    """
-    CCOMMENT and REGEXP1.2 could cause ambiguities?
-    Without adding priorities the following error may occur
-
-    UnexpectedToken: Unexpected token Token(REGEXP1, u'/*\n        C-style comment 2\n        */') at line 6, column 9.
-
-    The following snippet will produce an invalid Mapfile, as the start of the CCOMMENT is commented out with the #
-    Users will have to be careful when including comments in the output
-
-    MAP
-    NAME 'Test' # name comment /*
-            C-style comment 2
-            */
-    END
-
-    """
-    s = """
-    /*
-    C-style comment 1
-    */
-    MAP
-        /*
-        C-style comment 2
-        */
-        NAME "Test" # name comment
-    END
-    """
-    d = mappyfile.loads(s, include_comments=True, include_position=False)
-    p = Parser(include_comments=True)
-    m = MapfileToDict(include_position=False, include_comments=True)
-    ast = p.parse(s)
-    print(p._comments)
-    print(ast.pretty())
-    d = m.transform(ast)  # transform the rest
-    print(json.dumps(d, indent=4))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
-    s = pp.pprint(d)
-    assert len(p._comments) == 3
-
-
-def run_tests():
-    pytest.main(["-s", "tests/test_comments.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    logging.getLogger("mappyfile").setLevel(logging.DEBUG)
-    # test_comment_parsing()
-    # test_metadata_comment()
-    run_tests()
-    print("Done!")
+import collections
+import json
+import logging
+import pytest
+import mappyfile
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.transformer import MapfileToDict
+from mappyfile.parser import Parser
+from typing import Any
+
+
+def test_comment():
+    d: dict[str, Any] = collections.OrderedDict()
+    d["name"] = "Test"
+    d["__type__"] = "layer"
+    d["__comments__"] = {"name": "# Test comment"}
+    print(json.dumps(d, indent=4))
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    exp = """LAYER
+NAME 'Test' # Test comment
+END"""
+    print(s)
+    assert s == exp
+
+
+def test_double_comment():
+    d: dict[str, Any] = collections.OrderedDict()
+    d["name"] = "Test"
+    d["__type__"] = "layer"
+    d["__comments__"] = {"name": "# Name comment", "type": "# Type comment"}
+
+    d["type"] = "polygon"
+
+    print(json.dumps(d, indent=4))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    exp = """LAYER
+NAME 'Test' # Name comment
+TYPE POLYGON # Type comment
+END"""
+    print(s)
+    assert s == exp
+
+
+def test_header_comment():
+    """
+    __type__ is used as the key for any object-level comments
+    """
+    d: dict[str, Any] = collections.OrderedDict()
+    d["name"] = "Test"
+    d["__type__"] = "layer"
+    d["__comments__"] = {"__type__": "# Layer comment"}
+
+    print(json.dumps(d, indent=4))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    print(s)
+    exp = """# Layer comment
+LAYER
+NAME 'Test'
+END"""
+    assert s == exp
+
+
+def test_header_list_comments():
+    """
+    __type__ is used as the key for any object-level comments
+    """
+    d: dict[str, Any] = collections.OrderedDict()
+    d["name"] = "Test"
+    d["__type__"] = "layer"
+    d["__comments__"] = {"__type__": ["# Layer comment 1", "# Layer comment 2"]}
+    print(json.dumps(d, indent=4))
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    exp = """# Layer comment 1
+# Layer comment 2
+LAYER
+NAME 'Test'
+END"""
+    assert s == exp
+
+
+def test_example_comment_dict():
+    d = {
+        "__type__": "map",
+        "__comments__": {"__type__": ["# Map comment 1", "# Map comment 2"]},
+        "name": "Test",
+        "layers": [
+            {
+                "__type__": "layer",
+                "__comments__": {
+                    "__type__": "# Layer comment",
+                    "type": ["# This is a polygon!", "# Another comment"],
+                },
+                "type": "POLYGON",
+            }
+        ],
+    }
+    pp = PrettyPrinter(indent=4, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    print(s)
+
+
+def test_header_comment2():
+    s = """
+    # Map comment 1
+    # Map comment 2
+    MAP
+        # comment 2
+        NAME "Test" # name comment
+        # post name comment
+    END"""
+
+    p = Parser(include_comments=True)
+    ast = p.parse(s)
+    print(p._comments)
+    print(ast.pretty())
+    m = MapfileToDict(include_position=True, include_comments=True)
+    d = m.transform(ast)
+    print(json.dumps(d, indent=4))
+
+    pp = PrettyPrinter(indent=4, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    print(s)
+
+
+def test_comment_parsing():
+    s = """
+    # Map comment 1
+    # Map comment 2
+    MAP
+    NAME 'Test' # Name comment
+    # Layer comment
+    LAYER
+    TYPE POLYGON # This is a polygon!
+    END
+    END"""
+
+    p = Parser(include_comments=True)
+    m = MapfileToDict(include_position=False, include_comments=True)
+    ast = p.parse(s)
+    print(p._comments)
+    assert len(p._comments) == 5
+    print(ast.pretty())
+    d = m.transform(ast)  # transform the rest
+    print(json.dumps(d, indent=4))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    print(s)
+
+
+def test_metadata_comment():
+    txt = """MAP
+    # metadata comment
+    # on two lines
+    METADATA
+        # another comment
+        'wms_title' 'Test simple wms' # prop comment
+    END
+    END"""
+    d = mappyfile.loads(txt, include_comments=True, include_position=False)
+    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
+    expected = """MAP
+# metadata comment
+# on two lines
+METADATA
+'wms_title' 'Test simple wms' # another comment # prop comment
+END
+END"""
+    assert s == expected
+
+
+def test_projection_comment():
+    txt = """MAP
+    PROJECTION # block comment
+        "init=epsg:3857" # inline comment
+    END
+    NAME "test"
+    # header comment
+    LAYER
+        NAME "test" # attr comment
+    END
+END"""
+
+    d = mappyfile.loads(txt, include_comments=True, include_position=False)
+    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
+    expected = """MAP
+PROJECTION
+# block comment # inline comment
+'init=epsg:3857'
+END
+NAME 'test'
+# header comment
+LAYER
+NAME 'test' # attr comment
+END
+END"""
+
+    assert s == expected
+
+
+def test_metadata_duplicated_key_comment():
+    txt = """METADATA
+        'wms_title' 'Title1' # title1
+        'wms_title' 'Title2' # title2
+END"""
+    d = mappyfile.loads(txt, include_comments=True, include_position=False)
+    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
+    expected = """METADATA
+'wms_title' 'Title2' # title2
+END"""
+
+    assert s == expected
+
+
+def test_metadata_mixed_case_comment():
+    txt = """
+    METADATA
+        'wms_TITLE' 'Title1' # title1
+    END
+    """
+
+    d = mappyfile.loads(txt, include_comments=True, include_position=False)
+    s = mappyfile.dumps(d, indent=0, quote="'", newlinechar="\n")
+    expected = """METADATA
+'wms_title' 'Title1' # title1
+END"""
+
+    assert s == expected
+
+
+def test_metadata_unquoted_comment():
+    txt = """
+    METADATA
+      WMS_TITLE "Minor Civil Divisions" # comment
+    END
+    """
+
+    d = mappyfile.loads(txt, include_comments=True, include_position=False)
+    s = mappyfile.dumps(d, indent=0, quote='"', newlinechar="\n")
+    expected = """METADATA
+"wms_title" "Minor Civil Divisions" # comment
+END"""
+
+    assert s == expected
+
+
+def test_cstyle_comment():
+    s = """
+    MAP
+        /*
+        C-style comment 1
+        */
+        NAME "Test"
+    END
+    """
+    d = mappyfile.loads(s, include_comments=True, include_position=False)
+    p = Parser(include_comments=True)
+    m = MapfileToDict(include_position=False, include_comments=True)
+    ast = p.parse(s)
+    print(p._comments)
+    print(ast.pretty())
+    d = m.transform(ast)  # transform the rest
+    print(json.dumps(d, indent=4))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    print(s)
+    assert len(p._comments) == 1
+
+
+def test_cstyle_comment_start():
+    """
+    CCOMMENT and REGEXP1.2 could cause ambiguities?
+    Without adding priorities the following error may occur
+
+    UnexpectedToken: Unexpected token Token(REGEXP1, u'/*\n        C-style comment 2\n        */') at line 6, column 9.
+
+    The following snippet will produce an invalid Mapfile, as the start of the CCOMMENT is commented out with the #
+    Users will have to be careful when including comments in the output
+
+    MAP
+    NAME 'Test' # name comment /*
+            C-style comment 2
+            */
+    END
+
+    """
+    s = """
+    /*
+    C-style comment 1
+    */
+    MAP
+        /*
+        C-style comment 2
+        */
+        NAME "Test" # name comment
+    END
+    """
+    d = mappyfile.loads(s, include_comments=True, include_position=False)
+    p = Parser(include_comments=True)
+    m = MapfileToDict(include_position=False, include_comments=True)
+    ast = p.parse(s)
+    print(p._comments)
+    print(ast.pretty())
+    d = m.transform(ast)  # transform the rest
+    print(json.dumps(d, indent=4))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n")
+    s = pp.pprint(d)
+    assert len(p._comments) == 3
+
+
+def run_tests():
+    pytest.main(["-s", "tests/test_comments.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    logging.getLogger("mappyfile").setLevel(logging.DEBUG)
+    # test_comment_parsing()
+    # test_metadata_comment()
+    run_tests()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_config.py` & `mappyfile-1.0.2/tests/test_includes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,127 @@
-import logging
-import json
-import pytest
-from mappyfile.parser import Parser
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-from mappyfile.validator import Validator
-
-
-def output(s, include_position=True, schema_name="map"):
-    """
-    Parse, transform, validate, and pretty print
-    the result
-    """
-    p = Parser(is_config=True)
-    m = MapfileToDict(include_position=include_position)
-    ast = p.parse(s)
-    logging.debug(ast.pretty())
-    d = m.transform(ast)
-    logging.debug(json.dumps(d, indent=4))
-    v = Validator()
-    errors = v.validate(d, schema_name=schema_name)
-    logging.error(errors)
-    assert len(errors) == 0
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    # pp = PrettyPrinter()
-    s = pp.pprint(d)
-    logging.debug(s)
-    return s
-
-
-def test_config_file():
-    s = r"""
-    CONFIG
-      ENV
-        "ms_map_pattern" "."
-      END
-      MAPS
-        "itasca" "C:/MapServer/apps/itasca.map"
-      END
-      PLUGINS
-        "mssql" "C:/MapServer/bin/ms/plugins/mssql2008/msplugin_mssql2008.dll"
-      END
-    END
-    """
-
-    print(output(s, schema_name="config"))
-    exp = (
-        "CONFIG "
-        "ENV \"MS_MAP_PATTERN\" '.' END "
-        "MAPS \"ITASCA\" 'C:/MapServer/apps/itasca.map' END "
-        "PLUGINS \"MSSQL\" 'C:/MapServer/bin/ms/plugins/mssql2008/msplugin_mssql2008.dll' END "
-        "END"
-    )
-    # exp = "CONFIG ENV MS_MAP_PATTERN '.' END MAPS ITASCA 'C:/MapServer/apps/itasca.map' END PLUGINS ""MSSQL"" 'C:/MapServer/bin/ms/plugins/mssql2008/msplugin_mssql2008.dll' END END"    
-    assert output(s, schema_name="config") == exp
-
-
-def run_tests():
-    pytest.main(["tests/test_config.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    run_tests()
-    print("Done!")
+import json
+import logging
+import pytest
+import mappyfile
+from mappyfile.parser import Parser
+from mappyfile.transformer import MapfileToDict
+from mappyfile.pprint import PrettyPrinter
+
+
+def test_includes():
+    p = Parser()
+
+    ast = p.parse_file("./tests/samples/include1.map")
+    m = MapfileToDict()
+
+    d = m.transform(ast)  # works
+    print(mappyfile.dumps(d))
+    assert d["name"] == "include_test"
+
+
+def test_include_from_string():
+    """
+    Check that a file is correctly included when parsing text
+    and that the current working directory is used as the root path
+    for includes - see https://github.com/geographika/mappyfile/issues/55
+    """
+    s = """
+    MAP
+        INCLUDE "tests/samples/include3.map"
+    END
+    """
+
+    d = mappyfile.loads(s, expand_includes=True)
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    output = pp.pprint(d)
+    expected = "MAP NAME 'test' END"
+    assert output == expected
+
+
+def test_includes_nested_path():
+    p = Parser()
+
+    ast = p.parse_file("./tests/samples/include1_nested_path.map")
+    m = MapfileToDict()
+
+    d = m.transform(ast)  # works
+    print(mappyfile.dumps(d))
+
+
+def test_includes_relative_path():
+    """
+    File location can be given as a full path to the file, or (in MapServer >= 4.10.1) as a
+    path relative to the mapfile.
+    http://mapserver.org/mapfile/include.html
+    """
+    p = Parser()
+
+    ast = p.parse_file("./tests/samples/include4.map")
+    m = MapfileToDict()
+
+    d = m.transform(ast)  # works
+    print(mappyfile.dumps(d))
+
+
+def test_includes_max_recursion():
+    p = Parser()
+
+    with pytest.raises(Exception) as excinfo:
+        p.parse_file("./tests/samples/include1_recursive.map")
+
+    assert "Maximum nested include exceeded" in str(excinfo.value)
+
+
+def test_includes_no_expand():
+    """
+    https://github.com/geographika/mappyfile/issues/39
+    """
+    s = """
+    MAP
+        INCLUDE "includes/mymapfile.map"
+    END
+    """
+
+    d = mappyfile.loads(s, expand_includes=False)
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    output = pp.pprint(d)
+
+    expected = "MAP INCLUDE 'includes/mymapfile.map' END"
+    assert output == expected
+
+
+def test_two_includes():
+    s = """
+    MAP
+        INCLUDE "include1.txt"
+        INCLUDE "include2.txt"
+    END
+    """
+
+    d = mappyfile.loads(s, expand_includes=False)
+    logging.debug(json.dumps(d, indent=4))
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    output = pp.pprint(d)
+    print(output)
+    expected = "MAP INCLUDE 'include1.txt' INCLUDE 'include2.txt' END"
+    assert output == expected
+
+
+def test_include_from_filehandle():
+    fn = "./tests/samples/include1.map"
+
+    with open(fn) as f:
+        d = mappyfile.load(f)
+        assert d["name"] == "include_test"
+        print(mappyfile.dumps(d))
+
+
+def run_tests():
+    pytest.main(["tests/test_includes.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    logging.getLogger("mappyfile").setLevel(logging.INFO)
+    # run_tests()
+    test_include_from_filehandle()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_expressions.py` & `mappyfile-1.0.2/tests/test_expressions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,460 +1,460 @@
-# -*- coding: utf-8 -*-
-import logging
-import json
-import inspect
-import pytest
-from mappyfile.parser import Parser
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-
-
-def output(s):
-    """
-    Parse, transform, and pretty print
-    the result
-    """
-    p = Parser()
-    m = MapfileToDict(include_position=True)
-
-    # https://stackoverflow.com/questions/900392/getting-the-caller-function-name-inside-another-function-in-python
-    logging.info(inspect.stack()[1][3])
-
-    ast = p.parse(s)
-    logging.debug(ast.pretty())
-    d = m.transform(ast)
-    logging.debug(json.dumps(d, indent=4))
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    s = pp.pprint(d)
-    logging.debug(s)
-    return s
-
-
-def check_result(s):
-    try:
-        s2 = output(s)
-        assert s == s2
-    except AssertionError:
-        logging.info(s)
-        logging.info(s2)
-        raise
-
-
-def test_class_expression1():
-    s = """
-    CLASS
-      TEXT ([area])
-    END
-    """
-    exp = "CLASS TEXT ([area]) END"
-    assert output(s) == exp
-
-
-def test_class_expression2():
-    r"""
-    shp2img -m C:\Temp\msautotest\query\text.tmp.map  -l text_test002 -o c:\temp\tmp_onl0lk.png
-    """
-    s = """
-    CLASS
-      TEXT ("[area]")
-    END
-    """
-    exp = 'CLASS TEXT ("[area]") END'
-    assert output(s) == exp
-
-
-def test_complex_class_expression():
-    s = """
-    CLASS
-      TEXT ("Area is: " + tostring([area],"%.2f"))
-    END
-    """
-    exp = """CLASS TEXT ("Area is: " + (tostring([area],"%.2f"))) END"""
-    assert output(s) == exp
-
-
-def test_or_expressions():
-    """
-    See http://www.mapserver.org/mapfile/expressions.html#expressions
-    """
-
-    s = """
-    CLASS
-        EXPRESSION ("[style_class]" = "10" OR "[style_class]" = "20")
-    END
-    """
-
-    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) OR ( "[style_class]" = "20" ) ) END'
-    assert output(s) == exp
-
-    s = """
-    CLASS
-        EXPRESSION ("[style_class]" = "10" || "[style_class]" = "20")
-    END
-    """
-
-    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) OR ( "[style_class]" = "20" ) ) END'
-    assert output(s) == exp
-
-
-def test_and_expressions():
-    s = """
-    CLASS
-        EXPRESSION ("[style_class]" = "10" AND "[style_class]" = "20")
-    END
-    """
-
-    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) AND ( "[style_class]" = "20" ) ) END'
-    assert output(s) == exp
-
-    s = """
-    CLASS
-        EXPRESSION ("[style_class]" = "10" && "[style_class]" = "20")
-    END
-    """
-
-    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) AND ( "[style_class]" = "20" ) ) END'
-    assert output(s) == exp
-
-
-def test_not_expressions():
-    s = """
-    CLASS
-        EXPRESSION NOT("[style_class]" = "20")
-    END
-    """
-
-    exp = 'CLASS EXPRESSION NOT ( "[style_class]" = "20" ) END'
-    assert output(s) == exp
-
-    s = """
-    CLASS
-        EXPRESSION !("[style_class]" = "20")
-    END
-    """
-
-    exp = 'CLASS EXPRESSION NOT ( "[style_class]" = "20" ) END'
-    assert output(s) == exp
-
-
-def test_runtime_expression():
-    s = """
-    CLASS
-      EXPRESSION ( [EPPL_Q100_] = %eppl% )
-    END
-    """
-    exp = "CLASS EXPRESSION ( [EPPL_Q100_] = %eppl% ) END"
-    # print(output(s))
-    assert output(s) == exp
-
-
-def test_ne_comparison():
-    """
-    IS NOT is not valid
-    NE (Not Equals) should be used instead
-    """
-    s = """
-    CLASS
-        # EXPRESSION ( "[building]" IS NOT NULL) # incorrect syntax
-        EXPRESSION ( "[building]" NE NULL)
-    END
-    """
-    exp = 'CLASS EXPRESSION ( "[building]" NE NULL ) END'
-    assert output(s) == exp
-
-
-def test_eq_comparison():
-    """
-    Case is not changed for comparison (EQ/eq stay the same)
-    Uses Earley
-    """
-    s = """
-    CLASS
-        EXPRESSION ( "[building]" eq NULL)
-    END
-    """
-    exp = 'CLASS EXPRESSION ( "[building]" eq NULL ) END'
-    # print(output(s))
-    assert output(s) == exp
-
-
-def test_expression():
-    """
-    Addressed in issue #27, now parses successfully.
-    """
-    s = """
-    CLASS
-        EXPRESSION ('[construct]' ~* /Br.*$/)
-        STYLE
-            ANGLE 360
-        END
-    END
-    """
-    exp = "CLASS EXPRESSION ( '[construct]' ~* /Br.*$/ ) STYLE ANGLE 360 END END"
-    assert output(s) == exp
-
-
-def test_list_expression():
-    """
-    See issue #27
-    """
-    s = """
-    CLASS
-        EXPRESSION /NS_Bahn|NS_BahnAuto/
-    END
-    """
-    exp = "CLASS EXPRESSION /NS_Bahn|NS_BahnAuto/ END"
-    assert output(s) == exp
-
-
-def test_numerical_operator_ge_expression():
-    s = """
-    CLASS
-        EXPRESSION ([power] ge 10000)
-    END
-    """
-    exp = "CLASS EXPRESSION ( [power] ge 10000 ) END"
-    assert output(s) == exp
-
-
-def test_numerical_operator_gt_expression():
-    s = """
-    CLASS
-        EXPRESSION ([power] gt 10000)
-    END
-    """
-    exp = "CLASS EXPRESSION ( [power] gt 10000 ) END"
-    assert output(s) == exp
-
-
-def test_numerical_operator_le_expression():
-    s = """
-    CLASS
-        EXPRESSION ([power] le 100)
-    END
-    """
-    exp = "CLASS EXPRESSION ( [power] le 100 ) END"
-    assert output(s) == exp
-
-
-def test_numerical_operator_lt_expression():
-    s = """
-    CLASS
-        EXPRESSION ([power] lt 100)
-    END
-    """
-    exp = "CLASS EXPRESSION ( [power] lt 100 ) END"
-    assert output(s) == exp
-
-
-def test_divide():
-    """
-    Not sure if these should be in brackets or not
-    http://mapserver.org/mapfile/expressions.html
-    Implies with brackets will return a boolean value
-    and without will return a numeric value
-    """
-    s = """
-    CLASS
-        EXPRESSION ([field1] / [field2])
-    END
-    """
-    exp = "CLASS EXPRESSION ([field1] / [field2]) END"
-    assert output(s) == exp
-
-
-def test_multiply():
-    s = """
-    CLASS
-        EXPRESSION ([field1] * [field2])
-    END
-    """
-    exp = "CLASS EXPRESSION ([field1] * [field2]) END"
-    assert output(s) == exp
-
-
-def test_negation():
-    """
-    TODO - check the exact syntax for this
-    """
-    s = """
-    CLASS
-        EXPRESSION (-[field1])
-    END
-    """
-    exp = "CLASS EXPRESSION (-[field1]) END"
-    assert output(s) == exp
-
-
-def test_pointless_plus():
-    # Based on test_negation
-    s = """
-    CLASS
-        EXPRESSION (+[field1])
-    END
-    """
-    exp = "CLASS EXPRESSION ([field1]) END"
-    assert output(s) == exp
-
-
-def test_power():
-    s = """
-    CLASS
-        EXPRESSION ([field1] ^ [field2])
-    END
-    """
-    exp = "CLASS EXPRESSION ([field1] ^ [field2]) END"
-    assert output(s) == exp
-
-
-def test_divide_expression():
-    """
-    http://mapserver.org/mapfile/expressions.html
-    Also - * and ^
-    """
-    s = """
-    CLASS
-        EXPRESSION ([field1] / [field2] > 0.1)
-    END
-    """
-    exp = "CLASS EXPRESSION ( [field1] / [field2] > 0.1 ) END"
-    assert output(s) == exp
-
-
-def test_modulo_expression():
-    """
-    Not currently documented at http://mapserver.org/mapfile/expressions.html
-    """
-    s = """
-    CLASS
-        EXPRESSION  ( ([height] % 50) = 0 )
-    END
-    """
-    exp = "CLASS EXPRESSION ( ( [height] % 50 ) = 0 ) END"
-    assert output(s) == exp
-
-
-def test_escaped_string():
-    """
-    http://mapserver.org/mapfile/expressions.html#quotes-escaping-in-strings
-    Starting with MapServer 6.0 you don't need to escape single quotes within double quoted strings
-    and you don't need to escape double quotes within single quoted strings
-    """
-
-    s = r"""
-    CLASS
-        EXPRESSION "National \"hero\" statue"
-    END
-    """
-    exp = """CLASS EXPRESSION 'National \\"hero\\" statue' END"""
-    assert output(s) == exp
-
-
-def test_list_expression_alt():
-    """
-    See issue #38
-    http://mapserver.org/mapfile/expressions.html#list-expressions
-    These expressions are much more performant in MapServer
-    List expressions do not support quote escaping, or attribute values that contain a comma in them.
-
-    To activate them enclose a comma separated list of values between {}, without adding quotes
-    or extra spaces.
-    """
-    s = """
-    CLASS
-        EXPRESSION {2_Klass,Rte2etr}
-    END
-    """
-    exp = "CLASS EXPRESSION {2_Klass,Rte2etr} END"
-    assert output(s) == exp
-
-    s = """
-    CLASS
-        EXPRESSION {2_Klass,class with space}
-    END
-    """
-    exp = "CLASS EXPRESSION {2_Klass,class with space} END"
-    assert output(s) == exp
-
-
-def test_class_expression_oddname():
-    s = """
-    CLASS
-      TEXT ([area:ian])
-    END
-    """
-    exp = "CLASS TEXT ([area:ian]) END"
-    assert output(s) == exp
-
-
-def test_class_not_expression_brackets():
-    """
-    See issue #85 - coding of NOT logical expressions #85
-    Each expression should be bracketed independently and any NOT
-    clause should be outside the brackets
-    """
-    s = """
-    CLASS
-      EXPRESSION (("[TIME]" eq 'NOW') AND NOT ("[TYPE]" ~ "(something|completely|different)"))
-    END
-    """
-    exp = """CLASS EXPRESSION ( ( "[TIME]" eq 'NOW' ) AND NOT ( "[TYPE]" ~ "(something|completely|different)" ) ) END"""
-    print(output(s))
-    assert output(s) == exp
-
-
-def test_class_not_expression_no_brackets():
-    """
-    See issue #85 - coding of NOT logical expressions #85
-    This parses successfully in MapServer but not in mappyfile
-    """
-    s = """
-    CLASS
-      EXPRESSION ("[TIME]" eq 'NOW' AND NOT "[TYPE]" ~ "(something|completely|different)")
-    END
-    """
-    exp = """CLASS EXPRESSION ( ( "[TIME]" eq 'NOW' ) AND NOT ( "[TYPE]" ~ "(something|completely|different)" ) ) END"""
-    assert output(s) == exp
-
-
-def test_unquoted_unicode_string():
-    """
-    See pull request #92 - French unquoted string
-    """
-    s = """
-    CLASS
-      EXPRESSION {Aérodrome,Aéroport,Héliport,Base spatiale}
-    END
-    """
-
-    exp = """CLASS EXPRESSION {Aérodrome,Aéroport,Héliport,Base spatiale} END"""
-    assert output(s) == exp
-
-
-def test_list_with_apostrophe():
-    """
-    See https://github.com/geographika/mappyfile/issues/120
-    """
-    s = """
-    CLASS
-      EXPRESSION {bla,d'apostrophe}
-    END
-    """
-
-    exp = """CLASS EXPRESSION {bla,d'apostrophe} END"""
-    assert output(s) == exp
-
-
-def run_tests():
-    r"""
-    Need to comment out the following line in C:\VirtualEnvs\mappyfile\Lib\site-packages\pep8.py
-    #stdin_get_value = sys.stdin.read
-    Or get AttributeError: '_ReplInput' object has no attribute 'read'
-    """
-    pytest.main(["tests/test_expressions.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    test_list_with_apostrophe()
-    # run_tests()
-    print("Done!")
+# -*- coding: utf-8 -*-
+import logging
+import json
+import inspect
+import pytest
+from mappyfile.parser import Parser
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.transformer import MapfileToDict
+
+
+def output(s):
+    """
+    Parse, transform, and pretty print
+    the result
+    """
+    p = Parser()
+    m = MapfileToDict(include_position=True)
+
+    # https://stackoverflow.com/questions/900392/getting-the-caller-function-name-inside-another-function-in-python
+    logging.info(inspect.stack()[1][3])
+
+    ast = p.parse(s)
+    logging.debug(ast.pretty())
+    d = m.transform(ast)
+    logging.debug(json.dumps(d, indent=4))
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    s = pp.pprint(d)
+    logging.debug(s)
+    return s
+
+
+def check_result(s):
+    try:
+        s2 = output(s)
+        assert s == s2
+    except AssertionError:
+        logging.info(s)
+        logging.info(s2)
+        raise
+
+
+def test_class_expression1():
+    s = """
+    CLASS
+      TEXT ([area])
+    END
+    """
+    exp = "CLASS TEXT ([area]) END"
+    assert output(s) == exp
+
+
+def test_class_expression2():
+    r"""
+    shp2img -m C:\Temp\msautotest\query\text.tmp.map  -l text_test002 -o c:\temp\tmp_onl0lk.png
+    """
+    s = """
+    CLASS
+      TEXT ("[area]")
+    END
+    """
+    exp = 'CLASS TEXT ("[area]") END'
+    assert output(s) == exp
+
+
+def test_complex_class_expression():
+    s = """
+    CLASS
+      TEXT ("Area is: " + tostring([area],"%.2f"))
+    END
+    """
+    exp = """CLASS TEXT ("Area is: " + (tostring([area],"%.2f"))) END"""
+    assert output(s) == exp
+
+
+def test_or_expressions():
+    """
+    See http://www.mapserver.org/mapfile/expressions.html#expressions
+    """
+
+    s = """
+    CLASS
+        EXPRESSION ("[style_class]" = "10" OR "[style_class]" = "20")
+    END
+    """
+
+    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) OR ( "[style_class]" = "20" ) ) END'
+    assert output(s) == exp
+
+    s = """
+    CLASS
+        EXPRESSION ("[style_class]" = "10" || "[style_class]" = "20")
+    END
+    """
+
+    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) OR ( "[style_class]" = "20" ) ) END'
+    assert output(s) == exp
+
+
+def test_and_expressions():
+    s = """
+    CLASS
+        EXPRESSION ("[style_class]" = "10" AND "[style_class]" = "20")
+    END
+    """
+
+    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) AND ( "[style_class]" = "20" ) ) END'
+    assert output(s) == exp
+
+    s = """
+    CLASS
+        EXPRESSION ("[style_class]" = "10" && "[style_class]" = "20")
+    END
+    """
+
+    exp = 'CLASS EXPRESSION ( ( "[style_class]" = "10" ) AND ( "[style_class]" = "20" ) ) END'
+    assert output(s) == exp
+
+
+def test_not_expressions():
+    s = """
+    CLASS
+        EXPRESSION NOT("[style_class]" = "20")
+    END
+    """
+
+    exp = 'CLASS EXPRESSION NOT ( "[style_class]" = "20" ) END'
+    assert output(s) == exp
+
+    s = """
+    CLASS
+        EXPRESSION !("[style_class]" = "20")
+    END
+    """
+
+    exp = 'CLASS EXPRESSION NOT ( "[style_class]" = "20" ) END'
+    assert output(s) == exp
+
+
+def test_runtime_expression():
+    s = """
+    CLASS
+      EXPRESSION ( [EPPL_Q100_] = %eppl% )
+    END
+    """
+    exp = "CLASS EXPRESSION ( [EPPL_Q100_] = %eppl% ) END"
+    # print(output(s))
+    assert output(s) == exp
+
+
+def test_ne_comparison():
+    """
+    IS NOT is not valid
+    NE (Not Equals) should be used instead
+    """
+    s = """
+    CLASS
+        # EXPRESSION ( "[building]" IS NOT NULL) # incorrect syntax
+        EXPRESSION ( "[building]" NE NULL)
+    END
+    """
+    exp = 'CLASS EXPRESSION ( "[building]" NE NULL ) END'
+    assert output(s) == exp
+
+
+def test_eq_comparison():
+    """
+    Case is not changed for comparison (EQ/eq stay the same)
+    Uses Earley
+    """
+    s = """
+    CLASS
+        EXPRESSION ( "[building]" eq NULL)
+    END
+    """
+    exp = 'CLASS EXPRESSION ( "[building]" eq NULL ) END'
+    # print(output(s))
+    assert output(s) == exp
+
+
+def test_expression():
+    """
+    Addressed in issue #27, now parses successfully.
+    """
+    s = """
+    CLASS
+        EXPRESSION ('[construct]' ~* /Br.*$/)
+        STYLE
+            ANGLE 360
+        END
+    END
+    """
+    exp = "CLASS EXPRESSION ( '[construct]' ~* /Br.*$/ ) STYLE ANGLE 360 END END"
+    assert output(s) == exp
+
+
+def test_list_expression():
+    """
+    See issue #27
+    """
+    s = """
+    CLASS
+        EXPRESSION /NS_Bahn|NS_BahnAuto/
+    END
+    """
+    exp = "CLASS EXPRESSION /NS_Bahn|NS_BahnAuto/ END"
+    assert output(s) == exp
+
+
+def test_numerical_operator_ge_expression():
+    s = """
+    CLASS
+        EXPRESSION ([power] ge 10000)
+    END
+    """
+    exp = "CLASS EXPRESSION ( [power] ge 10000 ) END"
+    assert output(s) == exp
+
+
+def test_numerical_operator_gt_expression():
+    s = """
+    CLASS
+        EXPRESSION ([power] gt 10000)
+    END
+    """
+    exp = "CLASS EXPRESSION ( [power] gt 10000 ) END"
+    assert output(s) == exp
+
+
+def test_numerical_operator_le_expression():
+    s = """
+    CLASS
+        EXPRESSION ([power] le 100)
+    END
+    """
+    exp = "CLASS EXPRESSION ( [power] le 100 ) END"
+    assert output(s) == exp
+
+
+def test_numerical_operator_lt_expression():
+    s = """
+    CLASS
+        EXPRESSION ([power] lt 100)
+    END
+    """
+    exp = "CLASS EXPRESSION ( [power] lt 100 ) END"
+    assert output(s) == exp
+
+
+def test_divide():
+    """
+    Not sure if these should be in brackets or not
+    http://mapserver.org/mapfile/expressions.html
+    Implies with brackets will return a boolean value
+    and without will return a numeric value
+    """
+    s = """
+    CLASS
+        EXPRESSION ([field1] / [field2])
+    END
+    """
+    exp = "CLASS EXPRESSION ([field1] / [field2]) END"
+    assert output(s) == exp
+
+
+def test_multiply():
+    s = """
+    CLASS
+        EXPRESSION ([field1] * [field2])
+    END
+    """
+    exp = "CLASS EXPRESSION ([field1] * [field2]) END"
+    assert output(s) == exp
+
+
+def test_negation():
+    """
+    TODO - check the exact syntax for this
+    """
+    s = """
+    CLASS
+        EXPRESSION (-[field1])
+    END
+    """
+    exp = "CLASS EXPRESSION (-[field1]) END"
+    assert output(s) == exp
+
+
+def test_pointless_plus():
+    # Based on test_negation
+    s = """
+    CLASS
+        EXPRESSION (+[field1])
+    END
+    """
+    exp = "CLASS EXPRESSION ([field1]) END"
+    assert output(s) == exp
+
+
+def test_power():
+    s = """
+    CLASS
+        EXPRESSION ([field1] ^ [field2])
+    END
+    """
+    exp = "CLASS EXPRESSION ([field1] ^ [field2]) END"
+    assert output(s) == exp
+
+
+def test_divide_expression():
+    """
+    http://mapserver.org/mapfile/expressions.html
+    Also - * and ^
+    """
+    s = """
+    CLASS
+        EXPRESSION ([field1] / [field2] > 0.1)
+    END
+    """
+    exp = "CLASS EXPRESSION ( [field1] / [field2] > 0.1 ) END"
+    assert output(s) == exp
+
+
+def test_modulo_expression():
+    """
+    Not currently documented at http://mapserver.org/mapfile/expressions.html
+    """
+    s = """
+    CLASS
+        EXPRESSION  ( ([height] % 50) = 0 )
+    END
+    """
+    exp = "CLASS EXPRESSION ( ( [height] % 50 ) = 0 ) END"
+    assert output(s) == exp
+
+
+def test_escaped_string():
+    """
+    http://mapserver.org/mapfile/expressions.html#quotes-escaping-in-strings
+    Starting with MapServer 6.0 you don't need to escape single quotes within double quoted strings
+    and you don't need to escape double quotes within single quoted strings
+    """
+
+    s = r"""
+    CLASS
+        EXPRESSION "National \"hero\" statue"
+    END
+    """
+    exp = """CLASS EXPRESSION 'National \\"hero\\" statue' END"""
+    assert output(s) == exp
+
+
+def test_list_expression_alt():
+    """
+    See issue #38
+    http://mapserver.org/mapfile/expressions.html#list-expressions
+    These expressions are much more performant in MapServer
+    List expressions do not support quote escaping, or attribute values that contain a comma in them.
+
+    To activate them enclose a comma separated list of values between {}, without adding quotes
+    or extra spaces.
+    """
+    s = """
+    CLASS
+        EXPRESSION {2_Klass,Rte2etr}
+    END
+    """
+    exp = "CLASS EXPRESSION {2_Klass,Rte2etr} END"
+    assert output(s) == exp
+
+    s = """
+    CLASS
+        EXPRESSION {2_Klass,class with space}
+    END
+    """
+    exp = "CLASS EXPRESSION {2_Klass,class with space} END"
+    assert output(s) == exp
+
+
+def test_class_expression_oddname():
+    s = """
+    CLASS
+      TEXT ([area:ian])
+    END
+    """
+    exp = "CLASS TEXT ([area:ian]) END"
+    assert output(s) == exp
+
+
+def test_class_not_expression_brackets():
+    """
+    See issue #85 - coding of NOT logical expressions #85
+    Each expression should be bracketed independently and any NOT
+    clause should be outside the brackets
+    """
+    s = """
+    CLASS
+      EXPRESSION (("[TIME]" eq 'NOW') AND NOT ("[TYPE]" ~ "(something|completely|different)"))
+    END
+    """
+    exp = """CLASS EXPRESSION ( ( "[TIME]" eq 'NOW' ) AND NOT ( "[TYPE]" ~ "(something|completely|different)" ) ) END"""
+    print(output(s))
+    assert output(s) == exp
+
+
+def test_class_not_expression_no_brackets():
+    """
+    See issue #85 - coding of NOT logical expressions #85
+    This parses successfully in MapServer but not in mappyfile
+    """
+    s = """
+    CLASS
+      EXPRESSION ("[TIME]" eq 'NOW' AND NOT "[TYPE]" ~ "(something|completely|different)")
+    END
+    """
+    exp = """CLASS EXPRESSION ( ( "[TIME]" eq 'NOW' ) AND NOT ( "[TYPE]" ~ "(something|completely|different)" ) ) END"""
+    assert output(s) == exp
+
+
+def test_unquoted_unicode_string():
+    """
+    See pull request #92 - French unquoted string
+    """
+    s = """
+    CLASS
+      EXPRESSION {Aérodrome,Aéroport,Héliport,Base spatiale}
+    END
+    """
+
+    exp = """CLASS EXPRESSION {Aérodrome,Aéroport,Héliport,Base spatiale} END"""
+    assert output(s) == exp
+
+
+def test_list_with_apostrophe():
+    """
+    See https://github.com/geographika/mappyfile/issues/120
+    """
+    s = """
+    CLASS
+      EXPRESSION {bla,d'apostrophe}
+    END
+    """
+
+    exp = """CLASS EXPRESSION {bla,d'apostrophe} END"""
+    assert output(s) == exp
+
+
+def run_tests():
+    r"""
+    Need to comment out the following line in C:\VirtualEnvs\mappyfile\Lib\site-packages\pep8.py
+    #stdin_get_value = sys.stdin.read
+    Or get AttributeError: '_ReplInput' object has no attribute 'read'
+    """
+    pytest.main(["tests/test_expressions.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    test_list_with_apostrophe()
+    # run_tests()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_ordereddict.py` & `mappyfile-1.0.2/tests/test_ordereddict.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-import logging
-import json
-from copy import deepcopy
-import inspect
-import tempfile
-import pickle
-import pytest
-import mappyfile
-from mappyfile.parser import Parser
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-from mappyfile.ordereddict import DefaultOrderedDict, CaseInsensitiveOrderedDict
-
-
-def get_dict(s):
-    """
-    Parse, transform, and pretty print
-    the result
-    """
-    p = Parser()
-    m = MapfileToDict()
-    logging.info(inspect.stack()[1][3])
-
-    ast = p.parse(s)
-    logging.debug(ast.pretty())
-    d = m.transform(ast)
-    logging.debug(json.dumps(d, indent=4))
-
-    return d
-
-
-def output(d):
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    s = pp.pprint(d)
-    logging.debug(s)
-
-
-def test_dict():
-    d = DefaultOrderedDict()
-    d["key"] = ["value"]
-
-    print(d["key"])
-
-
-def test_config_directive():
-    s = """
-    MAP
-        NAME 'ConfigMap'
-        CONFIG MS_ERRORFILE 'stderr'
-        CONFIG 'PROJ_DEBUG' 'OFF'
-        CONFIG 'ON_MISSING_DATA' 'IGNORE'
-    END
-    """
-
-    d = get_dict(s)
-
-    d["name"] = "NewName"
-
-    print(d["name"])
-    assert d["name"] == "NewName"  # "'ConfigMap'")
-
-    print(
-        d["CONFIG"]
-    )  # even though this key is now lower-case it will correctly return (as DefaultOrderedDict calls key.lower())
-    assert d["config"]["PROJ_DEBUg"] == "OFF"
-    output(d)
-
-
-def test_debug():
-    s = """
-    MAP
-        DEBUG ON
-        DEFRESOLUTION 12
-    END
-    """
-
-    d = get_dict(s)
-
-    d["name"] = "NewName"
-    output(d)
-
-
-def test_false_value():
-    d = DefaultOrderedDict(DefaultOrderedDict)
-    d["key"] = False
-    print(json.dumps(d, indent=4))
-    assert d["key"] is False
-
-
-def test_case_sensitive_ordered_dict():
-    d = CaseInsensitiveOrderedDict()
-    d["KeY1"] = 1
-    d["KEY2"] = 2
-    d["key3"] = 3
-
-    print(json.dumps(d, indent=4))
-    assert d["kEy2"] == 2
-
-
-def test_update_case_sensitive_ordered_dict():
-    d = CaseInsensitiveOrderedDict(CaseInsensitiveOrderedDict)
-
-    d["b"] = "hello"
-    d["a"] = "goodbye"
-
-    print(json.dumps(d, indent=4))
-
-    d["config"]["ms_errorfile"] = "error.log"
-    print(json.dumps(d, indent=4))
-
-    d.update({"c": "hello"})
-
-    print(json.dumps(d, indent=4))
-
-    d.update(red=1, blue=2)
-
-    print(json.dumps(d, indent=4))
-    assert d["a"] == "goodbye"
-
-
-def test_pickling():
-    """
-    See issue #68
-    """
-
-    s = """
-    MAP
-        NAME "Test"
-        LAYER
-            NAME "Layer1"
-            CLASS
-                NAME "Class1"
-            END
-        END
-    END
-    """
-
-    d = get_dict(s)
-    tf1 = tempfile.NamedTemporaryFile(delete=False)
-    pickle.dump(d, tf1)
-    tf1.close()
-
-    with open(tf1.name, "rb") as tf2:
-        d2 = pickle.load(tf2)
-
-    assert d2["layers"][0]["classes"][0]["name"] == "Class1"
-
-
-def test_copy():
-    d = CaseInsensitiveOrderedDict()
-    d["key1"] = "val1"
-    c = d.copy()
-    c["key1"] = "val2"
-    assert d["key1"] == "val1"
-
-
-def test_has_key():
-    d = CaseInsensitiveOrderedDict()
-    d["key1"] = "val1"
-    assert "key1" in d
-    assert "key2" not in d
-
-
-def test_pop():
-    d = CaseInsensitiveOrderedDict()
-    d["key1"] = "val1"
-    v = d.pop("key1")
-    assert v == "val1"
-    assert len(d.keys()) == 0
-
-
-def test_deepcopy():
-    """
-    See issue #73
-    """
-    d = DefaultOrderedDict()
-    d["__type__"] = "layer"
-
-    c = deepcopy(d)
-    assert c["__type__"] == "layer"
-
-
-def test_adding_layers():
-    """
-    Test adding layers to an existing collection
-    """
-    m = mappyfile.loads("MAP LAYER TYPE POLYGON NAME 'TEST' END END")
-    lyr = mappyfile.loads("LAYER TYPE POLYGON NAME 'TEST' END")
-
-    assert len(m["layers"]) == 1
-    m["layers"].insert(0, lyr)
-    assert len(m["layers"]) == 2
-
-
-def test_adding_layers_to_empty():
-    """
-    Test adding layers when the layers object has not yet been created
-    """
-    m = mappyfile.loads("MAP END")
-    lyr = mappyfile.loads("LAYER TYPE POLYGON NAME 'TEST' END")
-
-    assert len(m["layers"]) == 0
-    m["layers"].insert(0, lyr)
-    assert len(m["layers"]) == 1
-    print(mappyfile.dumps(m))
-
-
-def run_tests():
-    # pytest.main(["tests/test_ordereddict.py::test_dict"])
-    pytest.main(["tests/test_ordereddict.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    # run_tests()
-    # test_update_case_sensitive_ordered_dict()
-    test_adding_layers_to_empty()
-    print("Done!")
+import logging
+import json
+from copy import deepcopy
+import inspect
+import tempfile
+import pickle
+import pytest
+import mappyfile
+from mappyfile.parser import Parser
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.transformer import MapfileToDict
+from mappyfile.ordereddict import DefaultOrderedDict, CaseInsensitiveOrderedDict
+
+
+def get_dict(s):
+    """
+    Parse, transform, and pretty print
+    the result
+    """
+    p = Parser()
+    m = MapfileToDict()
+    logging.info(inspect.stack()[1][3])
+
+    ast = p.parse(s)
+    logging.debug(ast.pretty())
+    d = m.transform(ast)
+    logging.debug(json.dumps(d, indent=4))
+
+    return d
+
+
+def output(d):
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    s = pp.pprint(d)
+    logging.debug(s)
+
+
+def test_dict():
+    d = DefaultOrderedDict()
+    d["key"] = ["value"]
+
+    print(d["key"])
+
+
+def test_config_directive():
+    s = """
+    MAP
+        NAME 'ConfigMap'
+        CONFIG MS_ERRORFILE 'stderr'
+        CONFIG 'PROJ_DEBUG' 'OFF'
+        CONFIG 'ON_MISSING_DATA' 'IGNORE'
+    END
+    """
+
+    d = get_dict(s)
+
+    d["name"] = "NewName"
+
+    print(d["name"])
+    assert d["name"] == "NewName"  # "'ConfigMap'")
+
+    print(
+        d["CONFIG"]
+    )  # even though this key is now lower-case it will correctly return (as DefaultOrderedDict calls key.lower())
+    assert d["config"]["PROJ_DEBUg"] == "OFF"
+    output(d)
+
+
+def test_debug():
+    s = """
+    MAP
+        DEBUG ON
+        DEFRESOLUTION 12
+    END
+    """
+
+    d = get_dict(s)
+
+    d["name"] = "NewName"
+    output(d)
+
+
+def test_false_value():
+    d = DefaultOrderedDict(DefaultOrderedDict)
+    d["key"] = False
+    print(json.dumps(d, indent=4))
+    assert d["key"] is False
+
+
+def test_case_sensitive_ordered_dict():
+    d = CaseInsensitiveOrderedDict()
+    d["KeY1"] = 1
+    d["KEY2"] = 2
+    d["key3"] = 3
+
+    print(json.dumps(d, indent=4))
+    assert d["kEy2"] == 2
+
+
+def test_update_case_sensitive_ordered_dict():
+    d = CaseInsensitiveOrderedDict(CaseInsensitiveOrderedDict)
+
+    d["b"] = "hello"
+    d["a"] = "goodbye"
+
+    print(json.dumps(d, indent=4))
+
+    d["config"]["ms_errorfile"] = "error.log"
+    print(json.dumps(d, indent=4))
+
+    d.update({"c": "hello"})
+
+    print(json.dumps(d, indent=4))
+
+    d.update(red=1, blue=2)
+
+    print(json.dumps(d, indent=4))
+    assert d["a"] == "goodbye"
+
+
+def test_pickling():
+    """
+    See issue #68
+    """
+
+    s = """
+    MAP
+        NAME "Test"
+        LAYER
+            NAME "Layer1"
+            CLASS
+                NAME "Class1"
+            END
+        END
+    END
+    """
+
+    d = get_dict(s)
+    tf1 = tempfile.NamedTemporaryFile(delete=False)
+    pickle.dump(d, tf1)
+    tf1.close()
+
+    with open(tf1.name, "rb") as tf2:
+        d2 = pickle.load(tf2)
+
+    assert d2["layers"][0]["classes"][0]["name"] == "Class1"
+
+
+def test_copy():
+    d = CaseInsensitiveOrderedDict()
+    d["key1"] = "val1"
+    c = d.copy()
+    c["key1"] = "val2"
+    assert d["key1"] == "val1"
+
+
+def test_has_key():
+    d = CaseInsensitiveOrderedDict()
+    d["key1"] = "val1"
+    assert "key1" in d
+    assert "key2" not in d
+
+
+def test_pop():
+    d = CaseInsensitiveOrderedDict()
+    d["key1"] = "val1"
+    v = d.pop("key1")
+    assert v == "val1"
+    assert len(d.keys()) == 0
+
+
+def test_deepcopy():
+    """
+    See issue #73
+    """
+    d = DefaultOrderedDict()
+    d["__type__"] = "layer"
+
+    c = deepcopy(d)
+    assert c["__type__"] == "layer"
+
+
+def test_adding_layers():
+    """
+    Test adding layers to an existing collection
+    """
+    m = mappyfile.loads("MAP LAYER TYPE POLYGON NAME 'TEST' END END")
+    lyr = mappyfile.loads("LAYER TYPE POLYGON NAME 'TEST' END")
+
+    assert len(m["layers"]) == 1
+    m["layers"].insert(0, lyr)
+    assert len(m["layers"]) == 2
+
+
+def test_adding_layers_to_empty():
+    """
+    Test adding layers when the layers object has not yet been created
+    """
+    m = mappyfile.loads("MAP END")
+    lyr = mappyfile.loads("LAYER TYPE POLYGON NAME 'TEST' END")
+
+    assert len(m["layers"]) == 0
+    m["layers"].insert(0, lyr)
+    assert len(m["layers"]) == 1
+    print(mappyfile.dumps(m))
+
+
+def run_tests():
+    # pytest.main(["tests/test_ordereddict.py::test_dict"])
+    pytest.main(["tests/test_ordereddict.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    # run_tests()
+    # test_update_case_sensitive_ordered_dict()
+    test_adding_layers_to_empty()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_pprint.py` & `mappyfile-1.0.2/tests/test_pprint.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,448 +1,448 @@
-# -*- coding: utf-8 -*-
-"""
-To check
-
-+ styleitem auto - should be capitalised (layer)
-+ Each of the units is different - [pixels|feet|inches|kilometers|meters|miles|nauticalmiles|dd] - standardise
-"""
-import logging
-import json
-import collections
-import pytest
-from mappyfile.parser import Parser
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-from mappyfile.ordereddict import DefaultOrderedDict
-import mappyfile
-
-
-def test_nested_quotes():
-    r"""
-    If values contain quotes then make sure they are escaped
-    shp2img -m C:\Temp\msautotest\misc\ogr_vrtconnect.tmp.map
-    """
-    s = """
-    LAYER
-        NAME shppoly
-        TYPE polygon
-        CONNECTIONTYPE OGR
-        CONNECTION '<OGRVRTDataSource><OGRVRTLayer name="poly"><SrcDataSource relativeToVRT="0">data/shppoly</SrcDataSource><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>'
-    END"""  # noqa: E501
-
-    ast = mappyfile.loads(s)
-    pp = PrettyPrinter(indent=0, quote='"', newlinechar=" ")  # expected
-    res = pp.pprint(ast)
-    print(res)
-    exp = (
-        'LAYER NAME "shppoly" TYPE POLYGON CONNECTIONTYPE OGR CONNECTION "<OGRVRTDataSource><OGRVRTLayer name="poly">'
-        '<SrcDataSource relativeToVRT="0">data/shppoly</SrcDataSource><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>" END'
-    )
-    assert res == exp
-
-
-def test_already_escaped():
-    """
-    Don't escape an already escaped quote
-    """
-    s = r'CLASS EXPRESSION "\"Tignish" END'
-    ast = mappyfile.loads(s)
-    pp = PrettyPrinter(indent=0, quote='"', newlinechar=" ")
-    res = pp.pprint(ast)
-    exp = r'CLASS EXPRESSION "\"Tignish" END'
-    assert res == exp
-
-    s = r"CLASS EXPRESSION '\'Tignish' END"
-    ast = mappyfile.loads(s)
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    res = pp.pprint(ast)
-    exp = r"CLASS EXPRESSION '\'Tignish' END"
-    assert res == exp
-
-
-def test_unicode():
-    s = """
-    MAP
-        METADATA
-          "ows_title" "éúáí"
-        END
-    END
-    """
-    ast = mappyfile.loads(s)
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    res = pp.pprint(ast)
-    exp = "MAP METADATA 'ows_title' 'éúáí' END END"
-    assert res == exp
-
-
-def test_enumeration():
-    s = """
-    MAP
-        EXTENT 0 0 100 100
-        DEBUG on
-        NAME Test
-        shapepath "test/path"
-        LAYER
-            CLASSITEM "Test"
-            CLASS
-                EXPRESSION "Field"
-                STYLE
-                    SIZE [sizefield]
-                END
-            END
-        END
-    END
-    """
-    p = Parser()
-    m = MapfileToDict()
-    ast = p.parse(s)
-    d = m.transform(ast)
-    print(d)
-    logging.debug(json.dumps(d, indent=4))
-    pp = PrettyPrinter(indent=4, quote="'", newlinechar="\n")
-    res = pp.pprint(d)
-    print(res)
-
-
-def test_points():
-    d = {
-        "points": [
-            [[1, 1], [50, 50], [1, 50], [1, 1]],
-            [[100, 100], [50, 50], [100, 50], [100, 100]],
-        ],
-        "__type__": "feature",
-    }
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert (
-        s
-        == "FEATURE POINTS 1 1 50 50 1 50 1 1 END POINTS 100 100 50 50 100 50 100 100 END END"
-    )
-
-
-def test_style_pattern():
-    d = {"pattern": [[10, 1], [50, 50], [1, 50], [1, 1]], "__type__": "style"}
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    assert s == "STYLE PATTERN 10 1 50 50 1 50 1 1 END END"
-
-
-def test_scaletoken():
-    sd = {"0": "ON", "255000000": "OFF"}
-
-    sd = collections.OrderedDict(sorted(sd.items()))
-
-    d = {"name": "%border%", "values": sd, "__type__": "scaletoken"}
-
-    d = collections.OrderedDict(sorted(d.items()))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "SCALETOKEN NAME '%border%' VALUES '0' 'ON' '255000000' 'OFF' END END"
-
-
-def test_metadata():
-    md = {"MS_ENABLE_MODES": "!*", "WMS_ENABLE_REQUEST": "*"}
-
-    md = collections.OrderedDict(sorted(md.items()))
-
-    d = {"metadata": md, "__type__": "map"}
-
-    d = collections.OrderedDict(sorted(d.items()))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "MAP METADATA 'MS_ENABLE_MODES' '!*' 'WMS_ENABLE_REQUEST' '*' END END"
-
-
-def test_connectionoptions():
-    values = {"FLATTEN_NESTED_ATTRIBUTES": "YES"}
-
-    d = {"connectionoptions": values, "__type__": "layer"}
-
-    d = collections.OrderedDict(sorted(d.items()))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "LAYER CONNECTIONOPTIONS 'FLATTEN_NESTED_ATTRIBUTES' 'YES' END END"
-
-
-def test_config():
-    cd = {"ms_nonsquare": "YES", "on_missing_data": "FAIL"}
-
-    cd = collections.OrderedDict(sorted(cd.items()))
-
-    d = {"config": cd, "__type__": "map"}
-
-    d = collections.OrderedDict(sorted(d.items()))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "MAP CONFIG 'MS_NONSQUARE' 'YES' CONFIG 'ON_MISSING_DATA' 'FAIL' END"
-
-
-def test_processing():
-    d = {
-        "name": "ProcessingLayer",
-        "processing": ["BANDS=1", "CONTOUR_ITEM=elevation", "CONTOUR_INTERVAL=20"],
-        "__type__": "layer",
-    }
-
-    d = collections.OrderedDict(sorted(d.items()))
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert (
-        s
-        == "LAYER NAME 'ProcessingLayer' PROCESSING 'BANDS=1' PROCESSING 'CONTOUR_ITEM=elevation' PROCESSING 'CONTOUR_INTERVAL=20' END"
-    )
-
-
-def test_multiple_layers():
-    d = {
-        "layers": [
-            {"name": "Layer1", "__type__": "layer"},
-            {"name": "Layer2", "__type__": "layer"},
-        ],
-        "__type__": "map",
-    }
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "MAP LAYER NAME 'Layer1' END LAYER NAME 'Layer2' END END"
-
-
-def test_projection():
-    d = {
-        "projection": [
-            "proj=utm",
-            "ellps=GRS80",
-            "datum=NAD83",
-            "zone=15",
-            "units=m",
-            "north",
-            "no_defs",
-        ],
-        "__type__": "map",
-    }
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert (
-        s
-        == "MAP PROJECTION 'proj=utm' 'ellps=GRS80' 'datum=NAD83' 'zone=15' 'units=m' 'north' 'no_defs' END END"
-    )
-
-
-def test_auto_projection():
-    d = {"projection": ["auto"], "__type__": "map"}
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "MAP PROJECTION AUTO END END"
-
-
-def test_single_string_projection():
-    d = {"projection": "init=epsg:4326", "__type__": "map"}
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "MAP PROJECTION 'init=epsg:4326' END END"
-
-
-def test_print_boolean():
-    d = {"transform": True, "__type__": "layer"}
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(d)
-    print(s)
-    assert s == "LAYER TRANSFORM TRUE END"
-
-
-def test_join():
-    d = {
-        "__type__": "layer",
-        "name": "Joined",
-        "joins": [{"__type__": "join", "name": "table_join"}],
-    }
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    d = collections.OrderedDict(sorted(d.items()))
-    s = pp.pprint(d)
-    assert s == "LAYER JOIN NAME 'table_join' END NAME 'Joined' END"
-
-
-def test_class_list():
-    d1 = {"text": "([area])", "expression": "([area])", "__type__": "class"}
-    d2 = {"text": '("[area]")', "expression": '("[area]")', "__type__": "class"}
-
-    od1 = collections.OrderedDict(sorted(d1.items()))
-    od2 = collections.OrderedDict(sorted(d2.items()))
-
-    classes = [od1, od2]
-
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
-    s = pp.pprint(classes)  # type: ignore
-    print(s)
-    assert (
-        s
-        == 'CLASS EXPRESSION ([area]) TEXT ([area]) END CLASS EXPRESSION ("[area]") TEXT ("[area]") END'
-    )
-
-
-def test_get_attribute_properties():
-    pp = PrettyPrinter()
-    props = pp.get_attribute_properties("layer", "connectiontype")
-    print(props)
-    assert len(props["enum"]) == 15
-
-
-def test_get_ref_attribute_properties():
-    pp = PrettyPrinter()
-    props = pp.get_attribute_properties("layer", "labelcache")
-    print(props)
-    assert len(props["enum"]) == 2
-
-
-def test_get_label_shadowcolor_properties():
-    # check a single ref is resolved
-    pp = PrettyPrinter()
-    props = pp.get_attribute_properties("label", "shadowcolor")
-    print(props)
-    assert len(props["oneOf"]) == 2
-
-
-def test_get_label_position_properties():
-    pp = PrettyPrinter()
-    props = pp.get_attribute_properties("label", "position")
-    assert props["oneOf"][1]["enum"] == [
-        "ul",
-        "uc",
-        "ur",
-        "cl",
-        "cc",
-        "cr",
-        "ll",
-        "lc",
-        "lr",
-    ]
-
-
-def test_map_layers_props():
-    pp = PrettyPrinter()
-    props = pp.get_attribute_properties("map", "layers")
-    print(props)
-    # assert(props["type"] == "object")
-    assert props["type"] == "array"
-
-
-def test_end_comment():
-    s = "MAP LAYER TYPE POINT NAME 'Test' END END"
-    ast = mappyfile.loads(s)
-    pp = PrettyPrinter(indent=4, quote='"', newlinechar="\n", end_comment=True)
-    res = pp.pprint(ast)
-    print(res)
-    exp = """MAP
-    LAYER
-        TYPE POINT
-        NAME "Test"
-    END # LAYER
-END # MAP"""
-    assert res == exp
-
-
-def test_empty_composite():
-    s = "MAP LAYER TYPE POINT NAME 'Test' END END"
-    ast = mappyfile.loads(s)
-    lyr = ast["layers"][0]
-
-    # as we are using DefaultOrderedDict then checks like this example
-    # will create an empty dictionary object
-    if lyr["connectiontype"]:
-        pass
-
-    assert isinstance(lyr["connectiontype"], DefaultOrderedDict)
-
-    pp = PrettyPrinter(indent=4, quote='"', newlinechar="\n", end_comment=True)
-    error_thrown = False
-
-    try:
-        pp.pprint(ast)
-    except ValueError:
-        error_thrown = True
-
-    assert error_thrown
-
-
-def test_align_values():
-    mapfile = """
-    MAP
-        EXTENT 0 0 100 100
-        DEBUG on
-        NAME Test
-        shapepath "test/path"
-    END
-    """
-    ast = mappyfile.loads(mapfile)
-    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n", align_values=True)
-    s = pp.pprint(ast)
-
-    aligned_indexes = set()
-    for line in s.splitlines():
-        words = line.split()
-        if len(words) > 1:
-            aligned_indexes.add(line.index(words[1]))
-    assert len(aligned_indexes) == 1
-
-
-def test_separate_complex_types():
-    s = """
-    MAP
-        EXTENT 0 0 100 100
-        shapepath "test/path"
-        LAYER
-            CLASS
-                EXPRESSION "Field"
-                STYLE
-                    SIZE [sizefield]
-                END
-                GROUP 'group1'
-            END
-            CLASSITEM "Test"
-        END
-        DEBUG on
-        NAME Test
-    END
-    """
-    ast = mappyfile.loads(s)
-    pp = PrettyPrinter(
-        indent=4, quote="'", newlinechar="\n", separate_complex_types=True
-    )
-    s = pp.pprint(ast)
-    assert s.index("NAME ") < s.index("LAYER\n")
-    assert s.index("DEBUG ") < s.index("LAYER\n")
-    assert s.index("CLASSITEM ") < s.index("CLASS\n")
-    assert s.index("GROUP") < s.index("STYLE\n")
-
-
-def run_tests():
-    # pytest.main(["tests/test_pprint.py::test_format_list"])
-    pytest.main(["tests/test_pprint.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.INFO)
-    test_empty_composite()
-    # run_tests()
-    print("Done!")
+# -*- coding: utf-8 -*-
+"""
+To check
+
++ styleitem auto - should be capitalised (layer)
++ Each of the units is different - [pixels|feet|inches|kilometers|meters|miles|nauticalmiles|dd] - standardise
+"""
+import logging
+import json
+import collections
+import pytest
+from mappyfile.parser import Parser
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.transformer import MapfileToDict
+from mappyfile.ordereddict import DefaultOrderedDict
+import mappyfile
+
+
+def test_nested_quotes():
+    r"""
+    If values contain quotes then make sure they are escaped
+    shp2img -m C:\Temp\msautotest\misc\ogr_vrtconnect.tmp.map
+    """
+    s = """
+    LAYER
+        NAME shppoly
+        TYPE polygon
+        CONNECTIONTYPE OGR
+        CONNECTION '<OGRVRTDataSource><OGRVRTLayer name="poly"><SrcDataSource relativeToVRT="0">data/shppoly</SrcDataSource><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>'
+    END"""  # noqa: E501
+
+    ast = mappyfile.loads(s)
+    pp = PrettyPrinter(indent=0, quote='"', newlinechar=" ")  # expected
+    res = pp.pprint(ast)
+    print(res)
+    exp = (
+        'LAYER NAME "shppoly" TYPE POLYGON CONNECTIONTYPE OGR CONNECTION "<OGRVRTDataSource><OGRVRTLayer name="poly">'
+        '<SrcDataSource relativeToVRT="0">data/shppoly</SrcDataSource><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>" END'
+    )
+    assert res == exp
+
+
+def test_already_escaped():
+    """
+    Don't escape an already escaped quote
+    """
+    s = r'CLASS EXPRESSION "\"Tignish" END'
+    ast = mappyfile.loads(s)
+    pp = PrettyPrinter(indent=0, quote='"', newlinechar=" ")
+    res = pp.pprint(ast)
+    exp = r'CLASS EXPRESSION "\"Tignish" END'
+    assert res == exp
+
+    s = r"CLASS EXPRESSION '\'Tignish' END"
+    ast = mappyfile.loads(s)
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    res = pp.pprint(ast)
+    exp = r"CLASS EXPRESSION '\'Tignish' END"
+    assert res == exp
+
+
+def test_unicode():
+    s = """
+    MAP
+        METADATA
+          "ows_title" "éúáí"
+        END
+    END
+    """
+    ast = mappyfile.loads(s)
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    res = pp.pprint(ast)
+    exp = "MAP METADATA 'ows_title' 'éúáí' END END"
+    assert res == exp
+
+
+def test_enumeration():
+    s = """
+    MAP
+        EXTENT 0 0 100 100
+        DEBUG on
+        NAME Test
+        shapepath "test/path"
+        LAYER
+            CLASSITEM "Test"
+            CLASS
+                EXPRESSION "Field"
+                STYLE
+                    SIZE [sizefield]
+                END
+            END
+        END
+    END
+    """
+    p = Parser()
+    m = MapfileToDict()
+    ast = p.parse(s)
+    d = m.transform(ast)
+    print(d)
+    logging.debug(json.dumps(d, indent=4))
+    pp = PrettyPrinter(indent=4, quote="'", newlinechar="\n")
+    res = pp.pprint(d)
+    print(res)
+
+
+def test_points():
+    d = {
+        "points": [
+            [[1, 1], [50, 50], [1, 50], [1, 1]],
+            [[100, 100], [50, 50], [100, 50], [100, 100]],
+        ],
+        "__type__": "feature",
+    }
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert (
+        s
+        == "FEATURE POINTS 1 1 50 50 1 50 1 1 END POINTS 100 100 50 50 100 50 100 100 END END"
+    )
+
+
+def test_style_pattern():
+    d = {"pattern": [[10, 1], [50, 50], [1, 50], [1, 1]], "__type__": "style"}
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    assert s == "STYLE PATTERN 10 1 50 50 1 50 1 1 END END"
+
+
+def test_scaletoken():
+    sd = {"0": "ON", "255000000": "OFF"}
+
+    sd = collections.OrderedDict(sorted(sd.items()))
+
+    d = {"name": "%border%", "values": sd, "__type__": "scaletoken"}
+
+    d = collections.OrderedDict(sorted(d.items()))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "SCALETOKEN NAME '%border%' VALUES '0' 'ON' '255000000' 'OFF' END END"
+
+
+def test_metadata():
+    md = {"MS_ENABLE_MODES": "!*", "WMS_ENABLE_REQUEST": "*"}
+
+    md = collections.OrderedDict(sorted(md.items()))
+
+    d = {"metadata": md, "__type__": "map"}
+
+    d = collections.OrderedDict(sorted(d.items()))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "MAP METADATA 'MS_ENABLE_MODES' '!*' 'WMS_ENABLE_REQUEST' '*' END END"
+
+
+def test_connectionoptions():
+    values = {"FLATTEN_NESTED_ATTRIBUTES": "YES"}
+
+    d = {"connectionoptions": values, "__type__": "layer"}
+
+    d = collections.OrderedDict(sorted(d.items()))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "LAYER CONNECTIONOPTIONS 'FLATTEN_NESTED_ATTRIBUTES' 'YES' END END"
+
+
+def test_config():
+    cd = {"ms_nonsquare": "YES", "on_missing_data": "FAIL"}
+
+    cd = collections.OrderedDict(sorted(cd.items()))
+
+    d = {"config": cd, "__type__": "map"}
+
+    d = collections.OrderedDict(sorted(d.items()))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "MAP CONFIG 'MS_NONSQUARE' 'YES' CONFIG 'ON_MISSING_DATA' 'FAIL' END"
+
+
+def test_processing():
+    d = {
+        "name": "ProcessingLayer",
+        "processing": ["BANDS=1", "CONTOUR_ITEM=elevation", "CONTOUR_INTERVAL=20"],
+        "__type__": "layer",
+    }
+
+    d = collections.OrderedDict(sorted(d.items()))
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert (
+        s
+        == "LAYER NAME 'ProcessingLayer' PROCESSING 'BANDS=1' PROCESSING 'CONTOUR_ITEM=elevation' PROCESSING 'CONTOUR_INTERVAL=20' END"
+    )
+
+
+def test_multiple_layers():
+    d = {
+        "layers": [
+            {"name": "Layer1", "__type__": "layer"},
+            {"name": "Layer2", "__type__": "layer"},
+        ],
+        "__type__": "map",
+    }
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "MAP LAYER NAME 'Layer1' END LAYER NAME 'Layer2' END END"
+
+
+def test_projection():
+    d = {
+        "projection": [
+            "proj=utm",
+            "ellps=GRS80",
+            "datum=NAD83",
+            "zone=15",
+            "units=m",
+            "north",
+            "no_defs",
+        ],
+        "__type__": "map",
+    }
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert (
+        s
+        == "MAP PROJECTION 'proj=utm' 'ellps=GRS80' 'datum=NAD83' 'zone=15' 'units=m' 'north' 'no_defs' END END"
+    )
+
+
+def test_auto_projection():
+    d = {"projection": ["auto"], "__type__": "map"}
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "MAP PROJECTION AUTO END END"
+
+
+def test_single_string_projection():
+    d = {"projection": "init=epsg:4326", "__type__": "map"}
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "MAP PROJECTION 'init=epsg:4326' END END"
+
+
+def test_print_boolean():
+    d = {"transform": True, "__type__": "layer"}
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(d)
+    print(s)
+    assert s == "LAYER TRANSFORM TRUE END"
+
+
+def test_join():
+    d = {
+        "__type__": "layer",
+        "name": "Joined",
+        "joins": [{"__type__": "join", "name": "table_join"}],
+    }
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    d = collections.OrderedDict(sorted(d.items()))
+    s = pp.pprint(d)
+    assert s == "LAYER JOIN NAME 'table_join' END NAME 'Joined' END"
+
+
+def test_class_list():
+    d1 = {"text": "([area])", "expression": "([area])", "__type__": "class"}
+    d2 = {"text": '("[area]")', "expression": '("[area]")', "__type__": "class"}
+
+    od1 = collections.OrderedDict(sorted(d1.items()))
+    od2 = collections.OrderedDict(sorted(d2.items()))
+
+    classes = [od1, od2]
+
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar=" ")
+    s = pp.pprint(classes)  # type: ignore
+    print(s)
+    assert (
+        s
+        == 'CLASS EXPRESSION ([area]) TEXT ([area]) END CLASS EXPRESSION ("[area]") TEXT ("[area]") END'
+    )
+
+
+def test_get_attribute_properties():
+    pp = PrettyPrinter()
+    props = pp.get_attribute_properties("layer", "connectiontype")
+    print(props)
+    assert len(props["enum"]) == 15
+
+
+def test_get_ref_attribute_properties():
+    pp = PrettyPrinter()
+    props = pp.get_attribute_properties("layer", "labelcache")
+    print(props)
+    assert len(props["enum"]) == 2
+
+
+def test_get_label_shadowcolor_properties():
+    # check a single ref is resolved
+    pp = PrettyPrinter()
+    props = pp.get_attribute_properties("label", "shadowcolor")
+    print(props)
+    assert len(props["oneOf"]) == 2
+
+
+def test_get_label_position_properties():
+    pp = PrettyPrinter()
+    props = pp.get_attribute_properties("label", "position")
+    assert props["oneOf"][1]["enum"] == [
+        "ul",
+        "uc",
+        "ur",
+        "cl",
+        "cc",
+        "cr",
+        "ll",
+        "lc",
+        "lr",
+    ]
+
+
+def test_map_layers_props():
+    pp = PrettyPrinter()
+    props = pp.get_attribute_properties("map", "layers")
+    print(props)
+    # assert(props["type"] == "object")
+    assert props["type"] == "array"
+
+
+def test_end_comment():
+    s = "MAP LAYER TYPE POINT NAME 'Test' END END"
+    ast = mappyfile.loads(s)
+    pp = PrettyPrinter(indent=4, quote='"', newlinechar="\n", end_comment=True)
+    res = pp.pprint(ast)
+    print(res)
+    exp = """MAP
+    LAYER
+        TYPE POINT
+        NAME "Test"
+    END # LAYER
+END # MAP"""
+    assert res == exp
+
+
+def test_empty_composite():
+    s = "MAP LAYER TYPE POINT NAME 'Test' END END"
+    ast = mappyfile.loads(s)
+    lyr = ast["layers"][0]
+
+    # as we are using DefaultOrderedDict then checks like this example
+    # will create an empty dictionary object
+    if lyr["connectiontype"]:
+        pass
+
+    assert isinstance(lyr["connectiontype"], DefaultOrderedDict)
+
+    pp = PrettyPrinter(indent=4, quote='"', newlinechar="\n", end_comment=True)
+    error_thrown = False
+
+    try:
+        pp.pprint(ast)
+    except ValueError:
+        error_thrown = True
+
+    assert error_thrown
+
+
+def test_align_values():
+    mapfile = """
+    MAP
+        EXTENT 0 0 100 100
+        DEBUG on
+        NAME Test
+        shapepath "test/path"
+    END
+    """
+    ast = mappyfile.loads(mapfile)
+    pp = PrettyPrinter(indent=0, quote="'", newlinechar="\n", align_values=True)
+    s = pp.pprint(ast)
+
+    aligned_indexes = set()
+    for line in s.splitlines():
+        words = line.split()
+        if len(words) > 1:
+            aligned_indexes.add(line.index(words[1]))
+    assert len(aligned_indexes) == 1
+
+
+def test_separate_complex_types():
+    s = """
+    MAP
+        EXTENT 0 0 100 100
+        shapepath "test/path"
+        LAYER
+            CLASS
+                EXPRESSION "Field"
+                STYLE
+                    SIZE [sizefield]
+                END
+                GROUP 'group1'
+            END
+            CLASSITEM "Test"
+        END
+        DEBUG on
+        NAME Test
+    END
+    """
+    ast = mappyfile.loads(s)
+    pp = PrettyPrinter(
+        indent=4, quote="'", newlinechar="\n", separate_complex_types=True
+    )
+    s = pp.pprint(ast)
+    assert s.index("NAME ") < s.index("LAYER\n")
+    assert s.index("DEBUG ") < s.index("LAYER\n")
+    assert s.index("CLASSITEM ") < s.index("CLASS\n")
+    assert s.index("GROUP") < s.index("STYLE\n")
+
+
+def run_tests():
+    # pytest.main(["tests/test_pprint.py::test_format_list"])
+    pytest.main(["tests/test_pprint.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.INFO)
+    test_empty_composite()
+    # run_tests()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_sample_maps.py` & `mappyfile-1.0.2/tests/test_sample_maps.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import os
-import logging
-import pytest
-import mappyfile
-from mappyfile.parser import Parser
-from mappyfile.transformer import MapfileToDict
-from mappyfile.pprint import PrettyPrinter
-from lark import UnexpectedToken
-from mappyfile.validator import Validator
-
-
-def test_all_maps():
-    sample_dir = os.path.join(os.path.dirname(__file__), "sample_maps")
-
-    # the following "map" files are includes used by other mapfiles in msautotest
-    # TODO - rename all these to .include in MapServer source to allow them to be more
-    # easily processed
-    ignore_list = [
-        "bdry_counpy2_mssql.map",
-        "bdry_counpy2_ogr.map",
-        "bdry_counpy2_postgis.map",
-        "bdry_counpy2_shapefile.map",
-        "indx_q100kpy4_ogr.map",
-        "indx_q100kpy4_shapefile.map",
-        "mssql_connection.map",
-        "quoted_text.MAP",
-        "style-size.map",
-        "wfs_ogr_export_metadata.map",
-    ]
-
-    # list any maps that are known not to parse and are to be fixed
-    ignore_list += ["centerline.map"]
-
-    p = Parser(expand_includes=False)
-    m = MapfileToDict(include_position=True)
-    v = Validator()
-
-    failing_maps = []
-
-    for fn in os.listdir(sample_dir):
-        if fn not in ignore_list:
-            print(fn)
-            try:
-                ast = p.parse_file(os.path.join(sample_dir, fn))
-                d = m.transform(ast)
-                errors = v.validate(d)
-                try:
-                    assert len(errors) == 0
-                except AssertionError as ex:
-                    logging.warning("Validation errors in %s ", fn)
-                    logging.error(ex)
-                    logging.warning(errors)
-            except (BaseException, UnexpectedToken) as ex:
-                logging.warning("Cannot process %s ", fn)
-                logging.error(ex)
-                failing_maps.append(fn)
-
-    logging.warning("The list of maps below have failed to parse")
-    logging.warning(failing_maps)
-
-
-def test_includes():
-    p = Parser()
-
-    ast = p.parse_file("./tests/samples/include1.map")
-    m = MapfileToDict()
-
-    d = m.transform(ast)  # works
-    print(mappyfile.dumps(d))
-
-
-def test_includes_nested_path():
-    p = Parser()
-
-    ast = p.parse_file("./tests/samples/include1_nested_path.map")
-    m = MapfileToDict()
-
-    d = m.transform(ast)  # works
-    print(mappyfile.dumps(d))
-
-
-def test_includes_max_recursion():
-    p = Parser()
-
-    with pytest.raises(Exception) as excinfo:
-        p.parse_file("./tests/samples/include1_recursive.map")
-
-    assert "Maximum nested include exceeded" in str(excinfo.value)
-
-
-def test_includes_no_expand():
-    """
-    https://github.com/geographika/mappyfile/issues/39
-    """
-    s = """
-    MAP
-        INCLUDE "includes/mymapfile.map"
-    END
-    """
-
-    d = mappyfile.loads(s, expand_includes=False)
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    output = pp.pprint(d)
-
-    expected = "MAP INCLUDE 'includes/mymapfile.map' END"
-    assert output == expected
-
-
-def test_two_includes():
-    s = """
-    MAP
-        INCLUDE "include1.txt"
-        INCLUDE "include2.txt"
-    END
-    """
-
-    d = mappyfile.loads(s, expand_includes=False)
-    logging.debug(d)
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    output = pp.pprint(d)
-    print(output)
-    expected = "MAP INCLUDE 'include1.txt' INCLUDE 'include2.txt' END"
-    assert output == expected
-
-
-def test_non_ascii():
-    p = Parser()
-
-    ast = p.parse_file("./tests/samples/non_ascii.map")
-    m = MapfileToDict()
-
-    d = m.transform(ast)  # works
-    print(mappyfile.dumps(d))
-
-
-def test_unicode_map():
-    with open("./tests/samples/unicode.map", "r") as mf_file:
-        mf = mappyfile.load(mf_file)
-
-    print(mappyfile.dumps(mf))
-
-
-def run_tests():
-    pytest.main(["tests/test_sample_maps.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    logging.getLogger("mappyfile").setLevel(logging.INFO)
-    # run_tests()
-    # test_unicode_map()
-    test_all_maps()
-    print("Done!")
+import os
+import logging
+import pytest
+import mappyfile
+from mappyfile.parser import Parser
+from mappyfile.transformer import MapfileToDict
+from mappyfile.pprint import PrettyPrinter
+from lark import UnexpectedToken
+from mappyfile.validator import Validator
+
+
+def test_all_maps():
+    sample_dir = os.path.join(os.path.dirname(__file__), "sample_maps")
+
+    # the following "map" files are includes used by other mapfiles in msautotest
+    # TODO - rename all these to .include in MapServer source to allow them to be more
+    # easily processed
+    ignore_list = [
+        "bdry_counpy2_mssql.map",
+        "bdry_counpy2_ogr.map",
+        "bdry_counpy2_postgis.map",
+        "bdry_counpy2_shapefile.map",
+        "indx_q100kpy4_ogr.map",
+        "indx_q100kpy4_shapefile.map",
+        "mssql_connection.map",
+        "quoted_text.MAP",
+        "style-size.map",
+        "wfs_ogr_export_metadata.map",
+    ]
+
+    # list any maps that are known not to parse and are to be fixed
+    ignore_list += ["centerline.map"]
+
+    p = Parser(expand_includes=False)
+    m = MapfileToDict(include_position=True)
+    v = Validator()
+
+    failing_maps = []
+
+    for fn in os.listdir(sample_dir):
+        if fn not in ignore_list:
+            print(fn)
+            try:
+                ast = p.parse_file(os.path.join(sample_dir, fn))
+                d = m.transform(ast)
+                errors = v.validate(d)
+                try:
+                    assert len(errors) == 0
+                except AssertionError as ex:
+                    logging.warning("Validation errors in %s ", fn)
+                    logging.error(ex)
+                    logging.warning(errors)
+            except (BaseException, UnexpectedToken) as ex:
+                logging.warning("Cannot process %s ", fn)
+                logging.error(ex)
+                failing_maps.append(fn)
+
+    logging.warning("The list of maps below have failed to parse")
+    logging.warning(failing_maps)
+
+
+def test_includes():
+    p = Parser()
+
+    ast = p.parse_file("./tests/samples/include1.map")
+    m = MapfileToDict()
+
+    d = m.transform(ast)  # works
+    print(mappyfile.dumps(d))
+
+
+def test_includes_nested_path():
+    p = Parser()
+
+    ast = p.parse_file("./tests/samples/include1_nested_path.map")
+    m = MapfileToDict()
+
+    d = m.transform(ast)  # works
+    print(mappyfile.dumps(d))
+
+
+def test_includes_max_recursion():
+    p = Parser()
+
+    with pytest.raises(Exception) as excinfo:
+        p.parse_file("./tests/samples/include1_recursive.map")
+
+    assert "Maximum nested include exceeded" in str(excinfo.value)
+
+
+def test_includes_no_expand():
+    """
+    https://github.com/geographika/mappyfile/issues/39
+    """
+    s = """
+    MAP
+        INCLUDE "includes/mymapfile.map"
+    END
+    """
+
+    d = mappyfile.loads(s, expand_includes=False)
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    output = pp.pprint(d)
+
+    expected = "MAP INCLUDE 'includes/mymapfile.map' END"
+    assert output == expected
+
+
+def test_two_includes():
+    s = """
+    MAP
+        INCLUDE "include1.txt"
+        INCLUDE "include2.txt"
+    END
+    """
+
+    d = mappyfile.loads(s, expand_includes=False)
+    logging.debug(d)
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    output = pp.pprint(d)
+    print(output)
+    expected = "MAP INCLUDE 'include1.txt' INCLUDE 'include2.txt' END"
+    assert output == expected
+
+
+def test_non_ascii():
+    p = Parser()
+
+    ast = p.parse_file("./tests/samples/non_ascii.map")
+    m = MapfileToDict()
+
+    d = m.transform(ast)  # works
+    print(mappyfile.dumps(d))
+
+
+def test_unicode_map():
+    with open("./tests/samples/unicode.map", "r") as mf_file:
+        mf = mappyfile.load(mf_file)
+
+    print(mappyfile.dumps(mf))
+
+
+def run_tests():
+    pytest.main(["tests/test_sample_maps.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    logging.getLogger("mappyfile").setLevel(logging.INFO)
+    # run_tests()
+    # test_unicode_map()
+    test_all_maps()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_snippets.py` & `mappyfile-1.0.2/tests/test_snippets.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,1056 +1,1056 @@
-# -*- coding: utf-8 -*-
-
-import logging
-import inspect
-import pytest
-import mappyfile
-from mappyfile.parser import Parser
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-from mappyfile.validator import Validator
-
-
-def output(s, include_position=True, schema_name="map"):
-    """
-    Parse, transform, validate, and pretty print
-    the result
-    """
-    p = Parser()
-    m = MapfileToDict(include_position=include_position)
-
-    # https://stackoverflow.com/questions/900392/getting-the-caller-function-name-inside-another-function-in-python
-    logging.info(inspect.stack()[1][3])
-
-    ast = p.parse(s)
-    logging.debug(ast.pretty())
-    d = m.transform(ast)
-    logging.debug(d)
-    v = Validator()
-    errors = v.validate(d, schema_name=schema_name)
-    logging.error(errors)
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    s = pp.pprint(d)
-    logging.debug(s)
-    assert len(errors) == 0
-    return s
-
-
-def check_result(s, schema_name="map"):
-    s2 = output(s, schema_name=schema_name)
-    try:
-        assert s == s2
-    except AssertionError:
-        logging.info(s)
-        logging.info(s2)
-        raise
-
-
-def test_layer():
-    s = "LAYER NAME 'Test' TYPE POINT END"
-    check_result(s, schema_name="layer")
-
-
-def test_class():
-    s = "CLASS NAME 'Test' END"
-    check_result(s, schema_name="class")
-
-
-def test_map_size():
-    s = """
-    MAP
-    SIZE 256 256
-    END"""
-
-    exp = "MAP SIZE 256 256 END"
-    assert output(s) == exp
-
-
-def test_style_color():
-    s = """
-    STYLE
-    COLOR 0 0 255
-    END"""
-
-    exp = "STYLE COLOR 0 0 255 END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style():
-    s = """
-    STYLE
-    COLOR 0 0 255
-    WIDTH 5
-    LINECAP BUTT
-    END"""
-
-    exp = "STYLE COLOR 0 0 255 WIDTH 5 LINECAP BUTT END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_oneline():
-    s = "STYLE COLOR 0 0 255 WIDTH 5 LINECAP BUTT END"
-    check_result(s, schema_name="style")
-
-
-def test_style_pattern():
-    s = """
-    STYLE
-        PATTERN 5 5 END
-    END
-    """
-
-    exp = "STYLE PATTERN 5 5 END END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_pattern2():
-    s = """
-    STYLE
-        PATTERN
-            5 5
-        END
-    END
-    """
-
-    exp = "STYLE PATTERN 5 5 END END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_pattern3():
-    """
-    Test a STYLE on one line can be parsed
-    """
-    s = "STYLE PATTERN 5 5 END END"
-    exp = "STYLE PATTERN 5 5 END END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_pattern4():
-    """
-    Test pattern values on separate lines are valid
-    """
-    s = """
-    STYLE
-        PATTERN
-            5
-            5
-        END
-    END
-    """
-    exp = "STYLE PATTERN 5 5 END END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_pattern5():
-    """
-    Test pattern with decimal places
-    """
-    s = """
-    STYLE
-        PATTERN
-            5.0 5.0
-        END
-    END
-    """
-    exp = "STYLE PATTERN 5.0 5.0 END END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_offset_mixed():
-    """
-    Test an attribute and numerical pair for a STYLE OFFSET
-    See https://github.com/geographika/mappyfile/issues/114
-    """
-    s = """
-    STYLE
-        OFFSET [attribute] -999
-    END
-    """
-    exp = "STYLE OFFSET [attribute] -999 END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_offset_mixed2():
-    """
-    As above but reversed
-    """
-    s = """
-    STYLE
-        OFFSET -999 [attribute]
-    END
-    """
-    exp = "STYLE OFFSET -999 [attribute] END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_metadata():
-    """
-    Parse metadata directly
-    """
-    s = """
-    METADATA
-        'wms_title' 'Test simple wms'
-    END
-    """
-    exp = """METADATA 'wms_title' 'Test simple wms' END"""
-    assert output(s, schema_name="metadata") == exp
-
-
-def test_metadata_uppercase():
-    s = """
-    METADATA
-        'WMS_TITLE' 'Test simple wms'
-    END
-    """
-    exp = """METADATA 'wms_title' 'Test simple wms' END"""
-    assert output(s, schema_name="metadata") == exp
-
-
-def test_duplicated_metadata_keys():
-    """
-    The second key will be used
-    """
-
-    s = """
-    METADATA
-        'wms_title' 'Test simple wms'
-        'wms_title' 'Test simple wms2'
-    END
-    """
-    exp = """METADATA 'wms_title' 'Test simple wms2' END"""
-    assert output(s, schema_name="metadata") == exp
-
-
-def test_metadata_unquoted():
-    """
-    The METADATA block doesn't need quotes
-    (as long as values don't have spaces)
-    The printer will add quotes automatically
-    """
-    s = """
-    METADATA
-        wms_title my_title
-    END
-    """
-    exp = "METADATA 'wms_title' 'my_title' END"
-    assert output(s, schema_name="metadata") == exp
-
-
-def test_validation():
-    """
-    Parse validation block directly
-    """
-    s = """
-    VALIDATION
-        "field1" "^[0-9,]+$"
-        "field2" "-1"
-        qstring '.'
-    END
-    """
-    exp = """VALIDATION 'field1' '^[0-9,]+$' 'field2' '-1' 'qstring' '.' END"""
-    assert output(s, schema_name="validation") == exp
-
-
-def test_layer_text_query():
-    s = """
-    CLASS
-        TEXT (tostring([area],"%.2f"))
-    END
-    """
-    exp = """CLASS TEXT (tostring([area],"%.2f")) END"""
-    assert output(s, schema_name="class") == exp
-
-
-def test_label():
-    s = """
-    LABEL
-      COLOR  0 0 0
-      FONT Vera
-      TYPE truetype
-      SIZE 8
-      POSITION AUTO
-      PARTIALS FALSE
-      OUTLINECOLOR 255 255 255
-    END
-    """
-    exp = "LABEL COLOR 0 0 0 FONT 'Vera' TYPE TRUETYPE SIZE 8 POSITION AUTO PARTIALS FALSE OUTLINECOLOR 255 255 255 END"
-    assert output(s, schema_name="label") == exp
-
-
-def test_output_format():
-    s = """
-    MAP
-        IMAGETYPE grid
-        OUTPUTFORMAT
-            NAME grid2
-            DRIVER "GDAL/AAIGRID"
-            IMAGEMODE INT16
-            FORMATOPTION 'NULLVALUE=-99'
-        END
-    END
-    """
-    exp = "MAP IMAGETYPE 'grid' OUTPUTFORMAT NAME 'grid2' DRIVER 'GDAL/AAIGRID' IMAGEMODE INT16 FORMATOPTION 'NULLVALUE=-99' END END"
-    assert output(s) == exp
-
-
-def test_class_symbol():
-    s = """
-    CLASS
-        STYLE # a shadow
-            COLOR 151 151 151
-            SYMBOL [symbol]
-            OFFSET 2 2
-            SIZE [size]
-        END
-    END
-    """
-    exp = "CLASS STYLE COLOR 151 151 151 SYMBOL [symbol] OFFSET 2 2 SIZE [size] END END"
-    assert output(s, schema_name="class") == exp
-
-
-def test_filter():
-    s = """
-    LAYER
-        TYPE POINT
-        NAME 'filters_test002'
-        FILTER 'aitkin'i
-    END
-    """
-
-    exp = "LAYER TYPE POINT NAME 'filters_test002' FILTER 'aitkin'i END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_like_filter():
-    s = """
-    LAYER
-        TYPE POINT
-        NAME 'filters_test003'
-        FILTER ("blpu_classification_code" LIKE 'RI%')
-    END
-    """
-
-    exp = r"""LAYER TYPE POINT NAME 'filters_test003' FILTER ( "blpu_classification_code" LIKE 'RI%' ) END"""
-    assert output(s, schema_name="layer") == exp
-
-
-def test_regex():
-    s = r"""
-    LAYER
-        TYPE POINT
-        NAME 'regexp-example'
-        FILTERITEM 'placename'
-        FILTER /hotel/
-    END
-    """
-    exp = r"LAYER TYPE POINT NAME 'regexp-example' FILTERITEM 'placename' FILTER /hotel/ END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_feature():
-    """
-    With multiple points
-    """
-
-    s = """
-    FEATURE
-        POINTS
-            0 10
-        END
-    END
-    """
-
-    exp = "FEATURE POINTS 0 10 END END"
-    assert output(s, schema_name="feature") == exp
-
-
-def test_multi_feature():
-    """
-    With multiple points
-    """
-
-    s = """
-        LAYER
-            TYPE LINE
-            FEATURE
-                POINTS
-                    0 10
-                END
-                POINTS
-                    -20 20
-                    20 20
-                    -20 -20
-                    0 -30
-                    20 -20
-                    -20 20
-                    -20 20
-                    30 30
-                END
-            END
-        END
-    """
-
-    exp = "LAYER TYPE LINE FEATURE POINTS 0 10 END POINTS -20 20 20 20 -20 -20 0 -30 20 -20 -20 20 -20 20 30 30 END END END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_triple_feature():
-    """
-    With multiple points
-    """
-
-    s = """
-    FEATURE
-        POINTS
-            0 10
-            5 2
-        END
-        POINTS
-            0 10
-            3 3
-        END
-        POINTS
-            0 10
-            7 7
-        END
-    END
-    """
-
-    exp = "FEATURE POINTS 0 10 5 2 END POINTS 0 10 3 3 END POINTS 0 10 7 7 END END"
-    assert output(s, schema_name="feature") == exp
-
-
-def test_symbol():
-    s = """
-    SYMBOL
-        NAME 'triangle'
-        TYPE VECTOR
-        POINTS
-            0 4
-            2 0
-            4 4
-            0 4
-        END
-        FILLED TRUE
-    END
-    """
-    exp = (
-        "SYMBOL NAME 'triangle' TYPE VECTOR POINTS 0 4 2 0 4 4 0 4 END FILLED TRUE END"
-    )
-    assert output(s, schema_name="symbol") == exp
-
-
-def test_processing_directive():
-    s = """
-    LAYER
-        NAME 'ProcessingLayer'
-        TYPE RASTER
-        PROCESSING 'BANDS=1'
-        PROCESSING 'CONTOUR_ITEM=elevation'
-        PROCESSING 'CONTOUR_INTERVAL=20'
-    END
-    """
-
-    exp = "LAYER NAME 'ProcessingLayer' TYPE RASTER PROCESSING 'BANDS=1' PROCESSING 'CONTOUR_ITEM=elevation' PROCESSING 'CONTOUR_INTERVAL=20' END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_config_directive():
-    s = """
-    MAP
-        NAME 'ConfigMap'
-        CONFIG MS_ERRORFILE 'stderr'
-        CONFIG 'PROJ_DEBUG' 'OFF'
-        CONFIG 'ON_MISSING_DATA' 'IGNORE'
-    END
-    """
-
-    exp = "MAP NAME 'ConfigMap' CONFIG 'MS_ERRORFILE' 'stderr' CONFIG 'PROJ_DEBUG' 'OFF' CONFIG 'ON_MISSING_DATA' 'IGNORE' END"
-    assert output(s) == exp
-
-
-def test_multiple_composites():
-    """
-    Allow for multiple root composites
-    This allows for easier addition of CLASSES and STYLES
-    """
-
-    s = """
-    CLASS
-        Name "Name1"
-    END
-    CLASS
-        Name "Name2"
-    END
-    """
-    exp = "CLASS NAME 'Name1' END CLASS NAME 'Name2' END"
-    assert output(s, schema_name="class") == exp
-
-
-def test_map():
-    s = """
-    MAP
-        LAYER
-            TYPE POINT
-            NAME 'test'
-        END
-    END
-    """
-
-    exp = "MAP LAYER TYPE POINT NAME 'test' END END"
-    assert output(s) == exp
-
-
-def test_querymap():
-    s = """
-    MAP
-        QUERYMAP
-           COLOR 255 255 0
-           SIZE -1 -1
-           STATUS OFF
-           STYLE HILITE
-         END
-    END
-    """
-    # print(output(s))
-    exp = "MAP QUERYMAP COLOR 255 255 0 SIZE -1 -1 STATUS OFF STYLE HILITE END END"
-    assert output(s) == exp
-
-
-def test_output_format_esri():
-    s = """
-    OUTPUTFORMAT
-        NAME "shapezip"
-        DRIVER "OGR/ESRI Shapefile"
-        TRANSPARENT ON
-        IMAGEMODE FEATURE
-    END
-    """
-    exp = "OUTPUTFORMAT NAME 'shapezip' DRIVER 'OGR/ESRI Shapefile' TRANSPARENT ON IMAGEMODE FEATURE END"
-    assert output(s, schema_name="outputformat") == exp
-
-
-def test_auto_projection():
-    """
-    Test an AUTO projection
-    """
-
-    s = """
-    MAP
-        PROJECTION
-            AUTO
-        END
-    END
-    """
-    exp = "MAP PROJECTION AUTO END END"
-    # print(output(s))
-    assert output(s) == exp
-
-
-def test_multiple_output_formats():
-    """
-    https://github.com/geographika/mappyfile/issues/20
-    """
-    s = """
-    OUTPUTFORMAT
-        FORMATOPTION "FORM=zip"
-        FORMATOPTION "SPATIAL_INDEX=YES"
-    END
-    """
-    exp = "OUTPUTFORMAT FORMATOPTION 'FORM=zip' FORMATOPTION 'SPATIAL_INDEX=YES' END"
-    assert output(s, schema_name="outputformat") == exp
-
-
-def test_config_case():
-    """
-    https://github.com/geographika/mappyfile/issues/18
-    """
-
-    s = """
-    MAP
-        CONFIG "PROJ_LIB" "projections"
-    END
-    """
-    exp = "MAP CONFIG 'PROJ_LIB' 'projections' END"
-    assert output(s) == exp
-
-
-def test_no_linebreaks():
-    """
-    Check that classes can be nested on a single line
-    Uses Earley
-    """
-    s = "CLASS NAME 'Test' STYLE OUTLINECOLOR 0 0 0 END END"
-    exp = "CLASS NAME 'Test' STYLE OUTLINECOLOR 0 0 0 END END"
-    assert output(s, schema_name="class") == exp
-
-
-def test_hexcolorrange():
-    """
-    {"colorrange": ["\"#0000ffff\"", "\"#ff0000ff\""], "datarange": [32, 255], "__type__": "style"}
-    heat.map(77) - extra hex characters to account for optional alpha values
-    COLORRANGE "#0000ffff" "#ff0000ff"
-    """
-    s = """
-    STYLE
-        COLORRANGE "#0000ffff" "#ff0000ff"
-        DATARANGE 32 255
-    END
-    """
-    exp = "STYLE COLORRANGE '#0000ffff' '#ff0000ff' DATARANGE 32 255 END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_hexcolorrange2():
-    """
-    Check different hex color formats and results are in lower-case
-    """
-
-    s = """
-    STYLE
-        DATARANGE 32 255
-        COLORRANGE '#FfF' '#Aaa'
-    END
-    """
-    exp = "STYLE DATARANGE 32 255 COLORRANGE '#fff' '#aaa' END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_colorrange():
-    s = """
-    STYLE
-      COLORRANGE 255 0 0  0 255 0
-      DATARANGE 0.01 0.05
-    END"""
-
-    exp = "STYLE COLORRANGE 255 0 0 0 255 0 DATARANGE 0.01 0.05 END"
-    print(output(s, schema_name="style"))
-    assert output(s, schema_name="style") == exp
-
-
-def test_path_numeric():
-    """
-    Make sure any folder ending with a number is not
-    split into a NAME and PATH token
-    """
-    s = """
-    LAYER
-        DATA folder123/file
-        TYPE POINT
-    END
-    """
-    exp = "LAYER DATA 'folder123/file' TYPE POINT END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_class_symbol_style():
-    """
-    barb_warm is not in quotes
-    """
-    s = """
-    CLASS
-        STYLE
-            INITIALGAP 15
-            SYMBOL "barb_warm"
-            GAP -45
-        END
-    END
-    """
-    exp = "CLASS STYLE INITIALGAP 15 SYMBOL 'barb_warm' GAP -45 END END"
-    assert output(s, schema_name="class") == exp
-
-
-def test_symbol_style():
-    """
-    barb_warm is not in quotes
-    """
-    s = """
-    STYLE
-        SYMBOL barb_warm
-    END
-    """
-    exp = "STYLE SYMBOL 'barb_warm' END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_symbol_style2():
-    """
-    barb_warm is not in quotes
-    any attributes after this cause the parser to fail
-    """
-    s = """
-    STYLE
-        SYMBOL barb_warm
-        GAP -45
-        SIZE 8
-    END
-    """
-    exp = "STYLE SYMBOL 'barb_warm' GAP -45 SIZE 8 END"
-    res = output(s, schema_name="style")
-    assert res == exp
-
-
-def test_extent():
-    """
-    Make sure any folder ending with a number is not
-    split into a NAME and PATH token
-    """
-    s = """
-    MAP
-        EXTENT -903661.3649 6426848.5209 201564.4067 8586384.8116
-    END
-    """
-    exp = "MAP EXTENT -903661.3649 6426848.5209 201564.4067 8586384.8116 END"
-    assert output(s) == exp
-
-
-def test_ogr_connection():
-    s = r"""
-    LAYER
-        CONNECTION '<OGRVRTDataSource><OGRVRTLayer name="poly"><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>'
-        TYPE POLYGON
-    END
-    """
-    exp = r"""LAYER CONNECTION '<OGRVRTDataSource><OGRVRTLayer name="poly"><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>' TYPE POLYGON END"""
-    assert output(s, schema_name="layer") == exp
-
-
-def test_quoted_data():
-    """
-    Make sure a raw string is used
-    """
-
-    s = r"""
-    LAYER
-        DATA "the_geom from (select * from road where \"lpoly_\"=3 order by gid) as foo using unique gid using srid=3978"
-        TYPE POLYGON
-    END
-    """
-    exp = r"""LAYER DATA 'the_geom from (select * from road where \"lpoly_\"=3 order by gid) as foo using unique gid using srid=3978' TYPE POLYGON END"""
-    assert output(s, schema_name="layer") == exp
-
-
-def test_name_hypens():
-    s = """
-    MAP
-        NAME ms-ogc-workshop
-    END
-    """
-    exp = "MAP NAME 'ms-ogc-workshop' END"
-    assert output(s) == exp
-
-
-def test_multiline_metadata():
-    s = """
-    METADATA
-    "ows_title" "layer_0"
-    "gml_include_items"
-    "all"
-    END
-    """
-    exp = "METADATA 'ows_title' 'layer_0' 'gml_include_items' 'all' END"
-    print(output(s, schema_name="metadata"))
-    assert output(s, schema_name="metadata") == exp
-
-
-def test_polaroffset():
-    s = """
-    STYLE  # polaroffset
-        SYMBOL "arrowhead"
-        COLOR 0 0 0
-        ANGLE [rotation]
-        POLAROFFSET [length_2] [rotation]
-    END"""
-
-    exp = "STYLE SYMBOL 'arrowhead' COLOR 0 0 0 ANGLE [rotation] POLAROFFSET [length_2] [rotation] END"
-    print(output(s, schema_name="style"))
-    assert output(s, schema_name="style") == exp
-
-
-def test_style_hexcolor():
-    s = """
-    style
-      color "#888888"
-      outlinecolor "#000000"
-    end
-    """
-
-    exp = "STYLE COLOR '#888888' OUTLINECOLOR '#000000' END"
-    print(output(s, schema_name="style"))
-    assert output(s, schema_name="style") == exp
-
-
-def test_escaped_string():
-    s = """
-    LAYER
-        FILTER (`[LASTMOD]` > `2010-12-01`)
-        TYPE POINT
-    END
-    """
-    exp = "LAYER FILTER ( `[LASTMOD]` > `2010-12-01` ) TYPE POINT END"
-    print(output(s, schema_name="layer"))
-    assert output(s, schema_name="layer") == exp
-
-
-def test_filename():
-    s = """
-    WEB
-        IMAGEURL "/tmp/"
-        TEMPLATE example3.html
-    END
-    """
-    exp = "WEB IMAGEURL '/tmp/' TEMPLATE 'example3.html' END"
-    print(output(s, schema_name="web"))
-    assert output(s, schema_name="web") == exp
-
-
-def test_label_position_uc():
-    s = """
-    LABEL
-      COLOR  0 0 0
-      FONT Vera
-      TYPE truetype
-      SIZE 8
-      POSITION UC
-      PARTIALS FALSE
-      OUTLINECOLOR 255 255 255
-    END
-    """
-    exp = "LABEL COLOR 0 0 0 FONT 'Vera' TYPE TRUETYPE SIZE 8 POSITION UC PARTIALS FALSE OUTLINECOLOR 255 255 255 END"
-    assert output(s, schema_name="label") == exp
-
-
-def test_label_attribute_properties():
-    """
-    See https://github.com/geographika/mappyfile/issues/118
-    Required allowing [property] names to be added for FONT, POSITION
-    """
-
-    s = """
-    LABEL
-        FONT [FONTNAME]
-        TYPE truetype
-        COLOR [TXTCLR]
-        SIZE [FONTSIZE]
-        ANGLE [TRIKT]
-        POSITION [MSPOS]
-        OUTLINECOLOR [OLNCLR]
-    END
-    """
-    exp = "LABEL FONT [FONTNAME] TYPE TRUETYPE COLOR [TXTCLR] SIZE [FONTSIZE] ANGLE [TRIKT] POSITION [MSPOS] OUTLINECOLOR [OLNCLR] END"
-    assert output(s, schema_name="label") == exp
-
-
-def test_style_geotransform():
-    """
-    GEOMTRANSFORM "end" (since END is used to end objects in the map file, end must be embedded in quotes)
-    http://mapserver.org/mapfile/geomtransform.html#end-and-start
-    """
-    s = """
-    STYLE
-        SIZE 0
-        GEOMTRANSFORM "end"
-    END
-    """
-
-    print(output(s, schema_name="style"))
-    exp = "STYLE SIZE 0 GEOMTRANSFORM 'end' END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_font_symbol():
-    """
-    GEOMTRANSFORM "end" (since END is used to end objects in the map file, end must be embedded in quotes)
-    http://mapserver.org/mapfile/geomtransform.html#end-and-start
-    """
-    s = """
-    LABEL
-        TEXT "►"
-        ANGLE FOLLOW
-        FONT "arial"
-        TYPE TRUETYPE
-    END
-    """
-
-    print(output(s, schema_name="label"))
-    exp = "LABEL TEXT '►' ANGLE FOLLOW FONT 'arial' TYPE TRUETYPE END"
-    assert output(s, schema_name="label") == exp
-
-
-def test_buffer_expression():
-    s = """
-    STYLE
-        GEOMTRANSFORM (buffer([shape], 20))
-    END
-    """
-
-    print(output(s, schema_name="style"))
-    exp = "STYLE GEOMTRANSFORM (buffer([shape],20)) END"
-    assert output(s, schema_name="style") == exp
-
-
-def test_single_layer_data():
-    s = """
-    LAYER
-        TYPE POINT
-        DATA "dataset1"
-    END
-    """
-    jsn = mappyfile.loads(s)
-    print(jsn)
-    jsn["data"] = "dataset1"
-    print(mappyfile.dumps(jsn))
-
-    print(output(s, schema_name="layer"))
-    exp = "LAYER TYPE POINT DATA 'dataset1' END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_cluster():
-    s = """
-    LAYER
-        TYPE POINT
-        CLUSTER
-            MAXDISTANCE 50
-            REGION "ELLIPSE"
-        END
-    END
-    """
-    print(output(s, schema_name="layer"))
-    exp = "LAYER TYPE POINT CLUSTER MAXDISTANCE 50 REGION 'ELLIPSE' END END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_cluster2():
-    """
-    Technically this is not correct and should not parse as the region
-    type should be in quotes. MapServer will throw an
-    a Symbol definition error. Parsing error near (ELLIPSE)
-    """
-    s = """
-    LAYER
-        TYPE POINT
-        CLUSTER
-            MAXDISTANCE 50
-            REGION ELLIPSE
-        END
-    END
-    """
-    print(output(s, schema_name="layer"))
-    exp = "LAYER TYPE POINT CLUSTER MAXDISTANCE 50 REGION 'ELLIPSE' END END"
-    assert output(s, schema_name="layer") == exp
-
-
-def test_outputformat_unquoted_keyword():
-    s = """
-    MAP
-        OUTPUTFORMAT
-          NAME grid
-          IMAGEMODE INT16
-        END
-    END
-    """
-
-    exp = "MAP OUTPUTFORMAT NAME 'grid' IMAGEMODE INT16 END END"
-    assert output(s, schema_name="map") == exp
-
-
-def test_multiple_compfilters():
-    """
-    See https://github.com/geographika/mappyfile/issues/150
-    """
-
-    s = """
-    LAYER
-        NAME "point-symbol-test"
-        TYPE POINT
-        COMPOSITE
-            COMPFILTER "blacken()"
-            COMPFILTER "translate(-6,-5)"
-            COMPFILTER "blur(7)"
-            COMPOP "soft-light"
-            OPACITY 50
-        END
-        COMPOSITE
-            OPACITY 100
-        END
-    END
-    """
-
-    print(output(s, schema_name="layer"))
-    exp = (
-        "LAYER NAME 'point-symbol-test' TYPE POINT COMPOSITE COMPFILTER 'blacken()' "
-        "COMPFILTER 'translate(-6,-5)' COMPFILTER 'blur(7)' COMPOP 'soft-light' OPACITY 50 END COMPOSITE OPACITY 100 END END"
-    )
-    assert output(s, schema_name="layer") == exp
-
-
-def test_multiple_leader_styles():
-    """
-    See https://github.com/geographika/mappyfile/issues/150
-    """
-
-    s = """
-LEADER
-    GRIDSTEP 10
-    MAXDISTANCE 100
-    STYLE
-        COLOR 255 255 255
-        WIDTH 3
-    END
-    STYLE
-        COLOR 80 80 80
-        WIDTH 1
-    END
-END"""
-
-    print(output(s, schema_name="leader"))
-    exp = "LEADER GRIDSTEP 10 MAXDISTANCE 100 STYLE COLOR 255 255 255 WIDTH 3 END STYLE COLOR 80 80 80 WIDTH 1 END END"
-    assert output(s, schema_name="leader") == exp
-
-
-@pytest.mark.xfail
-def test_geomtransform_nested_function():
-    s = """
-LAYER
-    NAME 'centerline1'
-    TYPE LINE
-    GEOMTRANSFORM (centerline(densify([shape], 5)))
-END"""
-
-    print(output(s, schema_name="layer"))
-    exp = "LAYER NAME 'centerline1' TYPE LINE GEOMTRANSFORM (centerline(densify([shape],5))) END"
-    assert output(s, schema_name="leader") == exp
-
-
-def test_class_regex_expression():
-    s = """
-CLASS
-    EXPRESSION /*1/
-    STYLE
-        COLOR 0 255 0
-    END
-END"""
-
-    print(output(s, schema_name="class"))
-    exp = "CLASS EXPRESSION /*1/ STYLE COLOR 0 255 0 END END"
-    assert output(s, schema_name="class") == exp
-
-
-def run_tests():
-    r"""
-    Need to comment out the following line in C:\VirtualEnvs\mappyfile\Lib\site-packages\pep8.py
-    #stdin_get_value = sys.stdin.read
-    Or get AttributeError: '_ReplInput' object has no attribute 'read'
-    """
-    # pytest.main(["tests/test_snippets.py::test_style_pattern"])
-    pytest.main(["tests/test_snippets.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    # test_multiple_compfilters()
-    # test_geomtransform_nested_function()
-    test_class_regex_expression()
-    # run_tests()
-    print("Done!")
+# -*- coding: utf-8 -*-
+
+import logging
+import inspect
+import pytest
+import mappyfile
+from mappyfile.parser import Parser
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.transformer import MapfileToDict
+from mappyfile.validator import Validator
+
+
+def output(s, include_position=True, schema_name="map"):
+    """
+    Parse, transform, validate, and pretty print
+    the result
+    """
+    p = Parser()
+    m = MapfileToDict(include_position=include_position)
+
+    # https://stackoverflow.com/questions/900392/getting-the-caller-function-name-inside-another-function-in-python
+    logging.info(inspect.stack()[1][3])
+
+    ast = p.parse(s)
+    logging.debug(ast.pretty())
+    d = m.transform(ast)
+    logging.debug(d)
+    v = Validator()
+    errors = v.validate(d, schema_name=schema_name)
+    logging.error(errors)
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    s = pp.pprint(d)
+    logging.debug(s)
+    assert len(errors) == 0
+    return s
+
+
+def check_result(s, schema_name="map"):
+    s2 = output(s, schema_name=schema_name)
+    try:
+        assert s == s2
+    except AssertionError:
+        logging.info(s)
+        logging.info(s2)
+        raise
+
+
+def test_layer():
+    s = "LAYER NAME 'Test' TYPE POINT END"
+    check_result(s, schema_name="layer")
+
+
+def test_class():
+    s = "CLASS NAME 'Test' END"
+    check_result(s, schema_name="class")
+
+
+def test_map_size():
+    s = """
+    MAP
+    SIZE 256 256
+    END"""
+
+    exp = "MAP SIZE 256 256 END"
+    assert output(s) == exp
+
+
+def test_style_color():
+    s = """
+    STYLE
+    COLOR 0 0 255
+    END"""
+
+    exp = "STYLE COLOR 0 0 255 END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style():
+    s = """
+    STYLE
+    COLOR 0 0 255
+    WIDTH 5
+    LINECAP BUTT
+    END"""
+
+    exp = "STYLE COLOR 0 0 255 WIDTH 5 LINECAP BUTT END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_oneline():
+    s = "STYLE COLOR 0 0 255 WIDTH 5 LINECAP BUTT END"
+    check_result(s, schema_name="style")
+
+
+def test_style_pattern():
+    s = """
+    STYLE
+        PATTERN 5 5 END
+    END
+    """
+
+    exp = "STYLE PATTERN 5 5 END END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_pattern2():
+    s = """
+    STYLE
+        PATTERN
+            5 5
+        END
+    END
+    """
+
+    exp = "STYLE PATTERN 5 5 END END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_pattern3():
+    """
+    Test a STYLE on one line can be parsed
+    """
+    s = "STYLE PATTERN 5 5 END END"
+    exp = "STYLE PATTERN 5 5 END END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_pattern4():
+    """
+    Test pattern values on separate lines are valid
+    """
+    s = """
+    STYLE
+        PATTERN
+            5
+            5
+        END
+    END
+    """
+    exp = "STYLE PATTERN 5 5 END END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_pattern5():
+    """
+    Test pattern with decimal places
+    """
+    s = """
+    STYLE
+        PATTERN
+            5.0 5.0
+        END
+    END
+    """
+    exp = "STYLE PATTERN 5.0 5.0 END END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_offset_mixed():
+    """
+    Test an attribute and numerical pair for a STYLE OFFSET
+    See https://github.com/geographika/mappyfile/issues/114
+    """
+    s = """
+    STYLE
+        OFFSET [attribute] -999
+    END
+    """
+    exp = "STYLE OFFSET [attribute] -999 END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_offset_mixed2():
+    """
+    As above but reversed
+    """
+    s = """
+    STYLE
+        OFFSET -999 [attribute]
+    END
+    """
+    exp = "STYLE OFFSET -999 [attribute] END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_metadata():
+    """
+    Parse metadata directly
+    """
+    s = """
+    METADATA
+        'wms_title' 'Test simple wms'
+    END
+    """
+    exp = """METADATA 'wms_title' 'Test simple wms' END"""
+    assert output(s, schema_name="metadata") == exp
+
+
+def test_metadata_uppercase():
+    s = """
+    METADATA
+        'WMS_TITLE' 'Test simple wms'
+    END
+    """
+    exp = """METADATA 'wms_title' 'Test simple wms' END"""
+    assert output(s, schema_name="metadata") == exp
+
+
+def test_duplicated_metadata_keys():
+    """
+    The second key will be used
+    """
+
+    s = """
+    METADATA
+        'wms_title' 'Test simple wms'
+        'wms_title' 'Test simple wms2'
+    END
+    """
+    exp = """METADATA 'wms_title' 'Test simple wms2' END"""
+    assert output(s, schema_name="metadata") == exp
+
+
+def test_metadata_unquoted():
+    """
+    The METADATA block doesn't need quotes
+    (as long as values don't have spaces)
+    The printer will add quotes automatically
+    """
+    s = """
+    METADATA
+        wms_title my_title
+    END
+    """
+    exp = "METADATA 'wms_title' 'my_title' END"
+    assert output(s, schema_name="metadata") == exp
+
+
+def test_validation():
+    """
+    Parse validation block directly
+    """
+    s = """
+    VALIDATION
+        "field1" "^[0-9,]+$"
+        "field2" "-1"
+        qstring '.'
+    END
+    """
+    exp = """VALIDATION 'field1' '^[0-9,]+$' 'field2' '-1' 'qstring' '.' END"""
+    assert output(s, schema_name="validation") == exp
+
+
+def test_layer_text_query():
+    s = """
+    CLASS
+        TEXT (tostring([area],"%.2f"))
+    END
+    """
+    exp = """CLASS TEXT (tostring([area],"%.2f")) END"""
+    assert output(s, schema_name="class") == exp
+
+
+def test_label():
+    s = """
+    LABEL
+      COLOR  0 0 0
+      FONT Vera
+      TYPE truetype
+      SIZE 8
+      POSITION AUTO
+      PARTIALS FALSE
+      OUTLINECOLOR 255 255 255
+    END
+    """
+    exp = "LABEL COLOR 0 0 0 FONT 'Vera' TYPE TRUETYPE SIZE 8 POSITION AUTO PARTIALS FALSE OUTLINECOLOR 255 255 255 END"
+    assert output(s, schema_name="label") == exp
+
+
+def test_output_format():
+    s = """
+    MAP
+        IMAGETYPE grid
+        OUTPUTFORMAT
+            NAME grid2
+            DRIVER "GDAL/AAIGRID"
+            IMAGEMODE INT16
+            FORMATOPTION 'NULLVALUE=-99'
+        END
+    END
+    """
+    exp = "MAP IMAGETYPE 'grid' OUTPUTFORMAT NAME 'grid2' DRIVER 'GDAL/AAIGRID' IMAGEMODE INT16 FORMATOPTION 'NULLVALUE=-99' END END"
+    assert output(s) == exp
+
+
+def test_class_symbol():
+    s = """
+    CLASS
+        STYLE # a shadow
+            COLOR 151 151 151
+            SYMBOL [symbol]
+            OFFSET 2 2
+            SIZE [size]
+        END
+    END
+    """
+    exp = "CLASS STYLE COLOR 151 151 151 SYMBOL [symbol] OFFSET 2 2 SIZE [size] END END"
+    assert output(s, schema_name="class") == exp
+
+
+def test_filter():
+    s = """
+    LAYER
+        TYPE POINT
+        NAME 'filters_test002'
+        FILTER 'aitkin'i
+    END
+    """
+
+    exp = "LAYER TYPE POINT NAME 'filters_test002' FILTER 'aitkin'i END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_like_filter():
+    s = """
+    LAYER
+        TYPE POINT
+        NAME 'filters_test003'
+        FILTER ("blpu_classification_code" LIKE 'RI%')
+    END
+    """
+
+    exp = r"""LAYER TYPE POINT NAME 'filters_test003' FILTER ( "blpu_classification_code" LIKE 'RI%' ) END"""
+    assert output(s, schema_name="layer") == exp
+
+
+def test_regex():
+    s = r"""
+    LAYER
+        TYPE POINT
+        NAME 'regexp-example'
+        FILTERITEM 'placename'
+        FILTER /hotel/
+    END
+    """
+    exp = r"LAYER TYPE POINT NAME 'regexp-example' FILTERITEM 'placename' FILTER /hotel/ END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_feature():
+    """
+    With multiple points
+    """
+
+    s = """
+    FEATURE
+        POINTS
+            0 10
+        END
+    END
+    """
+
+    exp = "FEATURE POINTS 0 10 END END"
+    assert output(s, schema_name="feature") == exp
+
+
+def test_multi_feature():
+    """
+    With multiple points
+    """
+
+    s = """
+        LAYER
+            TYPE LINE
+            FEATURE
+                POINTS
+                    0 10
+                END
+                POINTS
+                    -20 20
+                    20 20
+                    -20 -20
+                    0 -30
+                    20 -20
+                    -20 20
+                    -20 20
+                    30 30
+                END
+            END
+        END
+    """
+
+    exp = "LAYER TYPE LINE FEATURE POINTS 0 10 END POINTS -20 20 20 20 -20 -20 0 -30 20 -20 -20 20 -20 20 30 30 END END END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_triple_feature():
+    """
+    With multiple points
+    """
+
+    s = """
+    FEATURE
+        POINTS
+            0 10
+            5 2
+        END
+        POINTS
+            0 10
+            3 3
+        END
+        POINTS
+            0 10
+            7 7
+        END
+    END
+    """
+
+    exp = "FEATURE POINTS 0 10 5 2 END POINTS 0 10 3 3 END POINTS 0 10 7 7 END END"
+    assert output(s, schema_name="feature") == exp
+
+
+def test_symbol():
+    s = """
+    SYMBOL
+        NAME 'triangle'
+        TYPE VECTOR
+        POINTS
+            0 4
+            2 0
+            4 4
+            0 4
+        END
+        FILLED TRUE
+    END
+    """
+    exp = (
+        "SYMBOL NAME 'triangle' TYPE VECTOR POINTS 0 4 2 0 4 4 0 4 END FILLED TRUE END"
+    )
+    assert output(s, schema_name="symbol") == exp
+
+
+def test_processing_directive():
+    s = """
+    LAYER
+        NAME 'ProcessingLayer'
+        TYPE RASTER
+        PROCESSING 'BANDS=1'
+        PROCESSING 'CONTOUR_ITEM=elevation'
+        PROCESSING 'CONTOUR_INTERVAL=20'
+    END
+    """
+
+    exp = "LAYER NAME 'ProcessingLayer' TYPE RASTER PROCESSING 'BANDS=1' PROCESSING 'CONTOUR_ITEM=elevation' PROCESSING 'CONTOUR_INTERVAL=20' END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_config_directive():
+    s = """
+    MAP
+        NAME 'ConfigMap'
+        CONFIG MS_ERRORFILE 'stderr'
+        CONFIG 'PROJ_DEBUG' 'OFF'
+        CONFIG 'ON_MISSING_DATA' 'IGNORE'
+    END
+    """
+
+    exp = "MAP NAME 'ConfigMap' CONFIG 'MS_ERRORFILE' 'stderr' CONFIG 'PROJ_DEBUG' 'OFF' CONFIG 'ON_MISSING_DATA' 'IGNORE' END"
+    assert output(s) == exp
+
+
+def test_multiple_composites():
+    """
+    Allow for multiple root composites
+    This allows for easier addition of CLASSES and STYLES
+    """
+
+    s = """
+    CLASS
+        Name "Name1"
+    END
+    CLASS
+        Name "Name2"
+    END
+    """
+    exp = "CLASS NAME 'Name1' END CLASS NAME 'Name2' END"
+    assert output(s, schema_name="class") == exp
+
+
+def test_map():
+    s = """
+    MAP
+        LAYER
+            TYPE POINT
+            NAME 'test'
+        END
+    END
+    """
+
+    exp = "MAP LAYER TYPE POINT NAME 'test' END END"
+    assert output(s) == exp
+
+
+def test_querymap():
+    s = """
+    MAP
+        QUERYMAP
+           COLOR 255 255 0
+           SIZE -1 -1
+           STATUS OFF
+           STYLE HILITE
+         END
+    END
+    """
+    # print(output(s))
+    exp = "MAP QUERYMAP COLOR 255 255 0 SIZE -1 -1 STATUS OFF STYLE HILITE END END"
+    assert output(s) == exp
+
+
+def test_output_format_esri():
+    s = """
+    OUTPUTFORMAT
+        NAME "shapezip"
+        DRIVER "OGR/ESRI Shapefile"
+        TRANSPARENT ON
+        IMAGEMODE FEATURE
+    END
+    """
+    exp = "OUTPUTFORMAT NAME 'shapezip' DRIVER 'OGR/ESRI Shapefile' TRANSPARENT ON IMAGEMODE FEATURE END"
+    assert output(s, schema_name="outputformat") == exp
+
+
+def test_auto_projection():
+    """
+    Test an AUTO projection
+    """
+
+    s = """
+    MAP
+        PROJECTION
+            AUTO
+        END
+    END
+    """
+    exp = "MAP PROJECTION AUTO END END"
+    # print(output(s))
+    assert output(s) == exp
+
+
+def test_multiple_output_formats():
+    """
+    https://github.com/geographika/mappyfile/issues/20
+    """
+    s = """
+    OUTPUTFORMAT
+        FORMATOPTION "FORM=zip"
+        FORMATOPTION "SPATIAL_INDEX=YES"
+    END
+    """
+    exp = "OUTPUTFORMAT FORMATOPTION 'FORM=zip' FORMATOPTION 'SPATIAL_INDEX=YES' END"
+    assert output(s, schema_name="outputformat") == exp
+
+
+def test_config_case():
+    """
+    https://github.com/geographika/mappyfile/issues/18
+    """
+
+    s = """
+    MAP
+        CONFIG "PROJ_LIB" "projections"
+    END
+    """
+    exp = "MAP CONFIG 'PROJ_LIB' 'projections' END"
+    assert output(s) == exp
+
+
+def test_no_linebreaks():
+    """
+    Check that classes can be nested on a single line
+    Uses Earley
+    """
+    s = "CLASS NAME 'Test' STYLE OUTLINECOLOR 0 0 0 END END"
+    exp = "CLASS NAME 'Test' STYLE OUTLINECOLOR 0 0 0 END END"
+    assert output(s, schema_name="class") == exp
+
+
+def test_hexcolorrange():
+    """
+    {"colorrange": ["\"#0000ffff\"", "\"#ff0000ff\""], "datarange": [32, 255], "__type__": "style"}
+    heat.map(77) - extra hex characters to account for optional alpha values
+    COLORRANGE "#0000ffff" "#ff0000ff"
+    """
+    s = """
+    STYLE
+        COLORRANGE "#0000ffff" "#ff0000ff"
+        DATARANGE 32 255
+    END
+    """
+    exp = "STYLE COLORRANGE '#0000ffff' '#ff0000ff' DATARANGE 32 255 END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_hexcolorrange2():
+    """
+    Check different hex color formats and results are in lower-case
+    """
+
+    s = """
+    STYLE
+        DATARANGE 32 255
+        COLORRANGE '#FfF' '#Aaa'
+    END
+    """
+    exp = "STYLE DATARANGE 32 255 COLORRANGE '#fff' '#aaa' END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_colorrange():
+    s = """
+    STYLE
+      COLORRANGE 255 0 0  0 255 0
+      DATARANGE 0.01 0.05
+    END"""
+
+    exp = "STYLE COLORRANGE 255 0 0 0 255 0 DATARANGE 0.01 0.05 END"
+    print(output(s, schema_name="style"))
+    assert output(s, schema_name="style") == exp
+
+
+def test_path_numeric():
+    """
+    Make sure any folder ending with a number is not
+    split into a NAME and PATH token
+    """
+    s = """
+    LAYER
+        DATA folder123/file
+        TYPE POINT
+    END
+    """
+    exp = "LAYER DATA 'folder123/file' TYPE POINT END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_class_symbol_style():
+    """
+    barb_warm is not in quotes
+    """
+    s = """
+    CLASS
+        STYLE
+            INITIALGAP 15
+            SYMBOL "barb_warm"
+            GAP -45
+        END
+    END
+    """
+    exp = "CLASS STYLE INITIALGAP 15 SYMBOL 'barb_warm' GAP -45 END END"
+    assert output(s, schema_name="class") == exp
+
+
+def test_symbol_style():
+    """
+    barb_warm is not in quotes
+    """
+    s = """
+    STYLE
+        SYMBOL barb_warm
+    END
+    """
+    exp = "STYLE SYMBOL 'barb_warm' END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_symbol_style2():
+    """
+    barb_warm is not in quotes
+    any attributes after this cause the parser to fail
+    """
+    s = """
+    STYLE
+        SYMBOL barb_warm
+        GAP -45
+        SIZE 8
+    END
+    """
+    exp = "STYLE SYMBOL 'barb_warm' GAP -45 SIZE 8 END"
+    res = output(s, schema_name="style")
+    assert res == exp
+
+
+def test_extent():
+    """
+    Make sure any folder ending with a number is not
+    split into a NAME and PATH token
+    """
+    s = """
+    MAP
+        EXTENT -903661.3649 6426848.5209 201564.4067 8586384.8116
+    END
+    """
+    exp = "MAP EXTENT -903661.3649 6426848.5209 201564.4067 8586384.8116 END"
+    assert output(s) == exp
+
+
+def test_ogr_connection():
+    s = r"""
+    LAYER
+        CONNECTION '<OGRVRTDataSource><OGRVRTLayer name="poly"><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>'
+        TYPE POLYGON
+    END
+    """
+    exp = r"""LAYER CONNECTION '<OGRVRTDataSource><OGRVRTLayer name="poly"><SrcLayer>poly</SrcLayer></OGRVRTLayer></OGRVRTDataSource>' TYPE POLYGON END"""
+    assert output(s, schema_name="layer") == exp
+
+
+def test_quoted_data():
+    """
+    Make sure a raw string is used
+    """
+
+    s = r"""
+    LAYER
+        DATA "the_geom from (select * from road where \"lpoly_\"=3 order by gid) as foo using unique gid using srid=3978"
+        TYPE POLYGON
+    END
+    """
+    exp = r"""LAYER DATA 'the_geom from (select * from road where \"lpoly_\"=3 order by gid) as foo using unique gid using srid=3978' TYPE POLYGON END"""
+    assert output(s, schema_name="layer") == exp
+
+
+def test_name_hypens():
+    s = """
+    MAP
+        NAME ms-ogc-workshop
+    END
+    """
+    exp = "MAP NAME 'ms-ogc-workshop' END"
+    assert output(s) == exp
+
+
+def test_multiline_metadata():
+    s = """
+    METADATA
+    "ows_title" "layer_0"
+    "gml_include_items"
+    "all"
+    END
+    """
+    exp = "METADATA 'ows_title' 'layer_0' 'gml_include_items' 'all' END"
+    print(output(s, schema_name="metadata"))
+    assert output(s, schema_name="metadata") == exp
+
+
+def test_polaroffset():
+    s = """
+    STYLE  # polaroffset
+        SYMBOL "arrowhead"
+        COLOR 0 0 0
+        ANGLE [rotation]
+        POLAROFFSET [length_2] [rotation]
+    END"""
+
+    exp = "STYLE SYMBOL 'arrowhead' COLOR 0 0 0 ANGLE [rotation] POLAROFFSET [length_2] [rotation] END"
+    print(output(s, schema_name="style"))
+    assert output(s, schema_name="style") == exp
+
+
+def test_style_hexcolor():
+    s = """
+    style
+      color "#888888"
+      outlinecolor "#000000"
+    end
+    """
+
+    exp = "STYLE COLOR '#888888' OUTLINECOLOR '#000000' END"
+    print(output(s, schema_name="style"))
+    assert output(s, schema_name="style") == exp
+
+
+def test_escaped_string():
+    s = """
+    LAYER
+        FILTER (`[LASTMOD]` > `2010-12-01`)
+        TYPE POINT
+    END
+    """
+    exp = "LAYER FILTER ( `[LASTMOD]` > `2010-12-01` ) TYPE POINT END"
+    print(output(s, schema_name="layer"))
+    assert output(s, schema_name="layer") == exp
+
+
+def test_filename():
+    s = """
+    WEB
+        IMAGEURL "/tmp/"
+        TEMPLATE example3.html
+    END
+    """
+    exp = "WEB IMAGEURL '/tmp/' TEMPLATE 'example3.html' END"
+    print(output(s, schema_name="web"))
+    assert output(s, schema_name="web") == exp
+
+
+def test_label_position_uc():
+    s = """
+    LABEL
+      COLOR  0 0 0
+      FONT Vera
+      TYPE truetype
+      SIZE 8
+      POSITION UC
+      PARTIALS FALSE
+      OUTLINECOLOR 255 255 255
+    END
+    """
+    exp = "LABEL COLOR 0 0 0 FONT 'Vera' TYPE TRUETYPE SIZE 8 POSITION UC PARTIALS FALSE OUTLINECOLOR 255 255 255 END"
+    assert output(s, schema_name="label") == exp
+
+
+def test_label_attribute_properties():
+    """
+    See https://github.com/geographika/mappyfile/issues/118
+    Required allowing [property] names to be added for FONT, POSITION
+    """
+
+    s = """
+    LABEL
+        FONT [FONTNAME]
+        TYPE truetype
+        COLOR [TXTCLR]
+        SIZE [FONTSIZE]
+        ANGLE [TRIKT]
+        POSITION [MSPOS]
+        OUTLINECOLOR [OLNCLR]
+    END
+    """
+    exp = "LABEL FONT [FONTNAME] TYPE TRUETYPE COLOR [TXTCLR] SIZE [FONTSIZE] ANGLE [TRIKT] POSITION [MSPOS] OUTLINECOLOR [OLNCLR] END"
+    assert output(s, schema_name="label") == exp
+
+
+def test_style_geotransform():
+    """
+    GEOMTRANSFORM "end" (since END is used to end objects in the map file, end must be embedded in quotes)
+    http://mapserver.org/mapfile/geomtransform.html#end-and-start
+    """
+    s = """
+    STYLE
+        SIZE 0
+        GEOMTRANSFORM "end"
+    END
+    """
+
+    print(output(s, schema_name="style"))
+    exp = "STYLE SIZE 0 GEOMTRANSFORM 'end' END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_font_symbol():
+    """
+    GEOMTRANSFORM "end" (since END is used to end objects in the map file, end must be embedded in quotes)
+    http://mapserver.org/mapfile/geomtransform.html#end-and-start
+    """
+    s = """
+    LABEL
+        TEXT "►"
+        ANGLE FOLLOW
+        FONT "arial"
+        TYPE TRUETYPE
+    END
+    """
+
+    print(output(s, schema_name="label"))
+    exp = "LABEL TEXT '►' ANGLE FOLLOW FONT 'arial' TYPE TRUETYPE END"
+    assert output(s, schema_name="label") == exp
+
+
+def test_buffer_expression():
+    s = """
+    STYLE
+        GEOMTRANSFORM (buffer([shape], 20))
+    END
+    """
+
+    print(output(s, schema_name="style"))
+    exp = "STYLE GEOMTRANSFORM (buffer([shape],20)) END"
+    assert output(s, schema_name="style") == exp
+
+
+def test_single_layer_data():
+    s = """
+    LAYER
+        TYPE POINT
+        DATA "dataset1"
+    END
+    """
+    jsn = mappyfile.loads(s)
+    print(jsn)
+    jsn["data"] = "dataset1"
+    print(mappyfile.dumps(jsn))
+
+    print(output(s, schema_name="layer"))
+    exp = "LAYER TYPE POINT DATA 'dataset1' END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_cluster():
+    s = """
+    LAYER
+        TYPE POINT
+        CLUSTER
+            MAXDISTANCE 50
+            REGION "ELLIPSE"
+        END
+    END
+    """
+    print(output(s, schema_name="layer"))
+    exp = "LAYER TYPE POINT CLUSTER MAXDISTANCE 50 REGION 'ELLIPSE' END END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_cluster2():
+    """
+    Technically this is not correct and should not parse as the region
+    type should be in quotes. MapServer will throw an
+    a Symbol definition error. Parsing error near (ELLIPSE)
+    """
+    s = """
+    LAYER
+        TYPE POINT
+        CLUSTER
+            MAXDISTANCE 50
+            REGION ELLIPSE
+        END
+    END
+    """
+    print(output(s, schema_name="layer"))
+    exp = "LAYER TYPE POINT CLUSTER MAXDISTANCE 50 REGION 'ELLIPSE' END END"
+    assert output(s, schema_name="layer") == exp
+
+
+def test_outputformat_unquoted_keyword():
+    s = """
+    MAP
+        OUTPUTFORMAT
+          NAME grid
+          IMAGEMODE INT16
+        END
+    END
+    """
+
+    exp = "MAP OUTPUTFORMAT NAME 'grid' IMAGEMODE INT16 END END"
+    assert output(s, schema_name="map") == exp
+
+
+def test_multiple_compfilters():
+    """
+    See https://github.com/geographika/mappyfile/issues/150
+    """
+
+    s = """
+    LAYER
+        NAME "point-symbol-test"
+        TYPE POINT
+        COMPOSITE
+            COMPFILTER "blacken()"
+            COMPFILTER "translate(-6,-5)"
+            COMPFILTER "blur(7)"
+            COMPOP "soft-light"
+            OPACITY 50
+        END
+        COMPOSITE
+            OPACITY 100
+        END
+    END
+    """
+
+    print(output(s, schema_name="layer"))
+    exp = (
+        "LAYER NAME 'point-symbol-test' TYPE POINT COMPOSITE COMPFILTER 'blacken()' "
+        "COMPFILTER 'translate(-6,-5)' COMPFILTER 'blur(7)' COMPOP 'soft-light' OPACITY 50 END COMPOSITE OPACITY 100 END END"
+    )
+    assert output(s, schema_name="layer") == exp
+
+
+def test_multiple_leader_styles():
+    """
+    See https://github.com/geographika/mappyfile/issues/150
+    """
+
+    s = """
+LEADER
+    GRIDSTEP 10
+    MAXDISTANCE 100
+    STYLE
+        COLOR 255 255 255
+        WIDTH 3
+    END
+    STYLE
+        COLOR 80 80 80
+        WIDTH 1
+    END
+END"""
+
+    print(output(s, schema_name="leader"))
+    exp = "LEADER GRIDSTEP 10 MAXDISTANCE 100 STYLE COLOR 255 255 255 WIDTH 3 END STYLE COLOR 80 80 80 WIDTH 1 END END"
+    assert output(s, schema_name="leader") == exp
+
+
+@pytest.mark.xfail
+def test_geomtransform_nested_function():
+    s = """
+LAYER
+    NAME 'centerline1'
+    TYPE LINE
+    GEOMTRANSFORM (centerline(densify([shape], 5)))
+END"""
+
+    print(output(s, schema_name="layer"))
+    exp = "LAYER NAME 'centerline1' TYPE LINE GEOMTRANSFORM (centerline(densify([shape],5))) END"
+    assert output(s, schema_name="leader") == exp
+
+
+def test_class_regex_expression():
+    s = """
+CLASS
+    EXPRESSION /*1/
+    STYLE
+        COLOR 0 255 0
+    END
+END"""
+
+    print(output(s, schema_name="class"))
+    exp = "CLASS EXPRESSION /*1/ STYLE COLOR 0 255 0 END END"
+    assert output(s, schema_name="class") == exp
+
+
+def run_tests():
+    r"""
+    Need to comment out the following line in C:\VirtualEnvs\mappyfile\Lib\site-packages\pep8.py
+    #stdin_get_value = sys.stdin.read
+    Or get AttributeError: '_ReplInput' object has no attribute 'read'
+    """
+    # pytest.main(["tests/test_snippets.py::test_style_pattern"])
+    pytest.main(["tests/test_snippets.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    # test_multiple_compfilters()
+    # test_geomtransform_nested_function()
+    test_class_regex_expression()
+    # run_tests()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_symbolset.py` & `mappyfile-1.0.2/tests/test_symbolset.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import logging
-import json
-import pytest
-from mappyfile.parser import Parser
-from mappyfile.pprint import PrettyPrinter
-from mappyfile.transformer import MapfileToDict
-from mappyfile.validator import Validator
-
-
-def output(s, include_position=True, schema_name="map"):
-    """
-    Parse, transform, validate, and pretty print
-    the result
-    """
-    p = Parser()
-    m = MapfileToDict(include_position=include_position)
-    ast = p.parse(s)
-    logging.debug(ast.pretty())
-    d = m.transform(ast)
-    logging.debug(json.dumps(d, indent=4))
-    v = Validator()
-    errors = v.validate(d, schema_name=schema_name)
-    logging.error(errors)
-    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
-    s = pp.pprint(d)
-    logging.debug(s)
-    assert len(errors) == 0
-    return s
-
-
-def test_symbolset_include():
-    s = """
-    MAP
-        NAME "Test"
-        SYMBOLSET "./symbolset.txt"
-        SIZE 200 200
-    END
-    """
-
-    print(output(s, schema_name="map"))
-    exp = "MAP NAME 'Test' SYMBOLSET './symbolset.txt' SIZE 200 200 END"
-    assert output(s, schema_name="map") == exp
-
-
-def test_symbolset_file():
-    s = """
-    SYMBOLSET
-        SYMBOL
-            NAME 'default-circle'
-            TYPE ELLIPSE
-            FILLED TRUE
-            POINTS
-                1 1
-            END
-        END
-        SYMBOL
-            NAME 'other-circle'
-            TYPE ELLIPSE
-            FILLED FALSE
-            POINTS
-                1 1
-            END
-        END
-    END
-    """
-
-    print(output(s, schema_name="symbolset"))
-    exp = (
-        "SYMBOLSET SYMBOL NAME 'default-circle' TYPE ELLIPSE FILLED TRUE POINTS 1 1 END "
-        "END SYMBOL NAME 'other-circle' TYPE ELLIPSE FILLED FALSE POINTS 1 1 END END END"
-    )
-    assert output(s, schema_name="symbolset") == exp
-
-
-def run_tests():
-    pytest.main(["tests/test_symbolset.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    run_tests()
-    print("Done!")
+import logging
+import json
+import pytest
+from mappyfile.parser import Parser
+from mappyfile.pprint import PrettyPrinter
+from mappyfile.transformer import MapfileToDict
+from mappyfile.validator import Validator
+
+
+def output(s, include_position=True, schema_name="map"):
+    """
+    Parse, transform, validate, and pretty print
+    the result
+    """
+    p = Parser()
+    m = MapfileToDict(include_position=include_position)
+    ast = p.parse(s)
+    logging.debug(ast.pretty())
+    d = m.transform(ast)
+    logging.debug(json.dumps(d, indent=4))
+    v = Validator()
+    errors = v.validate(d, schema_name=schema_name)
+    logging.error(errors)
+    pp = PrettyPrinter(indent=0, newlinechar=" ", quote="'")
+    s = pp.pprint(d)
+    logging.debug(s)
+    assert len(errors) == 0
+    return s
+
+
+def test_symbolset_include():
+    s = """
+    MAP
+        NAME "Test"
+        SYMBOLSET "./symbolset.txt"
+        SIZE 200 200
+    END
+    """
+
+    print(output(s, schema_name="map"))
+    exp = "MAP NAME 'Test' SYMBOLSET './symbolset.txt' SIZE 200 200 END"
+    assert output(s, schema_name="map") == exp
+
+
+def test_symbolset_file():
+    s = """
+    SYMBOLSET
+        SYMBOL
+            NAME 'default-circle'
+            TYPE ELLIPSE
+            FILLED TRUE
+            POINTS
+                1 1
+            END
+        END
+        SYMBOL
+            NAME 'other-circle'
+            TYPE ELLIPSE
+            FILLED FALSE
+            POINTS
+                1 1
+            END
+        END
+    END
+    """
+
+    print(output(s, schema_name="symbolset"))
+    exp = (
+        "SYMBOLSET SYMBOL NAME 'default-circle' TYPE ELLIPSE FILLED TRUE POINTS 1 1 END "
+        "END SYMBOL NAME 'other-circle' TYPE ELLIPSE FILLED FALSE POINTS 1 1 END END END"
+    )
+    assert output(s, schema_name="symbolset") == exp
+
+
+def run_tests():
+    pytest.main(["tests/test_symbolset.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.DEBUG)
+    run_tests()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_transformer.py` & `mappyfile-1.0.2/tests/test_transformer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,385 +1,385 @@
-import json
-import pytest
-from mappyfile.parser import Parser
-from mappyfile.transformer import MapfileToDict, MapfileTransformer
-
-
-def test_processing_directive():
-    s = """
-    LAYER
-        NAME 'ProcessingLayer'
-        PROCESSING 'BANDS=1'
-        PROCESSING 'CONTOUR_ITEM=elevation'
-        PROCESSING 'CONTOUR_INTERVAL=20'
-    END
-    """
-
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["processing"]) == 3
-
-
-def test_config_directive():
-    s = """
-    MAP
-        NAME 'ConfigMap'
-        CONFIG MS_ERRORFILE "stderr"
-        CONFIG "PROJ_DEBUG" "OFF"
-        CONFIG "ON_MISSING_DATA" "IGNORE"
-    END
-    """
-
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["config"]) == 3
-
-
-def test_empty_config_directive():
-    """
-    Check that a config dict can be added directly without
-    needing to create a new dict separately
-    """
-
-    s = """
-    MAP
-        NAME 'ConfigMap'
-    END
-    """
-
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    d["config"]["ms_errorfile"] = "stderr"
-    print(json.dumps(d, indent=4))
-    assert d["config"]["ms_errorfile"] == "stderr"
-    assert d["config"]["MS_ERRORFILE"] == "stderr"
-
-
-def test_metadata():
-    s = """
-    MAP
-        METADATA
-            "wms_enable_request" "*"
-            "MS_ENABLE_MODES" "!*"
-        END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert d["metadata"]["wms_enable_request"] == "*"
-    assert d["metadata"]["MS_ENABLE_MODES"] == "!*"
-    assert d["metadata"]["wms_ENABLE_request"] == "*"
-    assert d["metadata"]["MS_enable_MODES"] == "!*"
-
-
-def test_scaletoken():
-    s = """
-    SCALETOKEN
-        NAME "%border%"
-        VALUES
-            "0" "ON"
-            "255000000" "OFF"
-        END
-    END
-    """
-
-    p = Parser()
-    ast = p.parse(s)
-    print(ast.pretty())
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(d)
-    print(json.dumps(d, indent=4))
-    # print(dict(d["metadata"]))
-    assert d["__type__"] == "scaletoken"
-    assert d["values"]["0"] == "ON"
-
-
-def test_layerlist():
-    s = """
-    MAP
-        LAYER
-            NAME "Layer1"
-            TYPE LINE
-        END
-        LAYER
-            NAME "Layer2"
-            TYPE LINE
-        END
-    END
-    """
-
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(d)
-    print(json.dumps(d, indent=4))
-    # print(dict(d["metadata"]))
-    assert len(d["layers"]) == 2
-    assert d["layers"][0]["name"] == "Layer1"
-
-
-def test_expression():
-    s = """
-    CLASS
-        TEXT ([area])
-        EXPRESSION ([area])
-    END
-    CLASS
-        TEXT ("[area]")
-        EXPRESSION ("[area]")
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(d)
-    print(json.dumps(d, indent=4))
-    assert d[0]["text"] == "([area])"
-    assert d[0]["expression"] == "([area])"
-    assert d[1]["text"] == '("[area]")'
-    assert d[1]["expression"] == '("[area]")'
-
-
-def test_or_expression():
-    s = """
-    CLASS
-        EXPRESSION (([val] = 'A') OR ([val] = 'B'))
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(d)
-    print(json.dumps(d, indent=4))
-    assert d["expression"] == "( ( [val] = 'A' ) OR ( [val] = 'B' ) )"
-
-
-def test_projection():
-    s = """
-    MAP
-        PROJECTION
-            "proj=utm"
-            "ellps=GRS80"
-            "datum=NAD83"
-            "zone=15"
-            "units=m"
-            "north"
-            "no_defs"
-        END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["projection"]) == 7
-
-
-def test_auto_projection():
-    s = """
-    MAP
-        PROJECTION
-            AUTO
-        END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["projection"]) == 1
-
-
-def test_points():
-    s = """
-    FEATURE
-        POINTS 1 1 50 50 1 50 1 1 END
-        POINTS 100 100 50 50 100 50 100 100 END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict(include_position=True)
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["points"]) == 2
-    assert len(d["points"][0]) == 4
-    assert len(d["points"][0][0]) == 2
-    assert d["points"][0][0][0] == 1
-
-
-def test_pattern():
-    s = """
-    STYLE
-        PATTERN 10 1 50 50 1 50 1 1 END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["pattern"]) == 4
-    assert len(d["pattern"][0]) == 2
-    assert d["pattern"][0][0] == 10
-
-
-def test_oneline_label():
-    s = """
-    label
-      type truetype size 8 font "default"
-    end
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert d["type"] == "truetype"
-    assert d["size"] == 8
-    assert d["font"] == "default"
-    assert d["__type__"] == "label"
-
-
-def test_boolean():
-    s = """
-    LAYER
-        TRANSFORM TRUE
-        TYPE POINT
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert d["transform"]
-
-
-@pytest.mark.xfail
-def test_multiple_layer_projection():
-    """
-    TODO add validation for this case
-    """
-
-    s = """
-    MAP
-    LAYER
-        PROJECTION
-            "init=epsg:4326"
-            "init=epsg:4326"
-        END
-        PROJECTION
-            "init=epsg:4326"
-            "init=epsg:4326"
-        END
-    END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict(include_position=True)
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-    assert len(d["projection"]) == 1
-
-    p = Parser()
-    m = MapfileToDict()
-
-    ast = p.parse(s)
-    d = m.transform(ast)
-
-    print(json.dumps(d, indent=4))
-
-    from mappyfile.validator import Validator
-
-    v = Validator()
-    return v.validate(d)
-
-
-def test_token_positions():
-    s = """
-    MAP
-        SIZE 600 600
-        LAYER
-            NAME "Test"
-            TYPE POLYGON
-        END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-    t = MapfileToDict()
-    d = t.transform(ast)
-    print(json.dumps(d, indent=4))
-
-    p = Parser()
-    m = MapfileToDict()
-
-    ast = p.parse(s)
-    d = m.transform(ast)
-
-    print(json.dumps(d, indent=4))
-
-
-def test_kwargs():
-    m = MapfileToDict(custom_param="custom")
-    assert "custom_param" in m.kwargs
-
-
-def test_custom_transformer():
-    """
-    Check a custom transformer can be used with MapfileToDict, and any custom
-    parameters can be passed on to this transformer (useful for plugins)
-    """
-
-    class CustomTransformer(MapfileTransformer):
-        def __init__(self, include_position=False, include_comments=False, **kwargs):
-            self.custom_param = kwargs["custom_param"]
-            super(CustomTransformer, self).__init__(include_position, include_comments)
-
-    m = MapfileToDict(transformer_class=CustomTransformer, custom_param="custom")
-
-    s = """
-    MAP
-        SIZE 600 600
-        LAYER
-            NAME "Test"
-            TYPE POLYGON
-        END
-    END
-    """
-    p = Parser()
-    ast = p.parse(s)
-
-    d = m.transform(ast)
-    print(d)
-    assert m.mapfile_transformer.__class__.__name__ == "CustomTransformer"
-    assert m.mapfile_transformer.custom_param == "custom"
-
-
-def run_tests():
-    # pytest.main(["tests/test_transformer.py::test_config_directive"])
-    pytest.main(["tests/test_transformer.py"])
-
-
-if __name__ == "__main__":
-    # test_custom_transformer()
-    run_tests()
-    print("Done!")
+import json
+import pytest
+from mappyfile.parser import Parser
+from mappyfile.transformer import MapfileToDict, MapfileTransformer
+
+
+def test_processing_directive():
+    s = """
+    LAYER
+        NAME 'ProcessingLayer'
+        PROCESSING 'BANDS=1'
+        PROCESSING 'CONTOUR_ITEM=elevation'
+        PROCESSING 'CONTOUR_INTERVAL=20'
+    END
+    """
+
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["processing"]) == 3
+
+
+def test_config_directive():
+    s = """
+    MAP
+        NAME 'ConfigMap'
+        CONFIG MS_ERRORFILE "stderr"
+        CONFIG "PROJ_DEBUG" "OFF"
+        CONFIG "ON_MISSING_DATA" "IGNORE"
+    END
+    """
+
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["config"]) == 3
+
+
+def test_empty_config_directive():
+    """
+    Check that a config dict can be added directly without
+    needing to create a new dict separately
+    """
+
+    s = """
+    MAP
+        NAME 'ConfigMap'
+    END
+    """
+
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    d["config"]["ms_errorfile"] = "stderr"
+    print(json.dumps(d, indent=4))
+    assert d["config"]["ms_errorfile"] == "stderr"
+    assert d["config"]["MS_ERRORFILE"] == "stderr"
+
+
+def test_metadata():
+    s = """
+    MAP
+        METADATA
+            "wms_enable_request" "*"
+            "MS_ENABLE_MODES" "!*"
+        END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert d["metadata"]["wms_enable_request"] == "*"
+    assert d["metadata"]["MS_ENABLE_MODES"] == "!*"
+    assert d["metadata"]["wms_ENABLE_request"] == "*"
+    assert d["metadata"]["MS_enable_MODES"] == "!*"
+
+
+def test_scaletoken():
+    s = """
+    SCALETOKEN
+        NAME "%border%"
+        VALUES
+            "0" "ON"
+            "255000000" "OFF"
+        END
+    END
+    """
+
+    p = Parser()
+    ast = p.parse(s)
+    print(ast.pretty())
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(d)
+    print(json.dumps(d, indent=4))
+    # print(dict(d["metadata"]))
+    assert d["__type__"] == "scaletoken"
+    assert d["values"]["0"] == "ON"
+
+
+def test_layerlist():
+    s = """
+    MAP
+        LAYER
+            NAME "Layer1"
+            TYPE LINE
+        END
+        LAYER
+            NAME "Layer2"
+            TYPE LINE
+        END
+    END
+    """
+
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(d)
+    print(json.dumps(d, indent=4))
+    # print(dict(d["metadata"]))
+    assert len(d["layers"]) == 2
+    assert d["layers"][0]["name"] == "Layer1"
+
+
+def test_expression():
+    s = """
+    CLASS
+        TEXT ([area])
+        EXPRESSION ([area])
+    END
+    CLASS
+        TEXT ("[area]")
+        EXPRESSION ("[area]")
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(d)
+    print(json.dumps(d, indent=4))
+    assert d[0]["text"] == "([area])"
+    assert d[0]["expression"] == "([area])"
+    assert d[1]["text"] == '("[area]")'
+    assert d[1]["expression"] == '("[area]")'
+
+
+def test_or_expression():
+    s = """
+    CLASS
+        EXPRESSION (([val] = 'A') OR ([val] = 'B'))
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(d)
+    print(json.dumps(d, indent=4))
+    assert d["expression"] == "( ( [val] = 'A' ) OR ( [val] = 'B' ) )"
+
+
+def test_projection():
+    s = """
+    MAP
+        PROJECTION
+            "proj=utm"
+            "ellps=GRS80"
+            "datum=NAD83"
+            "zone=15"
+            "units=m"
+            "north"
+            "no_defs"
+        END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["projection"]) == 7
+
+
+def test_auto_projection():
+    s = """
+    MAP
+        PROJECTION
+            AUTO
+        END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["projection"]) == 1
+
+
+def test_points():
+    s = """
+    FEATURE
+        POINTS 1 1 50 50 1 50 1 1 END
+        POINTS 100 100 50 50 100 50 100 100 END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict(include_position=True)
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["points"]) == 2
+    assert len(d["points"][0]) == 4
+    assert len(d["points"][0][0]) == 2
+    assert d["points"][0][0][0] == 1
+
+
+def test_pattern():
+    s = """
+    STYLE
+        PATTERN 10 1 50 50 1 50 1 1 END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["pattern"]) == 4
+    assert len(d["pattern"][0]) == 2
+    assert d["pattern"][0][0] == 10
+
+
+def test_oneline_label():
+    s = """
+    label
+      type truetype size 8 font "default"
+    end
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert d["type"] == "truetype"
+    assert d["size"] == 8
+    assert d["font"] == "default"
+    assert d["__type__"] == "label"
+
+
+def test_boolean():
+    s = """
+    LAYER
+        TRANSFORM TRUE
+        TYPE POINT
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert d["transform"]
+
+
+@pytest.mark.xfail
+def test_multiple_layer_projection():
+    """
+    TODO add validation for this case
+    """
+
+    s = """
+    MAP
+    LAYER
+        PROJECTION
+            "init=epsg:4326"
+            "init=epsg:4326"
+        END
+        PROJECTION
+            "init=epsg:4326"
+            "init=epsg:4326"
+        END
+    END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict(include_position=True)
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+    assert len(d["projection"]) == 1
+
+    p = Parser()
+    m = MapfileToDict()
+
+    ast = p.parse(s)
+    d = m.transform(ast)
+
+    print(json.dumps(d, indent=4))
+
+    from mappyfile.validator import Validator
+
+    v = Validator()
+    return v.validate(d)
+
+
+def test_token_positions():
+    s = """
+    MAP
+        SIZE 600 600
+        LAYER
+            NAME "Test"
+            TYPE POLYGON
+        END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+    t = MapfileToDict()
+    d = t.transform(ast)
+    print(json.dumps(d, indent=4))
+
+    p = Parser()
+    m = MapfileToDict()
+
+    ast = p.parse(s)
+    d = m.transform(ast)
+
+    print(json.dumps(d, indent=4))
+
+
+def test_kwargs():
+    m = MapfileToDict(custom_param="custom")
+    assert "custom_param" in m.kwargs
+
+
+def test_custom_transformer():
+    """
+    Check a custom transformer can be used with MapfileToDict, and any custom
+    parameters can be passed on to this transformer (useful for plugins)
+    """
+
+    class CustomTransformer(MapfileTransformer):
+        def __init__(self, include_position=False, include_comments=False, **kwargs):
+            self.custom_param = kwargs["custom_param"]
+            super(CustomTransformer, self).__init__(include_position, include_comments)
+
+    m = MapfileToDict(transformer_class=CustomTransformer, custom_param="custom")
+
+    s = """
+    MAP
+        SIZE 600 600
+        LAYER
+            NAME "Test"
+            TYPE POLYGON
+        END
+    END
+    """
+    p = Parser()
+    ast = p.parse(s)
+
+    d = m.transform(ast)
+    print(d)
+    assert m.mapfile_transformer.__class__.__name__ == "CustomTransformer"
+    assert m.mapfile_transformer.custom_param == "custom"
+
+
+def run_tests():
+    # pytest.main(["tests/test_transformer.py::test_config_directive"])
+    pytest.main(["tests/test_transformer.py"])
+
+
+if __name__ == "__main__":
+    # test_custom_transformer()
+    run_tests()
+    print("Done!")
```

### Comparing `mappyfile-1.0.1/tests/test_utils.py` & `mappyfile-1.0.2/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,163 +1,189 @@
-import logging
-import os
-import io
-import tempfile
-import mappyfile
-import pytest
-
-
-def test_open():
-    fn = "./tests/sample_maps/256_overlay_res.map"
-    d = mappyfile.open(fn)
-    assert d["name"] == "TEST"
-
-    d = mappyfile.open(fn, expand_includes=False)
-    assert d["name"] == "TEST"
-
-    d = mappyfile.open(fn, include_position=True)
-    assert d["name"] == "TEST"
-
-    d = mappyfile.open(fn, include_comments=True)
-    assert d["name"] == "TEST"
-
-
-def test_loads():
-    s = """MAP NAME "TEST" END"""
-
-    d = mappyfile.loads(s)
-    assert d["name"] == "TEST"
-
-    d = mappyfile.loads(s, expand_includes=False)
-    assert d["name"] == "TEST"
-
-    d = mappyfile.loads(s, include_position=True)
-    assert d["name"] == "TEST"
-
-    d = mappyfile.loads(s, include_comments=True)
-    assert d["name"] == "TEST"
-
-
-def test_dump():
-    s = """MAP NAME "TEST" END"""
-    d = mappyfile.loads(s)
-
-    with tempfile.NamedTemporaryFile(mode="w+", delete=False) as fp:
-        mappyfile.dump(d, fp)
-
-    with open(fp.name) as fp2:
-        d = mappyfile.load(fp2)
-
-    assert d["name"] == "TEST"
-
-
-def test_stringio():
-    s = """MAP NAME "TEST" END"""
-    ip = io.StringIO(s)
-
-    d = mappyfile.load(ip)
-
-    assert d["name"] == "TEST"
-
-
-def test_save():
-    s = """MAP NAME "TEST" END"""
-    d = mappyfile.loads(s)
-
-    output_file = os.path.join(tempfile.mkdtemp(), "test_mapfile.map")
-    mappyfile.save(d, output_file)
-
-    with open(output_file) as fp:
-        d = mappyfile.load(fp)
-
-    assert d["name"] == "TEST"
-
-
-def test_dumps():
-    s = """MAP NAME "TEST" END"""
-
-    d = mappyfile.loads(s)
-    output = mappyfile.dumps(d, indent=1, spacer="\t", newlinechar=" ")
-    print(output)
-    assert output == 'MAP 	NAME "TEST" END'
-
-
-def test_dump_with_end_comments():
-    s = """MAP NAME "TEST" END"""
-
-    d = mappyfile.loads(s)
-    output = mappyfile.dumps(
-        d, indent=1, spacer="\t", newlinechar=" ", end_comment=True
-    )
-    print(output)
-    assert output == 'MAP 	NAME "TEST" END # MAP'
-
-
-def test_create_map():
-    d = mappyfile.utils.create("map")
-    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
-    print(output)
-    assert (
-        output
-        == "MAP ANGLE 0 DEBUG 0 DEFRESOLUTION 72 IMAGETYPE 'png' MAXSIZE 4096 NAME 'MS' RESOLUTION 72 SIZE -1 -1 END"
-    )
-
-
-def test_create_layer():
-    d = mappyfile.utils.create("layer")
-    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
-    print(output)
-    assert output == "LAYER STATUS OFF TILEITEM 'location' UNITS METERS END"
-
-
-def test_create_label():
-    d = mappyfile.utils.create("label")
-    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
-    print(output)
-    assert (
-        output
-        == "LABEL ANGLE 0 ANTIALIAS FALSE BACKGROUNDSHADOWSIZE FALSE BUFFER 0 FORCE FALSE MAXOVERLAPANGLE 22.5 MAXSIZE 256 MINSIZE 4 "
-        "OFFSET 0 0 OUTLINEWIDTH 1 PARTIALS FALSE POSITION CC PRIORITY 1 REPEATDISTANCE 0 SHADOWSIZE 1 1 SIZE 10 END"
-    )
-
-
-def test_create_symbol():
-    d = mappyfile.utils.create("symbol")
-    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
-    print(output)
-    assert output == "SYMBOL ANCHORPOINT 0.5 0.5 ANTIALIAS FALSE FILLED FALSE END"
-
-
-def test_create_symbol_v6():
-    d = mappyfile.utils.create("symbol", version=6.0)
-    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
-    print(output)
-    assert output == "SYMBOL ANTIALIAS FALSE FILLED FALSE END"
-
-
-def test_create_symbol_v8():
-    d = mappyfile.utils.create("symbol", version=8.0)
-    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
-    print(output)
-    assert output == "SYMBOL ANCHORPOINT 0.5 0.5 FILLED FALSE END"
-
-
-def test_create_missing():
-    error_raised = False
-    try:
-        mappyfile.utils.create("missing")
-    except SyntaxError:
-        # raise
-        error_raised = True
-
-    assert error_raised is True
-
-
-def run_tests():
-    pytest.main(["tests/test_utils.py"])
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.INFO)
-    # run_tests()
-    test_create_missing()
-    print("Done!")
+import logging
+import os
+import io
+import tempfile
+import mappyfile
+import pytest
+from mappyfile.transformer import MapfileTransformer, MapfileToDict
+from mappyfile.parser import Parser
+
+
+class CustomTransformer(MapfileTransformer):
+    def __init__(
+        self,
+        include_position=False,
+        include_comments=False,
+        custom_parameter=False,
+    ):
+        self.custom_parameter = custom_parameter
+        super().__init__(include_position, include_comments)
+
+
+def test_open():
+    fn = "./tests/sample_maps/256_overlay_res.map"
+    d = mappyfile.open(fn)
+    assert d["name"] == "TEST"
+
+    d = mappyfile.open(fn, expand_includes=False)
+    assert d["name"] == "TEST"
+
+    d = mappyfile.open(fn, include_position=True)
+    assert d["name"] == "TEST"
+
+    d = mappyfile.open(fn, include_comments=True)
+    assert d["name"] == "TEST"
+
+
+def test_loads():
+    s = """MAP NAME "TEST" END"""
+
+    d = mappyfile.loads(s)
+    assert d["name"] == "TEST"
+
+    d = mappyfile.loads(s, expand_includes=False)
+    assert d["name"] == "TEST"
+
+    d = mappyfile.loads(s, include_position=True)
+    assert d["name"] == "TEST"
+
+    d = mappyfile.loads(s, include_comments=True)
+    assert d["name"] == "TEST"
+
+
+def test_loads_kwargs():
+    s = """MAP NAME "TEST" END"""
+    d = mappyfile.loads(s, transformer_class=CustomTransformer, custom_parameter=True)
+    assert d["name"] == "TEST"
+
+    p = Parser(expand_includes=True, include_comments=True, custom_parameter=True)
+    assert p.kwargs["custom_parameter"] is True
+    m = MapfileToDict(
+        include_position=True, include_comments=True, custom_parameter=True
+    )
+    assert m.kwargs["custom_parameter"] is True
+
+
+def test_dump():
+    s = """MAP NAME "TEST" END"""
+    d = mappyfile.loads(s)
+
+    with tempfile.NamedTemporaryFile(mode="w+", delete=False) as fp:
+        mappyfile.dump(d, fp)
+
+    with open(fp.name) as fp2:
+        d = mappyfile.load(fp2)
+
+    assert d["name"] == "TEST"
+
+
+def test_stringio():
+    s = """MAP NAME "TEST" END"""
+    ip = io.StringIO(s)
+
+    d = mappyfile.load(ip)
+
+    assert d["name"] == "TEST"
+
+
+def test_save():
+    s = """MAP NAME "TEST" END"""
+    d = mappyfile.loads(s)
+
+    output_file = os.path.join(tempfile.mkdtemp(), "test_mapfile.map")
+    mappyfile.save(d, output_file)
+
+    with open(output_file) as fp:
+        d = mappyfile.load(fp)
+
+    assert d["name"] == "TEST"
+
+
+def test_dumps():
+    s = """MAP NAME "TEST" END"""
+
+    d = mappyfile.loads(s)
+    output = mappyfile.dumps(d, indent=1, spacer="\t", newlinechar=" ")
+    print(output)
+    assert output == 'MAP 	NAME "TEST" END'
+
+
+def test_dump_with_end_comments():
+    s = """MAP NAME "TEST" END"""
+
+    d = mappyfile.loads(s)
+    output = mappyfile.dumps(
+        d, indent=1, spacer="\t", newlinechar=" ", end_comment=True
+    )
+    print(output)
+    assert output == 'MAP 	NAME "TEST" END # MAP'
+
+
+def test_create_map():
+    d = mappyfile.utils.create("map")
+    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
+    print(output)
+    assert (
+        output
+        == "MAP ANGLE 0 DEBUG 0 DEFRESOLUTION 72 IMAGETYPE 'png' MAXSIZE 4096 NAME 'MS' RESOLUTION 72 SIZE -1 -1 END"
+    )
+
+
+def test_create_layer():
+    d = mappyfile.utils.create("layer")
+    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
+    print(output)
+    assert output == "LAYER STATUS OFF TILEITEM 'location' UNITS METERS END"
+
+
+def test_create_label():
+    d = mappyfile.utils.create("label")
+    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
+    print(output)
+    assert (
+        output
+        == "LABEL ANGLE 0 ANTIALIAS FALSE BACKGROUNDSHADOWSIZE FALSE BUFFER 0 FORCE FALSE MAXOVERLAPANGLE 22.5 MAXSIZE 256 MINSIZE 4 "
+        "OFFSET 0 0 OUTLINEWIDTH 1 PARTIALS FALSE POSITION CC PRIORITY 1 REPEATDISTANCE 0 SHADOWSIZE 1 1 SIZE 10 END"
+    )
+
+
+def test_create_symbol():
+    d = mappyfile.utils.create("symbol")
+    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
+    print(output)
+    assert output == "SYMBOL ANCHORPOINT 0.5 0.5 ANTIALIAS FALSE FILLED FALSE END"
+
+
+def test_create_symbol_v6():
+    d = mappyfile.utils.create("symbol", version=6.0)
+    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
+    print(output)
+    assert output == "SYMBOL ANTIALIAS FALSE FILLED FALSE END"
+
+
+def test_create_symbol_v8():
+    d = mappyfile.utils.create("symbol", version=8.0)
+    output = mappyfile.dumps(d, indent=0, newlinechar=" ", quote="'")
+    print(output)
+    assert output == "SYMBOL ANCHORPOINT 0.5 0.5 FILLED FALSE END"
+
+
+def test_create_missing():
+    error_raised = False
+    try:
+        mappyfile.utils.create("missing")
+    except SyntaxError:
+        # raise
+        error_raised = True
+
+    assert error_raised is True
+
+
+def run_tests():
+    pytest.main(["tests/test_utils.py"])
+
+
+if __name__ == "__main__":
+    logging.basicConfig(level=logging.INFO)
+    # run_tests()
+    test_loads_kwargs()
+    print("Done!")
```

