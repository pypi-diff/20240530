# Comparing `tmp/civitdl-2.1.0.dev1.tar.gz` & `tmp/civitdl-2.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civitdl-2.1.0.dev1.tar", last modified: Mon May 27 19:49:05 2024, max compression
+gzip compressed data, was "civitdl-2.1.0.dev2.tar", last modified: Thu May 30 03:16:37 2024, max compression
```

## Comparing `civitdl-2.1.0.dev1.tar` & `civitdl-2.1.0.dev2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/License
--rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/args/
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/args/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/data/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/aliasconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/defaultconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/sorterconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/configmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/api/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/api/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/args/
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/args/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/batch/
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/batch/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/batch/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/batch/batch_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/civitdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/helpers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/__Init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/helpers/core/_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/_ui/__Init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/_ui/styler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/iohelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/hashmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/helpers/sorter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/__Init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sourcemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-30 03:16:25.000000 civitdl-2.1.0.dev2/License
+-rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-30 03:16:25.000000 civitdl-2.1.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.737135 civitdl-2.1.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitconfig/data/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/aliasconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/defaultconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/config/sorterconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitconfig/data/configmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitdl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitdl/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/api/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.741135 civitdl-2.1.0.dev2/src/civitdl/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/civitdl/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/batch/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/batch/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/civitdl/batch/batch_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/civitdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 03:16:37.000000 civitdl-2.1.0.dev2/src/civitdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/cachemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/__Init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/core/_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/_ui/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/_ui/styler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/iohelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:37.745135 civitdl-2.1.0.dev2/src/helpers/sorter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sorter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-30 03:16:26.000000 civitdl-2.1.0.dev2/src/helpers/sourcemanager.py
```

### Comparing `civitdl-2.1.0.dev1/License` & `civitdl-2.1.0.dev2/License`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/PKG-INFO` & `civitdl-2.1.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civitdl
-Version: 2.1.0.dev1
+Version: 2.1.0.dev2
 Summary: Package for batch downloading models from civitai.com
 Author: Owen Truong
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `civitdl-2.1.0.dev1/README.md` & `civitdl-2.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/pyproject.toml` & `civitdl-2.1.0.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 
 requires = [ "setuptools", "wheel", "build" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "civitdl"
-version = "2.1.0.dev1"
+version = "2.1.0.dev2"
 authors = [ 
    { name = "Owen Truong" } 
 ]
 description = "Package for batch downloading models from civitai.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "License"}
```

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/__main__.py` & `civitdl-2.1.0.dev2/src/civitconfig/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                 api_key=args['api_key'],
                 with_prompt=args['with_prompt'],
                 without_model=args['without_model'],
                 limit_rate=args['limit_rate'],
                 retry_count=args['retry_count'],
                 pause_time=args['pause_time'],
                 cache_mode=args['cache_mode'],
+                strict_mode=args['strict_mode'],
                 model_overwrite=args['model_overwrite'],
                 with_color=args['with_color']
             ))
             config_manager.print_defaults()
         elif subcommand == 'sorter':
             if args['add'] != None:
                 add_name, add_path = args['add']
```

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/args/argparser.py` & `civitdl-2.1.0.dev2/src/civitconfig/args/argparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,17 @@
                             help='Set the default max number of times to retry downloading a model if it fails.'
                             )
 
 default_parser.add_argument('--pause-time', type=float,
                             help='Set the default number of seconds to pause between each model\'s download'
                             )
 default_parser.add_argument('--cache-mode', type=str,
-                            help='Set the default cache mode. Valid modes are 0 and 1 for now. 2 is not implemented yet.')
+                            help='Set the default cache mode. Valid modes are 0 and 1. 0 to not use cache. 1 to use cache and copy existant models based on file path. Please refer to documentation for more detail.')
+default_parser.add_argument('--strict-mode', type=str,
+                            help='Sets the default strict mode. Valid modes are 0 and 1. 0 to disable integrity check. 1 to enable maximum integrity check. In scenarios where the user have previously downloaded the model and the program recognizes the repeated download, strict-mode of 1 adds a further integrity check with SHA256 hash against the local model file.')
 default_parser.add_argument('--model-overwrite', action=BooleanOptionalAction,
                             help='Set the default behavior on whether to overwrite or skip models that are already downloaded at path. model=overwrite to overwrite model. no-model-overwrite to skip model.')
 add_shared_option(default_parser)
 
 
 sorter_parser = subparsers.add_parser(
     'sorter', help='Sorter-related subcommand.\nCurrently supports listing, adding and deleting sorters.\nIf no options are provided, sorter will list all available sorters.\nExample usage: civitdl 123456 ./lora --sorter mysorter.',
```

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/data/config/aliasconfig.py` & `civitdl-2.1.0.dev2/src/civitconfig/data/config/aliasconfig.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/data/config/config.py` & `civitdl-2.1.0.dev2/src/civitconfig/data/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "with_prompt": True,
         "without_model": False,
         "limit_rate": '0',
         "retry_count": 3,
         "pause_time": 3.0,
 
         "cache_mode": '1',
+        "strict_mode": '1',
         "model_overwrite": False,
 
         "with_color": True
     },
     "sorters": [["basic", basic.sort_model.__doc__, 'basic'], ["tags", tags.sort_model.__doc__, 'tags']],
     "aliases": [["@example", "~/.models"]]
 }
```

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/data/config/defaultconfig.py` & `civitdl-2.1.0.dev2/src/civitconfig/data/config/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/data/config/sorterconfig.py` & `civitdl-2.1.0.dev2/src/civitconfig/data/config/sorterconfig.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/civitconfig/data/configmanager.py` & `civitdl-2.1.0.dev2/src/civitconfig/data/configmanager.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/civitdl/__main__.py` & `civitdl-2.1.0.dev2/src/civitdl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             with_prompt=args['with_prompt'],
             without_model=args['without_model'],
             limit_rate=args['limit_rate'],
             retry_count=args['retry_count'],
             pause_time=args['pause_time'],
 
             cache_mode=args['cache_mode'],
+            strict_mode=args['strict_mode'],
             model_overwrite=args['model_overwrite'],
 
             with_color=args['with_color'],
             verbose=args['verbose']
         )
 
         batch_download(
```

### Comparing `civitdl-2.1.0.dev1/src/civitdl/args/argparser.py` & `civitdl-2.1.0.dev2/src/civitdl/args/argparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,17 +76,20 @@
 )
 
 parser.add_argument(
     '--pause-time', metavar='FLOAT', type=float, help='Specify the number of seconds to pause between each model\'s download.'
 )
 
 parser.add_argument(
-    '--cache-mode', metavar='MODE', type=str, help='Specify the cache mode. 0 to not use cache. 1 to use cache and copy existant models based on file path. 2 to use cache and copy existant models based on file path + hashes of model. Note that mode 2 has not been implemented yet. See documentation on github for more info.'
+    '--cache-mode', metavar='MODE', type=str, help='Specify the cache mode. 0 to not use cache. 1 to use cache and copy existant models based on file path. See documentation on github for more info.'
 )
 
