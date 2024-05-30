# Comparing `tmp/test2va-1.0.8.tar.gz` & `tmp/test2va-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test2va-1.0.8.tar", last modified: Thu May 30 14:36:05 2024, max compression
+gzip compressed data, was "test2va-1.0.9.tar", last modified: Thu May 30 14:40:45 2024, max compression
```

## Comparing `test2va-1.0.8.tar` & `test2va-1.0.9.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.347462 test2va-1.0.8/
--rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       13 2024-05-30 14:32:50.000000 test2va-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      189 2024-05-30 14:36:05.346456 test2va-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.8/README.md
--rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 14:36:05.347462 test2va-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      563 2024-05-30 14:35:59.000000 test2va-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.190975 test2va-1.0.8/test2va/
--rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.8/test2va/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.205515 test2va-1.0.8/test2va/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.208519 test2va-1.0.8/test2va/const/
--rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.8/test2va/const/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.210514 test2va-1.0.8/test2va/const/__pycache__/
--rw-rw-rw-   0        0        0      275 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/const/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      264 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/const/__pycache__/const.cpython-312.pyc
--rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.8/test2va/const/const.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.175951 test2va-1.0.8/test2va/examples/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.213515 test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/
--rw-rw-rw-   0        0        0     2320 2024-05-29 17:38:34.000000 test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java
--rw-rw-rw-   0        0        0  3860356 2024-03-07 09:41:50.000000 test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.218534 test2va-1.0.8/test2va/generator/
--rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.8/test2va/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.221533 test2va-1.0.8/test2va/generator/__pycache__/
--rw-rw-rw-   0        0        0      198 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1344 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/__pycache__/generator.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.228047 test2va-1.0.8/test2va/generator/core/
--rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.8/test2va/generator/core/GUI.py
--rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/generator/core/GUIMethodReader.py
--rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.8/test2va/generator/core/Method.py
--rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.8/test2va/generator/core/MethodGenerator.py
--rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/generator/core/Mutant.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/generator/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.235073 test2va-1.0.8/test2va/generator/core/__pycache__/
--rw-rw-rw-   0        0        0    13039 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/GUI.cpython-312.pyc
--rw-rw-rw-   0        0        0     4552 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc
--rw-rw-rw-   0        0        0    10964 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/Method.cpython-312.pyc
--rw-rw-rw-   0        0        0     6697 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc
--rw-rw-rw-   0        0        0     9389 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc
--rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.239075 test2va-1.0.8/test2va/generator/exceptions/
--rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.8/test2va/generator/exceptions/GUIException.py
--rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.8/test2va/generator/exceptions/MethodException.py
--rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.8/test2va/generator/exceptions/MethodGeneratorException.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/generator/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.243580 test2va-1.0.8/test2va/generator/exceptions/__pycache__/
--rw-rw-rw-   0        0        0      600 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc
--rw-rw-rw-   0        0        0      609 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc
--rw-rw-rw-   0        0        0      636 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc
--rw-rw-rw-   0        0        0      176 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/generator/generator.py
--rw-rw-rw-   0        0        0    19901 2024-05-30 14:35:52.000000 test2va-1.0.8/test2va/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.245586 test2va-1.0.8/test2va/mutator/
--rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.8/test2va/mutator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.247586 test2va-1.0.8/test2va/mutator/__pycache__/
--rw-rw-rw-   0        0        0      194 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     6037 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/__pycache__/mutator.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.249585 test2va-1.0.8/test2va/mutator/mappings/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/mutator/mappings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.251090 test2va-1.0.8/test2va/mutator/mappings/__pycache__/
--rw-rw-rw-   0        0        0      172 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/mappings/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      910 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc
--rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.8/test2va/mutator/mappings/maps.py
--rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/mutator/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.260439 test2va-1.0.8/test2va/mutator/structs/
--rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/EspressoActions.py
--rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/EspressoCorrelations.py
--rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/EspressoCriteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator1Actions.py
--rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator1Criteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator2Actions.py
--rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator2Criteria.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/mutator/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.270030 test2va-1.0.8/test2va/mutator/structs/__pycache__/
--rw-rw-rw-   0        0        0     2743 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc
--rw-rw-rw-   0        0        0     2036 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc
--rw-rw-rw-   0        0        0    11035 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc
--rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc
--rw-rw-rw-   0        0        0     3580 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc
--rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc
--rw-rw-rw-   0        0        0      365 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator2Criteria.cpython-312.pyc
--rw-rw-rw-   0        0        0      171 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.284050 test2va-1.0.8/test2va/mutator/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/mutator/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.299569 test2va-1.0.8/test2va/mutator/util/__pycache__/
--rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     2661 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc
--rw-rw-rw-   0        0        0      792 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc
--rw-rw-rw-   0        0        0      422 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/clear_user_data.cpython-312.pyc
--rw-rw-rw-   0        0        0      864 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc
--rw-rw-rw-   0        0        0     2008 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc
--rw-rw-rw-   0        0        0     2890 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc
--rw-rw-rw-   0        0        0     1450 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc
--rw-rw-rw-   0        0        0     3207 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc
--rw-rw-rw-   0        0        0      869 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc
--rw-rw-rw-   0        0        0     1898 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc
--rw-rw-rw-   0        0        0     2608 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc
--rw-rw-rw-   0        0        0     2061 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc
--rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/util/base_test.py
--rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.8/test2va/mutator/util/build_xpath_from_element.py
--rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.8/test2va/mutator/util/clear_user_data.py
--rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/execute_action.py
--rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/execute_assertion.py
--rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/find_assertion_correlations.py
--rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/find_element.py
--rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.8/test2va/mutator/util/find_xml_element.py
--rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.8/test2va/mutator/util/get_element_info.py
--rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/get_true_page_source.py
--rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.8/test2va/mutator/util/grant_permissions.py
--rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/populate_mutators.py
--rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/setup_test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.301075 test2va-1.0.8/test2va/output/
--rw-rw-rw-   0        0        0        4 2024-05-30 14:13:40.000000 test2va-1.0.8/test2va/output/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.302081 test2va-1.0.8/test2va/parser/
--rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.8/test2va/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.305591 test2va-1.0.8/test2va/parser/__pycache__/
--rw-rw-rw-   0        0        0      192 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     4093 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/__pycache__/parser.cpython-312.pyc
--rw-rw-rw-   0        0        0     3416 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.310838 test2va-1.0.8/test2va/parser/structs/
--rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/EspressoDeclElement.py
--rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/UiAutomator1ExprElement.py
--rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/UiAutomator2ExprElement.py
--rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/XMLElement.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/parser/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.315934 test2va-1.0.8/test2va/parser/structs/__pycache__/
--rw-rw-rw-   0        0        0    20149 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc
--rw-rw-rw-   0        0        0    19514 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc
--rw-rw-rw-   0        0        0    15481 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc
--rw-rw-rw-   0        0        0     9641 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc
--rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.318444 test2va-1.0.8/test2va/parser/types/
--rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.8/test2va/parser/types/LibTypes.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/parser/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.320444 test2va-1.0.8/test2va/parser/types/__pycache__/
--rw-rw-rw-   0        0        0     2987 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc
--rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/types/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.326868 test2va-1.0.8/test2va/parser/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/parser/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.334370 test2va-1.0.8/test2va/parser/util/__pycache__/
--rw-rw-rw-   0        0        0      167 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1930 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc
--rw-rw-rw-   0        0        0     1917 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc
--rw-rw-rw-   0        0        0     2097 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc
--rw-rw-rw-   0        0        0     1949 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc
--rw-rw-rw-   0        0        0     1202 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc
--rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/util/find_all_test_methods.py
--rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/util/find_setup_method.py
--rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/parser/util/literal_format_check.py
--rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.8/test2va/parser/util/modify_srcml.py
--rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/util/traverse_elements.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.339375 test2va-1.0.8/test2va/util/
--rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.8/test2va/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.345457 test2va-1.0.8/test2va/util/__pycache__/
--rw-rw-rw-   0        0        0      301 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      487 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/camel_to_snake.cpython-312.pyc
--rw-rw-rw-   0        0        0      539 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/filter_list.cpython-312.pyc
--rw-rw-rw-   0        0        0      545 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/map_list.cpython-312.pyc
--rw-rw-rw-   0        0        0      538 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/write_json.cpython-312.pyc
--rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.8/test2va/util/camel_to_snake.py
--rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.8/test2va/util/filter_list.py
--rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.8/test2va/util/map_list.py
--rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/util/write_json.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.204514 test2va-1.0.8/test2va.egg-info/
--rw-rw-rw-   0        0        0      189 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6487 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.208059 test2va-1.0.9/
+-rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-05-30 14:32:50.000000 test2va-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      260 2024-05-30 14:40:45.207053 test2va-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.9/README.md
+-rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:40:45.208059 test2va-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      563 2024-05-30 14:40:39.000000 test2va-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.046400 test2va-1.0.9/test2va/
+-rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.9/test2va/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.068268 test2va-1.0.9/test2va/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.070269 test2va-1.0.9/test2va/const/
+-rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.9/test2va/const/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.073315 test2va-1.0.9/test2va/const/__pycache__/
+-rw-rw-rw-   0        0        0      275 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/const/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      264 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/const/__pycache__/const.cpython-312.pyc
+-rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.9/test2va/const/const.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.031219 test2va-1.0.9/test2va/examples/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.075326 test2va-1.0.9/test2va/examples/NOTES_SetLeftSwipeToDelete/
+-rw-rw-rw-   0        0        0     2320 2024-05-29 17:38:34.000000 test2va-1.0.9/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java
+-rw-rw-rw-   0        0        0  3860356 2024-03-07 09:41:50.000000 test2va-1.0.9/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.081326 test2va-1.0.9/test2va/generator/
+-rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.9/test2va/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.083835 test2va-1.0.9/test2va/generator/__pycache__/
+-rw-rw-rw-   0        0        0      198 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1344 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/__pycache__/generator.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.089840 test2va-1.0.9/test2va/generator/core/
+-rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.9/test2va/generator/core/GUI.py
+-rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/generator/core/GUIMethodReader.py
+-rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.9/test2va/generator/core/Method.py
+-rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.9/test2va/generator/core/MethodGenerator.py
+-rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/generator/core/Mutant.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/generator/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.097570 test2va-1.0.9/test2va/generator/core/__pycache__/
+-rw-rw-rw-   0        0        0    13039 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/core/__pycache__/GUI.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4552 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10964 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/core/__pycache__/Method.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6697 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9389 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc
+-rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/core/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.101086 test2va-1.0.9/test2va/generator/exceptions/
+-rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.9/test2va/generator/exceptions/GUIException.py
+-rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.9/test2va/generator/exceptions/MethodException.py
+-rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.9/test2va/generator/exceptions/MethodGeneratorException.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/generator/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.105596 test2va-1.0.9/test2va/generator/exceptions/__pycache__/
+-rw-rw-rw-   0        0        0      600 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc
+-rw-rw-rw-   0        0        0      609 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc
+-rw-rw-rw-   0        0        0      636 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc
+-rw-rw-rw-   0        0        0      176 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/generator/exceptions/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/generator/generator.py
+-rw-rw-rw-   0        0        0    19901 2024-05-30 14:35:52.000000 test2va-1.0.9/test2va/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.107972 test2va-1.0.9/test2va/mutator/
+-rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.9/test2va/mutator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.109973 test2va-1.0.9/test2va/mutator/__pycache__/
+-rw-rw-rw-   0        0        0      194 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6037 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/__pycache__/mutator.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.111971 test2va-1.0.9/test2va/mutator/mappings/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/mutator/mappings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.114048 test2va-1.0.9/test2va/mutator/mappings/__pycache__/
+-rw-rw-rw-   0        0        0      172 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/mappings/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      910 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc
+-rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.9/test2va/mutator/mappings/maps.py
+-rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/mutator/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.122053 test2va-1.0.9/test2va/mutator/structs/
+-rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/structs/EspressoActions.py
+-rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/structs/EspressoCorrelations.py
+-rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/structs/EspressoCriteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/structs/UiAutomator1Actions.py
+-rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/structs/UiAutomator1Criteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/structs/UiAutomator2Actions.py
+-rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.9/test2va/mutator/structs/UiAutomator2Criteria.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/mutator/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.131573 test2va-1.0.9/test2va/mutator/structs/__pycache__/
+-rw-rw-rw-   0        0        0     2743 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2036 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc
+-rw-rw-rw-   0        0        0    11035 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3580 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc
+-rw-rw-rw-   0        0        0      365 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator2Criteria.cpython-312.pyc
+-rw-rw-rw-   0        0        0      171 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/structs/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.145495 test2va-1.0.9/test2va/mutator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/mutator/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.160469 test2va-1.0.9/test2va/mutator/util/__pycache__/
+-rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2661 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc
+-rw-rw-rw-   0        0        0      792 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc
+-rw-rw-rw-   0        0        0      422 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/clear_user_data.cpython-312.pyc
+-rw-rw-rw-   0        0        0      864 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2008 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2890 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1450 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3207 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc
+-rw-rw-rw-   0        0        0      869 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1898 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2608 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2061 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.9/test2va/mutator/util/base_test.py
+-rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.9/test2va/mutator/util/build_xpath_from_element.py
+-rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.9/test2va/mutator/util/clear_user_data.py
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/execute_action.py
+-rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/execute_assertion.py
+-rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/find_assertion_correlations.py
+-rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/find_element.py
+-rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.9/test2va/mutator/util/find_xml_element.py
+-rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.9/test2va/mutator/util/get_element_info.py
+-rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/get_true_page_source.py
+-rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.9/test2va/mutator/util/grant_permissions.py
+-rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/populate_mutators.py
+-rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/mutator/util/setup_test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.161470 test2va-1.0.9/test2va/output/
+-rw-rw-rw-   0        0        0        4 2024-05-30 14:13:40.000000 test2va-1.0.9/test2va/output/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.163979 test2va-1.0.9/test2va/parser/
+-rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.9/test2va/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.165981 test2va-1.0.9/test2va/parser/__pycache__/
+-rw-rw-rw-   0        0        0      192 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4305 2024-05-30 14:39:52.000000 test2va-1.0.9/test2va/parser/__pycache__/parser.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3498 2024-05-30 14:39:51.000000 test2va-1.0.9/test2va/parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.171979 test2va-1.0.9/test2va/parser/structs/
+-rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/structs/EspressoDeclElement.py
+-rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/structs/UiAutomator1ExprElement.py
+-rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/structs/UiAutomator2ExprElement.py
+-rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/structs/XMLElement.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/parser/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.177992 test2va-1.0.9/test2va/parser/structs/__pycache__/
+-rw-rw-rw-   0        0        0    20149 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0    19514 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0    15481 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9641 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/structs/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.178998 test2va-1.0.9/test2va/parser/types/
+-rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.9/test2va/parser/types/LibTypes.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/parser/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.181998 test2va-1.0.9/test2va/parser/types/__pycache__/
+-rw-rw-rw-   0        0        0     2987 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc
+-rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/types/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.188511 test2va-1.0.9/test2va/parser/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.9/test2va/parser/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.194529 test2va-1.0.9/test2va/parser/util/__pycache__/
+-rw-rw-rw-   0        0        0      167 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/util/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1930 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1917 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2097 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1949 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1202 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/util/find_all_test_methods.py
+-rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/util/find_setup_method.py
+-rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.9/test2va/parser/util/literal_format_check.py
+-rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.9/test2va/parser/util/modify_srcml.py
+-rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/parser/util/traverse_elements.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.200035 test2va-1.0.9/test2va/util/
+-rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.9/test2va/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.205549 test2va-1.0.9/test2va/util/__pycache__/
+-rw-rw-rw-   0        0        0      301 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/util/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      487 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/util/__pycache__/camel_to_snake.cpython-312.pyc
+-rw-rw-rw-   0        0        0      539 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/util/__pycache__/filter_list.cpython-312.pyc
+-rw-rw-rw-   0        0        0      545 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/util/__pycache__/map_list.cpython-312.pyc
+-rw-rw-rw-   0        0        0      538 2024-05-30 14:05:53.000000 test2va-1.0.9/test2va/util/__pycache__/write_json.cpython-312.pyc
+-rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.9/test2va/util/camel_to_snake.py
+-rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.9/test2va/util/filter_list.py
+-rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.9/test2va/util/map_list.py
+-rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.9/test2va/util/write_json.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:40:45.067263 test2va-1.0.9/test2va.egg-info/
+-rw-rw-rw-   0        0        0      260 2024-05-30 14:40:44.000000 test2va-1.0.9/test2va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6487 2024-05-30 14:40:44.000000 test2va-1.0.9/test2va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:40:44.000000 test2va-1.0.9/test2va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 14:40:44.000000 test2va-1.0.9/test2va.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-05-30 14:40:44.000000 test2va-1.0.9/test2va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 14:40:44.000000 test2va-1.0.9/test2va.egg-info/top_level.txt
```

### Comparing `test2va-1.0.8/LICENSE` & `test2va-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/setup.py` & `test2va-1.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test2va',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     install_requires=['appium-python-client==3.1.1', 'pylibsrcml'],
     license='MIT',
     author='Anon',
     include_package_data=True,
     description='Test2VA',
     long_description=open('README.md').read(),
