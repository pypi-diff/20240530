# Comparing `tmp/lsst_utils-27.0.0rc2.tar.gz` & `tmp/lsst_utils-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_utils-27.0.0rc2.tar", last modified: Thu May 23 01:53:34 2024, max compression
+gzip compressed data, was "lsst_utils-27.2024.2200.tar", last modified: Thu May 30 09:56:42 2024, max compression
```

## Comparing `lsst_utils-27.0.0rc2.tar` & `lsst_utils-27.2024.2200.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.038531 lsst_utils-27.0.0rc2/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.042531 lsst_utils-27.0.0rc2/doc/lsst.utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/doc/lsst.utils/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/doc/lsst.utils/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.042531 lsst_utils-27.0.0rc2/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.042531 lsst_utils-27.0.0rc2/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.046531 lsst_utils-27.0.0rc2/python/lsst/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.046531 lsst_utils-27.0.0rc2/python/lsst/utils/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/plotting/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:53:33.000000 lsst_utils-27.0.0rc2/python/lsst/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/python/lsst/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:53:34.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:53:33.000000 lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:53:34.054531 lsst_utils-27.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_db_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_doImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_getPackageDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_getTempFilePath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_inheritDoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_plotting_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-23 01:53:27.000000 lsst_utils-27.0.0rc2/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.672266 lsst_utils-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-30 09:56:42.672266 lsst_utils-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.656266 lsst_utils-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.656266 lsst_utils-27.2024.2200/doc/lsst.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/doc/lsst.utils/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/doc/lsst.utils/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.656266 lsst_utils-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.656266 lsst_utils-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.664266 lsst_utils-27.2024.2200/python/lsst/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.664266 lsst_utils-27.2024.2200/python/lsst/utils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/plotting/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39013 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/python/lsst/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.664266 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:42.000000 lsst_utils-27.2024.2200/python/lsst_utils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 09:56:42.672266 lsst_utils-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:42.664266 lsst_utils-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18133 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_db_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_doImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_getPackageDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_getTempFilePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_inheritDoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_plotting_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-30 09:56:35.000000 lsst_utils-27.2024.2200/tests/test_wrappers.py
```

### Comparing `lsst_utils-27.0.0rc2/LICENSE` & `lsst_utils-27.2024.2200/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/PKG-INFO` & `lsst_utils-27.2024.2200/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 27.0.0rc2
+Version: 27.2024.2200
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
 License-File: COPYRIGHT
 License-File: LICENSE
 Requires-Dist: numpy>=1.17
 Requires-Dist: psutil>=5.7
 Requires-Dist: deprecated>=1.2
 Requires-Dist: pyyaml>=5.1
```

### Comparing `lsst_utils-27.0.0rc2/README.rst` & `lsst_utils-27.2024.2200/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/doc/lsst.utils/CHANGES.rst` & `lsst_utils-27.2024.2200/doc/lsst.utils/CHANGES.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,156 @@
+lsst-utils 27.0.0 (2024-05-28)
+==============================
+
+Now requires Python 3.10 or newer.
+
+New Features
+------------
+
+- Allow for skipping files in ``ImportTestCase`` using ``SKIP_FILES`` class variable. (`DM-40817 <https://rubinobs.atlassian.net/browse/DM-40817>`_)
+
+
+Bug Fixes
+---------
+
+- Fixed ``inheritDoc`` to insert newlines between the parent and child docstrings and also correct for indentation differences. (`DM-22287 <https://rubinobs.atlassian.net/browse/DM-22287>`_)
+- Fixed a race condition in ``Singleton`` that could cause more than one instance of a class to be created if two threads concurrently attempted to create the instance. (`DM-42317 <https://rubinobs.atlassian.net/browse/DM-42317>`_)
+
+
+Miscellaneous Changes of Minor Interest
+---------------------------------------
+
+- Export type aliases for LSST log adapters for use in downstream static typing. (`DM-40441 <https://rubinobs.atlassian.net/browse/DM-40441>`_)
+- Changed how Conda package versions are discovered, resulting in a 10x speed up.
+  No longer uses ``conda list``. (`DM-40803 <https://rubinobs.atlassian.net/browse/DM-40803>`_)
+- Use ``packages_distributions()`` from `importlib.metadata` to get mapping from import name to distribution name. (`DM-42391 <https://rubinobs.atlassian.net/browse/DM-42391>`_)
+
+
 lsst-utils v26.0.0 (2023-09-22)
 ===============================
 
 This release no longer works with Python 3.8.
 
 New Features
 ------------
 
 - Now works with Python 3.11.