+parser.add_argument('--strict-mode', metavar='MODE', type=str,
+                    help='Specify the strict mode. Valid modes are 0 and 1. 0 to disable integrity check. 1 to enable maximum integrity check. In scenarios where the user have previously downloaded the model and the program recognizes the repeated download, strict-mode of 1 adds a further integrity check with SHA256 hash against the local model file.')
+
 parser.add_argument(
     '--model-overwrite', action=BooleanOptionalAction, help='Determine whether to overwrite or skip model download if model is already in path. model=overwrite to overwrite model. no-model-overwrite to skip model.'
 )
 
 parser.add_argument(
     '--with-color', action=BooleanOptionalAction, help='Enable styles like colors, background colors and bold/italized texts.'
 )
@@ -119,13 +122,14 @@
         "with_prompt": parser_result.with_prompt if parser_result.with_prompt is not None else config_defaults.get('with_prompt', None),
         "without_model": parser_result.without_model if parser_result.without_model is not None else config_defaults.get('without_model', None),
         "limit_rate": parser_result.limit_rate or config_defaults.get('limit_rate', None),
         "retry_count": parser_result.retry_count or config_defaults.get('retry_count', None),
         "pause_time": parser_result.pause_time or config_defaults.get('pause_time', None),
 
         "cache_mode": parser_result.cache_mode or config_defaults.get('cache_mode', None),
