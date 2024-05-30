# Comparing `tmp/ingredient_slicer-1.0.3.tar.gz` & `tmp/ingredient_slicer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-1.0.3.tar", last modified: Sat May 25 16:29:22 2024, max compression
+gzip compressed data, was "ingredient_slicer-1.0.4.tar", last modified: Thu May 30 16:50:23 2024, max compression
```

## Comparing `ingredient_slicer-1.0.3.tar` & `ingredient_slicer-1.0.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.499187 ingredient_slicer-1.0.3/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.485881 ingredient_slicer-1.0.3/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.487074 ingredient_slicer-1.0.3/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.3/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.3/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.3/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-25 16:29:22.498879 ingredient_slicer-1.0.3/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.3/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.488133 ingredient_slicer-1.0.3/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-25 13:54:14.000000 ingredient_slicer-1.0.3/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   160805 2024-05-25 15:17:43.000000 ingredient_slicer-1.0.3/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   103245 2024-05-25 16:20:12.000000 ingredient_slicer-1.0.3/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    91510 2024-05-25 15:48:42.000000 ingredient_slicer-1.0.3/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   108927 2024-05-25 16:27:13.000000 ingredient_slicer-1.0.3/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.498208 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2156 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-25 16:29:22.000000 ingredient_slicer-1.0.3/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-25 16:29:11.000000 ingredient_slicer-1.0.3/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-25 16:29:22.499246 ingredient_slicer-1.0.3/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-25 16:29:22.497952 ingredient_slicer-1.0.3/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.3/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.3/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.3/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.3/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.3/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.3/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.3/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.3/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.3/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.3/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.3/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.3/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.3/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.3/tests/test_get_single_item_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4771 2024-05-25 16:28:38.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_edge_case_foods.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4899 2024-05-25 15:50:27.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_gram_weights.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.3/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.3/tests/test_is_approximate_quantity_only_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.3/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.3/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.3/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    45639 2024-05-25 15:12:12.000000 ingredient_slicer-1.0.3/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.3/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.3/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.3/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.3/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.3/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.3/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.3/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.3/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.3/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.3/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.3/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.3/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.3/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.3/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.3/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.3/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.3/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.3/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.3/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.3/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-30 16:50:23.023923 ingredient_slicer-1.0.4/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-30 16:50:23.007166 ingredient_slicer-1.0.4/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-30 16:50:23.008464 ingredient_slicer-1.0.4/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.4/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.4/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.4/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-30 16:50:23.023545 ingredient_slicer-1.0.4/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.4/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-30 16:50:23.009553 ingredient_slicer-1.0.4/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-30 16:38:21.000000 ingredient_slicer-1.0.4/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   162205 2024-05-30 16:49:29.000000 ingredient_slicer-1.0.4/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   103424 2024-05-30 16:37:54.000000 ingredient_slicer-1.0.4/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    91510 2024-05-25 15:48:42.000000 ingredient_slicer-1.0.4/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   109357 2024-05-30 16:38:01.000000 ingredient_slicer-1.0.4/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-30 16:50:23.022636 ingredient_slicer-1.0.4/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-30 16:50:22.000000 ingredient_slicer-1.0.4/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2156 2024-05-30 16:50:23.000000 ingredient_slicer-1.0.4/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-30 16:50:22.000000 ingredient_slicer-1.0.4/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-30 16:50:22.000000 ingredient_slicer-1.0.4/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-30 16:50:22.000000 ingredient_slicer-1.0.4/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-30 16:38:33.000000 ingredient_slicer-1.0.4/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-30 16:50:23.024167 ingredient_slicer-1.0.4/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-30 16:50:23.022034 ingredient_slicer-1.0.4/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.4/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.4/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.4/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.4/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.4/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.4/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.4/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.4/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.4/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.4/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.4/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.4/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.4/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3130 2024-05-30 16:38:05.000000 ingredient_slicer-1.0.4/tests/test_get_single_item_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4771 2024-05-25 16:28:38.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer_edge_case_foods.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4899 2024-05-25 15:50:27.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-30 16:49:46.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer_gram_weights.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.4/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.4/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.4/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.4/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.4/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    45639 2024-05-25 15:12:12.000000 ingredient_slicer-1.0.4/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.4/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.4/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.4/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.4/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.4/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.4/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.4/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.4/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.4/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.4/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.4/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.4/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.4/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.4/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.4/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.4/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.4/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.4/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.4/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.4/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-1.0.3/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-1.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-1.0.4/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/.gitignore` & `ingredient_slicer-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/LICENSE` & `ingredient_slicer-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/PKG-INFO` & `ingredient_slicer-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.3
+Version: 1.0.4
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.3/README.md` & `ingredient_slicer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer/__init__.py` & `ingredient_slicer-1.0.4/ingredient_slicer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # __init__.py
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from ._ingredient_slicer import IngredientSlicer
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP, \
     PRIMARY_CATEGORIES, SECONDARY_CATEGORIES, \