```

### Comparing `test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java` & `test2va-1.0.9/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk` & `test2va-1.0.9/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/__pycache__/generator.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/__pycache__/generator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/GUI.py` & `test2va-1.0.9/test2va/generator/core/GUI.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/GUIMethodReader.py` & `test2va-1.0.9/test2va/generator/core/GUIMethodReader.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/Method.py` & `test2va-1.0.9/test2va/generator/core/Method.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/MethodGenerator.py` & `test2va-1.0.9/test2va/generator/core/MethodGenerator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/Mutant.py` & `test2va-1.0.9/test2va/generator/core/Mutant.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/__pycache__/GUI.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/core/__pycache__/GUI.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/__pycache__/Method.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/core/__pycache__/Method.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc` & `test2va-1.0.9/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/generator/generator.py` & `test2va-1.0.9/test2va/generator/generator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/gui.py` & `test2va-1.0.9/test2va/gui.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/__pycache__/mutator.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/__pycache__/mutator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/mappings/maps.py` & `test2va-1.0.9/test2va/mutator/mappings/maps.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/mutator.py` & `test2va-1.0.9/test2va/mutator/mutator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/EspressoActions.py` & `test2va-1.0.9/test2va/mutator/structs/EspressoActions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/EspressoCorrelations.py` & `test2va-1.0.9/test2va/mutator/structs/EspressoCorrelations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/EspressoCriteria.py` & `test2va-1.0.9/test2va/mutator/structs/EspressoCriteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/UiAutomator1Criteria.py` & `test2va-1.0.9/test2va/mutator/structs/UiAutomator1Criteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc` & `test2va-1.0.9/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/base_test.py` & `test2va-1.0.9/test2va/mutator/util/base_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/execute_assertion.py` & `test2va-1.0.9/test2va/mutator/util/execute_assertion.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/find_assertion_correlations.py` & `test2va-1.0.9/test2va/mutator/util/find_assertion_correlations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/find_element.py` & `test2va-1.0.9/test2va/mutator/util/find_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/find_xml_element.py` & `test2va-1.0.9/test2va/mutator/util/find_xml_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/get_true_page_source.py` & `test2va-1.0.9/test2va/mutator/util/get_true_page_source.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/grant_permissions.py` & `test2va-1.0.9/test2va/mutator/util/grant_permissions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/populate_mutators.py` & `test2va-1.0.9/test2va/mutator/util/populate_mutators.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/mutator/util/setup_test.py` & `test2va-1.0.9/test2va/mutator/util/setup_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/__pycache__/parser.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/__pycache__/parser.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu May 30 13:57:45 2024 UTC, .py size: 3416 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 d985 5866 580d 0000  ..........XfX...
+00000000: cb0d 0d0a 0000 0000 b78f 5866 aa0d 0000  ..........Xf....
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0000 0000 00f3 b000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 6302 0100 6d04 5a05 0100 6400  l.m.c...m.Z...d.
 00000050: 6402 6c06 6d07 5a07 0100 6400 6403 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