+        "strict_mode": parser_result.strict_mode or config_defaults.get('strict_mode', None),
         "model_overwrite": parser_result.model_overwrite if parser_result.model_overwrite is not None else config_defaults.get('model_overwrite', None),
 
         "with_color": parser_result.with_color if parser_result.with_color is not None else config_defaults.get('with_color', None),
 
         "verbose": False if parser_result.verbose == None else parser_result.verbose
     }
```

### Comparing `civitdl-2.1.0.dev1/src/civitdl/batch/_metadata.py` & `civitdl-2.1.0.dev2/src/civitdl/batch/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                         id.model_id, version_id=id.version_id)
         elif id.model_id is not None:
             metadata = self.__get_model_version_metadata(id.model_id)
         else:
             raise UnexpectedException(
                 f'No model and version id found for "{id.original}"')
 
-        return (metadata, (metadata[0]['id'], metadata[1]['id']))
+        return (metadata, (str(metadata[0]['id']), str(metadata[1]['id'])))
 
     def __get_model_version_metadata(self, model_id: str, version_id: Optional[str] = None):
         model_dict = self.__get_model_metadata(model_id)
         key = 'modelVersions'
 
         if key not in model_dict:
             raise ResourcesException(
@@ -105,16 +105,16 @@
 class Metadata:
     __options_nsfw_mode: str
     __options_max_images: int
     __options_session: Session
 
     model_dict: Dict
     version_dict: Dict
-    model_id: int
-    version_id: int
+    model_id: str
+    version_id: str
     model_download_url: str
 
     model_name: str = 'unknown'
     version_hashes: Dict = {}
 
     nsfwLevel: int = -1
     image_dicts: List[Dict] = []
```

### Comparing `civitdl-2.1.0.dev1/src/civitdl/batch/_model.py` & `civitdl-2.1.0.dev2/src/civitdl/batch/_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from helpers.core.utils import Styler, InputException, UnexpectedException, APIException, print_newlines, sprint, print_verbose, concurrent_request
 from helpers.core.iohelper import IOHelper
 
 from helpers.sourcemanager import Id
 from helpers.options import BatchOptions
-from helpers.hashmanager import HashManager
+from helpers.cachemanager import CacheManager
 
 from ._metadata import Metadata
 
 
 class Model:
     __dst_root_path: str
     __batchOptions: BatchOptions
@@ -62,35 +62,92 @@
         data = 'hash_name, hash_id\n'
         for key, value in hashes.items():
             data += f'{key}, {value}\n'
         IOHelper.write_to_file(
             filepath, [data.rstrip()], encoding='UTF-8')
 
     def __download_model(self, dirpath, filename: str, model_res: requests.Response, version_id: str, version_hashes: Dict):
+        # FIXME: um, refactor later on
         os.makedirs(dirpath, exist_ok=True)
         filepath = os.path.join(dirpath, filename)
-        hash_manager = HashManager(
-            version_id) if self.__batchOptions.cache_mode != '0' else None
-        cached_filepath = hash_manager.get_local_model_path() if hash_manager else None
-
-        if cached_filepath and cached_filepath != os.path.abspath(filepath):
-            print_newlines(Styler.stylize(f"""Model already existed at the following path:
-                - Path: {cached_filepath}""", color='info'))
-            sprint(Styler.stylize(f"Copying to new path...", color='info'))
-            shutil.copy(cached_filepath, filepath)
-        else:
+        sha256_hash = version_hashes.get('SHA256', None)
+        try:
+            if self.__batchOptions.cache_mode == '1':
+                cache_manager = CacheManager(
+                    version_id)
+                cached_filepath = cache_manager.get_local_model_path()
+        except:
+            sprint(Styler.stylize('Unable to access cache.', color='warning'))
+
+        def download_new_model():
             content_chunks = model_res.iter_content(
                 ceil(self.__batchOptions.limit_rate / 8)
                 if self.__batchOptions.limit_rate is not None and self.__batchOptions.limit_rate != 0
                 else 1024*1024)
             IOHelper.write_to_file(filepath, content_chunks, mode='wb', limit_rate=self.__batchOptions.limit_rate,
-                                   overwrite=self.__batchOptions.model_overwrite, use_pb=True, total=float(model_res.headers.get('content-length', 0)), desc='Model')
-        if hash_manager:
-            hash_manager.set_local_model_cache(
-                filepath, version_hashes)
+                                   use_pb=True, total=float(model_res.headers.get('content-length', 0)), desc='Model')
+
+        def cache_model_info():
+            if self.__batchOptions.cache_mode == '1' and cache_manager:
+                cache_manager.set_local_model_cache(
+                    filepath, version_hashes)
+
+        if (self.__batchOptions.strict_mode == '1' and not sha256_hash):
+            sprint(
+                Styler.stylize(
+                    f'(Strict Mode) Error with fetching SHA256 hash from CivitAI. Proceeding to download model from CivitAI.', color='warning')
+            )
+            download_new_model()
+            cache_model_info()
+            return
+
+        # Check if filepath already exist
+        if not self.__batchOptions.model_overwrite and os.path.exists(filepath):
+            if (
+                self.__batchOptions.strict_mode == '1' and not IOHelper.compare_hash(
+                    filepath, sha256_hash)
+            ):
+                sprint(
+                    Styler.stylize(
+                        f'(Strict Mode) Model file already exist at destination file path, but file does not match the hash from CivitAI.', color='warning'
+                    )
+                )
+                # I want to check cache before giving up and downloading new model.
+            else:
+                print_newlines(Styler.stylize(f"""Model file already existed at the destination path:
+                    - Path: {filepath}""", color='info'))
+                cache_model_info()
+                return
+
+        # Check cache if file exist
+        if self.__batchOptions.cache_mode == '1' and cached_filepath:
+            if not os.path.exists(cached_filepath):
+                sprint(
+                    Styler.stylize(f'Model file does not exist at cached file path.', color='warning'))
+                download_new_model()
+                cache_model_info()
+                return
+            elif self.__batchOptions.strict_mode == '1' and not IOHelper.compare_hash(cached_filepath, sha256_hash):
+                sprint(
+                    Styler.stylize(
+                        f'(Strict Mode) Cached file path of model does not match the hash from CivitAI. Proceeding to download model from CivitAI.', color='warning'
+                    ))
+                download_new_model()
+                cache_model_info()
+                return
+            else:
+                print_newlines(Styler.stylize(f"""Model file already existed at the following path:
+                    - Path: {cached_filepath}""", color='info'))
+                sprint(Styler.stylize(f"Copying to new path...", color='info'))
+                shutil.copy(cached_filepath, filepath)
+                cache_model_info()
+                return
+
+        download_new_model()
+        cache_model_info()
 
     def __request_model(self, model_id: str, version_id: str, model_download_url: str):
         # Request model
         print_verbose('Preparing to send download model request...')
         print_verbose(f'Model Download API URL: {model_download_url}')
 
         headers = {
@@ -210,14 +267,16 @@
             model_name=metadata.model_name,
             image_download_urls=metadata.image_download_urls,
             content_disposition=model_res.headers.get('Content-Disposition') if model_res else None)
 
         sorter_data = self.__batchOptions.sorter(
             metadata.model_dict, metadata.version_dict, os.path.split(filenames['model'])[0], self.__dst_root_path)
 
