# Comparing `tmp/opera-utils-0.3.0.tar.gz` & `tmp/opera_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opera-utils-0.3.0.tar", last modified: Wed Feb 14 00:52:30 2024, max compression
+gzip compressed data, was "opera_utils-0.3.1.tar", last modified: Wed May 29 17:30:35 2024, max compression
```

## Comparing `opera-utils-0.3.0.tar` & `opera_utils-0.3.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.504990 opera-utils-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.492990 opera-utils-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.492990 opera-utils-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-14 00:52:16.000000 opera-utils-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-14 00:52:16.000000 opera-utils-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-02-14 00:52:16.000000 opera-utils-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-02-14 00:52:30.500990 opera-utils-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-14 00:52:16.000000 opera-utils-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.496990 opera-utils-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/background-theory.md
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/how-to-guides.md
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-14 00:52:16.000000 opera-utils-0.3.0/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-14 00:52:16.000000 opera-utils-0.3.0/environment-geo.yml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-14 00:52:16.000000 opera-utils-0.3.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-14 00:52:16.000000 opera-utils-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-14 00:52:16.000000 opera-utils-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-14 00:52:16.000000 opera-utils-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 00:52:30.504990 opera-utils-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.492990 opera-utils-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.496990 opera-utils-0.3.0/src/opera_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/_gslc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/burst_frame_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/bursts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/h5explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-02-14 00:52:16.000000 opera-utils-0.3.0/src/opera_utils/stitching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.500990 opera-utils-0.3.0/src/opera_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-14 00:52:30.000000 opera-utils-0.3.0/src/opera_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.500990 opera-utils-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.492990 opera-utils-0.3.0/tests/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.500990 opera-utils-0.3.0/tests/cassettes/test_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    26752 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/cassettes/test_datasets/test_registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:52:30.500990 opera-utils-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/data/idaho_slc_file_list.txt.zip
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_bursts.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_h5explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_missing_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-14 00:52:16.000000 opera-utils-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.383798 opera_utils-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.375798 opera_utils-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.375798 opera_utils-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-29 17:30:22.000000 opera_utils-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-29 17:30:22.000000 opera_utils-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-29 17:30:22.000000 opera_utils-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-29 17:30:35.383798 opera_utils-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-29 17:30:22.000000 opera_utils-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.375798 opera_utils-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/background-theory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/how-to-guides.md
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-29 17:30:22.000000 opera_utils-0.3.1/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 17:30:22.000000 opera_utils-0.3.1/environment-geo.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-29 17:30:22.000000 opera_utils-0.3.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-29 17:30:22.000000 opera_utils-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-29 17:30:22.000000 opera_utils-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 17:30:22.000000 opera_utils-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:30:35.383798 opera_utils-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.371798 opera_utils-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.379798 opera_utils-0.3.1/src/opera_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/_gslc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/burst_frame_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/bursts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/h5explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/missing_data_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-05-29 17:30:22.000000 opera_utils-0.3.1/src/opera_utils/stitching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.379798 opera_utils-0.3.1/src/opera_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 17:30:35.000000 opera_utils-0.3.1/src/opera_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.379798 opera_utils-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.371798 opera_utils-0.3.1/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.379798 opera_utils-0.3.1/tests/cassettes/test_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    26752 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/cassettes/test_datasets/test_registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:30:35.379798 opera_utils-0.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/data/idaho_slc_file_list.txt.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_bursts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_h5explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-29 17:30:22.000000 opera_utils-0.3.1/tests/test_utils.py
```

### Comparing `opera-utils-0.3.0/.github/workflows/cd.yml` & `opera_utils-0.3.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/.github/workflows/ci.yml` & `opera_utils-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/.gitignore` & `opera_utils-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/.pre-commit-config.yaml` & `opera_utils-0.3.1/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       - id: end-of-file-fixer
       - id: file-contents-sorter
         files: (requirements.txt)$
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1
+    rev: v0.2.2
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
         types_or: [python, jupyter]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
