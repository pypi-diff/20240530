# Comparing `tmp/hysetter-0.1.0.tar.gz` & `tmp/hysetter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hysetter-0.1.0.tar", last modified: Mon May 20 22:27:44 2024, max compression
+gzip compressed data, was "hysetter-0.1.1.tar", last modified: Thu May 30 12:39:42 2024, max compression
```

## Comparing `hysetter-0.1.0.tar` & `hysetter-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.949678 hysetter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 22:27:34.000000 hysetter-0.1.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 22:27:34.000000 hysetter-0.1.0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 22:27:34.000000 hysetter-0.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 22:27:34.000000 hysetter-0.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.945678 hysetter-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.945678 hysetter-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.945678 hysetter-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-20 22:27:34.000000 hysetter-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-20 22:27:34.000000 hysetter-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 22:27:34.000000 hysetter-0.1.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-20 22:27:34.000000 hysetter-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 22:27:34.000000 hysetter-0.1.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 22:27:34.000000 hysetter-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 22:27:34.000000 hysetter-0.1.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-20 22:27:34.000000 hysetter-0.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-20 22:27:34.000000 hysetter-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 22:27:34.000000 hysetter-0.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 22:27:34.000000 hysetter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 22:27:34.000000 hysetter-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-20 22:27:44.949678 hysetter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-20 22:27:34.000000 hysetter-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.937678 hysetter-0.1.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.945678 hysetter-0.1.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-20 22:27:34.000000 hysetter-0.1.0/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 22:27:34.000000 hysetter-0.1.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-20 22:27:34.000000 hysetter-0.1.0/config_demo.yml
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 22:27:34.000000 hysetter-0.1.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)   349263 2024-05-20 22:27:34.000000 hysetter-0.1.0/hs_demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-20 22:27:34.000000 hysetter-0.1.0/hs_help.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.949678 hysetter-0.1.0/hysetter/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/forcing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/hysetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/nid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/nlcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/nwis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/soil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-20 22:27:34.000000 hysetter-0.1.0/hysetter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.949678 hysetter-0.1.0/hysetter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 22:27:44.000000 hysetter-0.1.0/hysetter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-20 22:27:34.000000 hysetter-0.1.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-20 22:27:34.000000 hysetter-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:27:44.949678 hysetter-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:27:44.949678 hysetter-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-20 22:27:34.000000 hysetter-0.1.0/tests/test_hysetter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:42.007696 hysetter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 12:39:31.000000 hysetter-0.1.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 12:39:31.000000 hysetter-0.1.1/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 12:39:31.000000 hysetter-0.1.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 12:39:31.000000 hysetter-0.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:41.999695 hysetter-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:41.999695 hysetter-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:42.003696 hysetter-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-30 12:39:31.000000 hysetter-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-30 12:39:31.000000 hysetter-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 12:39:31.000000 hysetter-0.1.1/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-30 12:39:31.000000 hysetter-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 12:39:31.000000 hysetter-0.1.1/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 12:39:31.000000 hysetter-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-30 12:39:31.000000 hysetter-0.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-30 12:39:31.000000 hysetter-0.1.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-30 12:39:31.000000 hysetter-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-30 12:39:31.000000 hysetter-0.1.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 12:39:31.000000 hysetter-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 12:39:31.000000 hysetter-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-30 12:39:42.007696 hysetter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-30 12:39:31.000000 hysetter-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:41.995695 hysetter-0.1.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:42.003696 hysetter-0.1.1/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-30 12:39:31.000000 hysetter-0.1.1/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 12:39:31.000000 hysetter-0.1.1/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-30 12:39:31.000000 hysetter-0.1.1/config_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 12:39:31.000000 hysetter-0.1.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-05-30 12:39:31.000000 hysetter-0.1.1/hs_help.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:42.003696 hysetter-0.1.1/hysetter/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/hysetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/nid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/nlcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/soil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-30 12:39:31.000000 hysetter-0.1.1/hysetter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:42.007696 hysetter-0.1.1/hysetter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 12:39:41.000000 hysetter-0.1.1/hysetter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-30 12:39:31.000000 hysetter-0.1.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-30 12:39:31.000000 hysetter-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 12:39:42.007696 hysetter-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 12:39:42.007696 hysetter-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 12:39:31.000000 hysetter-0.1.1/tests/test_hysetter.py
```

### Comparing `hysetter-0.1.0/.github/ISSUE_TEMPLATE/bugreport.yml` & `hysetter-0.1.1/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/.github/ISSUE_TEMPLATE/newfeature.yml` & `hysetter-0.1.1/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/.github/workflows/codeql-analysis.yml` & `hysetter-0.1.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/.github/workflows/release.yml` & `hysetter-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/.github/workflows/test.yml` & `hysetter-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/.gitignore` & `hysetter-0.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -99,13 +99,14 @@
 /site
 
 # mypy
 .mypy_cache/
 
 # IDE settings
 .vscode/
+.idea/
 
 # logs
 .nvimlog
 data/
 tags*
 cache
```

### Comparing `hysetter-0.1.0/.pre-commit-config.yaml` & `hysetter-0.1.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   hooks:
   - id: blacken-docs
     name: Autoformat codes in docstrings with blacken-docs
     additional_dependencies: [black]
     args: [-t, py38, -l, '100']
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.4
+  rev: v0.4.6
   hooks:
   - id: ruff
     name: Linting with Ruff
     types_or: [python]
     args: [--fix, --unsafe-fixes]
   - id: ruff-format
     name: Formatting with Ruff
