# Comparing `tmp/ensembl_utils-0.1.2.tar.gz` & `tmp/ensembl_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembl_utils-0.1.2.tar", last modified: Wed May 29 16:13:00 2024, max compression
+gzip compressed data, was "ensembl_utils-0.1.3.tar", last modified: Thu May 30 17:25:07 2024, max compression
```

## Comparing `ensembl_utils-0.1.2.tar` & `ensembl_utils-0.1.3.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.067073 ensembl_utils-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.051073 ensembl_utils-0.1.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/.github/actions/python_build/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/actions/python_build/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-29 16:13:00.063073 ensembl_utils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/gen_ref_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)   133459 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/img/ebang.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/install.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:13:00.067073 ensembl_utils-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.055073 ensembl_utils-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.051073 ensembl_utils-0.1.2/src/ensembl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/src/ensembl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/src/ensembl/utils/rloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.063073 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 16:13:00.000000 ensembl_utils-0.1.2/src/ensembl_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/archive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/archive/test_archive/
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive/sample.tar
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive/sample.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive/sample.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/archive/test_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/argparse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/argparse/test_argparse/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/argparse/test_argparse/sample.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/argparse/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/logging/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.059073 ensembl_utils-0.1.2/tests/rloader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:13:00.063073 ensembl_utils-0.1.2/tests/rloader/test_rloader/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.env
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.ini
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader/sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-29 16:12:49.000000 ensembl_utils-0.1.2/tests/rloader/test_rloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.838777 ensembl_utils-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.826777 ensembl_utils-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.822776 ensembl_utils-0.1.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.826777 ensembl_utils-0.1.3/.github/actions/python_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.github/actions/python_build/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.826777 ensembl_utils-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.github/workflows/notice.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/.licenserc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-30 17:25:07.838777 ensembl_utils-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/docs/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   133459 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/docs/img/ebang.png
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/docs/install.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/docs/scripts/gen_ref_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:25:07.838777 ensembl_utils-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.826777 ensembl_utils-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.826777 ensembl_utils-0.1.3/src/ensembl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/src/ensembl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/src/ensembl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/src/ensembl/utils/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/src/ensembl/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/src/ensembl/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/src/ensembl/utils/rloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.834777 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-30 17:25:07.000000 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 17:25:07.000000 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:25:07.000000 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 17:25:07.000000 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 17:25:07.000000 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 17:25:07.000000 ensembl_utils-0.1.3/src/ensembl_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/tests/archive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/tests/archive/test_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/archive/test_archive/sample.tar
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/archive/test_archive/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/archive/test_archive/sample.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/archive/test_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.830777 ensembl_utils-0.1.3/tests/argparse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.834777 ensembl_utils-0.1.3/tests/argparse/test_argparse/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/argparse/test_argparse/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/argparse/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.834777 ensembl_utils-0.1.3/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/logging/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.834777 ensembl_utils-0.1.3/tests/rloader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:25:07.834777 ensembl_utils-0.1.3/tests/rloader/test_rloader/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/rloader/test_rloader/sample.env
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/rloader/test_rloader/sample.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/rloader/test_rloader/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/rloader/test_rloader/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/rloader/test_rloader/sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 17:24:56.000000 ensembl_utils-0.1.3/tests/rloader/test_rloader.py
```

### Comparing `ensembl_utils-0.1.2/.github/actions/python_build/action.yml` & `ensembl_utils-0.1.3/.github/actions/python_build/action.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/.github/dependabot.yml` & `ensembl_utils-0.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/.github/workflows/ci.yml` & `ensembl_utils-0.1.3/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -16,87 +16,100 @@
 name: "CI"
 
 on:
   push:
     branches:
       - main
   pull_request:
-
-permissions: write-all
+  workflow_dispatch:
 
 defaults:
   run:
     working-directory: ./
 
 env:
   PYTHON_VERSION: "3.9"
 
 jobs:
+  license_check:
+    name: Check missing license headers
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Check license header
+        uses: apache/skywalking-eyes/header@v0.6.0
+        with:
+          config: .licenserc.yml
+
   pylint:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