```

### Comparing `opera-utils-0.3.0/.readthedocs.yaml` & `opera_utils-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/CHANGELOG.md` & `opera_utils-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/LICENSE` & `opera_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/PKG-INFO` & `opera_utils-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opera-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Miscellaneous utilities for working with OPERA data products
 Author-email: Scott Staniewicz <scott.j.staniewicz@jpl.nasa.gov>
 Project-URL: Homepage, https://github.com/opera-adt/opera-utils
 Project-URL: Bug Tracker, https://github.com/opera-adt/opera-utils/issues
 Project-URL: Discussions, https://github.com/opera-adt/opera-utils/discussions
 Project-URL: Changelog, https://github.com/opera-adt/opera-utils/releases
 Classifier: Intended Audience :: Developers
```

### Comparing `opera-utils-0.3.0/README.md` & `opera_utils-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/docs/gen_ref_pages.py` & `opera_utils-0.3.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/docs/getting-started.md` & `opera_utils-0.3.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/docs/tutorials.md` & `opera_utils-0.3.1/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/mkdocs.yml` & `opera_utils-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/pyproject.toml` & `opera_utils-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/_dates.py` & `opera_utils-0.3.1/src/opera_utils/_dates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import datetime
 import itertools
+import operator
 import re
 from collections import defaultdict
 from typing import Iterable, overload
 
 from ._types import DateOrDatetime, Filename, PathLikeT
 from ._utils import _get_path_from_gdal_str
 
@@ -219,25 +220,16 @@
     Returns
     -------
     file_list : list[Filename]
         list of files sorted by date.
     dates : list[list[datetime.date,...]]
         Sorted list, where each entry has all the dates from the corresponding file.
     """
-
-    def sort_key(file_date_tuple):
-        # Key for sorting:
-        # To sort the files with the most dates first (the compressed SLCs which
-        # span a date range), sort the longer date lists first.
-        # Then, within each group of dates of the same length, use the date/dates
-        _, dates = file_date_tuple
-        try:
-            return (-len(dates), dates)
-        except TypeError:
-            return (-1, dates)
-
     file_date_tuples = [(f, get_dates(f, fmt=file_date_fmt)) for f in files]
-    file_dates = sorted([fd_tuple for fd_tuple in file_date_tuples], key=sort_key)
+    # Get the second item in the tuple for the key
+    file_dates = sorted(
+        [fd_tuple for fd_tuple in file_date_tuples], key=operator.itemgetter(1)
+    )
 
     # Unpack the sorted pairs with new sorted values
     file_list, dates = zip(*file_dates)  # type: ignore
     return list(file_list), list(dates)
```

### Comparing `opera-utils-0.3.0/src/opera_utils/_gslc.py` & `opera_utils-0.3.1/src/opera_utils/_gslc.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/_helpers.py` & `opera_utils-0.3.1/src/opera_utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/_io.py` & `opera_utils-0.3.1/src/opera_utils/_io.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/_types.py` & `opera_utils-0.3.1/src/opera_utils/_types.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/_utils.py` & `opera_utils-0.3.1/src/opera_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/burst_frame_db.py` & `opera_utils-0.3.1/src/opera_utils/burst_frame_db.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/bursts.py` & `opera_utils-0.3.1/src/opera_utils/bursts.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/cli.py` & `opera_utils-0.3.1/src/opera_utils/cli.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/constants.py` & `opera_utils-0.3.1/src/opera_utils/constants.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/datasets.py` & `opera_utils-0.3.1/src/opera_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/download.py` & `opera_utils-0.3.1/src/opera_utils/download.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/geometry.py` & `opera_utils-0.3.1/src/opera_utils/geometry.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,31 +55,31 @@
     burst_ids : Sequence[str] | None, optional
         Alternative to `frame_id`, manually specify CSLC burst IDs.
     output_dir : PathOrStr, optional
         Directory to store output geotiffs, by default Path(".")
     download_dir : PathOrStr | None, optional
         Directory to save files, by default None
     save_hdf5_files : bool, optional
-        _description_, by default False
-    layers : Sequence[Layer  |  str], optional
-        _description_, by default DEFAULT_LAYERS
+        Flag to retain HDF5 files. Defaults to False.
+    layers : Sequence[Layer | str], optional
+        Layers to process. Defaults to DEFAULT_LAYERS.
     strides : Mapping[str, int], optional
-        _description_, by default DEFAULT_STRIDES
+        Stride values for merging images. Defaults to DEFAULT_STRIDES.
     max_download_jobs : int, optional
-        _description_, by default 3
+        Maximum number of download jobs to run in parallel. Defaults to 3.
 
     Returns
     -------
     list[Path]
-        _description_
+        List of output files with paths.
 
     Raises
     ------
     ValueError
-        _description_
+        If neither `frame_id` nor `burst_ids` are provided.
     """
     if frame_id is not None:
         burst_ids = get_burst_ids_for_frame(frame_id=frame_id)
 
     if not burst_ids:
         raise ValueError("Must provide frame_id or burst_ids")
 
