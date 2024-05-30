# Comparing `tmp/grdwindinversion-0.2.3.post7.tar.gz` & `tmp/grdwindinversion-0.2.3.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grdwindinversion-0.2.3.post7.tar", last modified: Mon Feb 12 17:43:27 2024, max compression
+gzip compressed data, was "grdwindinversion-0.2.3.post8.tar", last modified: Thu May 30 09:25:29 2024, max compression
```

## Comparing `grdwindinversion-0.2.3.post7.tar` & `grdwindinversion-0.2.3.post8.tar`

### file list

```diff
@@ -1,70 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.869425 grdwindinversion-0.2.3.post7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.873425 grdwindinversion-0.2.3.post7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.869425 grdwindinversion-0.2.3.post7/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.873425 grdwindinversion-0.2.3.post7/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.873425 grdwindinversion-0.2.3.post7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.869425 grdwindinversion-0.2.3.post7/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.873425 grdwindinversion-0.2.3.post7/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/_static/css/grdwindinversion.css
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5704 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.873425 grdwindinversion-0.2.3.post7/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/examples/wind-inversion-from-grd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/grdwindinversion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/grdwindinversion/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/config_RCM.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/config_RS2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/config_S1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/config_hy2b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/config_prod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/config_prod_recal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28836 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/load_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/grdwindinversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-12 17:43:27.000000 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-02-12 17:43:27.000000 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 17:43:27.000000 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-12 17:43:27.000000 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-12 17:43:27.000000 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-12 17:43:27.000000 grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 17:43:27.877425 grdwindinversion-0.2.3.post7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/tests/test_grdwindinversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-12 17:43:13.000000 grdwindinversion-0.2.3.post7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.838355 grdwindinversion-0.2.3.post8/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.830355 grdwindinversion-0.2.3.post8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.830355 grdwindinversion-0.2.3.post8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-30 09:25:29.838355 grdwindinversion-0.2.3.post8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.830355 grdwindinversion-0.2.3.post8/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.830355 grdwindinversion-0.2.3.post8/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.834355 grdwindinversion-0.2.3.post8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.830355 grdwindinversion-0.2.3.post8/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.834355 grdwindinversion-0.2.3.post8/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/_static/css/grdwindinversion.css
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5704 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.834355 grdwindinversion-0.2.3.post8/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/examples/wind-inversion-from-grd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.834355 grdwindinversion-0.2.3.post8/grdwindinversion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.838355 grdwindinversion-0.2.3.post8/grdwindinversion/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/config_prod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/config_prod_recal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    33740 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/grdwindinversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.838355 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-30 09:25:29.000000 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-30 09:25:29.000000 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:25:29.000000 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 09:25:29.000000 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 09:25:29.000000 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 09:25:29.000000 grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:25:29.838355 grdwindinversion-0.2.3.post8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:25:29.838355 grdwindinversion-0.2.3.post8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/tests/test_grdwindinversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-30 09:25:19.000000 grdwindinversion-0.2.3.post8/tox.ini
```

### Comparing `grdwindinversion-0.2.3.post7/.github/workflows/publish.yml` & `grdwindinversion-0.2.3.post8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/.gitignore` & `grdwindinversion-0.2.3.post8/.gitignore`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/.pre-commit-config.yaml` & `grdwindinversion-0.2.3.post8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/CONTRIBUTING.rst` & `grdwindinversion-0.2.3.post8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/LICENSE` & `grdwindinversion-0.2.3.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/Makefile` & `grdwindinversion-0.2.3.post8/Makefile`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/PKG-INFO` & `grdwindinversion-0.2.3.post8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grdwindinversion
-Version: 0.2.3.post7
+Version: 0.2.3.post8
 Summary: Package to perform Wind inversion from GRD Level-1 SAR images
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `grdwindinversion-0.2.3.post7/README.md` & `grdwindinversion-0.2.3.post8/README.md`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/docs/Makefile` & `grdwindinversion-0.2.3.post8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/docs/conf.py` & `grdwindinversion-0.2.3.post8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/docs/examples/wind-inversion-from-grd.ipynb` & `grdwindinversion-0.2.3.post8/docs/examples/wind-inversion-from-grd.ipynb`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/docs/index.rst` & `grdwindinversion-0.2.3.post8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/docs/installation.rst` & `grdwindinversion-0.2.3.post8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/docs/make.bat` & `grdwindinversion-0.2.3.post8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/.gitignore` & `grdwindinversion-0.2.3.post8/grdwindinversion/.gitignore`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/.travis.yml` & `grdwindinversion-0.2.3.post8/grdwindinversion/.travis.yml`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/config_hy2b.yaml` & `grdwindinversion-0.2.3.post8/grdwindinversion/config_prod.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 S1A:
-    GMF_VV_NAME: "cmod5n"
-    GMF_VH_NAME: "gmf_hy2B"
+    GMF_VV_NAME: "gmf_cmod5n"
+    GMF_VH_NAME: "gmf_s1_v2"
     dsig_VH_NAME: "gmf_s1_v2"
     apply_flattening: True
     recalibration: False
 S1B:
-    GMF_VV_NAME: "cmod5n"
-    GMF_VH_NAME: "gmf_hy2B"
+    GMF_VV_NAME: "gmf_cmod5n"
+    GMF_VH_NAME: "gmf_s1_v2"
     dsig_VH_NAME: "gmf_s1_v2"
     apply_flattening: True
     recalibration: False
 RS2:
-    GMF_VV_NAME: "cmod5n"
-    GMF_VH_NAME: "gmf_hy2B"
-    dsig_VH_NAME: "gmf_s1_v2"
+    GMF_VV_NAME: "gmf_cmod5n"
+    GMF_VH_NAME: "gmf_rs2_v2"
+    dsig_VH_NAME: "gmf_rs2_v2"
     apply_flattening: False
     recalibration: False
 RCM:
-    GMF_VV_NAME: "cmod5n"
-    GMF_VH_NAME: "gmf_hy2B"
+    GMF_VV_NAME: "gmf_cmod5n"
+    GMF_VH_NAME: "gmf_rcm_noaa"
     dsig_VH_NAME: "gmf_s1_v2"
     apply_flattening: True
     recalibration: False
```

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/config_prod.yaml` & `grdwindinversion-0.2.3.post8/grdwindinversion/config_prod_recal.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 S1A:
-    GMF_VV_NAME: "cmod5n"
+    GMF_VV_NAME: "gmf_cmod5n"
     GMF_VH_NAME: "gmf_s1_v2"
     dsig_VH_NAME: "gmf_s1_v2"
     apply_flattening: True
-    recalibration: False
+    recalibration: True
 S1B:
-    GMF_VV_NAME: "cmod5n"
+    GMF_VV_NAME: "gmf_cmod5n"
     GMF_VH_NAME: "gmf_s1_v2"
     dsig_VH_NAME: "gmf_s1_v2"
     apply_flattening: True
