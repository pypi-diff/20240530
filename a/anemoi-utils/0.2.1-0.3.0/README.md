# Comparing `tmp/anemoi_utils-0.2.1.tar.gz` & `tmp/anemoi_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_utils-0.2.1.tar", last modified: Tue May 28 10:05:54 2024, max compression
+gzip compressed data, was "anemoi_utils-0.3.0.tar", last modified: Thu May 30 18:50:29 2024, max compression
```

## Comparing `anemoi_utils-0.2.1.tar` & `anemoi_utils-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.158770 anemoi_utils-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.150770 anemoi_utils-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.150770 anemoi_utils-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-28 10:05:54.158770 anemoi_utils-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.154770 anemoi_utils-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.154770 anemoi_utils-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.154770 anemoi_utils-0.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.154770 anemoi_utils-0.2.1/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/checkpoints.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/humanize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/provenance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/modules/text.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 10:05:54.158770 anemoi_utils-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.150770 anemoi_utils-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.150770 anemoi_utils-0.2.1/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.154770 anemoi_utils-0.2.1/src/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi/utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.154770 anemoi_utils-0.2.1/src/anemoi/utils/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/commands/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/humanize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.158770 anemoi_utils-0.2.1/src/anemoi/utils/mars/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/mars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/mars/mars.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/src/anemoi/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.158770 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 10:05:54.000000 anemoi_utils-0.2.1/src/anemoi_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:05:54.158770 anemoi_utils-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-28 10:05:44.000000 anemoi_utils-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.341353 anemoi_utils-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.329353 anemoi_utils-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-30 18:50:29.341353 anemoi_utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/checkpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/humanize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/modules/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:50:29.341353 anemoi_utils-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.333353 anemoi_utils-0.3.0/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.337353 anemoi_utils-0.3.0/src/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.337353 anemoi_utils-0.3.0/src/anemoi/utils/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/commands/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/humanize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.337353 anemoi_utils-0.3.0/src/anemoi/utils/mars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/mars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/mars/mars.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/src/anemoi/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.341353 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 18:50:29.000000 anemoi_utils-0.3.0/src/anemoi_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:50:29.337353 anemoi_utils-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-30 18:50:19.000000 anemoi_utils-0.3.0/tests/test_utils.py
```

### Comparing `anemoi_utils-0.2.1/.github/workflows/python-publish.yml` & `anemoi_utils-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/.gitignore` & `anemoi_utils-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/.pre-commit-config.yaml` & `anemoi_utils-0.3.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -9,27 +9,27 @@
       stages: [commit]
       language: python
       entry: jupyter nbconvert --ClearOutputPreprocessor.enabled=True --inplace
       additional_dependencies: [jupyter]
 
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.6.0
   hooks:
   - id: check-yaml # Check YAML files for syntax errors only
     args: [--unsafe, --allow-multiple-documents]
   - id: debug-statements # Check for debugger imports and py37+ breakpoint()
   - id: end-of-file-fixer # Ensure files end in a newline
   - id: trailing-whitespace # Trailing whitespace checker
   - id: no-commit-to-branch # Prevent committing to main / master
   - id: check-added-large-files # Check for large files added to git
   - id: check-merge-conflict # Check for files that contain merge conflict
 
 - repo: https://github.com/psf/black-pre-commit-mirror
-  rev: 24.1.1
+  rev: 24.4.2
   hooks:
     - id: black
       args: [--line-length=120]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.13.2
   hooks:
@@ -37,15 +37,15 @@
     args:
     - -l 120
     - --force-single-line-imports
     - --profile black
 
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.3.0
+  rev: v0.4.6
   hooks:
   - id: ruff
     exclude: '(dev/.*|.*_)\.py$'
     args:
     - --line-length=120
     - --fix
     - --exit-non-zero-on-fix
