# Comparing `tmp/test2va-1.0.1.tar.gz` & `tmp/test2va-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test2va-1.0.1.tar", last modified: Thu May 30 13:50:15 2024, max compression
+gzip compressed data, was "test2va-1.0.2.tar", last modified: Thu May 30 13:58:09 2024, max compression
```

## Comparing `test2va-1.0.1.tar` & `test2va-1.0.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.314485 test2va-1.0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      253 2024-05-30 13:50:15.313478 test2va-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.1/README.md
--rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 13:50:15.314485 test2va-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      524 2024-05-30 13:48:05.000000 test2va-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.243026 test2va-1.0.1/test2va/
--rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.1/test2va/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.253050 test2va-1.0.1/test2va/const/
--rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.1/test2va/const/__init__.py
--rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.1/test2va/const/const.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.255555 test2va-1.0.1/test2va/generator/
--rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.1/test2va/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.261070 test2va-1.0.1/test2va/generator/core/
--rw-rw-rw-   0        0        0    10657 2024-05-29 18:54:05.000000 test2va-1.0.1/test2va/generator/core/GUI.py
--rw-rw-rw-   0        0        0     4180 2024-05-29 18:54:05.000000 test2va-1.0.1/test2va/generator/core/GUIMethodReader.py
--rw-rw-rw-   0        0        0    10232 2024-05-29 18:54:05.000000 test2va-1.0.1/test2va/generator/core/Method.py
--rw-rw-rw-   0        0        0    24672 2024-05-30 13:24:35.000000 test2va-1.0.1/test2va/generator/core/MethodGenerator.py
--rw-rw-rw-   0        0        0     7071 2024-05-29 18:54:05.000000 test2va-1.0.1/test2va/generator/core/Mutant.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/generator/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.265590 test2va-1.0.1/test2va/generator/exceptions/
--rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.1/test2va/generator/exceptions/GUIException.py
--rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.1/test2va/generator/exceptions/MethodException.py
--rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.1/test2va/generator/exceptions/MethodGeneratorException.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/generator/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1322 2024-05-29 18:54:05.000000 test2va-1.0.1/test2va/generator/generator.py
--rw-rw-rw-   0        0        0    19854 2024-05-30 13:24:35.000000 test2va-1.0.1/test2va/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.267590 test2va-1.0.1/test2va/mutator/
--rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.1/test2va/mutator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.268589 test2va-1.0.1/test2va/mutator/mappings/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/mutator/mappings/__init__.py
--rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.1/test2va/mutator/mappings/maps.py
--rw-rw-rw-   0        0        0     7184 2024-05-29 18:51:39.000000 test2va-1.0.1/test2va/mutator/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.277608 test2va-1.0.1/test2va/mutator/structs/
--rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/structs/EspressoActions.py
--rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/structs/EspressoCorrelations.py
--rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/structs/EspressoCriteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/structs/UiAutomator1Actions.py
--rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/structs/UiAutomator1Criteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/structs/UiAutomator2Actions.py
--rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.1/test2va/mutator/structs/UiAutomator2Criteria.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/mutator/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.292129 test2va-1.0.1/test2va/mutator/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/mutator/util/__init__.py
--rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.1/test2va/mutator/util/base_test.py
--rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.1/test2va/mutator/util/build_xpath_from_element.py
--rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.1/test2va/mutator/util/clear_user_data.py
--rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/execute_action.py
--rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/execute_assertion.py
--rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/find_assertion_correlations.py
--rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/find_element.py
--rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.1/test2va/mutator/util/find_xml_element.py
--rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.1/test2va/mutator/util/get_element_info.py
--rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/get_true_page_source.py
--rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.1/test2va/mutator/util/grant_permissions.py
--rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/populate_mutators.py
--rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/mutator/util/setup_test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.294138 test2va-1.0.1/test2va/parser/
--rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.1/test2va/parser/__init__.py
--rw-rw-rw-   0        0        0     3496 2024-05-29 18:52:44.000000 test2va-1.0.1/test2va/parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.299144 test2va-1.0.1/test2va/parser/structs/
--rw-rw-rw-   0        0        0    16668 2024-05-29 18:52:04.000000 test2va-1.0.1/test2va/parser/structs/EspressoDeclElement.py
--rw-rw-rw-   0        0        0    15949 2024-05-29 18:51:00.000000 test2va-1.0.1/test2va/parser/structs/UiAutomator1ExprElement.py
--rw-rw-rw-   0        0        0    12630 2024-05-29 18:51:39.000000 test2va-1.0.1/test2va/parser/structs/UiAutomator2ExprElement.py
--rw-rw-rw-   0        0        0     6348 2024-05-29 18:57:54.000000 test2va-1.0.1/test2va/parser/structs/XMLElement.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/parser/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.301144 test2va-1.0.1/test2va/parser/types/
--rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.1/test2va/parser/types/LibTypes.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/parser/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.306599 test2va-1.0.1/test2va/parser/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.1/test2va/parser/util/__init__.py
--rw-rw-rw-   0        0        0     1042 2024-05-29 18:52:14.000000 test2va-1.0.1/test2va/parser/util/find_all_test_methods.py
--rw-rw-rw-   0        0        0     1057 2024-05-29 18:52:25.000000 test2va-1.0.1/test2va/parser/util/find_setup_method.py
--rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.1/test2va/parser/util/literal_format_check.py
--rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.1/test2va/parser/util/modify_srcml.py
--rw-rw-rw-   0        0        0      777 2024-05-29 18:50:00.000000 test2va-1.0.1/test2va/parser/util/traverse_elements.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.312109 test2va-1.0.1/test2va/util/
--rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.1/test2va/util/__init__.py
--rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.1/test2va/util/camel_to_snake.py
--rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.1/test2va/util/filter_list.py
--rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.1/test2va/util/map_list.py
--rw-rw-rw-   0        0        0      188 2024-05-29 18:52:50.000000 test2va-1.0.1/test2va/util/write_json.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:50:15.250537 test2va-1.0.1/test2va.egg-info/
--rw-rw-rw-   0        0        0      253 2024-05-30 13:50:15.000000 test2va-1.0.1/test2va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2024-05-30 13:50:15.000000 test2va-1.0.1/test2va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 13:50:15.000000 test2va-1.0.1/test2va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-30 13:50:15.000000 test2va-1.0.1/test2va.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-30 13:50:15.000000 test2va-1.0.1/test2va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-30 13:50:15.000000 test2va-1.0.1/test2va.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.679488 test2va-1.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      253 2024-05-30 13:58:09.678488 test2va-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.2/README.md
+-rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:58:09.679488 test2va-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      524 2024-05-30 13:58:07.000000 test2va-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.601740 test2va-1.0.2/test2va/
+-rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.2/test2va/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.616793 test2va-1.0.2/test2va/const/
+-rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.2/test2va/const/__init__.py
+-rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.2/test2va/const/const.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.618793 test2va-1.0.2/test2va/generator/
+-rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.2/test2va/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.624303 test2va-1.0.2/test2va/generator/core/
+-rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.2/test2va/generator/core/GUI.py
+-rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/generator/core/GUIMethodReader.py
+-rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.2/test2va/generator/core/Method.py
+-rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.2/test2va/generator/core/MethodGenerator.py
+-rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/generator/core/Mutant.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/generator/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.629099 test2va-1.0.2/test2va/generator/exceptions/
+-rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.2/test2va/generator/exceptions/GUIException.py
+-rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.2/test2va/generator/exceptions/MethodException.py
+-rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.2/test2va/generator/exceptions/MethodGeneratorException.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/generator/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/generator/generator.py
+-rw-rw-rw-   0        0        0    19854 2024-05-30 13:24:35.000000 test2va-1.0.2/test2va/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.630605 test2va-1.0.2/test2va/mutator/
+-rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.2/test2va/mutator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.632610 test2va-1.0.2/test2va/mutator/mappings/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/mutator/mappings/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.2/test2va/mutator/mappings/maps.py
+-rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/mutator/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.640610 test2va-1.0.2/test2va/mutator/structs/
+-rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/structs/EspressoActions.py
+-rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/structs/EspressoCorrelations.py
+-rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/structs/EspressoCriteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/structs/UiAutomator1Actions.py
+-rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/structs/UiAutomator1Criteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/structs/UiAutomator2Actions.py
+-rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.2/test2va/mutator/structs/UiAutomator2Criteria.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/mutator/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.655352 test2va-1.0.2/test2va/mutator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/mutator/util/__init__.py
+-rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.2/test2va/mutator/util/base_test.py
+-rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.2/test2va/mutator/util/build_xpath_from_element.py
+-rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.2/test2va/mutator/util/clear_user_data.py
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/execute_action.py
+-rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/execute_assertion.py
+-rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/find_assertion_correlations.py
+-rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/find_element.py
+-rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.2/test2va/mutator/util/find_xml_element.py
+-rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.2/test2va/mutator/util/get_element_info.py
+-rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/get_true_page_source.py
+-rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.2/test2va/mutator/util/grant_permissions.py
+-rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/populate_mutators.py
+-rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/mutator/util/setup_test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.657352 test2va-1.0.2/test2va/parser/
+-rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.2/test2va/parser/__init__.py
+-rw-rw-rw-   0        0        0     3416 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.662914 test2va-1.0.2/test2va/parser/structs/
+-rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/structs/EspressoDeclElement.py
+-rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/structs/UiAutomator1ExprElement.py
+-rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/structs/UiAutomator2ExprElement.py
+-rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/structs/XMLElement.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/parser/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.664915 test2va-1.0.2/test2va/parser/types/
+-rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.2/test2va/parser/types/LibTypes.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/parser/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.671418 test2va-1.0.2/test2va/parser/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.2/test2va/parser/util/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/util/find_all_test_methods.py
+-rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/util/find_setup_method.py
+-rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.2/test2va/parser/util/literal_format_check.py
+-rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.2/test2va/parser/util/modify_srcml.py
+-rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/parser/util/traverse_elements.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.677488 test2va-1.0.2/test2va/util/
+-rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.2/test2va/util/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.2/test2va/util/camel_to_snake.py
+-rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.2/test2va/util/filter_list.py
+-rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.2/test2va/util/map_list.py
+-rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.2/test2va/util/write_json.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:58:09.614789 test2va-1.0.2/test2va.egg-info/
+-rw-rw-rw-   0        0        0      253 2024-05-30 13:58:09.000000 test2va-1.0.2/test2va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2024-05-30 13:58:09.000000 test2va-1.0.2/test2va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:58:09.000000 test2va-1.0.2/test2va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 13:58:09.000000 test2va-1.0.2/test2va.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-30 13:58:09.000000 test2va-1.0.2/test2va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 13:58:09.000000 test2va-1.0.2/test2va.egg-info/top_level.txt
```

### Comparing `test2va-1.0.1/LICENSE` & `test2va-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/setup.py` & `test2va-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test2va',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     install_requires=['appium-python-client', 'pylibsrcml'],
     license='MIT',
     author='Anon',
     description='Test2VA',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `test2va-1.0.1/test2va/generator/core/GUI.py` & `test2va-1.0.2/test2va/generator/core/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from test2va.test2va.generator.exceptions.GUIException import GUIException
+from test2va.generator.exceptions.GUIException import GUIException
 
 TEXT_FEATURE_CONSTANT_STRING: str = 'text'
 CONTENT_DESCRIPTION_FEATURE_CONSTANT_STRING: str = 'content-desc'
 RESOURCE_ID_FEATURE_CONSTANT_STRING: str = 'resource-id'
 CLASS_FEATURE_CONSTANT_STRING: str = 'class'
 DISPLAYED_FEATURE_CONSTANT_STRING: str = 'displayed'
```