+        # print(sorter_data.metadata_dir_path)
+
         # 3. Download model and etc.
 
         self.__download_metadata(
             dirpath=sorter_data.metadata_dir_path,
             filename=filenames['metadata'],
             model_dict=metadata.model_dict
         )
```

### Comparing `civitdl-2.1.0.dev1/src/civitdl/batch/batch_download.py` & `civitdl-2.1.0.dev2/src/civitdl/batch/batch_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import time
 import traceback
 from typing import List
 
 from ._model import Model
 
 from helpers.core.utils import Styler, APIException, get_version, print_exc, print_verbose, run_verbose, sprint
@@ -19,15 +20,14 @@
 
 def batch_download(source_strings: List[str], rootdir: str, batchOptions: BatchOptions):
     """Batch downloads model from CivitAI one by one."""
 
     source_manager = SourceManager()
 
     for id in source_manager.parse_src(source_strings):
-
         iter = 0
         while True:
             try:
                 model = Model(dst_root_path=rootdir,
                               batchOptions=batchOptions).download(id=id)
                 _pause(batchOptions.pause_time)
                 break
```

### Comparing `civitdl-2.1.0.dev1/src/civitdl.egg-info/PKG-INFO` & `civitdl-2.1.0.dev2/src/civitdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civitdl
-Version: 2.1.0.dev1
+Version: 2.1.0.dev2
 Summary: Package for batch downloading models from civitai.com
 Author: Owen Truong
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `civitdl-2.1.0.dev1/src/civitdl.egg-info/SOURCES.txt` & `civitdl-2.1.0.dev2/src/civitdl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 src/civitdl/api/sorter.py
 src/civitdl/args/argparser.py
 src/civitdl/batch/_metadata.py
 src/civitdl/batch/_model.py
 src/civitdl/batch/batch_download.py
 src/helpers/__init__.py
 src/helpers/argparse.py
-src/helpers/hashmanager.py
+src/helpers/cachemanager.py
 src/helpers/options.py
 src/helpers/sourcemanager.py
 src/helpers/core/__Init__.py
 src/helpers/core/_validation.py
 src/helpers/core/constants.py
 src/helpers/core/iohelper.py
 src/helpers/core/utils.py
```