@@ -89,29 +89,64 @@
         download_dir = output_path / "hdf5"
     output_files: list[Path] = []
 
     with scratch_directory(download_dir, delete=not save_hdf5_files) as sd:
         local_hdf5_files = download_cslc_static_layers(
             burst_ids=burst_ids, output_dir=sd, max_jobs=max_download_jobs
         )
-        for layer in layers:
-            layer_enum = Layer(layer)
-            name = layer_enum.value
-            gdal_strings = [
-                format_nc_filename(f, ds_name=f"data/{name}") for f in local_hdf5_files
-            ]
-            nodata = LAYER_TO_NODATA[Layer(layer)]
-            cur_outfile = output_path / f"{name}.tif"
-            output_files.append(cur_outfile)
-            logger.info(f"Merging images for {name}")
-            stitching.merge_images(
-                file_list=gdal_strings,
-                outfile=cur_outfile,
-                strides=strides,
-                driver="GTIff",
-                options=EXTRA_COMPRESSED_TIFF_OPTIONS,
-                resample_alg="nearest",
-                in_nodata=nodata,
-                out_nodata=nodata,
-            )
+        output_files = stitch_geometry_layers(
+            local_hdf5_files=local_hdf5_files,
+            layers=layers,
+            strides=strides,
+            output_dir=output_path,
+        )
+
+    return output_files
+
+
+def stitch_geometry_layers(
+    local_hdf5_files: list[Path],
+    layers: Sequence[Layer | str] = DEFAULT_LAYERS,
+    strides: Mapping[str, int] = DEFAULT_STRIDES,
+    output_dir: PathOrStr = Path("."),
+) -> list[Path]:
+    """Stitch geometry layers from downloaded HDF5 files.
+
+    Parameters
+    ----------
+    local_hdf5_files : list[Path]
+        List of paths to the downloaded HDF5 files.
+    layers : Sequence[Layer | str]
+        Layers to be processed.
+    strides : Mapping[str, int]
+        Stride values for merging images.
+    output_dir : PathOrStr
+        Directory to store output Geotiffs.
+
+    Returns
+    -------
+    list[Path]
+        List of output files with paths.
+    """
+    output_files: list[Path] = []
 
+    for layer in layers:
+        layer_enum = Layer(layer)
+        name = layer_enum.value
+        gdal_strings = [
+            format_nc_filename(f, ds_name=f"data/{name}") for f in local_hdf5_files
+        ]
+        nodata = LAYER_TO_NODATA[Layer(layer)]
+        cur_outfile = Path(output_dir) / f"{name}.tif"
+        output_files.append(cur_outfile)
+        logger.info(f"Merging images for {name}")
+        stitching.merge_images(
+            file_list=gdal_strings,
+            outfile=cur_outfile,
+            strides=strides,
+            driver="GTIff",
+            options=EXTRA_COMPRESSED_TIFF_OPTIONS,
+            resample_alg="nearest",
+            in_nodata=nodata,
+            out_nodata=nodata,
+        )
     return output_files