+
       - uses: ./.github/actions/python_build
         with:
           tags: "[cicd]"
 
       - name: Run pylint
         run: |
           pylint --rcfile pyproject.toml src/ensembl
           pylint --rcfile pyproject.toml tests
 
   mypy:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
+
       - uses: ./.github/actions/python_build
         with:
           tags: "[cicd]"
 
       - name: Run mypy
         run: |
           mypy --config-file pyproject.toml src/ensembl
           mypy --config-file pyproject.toml tests
 
   black:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
+
       - uses: ./.github/actions/python_build
         with:
           tags: "[cicd]"
 
       - name: Run black
         run: |
           black --config pyproject.toml --check .
 
-  pytest_and_docs:
+  pytest:
+    name: Run pytest and generate coverage reports
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
+      checks: write
+      pull-requests: write
 
     steps:
       - uses: actions/checkout@v4
+
       - uses: ./.github/actions/python_build
         with:
-          tags: "[cicd,docs]"
+          tags: "[cicd]"
 
       - name: Run pytest with coverage
         run: |
           coverage run -m pytest --junitxml=./reports/test-results-${{ env.PYTHON_VERSION }}.xml
           coverage xml -o ./reports/coverage.xml
           coverage report -m
 
       - name: Add coverage reports
         if: ${{ github.event_name == 'pull_request' }}
         uses: MishaKav/pytest-coverage-comment@main
         with:
           pytest-xml-coverage-path: ./reports/coverage.xml
           junitxml-path: ./reports/test-results-${{ env.PYTHON_VERSION }}.xml
-
-      - name: Deploy documentation to GitHub Pages
-        if: ${{ github.event_name == 'push' && github.ref_name == 'main' }}
-        run: |
-          coverage html -d ./reports/htmlcov
-          genbadge coverage -i ./reports/coverage.xml -o ./reports/htmlcov/coverage-badge.svg
-          mkdocs gh-deploy --force
```

### Comparing `ensembl_utils-0.1.2/.github/workflows/publish.yml` & `ensembl_utils-0.1.3/.github/workflows/publish.yml`

 * *Files 25% similar despite different names*

```diff
@@ -23,25 +23,50 @@
   run:
     working-directory: ./
 
 env:
   PYTHON_VERSION: "3.9"
 
 jobs:
+  mkdocs:
+    name: Deploy documentation to GitHub Pages
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+
+    steps:
+      - uses: actions/checkout@v4
+
+      - uses: ./.github/actions/python_build
+        with:
+          tags: "[cicd,docs]"
+
+      - name: Generate coverage report
+        run: |
+          coverage run -m pytest
+          coverage html -d ./reports/htmlcov
+          coverage xml -o ./reports/coverage.xml
+          genbadge coverage -i ./reports/coverage.xml -o ./reports/htmlcov/coverage-badge.svg
+
+      - name: Run mkdocs
+        run: |
+          mkdocs gh-deploy --force
+
   pypi-publish:
     name: Publish release to PyPI
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/ensembl-utils
     permissions:
       id-token: write
 
     steps:
       - uses: actions/checkout@v4
+
       - uses: ./.github/actions/python_build
         with:
             tags: "[build]"
 
       - name: Build package
         run: |
           python -m build
```

### Comparing `ensembl_utils-0.1.2/.gitignore` & `ensembl_utils-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/LICENSE` & `ensembl_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/PKG-INFO` & `ensembl_utils-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ensembl-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ensembl Python general-purpose utils
 Author-email: Ensembl <dev@ensembl.org>
 License: Apache License 2.0
-Project-URL: homepage, https://www.ensembl.org
-Project-URL: documentation, https://ensembl.github.io/ensembl-utils/
-Project-URL: repository, https://github.com/Ensembl/ensembl-utils
+Project-URL: Homepage, https://www.ensembl.org
+Project-URL: Documentation, https://ensembl.github.io/ensembl-utils/
+Project-URL: Repository, https://github.com/Ensembl/ensembl-utils
 Keywords: ensembl,python,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
@@ -62,22 +62,11 @@
 
 For more information, please consult this repository's [GitHub pages](https://ensembl.github.io/ensembl-utils/).
 
 ## Getting Started
 
 ### Basic installation
 