-  Python 3.11 now ensures that the ``stacklevel`` parameter for logging methods is now consistent independent of how many method calls are involved internally. (`DM-37987 <https://jira.lsstcorp.org/browse/DM-37987>`_)
+  Python 3.11 now ensures that the ``stacklevel`` parameter for logging methods is now consistent independent of how many method calls are involved internally. (`DM-37987 <https://rubinobs.atlassian.net/browse/DM-37987>`_)
 - Added ``lsst.utils.tests.ImportTestCase`` class.
   This test case can be used to force the import of every file in a package.
-  This can be very useful for spotting obvious problems if a package does not export every file by default. (`DM-35901 <https://jira.lsstcorp.org/browse/DM-35901>`_)
-- Added a utility function, ``calculate_safe_plotting_limits``, located in ``lsst.utils.plotting.limits``, for calculating plotting limits for data with large outliers. (`DM-38386 <https://jira.lsstcorp.org/browse/DM-38386>`_)
-- ``MemoryTestCase`` now can accept an "ignore" list of regexps that match acceptable open files. (`DM-38764 <https://jira.lsstcorp.org/browse/DM-38764>`_)
+  This can be very useful for spotting obvious problems if a package does not export every file by default. (`DM-35901 <https://rubinobs.atlassian.net/browse/DM-35901>`_)
+- Added a utility function, ``calculate_safe_plotting_limits``, located in ``lsst.utils.plotting.limits``, for calculating plotting limits for data with large outliers. (`DM-38386 <https://rubinobs.atlassian.net/browse/DM-38386>`_)
+- ``MemoryTestCase`` now can accept an "ignore" list of regexps that match acceptable open files. (`DM-38764 <https://rubinobs.atlassian.net/browse/DM-38764>`_)
 - Adds an alternative way of interacting with ``calculate_safe_plotting_limits()``.
 
-  This change adds a factory interface, such that one can use the function to accumulate the safe plotting limits over many different data series without having them all in-hand, by using the ``make_calculate_safe_plotting_limits()`` function to return a ``calculate_safe_plotting_limits()`` which will return the common limits after the addition of each new data series. The original behaviour remains unchanged. (`DM-38900 <https://jira.lsstcorp.org/browse/DM-38900>`_)
+  This change adds a factory interface, such that one can use the function to accumulate the safe plotting limits over many different data series without having them all in-hand, by using the ``make_calculate_safe_plotting_limits()`` function to return a ``calculate_safe_plotting_limits()`` which will return the common limits after the addition of each new data series. The original behaviour remains unchanged. (`DM-38900 <https://rubinobs.atlassian.net/browse/DM-38900>`_)
 - Added ``lsst.utils.introspection.find_outside_stacklevel``.
-  This function can be used to calculate the stack level that should be passed to warnings and log messages in order to make them look like they came from the line outside the specified package in user code. (`DM-39628 <https://jira.lsstcorp.org/browse/DM-39628>`_)
-- Update the interface to ``lsst.utils.introspection.find_outside_stacklevel`` to allow multiple modules to be skipped in the hierarchy and also specify that some methods and modules should not be skipped. (`DM-40032 <https://jira.lsstcorp.org/browse/DM-40032>`_)
+  This function can be used to calculate the stack level that should be passed to warnings and log messages in order to make them look like they came from the line outside the specified package in user code. (`DM-39628 <https://rubinobs.atlassian.net/browse/DM-39628>`_)
+- Update the interface to ``lsst.utils.introspection.find_outside_stacklevel`` to allow multiple modules to be skipped in the hierarchy and also specify that some methods and modules should not be skipped. (`DM-40032 <https://rubinobs.atlassian.net/browse/DM-40032>`_)
 - Added the ability for ``find_outside_stacklevel`` to return additional information about the matching stack to the caller.