```

### Comparing `opera-utils-0.3.0/src/opera_utils/h5explorer.py` & `opera_utils-0.3.1/src/opera_utils/h5explorer.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils/missing_data.py` & `opera_utils-0.3.1/src/opera_utils/missing_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
-from datetime import date
+from datetime import datetime
 from itertools import groupby
 from typing import Iterable, Mapping, Optional, Sequence
 
 import numpy as np
 
 from ._dates import get_dates
 from ._helpers import flatten, powerset, sorted_deduped_values
@@ -27,63 +27,75 @@
 class BurstSubsetOption:
     """Dataclass for a possible subset of SLC data."""
 
     total_num_bursts: int
     """Total number of bursts used in this subset."""
     burst_ids: tuple[str, ...]
     """Burst IDs used in this subset."""
-    dates: tuple[date, ...]
+    dates: tuple[datetime, ...]
     """Dates used in this subset."""
     # subset_selected: list[bool]
     num_candidate_bursts: int
-    """The number of (burst_id, date) pairs that were passed as options."""
+    """The number of (burst_id, datetime) pairs that were passed as options."""
 
     @property
     def num_dates(self) -> int:
         return len(self.dates)
 
     @property
     def num_burst_ids(self) -> int:
         return len(self.burst_ids)
 
 
 def get_burst_id_to_dates(
     slc_files: Optional[Iterable[Filename]] = None,
-    burst_id_date_tuples: Optional[Iterable[tuple[str, date]]] = None,
-) -> dict[str, list[date]]:
+    burst_id_date_tuples: Optional[Iterable[tuple[str, datetime]]] = None,
+) -> dict[str, list[datetime]]:
     """Get a mapping of burst ID to list of dates.
 
-    Assumes that the `slc_files` have only one date in the name, or
-    that the first date in the `burst_id_date_tuples` is the relevant
+    Assumes that the `slc_files` have only one datetime in the name, or
+    that the first datetime in the `burst_id_date_tuples` is the relevant
     one (as is the case for OPERA CSLCs).
 
 
     Parameters
     ----------
     slc_files : Optional[Iterable[Filename]]
         List of OPERA CSLC filenames.
-    burst_id_date_tuples : Optional[Iterable[tuple[str, date]]]
-        Alternative input: list of all existing (burst_id, date) tuples.
+    burst_id_date_tuples : Optional[Iterable[tuple[str, datetime]]]
+        Alternative input: list of all existing (burst_id, datetime) tuples.
 
     Returns
     -------
-    dict[str, list[date]]
+    dict[str, list[datetime]]
         Mapping of burst ID to list of dates.
     """
     if slc_files is not None:
         return _burst_id_mapping_from_files(slc_files)
     elif burst_id_date_tuples is not None:
         return _burst_id_mapping_from_tuples(burst_id_date_tuples)
     else:
         raise ValueError("Must provide either slc_files or burst_id_date_tuples")
 
 
