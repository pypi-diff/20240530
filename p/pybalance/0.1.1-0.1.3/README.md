# Comparing `tmp/pybalance-0.1.1.tar.gz` & `tmp/pybalance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybalance-0.1.1.tar", last modified: Thu Jan 18 11:08:57 2024, max compression
+gzip compressed data, was "pybalance-0.1.3.tar", last modified: Thu May 30 08:28:48 2024, max compression
```

## Comparing `pybalance-0.1.1.tar` & `pybalance-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-18 11:06:22.000000 pybalance-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-18 11:08:57.243712 pybalance-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-18 11:06:22.000000 pybalance-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.235712 pybalance-0.1.1/pybalance/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/genetic/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/genetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/genetic/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/genetic/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/genetic/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/genetic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/genetic/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/genetic/tests/test_genetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/lp/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/lp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18311 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/lp/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/lp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/lp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/lp/tests/test_lp_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/propensity/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/propensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16222 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/propensity/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/propensity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/propensity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/propensity/tests/test_propensity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.239712 pybalance-0.1.1/pybalance/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/sim/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/pybalance/sim/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/sim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/sim/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/sim/tests/test_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/pybalance/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27049 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/balance_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/matching_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26388 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/pybalance/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/tests/test_balance_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/tests/test_matching_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/utils/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/pybalance/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19857 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/visualization/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/visualization/history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/pybalance/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/visualization/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-18 11:06:22.000000 pybalance-0.1.1/pybalance/visualization/tests/test_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 11:08:57.243712 pybalance-0.1.1/pybalance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-18 11:08:57.000000 pybalance-0.1.1/pybalance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-01-18 11:08:57.000000 pybalance-0.1.1/pybalance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 11:08:57.000000 pybalance-0.1.1/pybalance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-18 11:08:57.000000 pybalance-0.1.1/pybalance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-18 11:08:57.000000 pybalance-0.1.1/pybalance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 11:08:57.243712 pybalance-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-18 11:06:22.000000 pybalance-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.906411 pybalance-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-30 08:24:15.000000 pybalance-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 08:28:48.906411 pybalance-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-30 08:24:15.000000 pybalance-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.886410 pybalance-0.1.3/pybalance/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/genetic/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/genetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/genetic/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/genetic/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/genetic/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/genetic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/genetic/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/genetic/tests/test_genetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/lp/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/lp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18289 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/lp/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/lp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/lp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/lp/tests/test_lp_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/propensity/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/propensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/propensity/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/propensity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/propensity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/propensity/tests/test_propensity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance/sim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  9414688 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/sim/data/pool250000-target25000-normal0-lognormal0-binary4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/sim/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.906411 pybalance-0.1.3/pybalance/sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/sim/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/sim/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/sim/tests/test_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.906411 pybalance-0.1.3/pybalance/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27049 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/balance_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/matching_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26388 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.906411 pybalance-0.1.3/pybalance/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/tests/test_balance_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/tests/test_matching_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/utils/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.906411 pybalance-0.1.3/pybalance/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19811 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/visualization/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/visualization/history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.906411 pybalance-0.1.3/pybalance/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/visualization/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-30 08:24:15.000000 pybalance-0.1.3/pybalance/visualization/tests/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:28:48.890410 pybalance-0.1.3/pybalance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 08:28:48.000000 pybalance-0.1.3/pybalance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-30 08:28:48.000000 pybalance-0.1.3/pybalance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:28:48.000000 pybalance-0.1.3/pybalance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 08:28:48.000000 pybalance-0.1.3/pybalance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 08:28:48.000000 pybalance-0.1.3/pybalance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:28:48.906411 pybalance-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-30 08:24:15.000000 pybalance-0.1.3/setup.py
```

### Comparing `pybalance-0.1.1/LICENSE` & `pybalance-0.1.3/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Bayer AG.
+Copyright (c) 2024, Bayer AG.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pybalance-0.1.1/pybalance/genetic/initialization.py` & `pybalance-0.1.3/pybalance/genetic/initialization.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/genetic/logger.py` & `pybalance-0.1.3/pybalance/genetic/logger.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/genetic/matcher.py` & `pybalance-0.1.3/pybalance/genetic/matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pybalance.genetic.initialization import GeneticMatcherInitializer
 from pybalance.genetic.logger import BasicLogger
 import torch
 
 
 def _check_fitted(matcher):
     if matcher.best_match is None:
