# Comparing `tmp/lsst_pex_config-27.0.0rc2.tar.gz` & `tmp/lsst_pex_config-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_pex_config-27.0.0rc2.tar", last modified: Thu May 23 01:51:18 2024, max compression
+gzip compressed data, was "lsst_pex_config-27.2024.2200.tar", last modified: Thu May 30 09:55:48 2024, max compression
```

## Comparing `lsst_pex_config-27.0.0rc2.tar` & `lsst_pex_config-27.2024.2200.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.593458 lsst_pex_config-27.0.0rc2/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/design-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/field-types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/inspecting-configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/registry-intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.593458 lsst_pex_config-27.0.0rc2/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/python/lsst/pex/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.597458 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/_doNotImportMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/callStack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/choiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)    61518 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configDictField.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configField.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.601457 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableAction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionField.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionStructField.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableField.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/dictField.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/listField.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/rangeField.py
--rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/python/lsst/pex/config/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 01:51:18.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:51:17.000000 lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:51:18.605458 lsst_pex_config-27.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/testLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test__file__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configDictField.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configurableActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_configurableField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_dictField.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_listField.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1911.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1914.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1915.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1929.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket1995.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticket2818.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_ticketDM-7337.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_unloaded_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-23 01:51:06.000000 lsst_pex_config-27.0.0rc2/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.913359 lsst_pex_config-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-30 09:55:48.913359 lsst_pex_config-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.901359 lsst_pex_config-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.905359 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/design-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/field-types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/inspecting-configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/registry-intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.901359 lsst_pex_config-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.905359 lsst_pex_config-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.905359 lsst_pex_config-27.2024.2200/python/lsst/pex/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.909359 lsst_pex_config-27.2024.2200/python/lsst/pex/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/_doNotImportMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/callStack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/choiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61502 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23826 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configField.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.909359 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/_configurableAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/_configurableActionField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/_configurableActionStructField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/dictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/listField.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/rangeField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/python/lsst/pex/config/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.913359 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:55:48.000000 lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 09:55:48.913359 lsst_pex_config-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:48.913359 lsst_pex_config-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/testLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test__file__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_configurableActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_dictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_listField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticket1911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticket1914.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticket1915.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticket1929.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticket1995.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticket2818.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_ticketDM-7337.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_unloaded_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-30 09:55:41.000000 lsst_pex_config-27.2024.2200/tests/test_wrap.py
```

### Comparing `lsst_pex_config-27.0.0rc2/PKG-INFO` & `lsst_pex_config-27.2024.2200/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 27.0.0rc2
+Version: 27.2024.2200
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
 License-File: COPYRIGHT
 License-File: LICENSE
 License-File: gpl-v3.0.txt
 License-File: bsd_license.txt
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: numpy>=1.17
```

### Comparing `lsst_pex_config-27.0.0rc2/README.rst` & `lsst_pex_config-27.2024.2200/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/bsd_license.txt` & `lsst_pex_config-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/CHANGES.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/CHANGES.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+lsst-pex-config v27.0.0 (2024-05-29)
+====================================
+
+- Improved all docstrings to make them compliant with Numpydoc.
+- Minor code cleanups driven by Ruff linting. (`DM-42116 <https://rubinobs.atlassian.net/browse/DM-42116>`_)
+
 lsst-pex-config v26.0.0 (2023-09-22)
 ====================================
 
 New Features
 ------------
 
-- Added a dynamic-default callback argument to ``RegistryField``. (`DM-31924 <https://jira.lsstcorp.org/browse/DM-31924>`_)
-- Introduced ``ConfigurableActions``. These are ``pex_config`` fields and config types which function as a functor, state is set at config time, but the ``ConfigurableActions`` are callable at runtime to produce an action. (`DM-36649 <https://jira.lsstcorp.org/browse/DM-36649>`_)
+- Added a dynamic-default callback argument to ``RegistryField``. (`DM-31924 <https://rubinobs.atlassian.net/browse/DM-31924>`_)
+- Introduced ``ConfigurableActions``. These are ``pex_config`` fields and config types which function as a functor, state is set at config time, but the ``ConfigurableActions`` are callable at runtime to produce an action. (`DM-36649 <https://rubinobs.atlassian.net/browse/DM-36649>`_)
 
 
 API Changes
 -----------
 
