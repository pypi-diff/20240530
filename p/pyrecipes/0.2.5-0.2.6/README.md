# Comparing `tmp/pyrecipes-0.2.5.tar.gz` & `tmp/pyrecipes-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecipes-0.2.5.tar", last modified: Sat Apr 27 20:38:40 2024, max compression
+gzip compressed data, was "pyrecipes-0.2.6.tar", last modified: Thu May 30 17:36:31 2024, max compression
```

## Comparing `pyrecipes-0.2.5.tar` & `pyrecipes-0.2.6.tar`

### file list

```diff
@@ -1,510 +1,514 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.760682 pyrecipes-0.2.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.760682 pyrecipes-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/coverage.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.760682 pyrecipes-0.2.5/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    29470 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/imgs/python-cookbook-cover.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.760682 pyrecipes-0.2.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/requirements/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/requirements/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.736682 pyrecipes-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.760682 pyrecipes-0.2.5/src/pyrecipes/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/chapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cli/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cli/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/cookbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.736682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/01_unpacking_a_sequence_into_separate_variables/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/01_unpacking_a_sequence_into_separate_variables/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/06_mapping_keys_to_multiple_values_in_a_dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/06_mapping_keys_to_multiple_values_in_a_dictionary/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/07_keeping_dictionaries_in_order/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/07_keeping_dictionaries_in_order/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/08_calculating_with_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/08_calculating_with_dictionaries/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.764682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/09_finding_commonalities_between_two_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/09_finding_commonalities_between_two_dictionaries/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/10_removing_duplicates_from_a_sequence_while_maintaining_order/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/10_removing_duplicates_from_a_sequence_while_maintaining_order/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/11_naming_a_slice/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/11_naming_a_slice/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/12_determining_the_most_frequently_occurring_items_in_a_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/12_determining_the_most_frequently_occurring_items_in_a_sequence/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/13_sorting_a_list_of_dictionaries_by_a_common_key/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/13_sorting_a_list_of_dictionaries_by_a_common_key/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/14_sorting_objects_without_native_comparison_support/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/14_sorting_objects_without_native_comparison_support/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/15_grouping_records_together_based_on_a_field/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/15_grouping_records_together_based_on_a_field/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/16_filtering_sequence_element/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/16_filtering_sequence_element/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/17_extracting_a_subset_of_a_dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/17_extracting_a_subset_of_a_dictionary/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/18_mapping_names_to_a_sequence_of_elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/18_mapping_names_to_a_sequence_of_elements/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/19_transforming_and_reducing_data_at_the_same_time/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/19_transforming_and_reducing_data_at_the_same_time/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/20_combining_multiple_mappings_into_a_single_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/20_combining_multiple_mappings_into_a_single_mapping/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.740682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/01_splitting_strings_on_any_of_multiple_delimiters/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/01_splitting_strings_on_any_of_multiple_delimiters/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/02_matching_text_at_start_or_end_of_a_string/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/02_matching_text_at_start_or_end_of_a_string/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/03_matching_strings_using_shell_wildcard_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/03_matching_strings_using_shell_wildcard_patterns/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/04_matching_and_searching_for_text_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/04_matching_and_searching_for_text_patterns/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/05_searching_and_replacing_text/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/05_searching_and_replacing_text/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/06_searching_and_replacing_case_insensitive_text/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/06_searching_and_replacing_case_insensitive_text/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/07_specifying_a_regular_expression_for_the_shortest_match/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/07_specifying_a_regular_expression_for_the_shortest_match/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/08_writing_a_regular_expression_for_multiline_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/08_writing_a_regular_expression_for_multiline_patterns/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/09_normalizing_unicode_text_to_a_standard_representation/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/09_normalizing_unicode_text_to_a_standard_representation/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/10_working_with_unicode_characters_in_regular_expressions/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/10_working_with_unicode_characters_in_regular_expressions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.768682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/11_stripping_unwanted_characters_from_strings/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/11_stripping_unwanted_characters_from_strings/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/12_sanitizing_and_cleaning_up_text/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/12_sanitizing_and_cleaning_up_text/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/13_aligning_text_strings/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/13_aligning_text_strings/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/14_combining_and_concatenating_strings/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/14_combining_and_concatenating_strings/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/15_interpolating_variables_in_strings/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/15_interpolating_variables_in_strings/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/16_reformatting_text_to_a_fixed_number_of_columns/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/16_reformatting_text_to_a_fixed_number_of_columns/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/17_handling_html_and_xml_entities_in_text/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/17_handling_html_and_xml_entities_in_text/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/18_tokenizing_text/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/18_tokenizing_text/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/19_writing_a_simple_recursive_descent_parser/
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/19_writing_a_simple_recursive_descent_parser/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/20_performing_text_operations_on_byte_strings/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/20_performing_text_operations_on_byte_strings/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.740682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/01_rounding_numerical_values/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/01_rounding_numerical_values/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/02_performing_accurate_decimal_calculations/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/02_performing_accurate_decimal_calculations/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/03_formatting_numbers_for_output/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/03_formatting_numbers_for_output/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/04_working_with_binary_octal_and_hexidecimal_integers/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/04_working_with_binary_octal_and_hexidecimal_integers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/05_packing_and_unpacking_large_integers_from_bytes/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/05_packing_and_unpacking_large_integers_from_bytes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/06_performing_complex-valued_math/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/06_performing_complex-valued_math/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/07_working_with_infinity_and_nans/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/07_working_with_infinity_and_nans/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/08_calculating_in_fractions/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/08_calculating_in_fractions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/09_calculating_with_large_numerical_arrays/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/09_calculating_with_large_numerical_arrays/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/10_performing_matrix_and_linear_algebra_calculations/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/10_performing_matrix_and_linear_algebra_calculations/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/11_picking_things_at_random/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/11_picking_things_at_random/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/12_converting_days_to_seconds_and_other_basic_time_conversions/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/12_converting_days_to_seconds_and_other_basic_time_conversions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.772682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/13_determining_last_fridays_date/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/13_determining_last_fridays_date/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/14_finding_the_date_range_for_the_current_month/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/14_finding_the_date_range_for_the_current_month/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/15_converting_strings_into_datetimes/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/15_converting_strings_into_datetimes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/16_manipulating_dates_involving_time_zones/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/16_manipulating_dates_involving_time_zones/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.744682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/01_manually_consuming_an_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/01_manually_consuming_an_iterator/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/01_manually_consuming_an_iterator/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/02_delegating_iteration/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/02_delegating_iteration/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/03_creating_new_iteration_patterns_with_generators/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/03_creating_new_iteration_patterns_with_generators/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/04_implementing_the_iterator_protocol/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/04_implementing_the_iterator_protocol/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/05_iterating_in_reverse/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/05_iterating_in_reverse/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/07_taking_a_slice_of_an_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/07_taking_a_slice_of_an_iterator/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/08_skipping_the_first_part_of_an_iterable/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/08_skipping_the_first_part_of_an_iterable/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/08_skipping_the_first_part_of_an_iterable/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/09_iterating_over_all_possible_combinations_or_permutations/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/09_iterating_over_all_possible_combinations_or_permutations/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/10_iterating_over_the_index_value_pairs_of_a_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/10_iterating_over_the_index_value_pairs_of_a_sequence/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/11_iterating_over_multiple_sequences_simultaneously/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/11_iterating_over_multiple_sequences_simultaneously/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/12_iterating_on_items_in_separate_containers/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/12_iterating_on_items_in_separate_containers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.776682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.744682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.780682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/
--rwxr-xr-x   0 runner    (1001) docker     (127)   651619 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log
--rwxr-xr-x   0 runner    (1001) docker     (127)    46105 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0108.bz2
--rwxr-xr-x   0 runner    (1001) docker     (127)    46105 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0208.bz2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.780682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/
--rwxr-xr-x   0 runner    (1001) docker     (127)   651619 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log
--rwxr-xr-x   0 runner    (1001) docker     (127)    72261 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0108.gz
--rwxr-xr-x   0 runner    (1001) docker     (127)    72261 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0208.gz
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.780682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/14_flattening_a_nested_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/14_flattening_a_nested_sequence/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.780682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/15_iterating_in_sorted_order_over_merged_sorted_iterables/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/15_iterating_in_sorted_order_over_merged_sorted_iterables/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.780682 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/access-log
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.748682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/sample.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/02_printing_to_a_file/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/02_printing_to_a_file/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/02_printing_to_a_file/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/03_printing_with_a_different_separator_or_line_ending/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/03_printing_with_a_different_separator_or_line_ending/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/04_reading_and_writing_binary_data/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/04_reading_and_writing_binary_data/data.bin
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/04_reading_and_writing_binary_data/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/05_writing_to_a_file_that_doesnt_already_exist/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/05_writing_to_a_file_that_doesnt_already_exist/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/05_writing_to_a_file_that_doesnt_already_exist/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/06_performing_io_operations_on_a_string/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/06_performing_io_operations_on_a_string/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/somfile.bz2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/08_iterating_over_fixed_sized_records/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/08_iterating_over_fixed_sized_records/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/08_iterating_over_fixed_sized_records/somefile.data
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/sample.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/example.py
--rw-r--r--   0 runner    (1001) docker     (127)   100000 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/somefile.data
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/11_manipulating_pathnames/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/11_manipulating_pathnames/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.784682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/12_testing_for_the_existence_of_a_file/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/12_testing_for_the_existence_of_a_file/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_1/example_1_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_2/example_2_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/some_file
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/some_other_file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/example.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/jalapeño.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/15_printing_bad_filesnames/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/15_printing_bad_filesnames/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/16_adding_or_changing_the_encoding_of_an_already_open_file/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/16_adding_or_changing_the_encoding_of_an_already_open_file/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/17_writing_bytes_to_a_text_file/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/17_writing_bytes_to_a_text_file/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/somefile.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/19_making_temporary_files_or_directories/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/19_making_temporary_files_or_directories/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/20_communicating_with_serial_port/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/20_communicating_with_serial_port/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/pickled
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.748682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/stocks.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/02_reading_and_writing_json_data/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/02_reading_and_writing_json_data/data.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/02_reading_and_writing_json_data/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/sample.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.788682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    91959 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/potholes.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/05_turning_a_dictionary_into_xml/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/05_turning_a_dictionary_into_xml/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/pred.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/sample.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/08_interacting_with_a_relational_database/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/08_interacting_with_a_relational_database/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/09_decoding_and_encoding_hexadecimal_digits/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/09_decoding_and_encoding_hexadecimal_digits/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/10_decoding_and_encoding_base64/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/10_decoding_and_encoding_base64/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/data.b
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/create_poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/polys.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/13_summarizing_data_and_performing_statistics/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/13_summarizing_data_and_performing_statistics/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.748682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/01_writing_functions_that_accept_any_number_of_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/01_writing_functions_that_accept_any_number_of_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/02_writing_functions_that_only_accept_keyword_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/02_writing_functions_that_only_accept_keyword_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/03_attaching_informational_metadata_to_function_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/03_attaching_informational_metadata_to_function_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/04_returning_multiple_values_from_a_function/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/04_returning_multiple_values_from_a_function/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/05_defining_functions_with_default_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/05_defining_functions_with_default_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/06_defining_anonymous_or_inline_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/06_defining_anonymous_or_inline_functions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/07_capturing_variables_in_anonymous_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/07_capturing_variables_in_anonymous_functions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/08_making_an_n_argument_callable_work_as_a_callable_with_fewer_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/08_making_an_n_argument_callable_work_as_a_callable_with_fewer_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.792682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/09_replacing_single_method_classes_with_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/09_replacing_single_method_classes_with_functions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/10_carrying_extra_state_with_callback_functions/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/10_carrying_extra_state_with_callback_functions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/11_inlining_callback_functions/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/11_inlining_callback_functions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/12_accessing_variables_defined_inside_a_closure/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/12_accessing_variables_defined_inside_a_closure/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.752682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/01_changing_the_string_representation_of_instances/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/01_changing_the_string_representation_of_instances/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/02_customizing_string_formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/02_customizing_string_formatting/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/03_making_objects_support_the_context_management_protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/03_making_objects_support_the_context_management_protocol/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/04_saving_memory_when_creating_a_large_number_of_instances/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/04_saving_memory_when_creating_a_large_number_of_instances/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/05_encapsulating_names_in_a_class/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/05_encapsulating_names_in_a_class/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/06_creating_managed_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/06_creating_managed_attributes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/07_calling_a_method_on_a_parent_class/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/07_calling_a_method_on_a_parent_class/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/08_extending_a_property_in_a_subclass/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/08_extending_a_property_in_a_subclass/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/09_creating_a_new_kind_of_class_or_instance_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/09_creating_a_new_kind_of_class_or_instance_attribute/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/10_using_lazilly_computed_properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/10_using_lazilly_computed_properties/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/11_simplifying_the_initialization_of_a_data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/11_simplifying_the_initialization_of_a_data_structure/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/12_defining_an_interface_or_abstract_base_class/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/12_defining_an_interface_or_abstract_base_class/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/13_implementing_a_data_model_or_type_system/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/13_implementing_a_data_model_or_type_system/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/14_implementing_custom_containers/
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/14_implementing_custom_containers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/15_delegating_attribute_access/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/15_delegating_attribute_access/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/16_defining_more_than_one_constructor_in_a_class/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/16_defining_more_than_one_constructor_in_a_class/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/17_creating_an_instance_without_invoking_init/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/17_creating_an_instance_without_invoking_init/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/18_extending_classes_with_mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/18_extending_classes_with_mixins/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.796682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/19_implementing_stateful_objects_or_state_machines/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/19_implementing_stateful_objects_or_state_machines/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/20_calling_a_method_on_an_object_given_the_name_as_a_string/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/20_calling_a_method_on_an_object_given_the_name_as_a_string/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/21_implementing_the_visitor_pattern/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/21_implementing_the_visitor_pattern/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/23_managing_memory_in_cyclic_data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/23_managing_memory_in_cyclic_data_structures/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/24_making_classes_support_comparison_operations/
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/24_making_classes_support_comparison_operations/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/25_creating_cached_instances/
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/25_creating_cached_instances/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/01_putting_a_wrapper_around_a_function/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/01_putting_a_wrapper_around_a_function/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/02_preserving_function_metadata_when_writing_decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/02_preserving_function_metadata_when_writing_decorators/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/03_unwrapping_a_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/03_unwrapping_a_decorator/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/04_defining_a_decorator_that_takes_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/04_defining_a_decorator_that_takes_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/05_defining_a_decorator_with_user_adjustable_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/05_defining_a_decorator_with_user_adjustable_attributes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/06_defining_a_decorator_that_takes_an_optional_argument/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/06_defining_a_decorator_that_takes_an_optional_argument/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/07_enforcing_type_checking_on_a_function_using_a_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/07_enforcing_type_checking_on_a_function_using_a_decorator/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/08_defining_decorators_as_part_of_a_class/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/08_defining_decorators_as_part_of_a_class/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/09_defining_decorators_as_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/09_defining_decorators_as_classes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/10_applying_decorators_to_class_and_static_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/10_applying_decorators_to_class_and_static_methods/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/11_writing_decortors_that_add_arguments_to_wrapped_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/11_writing_decortors_that_add_arguments_to_wrapped_functions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/12_using_decorators_to_patch_class_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/12_using_decorators_to_patch_class_definitions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/13_using_a_metaclass_to_control_instance_creation/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/13_using_a_metaclass_to_control_instance_creation/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/14_capturing_class_attribute_definition_order/
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/14_capturing_class_attribute_definition_order/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.800682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/15_defining_a_metaclass_that_takes_optional_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/15_defining_a_metaclass_that_takes_optional_arguments/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/16_enforcing_an_argument_signature_on_args_and_kwargs/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/16_enforcing_an_argument_signature_on_args_and_kwargs/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/17_enforcing_coding_conventions_in_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/17_enforcing_coding_conventions_in_classes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/18_defining_a_class_programatically/
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/18_defining_a_class_programatically/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/19_initializing_class_members_at_definition_time/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/19_initializing_class_members_at_definition_time/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/20_implementing_multiple_dispatch_with_function_annotations/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/20_implementing_multiple_dispatch_with_function_annotations/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/21_avoiding_repetitive_proeprty_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/21_avoiding_repetitive_proeprty_methods/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/22_defining_context_managers_the_easy_way/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/22_defining_context_managers_the_easy_way/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/23_executing_code_with_local_side_effects/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/23_executing_code_with_local_side_effects/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/24_parsing_and_analyzing_python_source/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/24_parsing_and_analyzing_python_source/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/25_disassembling_python_byte_code/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/25_disassembling_python_byte_code/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/jpg.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/png.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/fill.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/line.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/02_controlling_the_import_of_everything/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/02_controlling_the_import_of_everything/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.804682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/grok.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/spam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/B/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/B/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/B/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/my_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/11_networking_and_web_programming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/11_networking_and_web_programming/01_interacting_with_http_services_as_a_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/11_networking_and_web_programming/01_interacting_with_http_services_as_a_client/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.756682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/01_starting_and_stopping_threads/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/01_starting_and_stopping_threads/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/02_determining_if_a_thread_has_started/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/02_determining_if_a_thread_has_started/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/03_communicating_between_threads/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/03_communicating_between_threads/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/07_creating_a_thread_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/07_creating_a_thread_pool/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.808682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.812682 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/
--rw-r--r--   0 runner    (1001) docker     (127)   139539 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121217.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   144283 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121218.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   138211 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121219.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   148719 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121220.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   137687 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121221.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   113107 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121222.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   115180 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121223.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   119009 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121224.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   121461 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121225.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   126602 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121226.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   131302 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121227.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   128106 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121228.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   119375 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121229.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)   121378 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121230.log.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/src/pyrecipes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/src/pyrecipes/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/src/pyrecipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-27 20:38:40.000000 pyrecipes-0.2.5/src/pyrecipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25906 2024-04-27 20:38:40.000000 pyrecipes-0.2.5/src/pyrecipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:38:40.000000 pyrecipes-0.2.5/src/pyrecipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 20:38:40.000000 pyrecipes-0.2.5/src/pyrecipes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-27 20:38:40.000000 pyrecipes-0.2.5/src/pyrecipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 20:38:40.000000 pyrecipes-0.2.5/src/pyrecipes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:38:40.816682 pyrecipes-0.2.5/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/tests/cli/test_commands_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/tests/test_chapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/tests/test_cookbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/tests/test_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-27 20:38:36.000000 pyrecipes-0.2.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.712684 pyrecipes-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.656684 pyrecipes-0.2.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.656684 pyrecipes-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 17:36:31.712684 pyrecipes-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.656684 pyrecipes-0.2.6/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    29470 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/imgs/python-cookbook-cover.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.656684 pyrecipes-0.2.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/requirements/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/requirements/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:36:31.712684 pyrecipes-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.632684 pyrecipes-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.656684 pyrecipes-0.2.6/src/pyrecipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/chapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/cookbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.632684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/01_unpacking_a_sequence_into_separate_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/01_unpacking_a_sequence_into_separate_variables/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/06_mapping_keys_to_multiple_values_in_a_dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/06_mapping_keys_to_multiple_values_in_a_dictionary/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/07_keeping_dictionaries_in_order/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/07_keeping_dictionaries_in_order/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/08_calculating_with_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/08_calculating_with_dictionaries/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/09_finding_commonalities_between_two_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/09_finding_commonalities_between_two_dictionaries/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/10_removing_duplicates_from_a_sequence_while_maintaining_order/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/10_removing_duplicates_from_a_sequence_while_maintaining_order/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/11_naming_a_slice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/11_naming_a_slice/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/12_determining_the_most_frequently_occurring_items_in_a_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/12_determining_the_most_frequently_occurring_items_in_a_sequence/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/13_sorting_a_list_of_dictionaries_by_a_common_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/13_sorting_a_list_of_dictionaries_by_a_common_key/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.660684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/14_sorting_objects_without_native_comparison_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/14_sorting_objects_without_native_comparison_support/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/15_grouping_records_together_based_on_a_field/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/15_grouping_records_together_based_on_a_field/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/16_filtering_sequence_element/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/16_filtering_sequence_element/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/17_extracting_a_subset_of_a_dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/17_extracting_a_subset_of_a_dictionary/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/18_mapping_names_to_a_sequence_of_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/18_mapping_names_to_a_sequence_of_elements/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/19_transforming_and_reducing_data_at_the_same_time/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/19_transforming_and_reducing_data_at_the_same_time/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/20_combining_multiple_mappings_into_a_single_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/20_combining_multiple_mappings_into_a_single_mapping/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.636685 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/01_splitting_strings_on_any_of_multiple_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/01_splitting_strings_on_any_of_multiple_delimiters/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/02_matching_text_at_start_or_end_of_a_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/02_matching_text_at_start_or_end_of_a_string/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/03_matching_strings_using_shell_wildcard_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/03_matching_strings_using_shell_wildcard_patterns/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/04_matching_and_searching_for_text_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/04_matching_and_searching_for_text_patterns/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/05_searching_and_replacing_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/05_searching_and_replacing_text/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/06_searching_and_replacing_case_insensitive_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/06_searching_and_replacing_case_insensitive_text/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/07_specifying_a_regular_expression_for_the_shortest_match/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/07_specifying_a_regular_expression_for_the_shortest_match/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/08_writing_a_regular_expression_for_multiline_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/08_writing_a_regular_expression_for_multiline_patterns/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/09_normalizing_unicode_text_to_a_standard_representation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/09_normalizing_unicode_text_to_a_standard_representation/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/10_working_with_unicode_characters_in_regular_expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/10_working_with_unicode_characters_in_regular_expressions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/11_stripping_unwanted_characters_from_strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/11_stripping_unwanted_characters_from_strings/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/12_sanitizing_and_cleaning_up_text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/12_sanitizing_and_cleaning_up_text/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/13_aligning_text_strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/13_aligning_text_strings/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/14_combining_and_concatenating_strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/14_combining_and_concatenating_strings/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.664684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/15_interpolating_variables_in_strings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/15_interpolating_variables_in_strings/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/16_reformatting_text_to_a_fixed_number_of_columns/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/16_reformatting_text_to_a_fixed_number_of_columns/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/17_handling_html_and_xml_entities_in_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/17_handling_html_and_xml_entities_in_text/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/18_tokenizing_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/18_tokenizing_text/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/19_writing_a_simple_recursive_descent_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/19_writing_a_simple_recursive_descent_parser/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/20_performing_text_operations_on_byte_strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/20_performing_text_operations_on_byte_strings/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.636685 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/01_rounding_numerical_values/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/01_rounding_numerical_values/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/02_performing_accurate_decimal_calculations/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/02_performing_accurate_decimal_calculations/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/03_formatting_numbers_for_output/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/03_formatting_numbers_for_output/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/04_working_with_binary_octal_and_hexidecimal_integers/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/04_working_with_binary_octal_and_hexidecimal_integers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/05_packing_and_unpacking_large_integers_from_bytes/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/05_packing_and_unpacking_large_integers_from_bytes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/06_performing_complex-valued_math/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/06_performing_complex-valued_math/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/07_working_with_infinity_and_nans/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/07_working_with_infinity_and_nans/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/08_calculating_in_fractions/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/08_calculating_in_fractions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/09_calculating_with_large_numerical_arrays/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/09_calculating_with_large_numerical_arrays/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/10_performing_matrix_and_linear_algebra_calculations/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/10_performing_matrix_and_linear_algebra_calculations/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/11_picking_things_at_random/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/11_picking_things_at_random/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/12_converting_days_to_seconds_and_other_basic_time_conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/12_converting_days_to_seconds_and_other_basic_time_conversions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/13_determining_last_fridays_date/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/13_determining_last_fridays_date/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/14_finding_the_date_range_for_the_current_month/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/14_finding_the_date_range_for_the_current_month/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/15_converting_strings_into_datetimes/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/15_converting_strings_into_datetimes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.668684 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/16_manipulating_dates_involving_time_zones/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/16_manipulating_dates_involving_time_zones/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.640684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/01_manually_consuming_an_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/01_manually_consuming_an_iterator/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/01_manually_consuming_an_iterator/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/02_delegating_iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/02_delegating_iteration/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/03_creating_new_iteration_patterns_with_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/03_creating_new_iteration_patterns_with_generators/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/04_implementing_the_iterator_protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/04_implementing_the_iterator_protocol/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/05_iterating_in_reverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/05_iterating_in_reverse/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/07_taking_a_slice_of_an_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/07_taking_a_slice_of_an_iterator/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/08_skipping_the_first_part_of_an_iterable/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/08_skipping_the_first_part_of_an_iterable/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/08_skipping_the_first_part_of_an_iterable/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/09_iterating_over_all_possible_combinations_or_permutations/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/09_iterating_over_all_possible_combinations_or_permutations/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/10_iterating_over_the_index_value_pairs_of_a_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/10_iterating_over_the_index_value_pairs_of_a_sequence/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/11_iterating_over_multiple_sequences_simultaneously/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/11_iterating_over_multiple_sequences_simultaneously/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/12_iterating_on_items_in_separate_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/12_iterating_on_items_in_separate_containers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.672685 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.640684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   651619 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46105 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0108.bz2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46105 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0208.bz2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   651619 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72261 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0108.gz
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72261 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0208.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/14_flattening_a_nested_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/14_flattening_a_nested_sequence/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/15_iterating_in_sorted_order_over_merged_sorted_iterables/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/15_iterating_in_sorted_order_over_merged_sorted_iterables/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/access-log
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.640684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/sample.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/02_printing_to_a_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/02_printing_to_a_file/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/02_printing_to_a_file/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/03_printing_with_a_different_separator_or_line_ending/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/03_printing_with_a_different_separator_or_line_ending/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.676684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/04_reading_and_writing_binary_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/04_reading_and_writing_binary_data/data.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/04_reading_and_writing_binary_data/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/05_writing_to_a_file_that_doesnt_already_exist/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/05_writing_to_a_file_that_doesnt_already_exist/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/05_writing_to_a_file_that_doesnt_already_exist/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/06_performing_io_operations_on_a_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/06_performing_io_operations_on_a_string/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/somfile.bz2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/08_iterating_over_fixed_sized_records/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/08_iterating_over_fixed_sized_records/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/08_iterating_over_fixed_sized_records/somefile.data
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/sample.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100000 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/somefile.data
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/11_manipulating_pathnames/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/11_manipulating_pathnames/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/12_testing_for_the_existence_of_a_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/12_testing_for_the_existence_of_a_file/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_1/example_1_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example_dir_2/example_2_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/some_file
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/some_other_file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/jalapeño.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/15_printing_bad_filesnames/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/15_printing_bad_filesnames/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.680684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/16_adding_or_changing_the_encoding_of_an_already_open_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/16_adding_or_changing_the_encoding_of_an_already_open_file/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/17_writing_bytes_to_a_text_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/17_writing_bytes_to_a_text_file/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/somefile.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/19_making_temporary_files_or_directories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/19_making_temporary_files_or_directories/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/20_communicating_with_serial_port/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/20_communicating_with_serial_port/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/pickled
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.644684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/stocks.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/02_reading_and_writing_json_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/02_reading_and_writing_json_data/data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/02_reading_and_writing_json_data/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/sample.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91959 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/potholes.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/05_turning_a_dictionary_into_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/05_turning_a_dictionary_into_xml/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/pred.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/sample.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/08_interacting_with_a_relational_database/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/08_interacting_with_a_relational_database/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/09_decoding_and_encoding_hexadecimal_digits/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/09_decoding_and_encoding_hexadecimal_digits/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.684684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/10_decoding_and_encoding_base64/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/10_decoding_and_encoding_base64/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/data.b
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/create_poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/polys.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/13_summarizing_data_and_performing_statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/13_summarizing_data_and_performing_statistics/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.644684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/01_writing_functions_that_accept_any_number_of_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/01_writing_functions_that_accept_any_number_of_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/02_writing_functions_that_only_accept_keyword_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/02_writing_functions_that_only_accept_keyword_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/03_attaching_informational_metadata_to_function_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/03_attaching_informational_metadata_to_function_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/04_returning_multiple_values_from_a_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/04_returning_multiple_values_from_a_function/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/05_defining_functions_with_default_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/05_defining_functions_with_default_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/06_defining_anonymous_or_inline_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/06_defining_anonymous_or_inline_functions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/07_capturing_variables_in_anonymous_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/07_capturing_variables_in_anonymous_functions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/08_making_an_n_argument_callable_work_as_a_callable_with_fewer_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/08_making_an_n_argument_callable_work_as_a_callable_with_fewer_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/09_replacing_single_method_classes_with_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/09_replacing_single_method_classes_with_functions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/10_carrying_extra_state_with_callback_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/10_carrying_extra_state_with_callback_functions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/11_inlining_callback_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/11_inlining_callback_functions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/12_accessing_variables_defined_inside_a_closure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/12_accessing_variables_defined_inside_a_closure/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.648684 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/01_changing_the_string_representation_of_instances/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/01_changing_the_string_representation_of_instances/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/02_customizing_string_formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/02_customizing_string_formatting/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/03_making_objects_support_the_context_management_protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/03_making_objects_support_the_context_management_protocol/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.688684 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/04_saving_memory_when_creating_a_large_number_of_instances/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/04_saving_memory_when_creating_a_large_number_of_instances/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/05_encapsulating_names_in_a_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/05_encapsulating_names_in_a_class/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/06_creating_managed_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/06_creating_managed_attributes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/07_calling_a_method_on_a_parent_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/07_calling_a_method_on_a_parent_class/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/08_extending_a_property_in_a_subclass/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/08_extending_a_property_in_a_subclass/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/09_creating_a_new_kind_of_class_or_instance_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/09_creating_a_new_kind_of_class_or_instance_attribute/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/10_using_lazilly_computed_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/10_using_lazilly_computed_properties/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/11_simplifying_the_initialization_of_a_data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/11_simplifying_the_initialization_of_a_data_structure/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/12_defining_an_interface_or_abstract_base_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/12_defining_an_interface_or_abstract_base_class/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/13_implementing_a_data_model_or_type_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/13_implementing_a_data_model_or_type_system/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/14_implementing_custom_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/14_implementing_custom_containers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/15_delegating_attribute_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/15_delegating_attribute_access/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/16_defining_more_than_one_constructor_in_a_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/16_defining_more_than_one_constructor_in_a_class/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/17_creating_an_instance_without_invoking_init/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/17_creating_an_instance_without_invoking_init/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/18_extending_classes_with_mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/18_extending_classes_with_mixins/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/19_implementing_stateful_objects_or_state_machines/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/19_implementing_stateful_objects_or_state_machines/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/20_calling_a_method_on_an_object_given_the_name_as_a_string/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/20_calling_a_method_on_an_object_given_the_name_as_a_string/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/21_implementing_the_visitor_pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/21_implementing_the_visitor_pattern/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/23_managing_memory_in_cyclic_data_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/23_managing_memory_in_cyclic_data_structures/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/24_making_classes_support_comparison_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/24_making_classes_support_comparison_operations/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/25_creating_cached_instances/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/25_creating_cached_instances/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.692685 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/01_putting_a_wrapper_around_a_function/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/01_putting_a_wrapper_around_a_function/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/02_preserving_function_metadata_when_writing_decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/02_preserving_function_metadata_when_writing_decorators/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/03_unwrapping_a_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/03_unwrapping_a_decorator/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/04_defining_a_decorator_that_takes_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/04_defining_a_decorator_that_takes_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/05_defining_a_decorator_with_user_adjustable_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/05_defining_a_decorator_with_user_adjustable_attributes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/06_defining_a_decorator_that_takes_an_optional_argument/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/06_defining_a_decorator_that_takes_an_optional_argument/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/07_enforcing_type_checking_on_a_function_using_a_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/07_enforcing_type_checking_on_a_function_using_a_decorator/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/08_defining_decorators_as_part_of_a_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/08_defining_decorators_as_part_of_a_class/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/09_defining_decorators_as_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/09_defining_decorators_as_classes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/10_applying_decorators_to_class_and_static_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/10_applying_decorators_to_class_and_static_methods/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/11_writing_decortors_that_add_arguments_to_wrapped_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/11_writing_decortors_that_add_arguments_to_wrapped_functions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/12_using_decorators_to_patch_class_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/12_using_decorators_to_patch_class_definitions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/13_using_a_metaclass_to_control_instance_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/13_using_a_metaclass_to_control_instance_creation/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/14_capturing_class_attribute_definition_order/
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/14_capturing_class_attribute_definition_order/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/15_defining_a_metaclass_that_takes_optional_arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/15_defining_a_metaclass_that_takes_optional_arguments/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/16_enforcing_an_argument_signature_on_args_and_kwargs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/16_enforcing_an_argument_signature_on_args_and_kwargs/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/17_enforcing_coding_conventions_in_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/17_enforcing_coding_conventions_in_classes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/18_defining_a_class_programatically/
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/18_defining_a_class_programatically/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/19_initializing_class_members_at_definition_time/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/19_initializing_class_members_at_definition_time/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/20_implementing_multiple_dispatch_with_function_annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/20_implementing_multiple_dispatch_with_function_annotations/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/21_avoiding_repetitive_proeprty_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/21_avoiding_repetitive_proeprty_methods/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/22_defining_context_managers_the_easy_way/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/22_defining_context_managers_the_easy_way/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.696684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/23_executing_code_with_local_side_effects/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/23_executing_code_with_local_side_effects/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/24_parsing_and_analyzing_python_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/24_parsing_and_analyzing_python_source/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/25_disassembling_python_byte_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/25_disassembling_python_byte_code/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/jpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/formats/png.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/src/graphics/primitive/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/02_controlling_the_import_of_everything/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/02_controlling_the_import_of_everything/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/grok.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/A/spam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/B/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/B/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/B/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/src/my_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.700684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/my_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/src/my_module/b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/11_networking_and_web_programming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/11_networking_and_web_programming/01_interacting_with_http_services_as_a_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/11_networking_and_web_programming/01_interacting_with_http_services_as_a_client/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.652685 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/01_starting_and_stopping_threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/01_starting_and_stopping_threads/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/02_determining_if_a_thread_has_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/02_determining_if_a_thread_has_started/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/03_communicating_between_threads/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/03_communicating_between_threads/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/07_creating_a_thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/07_creating_a_thread_pool/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.704684 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.708685 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)   139539 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121217.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   144283 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121218.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   138211 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121219.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   148719 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121220.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   137687 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121221.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   113107 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121222.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   115180 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121223.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   119009 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121224.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   121461 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121225.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   126602 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121226.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   131302 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121227.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   128106 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121228.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   119375 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121229.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   121378 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121230.log.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.708685 pyrecipes-0.2.6/src/pyrecipes/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/templates/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/templates/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.708685 pyrecipes-0.2.6/src/pyrecipes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/src/pyrecipes/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.708685 pyrecipes-0.2.6/src/pyrecipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 17:36:31.000000 pyrecipes-0.2.6/src/pyrecipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26018 2024-05-30 17:36:31.000000 pyrecipes-0.2.6/src/pyrecipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:36:31.000000 pyrecipes-0.2.6/src/pyrecipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 17:36:31.000000 pyrecipes-0.2.6/src/pyrecipes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 17:36:31.000000 pyrecipes-0.2.6/src/pyrecipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 17:36:31.000000 pyrecipes-0.2.6/src/pyrecipes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.708685 pyrecipes-0.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:31.708685 pyrecipes-0.2.6/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/tests/cli/test_commands_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/tests/test_chapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/tests/test_cookbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/tests/test_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-30 17:36:24.000000 pyrecipes-0.2.6/tests/test_utils.py
```

### Comparing `pyrecipes-0.2.5/.github/dependabot.yml` & `pyrecipes-0.2.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/.github/workflows/ci.yml` & `pyrecipes-0.2.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/.github/workflows/publish.yml` & `pyrecipes-0.2.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/.gitignore` & `pyrecipes-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/LICENSE` & `pyrecipes-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/PKG-INFO` & `pyrecipes-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecipes
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI tool to display useful Python recipes.
 Author-email: Chris Adams <cfh1990@msn.com>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/pyrecipes/
 Project-URL: Repository, https://github.com/ChrisA87/pyrecipes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyrecipes-0.2.5/README.md` & `pyrecipes-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/coverage.svg` & `pyrecipes-0.2.6/coverage.svg`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/imgs/python-cookbook-cover.jpeg` & `pyrecipes-0.2.6/imgs/python-cookbook-cover.jpeg`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/pyproject.toml` & `pyrecipes-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/requirements/dev-requirements.txt` & `pyrecipes-0.2.6/requirements/dev-requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile requirements/dev-requirements.in
 #