-  This allows, for example, the filename and lineno to be reported without the caller making another call to ``inspect.stack()`` or calling ``get_caller_name``. (`DM-40367 <https://jira.lsstcorp.org/browse/DM-40367>`_)
-- Added the ``lsst.utils.db_auth.DbAuth`` class that has been relocated from ``daf_butler``. (`DM-40462 <https://jira.lsstcorp.org/browse/DM-40462>`_)
+  This allows, for example, the filename and lineno to be reported without the caller making another call to ``inspect.stack()`` or calling ``get_caller_name``. (`DM-40367 <https://rubinobs.atlassian.net/browse/DM-40367>`_)
+- Added the ``lsst.utils.db_auth.DbAuth`` class that has been relocated from ``daf_butler``. (`DM-40462 <https://rubinobs.atlassian.net/browse/DM-40462>`_)
 
 
 Bug Fixes
 ---------
 
 - Fixed ``time_this`` when ``mem_usage=True`` to prevent memory statistics being gathered when the log message would not be issued.
-  We had been trapping this on the exit to the context manager but not entry for the initial memory statistics gathering. (`DM-38587 <https://jira.lsstcorp.org/browse/DM-38587>`_)
+  We had been trapping this on the exit to the context manager but not entry for the initial memory statistics gathering. (`DM-38587 <https://rubinobs.atlassian.net/browse/DM-38587>`_)
 - Updated the python version handling such that it is no longer a failure for the python package version to disagree with the ``.version`` property of that package.
-  The package version is now used in preference if there is a disagreement. (`DM-38665 <https://jira.lsstcorp.org/browse/DM-38665>`_)
+  The package version is now used in preference if there is a disagreement. (`DM-38665 <https://rubinobs.atlassian.net/browse/DM-38665>`_)
 
 
 Miscellaneous Changes of Minor Interest
 ---------------------------------------
 
 - Modified the code that determines the versions of Python packages so that it now uses `importlib.metadata`.
-  This is slightly slower than accessing ``__version__`` but does give more consistent results. (`DM-38812 <https://jira.lsstcorp.org/browse/DM-38812>`_)
+  This is slightly slower than accessing ``__version__`` but does give more consistent results. (`DM-38812 <https://rubinobs.atlassian.net/browse/DM-38812>`_)
 - Improved the performance of ``lsst.utils.packages.getPythonPackages()`` to use the namespace hierarchy so it now only needs to check as deep into the hierarchy as is needed to find a version.
-  Additionally, the code no longer tries to extract versions from Python standard library packages. (`DM-39402 <https://jira.lsstcorp.org/browse/DM-39402>`_)
+  Additionally, the code no longer tries to extract versions from Python standard library packages. (`DM-39402 <https://rubinobs.atlassian.net/browse/DM-39402>`_)
 
 
 An API Removal or Deprecation
 -----------------------------
 
-- Dropped support for Python 3.8. (`DM-35901 <https://jira.lsstcorp.org/browse/DM-35901>`_)
+- Dropped support for Python 3.8. (`DM-35901 <https://rubinobs.atlassian.net/browse/DM-35901>`_)
 - * Removed deprecated APIs from `lsst.utils.logging`.
   * Removed deprecated ``demangleType`` and ``backtrace`` that were forwarded from ``cpputils``.
-  * Removed ``cpputils`` from the EUPS table file. (`DM-37534 <https://jira.lsstcorp.org/browse/DM-37534>`_)
+  * Removed ``cpputils`` from the EUPS table file. (`DM-37534 <https://rubinobs.atlassian.net/browse/DM-37534>`_)
 - A Mypy workaround in the ``ellipsis`` module is not needed for Python 3.10 or newer.
-  Importing ``lsst.utils.ellipsis`` in these Python versions will produce a `DeprecationWarning`. (`DM-39410 <https://jira.lsstcorp.org/browse/DM-39410>`_)
-- Removed deprecated ``lsst.utils.get_caller_name``. Use ``lsst.utils.introspection``. (`DM-40032 <https://jira.lsstcorp.org/browse/DM-40032>`_)
+  Importing ``lsst.utils.ellipsis`` in these Python versions will produce a `DeprecationWarning`. (`DM-39410 <https://rubinobs.atlassian.net/browse/DM-39410>`_)
+- Removed deprecated ``lsst.utils.get_caller_name``. Use ``lsst.utils.introspection``. (`DM-40032 <https://rubinobs.atlassian.net/browse/DM-40032>`_)
 
 
 lsst-utils v25.0.0 (2023-02-17)
 ===============================
 
 New Features
 ------------
 
-- Added ``lsst.utils.timer.profile`` to allow code blocks to be profiled easily. (`DM-35697 <https://jira.lsstcorp.org/browse/DM-35697>`_)
+- Added ``lsst.utils.timer.profile`` to allow code blocks to be profiled easily. (`DM-35697 <https://rubinobs.atlassian.net/browse/DM-35697>`_)
 
 
 Miscellaneous Changes of Minor Interest
 ---------------------------------------
 