```

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer/_constants.py` & `ingredient_slicer-1.0.4/ingredient_slicer/_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -881,14 +881,22 @@
             "radish": ("vegetables", "root"),
             "radishes": ("vegetables", "root"),
             "turnip": ("vegetables", "root"),
             "turnips": ("vegetables", "root"),
             "artichoke": ("vegetables", "flower"),
             "artichokes": ("vegetables", "flower"),
             "cabbage": ("vegetables", "cruciferous"),
+            "serrano chiles" : ("vegetables", "fruit"),
+            "jalapeno chiles" : ("vegetables", "fruit"),
+            "poblano chiles" : ("vegetables", "fruit"),
+            "habanero chiles" : ("vegetables", "fruit"),
+            "serrano pepper" : ("vegetables", "fruit"),
+            "jalapeno pepper" : ("vegetables", "fruit"),
+            "poblano pepper" : ("vegetables", "fruit"),
+            "habanero pepper" : ("vegetables", "fruit"),
             "bell pepper": ("vegetables", "fruit"),
             "bell peppers": ("vegetables", "fruit"),
             "yellow bell pepper": ("vegetables", "fruit"),
             "yellow bell peppers": ("vegetables", "fruit"),
             "red bell pepper": ("vegetables", "fruit"),
             "red bell peppers": ("vegetables", "fruit"),
             "green bell pepper": ("vegetables", "fruit"),
@@ -1770,16 +1778,16 @@
             "cherries": ("fruits", "stone"),
             "fig": ("fruits", "fig"),
             "figs": ("fruits", "fig"),
             "date": ("fruits", "date"),
             "dates": ("fruits", "date"),
             "pomegranate": ("fruits", "tropical"),
             "pomegranates": ("fruits", "tropical"),
-            "coconut": ("fruits", "tropical"),
-            "coconuts": ("fruits", "tropical"),
+            "coconut": ("fruits", "drupe"),
+            "coconuts": ("fruits", "drupe"),
             "passion fruit": ("fruits", "tropical"),
             "passion fruits": ("fruits", "tropical"),
             "dragon fruit": ("fruits", "tropical"),
             "dragon fruits": ("fruits", "tropical"),
             "guava": ("fruits", "tropical"),
             "guavas": ("fruits", "tropical"),
             "star fruit": ("fruits", "tropical"),
@@ -2512,72 +2520,114 @@
     "beer" : "beer",
     "beers" : "beer"
 }
 
 # A map of common food items and their weight in grams (i.e. 1 egg is approximately 56.7 grams, 1 apple is approximately 195 grams, etc.)
 SINGLE_ITEM_FOOD_WEIGHTS = {
     'egg': '56.7',
+    'eggs': '56.7',
     'apple': '195',
+    'apples': '195',
     'apricot': '35',
+    'apricots': '35',
     'avocado': '170',
+    'avocados': '170',
     'banana': '120',
+    'bananas': '120',
     'blackberry': '2.45',
+    'blackberries': '2.45',
     'blueberry': '0.5',
+    'blueberries': '0.5',
+    'cherry': '5',
     'cherries': '5',
     'coconut': '680',
+    'cocunuts': '680',
     'cranberry': '1.13',
+    'cranberries': '1.13',
+    'date': '24',
+    'dates': '24',
+    'medjool date': '24',
+    'medjool dates': '24',
     'fig': '50',
+    'figs': '50',
     'grapefruit': '246',
+    'grapefruits': '246',
+    'grape': '5',
     'grapes': '5',
     'guava': '200',
     'jackfruit': '6800',
     'durian': '6800',
     'kiwi': '75',
+    'kiwis' : '75',
+    'kiwifruit': '75',
     'lemon': '100',
+    'lemons': '100',
     'lime': '50',
+    'limes': '50',
     'mango': '200',
+    'mangos': '200',
     'cantaloupe': '1360',
+    'cantaloupes': '1360',
     'honeydew': '1800',
+    'honeydew melon': '1800',
+    'honeydew melons': '1800',
     'melon': '1500',
+    'melons' : '1500',
     'nectarine': '150',
+    'olive': '5',
     'olives': '5',
     'orange': '130',
     'papaya': '450',
     'peach': '150',
+    'peaches': '150',
     'pear': '180',
+    'pears': '180',
     'pineapple': '1590',
+    'pineapples': '1590',
     'plum': '65',
+    'plums': '65',
     'pomegranate': '255',
     'pumpkin': '4500',
     'raspberry': '5',
+    'raspberries': '5',
     'strawberry': '12',
+    'strawberries': '12',
     'watermelon': '9000',
     'artichoke': '368',
+    'artichokes': '368',
     'asparagus': '22',
+    'asparaguses': '22',
     'eggplant': '453.5',
     'garlic': '5',
     'green beans': '5',
+    'beet' : '113',
     'beets': '113',
     'bell pepper': '170',
     'broccoli': '225',
+    'broccolini' : '16',
     'brussel sprouts': '14',
     'cabbage': '9070',
     'carrots': '60',
     'cauliflower': '500',
     'celery': '450',
     'corn': '180',
+    'corns': '180',
     'cucumber': '250',
     'kale': '198',
+    'kales': '198',
     'lettuce': '650',
     'mushrooms': '15',
     'onion': '160',
     'parsnip': '115',
     'pea': '0.2',
+    'peas': '0.2',
     'potato': '184',
+    'potatoes': '184',
     'snow pea': '2.5',
+    'snow peas': '2.5',
     'spinach': '30',
     'squash': '200',
     'butternut squash': '1100',
     'sweet potato': '113',
     'tomato': '170',
     'zucchini': '200'
 }
```

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-1.0.4/ingredient_slicer/_ingredient_slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1640,16 +1640,17 @@
         return
     
     def _add_gram_weights_for_single_item_foods(self):
 
         if not self._gram_weight:
 
             # print(f'THIS IS A SINGLE ITEM FOOD: {self._food}') if self.debug else None