@@ -35,15 +35,15 @@
   rev: v1.1.1
   hooks:
   - id: doc8
     name: Check documentation formats with doc8
     args: [--max-line-length, '100']
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.6
+  rev: v2.3.0
   hooks:
   - id: codespell
     name: Check common misspellings in text files with codespell.
     additional_dependencies:
     - tomli
 
 - repo: https://github.com/dosisod/refurb
@@ -51,15 +51,15 @@
   hooks:
   - id: refurb
     name: Modernizing Python codebases using Refurb
     additional_dependencies:
     - numpy
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 2.1.1
+  rev: 2.1.3
   hooks:
   - id: pyproject-fmt
     name: Apply a consistent format to pyproject.toml
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.6.0
   hooks:
@@ -91,12 +91,12 @@
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
   rev: v2.13.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
 
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.7.0
+  rev: v1.7.1
   hooks:
   - id: actionlint
     files: .github/workflows/
     args: [-ignore, SC1090, -ignore, SC2046, -ignore, SC2086, -ignore, SC2129, -ignore, SC2155]
```

### Comparing `hysetter-0.1.0/CITATION.cff` & `hysetter-0.1.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/CODE_OF_CONDUCT.rst` & `hysetter-0.1.1/CODE_OF_CONDUCT.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ----------
 
 In the interest of fostering an open and welcoming environment, we as
 contributors and maintainers pledge to making participation in our
 project and our community a harassment-free experience for everyone,
 regardless of age, body size, disability, ethnicity, sex
 characteristics, gender identity and expression, level of experience,
-education, socio-economic status, nationality, personal appearance,
+education, socioeconomic status, nationality, personal appearance,
 race, religion, or sexual identity and orientation.
 
 Our Standards
 -------------
 
 Examples of behavior that contributes to creating a positive environment
 include:
```

### Comparing `hysetter-0.1.0/CONTRIBUTING.rst` & `hysetter-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/LICENSE` & `hysetter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/PKG-INFO` & `hysetter-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysetter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Subset hydroclimate data using HyRiver Over CONUS.
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/hysetter.html
 Project-URL: CI, https://github.com/hyriver/hysetter/actions
 Project-URL: Homepage, https://docs.hyriver.io/readme/hysetter.html
 Project-URL: Issues, https://github.com/hyriver/hysetter/issues
@@ -21,35 +21,36 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: async-retriever>=0.16.1
+Requires-Dist: boto3
+Requires-Dist: dask[dataframe]
 Requires-Dist: flox
-Requires-Dist: hydrosignatures>=0.16
+Requires-Dist: geopandas
 Requires-Dist: numba
 Requires-Dist: numbagg
+Requires-Dist: pandas
 Requires-Dist: planetary-computer
 Requires-Dist: py3dep>=0.16.3
-Requires-Dist: py7zr
-Requires-Dist: pydantic
+Requires-Dist: pyarrow>=1.0.1
+Requires-Dist: pydantic>=2.7.1
 Requires-Dist: pydaymet>=0.16.3
-Requires-Dist: pygeohydro>=0.16.3
-Requires-Dist: pygeoogc>=0.16.3
-Requires-Dist: pygeoutils>=0.16.3
+Requires-Dist: pygeohydro>=0.16.4
 Requires-Dist: pygridmet>=0.16
 Requires-Dist: pynhd>=0.16.3
 Requires-Dist: pynldas2>=0.16
 Requires-Dist: pyogrio
 Requires-Dist: pystac-client
 Requires-Dist: pyyaml
-Requires-Dist: rich-click
+Requires-Dist: rich-click>=1.8.2
 Requires-Dist: typing-extensions
+Requires-Dist: xarray>=2024.5
 Requires-Dist: xarray-spatial
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-xdist[psutil]; extra == "test"
 
 HySetter: Hyroclimate Data Subsetter based on HyRiver
@@ -100,15 +101,17 @@
 
 HySetter is an open-source Python package, built on HyRiver software stack, that provides a
 command-line interface (CLI) for subsetting hydroclimate data from the following data sources
 over conterminous United States (CONUS):
 
 - **Area Of Interest**: From any `HUC <https://www.usgs.gov/national-hydrography/watershed-boundary-dataset>`__
   level, `GAGES-II basins <https://pubs.usgs.gov/publication/70046617>`__,
-  `NHDPlusV2 <https://www.nhdplus.com/NHDPlus/NHDPlusV2_home.php>`__ catchments,
+  `NHDPlusV2 <https://www.nhdplus.com/NHDPlus/NHDPlusV2_home.php>`__ catchments and their
+  attributes (`StreamCat <https://www.epa.gov/national-aquatic-resource-surveys/streamcat-dataset>`__
+  and `NLDI <https://labs.waterdata.usgs.gov/docs/nldi/about-nldi/index.html>`__),
   or a user-defined GeoDataFrame
 - **Drainage Network**: From NHDPlusV2
 - **Forcing**: From `Daymet <https://daymet.ornl.gov/>`__,
   `GridMET <https://www.climatologylab.org/gridmet.html>`__,
   or `NLDAS2 <https://ldas.gsfc.nasa.gov/nldas/v2/forcing>`__
 - **Streamflow**: From `NWIS <https://nwis.waterdata.usgs.gov/nwis>`__
 - **Soil**: From `gNATSGO <https://planetarycomputer.microsoft.com/dataset/gnatsgo-rasters>`__,