-- Moved a module with a typing workaround for the built-in ``Ellipsis`` (``...``) singleton here, from ``daf_butler``. (`DM-36108 <https://jira.lsstcorp.org/browse/DM-36108>`_)
-- Remove selected unit tests for memory reporting functions. (`DM-36960 <https://jira.lsstcorp.org/browse/DM-36960>`_)
+- Moved a module with a typing workaround for the built-in ``Ellipsis`` (``...``) singleton here, from ``daf_butler``. (`DM-36108 <https://rubinobs.atlassian.net/browse/DM-36108>`_)
+- Remove selected unit tests for memory reporting functions. (`DM-36960 <https://rubinobs.atlassian.net/browse/DM-36960>`_)
 
 
 lsst-utils v24.0.0 (2022-08-26)
 ===============================
 
 New Features
 ------------
 
-- Add option to ignore NaNs in ``lsst.utils.tests.assertFloatsAlmostEqual``. (`DM-29370 <https://jira.lsstcorp.org/browse/DM-29370>`_)
-- Add test decorators to operate on cartesian product. (`DM-31141 <https://jira.lsstcorp.org/browse/DM-31141>`_)
+- Add option to ignore NaNs in ``lsst.utils.tests.assertFloatsAlmostEqual``. (`DM-29370 <https://rubinobs.atlassian.net/browse/DM-29370>`_)
+- Add test decorators to operate on cartesian product. (`DM-31141 <https://rubinobs.atlassian.net/browse/DM-31141>`_)
 - * Several new packages added from ``pipe_base`` and ``daf_butler``:
 
     * ``lsst.utils.timer``
     * ``lsst.utils.classes``
     * ``lsst.utils.introspection``
     * ``lsst.utils.iteration``
     * ``lsst.utils.logging``
   * Added ``lsst.utils.doImportType`` to import a python type from a string and guarantee it is not a module.
-  * ``lsst.utils.get_caller_name`` is now deprecated in its current location and has been relocated to ``lsst.utils.introspection``. (`DM-31722 <https://jira.lsstcorp.org/browse/DM-31722>`_)
-- Add `lsst.utils.logging.trace_set_at` to control ``TRACE``-level loggers. (`DM-32142 <https://jira.lsstcorp.org/browse/DM-32142>`_)
-- Builds using ``setuptools`` now calculate versions from the Git repository, including the use of alpha releases for those associated with weekly tags. (`DM-32408 <https://jira.lsstcorp.org/browse/DM-32408>`_)
-- Context manager ``lsst.utils.timer.time_this`` can now include memory usage in its report. (`DM-33331 <https://jira.lsstcorp.org/browse/DM-33331>`_)
+  * ``lsst.utils.get_caller_name`` is now deprecated in its current location and has been relocated to ``lsst.utils.introspection``. (`DM-31722 <https://rubinobs.atlassian.net/browse/DM-31722>`_)
+- Add `lsst.utils.logging.trace_set_at` to control ``TRACE``-level loggers. (`DM-32142 <https://rubinobs.atlassian.net/browse/DM-32142>`_)
+- Builds using ``setuptools`` now calculate versions from the Git repository, including the use of alpha releases for those associated with weekly tags. (`DM-32408 <https://rubinobs.atlassian.net/browse/DM-32408>`_)
+- Context manager ``lsst.utils.timer.time_this`` can now include memory usage in its report. (`DM-33331 <https://rubinobs.atlassian.net/browse/DM-33331>`_)
 - A new package ``lsst.utils.packages`` has been added to allow system package versions to be obtained.
-  This code has been relocated from ``lsst.base``. (`DM-33403 <https://jira.lsstcorp.org/browse/DM-33403>`_)
+  This code has been relocated from ``lsst.base``. (`DM-33403 <https://rubinobs.atlassian.net/browse/DM-33403>`_)
 - Add ``lsst.utils.threads`` for control of threads.
   Use `lsst.utils.threads.disable_implicit_threading()` to disable implicit threading.
   This function should be used in place of ``lsst.base.disableImplicitThreading()`` in all new code.