@@ -64,7 +64,18 @@
       exclude: 'cli/.*' # Because we use argparse
 
 - repo: https://github.com/b8raoult/pre-commit-docconvert
   rev: "0.1.4"
   hooks:
   - id: docconvert
     args: ["numpy"]
+
+- repo: https://github.com/b8raoult/optional-dependencies-all
+  rev: "0.0.2"
+  hooks:
+  - id: optional-dependencies-all
+    args: ["--inplace", "--all-key", "all", "--exclude-keys", "dev,docs"]
+
+- repo: https://github.com/tox-dev/pyproject-fmt
+  rev: "2.1.3"
+  hooks:
+    - id: pyproject-fmt
```

### Comparing `anemoi_utils-0.2.1/LICENSE` & `anemoi_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/PKG-INFO` & `anemoi_utils-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.2.1
+Version: 0.3.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,55 +201,58 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://github.com/ecmwf/anemoi-utils/
 Project-URL: Documentation, https://anemoi-utils.readthedocs.io/
-Project-URL: Repository, https://github.com/ecmwf/anemoi-utils/
+Project-URL: Homepage, https://github.com/ecmwf/anemoi-utils/
 Project-URL: Issues, https://github.com/ecmwf/anemoi-utils/issues
-Keywords: tools,ai
+Project-URL: Repository, https://github.com/ecmwf/anemoi-utils/
+Keywords: ai,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: tomli
 Requires-Dist: pyyaml
+Requires-Dist: tomli
 Requires-Dist: tqdm
-Provides-Extra: provenance
-Requires-Dist: GitPython; extra == "provenance"
-Requires-Dist: nvsmi; extra == "provenance"
-Provides-Extra: text
-Requires-Dist: termcolor; extra == "text"
-Provides-Extra: grib
-Requires-Dist: requests; extra == "grib"
-Provides-Extra: docs
-Requires-Dist: tomli; extra == "docs"
-Requires-Dist: termcolor; extra == "docs"
-Requires-Dist: requests; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: pandoc; extra == "docs"
-Requires-Dist: sphinx_argparse; extra == "docs"
 Provides-Extra: all
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: GitPython; extra == "all"
+Requires-Dist: gitpython; extra == "all"
 Requires-Dist: nvsmi; extra == "all"
-Requires-Dist: termcolor; extra == "all"
+Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: requests; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: tomli; extra == "all"
+Requires-Dist: tqdm; extra == "all"
 Provides-Extra: dev
-Requires-Dist: tomli; extra == "dev"
-Requires-Dist: GitPython; extra == "dev"
+Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: nvsmi; extra == "dev"
-Requires-Dist: termcolor; extra == "dev"
 Requires-Dist: requests; extra == "dev"
+Requires-Dist: termcolor; extra == "dev"
+Requires-Dist: tomli; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: requests; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-argparse; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: termcolor; extra == "docs"
+Requires-Dist: tomli; extra == "docs"
+Provides-Extra: grib
+Requires-Dist: requests; extra == "grib"
+Provides-Extra: provenance
+Requires-Dist: gitpython; extra == "provenance"
+Requires-Dist: nvsmi; extra == "provenance"
+Provides-Extra: text
+Requires-Dist: termcolor; extra == "text"
```

### Comparing `anemoi_utils-0.2.1/README.md` & `anemoi_utils-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/docs/Makefile` & `anemoi_utils-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/docs/_static/logo.png` & `anemoi_utils-0.3.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/docs/_static/style.css` & `anemoi_utils-0.3.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/docs/conf.py` & `anemoi_utils-0.3.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,7 +110,9 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["style.css"]
 
 
 todo_include_todos = not read_the_docs_build
+
+autodoc_member_order = "bysource"  # Keep file order
```

### Comparing `anemoi_utils-0.2.1/docs/index.rst` & `anemoi_utils-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/docs/installing.rst` & `anemoi_utils-0.3.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/pyproject.toml` & `anemoi_utils-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -6,93 +6,103 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 
 [build-system]