@@ -160,15 +163,16 @@
 source, the area of interest (AOI), and the output directory. You can find an example
 configuration file in the
 `config_demo.yml <https://github.com/hyriver/hysetter/blob/main/config_demo.yml>`__.
 
 .. image:: https://raw.githubusercontent.com/hyriver/hysetter/main/hs_help.svg
     :align: center
 
-.. image:: https://raw.githubusercontent.com/hyriver/hysetter/main/hs_demo.gif
+.. image:: https://asciinema.org/a/660577.svg
+    :target: https://asciinema.org/a/660577?autoplay=1
     :align: center
 
 Contributing
 ------------
 Contributions are appreciated and very welcomed. Please read
 `CONTRIBUTING.rst <https://github.com/hyriver/hysetter/blob/main/CONTRIBUTING.rst>`__
 for instructions.
```

### Comparing `hysetter-0.1.0/README.rst` & `hysetter-0.1.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 
 HySetter is an open-source Python package, built on HyRiver software stack, that provides a
 command-line interface (CLI) for subsetting hydroclimate data from the following data sources
 over conterminous United States (CONUS):
 
 - **Area Of Interest**: From any `HUC <https://www.usgs.gov/national-hydrography/watershed-boundary-dataset>`__
   level, `GAGES-II basins <https://pubs.usgs.gov/publication/70046617>`__,
-  `NHDPlusV2 <https://www.nhdplus.com/NHDPlus/NHDPlusV2_home.php>`__ catchments,
+  `NHDPlusV2 <https://www.nhdplus.com/NHDPlus/NHDPlusV2_home.php>`__ catchments and their
+  attributes (`StreamCat <https://www.epa.gov/national-aquatic-resource-surveys/streamcat-dataset>`__
+  and `NLDI <https://labs.waterdata.usgs.gov/docs/nldi/about-nldi/index.html>`__),
   or a user-defined GeoDataFrame
 - **Drainage Network**: From NHDPlusV2
 - **Forcing**: From `Daymet <https://daymet.ornl.gov/>`__,
   `GridMET <https://www.climatologylab.org/gridmet.html>`__,
   or `NLDAS2 <https://ldas.gsfc.nasa.gov/nldas/v2/forcing>`__
 - **Streamflow**: From `NWIS <https://nwis.waterdata.usgs.gov/nwis>`__
 - **Soil**: From `gNATSGO <https://planetarycomputer.microsoft.com/dataset/gnatsgo-rasters>`__,
@@ -106,15 +108,16 @@
 source, the area of interest (AOI), and the output directory. You can find an example
 configuration file in the
 `config_demo.yml <https://github.com/hyriver/hysetter/blob/main/config_demo.yml>`__.
 
 .. image:: https://raw.githubusercontent.com/hyriver/hysetter/main/hs_help.svg
     :align: center
 
-.. image:: https://raw.githubusercontent.com/hyriver/hysetter/main/hs_demo.gif
+.. image:: https://asciinema.org/a/660577.svg
+    :target: https://asciinema.org/a/660577?autoplay=1
     :align: center
 
 Contributing
 ------------
 Contributions are appreciated and very welcomed. Please read
 `CONTRIBUTING.rst <https://github.com/hyriver/hysetter/blob/main/CONTRIBUTING.rst>`__
 for instructions.
```

### Comparing `hysetter-0.1.0/ci/requirements/environment-dev.yml` & `hysetter-0.1.1/ci/requirements/environment-dev.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - pygeoutils >=0.16.3
 - py3dep >=0.16.3
 - pynhd >=0.16.3
 - pygridmet >=0.16
 - pydaymet >=0.16.3
 - hydrosignatures >=0.16
 - pynldas2 >=0.16
-- pygeohydro >=0.16.3
+- pygeohydro >=0.16.4
 # performance
 - flox
 - numba
 - numbagg
 # config
 - pydantic
 - pyyaml
@@ -32,15 +32,15 @@
 - xarray-spatial
 # soil
 - pystac-client
 - planetary-computer
 - dask-expr
 - boto3
 # nhdplus
-# - py7zr
+- py7zr
 
 # dev deps
 - ipywidgets
 - ipykernel
 - codespell
 - tomli
 - nox
```

### Comparing `hysetter-0.1.0/ci/requirements/environment.yml` & `hysetter-0.1.1/ci/requirements/environment.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - pygeoutils >=0.16.3
 - py3dep >=0.16.3
 - pynhd >=0.16.3
 - pygridmet >=0.16
 - pydaymet >=0.16.3
 - hydrosignatures >=0.16
 - pynldas2 >=0.16
-- pygeohydro >=0.16.3
+- pygeohydro >=0.16.4
 # performance
 - flox
 - numba
 - numbagg
 # config
 - pydantic
 - pyyaml
@@ -31,15 +31,15 @@
 - xarray-spatial
 # soil
 - pystac-client
 - planetary-computer
 - dask-expr
 - boto3
 # nhdplus
-# - py7zr
+- py7zr
 
 # dev deps
 - psutil
 - pytest-cov
 - pytest-xdist
 - pytest-sugar
```

### Comparing `hysetter-0.1.0/config_demo.yml` & `hysetter-0.1.1/config_demo.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # Only `project` and `aoi` are required, the rest are optional
 project:
   # Data will be stored in `data_dir/name`
   name: example_1
   data_dir: data
 aoi:
+  # Only one of `huc_ids`, `nhdv2_ids`, `gagesii_basins`, or `geometry_file`
+  # should be given.
   # Could be a mix of different HUC levels
   huc_ids: []
   # NHDPlusV2 catchment IDs (featureid)
   nhdv2_ids: []
   # GAGES-II basin ID
   gagesii_basins: ['01031500', '01031450']
-  # Could be paruqet, feather or anything that geopandas.read_file acceps
+  # Could be paruqet, feather or anything that geopandas.read_file accepts
   geometry_file: ''
   # Whether to get NHDPlusV2 flowlines within AOI.
   # Flowlines for each geometry (row) in the AOI will be saved to a
   # subdirectory called data_dir/nhdv2_flowlines. The files are named
   # with this pattern `aio_geom_X.parquet` where `X` is the row number
   # in the AOI GeoDataFrame.
   nhdv2_flowlines: true
+  # A list of valid StreamCat attributes to get for flowlines within AOI.
+  # You can use `pynhd.streamcat()` to get a dataframe of the attrs'
+  # names and descriptions
+  streamcat_attrs: [fert, bfi]
+  # A list of valid NLDI attributes to get for flowlines within AOI.
+  # You can use `pynhd.nhdplus_attrs_s3()` to get a dataframe of the attrs'
+  # names and descriptions
+  nldi_attrs: [CAT_BFI, CAT_PET]
 forcing:
   # Could be `daymet`, `gridmet`, or `nldas2`
   source: daymet
   start_date: 2000-01-01
   end_date: 2000-01-02
   # Valid variable names depend on the source
   variables: [prcp, tmin]
```

### Comparing `hysetter-0.1.0/hs_help.svg` & `hysetter-0.1.1/hs_help.svg`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/hysetter/__init__.py` & `hysetter-0.1.1/hysetter/__init__.py`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/hysetter/cli.py` & `hysetter-0.1.1/hysetter/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,32 +8,35 @@
 from pathlib import Path
 
 import rich_click as click
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
-from . import aoi, forcing, nid, nlcd, nwis, soil, topo
 from . import hysetter as hs
 
 console = Console()
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
 
 def get_versions() -> dict[str, str]:
     """Get the versions of the dependencies."""
 
     def _get_version(module: str) -> str:
+        """Get the version of the module."""
         try:
             return importlib.metadata.version(module)
         except importlib.metadata.PackageNotFoundError:
             return "not installed"
 
+    hs_ver = _get_version("hysetter")
+    if "dev" in hs_ver:
+        hs_ver = ".".join(hs_ver.split(".")[:3]) + "-dev"
     return {
-        "HySetter": _get_version("hysetter"),
+        "HySetter": hs_ver,
         "HyRiver Stack": ".".join(_get_version("pygeohydro").split(".")[:2]),
         "Python": ".".join(map(str, sys.version_info[:3])),
     }
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("config_yml", type=click.Path(exists=True))
@@ -63,17 +66,11 @@
     console.print(f"Reading configuration file: [bold green]{Path(config_yml).resolve()}")
     cfg = hs.read_config(config_yml)
 
     if overwrite:
         console.print("Removing existing data")
         shutil.rmtree(cfg.project.data_dir, ignore_errors=True)
     try:
-        aoi.get_aoi(cfg)
-        forcing.get_forcing(cfg)
-        topo.get_topo(cfg)
-        soil.get_soil(cfg)
-        nlcd.get_nlcd(cfg)
-        nid.get_nid(cfg)
-        nwis.get_streamflow(cfg)
+        cfg.get_data()
     except Exception:
-        console.print_exception(extra_lines=8, show_locals=True)
+        console.print_exception(extra_lines=3, show_locals=True)
         sys.exit(1)