-    recalibration: False
+    recalibration: True
 RS2:
-    GMF_VV_NAME: "cmod5n"
+    GMF_VV_NAME: "gmf_cmod5n"
     GMF_VH_NAME: "gmf_rs2_v2"
     dsig_VH_NAME: "gmf_rs2_v2"
     apply_flattening: False
-    recalibration: False
+    recalibration: True
 RCM:
-    GMF_VV_NAME: "cmod5n"
+    GMF_VV_NAME: "gmf_cmod5n"
     GMF_VH_NAME: "gmf_rcm_noaa"
     dsig_VH_NAME: "gmf_s1_v2"
     apply_flattening: True
-    recalibration: False
+    recalibration: True
```

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/inversion.py` & `grdwindinversion-0.2.3.post8/grdwindinversion/inversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-import pdb
 import traceback
 
 import xsar
 import xsarsea
 from xsarsea import windspeed
 import grdwindinversion
 import xarray as xr
@@ -17,32 +15,32 @@
 
 import re
 import string
 import os
 from grdwindinversion.load_config import getConf
 # optional debug messages
 import logging
-
 logging.basicConfig()
 logging.getLogger('xsarsea.windspeed').setLevel(
     logging.INFO)  # or .setLevel(logging.INFO)
-# encode gcps as json string
-
-
-class JSONEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, np.integer):
-            return int(obj)
 
 
 def getSensorMetaDataset(filename):
     """
+    Find the sensor name and the corresponding meta and dataset functions
 
-    :param filename: str SAR SAFE or equivalent
-    :return:
+    Parameters
+    ----------
+    filename : str
+        input filename
+
+    Returns
+    -------
+    tuple
+        sensor name, sensor long name, meta function, dataset function
     """
     if ("S1A" in filename):
         return "S1A", "SENTINEL-1 A", xsar.Sentinel1Meta, xsar.Sentinel1Dataset
     elif ("S1B" in filename):
         return "S1B", "SENTINEL-1 B", xsar.Sentinel1Meta, xsar.Sentinel1Dataset
     elif ("RS2" in filename):
         return "RS2", "RADARSAT-2", xsar.RadarSat2Meta, xsar.RadarSat2Dataset
@@ -50,20 +48,31 @@
         return "RCM", "RADARSAT Constellation", xsar.RcmMeta, xsar.RcmDataset
     else:
         raise ValueError("must be S1A|S1B|RS2|RCM, got filename %s" % filename)
 
 
 def getOutputName2(input_file, out_folder, sensor, meta):
     """
+    Create output filename for L2-GRD product
 
-    :param input_file: str
-    :param out_folder: str
-    :param sensor: str S1A or S1B
-    :param meta: obj `xsar.Sentinel1Meta` (or any other supported SAR mission)
-    :return:
+    Parameters
+    ----------
+    input_file : str
+        input filename
+    out_folder : str
+        output folder
+    sensor : str
+        sensor name
+    meta : obj `xsar.BaseMeta` (one of the supported SAR mission)
+        meta object
+
+    Returns
+    -------
+    outfile : str
+        output filename
     """
     basename = os.path.basename(input_file)
     basename_match = basename
     meta_start_date = meta.start_date.split(".")[0].replace(
         "-", "").replace(":", "").replace(" ", "t").replace("Z", "")
     meta_stop_date = meta.stop_date.split(".")[0].replace(
         "-", "").replace(":", "").replace(" ", "t").replace("Z", "")
@@ -103,113 +112,207 @@
         return out_file
 
     else:
         raise ValueError(
             "sensor must be S1A|S1B|RS2|RCM, got sensor %s" % sensor)
 
 
-def getAncillary(meta):
+def getAncillary(meta, ancillary_name='ecmwf'):
+    """
+    Map ancillary wind from ECMWF.
+    This function is used to check if the ECMWF files are available and to map the model to the SAR data.
 
-    logging.debug('conf: %s', getConf())
-    ec01 = getConf()['ecmwf_0100_1h']
-    ec0125 = getConf()['ecmwf_0125_1h']
-    logging.debug('ec01 : %s', ec01)
-    meta.set_raster('ecmwf_0100_1h', ec01)
-    meta.set_raster('ecmwf_0125_1h', ec0125)
-
-    map_model = None
-    # only keep best ecmwf  (FIXME: it's hacky, and xsar should provide a better method to handle this)
-    for ecmwf_name in ['ecmwf_0125_1h', 'ecmwf_0100_1h']:
-        ecmwf_infos = meta.rasters.loc[ecmwf_name]
-        try:
-            ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
-                                                     date=datetime.datetime.strptime(meta.start_date,
-                                                                                     '%Y-%m-%d %H:%M:%S.%f'))[1]
-        # temporary for RCM issue https://github.com/umr-lops/xarray-safe-rcm/issues/34
-        except Exception as e:
-            ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
-                                                     date=datetime.datetime.strptime(meta.start_date,
-                                                                                     '%Y-%m-%d %H:%M:%S'))[1]
-
-        if not os.path.isfile(ecmwf_file):
-            # temporary
-            # if repro does not exist we look at not repro folder (only one will exist after)
-            if ecmwf_name == "ecmwf_0100_1h":
-                ecmwf_infos['resource'] = ecmwf_infos['resource'].replace(
-                    "netcdf_light_REPRO_tree", "netcdf_light")
-                try:
-                    ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
-                                                             date=datetime.datetime.strptime(meta.start_date,
-                                                                                             '%Y-%m-%d %H:%M:%S.%f'))[1]
-                except Exception as e:
-                    ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
-                                                             date=datetime.datetime.strptime(meta.start_date,
-                                                                                             '%Y-%m-%d %H:%M:%S'))[1]
+    Parameters
+    ----------
+    meta: obj `xsar.BaseMeta` (one of the supported SAR mission)
+
+    Returns
+    -------
+    dict
+        map model to SAR data
+    """
 
-                if not os.path.isfile(ecmwf_file):
-                    meta.rasters = meta.rasters.drop([ecmwf_name])
-                else:
-                    map_model = {'%s_%s' % (ecmwf_name, uv): 'model_%s' % uv for uv in [
-                        'U10', 'V10']}
+    if ancillary_name == 'ecmwf':
 
-            else:
+        logging.debug('conf: %s', getConf())
+        ec01 = getConf()['ecmwf_0100_1h']
+        ec0125 = getConf()['ecmwf_0125_1h']
+        logging.debug('ec01 : %s', ec01)
+        meta.set_raster('ecmwf_0100_1h', ec01)
+        meta.set_raster('ecmwf_0125_1h', ec0125)
+
+        map_model = None
+        # only keep best ecmwf  (FIXME: it's hacky, and xsar should provide a better method to handle this)
+        for ecmwf_name in ['ecmwf_0125_1h', 'ecmwf_0100_1h']:
+            ecmwf_infos = meta.rasters.loc[ecmwf_name]
+            try:
+                ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
+                                                         date=datetime.datetime.strptime(meta.start_date,
+                                                                                         '%Y-%m-%d %H:%M:%S.%f'))[1]
+            # temporary for RCM issue https://github.com/umr-lops/xarray-safe-rcm/issues/34
+            except Exception as e:
+                ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
+                                                         date=datetime.datetime.strptime(meta.start_date,
+                                                                                         '%Y-%m-%d %H:%M:%S'))[1]
+            if not os.path.isfile(ecmwf_file):
+                # temporary
+                # if repro does not exist we look at not repro folder (only one will exist after)
+                """
+                if ecmwf_name == "ecmwf_0100_1h":
+                    ecmwf_infos['resource'] = ecmwf_infos['resource'].replace(
+                        "netcdf_light_REPRO_tree", "netcdf_light")
+                    try:
+                        ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
+                                                                 date=datetime.datetime.strptime(meta.start_date,
+                                                                                                 '%Y-%m-%d %H:%M:%S.%f'))[1]
+                    except Exception as e:
+                        ecmwf_file = ecmwf_infos['get_function'](ecmwf_infos['resource'],
+                                                                 date=datetime.datetime.strptime(meta.start_date,
+                                                                                                 '%Y-%m-%d %H:%M:%S'))[1]
+
+                    if not os.path.isfile(ecmwf_file):
+                        meta.rasters = meta.rasters.drop([ecmwf_name])
+                    else:
+                        map_model = {'%s_%s' % (ecmwf_name, uv): 'model_%s' % uv for uv in [
+                            'U10', 'V10']}
+
+                else:
+                """
                 meta.rasters = meta.rasters.drop([ecmwf_name])
-        else:
-            map_model = {'%s_%s' % (ecmwf_name, uv): 'model_%s' %
-                         uv for uv in ['U10', 'V10']}
+            else:
+                map_model = {'%s_%s' % (ecmwf_name, uv): 'model_%s' %
+                             uv for uv in ['U10', 'V10']}
 
-    return map_model
+        return map_model
+
+    else:
+        raise ValueError("ancillary_name must be ecmwf, got %s" %
+                         ancillary_name)
 
 
 def inverse(dual_pol, inc, sigma0, sigma0_dual, ancillary_wind, dsig_cr, model_vv, model_vh):
+    """
+    Invert sigma0 to retrieve wind using model (lut or gmf).
+
+    Parameters
+    ----------
+    dual_pol: bool
+        True if dualpol, False if singlepol 
+    inc: xarray.DataArray
+        incidence angle
+    sigma0: xarray.DataArray
+        sigma0 to be inverted
+    sigma0_dual: xarray.DataArray 
+        sigma0 to be inverted for dualpol
+    ancillary_wind=: xarray.DataArray (numpy.complex28)
+        ancillary wind
+            | (for example ecmwf winds), in **model convention**
+    dsig_cr=: float or xarray.DataArray
+        parameters used for
+
+            | `Jsig_cr=((sigma0_gmf - sigma0) / dsig_cr) ** 2`    
+    model_vv=: str 
+        model to use for VV or HH polarization.
+    model_vh=: str 
+        model to use for VH or HV polarization.
+
+    Returns
+    -------
+    xarray.DataArray or tuple
+        inverted wind in **gmf convention** .
+
+    See Also
+    --------
+    xsarsea documentation 
+    https://cyclobs.ifremer.fr/static/sarwing_datarmor/xsarsea/examples/windspeed_inversion.html    
+    """
     logging.debug("inversion")
-    # 4 - Inversion
-    windspeeds = windspeed.invert_from_model(
+
+    # add potential missing gmfs (only cmod7 & ms1ahw)
+
+    if (model_vv == "gmf_cmod7"):
+        windspeed.register_cmod7(getConf()["lut_cmod7_path"])
+
+    if (model_vh == "sarwing_lut_cmodms1ahw"):
+        windspeed.register_one_sarwing_lut(getConf()["lut_ms1ahw_path"])
+
+    winds = windspeed.invert_from_model(
         inc,
         sigma0,
         sigma0_dual,
-        # ancillary_wind=-np.conj(xsar_dataset.dataset['ancillary_wind']),
-        ancillary_wind=-ancillary_wind,
+        ancillary_wind=-np.conj(ancillary_wind),
         dsig_cr=dsig_cr,
         model=(model_vv, model_vh))
+
     if dual_pol:
-        windspeed_co, windspeed_dual = windspeeds
-        
-        windspeed_cr = windspeed.invert_from_model(
+        wind_co, wind_dual = winds
+
+        wind_cross = windspeed.invert_from_model(
             inc.values,
             sigma0_dual.values,
-            # ancillary_wind=-np.conj(xsar_dataset.dataset['ancillary_wind']),
             dsig_cr=dsig_cr.values,
             model=model_vh)
 
-        return np.abs(windspeed_co), np.abs(windspeed_dual), np.abs(windspeed_cr)
+        return wind_co, wind_dual, wind_cross
     else:
-        windspeed_co = windspeeds
+        wind_co = winds
 
-    return np.abs(windspeed_co), None, None
+    return wind_co, None, None
 
 
+def makeL2asOwi(xr_dataset, dual_pol, copol, crosspol, copol_gmf, crosspol_gmf, config):
+    """
+    Rename xr_dataset variables and attributes to match naming convention.
 
+    Parameters
+    ----------
+    xr_dataset: xarray.Dataset
+        dataset to rename
+    dual_pol: bool
+        True if dualpol, False if singlepol
+    copol: str
+        copolarization name
+    crosspol: str
+        crosspolarization name
+    copol_gmf: str
+        copolarization GMF name
+    crosspol_gmf: str
+        crosspolarization GMF name
+    config: dict
+        configuration file
+
+    Returns
+    -------
+    xarray.Dataset
+        final dataset 
+    dict
+        encoding dict
 
-def makeL2asOwi(xr_dataset, dual_pol, copol, crosspol, copol_gmf, crosspol_gmf, config):
-    # rename to match sarwing naming
+    See Also
+    --------
+    """
 
     xr_dataset = xr_dataset.rename({
         'longitude': 'owiLon',
         'latitude': 'owiLat',
         'incidence': 'owiIncidenceAngle',
         'elevation': 'owiElevationAngle',
         'ground_heading': 'owiHeading',
         'land_mask': 'owiLandFlag',
-        'mask' : 'owiMask',
+        'offboresight': 'owiOffBoresightAngle',
+        'mask': 'owiMask',
         'windspeed_co': 'owiWindSpeed_co',
         'windspeed_cross': 'owiWindSpeed_cross',
-        'windspeed_dual': 'owiWindSpeed',     
+        'windspeed_dual': 'owiWindSpeed',
+        'winddir_co': 'owiWindDirection_co',
+        'winddir_cross': 'owiWindDirection_cross',
+        'winddir_dual': 'owiWindDirection',
+        'ancillary_wind_speed': 'owiEcmwfWindSpeed',
+        'ancillary_wind_direction': 'owiEcmwfWindDirection',
     })
-        
     xr_dataset['owiNrcs'] = xr_dataset['sigma0_ocean'].sel(pol=copol)
     xr_dataset.owiNrcs.attrs = xr_dataset.sigma0_ocean.attrs
     xr_dataset.owiNrcs.attrs['units'] = 'm^2 / m^2'
     xr_dataset.owiNrcs.attrs['long_name'] = 'Normalized Radar Cross Section'
     xr_dataset.owiNrcs.attrs['definition'] = 'owiNrcs_no_noise_correction - owiNesz'
 
     # NESZ & DSIG
@@ -220,44 +323,41 @@
     xr_dataset['owiNrcs_no_noise_correction'] = xr_dataset['sigma0_ocean_raw'].sel(
         pol=copol)
     xr_dataset.owiNrcs_no_noise_correction.attrs = xr_dataset.sigma0_ocean_raw.attrs
     xr_dataset.owiNrcs_no_noise_correction.attrs['units'] = 'm^2 / m^2'
     xr_dataset.owiNrcs_no_noise_correction.attrs[
         'long_name'] = 'Normalized Radar Cross Section ; no noise correction applied'
     xr_dataset.owiNrcs_no_noise_correction.attrs[
-            'comment'] = 'owiNrcs_no_noise_correction ; no recalibration'
-    
+        'comment'] = 'owiNrcs_no_noise_correction ; no recalibration'
+
     if 'swath_number' in xr_dataset:
         xr_dataset = xr_dataset.rename({
-             'swath_number' : 'owiSwathNumber',
-             'swath_number_flag' : 'owiSwathNumberFlag'
-            })
-        
+            'swath_number': 'owiSwathNumber',
+            'swath_number_flag': 'owiSwathNumberFlag'
+        })
+
     if "sigma0_raw__corrected" in xr_dataset:
-        xr_dataset['owiNrcs_no_noise_correction_recalibrated'] = xr_dataset['sigma0_raw__corrected'].sel(pol=copol)
+        xr_dataset['owiNrcs_no_noise_correction_recalibrated'] = xr_dataset['sigma0_raw__corrected'].sel(
+            pol=copol)
         xr_dataset.owiNrcs_no_noise_correction_recalibrated.attrs = xr_dataset.sigma0_raw__corrected.attrs
         xr_dataset.owiNrcs_no_noise_correction_recalibrated.attrs['units'] = 'm^2 / m^2'
         xr_dataset.owiNrcs_no_noise_correction_recalibrated.attrs[
             'long_name'] = 'Normalized Radar Cross Section, no noise correction applied'
         xr_dataset.owiNrcs_no_noise_correction_recalibrated.attrs[
-            'comment'] = 'owiNrcs_no_noise_correction ; recalibrated with kersten method'  
-        
-        xr_dataset.owiNrcs.attrs['definition'] = 'owiNrcs_no_noise_correction_recalibrated - owiNesz'
-
-            
+            'comment'] = 'owiNrcs_no_noise_correction ; recalibrated with kersten method'
 
+        xr_dataset.owiNrcs.attrs['definition'] = 'owiNrcs_no_noise_correction_recalibrated - owiNesz'
 
-    
     if dual_pol:
-        
+
         xr_dataset = xr_dataset.rename({
             'dsig_cross': 'owiDsig_cross',
-            'nesz_cross_final' : 'owiNesz_cross_final'
-        })        
-        
+            'nesz_cross_final': 'owiNesz_cross_final'
+        })
+
         xr_dataset['owiNrcs_cross'] = xr_dataset['sigma0_ocean'].sel(
             pol=crosspol)
         xr_dataset.owiNrcs_cross.attrs['units'] = 'm^2 / m^2'
         xr_dataset.owiNrcs_cross.attrs['long_name'] = 'Normalized Radar Cross Section'
         xr_dataset.owiNrcs_cross.attrs['definition'] = 'owiNrcs_cross_no_noise_correction - owiNesz_cross'
 
         xr_dataset = xr_dataset.assign(owiNesz_cross=(
@@ -268,45 +368,43 @@
             pol=crosspol)
 
         xr_dataset.owiNrcs_cross_no_noise_correction.attrs['units'] = 'm^2 / m^2'
         xr_dataset.owiNrcs_cross_no_noise_correction.attrs[
             'long_name'] = 'Normalized Radar Cross Section, no noise correction applied'
 
         if "sigma0_raw__corrected" in xr_dataset:
-            xr_dataset['owiNrcs_cross_no_noise_correction_recalibrated'] = xr_dataset['sigma0_raw__corrected'].sel(pol=crosspol)
+            xr_dataset['owiNrcs_cross_no_noise_correction_recalibrated'] = xr_dataset['sigma0_raw__corrected'].sel(
+                pol=crosspol)
             xr_dataset.owiNrcs_cross_no_noise_correction_recalibrated.attrs = xr_dataset.sigma0_raw__corrected.attrs
             xr_dataset.owiNrcs_cross_no_noise_correction_recalibrated.attrs['units'] = 'm^2 / m^2'
             xr_dataset.owiNrcs_cross_no_noise_correction_recalibrated.attrs[
                 'long_name'] = 'Normalized Radar Cross Section ; no noise correction applied'
             xr_dataset.owiNrcs_cross_no_noise_correction_recalibrated.attrs[
-            'comment'] = 'owiNrcs_cross_no_noise_correction ; recalibrated with kersten method'
-    
+                'comment'] = 'owiNrcs_cross_no_noise_correction ; recalibrated with kersten method'
+
             xr_dataset.owiNrcs_cross.attrs['definition'] = 'owiNrcs_cross_no_noise_correction_recalibrated - owiNesz_cross'
 
-    
-    
     xr_dataset["owiWindSpeed_co"].attrs["comment"] = xr_dataset["owiWindSpeed_co"].attrs["comment"].replace(
         "wind speed and direction", "wind speed")
 
+    xr_dataset["owiWindDirection_co"].attrs["comment"] = "wind direction in meteorological convention, 0=North, 90=East"
+
     if dual_pol:
         xr_dataset["owiWindSpeed"].attrs["comment"] = xr_dataset["owiWindSpeed"].attrs["comment"].replace(
             "wind speed and direction", "wind speed")
+        xr_dataset["owiWindDirection"].attrs["comment"] = "wind direction in meteorological convention, 0=North, 90=East"
 
         xr_dataset["owiWindSpeed_cross"].attrs['comment'] = "wind speed inverted from model %s (%s)" % (
             crosspol_gmf, crosspol)
 
+        xr_dataset["owiWindDirection_cross"].attrs["comment"] = "wind direction in meteorological convention, 0=North, 90=East, copied from dualpol"
+
         xr_dataset.owiWindSpeed_cross.attrs['model'] = crosspol_gmf
         xr_dataset.owiWindSpeed_cross.attrs['units'] = 'm/s'
 
-    xr_dataset = xr_dataset.assign(
-        owiEcmwfWindSpeed=(['line', 'sample'], np.abs(xr_dataset['ancillary_wind'].data)))
-    xr_dataset = xr_dataset.assign(
-        owiEcmwfWindDirection=(['line', 'sample'], np.angle(xr_dataset['ancillary_wind'])))
-    xr_dataset['owiEcmwfWindDirection'].attrs['comment'] = 'angle in radians, anticlockwise, 0=sample'
-
     xr_dataset['owiWindQuality'] = xr.full_like(xr_dataset.owiNrcs, 0)
     xr_dataset['owiWindQuality'].attrs[
         'long_name'] = "Quality flag taking into account the consistency_between_wind_inverted_and_NRCS_and_Doppler_measured"
     xr_dataset['owiWindQuality'].attrs['valid_range'] = np.array([0, 3])
     xr_dataset['owiWindQuality'].attrs['flag_values'] = np.array([
         0, 1, 2, 3])
     xr_dataset['owiWindQuality'].attrs['flag_meanings'] = "good medium low poor"
@@ -319,124 +417,126 @@
         0, 1, 2, 3])
     xr_dataset['owiWindFilter'].attrs[
         'flag_meanings'] = "homogeneous_NRCS, heterogeneous_from_co-polarization_NRCS, heterogeneous_from_cross-polarization_NRCS, heterogeneous_from_dual-polarization_NRCS"
     xr_dataset['owiWindFilter'].attrs['comment'] = 'not done yet'
 
     xr_dataset = xr_dataset.rename(
         {"line": "owiAzSize", "sample": "owiRaSize"})
-    
-   
-    xr_dataset = xr_dataset.drop_vars(['sigma0_ocean', 'sigma0', 'sigma0_ocean_raw','sigma0_raw', 'ancillary_wind','nesz','spatial_ref'])
+
+    xr_dataset = xr_dataset.drop_vars(
+        ['sigma0_ocean', 'sigma0', 'sigma0_ocean_raw', 'sigma0_raw', 'ancillary_wind', 'nesz', 'spatial_ref'])
     if 'sigma0_raw__corrected' in xr_dataset:
         xr_dataset = xr_dataset.drop_vars(["sigma0_raw__corrected"])
     xr_dataset = xr_dataset.drop_dims(['pol'])
-    
-    #attrs 
+
+    # attrs
 
     xr_dataset.compute()
 
     for var in ['footprint', 'multidataset', 'rawDataStartTime', 'specialHandlingRequired']:
         if var in xr_dataset.attrs:
             xr_dataset.attrs[var] = str(xr_dataset.attrs[var])
         if "approx_transform" in xr_dataset.attrs:
             del xr_dataset.attrs["approx_transform"]
 
-        xr_dataset.attrs["TITLE"] = "Sentinel-1 OWI Component"
-        xr_dataset.attrs["missionPhase"] = "Test"
-        xr_dataset.attrs["polarisation"] = xr_dataset.pols
-        xr_dataset.attrs["acquisitionStation"] = "/"
-        xr_dataset.attrs["softwareVersion"] = "/"
-        xr_dataset.attrs["pythonVersion"] = str(
-            sys.version_info.major)+'.'+str(sys.version_info.minor)
-        xr_dataset.attrs["polarisationRatio"] = "/"
-        xr_dataset.attrs["l2ProcessingUtcTime"] = datetime.datetime.now().strftime(
+    xr_dataset.attrs["TITLE"] = "Sentinel-1 OWI Component"
+    xr_dataset.attrs["missionPhase"] = "Test"
+    xr_dataset.attrs["acquisitionStation"] = "/"
+    xr_dataset.attrs["softwareVersion"] = "/"
+    xr_dataset.attrs["pythonVersion"] = str(
+        sys.version_info.major)+'.'+str(sys.version_info.minor)
+    xr_dataset.attrs["polarisationRatio"] = "/"
+    xr_dataset.attrs["l2ProcessingUtcTime"] = datetime.datetime.now().strftime(
+        "%Y-%m-%dT%H:%M:%SZ")
+    xr_dataset.attrs["processingCenter"] = "/"
+    try:
+        xr_dataset.attrs["firstMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['start_date'],
+                                                                              "%Y-%m-%d %H:%M:%S.%f").strftime(
             "%Y-%m-%dT%H:%M:%SZ")
-        xr_dataset.attrs["processingCenter"] = "/"
-        try:
-            xr_dataset.attrs["firstMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['start_date'],
-                                                                                "%Y-%m-%d %H:%M:%S.%f").strftime(
-                "%Y-%m-%dT%H:%M:%SZ")
-            xr_dataset.attrs["lastMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['stop_date'],
-                                                                               "%Y-%m-%d %H:%M:%S.%f").strftime(
-                "%Y-%m-%dT%H:%M:%SZ")
-        except:
-            xr_dataset.attrs["firstMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['start_date'],
-                                                                                "%Y-%m-%d %H:%M:%S").strftime(
-                "%Y-%m-%dT%H:%M:%SZ")
-            xr_dataset.attrs["lastMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['stop_date'],
-                                                                               "%Y-%m-%d %H:%M:%S").strftime(
-                "%Y-%m-%dT%H:%M:%SZ")
-        xr_dataset.attrs["clmSource"] = "/"
-        xr_dataset.attrs["bathySource"] = "/"
-        xr_dataset.attrs['oswAlgorithmName'] = 'grdwindinversion'
-        xr_dataset.attrs["owiAlgorithmVersion"] = grdwindinversion.__version__
-        xr_dataset.attrs["gmf"] = config['GMF_'+copol_gmf+'_NAME'] + \
-            ", " + config["GMF_"+crosspol_gmf+"_NAME"]
-        xr_dataset.attrs["iceSource"] = "/"
-        xr_dataset.attrs["owiNoiseCorrection"] = "False"
-        xr_dataset.attrs["inversionTabGMF"] = config['GMF_'+copol_gmf +
-                                                   '_NAME'] + ", " + config["GMF_"+crosspol_gmf+"_NAME"]
-        xr_dataset.attrs["wnf_3km_average"] = "/"
-        xr_dataset.attrs["owiWindSpeedSrc"] = "owiWindSpeed"
-        xr_dataset.attrs["owiWindDirectionSrc"] = "/"
-
-    for var in xr_dataset.variables:
-        if "history" in xr_dataset[var].attrs:
-            del xr_dataset[var].attrs["history"]
+        xr_dataset.attrs["lastMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['stop_date'],
+                                                                             "%Y-%m-%d %H:%M:%S.%f").strftime(
+            "%Y-%m-%dT%H:%M:%SZ")
+    except:
+        xr_dataset.attrs["firstMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['start_date'],
+                                                                              "%Y-%m-%d %H:%M:%S").strftime(
+            "%Y-%m-%dT%H:%M:%SZ")
+        xr_dataset.attrs["lastMeasurementTime"] = datetime.datetime.strptime(xr_dataset.attrs['stop_date'],
+                                                                             "%Y-%m-%d %H:%M:%S").strftime(
+            "%Y-%m-%dT%H:%M:%SZ")
+    xr_dataset.attrs["clmSource"] = "/"
+    xr_dataset.attrs["bathySource"] = "/"
+    xr_dataset.attrs['oswAlgorithmName'] = 'grdwindinversion'
+    xr_dataset.attrs["owiAlgorithmVersion"] = grdwindinversion.__version__
+    xr_dataset.attrs["gmf"] = config['GMF_'+copol_gmf+'_NAME'] + \
+        ", " + config["GMF_"+crosspol_gmf+"_NAME"]
+    xr_dataset.attrs["iceSource"] = "/"
+    xr_dataset.attrs["owiNoiseCorrection"] = "False"
+    xr_dataset.attrs["inversionTabGMF"] = config['GMF_'+copol_gmf +
+                                                 '_NAME'] + ", " + config["GMF_"+crosspol_gmf+"_NAME"]
+    xr_dataset.attrs["wnf_3km_average"] = "/"
+    xr_dataset.attrs["owiWindSpeedSrc"] = "owiWindSpeed"
+    xr_dataset.attrs["owiWindDirectionSrc"] = "/"
 
-            
     table_fillValue = {
         "owiWindQuality": -1,
         "owiHeading": 9999.99,
         "owiWindDirection_IPF": -9999.0,
         "owiWindSpeed_IPF": -9999.0,
         "owiWindDirection": -9999.0,
         "owiPBright": 999.99,
         "owiWindFilter": -1,
         "owiWindSpeed": -9999.0,
         "owiWindSpeed_co": -9999.0,
         "owiWindSpeed_cross": -9999.0,
     }
-    
+
     encoding = {}
     for var in list(set(xr_dataset.coords.keys()) | set(xr_dataset.keys())):
         encoding[var] = {}
         try:
-            # sarwing_ds[var].attrs["_FillValue"] = table_fillValue[var]
             encoding[var].update({'_FillValue': table_fillValue[var]})
         except:
-            # Nouvelles variables..
             if (var in ["owiWindSpeed_co", "owiWindSpeed_cross", "owiWindSpeed"]):
-                # sarwing_ds[var].attrs["_FillValue"] = -9999.0
                 encoding[var].update({'_FillValue': -9999.0})
             else:
                 encoding[var].update({'_FillValue': None})
 
     xr_dataset.attrs["xsar_version"] = xsar.__version__
     xr_dataset.attrs["xsarsea_version"] = xsarsea.__version__
-    
+
     return xr_dataset, encoding
 
 
 def makeL2(filename, out_folder, config_path, overwrite=False, generateCSV=True, resolution='1000m'):
     """
+    Main function to generate L2 product.
 
-    :param filename: str
-    :param out_folder: str
-    :param config_path: str
-    :param overwrite: bool True -> existing files will be overwritten
-    :return:
-     out_file: str
-     xr_dataset: xarray.Dataset final dataset with wind speed variables
+    Parameters
+    ----------
+    filename : str
+        input filename
+    out_folder : str
+        output folder
+    config_path : str
+        configuration file path
+    overwrite : bool, optional
+        overwrite existing file
+    generateCSV : bool, optional
+        generate CSV file
+    resolution : str, optional
+        working resolution
+
+    Returns
+    -------
+    str
+        output filename
+    xarray.Dataset
+        final dataset
     """
 
-    # final xr.Dataset
-
-    #  Step 1 - load L1 product
-
     sensor, sensor_longname, fct_meta, fct_dataset = getSensorMetaDataset(
         filename)
 
     if Path(config_path).exists():
         config = yaml.load(
             Path(config_path).open(),
             Loader=yaml.FullLoader
@@ -444,66 +544,73 @@
         try:
             config = config[sensor]
         except Exception:
             raise KeyError("sensor %s not in this config" % sensor)
     else:
         raise FileNotFoundError(
             'config_path do not exists, got %s ' % config_path)
-    
+
     recalibration = config["recalibration"]
-    if recalibration:
-        aux_config_name=config["aux_config_name"]
-    
     meta = fct_meta(filename)
     out_file = getOutputName2(filename, out_folder, sensor, meta)
 
-    
     if os.path.exists(out_file) and overwrite is False:
-        logging.info("out_file %s exists" % out_file)
+        logging.info("out_file %s exists ; returning empty Dataset" % out_file)
         return out_file, xr.Dataset()
 
-    # get ancillary wind from ECMWF
-    map_model = getAncillary(meta)
+    map_model = getAncillary(meta, ancillary_name=config["ancillary"])
     if map_model is None:
         raise Exception(
             'the weather model is not set `map_model` is None -> you probably don"t have access to ECMWF archive')
 
     try:
         if ((recalibration) & ("SENTINEL" in sensor_longname)):
-            logging.info('recalibration is True : Kersten formula is applied')
+            logging.info(
+                f'recalibration is {recalibration} : Kersten formula is applied')
             xsar_dataset = fct_dataset(
-                meta, resolution=resolution, recalibration=recalibration, aux_config_name = aux_config_name)
+                meta, resolution=resolution, recalibration=recalibration)
             xr_dataset = xsar_dataset.datatree['measurement'].to_dataset()
-            xr_dataset = xr_dataset.merge(xsar_dataset.datatree["recalibration"].to_dataset()[['swath_number','swath_number_flag','sigma0_raw__corrected']])
-  
+            xr_dataset = xr_dataset.merge(xsar_dataset.datatree["recalibration"].to_dataset()[
+                                          ['swath_number', 'swath_number_flag', 'sigma0_raw__corrected']])
+
         else:
             logging.info(
-                'recalibration is True : Kersten formula is not applied')
+                f'recalibration is {recalibration} : Kersten formula is not applied')
             if ("SENTINEL" in sensor_longname):
-                xsar_dataset = fct_dataset(meta, resolution=resolution,recalibration=recalibration)
+                xsar_dataset = fct_dataset(
+                    meta, resolution=resolution, recalibration=recalibration)
                 xr_dataset = xsar_dataset.datatree['measurement'].to_dataset()
-                xr_dataset = xr_dataset.merge(xsar_dataset.datatree["recalibration"].to_dataset()[['swath_number','swath_number_flag']])
+                xr_dataset = xr_dataset.merge(xsar_dataset.datatree["recalibration"].to_dataset()[
+                                              ['swath_number', 'swath_number_flag']])
 
-            else: 
+            else:
                 xsar_dataset = fct_dataset(meta, resolution=resolution)
                 xr_dataset = xsar_dataset.datatree['measurement'].to_dataset()
 
-                
         xr_dataset = xr_dataset.rename(map_model)
         # add attributes
         xr_dataset.attrs = xsar_dataset.dataset.attrs
         xr_dataset.attrs['L1_path'] = xr_dataset.attrs.pop('name')
         xr_dataset.attrs["sourceProduct"] = sensor
         xr_dataset.attrs["missionName"] = sensor_longname
-        
+        if ((recalibration) & ("SENTINEL" in sensor_longname)):
+            xr_dataset.attrs["path_aux_pp1_new"] = os.path.basename(os.path.dirname(
+                os.path.dirname(xsar_dataset.datatree['recalibration'].attrs['path_aux_pp1_new'])))
+            xr_dataset.attrs["path_aux_cal_new"] = os.path.basename(os.path.dirname(
+                os.path.dirname(xsar_dataset.datatree['recalibration'].attrs['path_aux_cal_new'])))
+
+            xr_dataset.attrs["path_aux_pp1_old"] = os.path.basename(os.path.dirname(
+                os.path.dirname(xsar_dataset.datatree['recalibration'].attrs['path_aux_pp1_old'])))
+            xr_dataset.attrs["path_aux_cal_old"] = os.path.basename(os.path.dirname(
+                os.path.dirname(xsar_dataset.datatree['recalibration'].attrs['path_aux_cal_old'])))
+
     except Exception as e:
         logging.info('%s', traceback.format_exc())
         logging.error(e)
         sys.exit(-1)
-    
 
     # defining dual_pol, and gmfs by channel
     if len(xr_dataset.pol.values) == 2:
         dual_pol = True
     else:
         dual_pol = False
 
@@ -549,29 +656,51 @@
     xr_dataset.mask.attrs = {}
     xr_dataset.mask.attrs['long_name'] = 'Mask of data'
     xr_dataset.mask.attrs['valid_range'] = np.array([0, 3])
     xr_dataset.mask.attrs['flag_values'] = np.array([0, 1, 2, 3])
     xr_dataset.mask.attrs['flag_meanings'] = 'valid land ice no_valid'
 
     # ANCILLARY
-    xr_dataset['ancillary_wind'] = (xr_dataset.model_U10 + 1j * xr_dataset.model_V10) * np.exp(
-        1j * np.deg2rad(xr_dataset.ground_heading))
+    xr_dataset['ancillary_wind_direction'] = (
+        90. - np.rad2deg(np.arctan2(xr_dataset.model_V10, xr_dataset.model_U10)) + 180) % 360
+
+    xr_dataset['ancillary_wind_direction'] = xr.where(xr_dataset['mask'], np.nan,
+                                                      xr_dataset['ancillary_wind_direction'].compute()).transpose(
+        *xr_dataset['ancillary_wind_direction'].dims)
+    xr_dataset['ancillary_wind_direction'].attrs = {}
+    xr_dataset['ancillary_wind_direction'].attrs['units'] = 'degrees_north'
+    xr_dataset['ancillary_wind_direction'].attrs[
+        'long_name'] = 'ECMWF Wind direction (meteorological convention)'
+    xr_dataset['ancillary_wind_direction'].attrs['standart_name'] = 'wind_direction'
+
+    xr_dataset['ancillary_wind_speed'] = np.sqrt(
+        xr_dataset['model_U10']**2+xr_dataset['model_V10']**2)
+    xr_dataset['ancillary_wind_speed'] = xr.where(xr_dataset['mask'], np.nan,
+                                                  xr_dataset['ancillary_wind_speed'].compute()).transpose(
+        *xr_dataset['ancillary_wind_speed'].dims)
+    xr_dataset['ancillary_wind_speed'].attrs = {}
+    xr_dataset['ancillary_wind_speed'].attrs['units'] = 'm s^-1'
+    xr_dataset['ancillary_wind_speed'].attrs[
+        'long_name'] = 'ECMWF Wind speed'
+    xr_dataset['ancillary_wind_speed'].attrs['standart_name'] = 'wind_speed'
+
     xr_dataset['ancillary_wind'] = xr.where(xr_dataset['mask'], np.nan,
-                                            xr_dataset['ancillary_wind'].compute()).transpose(
-        *xr_dataset['ancillary_wind'].dims)
+                                            (xr_dataset.ancillary_wind_speed * np.exp(1j * xsarsea.dir_geo_to_sample(xr_dataset.ancillary_wind_direction, xr_dataset.ground_heading))).compute()).transpose(
+        *xr_dataset['ancillary_wind_speed'].dims)
+
     xr_dataset.attrs['ancillary_source'] = xr_dataset['model_U10'].attrs['history'].split('decoded: ')[
         1].strip()
     xr_dataset = xr_dataset.drop_vars(['model_U10', 'model_V10'])
 
     # NRCS & NESZ
     xr_dataset['sigma0_ocean'] = xr.where(xr_dataset['mask'], np.nan,
                                           xr_dataset['sigma0'].compute()).transpose(*xr_dataset['sigma0'].dims)
     xr_dataset['sigma0_ocean'] = xr.where(
         xr_dataset['sigma0_ocean'] <= 0, np.nan, xr_dataset['sigma0_ocean'])
-    
+
     xr_dataset['sigma0_ocean'].attrs = xr_dataset['sigma0'].attrs
 
     xr_dataset['sigma0_ocean_raw'] = xr.where(xr_dataset['mask'], np.nan,
                                               xr_dataset['sigma0_raw'].compute()).transpose(*xr_dataset['sigma0_raw'].dims)
     xr_dataset['sigma0_ocean_raw'] = xr.where(
         xr_dataset['sigma0_ocean_raw'] <= 0, np.nan, xr_dataset['sigma0_ocean_raw'])
     xr_dataset['sigma0_ocean_raw'].attrs = xr_dataset['sigma0_raw'].attrs
@@ -596,34 +725,45 @@
 
         xr_dataset.dsig_cross.attrs['comment'] = 'variable used to ponderate copol and crosspol'
         dsig_cross = xr_dataset.dsig_cross
     else:
         sigma0_ocean_cross = None
         dsig_cross = 0.1  # default value set in xsarsea
 
-    windspeed_co, windspeed_dual, windspeed_cr = inverse(dual_pol,
-                                                    inc=xr_dataset.incidence,
-                                                    sigma0=xr_dataset['sigma0_ocean'].sel(
-                                                        pol=copol),
-                                                    sigma0_dual=sigma0_ocean_cross,
-                                                    ancillary_wind=xr_dataset['ancillary_wind'],
-                                                    dsig_cr=dsig_cross,
-                                                    model_vv=config["GMF_" +
-                                                                    copol_gmf+"_NAME"],
-                                                    model_vh=config["GMF_"+crosspol_gmf+"_NAME"])
+    wind_co, wind_dual, windspeed_cr = inverse(dual_pol,
+                                               inc=xr_dataset.incidence,
+                                               sigma0=xr_dataset['sigma0_ocean'].sel(
+                                                   pol=copol),
+                                               sigma0_dual=sigma0_ocean_cross,
+                                               ancillary_wind=xr_dataset['ancillary_wind'],
+                                               dsig_cr=dsig_cross,
+                                               model_vv=config["GMF_" +
+                                                               copol_gmf+"_NAME"],
+                                               model_vh=config["GMF_"+crosspol_gmf+"_NAME"])
+
+    #  get windspeeds
+    xr_dataset['windspeed_co'] = np.abs(wind_co)
+    xr_dataset['windspeed_dual'] = np.abs(wind_dual)
 
-    xr_dataset['windspeed_co']  = windspeed_co
-    xr_dataset['windspeed_dual'] = windspeed_dual
     if dual_pol:
         xr_dataset = xr_dataset.assign(
             windspeed_cross=(['line', 'sample'], windspeed_cr))
-    else : 
+    else:
         xr_dataset['windspeed_cross'] = windspeed_cr
 
-    xr_dataset, encoding = makeL2asOwi(xr_dataset, dual_pol, copol, crosspol, copol_gmf, crosspol_gmf, config)
+    #  get winddirections
+    xr_dataset['winddir_co'] = (
+        90 - (np.angle(-np.conj(wind_co), deg=True)) + xr_dataset.ground_heading) % 360
+
+    xr_dataset['winddir_dual'] = (
+        90 - (np.angle(-np.conj(wind_dual), deg=True)) + xr_dataset.ground_heading) % 360
+    xr_dataset['winddir_cross'] = xr_dataset['winddir_dual'].copy()
+
+    xr_dataset, encoding = makeL2asOwi(
+        xr_dataset, dual_pol, copol, crosspol, copol_gmf, crosspol_gmf, config)
 
     os.makedirs(os.path.dirname(out_file), exist_ok=True)
 
     xr_dataset.to_netcdf(out_file, mode="w", encoding=encoding)
     if generateCSV:
         df = xr_dataset.to_dataframe()
         df = df[df.owiMask == False]
```

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/load_config.py` & `grdwindinversion-0.2.3.post8/grdwindinversion/load_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from yaml import load
 import logging
 import os
 import grdwindinversion
 from yaml import CLoader as Loader