-        raise (ValueError, "Matcher has not been fitted!")
+        raise ValueError("Matcher has not been fitted!")
 
 
 def get_global_defaults(n_candidate_populations=5000):
     """
     Get a set of reasonable default values for evolutionary configuration. We
     break parameters into two groups: evolutionary, i.e., those that govern how
     the candidate populations are mixed, and initialization, i.e., those that
```

### Comparing `pybalance-0.1.1/pybalance/genetic/tests/test_genetic.py` & `pybalance-0.1.3/pybalance/genetic/tests/test_genetic.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/lp/matcher.py` & `pybalance-0.1.3/pybalance/lp/matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     BalanceCalculator,
     split_target_pool,
 )
 
 
 def _check_fitted(matcher):
     if matcher.best_match is None:
-        raise (ValueError, "Matcher has not been fitted!")
+        raise ValueError("Matcher has not been fitted!")
 
 
 def compute_truncation_error(x: np.ndarray) -> float:
     return np.abs(x.astype(int) - x).sum() / np.abs(x).sum()
 
 
 def _rescale_for_discretization(
@@ -445,15 +445,15 @@
 
         logger.info("Solving with %d workers ..." % solver.parameters.num_workers)
         # ========= Solve===========#
         # ----- Append the important stuff for printing -----#
 
         if self.verbose:
             solution_printer = SolutionPrinter(x, abs_deltas, self)
-            status = solver.SolveWithSolutionCallback(model, solution_printer)
+            status = solver.Solve(model, solution_printer)
             logger.info("Status = %s" % solver.StatusName(status))
             logger.info(
                 "Number of solutions found: %i" % solution_printer.solution_count()
             )
         else:
             status = solver.Solve(model)
```

### Comparing `pybalance-0.1.1/pybalance/lp/tests/test_lp_matcher.py` & `pybalance-0.1.3/pybalance/lp/tests/test_lp_matcher.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/propensity/matcher.py` & `pybalance-0.1.3/pybalance/propensity/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def _check_fitted(matcher):
     if matcher.best_match is None:
-        raise (ValueError, "Matcher has not been fitted!")
+        raise ValueError("Matcher has not been fitted!")
 
 
 class PropensityScoreMatcher:
     """
     Use a propensity score model to match two populations. The Matcher searches
     randomly over hyperparameters for the propensity score model and selects the
     match that performs best according to the given optimization objective.
```

### Comparing `pybalance-0.1.1/pybalance/propensity/tests/test_propensity.py` & `pybalance-0.1.3/pybalance/propensity/tests/test_propensity.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/sim/rng.py` & `pybalance-0.1.3/pybalance/sim/rng.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,16 +179,26 @@
         n_target, std_h=20, cor_ag=0.5, p_binary=[0.3, 0.5, 0.3, 0.5], seed=seed + 1
     )
     feature_data = pd.concat([pool, target])
     feature_data.loc[:, "patient_id"] = list(range(len(feature_data)))
     return MatchingData(feature_data)
 
 
-def load_paper_dataset():
+def get_paper_dataset_path():
     """
-    Load the simulated matching dataset presented in the pybalance paper.
+    Get the path to the simulated matching dataset presented in the pybalance paper
+    (https://onlinelibrary.wiley.com/doi/10.1002/pst.2352).
     """
     filepath = "pool250000-target25000-normal0-lognormal0-binary4.parquet"
     resource = os.path.join(
         os.path.dirname(os.path.abspath(__file__)), "data", filepath
     )
+    return resource
+
+
+def load_paper_dataset():
+    """
+    Load the simulated matching dataset presented in the pybalance paper
+    (https://onlinelibrary.wiley.com/doi/10.1002/pst.2352).
+    """
+    resource = get_paper_dataset_path()
     return MatchingData(resource)