### Comparing `civitdl-2.1.0.dev1/src/helpers/argparse.py` & `civitdl-2.1.0.dev2/src/helpers/argparse.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/helpers/core/_ui/styler.py` & `civitdl-2.1.0.dev2/src/helpers/core/_ui/styler.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/helpers/core/_validation.py` & `civitdl-2.1.0.dev2/src/helpers/core/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,17 +201,18 @@
 
         if len(value.strip()) is not len(value):
             print(Styler.stylize(
                 f'Directory path provided by {arg_name} contains leading and trailing space. Proceeding to trim the following "{value}"', color='WARNING')).encode()
             value = value.trim()
 
         modified_value = value.replace('/', '\\') if os.name == 'nt' else value
-        if os.name == 'nt' and os.path.isabs(modified_value):
-            modified_value = modified_value[2:]
-        dir_names = [s for s in modified_value.split(os.path.sep) if s != ""]
+
+        test_value = modified_value[2:] if os.name == 'nt' and os.path.isabs(
+            modified_value) else modified_value
+        dir_names = [s for s in test_value.split(os.path.sep) if s != ""]
         for dir_name in dir_names:
             try:
                 cls.validate_dir_name(dir_name, arg_name)
             except InputException as e:
                 raise InputException(
                     e, f'The invalid directory path is {value}')
```

### Comparing `civitdl-2.1.0.dev1/src/helpers/core/iohelper.py` & `civitdl-2.1.0.dev2/src/helpers/core/iohelper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import shutil
 import sys
 import time
 import csv