-            # NOTE: this is an arbitrary fuzzy string matching ratio of 0.5 for now
-            gram_weight = _utils._get_single_item_gram_weight(self._food, self._quantity, 0.5)
+            # NOTE: this is an arbitrary fuzzy string matching ratio of 0.85 for now, probably want this to be pretty strict 
+            # NOTE: so we don't get false positives (maybe even just make it 0.95 or 1 to just only match single character differences)
+            gram_weight = _utils._get_single_item_gram_weight(self._food, self._quantity, 0.85)
             
             # print(f" >>> Gram weight for single item food: {gram_weight}") if self.debug else None
             
             self._gram_weight = gram_weight
 
         return
```

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-1.0.4/ingredient_slicer/_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer/_utils.py` & `ingredient_slicer-1.0.4/ingredient_slicer/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2240,40 +2240,46 @@
     if gram_weight or unit in _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT or unit in _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT:
         return gram_weight
     
     est_weight = _estimate_single_item_gram_weights(food)
     
     return float(est_weight) * quantity if est_weight else None
 
-def _get_single_item_gram_weight(food:str, quantity:str, threshold:Union[float, None] = None) -> Union[str, None]:
+def _get_single_item_gram_weight(food:str, quantity:Union[str, int, float, None], threshold:Union[float, int, None] = 0.85) -> Union[str, None]:
 
     """ Get the weight of a single food item in grams
     Args:
         food: str, food item
-        quantity: str, quantity of the food item
-
+        quantity: str, int, or float, quantity of the food item. If None, the quantity is set to 1.
+        threshold: float, int, minimum similarity score to return a match. Score between 0 and 1, where 1 is a perfect match. Default is 0.85
     Returns:
         estimated weight of the food in grams as a string or None
     """
 
     if not isinstance(food, str):
         raise TypeError("'food' must be a string")
     
     if quantity is not None and not isinstance(quantity, (str, int, float)):
         raise TypeError("'quantity' must be a string, integer, or float")
+    
+    if threshold is not None and not isinstance(threshold, (float, int)):
+        raise TypeError("'threshold' must be a float or integer")
+    
+
 
     # food = "eggs"
     # unit = "cup"
     # unit = None
     # quantity = 1
     # gram_weight = None
     
     # set quantity to 1 if its None
-    quantity = 1 if not quantity else float(quantity)
-    
+    quantity  = 1 if not quantity else float(quantity)
+    threshold = 0.85 if not threshold else float(threshold)
+
     est_weight = _estimate_single_item_gram_weights(food,  threshold)
     
     return str(float(est_weight) * quantity) if est_weight else None
 
 
 # def _split_dimension_unit_x_ranges(ingredient: str) -> tuple[str]:
 #     """Split an ingredient string by any quantity dimension unit separated by an 'x' character.
```

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-1.0.4/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.3
+Version: 1.0.4
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.3/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-1.0.4/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/pyproject.toml` & `ingredient_slicer-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "1.0.3"
+version = "1.0.4"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-1.0.3/tests/test_avg_ranges.py` & `ingredient_slicer-1.0.4/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_casual_ingredients.py` & `ingredient_slicer-1.0.4/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-1.0.4/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-1.0.4/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-1.0.4/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_extract_dimensions.py` & `ingredient_slicer-1.0.4/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_extract_quantities_utils.py` & `ingredient_slicer-1.0.4/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_find_and_remove.py` & `ingredient_slicer-1.0.4/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-1.0.4/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-1.0.4/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_get_gram_weight.py` & `ingredient_slicer-1.0.4/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_get_single_item_gram_weight.py` & `ingredient_slicer-1.0.4/tests/test_get_single_item_gram_weight.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,45 +8,60 @@
 
 # -------------------------------------------------------------------------------
 # -------------------------------------------------------------------------------
 # ---- _get_gram_weight() tests ----
 # -------------------------------------------------------------------------------
     
 def test_get_single_item_gram_weight_one_egg():