-local_config_potential_path = os.path.join(os.path.dirname(grdwindinversion.__file__), 'local_data_config.yaml')
+local_config_potential_path = os.path.expanduser(
+    '~/.grdwindinversion/data_config.yaml')
 
 if os.path.exists(local_config_potential_path):
-   config_path = local_config_potential_path
+    config_path = local_config_potential_path
 else:
-   config_path = os.path.join(os.path.dirname(grdwindinversion.__file__), 'data_config.yaml')
-# config_path = "./data_config.yaml"
-logging.info('config path: %s',config_path)
+    config_path = os.path.join(os.path.dirname(
+        grdwindinversion.__file__), 'data_config.yaml')
+logging.info('config path: %s', config_path)
 stream = open(config_path, 'r')
 conf = load(stream, Loader=Loader)
-def getConf():
 
+
+def getConf():
     """
-    if grdwindinversion/local_data_config.yaml exists it will superseed grdwindinversion/data_config.yaml
+    if local_config_potential_path exists it will superseed config_path
     :return:
     """
     return conf
```

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/main.py` & `grdwindinversion-0.2.3.post8/grdwindinversion/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     import argparse, os
     from pathlib import Path
 
     parser = argparse.ArgumentParser(
         description='Perform inversion from S1(L1-GRD) SAFE, L1-RCM, L1-RS2 ; using xsar/xsarsea tools')
     parser.add_argument('--input_file', help='input file path', required=True)
     parser.add_argument('--config_file',
-                        help='config file path [if not provided will take config file based on input file]',required=False)
+                        help='config file path [if not provided will take config file based on input file]',required=True)
                         
     parser.add_argument('--resolution',required=False, default='1000m', help='set resolution ["full" | "1000m" | "xXxm"]')
      
     parser.add_argument('--outputdir', required=True)
     parser.add_argument('--verbose', action='store_true', default=False)
     parser.add_argument('--overwrite', action='store_true', default=False,
                         help='overwrite existing .nc files [default is False]', required=False)
@@ -39,29 +39,16 @@
     
     
     # if '1SDV' not in input_file and '_VV_VH' not in input_file:
     #     raise Exception('this processor only handle dual polarization acquisitions VV+VH for now.')
     # if '1SSH' in input_file or '1SDH' in input_file or '_HH_HV' in input_file:
     #     raise Exception('this processor only handle acquisitions with VV or VV+VH polarization for now.')
     
-    if args.config_file is None:
-        if 'S1' in input_file:
-            config_file = os.path.join(os.path.dirname(grdwindinversion.__file__),'config_S1.yaml')
-        elif 'RCM' in input_file:
-            config_file = os.path.join(os.path.dirname(grdwindinversion.__file__),'config_RCM.yaml')
-        elif 'RS2' in input_file:
-            config_file = os.path.join(os.path.dirname(grdwindinversion.__file__),'config_RS2.yaml')
-        elif 'hy2b' in input_file:
-            config_file = os.path.join(os.path.dirname(grdwindinversion.__file__),'config_hy2b.yaml')
-        else:
-            raise Exception('config data file cannot be defined using the input filename')
-    else:
-        config_file = args.config_file
-        
-    
+
+    config_file = args.config_file     
     out_folder = args.outputdir
     resolution = args.resolution
     if resolution == "full":
         resolution = None
     
     out_file,outputds = makeL2(input_file, out_folder, config_file, overwrite=args.overwrite,resolution = resolution, generateCSV = args.no_generate_csv)
     logging.info('out_file: %s', out_file)
```

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion/utils.py` & `grdwindinversion-0.2.3.post8/grdwindinversion/utils.py`

 * *Files identical despite different names*

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/PKG-INFO` & `grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grdwindinversion
-Version: 0.2.3.post7
+Version: 0.2.3.post8
 Summary: Package to perform Wind inversion from GRD Level-1 SAR images
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `grdwindinversion-0.2.3.post7/grdwindinversion.egg-info/SOURCES.txt` & `grdwindinversion-0.2.3.post8/grdwindinversion.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,18 +29,14 @@
 docs/readme.rst
 docs/usage.rst
 docs/_static/css/grdwindinversion.css
 docs/examples/wind-inversion-from-grd.ipynb
 grdwindinversion/.gitignore
 grdwindinversion/.travis.yml
 grdwindinversion/__init__.py
-grdwindinversion/config_RCM.yaml
-grdwindinversion/config_RS2.yaml
-grdwindinversion/config_S1.yaml
-grdwindinversion/config_hy2b.yaml
 grdwindinversion/config_prod.yaml
 grdwindinversion/config_prod_recal.yaml
 grdwindinversion/data_config.yaml
 grdwindinversion/inversion.py
 grdwindinversion/load_config.py
 grdwindinversion/main.py
 grdwindinversion/utils.py
```

### Comparing `grdwindinversion-0.2.3.post7/pyproject.toml` & `grdwindinversion-0.2.3.post8/pyproject.toml`

 * *Files identical despite different names*