+def _duplicated_bursts(burst_id_to_dates: Mapping[str, Sequence[datetime]]):
+    from collections import Counter
+
+    counts: Counter = Counter()
+    for burst_id, d_list in burst_id_to_dates.items():
+        for d in d_list:
+            counts[(burst_id, d)] += 1
+    # total_sum = sum([len(v) for k, v in burst_id_to_dates.items()])
+    # deduped_sum = sum([len(set(v)) for k, v in burst_id_to_dates.items()])
+    return [pair for pair, count in counts.items() if count > 1]
+
+
 def get_missing_data_options(
     slc_files: Optional[Iterable[Filename]] = None,
-    burst_id_date_tuples: Optional[Iterable[tuple[str, date]]] = None,
+    burst_id_date_tuples: Optional[Iterable[tuple[str, datetime]]] = None,
 ) -> list[BurstSubsetOption]:
     """Get a list of possible data subsets for a set of burst SLCs.
 
     The default optimization criteria for choosing among these subsets is
 
         maximize        total number of bursts used
         subject to      dates used for each burst ID are all equal
@@ -92,54 +104,59 @@
     avoid spatial discontinuities the estimated displacement/velocity,
     which can occur if different dates are used for different burst IDs.
 
     Parameters
     ----------
     slc_files : Optional[Iterable[Filename]]
         list of OPERA CSLC filenames.
-    burst_id_date_tuples : Optional[Iterable[tuple[str, date]]]
-        Alternative input: list of all existing (burst_id, date) tuples.
+    burst_id_date_tuples : Optional[Iterable[tuple[str, datetime]]]
+        Alternative input: list of all existing (burst_id, datetime) tuples.
 
     Returns
     -------
     list[BurstSubsetOption]
         List of possible subsets of the given SLC data.
         The options will be sorted by the total number of bursts used, so
         that the first option is the one that uses the most data.
     """
     burst_id_to_dates = get_burst_id_to_dates(
         slc_files=slc_files, burst_id_date_tuples=burst_id_date_tuples
     )
+    dupes = _duplicated_bursts(burst_id_to_dates)
+    if dupes:
+        s = "\n".join(f'{b}_{d.strftime("%Y%m%d")}' for (b, d) in dupes)
+        msg = f"Duplicated (burst_id, datetime) pairs passed:\n{s}."
+        raise ValueError(msg)
 
     all_burst_ids = list(burst_id_to_dates.keys())
     all_dates = sorted_deduped_values(burst_id_to_dates)
 
     B = get_burst_id_date_incidence(burst_id_to_dates)
     # In this matrix,
     # - Each row corresponds to one of the possible burst IDs
     # - Each column corresponds to one of the possible dates
     return generate_burst_subset_options(B, all_burst_ids, all_dates)
 
 
 def get_burst_id_date_incidence(
-    burst_id_to_dates: Mapping[str, list[date]],
+    burst_id_to_dates: Mapping[str, list[datetime]],
 ) -> np.ndarray:
-    """Create a matrix of burst ID vs. date incidence.
+    """Create a matrix of burst ID vs. datetime incidence.
 
     Parameters
     ----------
-    burst_id_to_dates : Mapping[str, list[date]]
+    burst_id_to_dates : Mapping[str, list[datetime]]
         Mapping of burst ID to list of dates.
 
     Returns
     -------
     np.ndarray[bool]
-        Matrix of burst ID vs. date incidence.
+        Matrix of burst ID vs. datetime incidence.
         Rows correspond to burst IDs, columns correspond to dates.