-  This package now depends on the ``threadpoolctl`` package. (`DM-33622 <https://jira.lsstcorp.org/browse/DM-33622>`_)
-- Added a new class `lsst.utils.logging.PeriodicLogger` to allow a user to issue log messages after some time interval has elapsed. (`DM-33919 <https://jira.lsstcorp.org/browse/DM-33919>`_)
-- Added ``lsst.utils.logging.getTraceLogger`` to simplify the creation of a trace logger that uses a ``TRACEn`` prefix for the logger name. (`DM-34208 <https://jira.lsstcorp.org/browse/DM-34208>`_)
+  This package now depends on the ``threadpoolctl`` package. (`DM-33622 <https://rubinobs.atlassian.net/browse/DM-33622>`_)
+- Added a new class `lsst.utils.logging.PeriodicLogger` to allow a user to issue log messages after some time interval has elapsed. (`DM-33919 <https://rubinobs.atlassian.net/browse/DM-33919>`_)
+- Added ``lsst.utils.logging.getTraceLogger`` to simplify the creation of a trace logger that uses a ``TRACEn`` prefix for the logger name. (`DM-34208 <https://rubinobs.atlassian.net/browse/DM-34208>`_)
 
 
 API Changes
 -----------
 
 - The values for max resident set size stored in metadata are now consistently reported as bytes.
-  Previously the units were platform specific (kibibytes on Liux and bytes on macOS). (`DM-20970 <https://jira.lsstcorp.org/browse/DM-20970>`_)
+  Previously the units were platform specific (kibibytes on Liux and bytes on macOS). (`DM-20970 <https://rubinobs.atlassian.net/browse/DM-20970>`_)
 - ``deprecate_pybind11`` now requires a ``version`` parameter.
-  This matches the upstream requirement from ``deprecated.deprecated`` (`DM-29701 <https://jira.lsstcorp.org/browse/DM-29701>`_)
-- Add parameter to `~lsst.utils.packages.getEnvironmentPackages` to return all EUPS packages rather than just those that are locally setup. (`DM-33934 <https://jira.lsstcorp.org/browse/DM-33934>`_)
+  This matches the upstream requirement from ``deprecated.deprecated`` (`DM-29701 <https://rubinobs.atlassian.net/browse/DM-29701>`_)
+- Add parameter to `~lsst.utils.packages.getEnvironmentPackages` to return all EUPS packages rather than just those that are locally setup. (`DM-33934 <https://rubinobs.atlassian.net/browse/DM-33934>`_)
 
 
 Performance Enhancement
 -----------------------
 
-- Fixed an optimization when using `lsst.utils.TemplateMeta` classes with `isinstance` or `issubclass`. (`DM-32661 <https://jira.lsstcorp.org/browse/DM-32661>`_)
+- Fixed an optimization when using `lsst.utils.TemplateMeta` classes with `isinstance` or `issubclass`. (`DM-32661 <https://rubinobs.atlassian.net/browse/DM-32661>`_)
 
 
 lsst-utils v23.0.0 (2021-09-27)
 ===============================
 
-- Moved all C++ code out of this package and into ``cpputils`` package and changed license to BSD 3-clause. (`DM-31721 <https://jira.lsstcorp.org/browse/DM-31721>`_)
+- Moved all C++ code out of this package and into ``cpputils`` package and changed license to BSD 3-clause. (`DM-31721 <https://rubinobs.atlassian.net/browse/DM-31721>`_)
 
 lsst-utils v22.0 (2021-07-09)
 =============================
 
 Bug fix
 -------
