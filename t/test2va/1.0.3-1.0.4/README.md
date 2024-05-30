# Comparing `tmp/test2va-1.0.3.tar.gz` & `tmp/test2va-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test2va-1.0.3.tar", last modified: Thu May 30 14:01:47 2024, max compression
+gzip compressed data, was "test2va-1.0.4.tar", last modified: Thu May 30 14:06:33 2024, max compression
```

## Comparing `test2va-1.0.3.tar` & `test2va-1.0.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.489496 test2va-1.0.3/
--rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      260 2024-05-30 14:01:47.488489 test2va-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.3/README.md
--rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 14:01:47.489496 test2va-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      531 2024-05-30 14:01:40.000000 test2va-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.410292 test2va-1.0.3/test2va/
--rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.3/test2va/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.428487 test2va-1.0.3/test2va/const/
--rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.3/test2va/const/__init__.py
--rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.3/test2va/const/const.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.430059 test2va-1.0.3/test2va/generator/
--rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.3/test2va/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.437242 test2va-1.0.3/test2va/generator/core/
--rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.3/test2va/generator/core/GUI.py
--rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/generator/core/GUIMethodReader.py
--rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.3/test2va/generator/core/Method.py
--rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.3/test2va/generator/core/MethodGenerator.py
--rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/generator/core/Mutant.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/generator/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.440243 test2va-1.0.3/test2va/generator/exceptions/
--rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.3/test2va/generator/exceptions/GUIException.py
--rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.3/test2va/generator/exceptions/MethodException.py
--rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.3/test2va/generator/exceptions/MethodGeneratorException.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/generator/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/generator/generator.py
--rw-rw-rw-   0        0        0    19854 2024-05-30 13:24:35.000000 test2va-1.0.3/test2va/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.442562 test2va-1.0.3/test2va/mutator/
--rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.3/test2va/mutator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.444563 test2va-1.0.3/test2va/mutator/mappings/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/mutator/mappings/__init__.py
--rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.3/test2va/mutator/mappings/maps.py
--rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/mutator/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.453079 test2va-1.0.3/test2va/mutator/structs/
--rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/structs/EspressoActions.py
--rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/structs/EspressoCorrelations.py
--rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/structs/EspressoCriteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/structs/UiAutomator1Actions.py
--rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/structs/UiAutomator1Criteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/structs/UiAutomator2Actions.py
--rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.3/test2va/mutator/structs/UiAutomator2Criteria.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/mutator/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.466597 test2va-1.0.3/test2va/mutator/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/mutator/util/__init__.py
--rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.3/test2va/mutator/util/base_test.py
--rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.3/test2va/mutator/util/build_xpath_from_element.py
--rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.3/test2va/mutator/util/clear_user_data.py
--rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/execute_action.py
--rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/execute_assertion.py
--rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/find_assertion_correlations.py
--rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/find_element.py
--rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.3/test2va/mutator/util/find_xml_element.py
--rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.3/test2va/mutator/util/get_element_info.py
--rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/get_true_page_source.py
--rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.3/test2va/mutator/util/grant_permissions.py
--rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/populate_mutators.py
--rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/mutator/util/setup_test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.468602 test2va-1.0.3/test2va/parser/
--rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.3/test2va/parser/__init__.py
--rw-rw-rw-   0        0        0     3416 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.474111 test2va-1.0.3/test2va/parser/structs/
--rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/structs/EspressoDeclElement.py
--rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/structs/UiAutomator1ExprElement.py
--rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/structs/UiAutomator2ExprElement.py
--rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/structs/XMLElement.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/parser/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.476112 test2va-1.0.3/test2va/parser/types/
--rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.3/test2va/parser/types/LibTypes.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/parser/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.481621 test2va-1.0.3/test2va/parser/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.3/test2va/parser/util/__init__.py
--rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/util/find_all_test_methods.py
--rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/util/find_setup_method.py
--rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.3/test2va/parser/util/literal_format_check.py
--rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.3/test2va/parser/util/modify_srcml.py
--rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/parser/util/traverse_elements.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.487131 test2va-1.0.3/test2va/util/
--rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.3/test2va/util/__init__.py
--rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.3/test2va/util/camel_to_snake.py
--rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.3/test2va/util/filter_list.py
--rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.3/test2va/util/map_list.py
--rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.3/test2va/util/write_json.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:01:47.426481 test2va-1.0.3/test2va.egg-info/
--rw-rw-rw-   0        0        0      260 2024-05-30 14:01:47.000000 test2va-1.0.3/test2va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2024-05-30 14:01:47.000000 test2va-1.0.3/test2va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:01:47.000000 test2va-1.0.3/test2va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-30 14:01:47.000000 test2va-1.0.3/test2va.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-30 14:01:47.000000 test2va-1.0.3/test2va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-30 14:01:47.000000 test2va-1.0.3/test2va.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.023939 test2va-1.0.4/
+-rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      260 2024-05-30 14:06:33.022940 test2va-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.4/README.md
+-rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:06:33.023939 test2va-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      531 2024-05-30 14:06:28.000000 test2va-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.946931 test2va-1.0.4/test2va/
+-rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.4/test2va/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.962470 test2va-1.0.4/test2va/const/
+-rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.4/test2va/const/__init__.py
+-rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.4/test2va/const/const.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.964470 test2va-1.0.4/test2va/generator/
+-rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.4/test2va/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.969979 test2va-1.0.4/test2va/generator/core/
+-rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.4/test2va/generator/core/GUI.py
+-rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/generator/core/GUIMethodReader.py
+-rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.4/test2va/generator/core/Method.py
+-rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.4/test2va/generator/core/MethodGenerator.py
+-rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/generator/core/Mutant.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/generator/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.974140 test2va-1.0.4/test2va/generator/exceptions/
+-rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.4/test2va/generator/exceptions/GUIException.py
+-rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.4/test2va/generator/exceptions/MethodException.py
+-rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.4/test2va/generator/exceptions/MethodGeneratorException.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/generator/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/generator/generator.py
+-rw-rw-rw-   0        0        0    19918 2024-05-30 14:04:08.000000 test2va-1.0.4/test2va/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.976140 test2va-1.0.4/test2va/mutator/
+-rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.4/test2va/mutator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.978140 test2va-1.0.4/test2va/mutator/mappings/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/mutator/mappings/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.4/test2va/mutator/mappings/maps.py
+-rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/mutator/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.986650 test2va-1.0.4/test2va/mutator/structs/
+-rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/structs/EspressoActions.py
+-rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/structs/EspressoCorrelations.py
+-rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/structs/EspressoCriteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/structs/UiAutomator1Actions.py
+-rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/structs/UiAutomator1Criteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/structs/UiAutomator2Actions.py
+-rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.4/test2va/mutator/structs/UiAutomator2Criteria.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/mutator/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.001120 test2va-1.0.4/test2va/mutator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/mutator/util/__init__.py
+-rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.4/test2va/mutator/util/base_test.py
+-rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.4/test2va/mutator/util/build_xpath_from_element.py
+-rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.4/test2va/mutator/util/clear_user_data.py
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/execute_action.py
+-rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/execute_assertion.py
+-rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/find_assertion_correlations.py
+-rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/find_element.py
+-rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.4/test2va/mutator/util/find_xml_element.py
+-rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.4/test2va/mutator/util/get_element_info.py
+-rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/get_true_page_source.py
+-rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.4/test2va/mutator/util/grant_permissions.py
+-rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/populate_mutators.py
+-rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/mutator/util/setup_test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.003121 test2va-1.0.4/test2va/parser/
+-rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.4/test2va/parser/__init__.py
+-rw-rw-rw-   0        0        0     3416 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.008406 test2va-1.0.4/test2va/parser/structs/
+-rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/structs/EspressoDeclElement.py
+-rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/structs/UiAutomator1ExprElement.py
+-rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/structs/UiAutomator2ExprElement.py
+-rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/structs/XMLElement.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/parser/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.009911 test2va-1.0.4/test2va/parser/types/
+-rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.4/test2va/parser/types/LibTypes.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/parser/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.015921 test2va-1.0.4/test2va/parser/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.4/test2va/parser/util/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/util/find_all_test_methods.py
+-rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/util/find_setup_method.py
+-rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.4/test2va/parser/util/literal_format_check.py
+-rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.4/test2va/parser/util/modify_srcml.py
+-rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/parser/util/traverse_elements.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:33.020430 test2va-1.0.4/test2va/util/
+-rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.4/test2va/util/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.4/test2va/util/camel_to_snake.py
+-rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.4/test2va/util/filter_list.py
+-rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.4/test2va/util/map_list.py
+-rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.4/test2va/util/write_json.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:06:32.960470 test2va-1.0.4/test2va.egg-info/
+-rw-rw-rw-   0        0        0      260 2024-05-30 14:06:32.000000 test2va-1.0.4/test2va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2024-05-30 14:06:32.000000 test2va-1.0.4/test2va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:06:32.000000 test2va-1.0.4/test2va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 14:06:32.000000 test2va-1.0.4/test2va.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-05-30 14:06:32.000000 test2va-1.0.4/test2va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 14:06:32.000000 test2va-1.0.4/test2va.egg-info/top_level.txt
```

### Comparing `test2va-1.0.3/LICENSE` & `test2va-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/setup.py` & `test2va-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test2va',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     install_requires=['appium-python-client==3.1.1', 'pylibsrcml'],
     license='MIT',
     author='Anon',
     description='Test2VA',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `test2va-1.0.3/test2va/generator/core/GUI.py` & `test2va-1.0.4/test2va/generator/core/GUI.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/generator/core/GUIMethodReader.py` & `test2va-1.0.4/test2va/generator/core/GUIMethodReader.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/generator/core/Method.py` & `test2va-1.0.4/test2va/generator/core/Method.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/generator/core/MethodGenerator.py` & `test2va-1.0.4/test2va/generator/core/MethodGenerator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/generator/core/Mutant.py` & `test2va-1.0.4/test2va/generator/core/Mutant.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/generator/generator.py` & `test2va-1.0.4/test2va/generator/generator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/gui.py` & `test2va-1.0.4/test2va/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import tkinter as tk
 from tkinter import filedialog
 
 from appium.options.android.uiautomator2.base import UiAutomator2Options
 from appium import webdriver
 
-import mutator
-import parser
-import generator
+from test2va.mutator import mutator
+from test2va.parser import parser
+from test2va.generator import generator
 from util.write_json import write_json
 
 
 def browse(text):
     file_path = filedialog.askopenfilename()
     if file_path:
         text.delete(0, tk.END)
```