-    assert _utils._get_single_item_gram_weight("egg", "1") == '56.7'
+    assert _utils._get_single_item_gram_weight("egg", "1", 0.5) == '56.7'
     
 def test_get_single_item_gram_weight_two_eggs():
-    assert _utils._get_single_item_gram_weight("egg", "2") == '113.4'
+    assert _utils._get_single_item_gram_weight("egg", "2", 0.5) == '113.4'
 
 def test_get_single_item_gram_weight_one_banana():
-    assert _utils._get_single_item_gram_weight("banana", "1") == '120.0'
+    assert _utils._get_single_item_gram_weight("banana", "1", 0.5) == '120.0'
 
 def test_get_single_item_gram_weight_two_bananas():
-    assert _utils._get_single_item_gram_weight("banana", "2") == '240.0'
+    assert _utils._get_single_item_gram_weight("banana", "2", 0.5) == '240.0'
 
 def test_get_single_item_gram_weight_one_and_a_half_bananas():
-    assert _utils._get_single_item_gram_weight("banana", "1.5") == '180.0'
+    assert _utils._get_single_item_gram_weight("banana", "1.5", 0.5) == '180.0'
 
 def test_get_single_item_gram_weight_one_apple():
-    assert _utils._get_single_item_gram_weight("apple", "1") == '195.0'
+    assert _utils._get_single_item_gram_weight("apple", "1", 0.5)== '195.0'
 
 def test_get_single_item_gram_weight_two_apples():
-    assert _utils._get_single_item_gram_weight("apple", "2") == '390.0'
+    assert _utils._get_single_item_gram_weight("apple", "2", 0.5)== '390.0'
 
 def test_get_single_item_gram_weight_one_egg_no_quantity():