-This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management tool, e.g.
 ```bash
 pip install ensembl-utils
 ```
-
-### Installing the development environment (with Python `venv`)
-
-If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
-```bash
-python -m venv <VIRTUAL_ENVIRONMENT_NAME>
-source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
-git clone https://github.com/Ensembl/ensembl-utils.git
-cd ensembl-utils
-pip install -e .[cicd,docs]
-```
```

### Comparing `ensembl_utils-0.1.2/README.md` & `ensembl_utils-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,11 @@
 
 For more information, please consult this repository's [GitHub pages](https://ensembl.github.io/ensembl-utils/).
 
 ## Getting Started
 
 ### Basic installation
 
-This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management tool, e.g.
 ```bash
 pip install ensembl-utils
 ```
-
-### Installing the development environment (with Python `venv`)
-
-If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
-```bash
-python -m venv <VIRTUAL_ENVIRONMENT_NAME>
-source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
-git clone https://github.com/Ensembl/ensembl-utils.git
-cd ensembl-utils
-pip install -e .[cicd,docs]
-```
```

### Comparing `ensembl_utils-0.1.2/docs/gen_ref_pages.py` & `ensembl_utils-0.1.3/docs/scripts/gen_ref_pages.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,31 @@
 from pathlib import Path
 
 import mkdocs_gen_files
 
 
 nav = mkdocs_gen_files.Nav()
 
-root = Path("src/ensembl")
-num_parents = len(root.parents) - 1
+root = Path("src").resolve()
 for py_path in sorted(root.rglob("*.py")):
-    # Get the relative module path
+    # Get the relative module path and corresponding documentation paths
     module_path = py_path.relative_to(root)
     doc_path = module_path.with_suffix(".md")
     full_doc_path = Path("reference", doc_path)
-    # Drop all the parents of the namespace from the path components as well as ".py" extension
-    parts = py_path.parts[num_parents:-1] + (py_path.stem,)
-    # Drop "__init__.py" file from the path components as well (if present)
+    # Get all the parts of the module path without the ".py" extension
+    parts = tuple(module_path.with_suffix("").parts)
+    # Drop "__init__" file from the path components as well (if present)
     if parts[-1] == "__init__":
         parts = parts[:-1]
         doc_path = doc_path.with_name("index.md")
         full_doc_path = full_doc_path.with_name("index.md")
     # Add markdown file path with its index tree
     nav[parts] = doc_path.as_posix()
-    # Populate the markdown file with the doc stub of this Python module
-    with mkdocs_gen_files.open(full_doc_path, "a") as fd:
+    # Populate the markdown file with the doc stub of this module
+    with mkdocs_gen_files.open(full_doc_path, "w") as fd:
         identifier = ".".join(parts)
         fd.write(f"::: {identifier}\n")
     # Correct the path
-    mkdocs_gen_files.set_edit_path(full_doc_path, Path("../") / py_path)
+    mkdocs_gen_files.set_edit_path(full_doc_path, module_path)
 
 with mkdocs_gen_files.open("reference/summary.md", "w") as nav_file:
     nav_file.writelines(nav.build_literate_nav())
```

### Comparing `ensembl_utils-0.1.2/docs/img/ebang.png` & `ensembl_utils-0.1.3/docs/img/ebang.png`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/docs/index.md` & `ensembl_utils-0.1.3/docs/index.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,10 +2,13 @@
 
 Centralise generic Python utils used by other project within Ensembl design to facilitate frequent tasks such as input file path checks, archive files IO manipulation or logging setup, among others.
 
 ## Contents
 Check out [installation](install.md) section for further information on how to install the project.
 
 1. [Install](install.md)
+2. [Code of Conduct](code_of_conduct.md)
+3. [Coverage report](coverage.md)
+4. [Code reference](reference/)
 
 ## License
 Software as part of [Ensembl Python general-purpose utils](https://github.com/Ensembl/ensembl-utils) is distributed under the [Apache-2.0 License](https://www.apache.org/licenses/LICENSE-2.0.txt).
```