```

### Comparing `lsst_utils-27.0.0rc2/doc/lsst.utils/index.rst` & `lsst_utils-27.2024.2200/doc/lsst.utils/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/pyproject.toml` & `lsst_utils-27.2024.2200/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = ["setuptools", "lsst-versions >= 1.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsst-utils"
-requires-python = ">=3.9.0"
+requires-python = ">=3.10.0"
 description = "Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST)."
 license = {text = "BSD 3-Clause License"}
 readme = "README.rst"
 authors = [
     {name="Rubin Observatory Data Management", email="dm-admin@lists.lsst.org"},
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 keywords=["lsst"]
 dependencies = [
     "numpy >= 1.17",
@@ -55,15 +54,15 @@
 
 [tool.towncrier]
     package = "lsst.utils"
     package_dir = "python"
     filename = "doc/lsst.utils/CHANGES.rst"
     directory = "doc/changes"
     title_format = "lsst-utils {version} ({project_date})"
-    issue_format = "`{issue} <https://jira.lsstcorp.org/browse/{issue}>`_"
+    issue_format = "`{issue} <https://rubinobs.atlassian.net/browse/{issue}>`_"
 
 
     [[tool.towncrier.type]]
         directory = "feature"
         name = "New Features"
         showcontent = true
```

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/__init__.py` & `lsst_utils-27.2024.2200/python/lsst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/_packaging.py` & `lsst_utils-27.2024.2200/python/lsst/utils/_packaging.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/classes.py` & `lsst_utils-27.2024.2200/python/lsst/utils/classes.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/db_auth.py` & `lsst_utils-27.2024.2200/python/lsst/utils/db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/deprecated.py` & `lsst_utils-27.2024.2200/python/lsst/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/doImport.py` & `lsst_utils-27.2024.2200/python/lsst/utils/doImport.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/ellipsis.py` & `lsst_utils-27.2024.2200/python/lsst/utils/ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/inheritDoc.py` & `lsst_utils-27.2024.2200/python/lsst/utils/inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/introspection.py` & `lsst_utils-27.2024.2200/python/lsst/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/iteration.py` & `lsst_utils-27.2024.2200/python/lsst/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/logging.py` & `lsst_utils-27.2024.2200/python/lsst/utils/logging.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/packages.py` & `lsst_utils-27.2024.2200/python/lsst/utils/packages.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/plotting/limits.py` & `lsst_utils-27.2024.2200/python/lsst/utils/plotting/limits.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/tests.py` & `lsst_utils-27.2024.2200/python/lsst/utils/tests.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/threads.py` & `lsst_utils-27.2024.2200/python/lsst/utils/threads.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/timer.py` & `lsst_utils-27.2024.2200/python/lsst/utils/timer.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/usage.py` & `lsst_utils-27.2024.2200/python/lsst/utils/usage.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst/utils/wrappers.py` & `lsst_utils-27.2024.2200/python/lsst/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/PKG-INFO` & `lsst_utils-27.2024.2200/python/lsst_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: lsst-utils
-Version: 27.0.0rc2
+Version: 27.2024.2200
 Summary: Utility functions from Rubin Observatory Data Management for the Legacy Survey of Space and Time (LSST).
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/utils
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
 License-File: COPYRIGHT
 License-File: LICENSE
 Requires-Dist: numpy>=1.17
 Requires-Dist: psutil>=5.7
 Requires-Dist: deprecated>=1.2
 Requires-Dist: pyyaml>=5.1
```

### Comparing `lsst_utils-27.0.0rc2/python/lsst_utils.egg-info/SOURCES.txt` & `lsst_utils-27.2024.2200/python/lsst_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_classes.py` & `lsst_utils-27.2024.2200/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_db_auth.py` & `lsst_utils-27.2024.2200/tests/test_db_auth.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_decorators.py` & `lsst_utils-27.2024.2200/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_deprecated.py` & `lsst_utils-27.2024.2200/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_doImport.py` & `lsst_utils-27.2024.2200/tests/test_doImport.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_ellipsis.py` & `lsst_utils-27.2024.2200/tests/test_ellipsis.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_executables.py` & `lsst_utils-27.2024.2200/tests/test_executables.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_getPackageDir.py` & `lsst_utils-27.2024.2200/tests/test_getPackageDir.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_getTempFilePath.py` & `lsst_utils-27.2024.2200/tests/test_getTempFilePath.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_import.py` & `lsst_utils-27.2024.2200/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_inheritDoc.py` & `lsst_utils-27.2024.2200/tests/test_inheritDoc.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_introspection.py` & `lsst_utils-27.2024.2200/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_iteration.py` & `lsst_utils-27.2024.2200/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_logging.py` & `lsst_utils-27.2024.2200/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_ordering.py` & `lsst_utils-27.2024.2200/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_packages.py` & `lsst_utils-27.2024.2200/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_plotting_limits.py` & `lsst_utils-27.2024.2200/tests/test_plotting_limits.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_threads.py` & `lsst_utils-27.2024.2200/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_timer.py` & `lsst_utils-27.2024.2200/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_usage.py` & `lsst_utils-27.2024.2200/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_utils.py` & `lsst_utils-27.2024.2200/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_utils-27.0.0rc2/tests/test_wrappers.py` & `lsst_utils-27.2024.2200/tests/test_wrappers.py`

 * *Files identical despite different names*