```

### Comparing `hysetter-0.1.0/hysetter/exceptions.py` & `hysetter-0.1.1/hysetter/exceptions.py`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/hysetter/hysetter.py` & `hysetter-0.1.1/hysetter/hysetter.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,64 @@
 
 from __future__ import annotations
 
 import functools
 from dataclasses import dataclass
 from datetime import datetime  # noqa: TCH003
 from pathlib import Path
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
 import yaml
 from pydantic import BaseModel, Field, ValidationError, model_validator
 from typing_extensions import Self
 
-__all__ = ["read_config", "write_config"]
+from . import aoi, forcing, nid, nlcd, nwis, soil, topo
+
+if TYPE_CHECKING:
+    from yaml.nodes import Node
+
+__all__ = [
+    "read_config",
+    "write_config",
+    "AOI",
+    "Config",
+    "Project",
+    "Forcing",
+    "Topo",
+    "Soil",
+    "NLCD",
+    "NID",
+    "Streamflow",
+    "FilePaths",
+]
 
 yaml_load = functools.partial(yaml.load, Loader=getattr(yaml, "CSafeLoader", yaml.SafeLoader))
-Dumper = getattr(yaml, "CSafeDumper", yaml.SafeDumper)
+SafeDumper = getattr(yaml, "CSafeDumper", yaml.SafeDumper)
+
+
+class PathDumper(SafeDumper):  # pyright: ignore[reportGeneralTypeIssues,reportUntypedBaseClass]
+    """A dumper that can represent pathlib.Path objects as strings."""
+
+    def represent_data(self, data: Any) -> Node:
+        """Represent Path objects as strings."""
+        if isinstance(data, Path):
+            return self.represent_scalar("tag:yaml.org,2002:str", str(data))
+        return super().represent_data(data)
 
 
 def yaml_dump(o: Any, **kwargs: Any) -> str:
     """Dump YAML.
 
     Notes
     -----
-    When python/mypy#1484 is solved, this can be `functools.partial`
+    When python/mypy#1484 is solved, this can be ``functools.partial``
     """
     return yaml.dump(
         o,
-        Dumper=Dumper,
+        Dumper=PathDumper,
         stream=None,
         default_flow_style=False,
         indent=2,
         sort_keys=False,
         **kwargs,
     )
 
@@ -72,21 +100,31 @@
         List of GAGES-II basin IDs, by default None. The IDs must be strings.
     geometry_file : str, optional
         Path to a geometry file, by default None. Supported file extensions are
         ``.feather``, ``.parquet``, and any format supported by
         ``geopandas.read_file`` (e.g., ``.shp``, ``.geojson``, and ``.gpkg``).
     nhdv2_flowlines : bool, optional
         Whether to retrieve the NHDPlus V2 flowlines within the AOI, by default False.
+    streamcat_attrs : list of str, optional
+        List of StreamCat attributes to retrieve, by default None. This will
+        set the ``nhdv2_flowlines`` to True. Use ``pynhd.StreamCat().metrics_df``
+        to get a dataframe of all available attributes with their descriptions.
+    nldi_attrs : list of str, optional
+        List of slelect attributes to retrieve, by default None.
+        Use ``pynhd.nhdplus_attrs_s3()`` to get a dataframe of all available
+        attributes with their descriptions.
     """
 
     huc_ids: list[str] | None = None
     nhdv2_ids: list[int] | None = None
     gagesii_basins: list[str] | None = None
     geometry_file: str | None = None
     nhdv2_flowlines: bool = False
+    streamcat_attrs: list[str] | None = None
+    nldi_attrs: list[str] | None = None
 
     @model_validator(mode="after")
     def check_exclusive_options(self) -> Self:
         """Check if only one of the options is provided."""
         provided_options = [
             option
             for option in (self.huc_ids, self.nhdv2_ids, self.gagesii_basins, self.geometry_file)
@@ -204,37 +242,37 @@
     frequency : str
         Frequency of the streamflow data. Supported frequencies are
         "daily" and "instantaneous".
     """
 
     start_date: datetime
     end_date: datetime
-    frequency: str
+    frequency: Literal["daily", "instantaneous"]
 
     @model_validator(mode="after")
     def check_exclusive_options(self) -> Self:
         """Check if the frequency is either 'daily' or 'instantaneous'."""
         if self.frequency not in ("daily", "instantaneous"):
             raise ValueError("Frequency must be either 'daily' or 'instantaneous'.")
         return self
 
 
 @dataclass
 class FilePaths:
     """File paths to store the data."""
 
-    project_dir: Path
+    project: Path
     aoi_parquet: Path
-    flowlines_dir: Path
-    forcing_dir: Path
-    topo_dir: Path
-    soil_dir: Path
-    nlcd_dir: Path
-    nid_dir: Path
-    streamflow_dir: Path
+    flowlines: Path
+    forcing: Path
+    topo: Path
+    soil: Path
+    nlcd: Path
+    nid: Path
+    streamflow: Path
 
 
 class Config(BaseModel):
     """Configuration for HySetter.
 
     Notes
     -----
@@ -254,16 +292,14 @@
         Soil data, by default None.
     nlcd : NLCD, optional
         National Land Cover Database (NLCD) data, by default None.
     nid : NID, optional
         National Inventory of Dams (NID) data, by default None.
     streamflow : Streamflow, optional
         Streamflow data from NWIS, by default None.
-    file_paths : FilePaths
-        File paths to store the data.
     """
 
     project: Project
     aoi: AOI
     forcing: Forcing | None = None
     topo: Topo | None = None
     soil: Soil | None = None
@@ -272,32 +308,52 @@
     streamflow: Streamflow | None = None
     file_paths: FilePaths = Field(default=None, init=False)
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         project_dir = Path(self.project.data_dir, self.project.name.replace(" ", "_"))
         self.file_paths = FilePaths(
-            project_dir=project_dir,
+            project=project_dir,
             aoi_parquet=Path(project_dir, "aoi.parquet"),
-            flowlines_dir=Path(project_dir, "nhdv2_flowlines"),
-            forcing_dir=Path(project_dir, "forcing"),
-            topo_dir=Path(project_dir, "topo"),
-            soil_dir=Path(project_dir, "soil"),
-            nlcd_dir=Path(project_dir, "nlcd"),
-            nid_dir=Path(project_dir, "nid"),
-            streamflow_dir=Path(project_dir, "streamflow"),
+            flowlines=Path(project_dir, "nhdv2_flowlines"),
+            forcing=Path(project_dir, "forcing"),
+            topo=Path(project_dir, "topo"),
+            soil=Path(project_dir, "soil"),
+            nlcd=Path(project_dir, "nlcd"),
+            nid=Path(project_dir, "nid"),
+            streamflow=Path(project_dir, "streamflow"),
         )
 
+    def get_data(self) -> None:
+        """Iterate over non-None attributes."""
+        get_func = {
+            "aoi": aoi.get_aoi,
+            "forcing": forcing.get_forcing,
+            "topo": topo.get_topo,
+            "soil": soil.get_soil,
+            "nlcd": nlcd.get_nlcd,
+            "nid": nid.get_nid,
+            "streamflow": nwis.get_streamflow,
+        }
+        self.file_paths.project.mkdir(exist_ok=True, parents=True)
+        for name, func in get_func.items():
+            cfg = getattr(self, name)
+            if cfg is not None:
+                fdir = (
+                    self.file_paths.flowlines if name == "aoi" else getattr(self.file_paths, name)
+                )
+                func(cfg, fdir, self.file_paths.aoi_parquet)
+
 
 def read_config(file_path: str | Path) -> Config:
     """Read a configuration file and return a Config object.
 
     Parameters
     ----------
-    file_path : str or Path
+    file_path : str or pathlib.Path
         Path to the configuration file.
 
     Returns
     -------
     Config
         A Config object.
     """
@@ -311,11 +367,11 @@
 def write_config(config: Config, file_path: str | Path) -> None:
     """Write a Config object to a file.
 
     Parameters
     ----------
     config : Config
         A Config object.
-    file_path : str or Path
+    file_path : str or pathlib.Path
         Path to the configuration file.
     """
     Path(file_path).write_text(yaml_dump(config.model_dump()))
```