-requires = ["setuptools>=60", "setuptools-scm>=8.0"]
+requires = [
+  "setuptools>=60",
+  "setuptools-scm>=8",
+]
 
 [project]
-description = "A package to hold various functions to support training of ML models on ECMWF data."
 name = "anemoi-utils"
 
-dynamic = ["version"]
-license = { file = "LICENSE" }
-requires-python = ">=3.9"
+description = "A package to hold various functions to support training of ML models on ECMWF data."
+keywords = [
+  "ai",
+  "tools",
+]
 
+license = { file = "LICENSE" }
 authors = [
-    { name = "European Centre for Medium-Range Weather Forecasts (ECMWF)", email = "software.support@ecmwf.int" },
+  { name = "European Centre for Medium-Range Weather Forecasts (ECMWF)", email = "software.support@ecmwf.int" },
 ]
 
-keywords = ["tools", "ai"]
+requires-python = ">=3.9"
 
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
-    "Operating System :: OS Independent",
+  "Development Status :: 4 - Beta",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: Apache Software License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
+dynamic = [
+  "version",
+]
 dependencies = [
-    "tomli",  # Only needed before 3.11
-    "pyyaml",
-    "tqdm",
+  "pyyaml",
+  "tomli",  # Only needed before 3.11
+  "tqdm",
+]
+
+optional-dependencies.all = [
+  "gitpython",
+  "nvsmi",
+  "pyyaml",
+  "requests",
+  "termcolor",
+  "tomli",
+  "tqdm",
+]
+optional-dependencies.dev = [
+  "gitpython",
+  "nvsmi",
+  "requests",
+  "termcolor",
+  "tomli",     # Only needed before 3.11
 ]
-
-[project.optional-dependencies]
-provenance = ["GitPython", "nvsmi"]
-
-text = ["termcolor"]
-
-grib = ["requests"]
-
 # Loaded by read-the-docs
 # `pip install .[docs]`
-docs = [
-    "tomli",            # Only needed before 3.11
-    "termcolor",
-    "requests",
-    "sphinx",
-    "sphinx_rtd_theme",
-    "nbsphinx",
-    "pandoc",
-    "sphinx_argparse",
-]
-
-all = [
-    "tomli",     # Only needed before 3.11
-    "GitPython",
-    "nvsmi",
-    "termcolor",
-    "requests",
-]
-
-dev = [
-    "tomli",     # Only needed before 3.11
-    "GitPython",
-    "nvsmi",
-    "termcolor",
-    "requests",
-]
-
-[project.urls]
-Homepage = "https://github.com/ecmwf/anemoi-utils/"
-Documentation = "https://anemoi-utils.readthedocs.io/"
-Repository = "https://github.com/ecmwf/anemoi-utils/"
-Issues = "https://github.com/ecmwf/anemoi-utils/issues"
-# Changelog = "https://github.com/ecmwf/anemoi-utils/CHANGELOG.md"
+optional-dependencies.docs = [
+  "nbsphinx",
+  "pandoc",
+  "requests",
+  "sphinx",
+  "sphinx-argparse",
+  "sphinx-rtd-theme",
+  "termcolor",
+  "tomli",            # Only needed before 3.11
+]
+optional-dependencies.grib = [
+  "requests",
+]
+
+optional-dependencies.provenance = [
+  "gitpython",
+  "nvsmi",
+]
+optional-dependencies.text = [
+  "termcolor",
+]
+urls.Documentation = "https://anemoi-utils.readthedocs.io/"
+urls.Homepage = "https://github.com/ecmwf/anemoi-utils/"
+urls.Issues = "https://github.com/ecmwf/anemoi-utils/issues"
+urls.Repository = "https://github.com/ecmwf/anemoi-utils/"
+scripts.anemoi-utils = "anemoi.utils.__main__:main"
 
