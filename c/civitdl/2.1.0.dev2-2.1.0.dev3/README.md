# Comparing `tmp/civitdl-2.1.0.dev2.tar.gz` & `tmp/civitdl-2.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civitdl-2.1.0.dev2.tar", last modified: Thu May 30 03:16:37 2024, max compression
+gzip compressed data, was "civitdl-2.1.0.dev3.tar", last modified: Thu May 30 16:44:55 2024, max compression
```

## Comparing `civitdl-2.1.0.dev2.tar` & `civitdl-2.1.0.dev3.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-30 03:16:25.000000 civitdl-2.1.0.dev2/License
--rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-30 03:16:25.000000 civitdl-2.1.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.737135 civitdl-2.1.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/args/
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/args/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/data/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/aliasconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/defaultconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/sorterconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/configmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitdl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitdl/api/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/api/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitdl/args/
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/args/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/civitdl/batch/
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/batch/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/batch/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/batch/batch_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/civitdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/cachemanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/__Init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/core/_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/_ui/__Init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/_ui/styler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/iohelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/sorter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/__Init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sourcemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.815598 civitdl-2.1.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-30 16:44:50.000000 civitdl-2.1.0.dev3/License
+-rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-05-30 16:44:55.815598 civitdl-2.1.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-30 16:44:50.000000 civitdl-2.1.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:44:55.815598 civitdl-2.1.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.803598 civitdl-2.1.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.807598 civitdl-2.1.0.dev3/src/civitconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.807598 civitdl-2.1.0.dev3/src/civitconfig/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.807598 civitdl-2.1.0.dev3/src/civitconfig/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.807598 civitdl-2.1.0.dev3/src/civitconfig/data/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/config/aliasconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/config/defaultconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/config/sorterconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitconfig/data/configmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.807598 civitdl-2.1.0.dev3/src/civitdl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/civitdl/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/api/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/civitdl/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/civitdl/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/batch/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/batch/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitdl/batch/batch_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.815598 civitdl-2.1.0.dev3/src/civitdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-05-30 16:44:55.000000 civitdl-2.1.0.dev3/src/civitdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 16:44:55.000000 civitdl-2.1.0.dev3/src/civitdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:44:55.000000 civitdl-2.1.0.dev3/src/civitdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 16:44:55.000000 civitdl-2.1.0.dev3/src/civitdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 16:44:55.000000 civitdl-2.1.0.dev3/src/civitdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:44:55.000000 civitdl-2.1.0.dev3/src/civitdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/civitmisc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitmisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitmisc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/civitmisc/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/civitmisc/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/helpers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/__Init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.811598 civitdl-2.1.0.dev3/src/helpers/core/_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/_ui/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/_ui/styler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/iohelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:55.815598 civitdl-2.1.0.dev3/src/helpers/sorter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/sorter/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/sorter/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/sorter/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/sorter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-30 16:44:51.000000 civitdl-2.1.0.dev3/src/helpers/sourcemanager.py
```

### Comparing `civitdl-2.1.0.dev2/License` & `civitdl-2.1.0.dev3/License`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/PKG-INFO` & `civitdl-2.1.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civitdl
-Version: 2.1.0.dev2
+Version: 2.1.0.dev3
 Summary: Package for batch downloading models from civitai.com
 Author: Owen Truong
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Repository, https://github.com/OwenTruong/civitdl
 Project-URL: Bug Tracker, https://github.com/OwenTruong/civitdl/issues
 Keywords: civitai,batch download
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: tqdm<5,>=4.66.1
 Requires-Dist: appdirs<2,>=1.4.4
 Requires-Dist: argparse<2,>=1.4
@@ -231,14 +231,15 @@
 
 ## Navigate
 - [README Page](/README.md)
 - [Alias Page](/doc/alias.md)
 - [API Key Page](/doc/api_key.md)
 - [Civitconfig / Configuration Page](/doc/civitconfig.md)
 - [Civitdl Page](/doc/civitdl.md)
+- [Civitmisc Page](/doc/civitmisc.md)
 - [Sorter Page](/doc/sorter.md)
 
 <br/>
 
 ## Table Of Contents
 - [civitdl (civitai-batch-download)](#civitdl-civitai-batch-download)
   - [Navigate](#navigate)
```

### Comparing `civitdl-2.1.0.dev2/README.md` & `civitdl-2.1.0.dev3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ## Navigate
 - [README Page](/README.md)
 - [Alias Page](/doc/alias.md)
 - [API Key Page](/doc/api_key.md)
 - [Civitconfig / Configuration Page](/doc/civitconfig.md)
 - [Civitdl Page](/doc/civitdl.md)