### Comparing `hysetter-0.1.0/hysetter/nid.py` & `hysetter-0.1.1/hysetter/nid.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from typing import TYPE_CHECKING
 
 import geopandas as gpd
 from rich.console import Console
 from rich.progress import track
 
 if TYPE_CHECKING:
-    from .hysetter import Config
+    from .hysetter import NID
 
 __all__ = ["get_nid"]
 
 
-def get_nid(config: Config) -> None:
+def get_nid(cfg_nid: NID, nid_dir: Path, aoi_parquet: Path) -> None:
     """Get NID data for the area of interest.
 
     Parameters
     ----------
-    config : Config
-        A Config object.
+    cfg_nid : NID
+        A NID object.
+    nid_dir : Path
+        Path to the directory where the NID data will be saved.
+    aoi_parquet : Path
+        The path to the AOI parquet file.
     """
     from pygeohydro import NID
 
     console = Console()
-    if config.nid is None:
-        return
-
-    gdf = gpd.read_parquet(config.file_paths.aoi_parquet)
-    config.file_paths.nid_dir.mkdir(exist_ok=True, parents=True)
+    gdf = gpd.read_parquet(aoi_parquet)
+    nid_dir.mkdir(exist_ok=True, parents=True)
     nid = NID()
-    nid.stage_nid_inventory(Path(config.file_paths.project_dir, "full_nid_inventory.parquet"))
-    if not config.nid.within_aoi:
+    nid.stage_nid_inventory(Path(nid_dir, "full_nid_inventory.parquet"))
+    if not cfg_nid.within_aoi:
         return
 
     for i, geom in track(
         enumerate(gdf.geometry), description="Getting dams from NID", total=len(gdf)
     ):
-        fpath = Path(config.file_paths.nid_dir, f"nid_geom_{i}.parquet")
+        fpath = Path(nid_dir, f"nid_geom_{i}.parquet")
         if fpath.exists():
             continue
         try:
             nid.get_bygeom(geom, gdf.crs).to_parquet(fpath)
         except Exception:
             console.print_exception(show_locals=True, max_frames=4)
             console.print(f"Failed to get NID data for AOI index {i}")
```

### Comparing `hysetter-0.1.0/hysetter/nwis.py` & `hysetter-0.1.1/hysetter/nwis.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,46 +6,47 @@
 from typing import TYPE_CHECKING
 
 import geopandas as gpd
 from rich.console import Console
 from rich.progress import track
 
 if TYPE_CHECKING:
-    from .hysetter import Config
+    from .hysetter import Streamflow
 
 __all__ = ["get_streamflow"]
 
 
-def get_streamflow(config: Config) -> None:
+def get_streamflow(cfg_streamflow: Streamflow, streamflow_dir: Path, aoi_parquet: Path) -> None:
     """Get streamflow data for the area of interest.
 
     Parameters
     ----------
-    config : Config
-        A Config object.
+    cfg_streamflow : Streamflow
+        A Streamflow object.
+    streamflow_dir : Path
+        Path to the directory where the streamflow data will be saved.
+    aoi_parquet : Path
+        The path to the AOI parquet file.
     """
     from pygeohydro import NWIS
 
     console = Console()
-    if config.streamflow is None:
-        return
+    gdf = gpd.read_parquet(aoi_parquet)
+    streamflow_dir.mkdir(exist_ok=True, parents=True)
 
-    gdf = gpd.read_parquet(config.file_paths.aoi_parquet)
-    config.file_paths.streamflow_dir.mkdir(exist_ok=True, parents=True)
-
-    start = config.streamflow.start_date.strftime("%Y-%m-%d")
-    end = config.streamflow.end_date.strftime("%Y-%m-%d")
-    freq = "dv" if config.streamflow.frequency == "daily" else "iv"
+    start = cfg_streamflow.start_date.strftime("%Y-%m-%d")
+    end = cfg_streamflow.end_date.strftime("%Y-%m-%d")
+    freq = "dv" if cfg_streamflow.frequency == "daily" else "iv"
     nwis = NWIS()
     for i, geom in track(
         enumerate(gdf.geometry.to_crs(4326)),
         description="Getting streamflow from NWIS",
         total=len(gdf),
     ):
-        fpath = Path(config.file_paths.streamflow_dir, f"streamflow_geom_{i}.nc")
+        fpath = Path(streamflow_dir, f"streamflow_geom_{i}.nc")
         if fpath.exists():
             continue
         try:
             query = {"bBox": ",".join(f"{b:.06f}" for b in geom.bounds), "outputDataTypeCd": freq}
             siteinfo = nwis.get_info(query)
             sids = siteinfo.loc[siteinfo.within(geom), "site_no"].unique().tolist()
             qobs = nwis.get_streamflow(sids, (start, end), freq=freq, to_xarray=True)