-black==24.4.0
+black==24.4.2
     # via -r dev-requirements.in
 click==8.1.7
     # via
     #   -c requirements.txt
     #   black
-coverage==7.4.4
+coverage==7.5.1
     # via -r dev-requirements.in
 exceptiongroup==1.2.0
     # via pytest
 flake8==7.0.0
     # via -r dev-requirements.in
 iniconfig==2.0.0
     # via pytest
@@ -26,21 +26,21 @@
     # via
     #   black
     #   pytest
 pathspec==0.12.1
     # via black
 platformdirs==4.1.0
     # via black
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pycodestyle==2.11.1
     # via flake8
 pyflakes==3.2.0
     # via flake8
-pytest==8.1.1
+pytest==8.2.1
     # via -r dev-requirements.in
 tomli==2.0.1
     # via
     #   black
     #   pytest
 typing-extensions==4.9.0
     # via black
```

### Comparing `pyrecipes-0.2.5/src/pyrecipes/chapter.py` & `pyrecipes-0.2.6/src/pyrecipes/chapter.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/cli/ls.py` & `pyrecipes-0.2.6/src/pyrecipes/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/cli/search.py` & `pyrecipes-0.2.6/src/pyrecipes/cli/search.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/cookbook.py` & `pyrecipes-0.2.6/src/pyrecipes/cookbook.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipe.py` & `pyrecipes-0.2.6/src/pyrecipes/recipe.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/06_mapping_keys_to_multiple_values_in_a_dictionary/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/06_mapping_keys_to_multiple_values_in_a_dictionary/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/08_calculating_with_dictionaries/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/08_calculating_with_dictionaries/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/09_finding_commonalities_between_two_dictionaries/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/09_finding_commonalities_between_two_dictionaries/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/10_removing_duplicates_from_a_sequence_while_maintaining_order/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/10_removing_duplicates_from_a_sequence_while_maintaining_order/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/11_naming_a_slice/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/11_naming_a_slice/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/12_determining_the_most_frequently_occurring_items_in_a_sequence/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/12_determining_the_most_frequently_occurring_items_in_a_sequence/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/13_sorting_a_list_of_dictionaries_by_a_common_key/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/13_sorting_a_list_of_dictionaries_by_a_common_key/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/14_sorting_objects_without_native_comparison_support/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/14_sorting_objects_without_native_comparison_support/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/15_grouping_records_together_based_on_a_field/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/15_grouping_records_together_based_on_a_field/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/16_filtering_sequence_element/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/16_filtering_sequence_element/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/17_extracting_a_subset_of_a_dictionary/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/17_extracting_a_subset_of_a_dictionary/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/18_mapping_names_to_a_sequence_of_elements/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/18_mapping_names_to_a_sequence_of_elements/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/19_transforming_and_reducing_data_at_the_same_time/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/19_transforming_and_reducing_data_at_the_same_time/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/01_data_structures_and_algorithms/20_combining_multiple_mappings_into_a_single_mapping/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/01_data_structures_and_algorithms/20_combining_multiple_mappings_into_a_single_mapping/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/01_splitting_strings_on_any_of_multiple_delimiters/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/01_splitting_strings_on_any_of_multiple_delimiters/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/02_matching_text_at_start_or_end_of_a_string/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/02_matching_text_at_start_or_end_of_a_string/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/03_matching_strings_using_shell_wildcard_patterns/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/03_matching_strings_using_shell_wildcard_patterns/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/04_matching_and_searching_for_text_patterns/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/04_matching_and_searching_for_text_patterns/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/05_searching_and_replacing_text/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/05_searching_and_replacing_text/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/06_searching_and_replacing_case_insensitive_text/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/06_searching_and_replacing_case_insensitive_text/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/07_specifying_a_regular_expression_for_the_shortest_match/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/07_specifying_a_regular_expression_for_the_shortest_match/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/08_writing_a_regular_expression_for_multiline_patterns/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/08_writing_a_regular_expression_for_multiline_patterns/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/09_normalizing_unicode_text_to_a_standard_representation/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/09_normalizing_unicode_text_to_a_standard_representation/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/10_working_with_unicode_characters_in_regular_expressions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/10_working_with_unicode_characters_in_regular_expressions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/11_stripping_unwanted_characters_from_strings/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/11_stripping_unwanted_characters_from_strings/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/12_sanitizing_and_cleaning_up_text/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/12_sanitizing_and_cleaning_up_text/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/15_interpolating_variables_in_strings/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/15_interpolating_variables_in_strings/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/16_reformatting_text_to_a_fixed_number_of_columns/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/16_reformatting_text_to_a_fixed_number_of_columns/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/17_handling_html_and_xml_entities_in_text/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/17_handling_html_and_xml_entities_in_text/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/18_tokenizing_text/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/18_tokenizing_text/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/19_writing_a_simple_recursive_descent_parser/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/19_writing_a_simple_recursive_descent_parser/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/02_strings_and_text/20_performing_text_operations_on_byte_strings/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/02_strings_and_text/20_performing_text_operations_on_byte_strings/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/01_rounding_numerical_values/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/01_rounding_numerical_values/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/02_performing_accurate_decimal_calculations/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/02_performing_accurate_decimal_calculations/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/03_formatting_numbers_for_output/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/03_formatting_numbers_for_output/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/04_working_with_binary_octal_and_hexidecimal_integers/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/04_working_with_binary_octal_and_hexidecimal_integers/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/05_packing_and_unpacking_large_integers_from_bytes/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/05_packing_and_unpacking_large_integers_from_bytes/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/06_performing_complex-valued_math/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/06_performing_complex-valued_math/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/07_working_with_infinity_and_nans/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/07_working_with_infinity_and_nans/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/08_calculating_in_fractions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/08_calculating_in_fractions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/09_calculating_with_large_numerical_arrays/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/09_calculating_with_large_numerical_arrays/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/10_performing_matrix_and_linear_algebra_calculations/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/10_performing_matrix_and_linear_algebra_calculations/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/11_picking_things_at_random/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/11_picking_things_at_random/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/12_converting_days_to_seconds_and_other_basic_time_conversions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/12_converting_days_to_seconds_and_other_basic_time_conversions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/13_determining_last_fridays_date/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/13_determining_last_fridays_date/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/14_finding_the_date_range_for_the_current_month/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/14_finding_the_date_range_for_the_current_month/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/03_numbers_dates_and_times/16_manipulating_dates_involving_time_zones/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/03_numbers_dates_and_times/16_manipulating_dates_involving_time_zones/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/02_delegating_iteration/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/02_delegating_iteration/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/03_creating_new_iteration_patterns_with_generators/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/03_creating_new_iteration_patterns_with_generators/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/04_implementing_the_iterator_protocol/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/04_implementing_the_iterator_protocol/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/05_iterating_in_reverse/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/05_iterating_in_reverse/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/06_defining_a_generator_function_with_extra_state/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/09_iterating_over_all_possible_combinations_or_permutations/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/09_iterating_over_all_possible_combinations_or_permutations/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/11_iterating_over_multiple_sequences_simultaneously/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/11_iterating_over_multiple_sequences_simultaneously/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/12_iterating_on_items_in_separate_containers/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/12_iterating_on_items_in_separate_containers/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0108.bz2` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0108.bz2`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0208.bz2` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/bar/access-log-0208.bz2`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0108.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0108.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0208.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/data/foo/access-log-0208.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/13_creating_data_processing_pipelines/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/14_flattening_a_nested_sequence/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/14_flattening_a_nested_sequence/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/04_iterators_and_generators/16_replacing_infinite_while_loops_with_an_iterator/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/01_reading_and_writing_text_files/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/07_reading_and_writing_compressed_datafiles/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/09_reading_binary_data_into_a_mutable_buffer/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/10_memory_mapping_binary_files/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/13_getting_a_directory_listing/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/14_bypassing_filename_encoding/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/16_adding_or_changing_the_encoding_of_an_already_open_file/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/16_adding_or_changing_the_encoding_of_an_already_open_file/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/18_wrapping_an_existing_file_descriptor_as_a_file_object/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/19_making_temporary_files_or_directories/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/19_making_temporary_files_or_directories/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/20_communicating_with_serial_port/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/20_communicating_with_serial_port/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/05_files_and_io/21_serializing_python_objects/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/01_reading_and_writing_csv_data/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/sample.xml` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/03_parsing_simple_xml_data/sample.xml`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/potholes.xml` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/04_parsing_huge_xml_files_incrementally/potholes.xml`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/05_turning_a_dictionary_into_xml/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/05_turning_a_dictionary_into_xml/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/06_parsing_modifying_and_rewriting_xml/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/07_parsing_xml_documents_with_namespaces/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/08_interacting_with_a_relational_database/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/08_interacting_with_a_relational_database/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/11_reading_and_writing_binary_arrays_of_structures/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/create_poly.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/create_poly.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/12_reading_nested_and_variable_sized_binary_structures/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/06_data_encoding_and_processing/13_summarizing_data_and_performing_statistics/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/06_data_encoding_and_processing/13_summarizing_data_and_performing_statistics/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/01_writing_functions_that_accept_any_number_of_arguments/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/01_writing_functions_that_accept_any_number_of_arguments/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/02_writing_functions_that_only_accept_keyword_arguments/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/02_writing_functions_that_only_accept_keyword_arguments/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/06_defining_anonymous_or_inline_functions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/06_defining_anonymous_or_inline_functions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/07_capturing_variables_in_anonymous_functions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/07_capturing_variables_in_anonymous_functions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/08_making_an_n_argument_callable_work_as_a_callable_with_fewer_arguments/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/08_making_an_n_argument_callable_work_as_a_callable_with_fewer_arguments/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/09_replacing_single_method_classes_with_functions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/09_replacing_single_method_classes_with_functions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/10_carrying_extra_state_with_callback_functions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/10_carrying_extra_state_with_callback_functions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/11_inlining_callback_functions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/11_inlining_callback_functions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/07_functions/12_accessing_variables_defined_inside_a_closure/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/07_functions/12_accessing_variables_defined_inside_a_closure/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/02_customizing_string_formatting/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/02_customizing_string_formatting/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/03_making_objects_support_the_context_management_protocol/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/03_making_objects_support_the_context_management_protocol/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/05_encapsulating_names_in_a_class/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/05_encapsulating_names_in_a_class/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/06_creating_managed_attributes/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/06_creating_managed_attributes/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/07_calling_a_method_on_a_parent_class/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/07_calling_a_method_on_a_parent_class/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/08_extending_a_property_in_a_subclass/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/08_extending_a_property_in_a_subclass/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/09_creating_a_new_kind_of_class_or_instance_attribute/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/09_creating_a_new_kind_of_class_or_instance_attribute/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/10_using_lazilly_computed_properties/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/10_using_lazilly_computed_properties/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/11_simplifying_the_initialization_of_a_data_structure/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/11_simplifying_the_initialization_of_a_data_structure/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/12_defining_an_interface_or_abstract_base_class/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/12_defining_an_interface_or_abstract_base_class/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/13_implementing_a_data_model_or_type_system/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/13_implementing_a_data_model_or_type_system/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/14_implementing_custom_containers/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/14_implementing_custom_containers/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/15_delegating_attribute_access/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/15_delegating_attribute_access/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/16_defining_more_than_one_constructor_in_a_class/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/16_defining_more_than_one_constructor_in_a_class/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/17_creating_an_instance_without_invoking_init/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/17_creating_an_instance_without_invoking_init/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/18_extending_classes_with_mixins/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/18_extending_classes_with_mixins/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/19_implementing_stateful_objects_or_state_machines/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/19_implementing_stateful_objects_or_state_machines/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/20_calling_a_method_on_an_object_given_the_name_as_a_string/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/20_calling_a_method_on_an_object_given_the_name_as_a_string/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/21_implementing_the_visitor_pattern/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/21_implementing_the_visitor_pattern/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/node.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/22_implementing_the_visitor_pattern_without_recursion/node.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/23_managing_memory_in_cyclic_data_structures/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/23_managing_memory_in_cyclic_data_structures/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/24_making_classes_support_comparison_operations/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/24_making_classes_support_comparison_operations/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/08_classes_and_objects/25_creating_cached_instances/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/08_classes_and_objects/25_creating_cached_instances/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/01_putting_a_wrapper_around_a_function/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/01_putting_a_wrapper_around_a_function/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/02_preserving_function_metadata_when_writing_decorators/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/02_preserving_function_metadata_when_writing_decorators/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/03_unwrapping_a_decorator/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/03_unwrapping_a_decorator/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/04_defining_a_decorator_that_takes_arguments/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/04_defining_a_decorator_that_takes_arguments/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/05_defining_a_decorator_with_user_adjustable_attributes/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/05_defining_a_decorator_with_user_adjustable_attributes/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/06_defining_a_decorator_that_takes_an_optional_argument/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/06_defining_a_decorator_that_takes_an_optional_argument/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/07_enforcing_type_checking_on_a_function_using_a_decorator/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/07_enforcing_type_checking_on_a_function_using_a_decorator/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/08_defining_decorators_as_part_of_a_class/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/08_defining_decorators_as_part_of_a_class/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/09_defining_decorators_as_classes/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/09_defining_decorators_as_classes/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/10_applying_decorators_to_class_and_static_methods/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/10_applying_decorators_to_class_and_static_methods/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/11_writing_decortors_that_add_arguments_to_wrapped_functions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/11_writing_decortors_that_add_arguments_to_wrapped_functions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/12_using_decorators_to_patch_class_definitions/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/12_using_decorators_to_patch_class_definitions/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/13_using_a_metaclass_to_control_instance_creation/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/13_using_a_metaclass_to_control_instance_creation/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/14_capturing_class_attribute_definition_order/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/14_capturing_class_attribute_definition_order/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/15_defining_a_metaclass_that_takes_optional_arguments/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/15_defining_a_metaclass_that_takes_optional_arguments/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/16_enforcing_an_argument_signature_on_args_and_kwargs/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/16_enforcing_an_argument_signature_on_args_and_kwargs/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/17_enforcing_coding_conventions_in_classes/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/17_enforcing_coding_conventions_in_classes/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/18_defining_a_class_programatically/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/18_defining_a_class_programatically/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/19_initializing_class_members_at_definition_time/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/19_initializing_class_members_at_definition_time/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/20_implementing_multiple_dispatch_with_function_annotations/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/20_implementing_multiple_dispatch_with_function_annotations/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/21_avoiding_repetitive_proeprty_methods/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/21_avoiding_repetitive_proeprty_methods/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/22_defining_context_managers_the_easy_way/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/22_defining_context_managers_the_easy_way/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/23_executing_code_with_local_side_effects/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/23_executing_code_with_local_side_effects/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/24_parsing_and_analyzing_python_source/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/24_parsing_and_analyzing_python_source/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/09_metaprogramming/25_disassembling_python_byte_code/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/09_metaprogramming/25_disassembling_python_byte_code/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/01_making_a_hierarchical_package_of_modules/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/02_controlling_the_import_of_everything/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/02_controlling_the_import_of_everything/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/03_importing_package_submodules_using_relative_names/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/10_modules_and_packages/04_splitting_a_module_into_multiple_files/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/11_networking_and_web_programming/01_interacting_with_http_services_as_a_client/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/11_networking_and_web_programming/01_interacting_with_http_services_as_a_client/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/01_starting_and_stopping_threads/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/01_starting_and_stopping_threads/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/02_determining_if_a_thread_has_started/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/02_determining_if_a_thread_has_started/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/03_communicating_between_threads/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/03_communicating_between_threads/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/07_creating_a_thread_pool/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/07_creating_a_thread_pool/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/example.py` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/example.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121217.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121217.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121218.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121218.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121219.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121219.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121220.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121220.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121221.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121221.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121222.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121222.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121223.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121223.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121224.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121224.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121225.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121225.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121226.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121226.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121227.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121227.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121228.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121228.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121229.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121229.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121230.log.gz` & `pyrecipes-0.2.6/src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121230.log.gz`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/utils/cli.py` & `pyrecipes-0.2.6/src/pyrecipes/utils/cli.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes/utils/text.py` & `pyrecipes-0.2.6/src/pyrecipes/utils/text.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/src/pyrecipes.egg-info/PKG-INFO` & `pyrecipes-0.2.6/src/pyrecipes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecipes
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI tool to display useful Python recipes.
 Author-email: Chris Adams <cfh1990@msn.com>
 License: MIT
 Project-URL: Homepage, https://pypi.org/project/pyrecipes/
 Project-URL: Repository, https://github.com/ChrisA87/pyrecipes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyrecipes-0.2.5/src/pyrecipes.egg-info/SOURCES.txt` & `pyrecipes-0.2.6/src/pyrecipes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 requirements/requirements.in
 requirements/requirements.txt
 src/pyrecipes/__init__.py
 src/pyrecipes/chapter.py
 src/pyrecipes/cookbook.py
 src/pyrecipes/errors.py
 src/pyrecipes/recipe.py