-    assert _utils._get_single_item_gram_weight("egg", "") == '56.7'
+    assert _utils._get_single_item_gram_weight("egg", "", 0.5)== '56.7'
 
 def test_get_single_item_gram_weight_one_egg_none_quantity():
-    assert _utils._get_single_item_gram_weight("egg", None) == '56.7'
+    assert _utils._get_single_item_gram_weight("egg", None, 0.5) == '56.7'
 
 # TODO: Need to refine behavior for foods that dont have a real unit or any unit at all
 # TODO: Reference the _get_single_item_gram_weight() function that tries to take a food with no weight or volume unit 
 # TODO: and get the gram weight. _get_single_item_gram_weight() assumes that if a food has no unit and or a Non weight/volume unit (i.e. 'heads') than the ingredient 
 # TODO: is an individual item type ingredient where the food is also the unit (i.e. 2 eggs). There is a small/hacky SINGLE_ITEM_FOOD_WEIGHTS dictionary 
 # TODO:  with an average gram weight of some common single item foods (primarly fruits, vegetables, and eggs)
 def test_get_single_item_gram_weight_food_not_in_lookup_table():
-    assert _utils._get_single_item_gram_weight("olive oil", "1") ==  '5.0'
+    assert _utils._get_single_item_gram_weight("olive oil", "1", 0.5) ==  '5.0'
 
 
 def test_error_with_giving_integers_for_food_and_quantity():
     with pytest.raises(TypeError):
-        _utils._get_single_item_gram_weight(1, 1)
+        _utils._get_single_item_gram_weight(1, 1, 0.5)
+
+
+def test_strict_threshold_for_word_eggplants():
+    assert _utils._get_single_item_gram_weight("eggplants", "1", 1) is None
+
+def test_looser_threshold_for_word_eggplants():
+    assert _utils._get_single_item_gram_weight("eggplants", "1", 0.85) == '453.5'
+
+def test_multiple_repeated_matching_words():
+    assert _utils._get_single_item_gram_weight("eggplants eggplants", "1", 0.85) == '453.5'
+
+def test_strict_threshold_for_word_eggplant():
+    assert _utils._get_single_item_gram_weight("eggplant", "1", 1) == '453.5'
+
+_utils._get_single_item_gram_weight("brocollini", "1", 0.5)
```

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_edge_case_foods.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer_edge_case_foods.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_gram_weights.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer_gram_weights.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_parenthesis.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-1.0.4/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_is_approximate_quantity_only_parenthesis.py` & `ingredient_slicer-1.0.4/tests/test_is_approximate_quantity_only_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_make_int_or_float_str.py` & `ingredient_slicer-1.0.4/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-1.0.4/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_merge_numbers.py` & `ingredient_slicer-1.0.4/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_number_ranges.py` & `ingredient_slicer-1.0.4/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-1.0.4/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-1.0.4/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_parenthesis.py` & `ingredient_slicer-1.0.4/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_parenthesis_utils.py` & `ingredient_slicer-1.0.4/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_percentages.py` & `ingredient_slicer-1.0.4/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-1.0.4/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_prep_words.py` & `ingredient_slicer-1.0.4/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_quantity_range_regex.py` & `ingredient_slicer-1.0.4/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_quantity_units_regex.py` & `ingredient_slicer-1.0.4/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-1.0.4/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_remove_x_separators.py` & `ingredient_slicer-1.0.4/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-1.0.4/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_separate_dimensions.py` & `ingredient_slicer-1.0.4/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_size_modifiers.py` & `ingredient_slicer-1.0.4/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_spaced_numbers.py` & `ingredient_slicer-1.0.4/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_unit_regex.py` & `ingredient_slicer-1.0.4/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_wild_ingredients.py` & `ingredient_slicer-1.0.4/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_word_fractions.py` & `ingredient_slicer-1.0.4/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_word_numbers.py` & `ingredient_slicer-1.0.4/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.3/tests/test_x_after_number_regex.py` & `ingredient_slicer-1.0.4/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