-        A value of True indicates that the burst ID was acquired on that date.
+        A value of True indicates that the burst ID was acquired on that datetime.
     """
     all_dates = sorted_deduped_values(burst_id_to_dates)
 
     # Construct the incidence matrix of dates vs. burst IDs
     burst_id_to_date_incidence = {}
     for burst_id, date_list in burst_id_to_dates.items():
         cur_incidences = np.zeros(len(all_dates), dtype=bool)
@@ -147,60 +164,60 @@
         cur_incidences[idxs] = True
         burst_id_to_date_incidence[burst_id] = cur_incidences
 
     return np.array(list(burst_id_to_date_incidence.values()))
 
 
 def _burst_id_mapping_from_tuples(
-    burst_id_date_tuples: Iterable[tuple[str, date]],
-) -> dict[str, list[date]]:
-    """Create a {burst_id -> [date,...]} (burst_id, date) tuples."""
+    burst_id_date_tuples: Iterable[tuple[str, datetime]],
+) -> dict[str, list[datetime]]:
+    """Create a {burst_id -> [datetime,...]} (burst_id, datetime) tuples."""
     # Don't exhaust the iterator for multiple groupings
     burst_id_date_tuples = list(burst_id_date_tuples)
 
-    # Group the possible SLC files by their date and by their Burst ID
+    # Group the possible SLC files by their datetime and by their Burst ID
     return {
-        burst_id: [date for burst_id, date in g]
+        burst_id: [d for burst_id, d in g]
         for burst_id, g in groupby(burst_id_date_tuples, key=lambda x: x[0])
     }
 
 
 def _burst_id_mapping_from_files(
     slc_files: Iterable[Filename],
-) -> dict[str, list[date]]:
-    """Create a {burst_id -> [date,...]} mapping from filenames."""
+) -> dict[str, list[datetime]]:
+    """Create a {burst_id -> [datetime,...]} mapping from filenames."""
     # Don't exhaust the iterator for multiple groupings
     slc_file_list = list(map(str, slc_files))
 
-    # Group the possible SLC files by their date and by their Burst ID
+    # Group the possible SLC files by their datetime and by their Burst ID
     burst_id_to_files = group_by_burst(slc_file_list)
 
     date_tuples = [get_dates(f) for f in slc_file_list]
     assert all(len(tup) == 1 for tup in date_tuples)
 
     return {
         burst_id: [get_dates(f)[0] for f in file_list]
         for (burst_id, file_list) in burst_id_to_files.items()
     }
 
 
 def generate_burst_subset_options(
-    B: np.ndarray, burst_ids: Sequence[str], dates: Sequence[date]
+    B: np.ndarray, burst_ids: Sequence[str], dates: Sequence[datetime]
 ) -> list[BurstSubsetOption]:
     """Generate possible valid subsets of the given SLC data.
 
     Parameters
     ----------
     B : NDArray[np.bool]
-        Matrix of burst ID vs. date incidence.
+        Matrix of burst ID vs. datetime incidence.
         Rows correspond to burst IDs, columns correspond to dates.
-        A value of True indicates that the burst ID was acquired on that date.
+        A value of True indicates that the burst ID was acquired on that datetime.
     burst_ids : Sequence[str]
         List of all burst IDs.
-    dates : Sequence[date]
+    dates : Sequence[datetime]
         List of all dates.
 
     Returns
     -------
     list[BurstSubsetOption]
         List of possible subsets of the given SLC data.
         The options will be sorted by the total number of bursts used, so
@@ -263,15 +280,15 @@
         # Check if all rows have the same pattern in the remaining columns
         if not (B_sub2.size > 0):
             logger.debug("No remaining entries in B_sub2")
             continue
         if not np.all(B_sub2 == B_sub2[[0]]):
             logger.debug("Not all rows have the same pattern in the remaining columns")
             continue