### Comparing `test2va-1.0.3/test2va/mutator/mappings/maps.py` & `test2va-1.0.4/test2va/mutator/mappings/maps.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/mutator.py` & `test2va-1.0.4/test2va/mutator/mutator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/structs/EspressoActions.py` & `test2va-1.0.4/test2va/mutator/structs/EspressoActions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/structs/EspressoCorrelations.py` & `test2va-1.0.4/test2va/mutator/structs/EspressoCorrelations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/structs/EspressoCriteria.py` & `test2va-1.0.4/test2va/mutator/structs/EspressoCriteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/structs/UiAutomator1Criteria.py` & `test2va-1.0.4/test2va/mutator/structs/UiAutomator1Criteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/base_test.py` & `test2va-1.0.4/test2va/mutator/util/base_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/execute_assertion.py` & `test2va-1.0.4/test2va/mutator/util/execute_assertion.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/find_assertion_correlations.py` & `test2va-1.0.4/test2va/mutator/util/find_assertion_correlations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/find_element.py` & `test2va-1.0.4/test2va/mutator/util/find_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/find_xml_element.py` & `test2va-1.0.4/test2va/mutator/util/find_xml_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/get_true_page_source.py` & `test2va-1.0.4/test2va/mutator/util/get_true_page_source.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/grant_permissions.py` & `test2va-1.0.4/test2va/mutator/util/grant_permissions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/populate_mutators.py` & `test2va-1.0.4/test2va/mutator/util/populate_mutators.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/mutator/util/setup_test.py` & `test2va-1.0.4/test2va/mutator/util/setup_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/parser.py` & `test2va-1.0.4/test2va/parser/parser.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/structs/EspressoDeclElement.py` & `test2va-1.0.4/test2va/parser/structs/EspressoDeclElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/structs/UiAutomator1ExprElement.py` & `test2va-1.0.4/test2va/parser/structs/UiAutomator1ExprElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/structs/UiAutomator2ExprElement.py` & `test2va-1.0.4/test2va/parser/structs/UiAutomator2ExprElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/structs/XMLElement.py` & `test2va-1.0.4/test2va/parser/structs/XMLElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/types/LibTypes.py` & `test2va-1.0.4/test2va/parser/types/LibTypes.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/util/find_all_test_methods.py` & `test2va-1.0.4/test2va/parser/util/find_all_test_methods.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/util/find_setup_method.py` & `test2va-1.0.4/test2va/parser/util/find_setup_method.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/util/literal_format_check.py` & `test2va-1.0.4/test2va/parser/util/literal_format_check.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/util/modify_srcml.py` & `test2va-1.0.4/test2va/parser/util/modify_srcml.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va/parser/util/traverse_elements.py` & `test2va-1.0.4/test2va/parser/util/traverse_elements.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.3/test2va.egg-info/SOURCES.txt` & `test2va-1.0.4/test2va.egg-info/SOURCES.txt`

 * *Files identical despite different names*