-[project.scripts]
-anemoi-utils = "anemoi.utils.__main__:main"
+[tool.setuptools.package-data]
+"anemoi.utils.mars" = [
+  "*.yaml",
+]
 
 [tool.setuptools_scm]
 version_file = "src/anemoi/utils/_version.py"
-
-[tool.setuptools.package-data]
-"anemoi.utils.mars" = ["*.yaml"]
```

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/__main__.py` & `anemoi_utils-0.3.0/src/anemoi/utils/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-#!/usr/bin/env python
-# (C) Copyright 2024 ECMWF.
-#
+# (C) Copyright 2024 European Centre for Medium-Range Weather Forecasts.
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
-#
-
 
 import argparse
+import importlib
 import logging
+import os
 import sys
 import traceback
 
-from . import __version__
-from .commands import COMMANDS
-
 LOG = logging.getLogger(__name__)
 
 
-def create_parser():
-    parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter)
+class Command:
+    def run(self, args):
+        raise NotImplementedError(f"Command not implemented: {args.command}")
+
+
+def make_parser(description, commands):
+    parser = argparse.ArgumentParser(
+        description=description,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
 
     parser.add_argument(
         "--version",
         "-V",
         action="store_true",
         help="show the version and exit",
     )
@@ -33,34 +36,82 @@
         "--debug",
         "-d",
         action="store_true",
         help="Debug mode",
     )
 
     subparsers = parser.add_subparsers(help="commands:", dest="command")
-    for name, command in COMMANDS.items():
+    for name, command in commands.items():
         command_parser = subparsers.add_parser(name, help=command.__doc__)
         command.add_arguments(command_parser)
 
     return parser
 
 
-def main():
-    parser = create_parser()
+class Failed(Command):
+    def __init__(self, name, error):
+        self.name = name
+        self.error = error
+
+    def add_arguments(self, command_parser):
+        command_parser.add_argument("x", nargs=argparse.REMAINDER)
+
+    def run(self, args):
+        print(f"Command '{self.name}' not available: {self.error}")
+        sys.exit(1)
+
+
+def register_commands(here, package, select, fail=None):
+    result = {}
+    not_available = {}
+
+    for p in os.listdir(here):
+        full = os.path.join(here, p)
+        if p.startswith("_"):
+            continue
+        if not (p.endswith(".py") or (os.path.isdir(full) and os.path.exists(os.path.join(full, "__init__.py")))):
+            continue
+
+        name, _ = os.path.splitext(p)
+
+        try:
+            imported = importlib.import_module(
+                f".{name}",
+                package=package,
+            )
+        except ImportError as e:
+            not_available[name] = e
+            continue
+
+        obj = select(imported)
+        if obj is not None:
+            result[name] = obj
+
+    for name, e in not_available.items():
+        if fail is None:
+            pass
+        if callable(fail):
+            result[name] = fail(name, e)
+
+    return result
+
+
+def cli_main(version, description, commands):
+    parser = make_parser(description, commands)
     args = parser.parse_args()
 
     if args.version:
-        print(__version__)
+        print(version)
         return
 
     if args.command is None:
         parser.print_help()
         return
 
-    cmd = COMMANDS[args.command]
+    cmd = commands[args.command]
 
     logging.basicConfig(
         format="%(asctime)s %(levelname)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
         level=logging.DEBUG if args.debug else logging.INFO,
     )
 
@@ -68,10 +119,8 @@
         cmd.run(args)
     except ValueError as e:
         traceback.print_exc()
         LOG.error("\n💣 %s", str(e).lstrip())
         LOG.error("💣 Exiting")
         sys.exit(1)
 
-
-if __name__ == "__main__":
-    main()
+    sys.exit(0)
```

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/caching.py` & `anemoi_utils-0.3.0/src/anemoi/utils/caching.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/checkpoints.py` & `anemoi_utils-0.3.0/src/anemoi/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/commands/checkpoint.py` & `anemoi_utils-0.3.0/src/anemoi/utils/commands/checkpoint.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/config.py` & `anemoi_utils-0.3.0/src/anemoi/utils/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/dates.py` & `anemoi_utils-0.3.0/src/anemoi/utils/dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/grib.py` & `anemoi_utils-0.3.0/src/anemoi/utils/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/humanize.py` & `anemoi_utils-0.3.0/src/anemoi/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/mars/__init__.py` & `anemoi_utils-0.3.0/src/anemoi/utils/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/provenance.py` & `anemoi_utils-0.3.0/src/anemoi/utils/provenance.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/text.py` & `anemoi_utils-0.3.0/src/anemoi/utils/text.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/src/anemoi/utils/timer.py` & `anemoi_utils-0.3.0/src/anemoi/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 from .humanize import seconds
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Timer:
+    """Context manager to measure elapsed time."""
+
     def __init__(self, title, logger=LOGGER):
         self.title = title
         self.start = time.time()
         self.logger = logger
 
     def __enter__(self):
         return self