### Comparing `test2va-1.0.1/test2va/generator/core/GUIMethodReader.py` & `test2va-1.0.2/test2va/generator/core/GUIMethodReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import re
 from typing import TextIO
 
-from test2va.test2va.generator.core.GUI import GUIEvent, GUIMethod, GUIElement, GUIControl
-from test2va.test2va.generator.core.GUI import (TEXT_FEATURE_CONSTANT_STRING, CONTENT_DESCRIPTION_FEATURE_CONSTANT_STRING,
+from test2va.generator.core.GUI import GUIEvent, GUIMethod, GUIElement, GUIControl
+from test2va.generator.core.GUI import (TEXT_FEATURE_CONSTANT_STRING, CONTENT_DESCRIPTION_FEATURE_CONSTANT_STRING,
                                             RESOURCE_ID_FEATURE_CONSTANT_STRING, CLASS_FEATURE_CONSTANT_STRING, 
                                             DISPLAYED_FEATURE_CONSTANT_STRING)
 
 
 def get_class_name_from_xpath(xpath: str):
     pattern = r"\/\/(.*?)\["
     match = re.search(pattern, xpath)
```

### Comparing `test2va-1.0.1/test2va/generator/core/Method.py` & `test2va-1.0.2/test2va/generator/core/Method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from test2va.test2va.generator.core.GUI import GUIEvent, GUIMethod
-from test2va.test2va.generator.exceptions.MethodException import MethodException
+from test2va.generator.core.GUI import GUIEvent, GUIMethod
+from test2va.generator.exceptions.MethodException import MethodException
 from queue import Queue
 
 TEXT_IDENTIFIER_CONSTANT = 'text'
 CD_IDENTIFIER_CONSTANT = 'content-desc'
 TAB_CONSTANT = "    "
 END_OF_STATEMENT_CONSTANT = ";\n"
```

### Comparing `test2va-1.0.1/test2va/generator/core/MethodGenerator.py` & `test2va-1.0.2/test2va/generator/core/MethodGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import copy
 import json
 from typing import TextIO, Dict, Union, Any, List
 import os
 from queue import Queue
 
-from test2va.test2va.generator.core.GUI import GUIEvent, GUIMethod, GUIElement, GUIControl
-from test2va.test2va.generator.core.Mutant import MutantInfoPerEvent
-from test2va.test2va.generator.exceptions.MethodGeneratorException import MethodGeneratorException
-from test2va.test2va.generator.core.Method import Statement, Header
+from test2va.generator.core.GUI import GUIEvent, GUIMethod, GUIElement, GUIControl
+from test2va.generator.core.Mutant import MutantInfoPerEvent
+from test2va.generator.exceptions.MethodGeneratorException import MethodGeneratorException
+from test2va.generator.core.Method import Statement, Header
 
 TAB_CONSTANT = "    "
 END_OF_STATEMENT_CONSTANT = ";\n"
 
 
 # def write_header_java(method: GUIMethod, method_file: TextIO):
 #
```

### Comparing `test2va-1.0.1/test2va/generator/core/Mutant.py` & `test2va-1.0.2/test2va/generator/core/Mutant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from test2va.test2va.generator.core import GUIMethodReader
-from test2va.test2va.generator.core.GUI import GUIElement, GUIEvent, GUIControl
+from test2va.generator.core import GUIMethodReader
+from test2va.generator.core.GUI import GUIElement, GUIEvent, GUIControl
 
 
 class MutantException(Exception):
     def __init__(self, message):
         super().__init__(message)
```

### Comparing `test2va-1.0.1/test2va/generator/generator.py` & `test2va-1.0.2/test2va/generator/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-from test2va.test2va.generator.core.GUIMethodReader import get_gui_method
-from test2va.test2va.generator.core.MethodGenerator import generate
+from test2va.generator.core.GUIMethodReader import get_gui_method
+from test2va.generator.core.MethodGenerator import generate
 import os
 
 from .core.GUI import GUIMethod
 
 
 # Define the folder path
 def generator(input_path):
```

### Comparing `test2va-1.0.1/test2va/gui.py` & `test2va-1.0.2/test2va/gui.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/mappings/maps.py` & `test2va-1.0.2/test2va/mutator/mappings/maps.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/mutator.py` & `test2va-1.0.2/test2va/mutator/mutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from appium.webdriver.common.appiumby import AppiumBy
 from appium.webdriver.webdriver import WebDriver
 from selenium.common import TimeoutException, NoSuchElementException, StaleElementReferenceException
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 
-from test2va.test2va.const.const import FIND_ELEMENT_WAIT
-from test2va.test2va.mutator.mappings.maps import AssertionCorrelationMap
-from test2va.test2va.mutator.util.base_test import base_test
-from test2va.test2va.mutator.util.clear_user_data import clear_user_data
-from test2va.test2va.mutator.util.execute_action import execute_action
-from test2va.test2va.mutator.util.execute_assertion import execute_assertion
-from test2va.test2va.mutator.util.find_assertion_correlations import find_correlations
-from test2va.test2va.mutator.util.find_element import find_element
-from test2va.test2va.mutator.util.get_element_info import get_element_info
-from test2va.test2va.mutator.util.grant_permissions import grant_permissions
-from test2va.test2va.mutator.util.setup_test import setup_test
-from test2va.test2va.parser.types.LibTypes import ParsedData
-from test2va.test2va.util.camel_to_snake import camel_to_snake
+from test2va.const.const import FIND_ELEMENT_WAIT
+from test2va.mutator.mappings.maps import AssertionCorrelationMap
+from test2va.mutator.util.base_test import base_test
+from test2va.mutator.util.clear_user_data import clear_user_data
+from test2va.mutator.util.execute_action import execute_action
+from test2va.mutator.util.execute_assertion import execute_assertion
+from test2va.mutator.util.find_assertion_correlations import find_correlations
+from test2va.mutator.util.find_element import find_element
+from test2va.mutator.util.get_element_info import get_element_info
+from test2va.mutator.util.grant_permissions import grant_permissions
+from test2va.mutator.util.setup_test import setup_test
+from test2va.parser.types.LibTypes import ParsedData
+from test2va.util.camel_to_snake import camel_to_snake
 
 
 def mutator(driver: WebDriver, data: ParsedData, auto_grant_perms):
     # Where the potential mutators are stored.
     mutators = []
 
     app_id = driver.current_package
```

### Comparing `test2va-1.0.1/test2va/mutator/structs/EspressoActions.py` & `test2va-1.0.2/test2va/mutator/structs/EspressoActions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/structs/EspressoCorrelations.py` & `test2va-1.0.2/test2va/mutator/structs/EspressoCorrelations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/structs/EspressoCriteria.py` & `test2va-1.0.2/test2va/mutator/structs/EspressoCriteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/structs/UiAutomator1Criteria.py` & `test2va-1.0.2/test2va/mutator/structs/UiAutomator1Criteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/base_test.py` & `test2va-1.0.2/test2va/mutator/util/base_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/execute_assertion.py` & `test2va-1.0.2/test2va/mutator/util/execute_assertion.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/find_assertion_correlations.py` & `test2va-1.0.2/test2va/mutator/util/find_assertion_correlations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/find_element.py` & `test2va-1.0.2/test2va/mutator/util/find_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/find_xml_element.py` & `test2va-1.0.2/test2va/mutator/util/find_xml_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/get_true_page_source.py` & `test2va-1.0.2/test2va/mutator/util/get_true_page_source.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/grant_permissions.py` & `test2va-1.0.2/test2va/mutator/util/grant_permissions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/populate_mutators.py` & `test2va-1.0.2/test2va/mutator/util/populate_mutators.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/mutator/util/setup_test.py` & `test2va-1.0.2/test2va/mutator/util/setup_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/parser/parser.py` & `test2va-1.0.2/test2va/parser/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import shutil
 import os
 import xml.etree.ElementTree as ET
 from typing import Literal
 
-from test2va.test2va.const.const import NSURL
-from test2va.test2va.parser.structs.UiAutomator1ExprElement import UiAutomator1ExprElement
-from test2va.test2va.parser.structs.UiAutomator2ExprElement import UiAutomator2ExprElement
-from test2va.test2va.parser.structs.EspressoDeclElement import EspressoDeclElement
-from test2va.test2va.parser.types.LibTypes import ParsedData
-from test2va.test2va.parser.util.find_all_test_methods import find_all_test_methods
-from test2va.test2va.parser.util.find_setup_method import find_setup_method
-from test2va.test2va.parser.util.modify_srcml import modify_srcml
-from test2va.test2va.parser.util.traverse_elements import traverse_elements
-from test2va.test2va.util.write_json import write_json
+from test2va.const.const import NSURL
+from test2va.parser.structs.UiAutomator1ExprElement import UiAutomator1ExprElement
+from test2va.parser.structs.UiAutomator2ExprElement import UiAutomator2ExprElement
+from test2va.parser.structs.EspressoDeclElement import EspressoDeclElement
+from test2va.parser.types.LibTypes import ParsedData
+from test2va.parser.util.find_all_test_methods import find_all_test_methods
+from test2va.parser.util.find_setup_method import find_setup_method
+from test2va.parser.util.modify_srcml import modify_srcml
+from test2va.parser.util.traverse_elements import traverse_elements
+from test2va.util.write_json import write_json
 
 
 def parser(file_name, gui):
     # srcml must be installed on the local machine.
     # The module has a hard time finding the dll path.
     try:
         modify_srcml(gui.srcml_input_text.get())
```

### Comparing `test2va-1.0.1/test2va/parser/structs/EspressoDeclElement.py` & `test2va-1.0.2/test2va/parser/structs/EspressoDeclElement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Literal
 
-from test2va.test2va.const.const import NSURL
-from test2va.test2va.parser.structs.XMLElement import XMLElement
-from test2va.test2va.parser.types.LibTypes import ActionData, CriteriaData, NestedCriteria, SelectorData, ActionArg, AssertionData, \
+from test2va.const.const import NSURL
+from test2va.parser.structs.XMLElement import XMLElement
+from test2va.parser.types.LibTypes import ActionData, CriteriaData, NestedCriteria, SelectorData, ActionArg, AssertionData, \
     NestedActionArg, CriteriaArgument
-from test2va.test2va.parser.util.literal_format_check import literal_format_check
-from test2va.test2va.util.filter_list import filter_list
-from test2va.test2va.util.map_list import map_list
+from test2va.parser.util.literal_format_check import literal_format_check
+from test2va.util.filter_list import filter_list
+from test2va.util.map_list import map_list
 
 
 class EspressoDeclElement(XMLElement):
 
     def __init__(self, tag: str, attrib: dict = {}, **extra):
         super().__init__(tag, attrib, **extra)
         # This is assigned after this is constructed.
```

### Comparing `test2va-1.0.1/test2va/parser/structs/UiAutomator1ExprElement.py` & `test2va-1.0.2/test2va/parser/structs/UiAutomator1ExprElement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
-from test2va.test2va.const.const import NSURL
-from test2va.test2va.parser.structs.XMLElement import XMLElement
-from test2va.test2va.parser.types.LibTypes import ActionData, CriteriaArgument, CriteriaData, NestedCriteria, SelectorData, ActionArg, AssertionData
-from test2va.test2va.parser.util.literal_format_check import literal_format_check
-from test2va.test2va.util.filter_list import filter_list
-from test2va.test2va.util.map_list import map_list
+from test2va.const.const import NSURL
+from test2va.parser.structs.XMLElement import XMLElement
+from test2va.parser.types.LibTypes import ActionData, CriteriaArgument, CriteriaData, NestedCriteria, SelectorData, ActionArg, AssertionData
+from test2va.parser.util.literal_format_check import literal_format_check
+from test2va.util.filter_list import filter_list
+from test2va.util.map_list import map_list
 
 UIS1_NESTED_SELECTOR_NAMES = ["childSelector", "fromParent"]
 
 
 class UiAutomator1ExprElement(XMLElement):
 
     def __init__(self, tag: str, attrib: dict = {}, **extra):
```

### Comparing `test2va-1.0.1/test2va/parser/structs/UiAutomator2ExprElement.py` & `test2va-1.0.2/test2va/parser/structs/UiAutomator2ExprElement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 
-from test2va.test2va.const.const import NSURL
-from test2va.test2va.parser.structs.XMLElement import XMLElement
-from test2va.test2va.parser.types.LibTypes import ActionData, CriteriaData, NestedCriteria, SelectorData, ActionArg, AssertionData, \
+from test2va.const.const import NSURL
+from test2va.parser.structs.XMLElement import XMLElement
+from test2va.parser.types.LibTypes import ActionData, CriteriaData, NestedCriteria, SelectorData, ActionArg, AssertionData, \
     NestedActionArg, CriteriaArgument
-from test2va.test2va.parser.util.literal_format_check import literal_format_check
-from test2va.test2va.util.filter_list import filter_list
-from test2va.test2va.util.map_list import map_list
+from test2va.parser.util.literal_format_check import literal_format_check
+from test2va.util.filter_list import filter_list
+from test2va.util.map_list import map_list
 
 
 class UiAutomator2ExprElement(XMLElement):
 
     def __init__(self, tag: str, attrib: dict = {}, **extra):
         super().__init__(tag, attrib, **extra)
         # This is assigned after this is constructed.
```

### Comparing `test2va-1.0.1/test2va/parser/structs/XMLElement.py` & `test2va-1.0.2/test2va/parser/structs/XMLElement.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,39 +121,39 @@
     def set_index(self, index: int):
         self._index = index
 
     def index(self, **kwargs) -> int:
         return self._index
 
     def as_uis1(self) -> "UiSelector1ExprElement":
-        from test2va.test2va.parser.structs.UiAutomator1ExprElement import UiAutomator1ExprElement as UIA1E
+        from test2va.parser.structs.UiAutomator1ExprElement import UiAutomator1ExprElement as UIA1E
         u_expr = UIA1E(self.tag, self.attrib)
         u_expr.tag = self.tag
         u_expr.attrib = self.attrib
         u_expr._text = self._text
         u_expr._parent = self._parent
         u_expr._depth = self._depth
         u_expr._index = self._index
         u_expr._element = self
         return u_expr
 
     def as_uia2(self) -> "UiAutomator2ExprElement":
-        from test2va.test2va.parser.structs.UiAutomator2ExprElement import UiAutomator2ExprElement as UIA2E
+        from test2va.parser.structs.UiAutomator2ExprElement import UiAutomator2ExprElement as UIA2E
         u2_expr = UIA2E(self)
         u2_expr.tag = self.tag
         u2_expr.attrib = self.attrib
         u2_expr.text = self.text
         u2_expr._parent = self._parent
         u2_expr._depth = self._depth
         u2_expr._index = self._index
         u2_expr._element = self
         return u2_expr
 
     def as_espresso_decl(self) -> "EspressoDeclElement":
-        from test2va.test2va.parser.structs.EspressoDeclElement import EspressoDeclElement as EDE
+        from test2va.parser.structs.EspressoDeclElement import EspressoDeclElement as EDE
         e_decl = EDE(self)
         e_decl.tag = self.tag
         e_decl.attrib = self.attrib
         e_decl.text = self.text
         e_decl._parent = self._parent
         e_decl._depth = self._depth
         e_decl._index = self._index
```

### Comparing `test2va-1.0.1/test2va/parser/types/LibTypes.py` & `test2va-1.0.2/test2va/parser/types/LibTypes.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/parser/util/find_all_test_methods.py` & `test2va-1.0.2/test2va/parser/util/find_all_test_methods.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from test2va.test2va.const.const import NSURL
-from test2va.test2va.parser.structs.XMLElement import XMLElement
+from test2va.const.const import NSURL
+from test2va.parser.structs.XMLElement import XMLElement
 
-from test2va.test2va.util.filter_list import filter_list
-from test2va.test2va.util.map_list import map_list
+from test2va.util.filter_list import filter_list
+from test2va.util.map_list import map_list
 
 
 def find_all_test_methods(root: XMLElement) -> List[XMLElement]:
     # First we are going to find all annotation tags.
     res = root.find_descendants(lambda e: e.tag == f"{{{NSURL}}}annotation")
     # Then we are going to filter these out to only find the ones with a name tag with
     # text that contains the word "Test".
```

### Comparing `test2va-1.0.1/test2va/parser/util/find_setup_method.py` & `test2va-1.0.2/test2va/parser/util/find_setup_method.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from test2va.test2va.const.const import NSURL
-from test2va.test2va.parser.structs.XMLElement import XMLElement
+from test2va.const.const import NSURL
+from test2va.parser.structs.XMLElement import XMLElement
 
-from test2va.test2va.util.filter_list import filter_list
-from test2va.test2va.util.map_list import map_list
+from test2va.util.filter_list import filter_list
+from test2va.util.map_list import map_list
 
 
 def find_setup_method(root: XMLElement) -> XMLElement | None:
     # First we are going to find all annotation tags.
     res = root.find_descendants(lambda e: e.tag == f"{{{NSURL}}}annotation")
     # Then we are going to filter these out to only find the ones with a name tag with "Before".
     test_methods = filter_list(res,
```

### Comparing `test2va-1.0.1/test2va/parser/util/literal_format_check.py` & `test2va-1.0.2/test2va/parser/util/literal_format_check.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/parser/util/modify_srcml.py` & `test2va-1.0.2/test2va/parser/util/modify_srcml.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.1/test2va/parser/util/traverse_elements.py` & `test2va-1.0.2/test2va/parser/util/traverse_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import deque
 
-from test2va.test2va.parser.structs.XMLElement import XMLElement
+from test2va.parser.structs.XMLElement import XMLElement
 
 
 def traverse_elements(element):
     root = XMLElement(element.tag, element.attrib)
     root._parent = None
     root._depth = 0
     root._extend_element(element)
```

### Comparing `test2va-1.0.1/test2va.egg-info/SOURCES.txt` & `test2va-1.0.2/test2va.egg-info/SOURCES.txt`

 * *Files identical despite different names*