-        # Create a BurstSubsetOption if we have at least one burst and one date
+        # Create a BurstSubsetOption if we have at least one burst and one datetime
         assert np.all(B_sub2)
 
         selected_burst_ids = tuple(burst_ids[i] for i in valid_row_idxs)
         selected_dates = tuple(dates[i] for i in valid_col_idxs)
         total_num_bursts = B_sub2.sum()
         # breakpoint()
         options.append(
```

### Comparing `opera-utils-0.3.0/src/opera_utils/stitching.py` & `opera_utils-0.3.1/src/opera_utils/stitching.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/src/opera_utils.egg-info/PKG-INFO` & `opera_utils-0.3.1/src/opera_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opera-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Miscellaneous utilities for working with OPERA data products
 Author-email: Scott Staniewicz <scott.j.staniewicz@jpl.nasa.gov>
 Project-URL: Homepage, https://github.com/opera-adt/opera-utils
 Project-URL: Bug Tracker, https://github.com/opera-adt/opera-utils/issues
 Project-URL: Discussions, https://github.com/opera-adt/opera-utils/discussions
 Project-URL: Changelog, https://github.com/opera-adt/opera-utils/releases
 Classifier: Intended Audience :: Developers
```

### Comparing `opera-utils-0.3.0/src/opera_utils.egg-info/SOURCES.txt` & `opera_utils-0.3.1/src/opera_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/opera_utils/cli.py
 src/opera_utils/constants.py
 src/opera_utils/datasets.py
 src/opera_utils/download.py
 src/opera_utils/geometry.py
 src/opera_utils/h5explorer.py
 src/opera_utils/missing_data.py
+src/opera_utils/missing_data_plots.py
 src/opera_utils/py.typed
 src/opera_utils/stitching.py
 src/opera_utils.egg-info/PKG-INFO
 src/opera_utils.egg-info/SOURCES.txt
 src/opera_utils.egg-info/dependency_links.txt
 src/opera_utils.egg-info/entry_points.txt
 src/opera_utils.egg-info/requires.txt
```

### Comparing `opera-utils-0.3.0/tests/cassettes/test_datasets/test_registry.yaml` & `opera_utils-0.3.1/tests/cassettes/test_datasets/test_registry.yaml`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/tests/data/idaho_slc_file_list.txt.zip` & `opera_utils-0.3.1/tests/data/idaho_slc_file_list.txt.zip`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/tests/test_bursts.py` & `opera_utils-0.3.1/tests/test_bursts.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/tests/test_dates.py` & `opera_utils-0.3.1/tests/test_dates.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,40 +176,40 @@
         [datetime.datetime(2020, 3, 3), datetime.datetime(2022, 1, 1)],
     ]
     sorted_files, sorted_dates = _dates.sort_files_by_date(files)
     assert sorted_files == sorted(files)  # here lexicographic order is correct
     assert sorted_dates == sorted(dates)
 
 
-def test_sort_files_by_date_compressed_first():
-    # Check that compressed SLCs go first, then SLCs are sorted by date
+def test_sort_files_with_varying_date_lengths():
+    """Check we handle files with varying date lengths, looking at first date only."""
     unsorted_files = [
         "slc_20200101.tif",
         "slc_20210101.tif",
         "slc_20190101.tif",
         "compressed_20180101_20200101.tif",
-        "slc_20180101.tif",
-        "compressed_20200101_20210101.tif",
+        "slc_20180102.tif",
+        "compressed_20200102_20210101.tif",
     ]
     expected_dates = [
         [datetime.datetime(2018, 1, 1), datetime.datetime(2020, 1, 1)],
-        [datetime.datetime(2020, 1, 1), datetime.datetime(2021, 1, 1)],
-        [datetime.datetime(2018, 1, 1)],
+        [datetime.datetime(2018, 1, 2)],
         [datetime.datetime(2019, 1, 1)],
         [datetime.datetime(2020, 1, 1)],
+        [datetime.datetime(2020, 1, 2), datetime.datetime(2021, 1, 1)],
         [datetime.datetime(2021, 1, 1)],
     ]
 
     sorted_files, sorted_dates = _dates.sort_files_by_date(unsorted_files)
     assert sorted_files == [
         "compressed_20180101_20200101.tif",
-        "compressed_20200101_20210101.tif",
-        "slc_20180101.tif",
+        "slc_20180102.tif",
         "slc_20190101.tif",
         "slc_20200101.tif",
+        "compressed_20200102_20210101.tif",
         "slc_20210101.tif",
     ]
     assert sorted_dates == expected_dates
 
 
 def test_sort_by_date_different_fmt():
     # Check that it works with different date formats
```

### Comparing `opera-utils-0.3.0/tests/test_h5explorer.py` & `opera_utils-0.3.1/tests/test_h5explorer.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/tests/test_io.py` & `opera_utils-0.3.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/tests/test_missing_data.py` & `opera_utils-0.3.1/tests/test_missing_data.py`

 * *Files identical despite different names*

### Comparing `opera-utils-0.3.0/tests/test_utils.py` & `opera_utils-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

