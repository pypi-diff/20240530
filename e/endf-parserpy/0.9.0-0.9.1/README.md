# Comparing `tmp/endf_parserpy-0.9.0.tar.gz` & `tmp/endf_parserpy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endf_parserpy-0.9.0.tar", max compression
+gzip compressed data, was "endf_parserpy-0.9.1.tar", max compression
```

## Comparing `endf_parserpy-0.9.0.tar` & `endf_parserpy-0.9.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1096 2024-02-13 06:37:52.087847 endf_parserpy-0.9.0/LICENSE.MIT
--rw-r--r--   0        0        0     2457 2024-02-13 06:37:52.087847 endf_parserpy-0.9.0/README.md
--rw-r--r--   0        0        0       97 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/__init__.py
--rw-r--r--   0        0        0    20126 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/accessories.py
--rw-r--r--   0        0        0     2381 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/cmd.py
--rw-r--r--   0        0        0     1611 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/custom_exceptions.py
--rw-r--r--   0        0        0    10692 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/debugging_utils.py
--rw-r--r--   0        0        0     5969 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf6_plumbing.py
--rw-r--r--   0        0        0     5098 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_lark.py
--rw-r--r--   0        0        0    11563 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_mapping_core.py
--rw-r--r--   0        0        0    12403 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_mapping_utils.py
--rw-r--r--   0        0        0    14733 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_mappings.py
--rw-r--r--   0        0        0    45037 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_parser.py
--rw-r--r--   0        0        0     2005 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipe_utils.py
--rw-r--r--   0        0        0     4518 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/__init__.py
--rw-r--r--   0        0        0      413 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf0_mt0.py
--rw-r--r--   0        0        0      536 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf10.py
--rw-r--r--   0        0        0     1102 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf12.py
--rw-r--r--   0        0        0      612 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf13.py
--rw-r--r--   0        0        0     1338 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf14.py
--rw-r--r--   0        0        0     1051 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf15.py
--rw-r--r--   0        0        0     8312 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt451.py
--rw-r--r--   0        0        0      583 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt452.py
--rw-r--r--   0        0        0     1284 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt455.py
--rw-r--r--   0        0        0      570 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt456.py
--rw-r--r--   0        0        0     1385 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt458.py
--rw-r--r--   0        0        0      704 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt460.py
--rw-r--r--   0        0        0      476 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf23.py
--rw-r--r--   0        0        0      427 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf26.py
--rw-r--r--   0        0        0      469 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf27.py
--rw-r--r--   0        0        0      424 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf28.py
--rw-r--r--   0        0        0     6138 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf2_mt151.py
--rw-r--r--   0        0        0     2524 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf3.py
--rw-r--r--   0        0        0      684 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf31_mt452_455_456.py
--rw-r--r--   0        0        0     7057 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf32.py
--rw-r--r--   0        0        0     2569 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf33.py
--rw-r--r--   0        0        0     1605 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf34.py
--rw-r--r--   0        0        0      664 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf35.py
--rw-r--r--   0        0        0     1690 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf4.py
--rw-r--r--   0        0        0     3005 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf40.py
--rw-r--r--   0        0        0     2079 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf5.py
--rw-r--r--   0        0        0     2030 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf6.py
--rw-r--r--   0        0        0     1607 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf7.py
--rw-r--r--   0        0        0      804 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8.py
--rw-r--r--   0        0        0      681 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8_mt454.py
--rw-r--r--   0        0        0     2606 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8_mt457.py
--rw-r--r--   0        0        0      681 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8_mt459.py
--rw-r--r--   0        0        0      540 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf9.py
--rw-r--r--   0        0        0    19240 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/endf_utils.py
--rw-r--r--   0        0        0     5979 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/fortran_utils.py
--rw-r--r--   0        0        0     3717 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/logging_utils.py
--rw-r--r--   0        0        0     2295 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/math_utils.py
--rw-r--r--   0        0        0    12603 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/meta_control_utils.py
--rw-r--r--   0        0        0     2569 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/tree_utils.py
--rw-r--r--   0        0        0     4822 2024-02-13 06:37:52.091847 endf_parserpy-0.9.0/endf_parserpy/user_tools.py
--rw-r--r--   0        0        0      514 2024-02-13 06:38:02.631915 endf_parserpy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 endf_parserpy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/LICENSE.MIT
+-rw-r--r--   0        0        0     2457 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/README.md
+-rw-r--r--   0        0        0       97 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/__init__.py
+-rw-r--r--   0        0        0    20126 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/accessories.py
+-rw-r--r--   0        0        0     2485 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/cmd.py
+-rw-r--r--   0        0        0     1611 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/custom_exceptions.py
+-rw-r--r--   0        0        0    10692 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/debugging_utils.py
+-rw-r--r--   0        0        0     5969 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/endf6_plumbing.py
+-rw-r--r--   0        0        0     5098 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/endf_lark.py
+-rw-r--r--   0        0        0    11563 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/endf_mapping_core.py
+-rw-r--r--   0        0        0    12403 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/endf_mapping_utils.py
+-rw-r--r--   0        0        0    14733 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/endf_mappings.py
+-rw-r--r--   0        0        0    45434 2024-02-16 07:41:40.311188 endf_parserpy-0.9.1/endf_parserpy/endf_parser.py
+-rw-r--r--   0        0        0     2005 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipe_utils.py
+-rw-r--r--   0        0        0     4518 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/__init__.py
+-rw-r--r--   0        0        0      413 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf0_mt0.py
+-rw-r--r--   0        0        0      536 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf10.py
+-rw-r--r--   0        0        0     1102 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf12.py
+-rw-r--r--   0        0        0      612 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf13.py
+-rw-r--r--   0        0        0     1338 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf14.py
+-rw-r--r--   0        0        0     1051 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf15.py
+-rw-r--r--   0        0        0     8312 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt451.py
+-rw-r--r--   0        0        0      583 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt452.py
+-rw-r--r--   0        0        0     1284 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt455.py
+-rw-r--r--   0        0        0      570 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt456.py
+-rw-r--r--   0        0        0     1385 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt458.py
+-rw-r--r--   0        0        0      704 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt460.py
+-rw-r--r--   0        0        0      476 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf23.py
+-rw-r--r--   0        0        0      427 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf26.py
+-rw-r--r--   0        0        0      469 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf27.py
+-rw-r--r--   0        0        0      424 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf28.py
+-rw-r--r--   0        0        0     6138 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf2_mt151.py
+-rw-r--r--   0        0        0     2524 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf3.py
+-rw-r--r--   0        0        0      684 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf31_mt452_455_456.py
+-rw-r--r--   0        0        0     7057 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf32.py
+-rw-r--r--   0        0        0     2569 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf33.py
+-rw-r--r--   0        0        0     1605 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf34.py
+-rw-r--r--   0        0        0      664 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf35.py
+-rw-r--r--   0        0        0     1690 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf4.py
+-rw-r--r--   0        0        0     3005 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf40.py
+-rw-r--r--   0        0        0     2079 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf5.py
+-rw-r--r--   0        0        0     2030 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf6.py
+-rw-r--r--   0        0        0     1607 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf7.py
+-rw-r--r--   0        0        0      804 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8.py
+-rw-r--r--   0        0        0      681 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8_mt454.py
+-rw-r--r--   0        0        0     2606 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8_mt457.py
+-rw-r--r--   0        0        0      681 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8_mt459.py
+-rw-r--r--   0        0        0      540 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf9.py
+-rw-r--r--   0        0        0    19240 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/endf_utils.py
+-rw-r--r--   0        0        0     5979 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/fortran_utils.py
+-rw-r--r--   0        0        0     3717 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/logging_utils.py
+-rw-r--r--   0        0        0     2295 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/math_utils.py
+-rw-r--r--   0        0        0    12603 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/meta_control_utils.py
+-rw-r--r--   0        0        0     2569 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/tree_utils.py
+-rw-r--r--   0        0        0     4822 2024-02-16 07:41:40.315188 endf_parserpy-0.9.1/endf_parserpy/user_tools.py
+-rw-r--r--   0        0        0      514 2024-02-16 07:41:50.243152 endf_parserpy-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 endf_parserpy-0.9.1/PKG-INFO
```

### Comparing `endf_parserpy-0.9.0/LICENSE.MIT` & `endf_parserpy-0.9.1/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/README.md` & `endf_parserpy-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/accessories.py` & `endf_parserpy-0.9.1/endf_parserpy/accessories.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/cmd.py` & `endf_parserpy-0.9.1/endf_parserpy/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ############################################################
 #
 # Author(s):       Georg Schnabel
 # Email:           g.schnabel@iaea.org
 # Creation date:   2024/02/05