### Comparing `ensembl_utils-0.1.2/docs/install.md` & `ensembl_utils-0.1.3/docs/install.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # How to install this repository
 
 This Python library only requires Python 3.9+ to work.
 
 ## Basic installation
 
-This library is publicly available in [pypi.org](https://pypi.org) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management tool, e.g.
 ```bash
 pip install ensembl-utils
 ```
 
 ## Development-oriented installation
 
 If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
```

### Comparing `ensembl_utils-0.1.2/mkdocs.yml` & `ensembl_utils-0.1.3/mkdocs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -41,26 +41,27 @@
   - toc:
       permalink: true
 
 plugins:
 - search
 - gen-files:
      scripts:
-     - docs/gen_ref_pages.py
+     - docs/scripts/gen_ref_pages.py
 - literate-nav:
     nav_file: summary.md
 - section-index
 - mkdocstrings:
     enabled: !ENV [ENABLE_MKDOCSTRINGS, true]
     default_handler: python
     handlers:
       python:
+        paths: [src]
         options:
-          inherited_members: true
-          members: true
+          filters: ["!^_"]
+          show_if_no_docstring: true
           show_root_heading: true
           show_source: true
           show_symbol_type_heading: true
           show_symbol_type_toc: true
 - coverage:
     page_name: coverage
     html_report_dir: reports/htmlcov
```

#### html2text {}

```diff
@@ -11,15 +11,16 @@
 github.com/Ensembl/ensembl-utils" repo_name: "Ensembl/ensembl-utils" copyright:
 "Copyright © [2016-
 ] EMBL-European Bioinformatics Institute" theme: name: "material" logo: img/
 ebang.png icon: repo: fontawesome/brands/github palette: scheme: ensembl
 features: - content.tooltips - navigation.expand - navigation.tabs -
 navigation.tabs.sticky - navigation.top - search.highlight - search.suggest -
 toc.follow extra_css: - stylesheets/extra.css markdown_extensions: - toc:
-permalink: true plugins: - search - gen-files: scripts: - docs/gen_ref_pages.py
-- literate-nav: nav_file: summary.md - section-index - mkdocstrings: enabled:
-!ENV [ENABLE_MKDOCSTRINGS, true] default_handler: python handlers: python:
-options: inherited_members: true members: true show_root_heading: true
-show_source: true show_symbol_type_heading: true show_symbol_type_toc: true -
-coverage: page_name: coverage html_report_dir: reports/htmlcov nav: - Home: -
-Overview: index.md - Install: install.md - Development: - Code of Conduct:
-code_of_conduct.md - Coverage report: coverage.md - Code reference: reference/
+permalink: true plugins: - search - gen-files: scripts: - docs/scripts/
+gen_ref_pages.py - literate-nav: nav_file: summary.md - section-index -
+mkdocstrings: enabled: !ENV [ENABLE_MKDOCSTRINGS, true] default_handler: python
+handlers: python: paths: [src] options: filters: ["!^_"] show_if_no_docstring:
+true show_root_heading: true show_source: true show_symbol_type_heading: true
+show_symbol_type_toc: true - coverage: page_name: coverage html_report_dir:
+reports/htmlcov nav: - Home: - Overview: index.md - Install: install.md -
+Development: - Code of Conduct: code_of_conduct.md - Coverage report:
+coverage.md - Code reference: reference/
```

### Comparing `ensembl_utils-0.1.2/pyproject.toml` & `ensembl_utils-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,17 @@
     "mkdocs-material-extensions",
     "mkdocs-section-index",
     "mkdocstrings",
     "mkdocstrings-python",
 ]
 
 [project.urls]
-homepage = "https://www.ensembl.org"
-documentation = "https://ensembl.github.io/ensembl-utils/"
-repository = "https://github.com/Ensembl/ensembl-utils"
+Homepage = "https://www.ensembl.org"
+Documentation = "https://ensembl.github.io/ensembl-utils/"
+Repository = "https://github.com/Ensembl/ensembl-utils"
 
 [project.scripts]
 extract_file = "ensembl.utils.archive:extract_file_cli"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