-src/pyrecipes/template.py
 src/pyrecipes.egg-info/PKG-INFO
 src/pyrecipes.egg-info/SOURCES.txt
 src/pyrecipes.egg-info/dependency_links.txt
 src/pyrecipes.egg-info/entry_points.txt
 src/pyrecipes.egg-info/requires.txt
 src/pyrecipes.egg-info/top_level.txt
 src/pyrecipes/cli/__init__.py
 src/pyrecipes/cli/chapters.py
 src/pyrecipes/cli/ls.py
 src/pyrecipes/cli/run.py
 src/pyrecipes/cli/search.py
 src/pyrecipes/cli/show.py
+src/pyrecipes/cli/template.py
 src/pyrecipes/recipes/__init__.py
 src/pyrecipes/recipes/01_data_structures_and_algorithms/01_unpacking_a_sequence_into_separate_variables/example.py
 src/pyrecipes/recipes/01_data_structures_and_algorithms/02_unpacking_elements_from_iterables_of_arbitrary_length/example.py
 src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/example.py
 src/pyrecipes/recipes/01_data_structures_and_algorithms/03_keep_last_n_items/somefile.txt
 src/pyrecipes/recipes/01_data_structures_and_algorithms/04_finding_largest_or_smallest_n_items/example.py
 src/pyrecipes/recipes/01_data_structures_and_algorithms/05_implementing_a_priority_queue/example.py