-# Last modified:   2024/02/05
+# Last modified:   2024/02/13
 # License:         MIT
 # Copyright (c) 2024 International Atomic Energy Agency (IAEA)
 #
 ############################################################
 
 import argparse
 import sys
@@ -26,14 +26,17 @@
     fuzzy_matching = not strict
     parser = EndfParser(
         ignore_number_mismatch=ignore_number_mismatch,
         ignore_zero_mismatch=ignore_zero_mismatch,
         fuzzy_matching=fuzzy_matching,
         ignore_varspec_mismatch=False,
         accept_spaces=False,
+        ignore_blank_lines=False,
+        ignore_send_records=False,
+        ignore_missing_tpid=False,
     )
     any_failed = False
     file_status_list = []
     for file in files:
         try:
             parser.parsefile(file)
             file_status_list.append((file, "ok"))
```

### Comparing `endf_parserpy-0.9.0/endf_parserpy/custom_exceptions.py` & `endf_parserpy-0.9.1/endf_parserpy/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/debugging_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf6_plumbing.py` & `endf_parserpy-0.9.1/endf_parserpy/endf6_plumbing.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_lark.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_lark.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_mapping_core.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_mapping_core.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_mapping_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_mappings.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_mappings.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_parser.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ############################################################
 #
 # Author(s):       Georg Schnabel
 # Email:           g.schnabel@iaea.org
 # Creation date:   2022/05/30