+- [Civitmisc Page](/doc/civitmisc.md)
 - [Sorter Page](/doc/sorter.md)
 
 <br/>
 
 ## Table Of Contents
 - [civitdl (civitai-batch-download)](#civitdl-civitai-batch-download)
   - [Navigate](#navigate)
```

### Comparing `civitdl-2.1.0.dev2/pyproject.toml` & `civitdl-2.1.0.dev3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 
 requires = [ "setuptools", "wheel", "build" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "civitdl"
-version = "2.1.0.dev2"
+version = "2.1.0.dev3"
 authors = [ 
    { name = "Owen Truong" } 
 ]
 description = "Package for batch downloading models from civitai.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "License"}
 keywords = ["civitai", "batch download"]
 classifiers = [
    "Programming Language :: Python :: 3.8",
-   "License :: OSI Approved :: MIT License",
+   "License :: OSI Approved :: Apache Software License",
    "Operating System :: OS Independent"
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Repository = "https://github.com/OwenTruong/civitdl"
 "Bug Tracker" = "https://github.com/OwenTruong/civitdl/issues"
 
 [project.scripts]
 civitdl = "civitdl.__main__:main"
-civitconfig = "civitconfig.__main__:main"
+civitconfig = "civitconfig.__main__:main"
+civitmisc = "civitmisc.__main__:main"
```

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/__main__.py` & `civitdl-2.1.0.dev3/src/civitconfig/__main__.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/args/argparser.py` & `civitdl-2.1.0.dev3/src/civitconfig/args/argparser.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/data/config/aliasconfig.py` & `civitdl-2.1.0.dev3/src/civitconfig/data/config/aliasconfig.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/data/config/config.py` & `civitdl-2.1.0.dev3/src/civitconfig/data/config/config.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/data/config/defaultconfig.py` & `civitdl-2.1.0.dev3/src/civitconfig/data/config/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/data/config/sorterconfig.py` & `civitdl-2.1.0.dev3/src/civitconfig/data/config/sorterconfig.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitconfig/data/configmanager.py` & `civitdl-2.1.0.dev3/src/civitconfig/data/configmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,7 +98,9 @@
         if os.path.isdir(dst_path):
             dst_path = os.path.join(dst_path, 'civitdl_config')
 
         sprint(Styler.stylize(
             f'Downloading zipped config to {dst_path}.zip', color='main'))
         shutil.make_archive(dst_path, 'zip',
                             self._config_dir_path)
+
+    # def scanPath(self, dir_path):
```

### Comparing `civitdl-2.1.0.dev2/src/civitdl/__main__.py` & `civitdl-2.1.0.dev3/src/civitdl/__main__.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitdl/args/argparser.py` & `civitdl-2.1.0.dev3/src/civitdl/args/argparser.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitdl/batch/_metadata.py` & `civitdl-2.1.0.dev3/src/civitdl/batch/_metadata.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitdl/batch/_model.py` & `civitdl-2.1.0.dev3/src/civitdl/batch/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from helpers.core.utils import Styler, InputException, UnexpectedException, APIException, print_newlines, sprint, print_verbose, concurrent_request
 from helpers.core.iohelper import IOHelper
 
 from helpers.sourcemanager import Id
 from helpers.options import BatchOptions
-from helpers.cachemanager import CacheManager
+from helpers.cache import Cache
 
 from ._metadata import Metadata
 
 
 class Model:
     __dst_root_path: str
     __batchOptions: BatchOptions
@@ -68,31 +68,31 @@
     def __download_model(self, dirpath, filename: str, model_res: requests.Response, version_id: str, version_hashes: Dict):
         # FIXME: um, refactor later on
         os.makedirs(dirpath, exist_ok=True)
         filepath = os.path.join(dirpath, filename)
         sha256_hash = version_hashes.get('SHA256', None)
         try:
             if self.__batchOptions.cache_mode == '1':
-                cache_manager = CacheManager(
+                cache = Cache(
                     version_id)
-                cached_filepath = cache_manager.get_local_model_path()
+                cached_filepath = cache.get_local_model_path()
         except:
             sprint(Styler.stylize('Unable to access cache.', color='warning'))
 
         def download_new_model():
             content_chunks = model_res.iter_content(
                 ceil(self.__batchOptions.limit_rate / 8)
                 if self.__batchOptions.limit_rate is not None and self.__batchOptions.limit_rate != 0
                 else 1024*1024)
             IOHelper.write_to_file(filepath, content_chunks, mode='wb', limit_rate=self.__batchOptions.limit_rate,
                                    use_pb=True, total=float(model_res.headers.get('content-length', 0)), desc='Model')
 
         def cache_model_info():
-            if self.__batchOptions.cache_mode == '1' and cache_manager:
-                cache_manager.set_local_model_cache(
+            if self.__batchOptions.cache_mode == '1' and cache:
+                cache.set_local_model_cache(
                     filepath, version_hashes)
 
         if (self.__batchOptions.strict_mode == '1' and not sha256_hash):
             sprint(
                 Styler.stylize(
                     f'(Strict Mode) Error with fetching SHA256 hash from CivitAI. Proceeding to download model from CivitAI.', color='warning')
             )
```

### Comparing `civitdl-2.1.0.dev2/src/civitdl/batch/batch_download.py` & `civitdl-2.1.0.dev3/src/civitdl/batch/batch_download.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/civitdl.egg-info/PKG-INFO` & `civitdl-2.1.0.dev3/src/civitdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civitdl
-Version: 2.1.0.dev2
+Version: 2.1.0.dev3
 Summary: Package for batch downloading models from civitai.com
 Author: Owen Truong
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Repository, https://github.com/OwenTruong/civitdl
 Project-URL: Bug Tracker, https://github.com/OwenTruong/civitdl/issues
 Keywords: civitai,batch download
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: tqdm<5,>=4.66.1
 Requires-Dist: appdirs<2,>=1.4.4
 Requires-Dist: argparse<2,>=1.4
@@ -231,14 +231,15 @@
 
 ## Navigate
 - [README Page](/README.md)
 - [Alias Page](/doc/alias.md)
 - [API Key Page](/doc/api_key.md)
 - [Civitconfig / Configuration Page](/doc/civitconfig.md)
 - [Civitdl Page](/doc/civitdl.md)
+- [Civitmisc Page](/doc/civitmisc.md)
 - [Sorter Page](/doc/sorter.md)
 
 <br/>
 
 ## Table Of Contents
 - [civitdl (civitai-batch-download)](#civitdl-civitai-batch-download)
   - [Navigate](#navigate)
```

### Comparing `civitdl-2.1.0.dev2/src/civitdl.egg-info/SOURCES.txt` & `civitdl-2.1.0.dev3/src/civitdl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 src/civitdl.egg-info/requires.txt
 src/civitdl.egg-info/top_level.txt
 src/civitdl/api/sorter.py
 src/civitdl/args/argparser.py
 src/civitdl/batch/_metadata.py
 src/civitdl/batch/_model.py
 src/civitdl/batch/batch_download.py
+src/civitmisc/__init__.py
+src/civitmisc/__main__.py
+src/civitmisc/args/argparser.py
 src/helpers/__init__.py
 src/helpers/argparse.py
-src/helpers/cachemanager.py
+src/helpers/cache.py
 src/helpers/options.py
 src/helpers/sourcemanager.py
 src/helpers/core/__Init__.py
 src/helpers/core/_validation.py
 src/helpers/core/constants.py
 src/helpers/core/iohelper.py
 src/helpers/core/utils.py
```

### Comparing `civitdl-2.1.0.dev2/src/helpers/argparse.py` & `civitdl-2.1.0.dev3/src/helpers/argparse.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/core/_ui/styler.py` & `civitdl-2.1.0.dev3/src/helpers/core/_ui/styler.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/core/_validation.py` & `civitdl-2.1.0.dev3/src/helpers/core/_validation.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/core/iohelper.py` & `civitdl-2.1.0.dev3/src/helpers/core/iohelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 import sys
 import time
 import csv
 import hashlib
-from typing import IO, Callable, Iterable, Union
+from typing import IO, Callable, Iterable, List, Union
 
 from ._ui.styler import Styler, InputException, UnexpectedException
 from .utils import get_progress_bar, print_verbose, sprint
 
 
 class IOHelper:
 
@@ -60,14 +60,18 @@
                     raise InputException(
                         f'CSV file is invalid. File contains rows with more than two columns.\nThe filepath for the invalid csv is "{filepath}"')
                 except:
                     csv_dict[row[0]] = row[1]
 
         return csv_dict
 
+    # @staticmethod
+    # def read_multiple_columns_from_csv(filepath: str):
+    #     return {}
+
     @staticmethod
     def compare_hash(filepath: str, hash: str):
         hasher = hashlib.sha256()
         chunk_size = 2**20
 
         with open(filepath, 'rb') as file:
             while True:
@@ -77,14 +81,15 @@
                 hasher.update(chunk)
 
         digest = hasher.hexdigest().upper()
         print_verbose(f'Computed SHA256: "{digest}", Expected SHA256: "{hash}"')  # nopep8
         return digest == hash
 
     # Level 1 #
+
     @classmethod
     def write_to_file(cls, filepath: str, content_chunks: Iterable, mode: str = None, limit_rate: Union[int, None] = 0, encoding: Union[str, None] = None, overwrite: bool = True, use_pb: bool = False, total: float = 0, desc: str = None):
         """Uses content_chunks to write to filepath bit by bit. If use_pb is enabled, it is recommended to set total kwarg to the length of the file to be written."""
         progress_bar = get_progress_bar(total, desc) if use_pb else None
 
         def update_progress_bar(bytes_downloaded):
             if progress_bar:
```

### Comparing `civitdl-2.1.0.dev2/src/helpers/core/utils.py` & `civitdl-2.1.0.dev3/src/helpers/core/utils.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/options.py` & `civitdl-2.1.0.dev3/src/helpers/options.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/sorter/basic.py` & `civitdl-2.1.0.dev3/src/helpers/sorter/basic.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/sorter/tags.py` & `civitdl-2.1.0.dev3/src/helpers/sorter/tags.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/sorter/utils.py` & `civitdl-2.1.0.dev3/src/helpers/sorter/utils.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev2/src/helpers/sourcemanager.py` & `civitdl-2.1.0.dev3/src/helpers/sourcemanager.py`

 * *Files identical despite different names*