-- The ``loadFromStream`` and ``loadFromString`` methods now take a dictionary as an optional argument which allows specifying additional variables to use in local scope when reading configs. (`DM-40198 <https://jira.lsstcorp.org/browse/DM-40198>`_)
+- The ``loadFromStream`` and ``loadFromString`` methods now take a dictionary as an optional argument which allows specifying additional variables to use in local scope when reading configs. (`DM-40198 <https://rubinobs.atlassian.net/browse/DM-40198>`_)
 
 
 Other Changes and Additions
 ---------------------------
 
-- There is now a requirement for configuration parameters to have a non-empty docstring. (`DM-4037 <https://jira.lsstcorp.org/browse/DM-4037>`_)
+- There is now a requirement for configuration parameters to have a non-empty docstring. (`DM-4037 <https://rubinobs.atlassian.net/browse/DM-4037>`_)
 
 
 lsst-pex-config v25.0.0 (2023-02-28)
 ====================================
 
 Other Changes and Additions
 ---------------------------
 
-- Some sorting now happens when saving config files (via DM-33027). (`DM-35060 <https://jira.lsstcorp.org/browse/DM-35060>`_)
+- Some sorting now happens when saving config files (via DM-33027). (`DM-35060 <https://rubinobs.atlassian.net/browse/DM-35060>`_)
 
 
 lsst-pex-config v24.0.0 (2022-08-30)
 ====================================
 
 New Features
 ------------