-# Last modified:   2024/02/12
+# Last modified:   2024/02/16
 # License:         MIT
 # Copyright (c) 2022-2024 International Atomic Energy Agency (IAEA)
 #
 ############################################################
 
 from collections.abc import Mapping
 import logging
@@ -772,14 +772,23 @@
         self.rwmode = parser_state["rwmode"]
         self.ofs = parser_state["ofs"]
         self.logbuffer.load_state(parser_state["logbuffer_state"])
         self.parse_opts = parser_state["parse_opts"]
         self.current_path = parser_state["current_path"]
 
     def should_skip_section(self, mf, mt, exclude=None, include=None):
+        if include is not None:
+            if isinstance(include, int):
+                include = (include,)
+            include = tuple(tuple(p) if hasattr(p, "__iter__") else p for p in include)
+        if exclude is not None:
+            if isinstance(exclude, int):
+                exclude = (exclude,)
+            exclude = tuple(tuple(p) if hasattr(p, "__iter__") else p for p in exclude)
+
         if exclude is None:
             if include is not None:
                 if mf not in include and (mf, mt) not in include:
                     return True
         # exclude not None
         else:
             if mf in exclude:
```

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipe_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipe_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/__init__.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf10.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf10.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf12.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf12.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf13.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf13.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf14.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf14.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf15.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf15.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt451.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt451.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt452.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt452.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt455.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt455.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt456.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt456.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt458.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt458.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf1_mt460.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf1_mt460.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf2_mt151.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf2_mt151.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf3.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf3.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf31_mt452_455_456.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf31_mt452_455_456.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf32.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf32.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf33.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf33.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf34.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf34.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf35.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf35.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf4.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf4.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf40.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf40.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf5.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf5.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf6.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf6.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf7.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf7.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8_mt454.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8_mt454.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8_mt457.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8_mt457.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf8_mt459.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf8_mt459.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_recipes/endf_recipe_mf9.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_recipes/endf_recipe_mf9.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/endf_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/endf_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/fortran_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/fortran_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/logging_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/logging_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/math_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/math_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/meta_control_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/meta_control_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/tree_utils.py` & `endf_parserpy-0.9.1/endf_parserpy/tree_utils.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/endf_parserpy/user_tools.py` & `endf_parserpy-0.9.1/endf_parserpy/user_tools.py`

 * *Files identical despite different names*

### Comparing `endf_parserpy-0.9.0/pyproject.toml` & `endf_parserpy-0.9.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "endf-parserpy"
-version = "v0.9.0"
+version = "v0.9.1"
 description = "A Python package for reading, writing, verifying and translating ENDF-6 files"
 authors = ["Georg Schnabel"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/iaea-nds/endf-parserpy"
 
 [tool.poetry.dependencies]
```

### Comparing `endf_parserpy-0.9.0/PKG-INFO` & `endf_parserpy-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endf-parserpy
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python package for reading, writing, verifying and translating ENDF-6 files
 Home-page: https://github.com/iaea-nds/endf-parserpy
 License: MIT
 Author: Georg Schnabel
 Requires-Python: >=3.6.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