@@ -22,15 +22,15 @@
 00000150: 6129 01da 1566 696e 645f 616c 6c5f 7465  a)...find_all_te
 00000160: 7374 5f6d 6574 686f 6473 2901 da11 6669  st_methods)...fi
 00000170: 6e64 5f73 6574 7570 5f6d 6574 686f 6429  nd_setup_method)
 00000180: 01da 0c6d 6f64 6966 795f 7372 636d 6c29  ...modify_srcml)
 00000190: 01da 1174 7261 7665 7273 655f 656c 656d  ...traverse_elem
 000001a0: 656e 7473 2901 da0a 7772 6974 655f 6a73  ents)...write_js
 000001b0: 6f6e 6302 0000 0000 0000 0000 0000 0007  onc.............
-000001c0: 0000 0003 0000 00f3 2605 0000 9700 0900  ........&.......
+000001c0: 0000 0003 0000 00f3 a805 0000 9700 0900  ................
 000001d0: 7401 0000 0000 0000 0000 7c01 6a02 0000  t.........|.j...
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 6a05 0000 0000 0000 0000 0000 0000 0000  j...............
 00000200: 0000 0000 ab00 0000 0000 0000 ab01 0000  ................
 00000210: 0000 0000 0100 6403 6404 6c05 6d06 7d03  ......d.d.l.m.}.
 00000220: 0100 7c00 9b00 6405 9d02 7d04 0900 7c03  ..|...d...}...|.
 00000230: 6a0d 0000 0000 0000 0000 0000 0000 0000  j...............
@@ -80,177 +80,191 @@
 000004f0: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
 00000500: 0000 0000 ab01 0000 0000 0000 0100 8c26  ...............&
 00000510: 0400 7c0d 6a2f 0000 0000 0000 0000 0000  ..|.j/..........
 00000520: 0000 0000 0000 0000 7c0a ab01 0000 0000  ........|.......
 00000530: 0000 7c0e 640f 3c00 0000 7c09 6a2b 0000  ..|.d.<...|.j+..
 00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000550: 7c0e ab01 0000 0000 0000 0100 9001 8c27  |..............'