+import hashlib
 from typing import IO, Callable, Iterable, Union
 
 from ._ui.styler import Styler, InputException, UnexpectedException
-from .utils import get_progress_bar, sprint
+from .utils import get_progress_bar, print_verbose, sprint
 
 
 class IOHelper:
 
     # Level 0 #
 
     @staticmethod
@@ -59,14 +60,30 @@
                     raise InputException(
                         f'CSV file is invalid. File contains rows with more than two columns.\nThe filepath for the invalid csv is "{filepath}"')
                 except:
                     csv_dict[row[0]] = row[1]
 
         return csv_dict
 
+    @staticmethod
+    def compare_hash(filepath: str, hash: str):
+        hasher = hashlib.sha256()
+        chunk_size = 2**20
+
+        with open(filepath, 'rb') as file:
+            while True:
+                chunk = file.read(chunk_size)
+                if not chunk:
+                    break
+                hasher.update(chunk)
+
+        digest = hasher.hexdigest().upper()
+        print_verbose(f'Computed SHA256: "{digest}", Expected SHA256: "{hash}"')  # nopep8
+        return digest == hash
+
     # Level 1 #
     @classmethod
     def write_to_file(cls, filepath: str, content_chunks: Iterable, mode: str = None, limit_rate: Union[int, None] = 0, encoding: Union[str, None] = None, overwrite: bool = True, use_pb: bool = False, total: float = 0, desc: str = None):
         """Uses content_chunks to write to filepath bit by bit. If use_pb is enabled, it is recommended to set total kwarg to the length of the file to be written."""
         progress_bar = get_progress_bar(total, desc) if use_pb else None
 
         def update_progress_bar(bytes_downloaded):
```

### Comparing `civitdl-2.1.0.dev1/src/helpers/core/utils.py` & `civitdl-2.1.0.dev2/src/helpers/core/utils.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/helpers/hashmanager.py` & `civitdl-2.1.0.dev2/src/helpers/cachemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from helpers.core.utils import Styler, print_verbose, sprint
 from helpers.core.constants import app_dirs
 
 # TODO: Watch out for edge cases where one of the hash is empty.
 # { '123456': { 'model_filepath': 'path', 'SHA256': 'hash1', 'BLAKE3': 'hash2' } }
 
 
-class HashManager:
+class CacheManager:
     __CACHE_COLUMNS = ['volume_id', 'model_filepath', 'SHA256', 'BLAKE3']
     __version_id: str
     __filepath: str
     __hashes_dict: Dict
 
     def __init__(self, version_id: str):
         self.__version_id = version_id
```

### Comparing `civitdl-2.1.0.dev1/src/helpers/options.py` & `civitdl-2.1.0.dev2/src/helpers/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 
     with_prompt: bool = True
     without_model: bool = False
     limit_rate: int = 0
     retry_count: int = 3
     pause_time: int = 3
 
-    cache_mode: Literal['0', '1', '2'] = '1'
+    cache_mode: Literal['0', '1'] = '1'
+    strict_mode: Literal['0', '1'] = '1'
+
     model_overwrite: bool = False
 
     with_color: bool = False
     verbose: Optional[bool] = None
 
     def __get_sorter(self, sorter: str):
         if not isinstance(sorter, property) and not isinstance(sorter, str):
@@ -62,15 +64,15 @@
             self._sorter = tags.sort_model if sorter_str == 'tags' else basic.sort_model
         else:
             self._sorter = import_sort_model(sorter_str)
 
         print_verbose("Chosen Sorter Description: ", self._sorter.__doc__)
         return self._sorter
 
-    def __init__(self, retry_count, pause_time, max_images, nsfw_mode, with_prompt, without_model, api_key, verbose, sorter, limit_rate, cache_mode, model_overwrite, with_color):
+    def __init__(self, retry_count, pause_time, max_images, nsfw_mode, with_prompt, without_model, api_key, verbose, sorter, limit_rate, cache_mode, strict_mode, model_overwrite, with_color):
         self.session = requests.Session()
 
         # FIXME: Move usage of with_color and verbose outside of options
         if with_color is not None:
             Validation.validate_bool(with_color, 'with_color')
             self.with_color = with_color
             if with_color == False:
@@ -120,20 +122,23 @@
 
         if pause_time is not None:
             Validation.validate_float(pause_time, 'pause_time', min_value=0)
             self.pause_time = pause_time
 
         if cache_mode is not None:
             Validation.validate_string(
-                cache_mode, 'cache_mode', whitelist=['0', '1', '2'])
-            if cache_mode == '2':
-                raise NotImplementedException(
-                    'cache mode of 2 has not been implemented yet')
+                cache_mode, 'cache_mode', whitelist=['0', '1'])
             self.cache_mode = cache_mode
 
+        if strict_mode is not None:
+            Validation.validate_string(
+                strict_mode, 'strict_mode', whitelist=['0', '1']
+            )
+            self.strict_mode = strict_mode
+
         if model_overwrite is not None:
             Validation.validate_bool(model_overwrite, 'model_overwrite')
             self.model_overwrite = model_overwrite
 
 
 class DefaultOptions:
     sorter: Optional[str] = None
@@ -143,20 +148,21 @@
 
     with_prompt: Optional[bool] = None
     without_model: Optional[bool] = None
     limit_rate: Optional[str] = None
     retry_count: Optional[int] = None
     pause_time: Optional[int] = None
 
-    cache_mode: Optional[int] = None
+    cache_mode: Optional[str] = None
+    strict_mode: Optional[str] = None
     model_overwrite: Optional[bool] = None
 
     with_color: Optional[bool] = None
 
-    def __init__(self, sorter=None, max_images=None, nsfw_mode=None, api_key=None, with_prompt=None, without_model=None, limit_rate=None, retry_count=None, pause_time=None, cache_mode=None, model_overwrite=None, with_color=None):
+    def __init__(self, sorter=None, max_images=None, nsfw_mode=None, api_key=None, with_prompt=None, without_model=None, limit_rate=None, retry_count=None, pause_time=None, cache_mode=None, strict_mode=None, model_overwrite=None, with_color=None):
         if sorter is not None:
             Validation.validate_string(
                 sorter, 'sorter')
 
             self.sorter = sorter
 
         if max_images is not None:
@@ -198,21 +204,24 @@
             Validation.validate_float(
                 pause_time, 'pause_time', min_value=0
             )
             self.pause_time = pause_time
 
         if cache_mode is not None:
             Validation.validate_string(
-                cache_mode, 'cache_mode', whitelist=['0', '1', '2']
+                cache_mode, 'cache_mode', whitelist=['0', '1']
             )
-            if cache_mode == '2':
-                raise NotImplementedException(
-                    'cache mode of 2 has not been implemented yet')
             self.cache_mode = cache_mode
 
+        if strict_mode is not None:
+            Validation.validate_string(
+                strict_mode, 'strict_mode', whitelist=['0', '1']
+            )
+            self.strict_mode = strict_mode
+
         if model_overwrite is not None:
             Validation.validate_bool(model_overwrite, 'model_overwrite')
             self.model_overwrite = model_overwrite
 
         if with_color is not None:
             Validation.validate_bool(with_color, 'with_color')
             self.with_color = with_color
```

### Comparing `civitdl-2.1.0.dev1/src/helpers/sorter/basic.py` & `civitdl-2.1.0.dev2/src/helpers/sorter/basic.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/helpers/sorter/tags.py` & `civitdl-2.1.0.dev2/src/helpers/sorter/tags.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/helpers/sorter/utils.py` & `civitdl-2.1.0.dev2/src/helpers/sorter/utils.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.1.0.dev1/src/helpers/sourcemanager.py` & `civitdl-2.1.0.dev2/src/helpers/sourcemanager.py`

 * *Files identical despite different names*