@@ -274,14 +274,17 @@
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121224.log.gz
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121225.log.gz
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121226.log.gz
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121227.log.gz
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121228.log.gz
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121229.log.gz
 src/pyrecipes/recipes/12_concurrency/08_performing_simple_parallel_programming/logs/20121230.log.gz
+src/pyrecipes/templates/.gitignore
+src/pyrecipes/templates/pyproject.toml
+src/pyrecipes/templates/recipe.py
 src/pyrecipes/utils/__init__.py
 src/pyrecipes/utils/cli.py
 src/pyrecipes/utils/text.py
 tests/conftest.py
 tests/test_chapter.py
 tests/test_cookbook.py
 tests/test_recipe.py
```

### Comparing `pyrecipes-0.2.5/tests/cli/test_commands_basic.py` & `pyrecipes-0.2.6/tests/cli/test_commands_basic.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/tests/conftest.py` & `pyrecipes-0.2.6/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
-from pyrecipes import COOKBOOK_DIR, TEMPLATE_PATH
+from pyrecipes import COOKBOOK_DIR, TEMPLATE_DIR
 import pyrecipes
 from pyrecipes.recipe import Recipe
 
 
-TEMPLATE = TEMPLATE_PATH.read_text()
+TEMPLATE = (TEMPLATE_DIR / "recipe.py").read_text()
 
 
 @pytest.fixture(params=list(COOKBOOK_DIR.glob("**/example.py")))
 def recipe_path(request):
     """Iters over every recipe."""
     yield request.param.parent
```

### Comparing `pyrecipes-0.2.5/tests/test_chapter.py` & `pyrecipes-0.2.6/tests/test_chapter.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/tests/test_cookbook.py` & `pyrecipes-0.2.6/tests/test_cookbook.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/tests/test_recipe.py` & `pyrecipes-0.2.6/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `pyrecipes-0.2.5/tests/test_utils.py` & `pyrecipes-0.2.6/tests/test_utils.py`

 * *Files identical despite different names*