```

### Comparing `pybalance-0.1.1/pybalance/utils/__init__.py` & `pybalance-0.1.3/pybalance/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/utils/balance_calculators.py` & `pybalance-0.1.3/pybalance/utils/balance_calculators.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/utils/matching_data.py` & `pybalance-0.1.3/pybalance/utils/matching_data.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/utils/preprocess.py` & `pybalance-0.1.3/pybalance/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/utils/tests/test_balance_calculators.py` & `pybalance-0.1.3/pybalance/utils/tests/test_balance_calculators.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/utils/tests/test_matching_data.py` & `pybalance-0.1.3/pybalance/utils/tests/test_matching_data.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/utils/tests/test_preprocess.py` & `pybalance-0.1.3/pybalance/utils/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance/visualization/distributions.py` & `pybalance-0.1.3/pybalance/visualization/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Some helpful functions for plotting distribution.
 """
+
 from collections import defaultdict
 from typing import List, Optional
 import itertools
 
 import matplotlib
 
 matplotlib.use("agg")
@@ -239,17 +240,17 @@
     if standardize_difference:
         variance = frequencies["value"] * (1 - frequencies["value"]) + frequencies[
             "value_target"
         ] * (1 - frequencies["value_target"])
         frequencies.loc[:, "difference"] = frequencies.loc[:, "difference"] / np.sqrt(
             variance
         )
-        difference_label = "Standard Difference"
+        difference_label = "Std. Mean\nDifference"
     else:
-        difference_label = "Abs Difference"
+        difference_label = "Abs. Mean\nDifference"
 
     # Restrict to top features
     frequencies = frequencies.sort_values(
         [matching_data.population_col, "difference"], ascending=[False, False]
     )
     features = (
         frequencies[frequencies[matching_data.population_col] != reference_population][
@@ -271,83 +272,89 @@
     frequencies = pd.concat([pool_frequencies, non_pool_frequencies])
     plt.rc("legend", fontsize=14)
 
     if orient_horizontal:
         fig, axes = plt.subplots(
             nrows=2,
             ncols=1,
-            figsize=(len(pool_frequencies) / 2, 16),
+            figsize=(len(pool_frequencies) / 2, 8),
             gridspec_kw={"height_ratios": [1, 3]},
         )
 
         plt.subplot(2, 1, 1)
         sns.barplot(data=frequencies, y="difference", x="index", **default_params)
-        xticks, labels = plt.xticks()
-        plt.gca().set_xticks(xticks + 0.5, minor=False)
-        plt.gca().set_xticks(xticks, minor=True)
-        plt.gca().set_xticklabels([""] * len(labels), minor=True, rotation=90)
+        ticks, labels = plt.xticks()
+        ticks = np.array(ticks)
+        plt.gca().set_xticks(ticks + 0.5, minor=False)
+        plt.gca().set_xticklabels([""] * len(labels), minor=True)
+        plt.gca().set_xticklabels([""] * len(labels), minor=False)
         plt.grid(True)
         plt.axhline(
             y=0.1,
-            xmin=xticks.min(),
-            xmax=xticks.max(),
+            xmin=ticks.min(),
+            xmax=ticks.max(),
             c="k",
             lw=2.5,
             zorder=10000,
             linestyle="--",
         )
         plt.ylim([0, 0.25])
-        plt.ylabel("Abs Difference", fontsize=18)
+        plt.ylabel(difference_label, fontsize=14)
         plt.gca().get_legend().remove()
         plt.xlabel("")
 
         plt.subplot(2, 1, 2)
         sns.barplot(data=frequencies, y="value", x="index", **default_params)
-        xticks, labels = plt.xticks()
-        plt.gca().set_xticks(xticks + 0.5, minor=False)
-        plt.gca().set_xticks(xticks, minor=True)
-        plt.gca().set_xticklabels(
-            labels, minor=True, rotation=45, ha="right", fontsize=16
-        )
+        ticks, labels = plt.xticks()
+        ticks = np.array(ticks)
+        plt.gca().set_xticks(ticks, minor=True)
+        plt.gca().set_xticklabels(labels, minor=True)
+        plt.gca().set_xticks(ticks + 0.5, minor=False)
+        plt.gca().set_xticklabels([""] * len(labels), minor=False)
+        plt.xticks(rotation=90, fontsize=12, ha="right", minor=True)
         plt.grid(True)
-        plt.ylabel("Frequency", fontsize=18)
-        plt.xlabel("Feature")
+        plt.ylabel("Frequency", fontsize=14)
+        plt.xlabel("Feature", fontsize=14)
 
     else:
         fig, axes = plt.subplots(
             nrows=1,
             ncols=2,
-            figsize=(16, len(pool_frequencies) / 2),
+            figsize=(8, len(pool_frequencies) / 2),
             gridspec_kw={"width_ratios": [3, 1]},
         )
 
         plt.subplot(1, 2, 2)
         sns.barplot(data=frequencies, x="difference", y="index", **default_params)
         ticks, labels = plt.yticks()
+        ticks = np.array(ticks)
         plt.gca().set_yticks(ticks + 0.5, minor=False)
-        plt.gca().set_yticks(ticks, minor=True)
         plt.gca().set_yticklabels([""] * len(labels), minor=True)
+        plt.gca().set_yticklabels([""] * len(labels), minor=False)
         plt.grid(True)
         plt.axvline(
             x=0.1, ymin=ticks.min(), ymax=ticks.max(), c="k", lw=2.5, linestyle="--"
         )
         plt.xlim([0, 0.25])
-        plt.xlabel(difference_label, fontsize=18)
+        plt.xlabel(difference_label, fontsize=14)
         plt.gca().get_legend().remove()
         plt.ylabel("")
 
         plt.subplot(1, 2, 1)
         sns.barplot(data=frequencies, x="value", y="index", **default_params)
         ticks, labels = plt.yticks()
-        plt.gca().set_yticks(ticks + 0.5, minor=False)
+        ticks = np.array(ticks)
         plt.gca().set_yticks(ticks, minor=True)
-        plt.gca().set_yticklabels(labels, minor=True, fontsize=16)
+        plt.gca().set_yticklabels(labels, minor=True)
+        plt.gca().set_yticks(ticks + 0.5, minor=False)
+        plt.gca().set_yticklabels([""] * len(labels), minor=False)
+        plt.yticks(rotation=0, fontsize=12, minor=True)
         plt.grid(True)
-        plt.xlabel("Frequency", fontsize=18)
-        plt.ylabel("Feature")
+        plt.xlabel("Frequency", fontsize=14)
+        plt.ylabel("Feature", fontsize=14)
 
     plt.tight_layout()
     return fig
 
 
 def plot_per_feature_loss(
     matching_data: MatchingData,
@@ -453,16 +460,16 @@
     ]
 
     fig.gca().legend(handles, labels)
     plt.title(f"Contribution to {balance_calculator.name} by feature")
 
     plt.ylim(ymin=0)
     ymin, ymax = fig.gca().get_ylim()
-    plt.vlines(plt.xticks()[0] + 0.5, ymin, ymax, linewidth=0.5, color="k")
-    plt.vlines(plt.xticks()[0][0] - 0.5, ymin, ymax, linewidth=0.5, color="k")
+    plt.vlines(np.array(plt.xticks()[0]) + 0.5, ymin, ymax, linewidth=0.5, color="k")
+    plt.vlines(np.array(plt.xticks()[0]) - 0.5, ymin, ymax, linewidth=0.5, color="k")
 
     plt.xticks(rotation=90)
     xmin, xmax = plt.xticks()[0][0] - 0.5, plt.xticks()[0][-1] + 0.5
     plt.hlines(0.1, xmin, xmax, linewidth=2.5, color="k", linestyle="--")
     plt.xlim(xmin, xmax)
 
     return fig
@@ -489,15 +496,15 @@
     headers_numeric = include_only_numeric or matching_data.headers["numeric"]
     headers_categoric = include_only_categoric or matching_data.headers["categoric"]
 
     for x, y in itertools.product(headers_categoric, headers_numeric):
         g = sns.JointGrid(data=matching_data.data, x=x, y=y, **default_params)
         grids.append(g)
 
-        g.plot_joint(sns.violinplot, s=25, split=True, saturation=0.9, dodge=True)
+        g.plot_joint(sns.violinplot, split=True, saturation=0.9, dodge=True)
         g.ax_joint.grid(True)
 
         sns.histplot(
             data=matching_data.data,
             x=x,
             multiple="dodge",
             shrink=0.8,
@@ -547,25 +554,15 @@
         g = sns.JointGrid(data=matching_data.data, x=x, y=y, **default_params)
         grids.append(g)
 
         if joint_kind == "kde":
             g.plot_joint(sns.kdeplot, levels=5)
 
         elif joint_kind == "scatter":
-            # Give larger populations more alpha, so they don't overwhelm the plot
-            counts = matching_data.counts()
-            weights = (1 - counts / counts.sum()).reset_index()
-            alpha = np.clip(
-                matching_data.data.merge(weights, on=matching_data.population_col)[
-                    "N"
-                ].values,
-                0.25,
-                1,
-            )
-            g.plot_joint(sns.scatterplot, s=25, alpha=alpha)
+            g.plot_joint(sns.scatterplot, s=25)
 
         else:
             raise NotImplementedError(f"Unsupported joint_kind: {joint_kind}.")
 
         g.ax_joint.grid(True)
         g.plot_marginals(sns.histplot, bins=20, common_norm=False, stat="probability")
```

### Comparing `pybalance-0.1.1/pybalance/visualization/history.py` & `pybalance-0.1.3/pybalance/visualization/history.py`

 * *Files identical despite different names*

### Comparing `pybalance-0.1.1/pybalance.egg-info/SOURCES.txt` & `pybalance-0.1.3/pybalance.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 pybalance/lp/tests/test_lp_matcher.py
 pybalance/propensity/__init__.py
 pybalance/propensity/matcher.py
 pybalance/propensity/tests/__init__.py
 pybalance/propensity/tests/test_propensity.py
 pybalance/sim/__init__.py
 pybalance/sim/rng.py
+pybalance/sim/data/pool250000-target25000-normal0-lognormal0-binary4.parquet
 pybalance/sim/tests/__init__.py
 pybalance/sim/tests/test_datasets.py
 pybalance/sim/tests/test_sim.py
 pybalance/utils/__init__.py
 pybalance/utils/balance_calculators.py
 pybalance/utils/matching_data.py
 pybalance/utils/misc.py
```