-00000560: 0400 0900 7431 0000 0000 0000 0000 7c09  ....t1........|.
-00000570: 6410 7c00 9b00 6411 9d03 ab02 0000 0000  d.|...d.........
-00000580: 0000 0100 7433 0000 0000 0000 0000 6a34  ....t3........j4
-00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 7c04 ab01 0000 0000 0000 0100 7c09  ..|...........|.
-000005b0: 5300 2300 7406 0000 0000 0000 0000 2400  S.#.t.........$.
-000005c0: 722f 7d02 7c01 6a09 0000 0000 0000 0000  r/}.|.j.........
-000005d0: 0000 0000 0000 0000 0000 6401 7c02 9b00  ..........d.|...
-000005e0: 9d02 ab01 0000 0000 0000 0100 7c01 6a09  ............|.j.
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 0000 6402 ab01 0000 0000 0000 0100 5900  ..d...........Y.
-00000610: 6400 7d02 7e02 7900 6400 7d02 7e02 7701  d.}.~.y.d.}.~.w.
-00000620: 7700 7803 5900 7701 2300 7406 0000 0000  w.x.Y.w.#.t.....
-00000630: 0000 0000 2400 722f 7d02 7c01 6a09 0000  ....$.r/}.|.j...
-00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000650: 6406 7c02 9b00 9d02 ab01 0000 0000 0000  d.|.............
-00000660: 0100 7c01 6a09 0000 0000 0000 0000 0000  ..|.j...........
-00000670: 0000 0000 0000 0000 6407 ab01 0000 0000  ........d.......
-00000680: 0000 0100 5900 6400 7d02 7e02 7900 6400  ....Y.d.}.~.y.d.
-00000690: 7d02 7e02 7701 7700 7803 5900 7701 2300  }.~.w.w.x.Y.w.#.
-000006a0: 7406 0000 0000 0000 0000 2400 721e 7d02  t.........$.r.}.
-000006b0: 7c01 6a09 0000 0000 0000 0000 0000 0000  |.j.............
-000006c0: 0000 0000 0000 6412 7c02 9b00 9d02 ab01  ......d.|.......
-000006d0: 0000 0000 0000 0100 5900 6400 7d02 7e02  ........Y.d.}.~.
-000006e0: 7900 6400 7d02 7e02 7701 7700 7803 5900  y.d.}.~.w.w.x.Y.
-000006f0: 7701 2913 4e75 1600 0000 e29b 9420 5352  w.).Nu....... SR
-00000700: 434d 4c20 5061 7468 2045 7272 6f72 3a20  CML Path Error: 
-00000710: 7521 0000 00e2 9aa0 efb8 8f20 5665 7269  u!......... Veri
-00000720: 6679 2073 7263 6d6c 2064 6c6c 2066 696c  fy srcml dll fil
-00000730: 6520 7061 7468 7202 0000 0029 01da 0573  e pathr....)...s
-00000740: 7263 6d6c 7a04 2e78 6d6c 7511 0000 00e2  rcmlz..xmlu.....
-00000750: 9b94 2053 5243 4d4c 2045 7272 6f72 3a20  .. SRCML Error: 
-00000760: 751d 0000 00e2 9aa0 efb8 8f20 5665 7269  u.......... Veri
-00000770: 6679 2069 6e70 7574 206a 6176 6120 6669  fy input java fi
-00000780: 6c65 6301 0000 0000 0000 0000 0000 0004  lec.............
-00000790: 0000 0013 0000 00f3 3000 0000 9700 7c00  ........0.....|.
-000007a0: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
-000007b0: 0000 0000 6401 7402 0000 0000 0000 0000  ....d.t.........
-000007c0: 9b00 6402 9d03 6b28 0000 5300 2903 4efa  ..d...k(..S.).N.
-000007d0: 017b 7a05 7d6e 616d 6529 02da 0374 6167  .{z.}name)...tag
-000007e0: 7204 0000 0029 01da 0165 7301 0000 0020  r....)...es.... 
-000007f0: fa3f 433a 5c55 7365 7273 5c73 6865 6572  .?C:\Users\sheer
-00000800: 5c50 7963 6861 726d 5072 6f6a 6563 7473  \PycharmProjects
-00000810: 5c74 6573 7432 7661 5c74 6573 7432 7661  \test2va\test2va
-00000820: 5c70 6172 7365 725c 7061 7273 6572 2e70  \parser\parser.p
-00000830: 79fa 083c 6c61 6d62 6461 3e7a 1870 6172  y..<lambda>z.par
-00000840: 7365 722e 3c6c 6f63 616c 733e 2e3c 6c61  ser.<locals>.<la
-00000850: 6d62 6461 3e35 0000 0073 1800 0000 8000  mbda>5...s......
-00000860: b011 b715 b115 b842 bc75 b867 c056 d03a  .......B.u.g.V.:
-00000870: 4cd1 314c 8000 f300 0000 00da 0c55 6941  L.1L.........UiA
-00000880: 7574 6f6d 6174 6f72 31da 0c55 6941 7574  utomator1..UiAut
-00000890: 6f6d 6174 6f72 32da 0845 7370 7265 7373  omator2..Espress
-000008a0: 6f29 05da 046e 616d 65da 0973 656c 6563  o)...name..selec
-000008b0: 746f 7273 da06 6265 666f 7265 da09 6173  tors..before..as
-000008c0: 7365 7274 696f 6eda 076c 6962 7261 7279  sertion..library
-000008d0: 721c 0000 0072 1b00 0000 721d 0000 007a  r....r....r....z
-000008e0: 076f 7574 7075 742f 7a0c 5f70 6172 7365  .output/z._parse
-000008f0: 642e 6a73 6f6e 7516 0000 00e2 9b94 204a  d.jsonu....... J
-00000900: 534f 4e20 5772 6974 6520 4572 726f 723a  SON Write Error:
-00000910: 2029 1b72 0b00 0000 da10 7372 636d 6c5f   ).r......srcml_
-00000920: 696e 7075 745f 7465 7874 da03 6765 74da  input_text..get.
-00000930: 0945 7863 6570 7469 6f6e da03 6f75 74da  .Exception..out.
-00000940: 0a70 796c 6962 7372 636d 6c72 0f00 0000  .pylibsrcmlr....
-00000950: da0f 6a61 7661 5f69 6e70 7574 5f74 6578  ..java_input_tex
-00000960: 74da 0245 54da 0570 6172 7365 720c 0000  t..ET..parser...
-00000970: 00da 0767 6574 726f 6f74 7209 0000 0072  ...getrootr....r
-00000980: 0a00 0000 da10 6669 6e64 5f66 6972 7374  ......find_first
-00000990: 5f63 6869 6c64 da04 7465 7874 da03 6c65  _child..text..le
-000009a0: 6e72 0500 0000 da18 6669 6e64 5f73 656c  nr......find_sel
-000009b0: 6563 746f 725f 7374 7275 6374 7572 6573  ector_structures
-000009c0: 7206 0000 0072 0700 0000 da06 6170 7065  r....r......appe
-000009d0: 6e64 da08 6765 745f 6461 7461 da0f 7061  nd..get_data..pa
-000009e0: 7273 655f 6173 7365 7274 696f 6e72 0d00  rse_assertionr..
-000009f0: 0000 da02 6f73 da06 7265 6d6f 7665 2912  ....os..remove).
-00000a00: da09 6669 6c65 5f6e 616d 65da 0367 7569  ..file_name..gui
-00000a10: 7213 0000 0072 0f00 0000 da03 786d 6cda  r....r......xml.
-00000a20: 0474 7265 65da 0472 6f6f 74da 0c74 6573  .tree..root..tes
-00000a30: 745f 6d65 7468 6f64 73da 0c73 6574 7570  t_methods..setup
-00000a40: 5f6d 6574 686f 64da 0464 6174 61da 066d  _method..data..m
-00000a50: 6574 686f 6472 1a00 0000 da03 6c69 62da  ethodr......lib.
-00000a60: 0563 6c61 7a7a da0b 6d65 7468 6f64 5f64  .clazz..method_d
-00000a70: 6174 6172 1b00 0000 da0f 7365 7475 705f  atar......setup_
-00000a80: 7365 6c65 6374 6f72 73da 0873 656c 6563  selectors..selec
-00000a90: 746f 7273 1200 0000 2020 2020 2020 2020  tors....        
-00000aa0: 2020 2020 2020 2020 2020 7214 0000 00da            r.....
-00000ab0: 0670 6172 7365 7272 3f00 0000 1200 0000  .parserr?.......
-00000ac0: 7395 0200 0080 00f0 0605 050f dc08 1490  s...............
-00000ad0: 53d7 1529 d115 29d7 152d d115 2dd3 152f  S..)..)..-..-../
-00000ae0: d408 30f5 0c00 0521 e00d 1688 4b90 74d0  ..0....!....K.t.
-00000af0: 0a1c 8043 f004 0505 0fd8 080d 8f0b 890b  ...C............
-00000b00: 9043 d714 27d1 1427 d714 2bd1 142b d314  .C..'..'..+..+..
-00000b10: 2da8 73d4 0833 f40c 000c 0e8f 3889 3890  -.s..3......8.8.
-00000b20: 438b 3d80 44dc 0b1c 9854 9f5c 995c 9b5e  C.=.D....T.\.\.^
-00000b30: d30b 2c80 44f4 0600 1429 a814 d313 2e80  ..,.D....)......
-00000b40: 4cf4 0600 1425 a054 d313 2a80 4cf0 0600  L....%.T..*.L...
-00000b50: 0c0e 8044 f006 0013 1ff3 0026 0521 8806  ...D.......&.!..
-00000b60: d80f 15d7 0f26 d10f 26d1 274c d30f 4dd7  .....&..&.'L..M.
-00000b70: 0f52 d10f 5288 04e4 0b0e d40f 26d7 0f3f  .R..R.......&..?
-00000b80: d10f 3fc0 06d3 0f47 d30b 48c8 31d2 0b4c  ..?....G..H.1..L
-00000b90: d82b 3988 43dc 142b 8945 dc0d 10d4 1128  .+9.C..+.E.....(
-00000ba0: d711 41d1 1141 c026 d311 49d3 0d4a c851  ..A..A.&..I..J.Q
-00000bb0: d20d 4ed8 2b39 8843 dc14 2b89 45e0 2731  ..N.+9.C..+.E.'1
-00000bc0: 8843 dc14 2788 45f0 0600 1519 d819 1bd8  .C..'.E.........
-00000bd0: 1618 d819 1bd8 171a f10b 0623 0a88 0bf0  ...........#....
-00000be0: 1200 151a d714 32d1 1432 b036 d314 3a88  ......2..2.6..:.
-00000bf0: 09f0 0600 0c18 d00b 23d8 1e23 d71e 3cd1  ........#..#..<.
-00000c00: 1e3c b85c d31e 4a88 4fd8 1c2b f200 010d  .<.\..J.O..+....
-00000c10: 4201 9008 d810 1b98 48d1 1025 d710 2cd1  B.......H..%..,.
-00000c20: 102c a858 d72d 3ed1 2d3e d32d 40d5 1041  .,.X.->.->.-@..A
-00000c30: f103 010d 4201 f006 0025 2988 4b98 08d1  ....B....%).K...
-00000c40: 0c21 f006 0019 22f2 0001 0941 0188 48d8  .!...."....A..H.
-00000c50: 0c17 980b d10c 24d7 0c2b d10c 2ba8 48d7  ......$..+..+.H.
-00000c60: 2c3d d12c 3dd3 2c3f d50c 40f0 0301 0941  ,=.,=.,?..@....A
-00000c70: 01f0 0600 2429 d723 38d1 2338 b816 d323  ....$).#8.#8...#
-00000c80: 4088 0b90 4bd1 0820 e008 0c8f 0b89 0b90  @...K.. ........
-00000c90: 4bd6 0820 f04d 0126 0521 f050 0104 050f  K.. .M.&.!.P....
-00000ca0: dc08 1290 3498 37a0 39a0 2ba8 5cd0 193a  ....4.7.9.+.\..:
-00000cb0: d408 3bf4 0a00 0507 8749 8149 8863 844e  ..;......I.I.c.N
-00000cc0: e00b 0f80 4bf8 f45b 0200 0c15 f200 0305  ....K..[........
-00000cd0: 0fd8 080b 8f07 8907 d012 28a8 11a8 03d0  ..........(.....
-00000ce0: 102c d408 2dd8 080b 8f07 8907 d010 33d4  .,..-.........3.
-00000cf0: 0834 dc08 0efb f007 0305 0ffb f416 000c  .4..............
-00000d00: 15f2 0003 050f d808 0b8f 0789 07d0 1223  ...............#
-00000d10: a041 a033 d010 27d4 0828 d808 0b8f 0789  .A.3..'..(......
-00000d20: 07d0 102f d408 30dc 080e fbf0 0703 050f  .../..0.........
-00000d30: fbf4 7801 000c 15f2 0002 050f d808 0b8f  ..x.............
-00000d40: 0789 07d0 1228 a811 a803 d010 2cd4 082d  .....(......,..-
-00000d50: dc08 0efb f005 0205 0ffa 7346 0000 0082  ..........sF....
-00000d60: 2347 3300 b12a 482e 00c7 0c10 4929 00c7  #G3..*H.....I)..
-00000d70: 3309 482b 03c7 3c25 4826 03c8 2605 482b  3.H+..<%H&..&.H+
-00000d80: 03c8 2e09 4926 03c8 3725 4921 03c9 2105  ....I&..7%I!..!.
-00000d90: 4926 03c9 2909 4a10 03c9 3214 4a0b 03ca  I&..).J...2.J...
-00000da0: 0b05 4a10 0329 1dda 0673 6875 7469 6c72  ..J..)...shutilr
-00000db0: 2f00 0000 da15 786d 6c2e 6574 7265 652e  /.....xml.etree.
-00000dc0: 456c 656d 656e 7454 7265 65da 0565 7472  ElementTree..etr
-00000dd0: 6565 da0b 456c 656d 656e 7454 7265 6572  ee..ElementTreer
-00000de0: 2500 0000 da06 7479 7069 6e67 7203 0000  %.....typingr...
-00000df0: 00da 1374 6573 7432 7661 2e63 6f6e 7374  ...test2va.const
-00000e00: 2e63 6f6e 7374 7204 0000 00da 2e74 6573  .constr......tes
-00000e10: 7432 7661 2e70 6172 7365 722e 7374 7275  t2va.parser.stru
-00000e20: 6374 732e 5569 4175 746f 6d61 746f 7231  cts.UiAutomator1
-00000e30: 4578 7072 456c 656d 656e 7472 0500 0000  ExprElementr....
-00000e40: da2e 7465 7374 3276 612e 7061 7273 6572  ..test2va.parser
-00000e50: 2e73 7472 7563 7473 2e55 6941 7574 6f6d  .structs.UiAutom
-00000e60: 6174 6f72 3245 7870 7245 6c65 6d65 6e74  ator2ExprElement
-00000e70: 7206 0000 00da 2a74 6573 7432 7661 2e70  r.....*test2va.p
-00000e80: 6172 7365 722e 7374 7275 6374 732e 4573  arser.structs.Es
-00000e90: 7072 6573 736f 4465 636c 456c 656d 656e  pressoDeclElemen
-00000ea0: 7472 0700 0000 da1d 7465 7374 3276 612e  tr......test2va.
-00000eb0: 7061 7273 6572 2e74 7970 6573 2e4c 6962  parser.types.Lib
-00000ec0: 5479 7065 7372 0800 0000 da29 7465 7374  Typesr.....)test
-00000ed0: 3276 612e 7061 7273 6572 2e75 7469 6c2e  2va.parser.util.
-00000ee0: 6669 6e64 5f61 6c6c 5f74 6573 745f 6d65  find_all_test_me
-00000ef0: 7468 6f64 7372 0900 0000 da25 7465 7374  thodsr.....%test
-00000f00: 3276 612e 7061 7273 6572 2e75 7469 6c2e  2va.parser.util.
-00000f10: 6669 6e64 5f73 6574 7570 5f6d 6574 686f  find_setup_metho
-00000f20: 6472 0a00 0000 da20 7465 7374 3276 612e  dr..... test2va.
-00000f30: 7061 7273 6572 2e75 7469 6c2e 6d6f 6469  parser.util.modi
-00000f40: 6679 5f73 7263 6d6c 720b 0000 00da 2574  fy_srcmlr.....%t
-00000f50: 6573 7432 7661 2e70 6172 7365 722e 7574  est2va.parser.ut
-00000f60: 696c 2e74 7261 7665 7273 655f 656c 656d  il.traverse_elem
-00000f70: 656e 7473 720c 0000 00da 1774 6573 7432  entsr......test2
-00000f80: 7661 2e75 7469 6c2e 7772 6974 655f 6a73  va.util.write_js
-00000f90: 6f6e 720d 0000 0072 3f00 0000 a900 7216  onr....r?.....r.
-00000fa0: 0000 0072 1400 0000 fa08 3c6d 6f64 756c  ...r......<modul
-00000fb0: 653e 7250 0000 0001 0000 0073 3800 0000  e>rP.......s8...
-00000fc0: f003 0101 01db 000d db00 09df 0022 d000  ............."..
-00000fd0: 22dd 001a e500 25dd 0052 dd00 52dd 004a  ".....%..R..R..J
-00000fe0: dd00 34dd 004b dd00 43dd 0039 dd00 43dd  ..4..K..C..9..C.
-00000ff0: 002e f306 5201 0110 7216 0000 00         ....R...r....
+00000560: 0400 0900 7430 0000 0000 0000 0000 6a32  ....t0........j2
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0000 6a35 0000 0000 0000 0000 0000 0000  ..j5............
+00000590: 0000 0000 0000 7430 0000 0000 0000 0000  ......t0........
+000005a0: 6a32 0000 0000 0000 0000 0000 0000 0000  j2..............
+000005b0: 0000 0000 6a37 0000 0000 0000 0000 0000  ....j7..........
+000005c0: 0000 0000 0000 0000 7438 0000 0000 0000  ........t8......
+000005d0: 0000 ab01 0000 0000 0000 6410 7c00 9b00  ..........d.|...
+000005e0: 6411 9d02 ab03 0000 0000 0000 7d12 743b  d...........}.t;
+000005f0: 0000 0000 0000 0000 7c09 7c12 ab02 0000  ........|.|.....
+00000600: 0000 0000 0100 7431 0000 0000 0000 0000  ......t1........
+00000610: 6a3c 0000 0000 0000 0000 0000 0000 0000  j<..............
+00000620: 0000 0000 7c04 ab01 0000 0000 0000 0100  ....|...........
+00000630: 7c09 5300 2300 7406 0000 0000 0000 0000  |.S.#.t.........
+00000640: 2400 722f 7d02 7c01 6a09 0000 0000 0000  $.r/}.|.j.......
+00000650: 0000 0000 0000 0000 0000 0000 6401 7c02  ............d.|.
+00000660: 9b00 9d02 ab01 0000 0000 0000 0100 7c01  ..............|.
+00000670: 6a09 0000 0000 0000 0000 0000 0000 0000  j...............
+00000680: 0000 0000 6402 ab01 0000 0000 0000 0100  ....d...........
+00000690: 5900 6400 7d02 7e02 7900 6400 7d02 7e02  Y.d.}.~.y.d.}.~.
+000006a0: 7701 7700 7803 5900 7701 2300 7406 0000  w.w.x.Y.w.#.t...
+000006b0: 0000 0000 0000 2400 722f 7d02 7c01 6a09  ......$.r/}.|.j.
+000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006d0: 0000 6406 7c02 9b00 9d02 ab01 0000 0000  ..d.|...........
+000006e0: 0000 0100 7c01 6a09 0000 0000 0000 0000  ....|.j.........
+000006f0: 0000 0000 0000 0000 0000 6407 ab01 0000  ..........d.....
+00000700: 0000 0000 0100 5900 6400 7d02 7e02 7900  ......Y.d.}.~.y.
+00000710: 6400 7d02 7e02 7701 7700 7803 5900 7701  d.}.~.w.w.x.Y.w.
+00000720: 2300 7406 0000 0000 0000 0000 2400 721e  #.t.........$.r.
+00000730: 7d02 7c01 6a09 0000 0000 0000 0000 0000  }.|.j...........
+00000740: 0000 0000 0000 0000 6412 7c02 9b00 9d02  ........d.|.....
+00000750: ab01 0000 0000 0000 0100 5900 6400 7d02  ..........Y.d.}.
+00000760: 7e02 7900 6400 7d02 7e02 7701 7700 7803  ~.y.d.}.~.w.w.x.
+00000770: 5900 7701 2913 4e75 1600 0000 e29b 9420  Y.w.).Nu....... 
+00000780: 5352 434d 4c20 5061 7468 2045 7272 6f72  SRCML Path Error
+00000790: 3a20 7521 0000 00e2 9aa0 efb8 8f20 5665  : u!......... Ve
+000007a0: 7269 6679 2073 7263 6d6c 2064 6c6c 2066  rify srcml dll f
+000007b0: 696c 6520 7061 7468 7202 0000 0029 01da  ile pathr....)..
+000007c0: 0573 7263 6d6c 7a04 2e78 6d6c 7511 0000  .srcmlz..xmlu...
+000007d0: 00e2 9b94 2053 5243 4d4c 2045 7272 6f72  .... SRCML Error
+000007e0: 3a20 751d 0000 00e2 9aa0 efb8 8f20 5665  : u.......... Ve
+000007f0: 7269 6679 2069 6e70 7574 206a 6176 6120  rify input java 
+00000800: 6669 6c65 6301 0000 0000 0000 0000 0000  filec...........
+00000810: 0004 0000 0013 0000 00f3 3000 0000 9700  ..........0.....
+00000820: 7c00 6a00 0000 0000 0000 0000 0000 0000  |.j.............
+00000830: 0000 0000 0000 6401 7402 0000 0000 0000  ......d.t.......
+00000840: 0000 9b00 6402 9d03 6b28 0000 5300 2903  ....d...k(..S.).
+00000850: 4efa 017b 7a05 7d6e 616d 6529 02da 0374  N..{z.}name)...t
+00000860: 6167 7204 0000 0029 01da 0165 7301 0000  agr....)...es...
+00000870: 0020 fa3f 433a 5c55 7365 7273 5c73 6865  . .?C:\Users\she
+00000880: 6572 5c50 7963 6861 726d 5072 6f6a 6563  er\PycharmProjec
+00000890: 7473 5c74 6573 7432 7661 5c74 6573 7432  ts\test2va\test2
+000008a0: 7661 5c70 6172 7365 725c 7061 7273 6572  va\parser\parser
+000008b0: 2e70 79fa 083c 6c61 6d62 6461 3e7a 1870  .py..<lambda>z.p
+000008c0: 6172 7365 722e 3c6c 6f63 616c 733e 2e3c  arser.<locals>.<
+000008d0: 6c61 6d62 6461 3e35 0000 0073 1800 0000  lambda>5...s....
+000008e0: 8000 b011 b715 b115 b842 bc75 b867 c056  .........B.u.g.V
+000008f0: d03a 4cd1 314c 8000 f300 0000 00da 0c55  .:L.1L.........U
+00000900: 6941 7574 6f6d 6174 6f72 31da 0c55 6941  iAutomator1..UiA
+00000910: 7574 6f6d 6174 6f72 32da 0845 7370 7265  utomator2..Espre
+00000920: 7373 6f29 05da 046e 616d 65da 0973 656c  sso)...name..sel
+00000930: 6563 746f 7273 da06 6265 666f 7265 da09  ectors..before..
+00000940: 6173 7365 7274 696f 6eda 076c 6962 7261  assertion..libra
+00000950: 7279 721c 0000 0072 1b00 0000 721d 0000  ryr....r....r...
+00000960: 007a 092e 2e2f 6f75 7470 7574 7a0c 5f70  .z.../outputz._p
+00000970: 6172 7365 642e 6a73 6f6e 7516 0000 00e2  arsed.jsonu.....
+00000980: 9b94 204a 534f 4e20 5772 6974 6520 4572  .. JSON Write Er
+00000990: 726f 723a 2029 1f72 0b00 0000 da10 7372  ror: ).r......sr
+000009a0: 636d 6c5f 696e 7075 745f 7465 7874 da03  cml_input_text..
+000009b0: 6765 74da 0945 7863 6570 7469 6f6e da03  get..Exception..
+000009c0: 6f75 74da 0a70 796c 6962 7372 636d 6c72  out..pylibsrcmlr
+000009d0: 0f00 0000 da0f 6a61 7661 5f69 6e70 7574  ......java_input
+000009e0: 5f74 6578 74da 0245 54da 0570 6172 7365  _text..ET..parse
+000009f0: 720c 0000 00da 0767 6574 726f 6f74 7209  r......getrootr.
+00000a00: 0000 0072 0a00 0000 da10 6669 6e64 5f66  ...r......find_f
+00000a10: 6972 7374 5f63 6869 6c64 da04 7465 7874  irst_child..text
+00000a20: da03 6c65 6e72 0500 0000 da18 6669 6e64  ..lenr......find
+00000a30: 5f73 656c 6563 746f 725f 7374 7275 6374  _selector_struct
+00000a40: 7572 6573 7206 0000 0072 0700 0000 da06  uresr....r......
+00000a50: 6170 7065 6e64 da08 6765 745f 6461 7461  append..get_data
+00000a60: da0f 7061 7273 655f 6173 7365 7274 696f  ..parse_assertio
+00000a70: 6eda 026f 73da 0470 6174 68da 046a 6f69  n..os..path..joi
+00000a80: 6eda 0764 6972 6e61 6d65 da08 5f5f 6669  n..dirname..__fi
+00000a90: 6c65 5f5f 720d 0000 00da 0672 656d 6f76  le__r......remov
+00000aa0: 6529 13da 0966 696c 655f 6e61 6d65 da03  e)...file_name..
+00000ab0: 6775 6972 1300 0000 720f 0000 00da 0378  guir....r......x
+00000ac0: 6d6c da04 7472 6565 da04 726f 6f74 da0c  ml..tree..root..
+00000ad0: 7465 7374 5f6d 6574 686f 6473 da0c 7365  test_methods..se
+00000ae0: 7475 705f 6d65 7468 6f64 da04 6461 7461  tup_method..data
+00000af0: da06 6d65 7468 6f64 721a 0000 00da 036c  ..methodr......l
+00000b00: 6962 da05 636c 617a 7ada 0b6d 6574 686f  ib..clazz..metho
+00000b10: 645f 6461 7461 721b 0000 00da 0f73 6574  d_datar......set
+00000b20: 7570 5f73 656c 6563 746f 7273 da08 7365  up_selectors..se
+00000b30: 6c65 6374 6f72 da0b 6f75 7470 7574 5f70  lector..output_p
+00000b40: 6174 6873 1300 0000 2020 2020 2020 2020  aths....        
+00000b50: 2020 2020 2020 2020 2020 2072 1400 0000             r....
+00000b60: da06 7061 7273 6572 7244 0000 0012 0000  ..parserrD......
+00000b70: 0073 b702 0000 8000 f006 0505 0fdc 0814  .s..............
+00000b80: 9053 d715 29d1 1529 d715 2dd1 152d d315  .S..)..)..-..-..
+00000b90: 2fd4 0830 f50c 0005 21e0 0d16 884b 9074  /..0....!....K.t
+00000ba0: d00a 1c80 43f0 0405 050f d808 0d8f 0b89  ....C...........
+00000bb0: 0b90 43d7 1427 d114 27d7 142b d114 2bd3  ..C..'..'..+..+.
+00000bc0: 142d a873 d408 33f4 0c00 0c0e 8f38 8938  .-.s..3......8.8
+00000bd0: 9043 8b3d 8044 dc0b 1c98 549f 5c99 5c9b  .C.=.D....T.\.\.
+00000be0: 5ed3 0b2c 8044 f406 0014 29a8 14d3 132e  ^..,.D....).....
+00000bf0: 804c f406 0014 25a0 54d3 132a 804c f006  .L....%.T..*.L..
+00000c00: 000c 0e80 44f0 0600 131f f300 2605 2188  ....D.......&.!.
+00000c10: 06d8 0f15 d70f 26d1 0f26 d127 4cd3 0f4d  ......&..&.'L..M
+00000c20: d70f 52d1 0f52 8804 e40b 0ed4 0f26 d70f  ..R..R.......&..
+00000c30: 3fd1 0f3f c006 d30f 47d3 0b48 c831 d20b  ?..?....G..H.1..
+00000c40: 4cd8 2b39 8843 dc14 2b89 45dc 0d10 d411  L.+9.C..+.E.....
+00000c50: 28d7 1141 d111 41c0 26d3 1149 d30d 4ac8  (..A..A.&..I..J.
+00000c60: 51d2 0d4e d82b 3988 43dc 142b 8945 e027  Q..N.+9.C..+.E.'
+00000c70: 3188 43dc 1427 8845 f006 0015 19d8 191b  1.C..'.E........
+00000c80: d816 18d8 191b d817 1af1 0b06 230a 880b  ............#...
+00000c90: f012 0015 1ad7 1432 d114 32b0 36d3 143a  .......2..2.6..:
+00000ca0: 8809 f006 000c 18d0 0b23 d81e 23d7 1e3c  .........#..#..<
+00000cb0: d11e 3cb8 5cd3 1e4a 884f d81c 2bf2 0001  ..<.\..J.O..+...
+00000cc0: 0d42 0190 08d8 101b 9848 d110 25d7 102c  .B.......H..%..,
+00000cd0: d110 2ca8 58d7 2d3e d12d 3ed3 2d40 d510  ..,.X.->.->.-@..
+00000ce0: 41f1 0301 0d42 01f0 0600 2529 884b 9808  A....B....%).K..
+00000cf0: d10c 21f0 0600 1922 f200 0109 4101 8848  ..!...."....A..H
+00000d00: d80c 1798 0bd1 0c24 d70c 2bd1 0c2b a848  .......$..+..+.H
+00000d10: d72c 3dd1 2c3d d32c 3fd5 0c40 f003 0109  .,=.,=.,?..@....
+00000d20: 4101 f006 0024 29d7 2338 d123 38b8 16d3  A....$).#8.#8...
+00000d30: 2340 880b 904b d108 20e0 080c 8f0b 890b  #@...K.. .......
+00000d40: 904b d608 20f0 4d01 2605 21f0 5001 0505  .K.. .M.&.!.P...
+00000d50: 0fdc 1618 9767 9167 976c 916c a432 a737  .....g.g.l.l.2.7
+00000d60: a137 a73f a13f b438 d323 3cb8 6bc8 69c8  .7.?.?.8.#<.k.i.
+00000d70: 5bd0 5864 d04b 65d3 1666 880b dc08 1290  [.Xd.Ke..f......
+00000d80: 3498 1bd4 0825 f40a 0005 0787 4981 4988  4....%......I.I.
+00000d90: 6384 4ee0 0b0f 804b f8f4 5d02 000c 15f2  c.N....K..].....
+00000da0: 0003 050f d808 0b8f 0789 07d0 1228 a811  .............(..
+00000db0: a803 d010 2cd4 082d d808 0b8f 0789 07d0  ....,..-........
+00000dc0: 1033 d408 34dc 080e fbf0 0703 050f fbf4  .3..4...........
+00000dd0: 1600 0c15 f200 0305 0fd8 080b 8f07 8907  ................
+00000de0: d012 23a0 41a0 33d0 1027 d408 28d8 080b  ..#.A.3..'..(...
+00000df0: 8f07 8907 d010 2fd4 0830 dc08 0efb f007  ....../..0......
+00000e00: 0305 0ffb f47a 0100 0c15 f200 0205 0fd8  .....z..........
+00000e10: 080b 8f07 8907 d012 28a8 11a8 03d0 102c  ........(......,
+00000e20: d408 2ddc 080e fbf0 0502 050f fa73 4700  ..-..........sG.
+00000e30: 0000 8223 4834 00b1 2a49 2f00 c70c 4111  ...#H4..*I/...A.
+00000e40: 4a2a 00c8 3409 492c 03c8 3d25 4927 03c9  J*..4.I,..=%I'..
+00000e50: 2705 492c 03c9 2f09 4a27 03c9 3825 4a22  '.I,../.J'..8%J"
+00000e60: 03ca 2205 4a27 03ca 2a09 4b11 03ca 3314  ..".J'..*.K...3.
+00000e70: 4b0c 03cb 0c05 4b11 0329 1dda 0673 6875  K.....K..)...shu
+00000e80: 7469 6c72 2f00 0000 da15 786d 6c2e 6574  tilr/.....xml.et
+00000e90: 7265 652e 456c 656d 656e 7454 7265 65da  ree.ElementTree.
+00000ea0: 0565 7472 6565 da0b 456c 656d 656e 7454  .etree..ElementT
+00000eb0: 7265 6572 2500 0000 da06 7479 7069 6e67  reer%.....typing
+00000ec0: 7203 0000 00da 1374 6573 7432 7661 2e63  r......test2va.c
+00000ed0: 6f6e 7374 2e63 6f6e 7374 7204 0000 00da  onst.constr.....
+00000ee0: 2e74 6573 7432 7661 2e70 6172 7365 722e  .test2va.parser.
+00000ef0: 7374 7275 6374 732e 5569 4175 746f 6d61  structs.UiAutoma
+00000f00: 746f 7231 4578 7072 456c 656d 656e 7472  tor1ExprElementr
+00000f10: 0500 0000 da2e 7465 7374 3276 612e 7061  ......test2va.pa
+00000f20: 7273 6572 2e73 7472 7563 7473 2e55 6941  rser.structs.UiA
+00000f30: 7574 6f6d 6174 6f72 3245 7870 7245 6c65  utomator2ExprEle
+00000f40: 6d65 6e74 7206 0000 00da 2a74 6573 7432  mentr.....*test2
+00000f50: 7661 2e70 6172 7365 722e 7374 7275 6374  va.parser.struct
+00000f60: 732e 4573 7072 6573 736f 4465 636c 456c  s.EspressoDeclEl
+00000f70: 656d 656e 7472 0700 0000 da1d 7465 7374  ementr......test
+00000f80: 3276 612e 7061 7273 6572 2e74 7970 6573  2va.parser.types
+00000f90: 2e4c 6962 5479 7065 7372 0800 0000 da29  .LibTypesr.....)
+00000fa0: 7465 7374 3276 612e 7061 7273 6572 2e75  test2va.parser.u
+00000fb0: 7469 6c2e 6669 6e64 5f61 6c6c 5f74 6573  til.find_all_tes
+00000fc0: 745f 6d65 7468 6f64 7372 0900 0000 da25  t_methodsr.....%
+00000fd0: 7465 7374 3276 612e 7061 7273 6572 2e75  test2va.parser.u
+00000fe0: 7469 6c2e 6669 6e64 5f73 6574 7570 5f6d  til.find_setup_m
+00000ff0: 6574 686f 6472 0a00 0000 da20 7465 7374  ethodr..... test
+00001000: 3276 612e 7061 7273 6572 2e75 7469 6c2e  2va.parser.util.
+00001010: 6d6f 6469 6679 5f73 7263 6d6c 720b 0000  modify_srcmlr...
+00001020: 00da 2574 6573 7432 7661 2e70 6172 7365  ..%test2va.parse
+00001030: 722e 7574 696c 2e74 7261 7665 7273 655f  r.util.traverse_
+00001040: 656c 656d 656e 7473 720c 0000 00da 1774  elementsr......t
+00001050: 6573 7432 7661 2e75 7469 6c2e 7772 6974  est2va.util.writ
+00001060: 655f 6a73 6f6e 720d 0000 0072 4400 0000  e_jsonr....rD...
+00001070: a900 7216 0000 0072 1400 0000 fa08 3c6d  ..r....r......<m
+00001080: 6f64 756c 653e 7255 0000 0001 0000 0073  odule>rU.......s
+00001090: 3800 0000 f003 0101 01db 000d db00 09df  8...............
+000010a0: 0022 d000 22dd 001a e500 25dd 0052 dd00  ."..".....%..R..
+000010b0: 52dd 004a dd00 34dd 004b dd00 43dd 0039  R..J..4..K..C..9
+000010c0: dd00 43dd 002e f306 5301 0110 7216 0000  ..C.....S...r...
+000010d0: 00                                       .
```

### Comparing `test2va-1.0.8/test2va/parser/parser.py` & `test2va-1.0.9/test2va/parser/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,16 @@
             method_data["selectors"].append(selector.get_data())
 
         method_data["assertion"] = clazz.parse_assertion(method)
 
         data.append(method_data)
 
     try:
-        write_json(data, f"output/{file_name}_parsed.json")
+        output_path = os.path.join(os.path.dirname(__file__), "../output", f"{file_name}_parsed.json")
+        write_json(data, output_path)
     except Exception as e:
         gui.out(f"⛔ JSON Write Error: {e}")
         return
 
     os.remove(xml)
 
     return data
```

### Comparing `test2va-1.0.8/test2va/parser/structs/EspressoDeclElement.py` & `test2va-1.0.9/test2va/parser/structs/EspressoDeclElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/UiAutomator1ExprElement.py` & `test2va-1.0.9/test2va/parser/structs/UiAutomator1ExprElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/UiAutomator2ExprElement.py` & `test2va-1.0.9/test2va/parser/structs/UiAutomator2ExprElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/XMLElement.py` & `test2va-1.0.9/test2va/parser/structs/XMLElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/types/LibTypes.py` & `test2va-1.0.9/test2va/parser/types/LibTypes.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc` & `test2va-1.0.9/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/find_all_test_methods.py` & `test2va-1.0.9/test2va/parser/util/find_all_test_methods.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/find_setup_method.py` & `test2va-1.0.9/test2va/parser/util/find_setup_method.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/literal_format_check.py` & `test2va-1.0.9/test2va/parser/util/literal_format_check.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/modify_srcml.py` & `test2va-1.0.9/test2va/parser/util/modify_srcml.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/parser/util/traverse_elements.py` & `test2va-1.0.9/test2va/parser/util/traverse_elements.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/util/__pycache__/filter_list.cpython-312.pyc` & `test2va-1.0.9/test2va/util/__pycache__/filter_list.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/util/__pycache__/map_list.cpython-312.pyc` & `test2va-1.0.9/test2va/util/__pycache__/map_list.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va/util/__pycache__/write_json.cpython-312.pyc` & `test2va-1.0.9/test2va/util/__pycache__/write_json.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.8/test2va.egg-info/SOURCES.txt` & `test2va-1.0.9/test2va.egg-info/SOURCES.txt`

 * *Files identical despite different names*