```

### Comparing `anemoi_utils-0.2.1/src/anemoi_utils.egg-info/PKG-INFO` & `anemoi_utils-0.3.0/src/anemoi_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.2.1
+Version: 0.3.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,55 +201,58 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
-Project-URL: Homepage, https://github.com/ecmwf/anemoi-utils/
 Project-URL: Documentation, https://anemoi-utils.readthedocs.io/
-Project-URL: Repository, https://github.com/ecmwf/anemoi-utils/
+Project-URL: Homepage, https://github.com/ecmwf/anemoi-utils/
 Project-URL: Issues, https://github.com/ecmwf/anemoi-utils/issues
-Keywords: tools,ai
+Project-URL: Repository, https://github.com/ecmwf/anemoi-utils/
+Keywords: ai,tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: tomli
 Requires-Dist: pyyaml
+Requires-Dist: tomli
 Requires-Dist: tqdm
-Provides-Extra: provenance
-Requires-Dist: GitPython; extra == "provenance"
-Requires-Dist: nvsmi; extra == "provenance"
-Provides-Extra: text
-Requires-Dist: termcolor; extra == "text"
-Provides-Extra: grib
-Requires-Dist: requests; extra == "grib"
-Provides-Extra: docs
-Requires-Dist: tomli; extra == "docs"
-Requires-Dist: termcolor; extra == "docs"
-Requires-Dist: requests; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: pandoc; extra == "docs"
-Requires-Dist: sphinx_argparse; extra == "docs"
 Provides-Extra: all
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: GitPython; extra == "all"
+Requires-Dist: gitpython; extra == "all"
 Requires-Dist: nvsmi; extra == "all"
-Requires-Dist: termcolor; extra == "all"
+Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: requests; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: tomli; extra == "all"
+Requires-Dist: tqdm; extra == "all"
 Provides-Extra: dev
-Requires-Dist: tomli; extra == "dev"
-Requires-Dist: GitPython; extra == "dev"
+Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: nvsmi; extra == "dev"
-Requires-Dist: termcolor; extra == "dev"
 Requires-Dist: requests; extra == "dev"
+Requires-Dist: termcolor; extra == "dev"
+Requires-Dist: tomli; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: requests; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-argparse; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: termcolor; extra == "docs"
+Requires-Dist: tomli; extra == "docs"
+Provides-Extra: grib
+Requires-Dist: requests; extra == "grib"
+Provides-Extra: provenance
+Requires-Dist: gitpython; extra == "provenance"
+Requires-Dist: nvsmi; extra == "provenance"
+Provides-Extra: text
+Requires-Dist: termcolor; extra == "text"
```

### Comparing `anemoi_utils-0.2.1/src/anemoi_utils.egg-info/SOURCES.txt` & `anemoi_utils-0.3.0/src/anemoi_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/tests/test_dates.py` & `anemoi_utils-0.3.0/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_utils-0.2.1/tests/test_utils.py` & `anemoi_utils-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