```

### Comparing `hysetter-0.1.0/hysetter/print_versions.py` & `hysetter-0.1.1/hysetter/print_versions.py`

 * *Files identical despite different names*

### Comparing `hysetter-0.1.0/hysetter/topo.py` & `hysetter-0.1.1/hysetter/topo.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import geopandas as gpd
 from rich.console import Console
 from rich.progress import track
 
 if TYPE_CHECKING:
     from xarray import DataArray
 
-    from .hysetter import Config
+    from .hysetter import Topo
 
 __all__ = ["get_topo"]
 
 
 def _slope(dem: DataArray) -> DataArray:
     """Calculate slope in degrees."""
     from xrspatial import slope
@@ -41,45 +41,50 @@
     A negative value indicates it is upwardly concave. A value of 0 indicates a flat surface.
     """
     from xrspatial import curvature
 
     return curvature(dem)
 
 
-def get_topo(config: Config) -> None:
+def get_topo(cfg_topo: Topo, topo_dir: Path, aoi_parquet: Path) -> None:
     """Get topo data for the area of interest.
 
     Parameters
     ----------
-    config : Config
-        A Config object.
+    cfg_topo : Topo
+        A Topo object.
+    topo_dir : Path
+        Path to the directory where the topo data will be saved.
+    aoi_parquet : Path
+        The path to the AOI parquet file.
     """
     import xarray as xr
     from py3dep import get_dem
 
     console = Console()
-    if config.topo is None:
-        return
+
     topo_functions = {"slope": _slope, "aspect": _aspect, "curvature": _curvature}
 
-    gdf = gpd.read_parquet(config.file_paths.aoi_parquet)
-    config.file_paths.topo_dir.mkdir(exist_ok=True, parents=True)
+    gdf = gpd.read_parquet(aoi_parquet)
+    topo_dir.mkdir(exist_ok=True, parents=True)
     for i, geom in track(
         enumerate(gdf.geometry), description="Getting DEM from 3DEP", total=len(gdf)
     ):
-        fpath = Path(config.file_paths.topo_dir, f"topo_geom_{i}.nc")
+        fpath = Path(topo_dir, f"topo_geom_{i}.nc")
         if fpath.exists():
             continue
         try:
-            topo = get_dem(geom, config.topo.resolution_m, gdf.crs)
+            topo = get_dem(geom, cfg_topo.resolution_m, gdf.crs).rio.reproject(5070)
+            topo = topo.where(topo.notnull(), drop=True).rio.write_transform()
         except Exception:
             console.print_exception(show_locals=True, max_frames=4)
             console.print(f"Failed to get topo data for AOI index {i}")
             continue
-        if config.topo.derived_variables:
+        if cfg_topo.derived_variables:
+            topo.attrs["res"] = topo.rio.resolution()
             topo_list = [
                 topo_functions[var](topo)
-                for var in config.topo.derived_variables
+                for var in cfg_topo.derived_variables
                 if var in topo_functions
             ]
             topo = xr.merge([topo, *topo_list])
         topo.to_netcdf(fpath)
```

### Comparing `hysetter-0.1.0/hysetter.egg-info/PKG-INFO` & `hysetter-0.1.1/hysetter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hysetter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Subset hydroclimate data using HyRiver Over CONUS.
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/hysetter.html
 Project-URL: CI, https://github.com/hyriver/hysetter/actions
 Project-URL: Homepage, https://docs.hyriver.io/readme/hysetter.html
 Project-URL: Issues, https://github.com/hyriver/hysetter/issues
@@ -21,35 +21,36 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: async-retriever>=0.16.1
+Requires-Dist: boto3
+Requires-Dist: dask[dataframe]
 Requires-Dist: flox
-Requires-Dist: hydrosignatures>=0.16
+Requires-Dist: geopandas
 Requires-Dist: numba
 Requires-Dist: numbagg
+Requires-Dist: pandas
 Requires-Dist: planetary-computer
 Requires-Dist: py3dep>=0.16.3
-Requires-Dist: py7zr
-Requires-Dist: pydantic
+Requires-Dist: pyarrow>=1.0.1
+Requires-Dist: pydantic>=2.7.1
 Requires-Dist: pydaymet>=0.16.3
-Requires-Dist: pygeohydro>=0.16.3
-Requires-Dist: pygeoogc>=0.16.3
-Requires-Dist: pygeoutils>=0.16.3
+Requires-Dist: pygeohydro>=0.16.4
 Requires-Dist: pygridmet>=0.16
 Requires-Dist: pynhd>=0.16.3
 Requires-Dist: pynldas2>=0.16
 Requires-Dist: pyogrio
 Requires-Dist: pystac-client
 Requires-Dist: pyyaml
-Requires-Dist: rich-click
+Requires-Dist: rich-click>=1.8.2
 Requires-Dist: typing-extensions
+Requires-Dist: xarray>=2024.5
 Requires-Dist: xarray-spatial
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-xdist[psutil]; extra == "test"
 
 HySetter: Hyroclimate Data Subsetter based on HyRiver
@@ -100,15 +101,17 @@
 
 HySetter is an open-source Python package, built on HyRiver software stack, that provides a
 command-line interface (CLI) for subsetting hydroclimate data from the following data sources
 over conterminous United States (CONUS):
 
 - **Area Of Interest**: From any `HUC <https://www.usgs.gov/national-hydrography/watershed-boundary-dataset>`__
   level, `GAGES-II basins <https://pubs.usgs.gov/publication/70046617>`__,
-  `NHDPlusV2 <https://www.nhdplus.com/NHDPlus/NHDPlusV2_home.php>`__ catchments,
+  `NHDPlusV2 <https://www.nhdplus.com/NHDPlus/NHDPlusV2_home.php>`__ catchments and their
+  attributes (`StreamCat <https://www.epa.gov/national-aquatic-resource-surveys/streamcat-dataset>`__
+  and `NLDI <https://labs.waterdata.usgs.gov/docs/nldi/about-nldi/index.html>`__),
   or a user-defined GeoDataFrame
 - **Drainage Network**: From NHDPlusV2
 - **Forcing**: From `Daymet <https://daymet.ornl.gov/>`__,
   `GridMET <https://www.climatologylab.org/gridmet.html>`__,
   or `NLDAS2 <https://ldas.gsfc.nasa.gov/nldas/v2/forcing>`__
 - **Streamflow**: From `NWIS <https://nwis.waterdata.usgs.gov/nwis>`__
 - **Soil**: From `gNATSGO <https://planetarycomputer.microsoft.com/dataset/gnatsgo-rasters>`__,
@@ -160,15 +163,16 @@
 source, the area of interest (AOI), and the output directory. You can find an example
 configuration file in the
 `config_demo.yml <https://github.com/hyriver/hysetter/blob/main/config_demo.yml>`__.
 
 .. image:: https://raw.githubusercontent.com/hyriver/hysetter/main/hs_help.svg
     :align: center
 
-.. image:: https://raw.githubusercontent.com/hyriver/hysetter/main/hs_demo.gif
+.. image:: https://asciinema.org/a/660577.svg
+    :target: https://asciinema.org/a/660577?autoplay=1
     :align: center
 
 Contributing
 ------------
 Contributions are appreciated and very welcomed. Please read
 `CONTRIBUTING.rst <https://github.com/hyriver/hysetter/blob/main/CONTRIBUTING.rst>`__
 for instructions.
```

### Comparing `hysetter-0.1.0/hysetter.egg-info/SOURCES.txt` & `hysetter-0.1.1/hysetter.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 config_demo.yml
 conftest.py
-hs_demo.gif
 hs_help.svg
 noxfile.py
 pyproject.toml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bugreport.yml
 .github/ISSUE_TEMPLATE/config.yml
```

### Comparing `hysetter-0.1.0/pyproject.toml` & `hysetter-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -29,35 +29,36 @@
   "Topic :: Scientific/Engineering :: Hydrology",
   "Typing :: Typed",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "async-retriever>=0.16.1",
+  "boto3",
+  "dask[dataframe]",
   "flox",
-  "hydrosignatures>=0.16",
+  "geopandas",
   "numba",
   "numbagg",
+  "pandas",
   "planetary-computer",
   "py3dep>=0.16.3",
-  "py7zr",
-  "pydantic",
+  "pyarrow>=1.0.1",
+  "pydantic>=2.7.1",
   "pydaymet>=0.16.3",
-  "pygeohydro>=0.16.3",
-  "pygeoogc>=0.16.3",
-  "pygeoutils>=0.16.3",
+  "pygeohydro>=0.16.4",
   "pygridmet>=0.16",
   "pynhd>=0.16.3",
   "pynldas2>=0.16",
   "pyogrio",
   "pystac-client",
   "pyyaml",
-  "rich-click",
+  "rich-click>=1.8.2",
   "typing-extensions",
+  "xarray>=2024.5",
   "xarray-spatial",
 ]
 optional-dependencies.test = [
   "pytest-cov",
   "pytest-sugar",
   "pytest-xdist[psutil]",
 ]
@@ -154,14 +155,27 @@
   "UP",
   # Warning
   "W",
   # flake8-2020
   "YTT",
 ]
 
+lint.ignore = [
+  # docstring in class __init__
+  "D107",
+  # long too long, let the formatter handle it
+  "E501",
+  # conflict with ruff-formatter
+  "ISC001",
+  # too many arguments
+  "PLR0913",
+  # custom exceptions
+  "TRY003",
+]
+
 lint.per-file-ignores."tests/*.py" = [
   # Disable all docstring checks in tests
   "D100",
   "D101",
   "D102",
   "D103",
   "D104",
@@ -184,33 +198,21 @@
 lint.isort.known-first-party = [
   "hysetter",
 ]
 lint.isort.required-imports = [
   "from __future__ import annotations",
 ]
 lint.pydocstyle.convention = "numpy"
-lint.ignore = [
-  # docstring in class __init__
-  "D107",
-  # long too long, let the formatter handle it
-  "E501",
-  # conflict with ruff-formatter
-  "ISC001",
-  # too many arguments
-  "PLR0913",
-  # custom exceptions
-  "TRY003",
-]
 
 [tool.codespell]
 skip = "__pycache__,_build,.mypy_cache,.git,./htmlcov,.nox"
 ignore-words-list = "gage,gages"
 
 [tool.pytest.ini_options]
-addopts = "-n=auto -v --cov=hysetter --cov-report xml --durations=5"
+addopts = "-n=auto -v --durations=5"
 doctest_optionflags = 'NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL NUMBER'
 filterwarnings = [
   "ignore:.*numpy.ndarray size changed.*",
 ]
 testpaths = [
   "tests",
   "hysetter",
```