```

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/design-notes.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/design-notes.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/field-types.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/field-types.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/index.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/inspecting-configs.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/inspecting-configs.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/overview.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/overview.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/registry-intro.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/registry-intro.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/doc/lsst.pex.config/wrapping-cpp-control-objects.rst` & `lsst_pex_config-27.2024.2200/doc/lsst.pex.config/wrapping-cpp-control-objects.rst`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/gpl-v3.0.txt` & `lsst_pex_config-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/pyproject.toml` & `lsst_pex_config-27.2024.2200/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["setuptools", "lsst-versions >= 1.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsst-pex-config"
+requires-python = ">=3.10.0"
 description = "A flexible configuration system using Python files."
 license = {text = "BSD 3-Clause License, GPLv3+"}
 readme = "README.rst"
 authors = [
     {name="Rubin Observatory Data Management", email="dm-admin@lists.lsst.org"},
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 keywords = ["lsst"]
 dependencies = [
     "pyyaml >=5.1",
     "numpy >= 1.17",
 ]
@@ -59,15 +61,15 @@
 
 [tool.towncrier]
     package = "lsst.pex.config"
     package_dir = "python"
     filename = "doc/lsst.pex.config/CHANGES.rst"
     directory = "doc/changes"
     title_format = "lsst-pex-config {version} ({project_date})"
-    issue_format = "`{issue} <https://jira.lsstcorp.org/browse/{issue}>`_"
+    issue_format = "`{issue} <https://rubinobs.atlassian.net/browse/{issue}>`_"
 
     [[tool.towncrier.type]]
         directory = "feature"
         name = "New Features"
         showcontent = true
 
     [[tool.towncrier.type]]
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/__init__.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/callStack.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/callStack.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/choiceField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/choiceField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/comparison.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/comparison.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/config.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,22 +712,20 @@
         the field values in the subconfig.
         """
         return self.__get__(instance)
 
     @overload
     def __get__(
         self, instance: None, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> Field[FieldTypeVar]:
-        ...
+    ) -> Field[FieldTypeVar]: ...
 
     @overload
     def __get__(
         self, instance: Config, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> FieldTypeVar:
-        ...
+    ) -> FieldTypeVar: ...
 
     def __get__(self, instance, owner=None, at=None, label="default"):
         """Define how attribute access should occur on the Config instance
         This is invoked by the owning config object and should not be called
         directly.
 
         When the field attribute is accessed on a Config class object, it
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configChoiceField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configChoiceField.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,22 +515,20 @@
             history.append(("Initialized from defaults", at, label))
 
         return instanceDict
 
     @overload
     def __get__(
         self, instance: None, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigChoiceField:
-        ...
+    ) -> ConfigChoiceField: ...
 
     @overload
     def __get__(
         self, instance: Config, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigInstanceDict:
-        ...
+    ) -> ConfigInstanceDict: ...
 
     def __get__(self, instance, owner=None, at=None, label="default"):
         if instance is None or not isinstance(instance, Config):
             return self
         else:
             return self._getOrMake(instance)
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configDictField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configField.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,22 +95,20 @@
             source=source,
             deprecated=deprecated,
         )
 
     @overload
     def __get__(
         self, instance: None, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> "ConfigField[FieldTypeVar]":
-        ...
+    ) -> "ConfigField[FieldTypeVar]": ...
 
     @overload
     def __get__(
         self, instance: Config, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> FieldTypeVar:
-        ...
+    ) -> FieldTypeVar: ...
 
     def __get__(self, instance, owner=None, at=None, label="default"):
         if instance is None or not isinstance(instance, Config):
             return self
         else:
             value = instance._storage.get(self.name, None)
             if value is None:
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/__init__.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableAction.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/_configurableAction.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/_configurableActionField.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,20 +89,18 @@
             instance._storage[self.name] = value(__name=name, __at=at, __label=label)
         history = instance._history.setdefault(self.name, [])
         history.append(("config value set", at, label))
 
     @overload
     def __get__(
         self, instance: None, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigurableActionField[ActionTypeVar]:
-        ...
+    ) -> ConfigurableActionField[ActionTypeVar]: ...
 
     @overload
-    def __get__(self, instance: Config, owner: Any = None, at: Any = None, label: str = "default") -> Any:
-        ...
+    def __get__(self, instance: Config, owner: Any = None, at: Any = None, label: str = "default") -> Any: ...
 
     def __get__(self, instance, owner=None, at=None, label="default"):
         result = super().__get__(instance, owner)
         if instance is not None:
             # ignore is due to typing resolved in overloads not translating to
             # type checker not knowing this is not a Field
             result.identity = self.name  # type: ignore
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/_configurableActionStructField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/_configurableActionStructField.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,22 +350,20 @@
                 self, instance, "Can only assign things that are subclasses of Configurable Action"
             )
         instance._storage[self.name] = value
 
     @overload
     def __get__(
         self, instance: None, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigurableActionStruct[ActionTypeVar]:
-        ...
+    ) -> ConfigurableActionStruct[ActionTypeVar]: ...
 
     @overload
     def __get__(
         self, instance: Config, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigurableActionStruct[ActionTypeVar]:
-        ...
+    ) -> ConfigurableActionStruct[ActionTypeVar]: ...
 
     def __get__(self, instance, owner=None, at=None, label="default"):
         if instance is None or not isinstance(instance, Config):
             return self
         else:
             field: ConfigurableActionStruct | None = instance._storage[self.name]
             return field
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableActions/tests.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableActions/tests.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/configurableField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/configurableField.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,22 +356,20 @@
             value = ConfigurableInstance(instance, self, at=at, label=label)
             instance._storage[self.name] = value
         return value
 
     @overload
     def __get__(
         self, instance: None, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigurableField:
-        ...
+    ) -> ConfigurableField: ...
 
     @overload
     def __get__(
         self, instance: Config, owner: Any = None, at: Any = None, label: str = "default"
-    ) -> ConfigurableInstance[FieldTypeVar]:
-        ...
+    ) -> ConfigurableInstance[FieldTypeVar]: ...
 
     def __get__(self, instance, owner=None, at=None, label="default"):
         if instance is None or not isinstance(instance, Config):
             return self
         else:
             return self.__getOrMake(instance, at=at, label=label)
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/convert.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/convert.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/dictField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/dictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/history.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/history.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/listField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/listField.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,27 +140,25 @@
 
     def __len__(self):
         return len(self._list)
 
     @overload
     def __setitem__(
         self, i: int, x: FieldTypeVar, at: Any = None, label: str = "setitem", setHistory: bool = True
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @overload
     def __setitem__(
         self,
         i: slice,
         x: Iterable[FieldTypeVar],
         at: Any = None,
         label: str = "setitem",
         setHistory: bool = True,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def __setitem__(self, i, x, at=None, label="setitem", setHistory=True):
         if self._config._frozen:
             raise FieldValidationError(self._field, self._config, "Cannot modify a frozen Config")
         if isinstance(i, slice):
             k, stop, step = i.indices(len(self))
             for j, xj in enumerate(x):
@@ -175,20 +173,18 @@
         self._list[i] = x
         if setHistory:
             if at is None:
                 at = getCallStack()
             self.history.append((list(self._list), at, label))
 
     @overload
-    def __getitem__(self, i: int) -> FieldTypeVar:
-        ...
+    def __getitem__(self, i: int) -> FieldTypeVar: ...
 
     @overload
-    def __getitem__(self, i: slice) -> MutableSequence[FieldTypeVar]:
-        ...
+    def __getitem__(self, i: slice) -> MutableSequence[FieldTypeVar]: ...
 
     def __getitem__(self, i):
         return self._list[i]
 
     def __delitem__(self, i, at=None, label="delitem", setHistory=True):
         if self._config._frozen:
             raise FieldValidationError(self._field, self._config, "Cannot modify a frozen Config")
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/rangeField.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/rangeField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/registry.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/registry.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst/pex/config/wrap.py` & `lsst_pex_config-27.2024.2200/python/lsst/pex/config/wrap.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/PKG-INFO` & `lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 27.0.0rc2
+Version: 27.2024.2200
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.10.0
 Description-Content-Type: text/x-rst
 License-File: COPYRIGHT
 License-File: LICENSE
 License-File: gpl-v3.0.txt
 License-File: bsd_license.txt
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: numpy>=1.17
```

### Comparing `lsst_pex_config-27.0.0rc2/python/lsst_pex_config.egg-info/SOURCES.txt` & `lsst_pex_config-27.2024.2200/python/lsst_pex_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/testLib.py` & `lsst_pex_config-27.2024.2200/tests/testLib.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_Config.py` & `lsst_pex_config-27.2024.2200/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test__file__.py` & `lsst_pex_config-27.2024.2200/tests/test__file__.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_configChoiceField.py` & `lsst_pex_config-27.2024.2200/tests/test_configChoiceField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_configDictField.py` & `lsst_pex_config-27.2024.2200/tests/test_configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_configurableActions.py` & `lsst_pex_config-27.2024.2200/tests/test_configurableActions.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_configurableField.py` & `lsst_pex_config-27.2024.2200/tests/test_configurableField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_dictField.py` & `lsst_pex_config-27.2024.2200/tests/test_dictField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_history.py` & `lsst_pex_config-27.2024.2200/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_listField.py` & `lsst_pex_config-27.2024.2200/tests/test_listField.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_registry.py` & `lsst_pex_config-27.2024.2200/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticket1911.py` & `lsst_pex_config-27.2024.2200/tests/test_ticket1911.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticket1914.py` & `lsst_pex_config-27.2024.2200/tests/test_ticket1914.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticket1915.py` & `lsst_pex_config-27.2024.2200/tests/test_ticket1915.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticket1929.py` & `lsst_pex_config-27.2024.2200/tests/test_ticket1929.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticket1995.py` & `lsst_pex_config-27.2024.2200/tests/test_ticket1995.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticket2818.py` & `lsst_pex_config-27.2024.2200/tests/test_ticket2818.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_ticketDM-7337.py` & `lsst_pex_config-27.2024.2200/tests/test_ticketDM-7337.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_unloaded_yaml.py` & `lsst_pex_config-27.2024.2200/tests/test_unloaded_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_pex_config-27.0.0rc2/tests/test_wrap.py` & `lsst_pex_config-27.2024.2200/tests/test_wrap.py`

 * *Files identical despite different names*