```

### Comparing `ensembl_utils-0.1.2/setup.py` & `ensembl_utils-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/src/ensembl/utils/__init__.py` & `ensembl_utils-0.1.3/src/ensembl/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Ensembl Python general-purpose utils library."""
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 __all__ = [
     "StrPath",
 ]
 
 import os
 from typing import Union
```

### Comparing `ensembl_utils-0.1.2/src/ensembl/utils/archive.py` & `ensembl_utils-0.1.3/src/ensembl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/src/ensembl/utils/argparse.py` & `ensembl_utils-0.1.3/src/ensembl/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/src/ensembl/utils/logging.py` & `ensembl_utils-0.1.3/src/ensembl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/src/ensembl/utils/rloader.py` & `ensembl_utils-0.1.3/src/ensembl/utils/rloader.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/src/ensembl_utils.egg-info/PKG-INFO` & `ensembl_utils-0.1.3/src/ensembl_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ensembl-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ensembl Python general-purpose utils
 Author-email: Ensembl <dev@ensembl.org>
 License: Apache License 2.0
-Project-URL: homepage, https://www.ensembl.org
-Project-URL: documentation, https://ensembl.github.io/ensembl-utils/
-Project-URL: repository, https://github.com/Ensembl/ensembl-utils
+Project-URL: Homepage, https://www.ensembl.org
+Project-URL: Documentation, https://ensembl.github.io/ensembl-utils/
+Project-URL: Repository, https://github.com/Ensembl/ensembl-utils
 Keywords: ensembl,python,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
@@ -62,22 +62,11 @@
 
 For more information, please consult this repository's [GitHub pages](https://ensembl.github.io/ensembl-utils/).
 
 ## Getting Started
 
 ### Basic installation
 
-This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management, e.g.
+This library is publicly available in [PyPI](https://pypi.org/project/ensembl-utils/) so it can be easily installed with your favourite Python dependency and packaging management tool, e.g.
 ```bash
 pip install ensembl-utils
 ```
-
-### Installing the development environment (with Python `venv`)
-
-If you want to install this library in editable mode, we suggest you to do so via Python's virtual environment module ([venv](https://docs.python.org/3/library/venv.html)):
-```bash
-python -m venv <VIRTUAL_ENVIRONMENT_NAME>
-source <VIRTUAL_ENVIRONMENT_NAME>/bin/activate
-git clone https://github.com/Ensembl/ensembl-utils.git
-cd ensembl-utils
-pip install -e .[cicd,docs]
-```
```

### Comparing `ensembl_utils-0.1.2/src/ensembl_utils.egg-info/SOURCES.txt` & `ensembl_utils-0.1.3/src/ensembl_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 .gitignore
+.licenserc.yml
 LICENSE
 NOTICE
 README.md
 mkdocs.yml
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/actions/python_build/action.yml
 .github/workflows/ci.yml
+.github/workflows/notice.yml
 .github/workflows/publish.yml
 docs/code_of_conduct.md
-docs/gen_ref_pages.py
 docs/index.md
 docs/install.md
 docs/img/ebang.png
+docs/scripts/gen_ref_pages.py
 docs/stylesheets/extra.css
 src/ensembl/utils/__init__.py
 src/ensembl/utils/archive.py
 src/ensembl/utils/argparse.py
 src/ensembl/utils/logging.py
 src/ensembl/utils/rloader.py
 src/ensembl_utils.egg-info/PKG-INFO
```

### Comparing `ensembl_utils-0.1.2/tests/archive/test_archive/sample.tar` & `ensembl_utils-0.1.3/tests/archive/test_archive/sample.tar`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/tests/archive/test_archive.py` & `ensembl_utils-0.1.3/tests/archive/test_archive.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/tests/argparse/test_argparse.py` & `ensembl_utils-0.1.3/tests/argparse/test_argparse.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/tests/conftest.py` & `ensembl_utils-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/tests/logging/test_logging.py` & `ensembl_utils-0.1.3/tests/logging/test_logging.py`

 * *Files identical despite different names*

### Comparing `ensembl_utils-0.1.2/tests/rloader/test_rloader.py` & `ensembl_utils-0.1.3/tests/rloader/test_rloader.py`

 * *Files identical despite different names*

