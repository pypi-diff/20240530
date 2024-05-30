# Comparing `tmp/test2va-1.0.7.tar.gz` & `tmp/test2va-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test2va-1.0.7.tar", last modified: Thu May 30 14:32:53 2024, max compression
+gzip compressed data, was "test2va-1.0.8.tar", last modified: Thu May 30 14:36:05 2024, max compression
```

## Comparing `test2va-1.0.7.tar` & `test2va-1.0.8.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.679841 test2va-1.0.7/
--rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       13 2024-05-30 14:32:50.000000 test2va-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      260 2024-05-30 14:32:53.678841 test2va-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.7/README.md
--rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 14:32:53.679841 test2va-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      563 2024-05-30 14:32:18.000000 test2va-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.519366 test2va-1.0.7/test2va/
--rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.7/test2va/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.534345 test2va-1.0.7/test2va/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.536475 test2va-1.0.7/test2va/const/
--rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.7/test2va/const/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.538474 test2va-1.0.7/test2va/const/__pycache__/
--rw-rw-rw-   0        0        0      275 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/const/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      264 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/const/__pycache__/const.cpython-312.pyc
--rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.7/test2va/const/const.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.503430 test2va-1.0.7/test2va/examples/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.540474 test2va-1.0.7/test2va/examples/NOTES_SetLeftSwipeToDelete/
--rw-rw-rw-   0        0        0     2320 2024-05-29 17:38:34.000000 test2va-1.0.7/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java
--rw-rw-rw-   0        0        0  3860356 2024-03-07 09:41:50.000000 test2va-1.0.7/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.546495 test2va-1.0.7/test2va/generator/
--rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.7/test2va/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.549494 test2va-1.0.7/test2va/generator/__pycache__/
--rw-rw-rw-   0        0        0      198 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1344 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/__pycache__/generator.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.555672 test2va-1.0.7/test2va/generator/core/
--rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.7/test2va/generator/core/GUI.py
--rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/generator/core/GUIMethodReader.py
--rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.7/test2va/generator/core/Method.py
--rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.7/test2va/generator/core/MethodGenerator.py
--rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/generator/core/Mutant.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/generator/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.562723 test2va-1.0.7/test2va/generator/core/__pycache__/
--rw-rw-rw-   0        0        0    13039 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/core/__pycache__/GUI.cpython-312.pyc
--rw-rw-rw-   0        0        0     4552 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc
--rw-rw-rw-   0        0        0    10964 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/core/__pycache__/Method.cpython-312.pyc
--rw-rw-rw-   0        0        0     6697 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc
--rw-rw-rw-   0        0        0     9389 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc
--rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/core/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.567232 test2va-1.0.7/test2va/generator/exceptions/
--rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.7/test2va/generator/exceptions/GUIException.py
--rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.7/test2va/generator/exceptions/MethodException.py
--rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.7/test2va/generator/exceptions/MethodGeneratorException.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/generator/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.571232 test2va-1.0.7/test2va/generator/exceptions/__pycache__/
--rw-rw-rw-   0        0        0      600 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc
--rw-rw-rw-   0        0        0      609 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc
--rw-rw-rw-   0        0        0      636 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc
--rw-rw-rw-   0        0        0      176 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/generator/exceptions/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/generator/generator.py
--rw-rw-rw-   0        0        0    19926 2024-05-30 14:30:05.000000 test2va-1.0.7/test2va/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.573232 test2va-1.0.7/test2va/mutator/
--rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.7/test2va/mutator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.576284 test2va-1.0.7/test2va/mutator/__pycache__/
--rw-rw-rw-   0        0        0      194 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     6037 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/__pycache__/mutator.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.578283 test2va-1.0.7/test2va/mutator/mappings/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/mutator/mappings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.580282 test2va-1.0.7/test2va/mutator/mappings/__pycache__/
--rw-rw-rw-   0        0        0      172 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/mappings/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      910 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc
--rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.7/test2va/mutator/mappings/maps.py
--rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/mutator/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.588296 test2va-1.0.7/test2va/mutator/structs/
--rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/structs/EspressoActions.py
--rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/structs/EspressoCorrelations.py
--rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/structs/EspressoCriteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/structs/UiAutomator1Actions.py
--rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/structs/UiAutomator1Criteria.py
--rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/structs/UiAutomator2Actions.py
--rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.7/test2va/mutator/structs/UiAutomator2Criteria.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/mutator/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.599318 test2va-1.0.7/test2va/mutator/structs/__pycache__/
--rw-rw-rw-   0        0        0     2743 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc
--rw-rw-rw-   0        0        0     2036 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc
--rw-rw-rw-   0        0        0    11035 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc
--rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc
--rw-rw-rw-   0        0        0     3580 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc
--rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc
--rw-rw-rw-   0        0        0      365 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator2Criteria.cpython-312.pyc
--rw-rw-rw-   0        0        0      171 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/structs/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.614052 test2va-1.0.7/test2va/mutator/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/mutator/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.631076 test2va-1.0.7/test2va/mutator/util/__pycache__/
--rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     2661 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc
--rw-rw-rw-   0        0        0      792 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc
--rw-rw-rw-   0        0        0      422 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/clear_user_data.cpython-312.pyc
--rw-rw-rw-   0        0        0      864 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc
--rw-rw-rw-   0        0        0     2008 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc
--rw-rw-rw-   0        0        0     2890 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc
--rw-rw-rw-   0        0        0     1450 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc
--rw-rw-rw-   0        0        0     3207 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc
--rw-rw-rw-   0        0        0      869 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc
--rw-rw-rw-   0        0        0     1898 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc
--rw-rw-rw-   0        0        0     2608 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc
--rw-rw-rw-   0        0        0     2061 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc
--rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.7/test2va/mutator/util/base_test.py
--rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.7/test2va/mutator/util/build_xpath_from_element.py
--rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.7/test2va/mutator/util/clear_user_data.py
--rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/execute_action.py
--rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/execute_assertion.py
--rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/find_assertion_correlations.py
--rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/find_element.py
--rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.7/test2va/mutator/util/find_xml_element.py
--rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.7/test2va/mutator/util/get_element_info.py
--rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/get_true_page_source.py
--rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.7/test2va/mutator/util/grant_permissions.py
--rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/populate_mutators.py
--rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/mutator/util/setup_test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.632075 test2va-1.0.7/test2va/output/
--rw-rw-rw-   0        0        0        4 2024-05-30 14:13:40.000000 test2va-1.0.7/test2va/output/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.634075 test2va-1.0.7/test2va/parser/
--rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.7/test2va/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.636147 test2va-1.0.7/test2va/parser/__pycache__/
--rw-rw-rw-   0        0        0      192 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     4093 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/__pycache__/parser.cpython-312.pyc
--rw-rw-rw-   0        0        0     3416 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.641660 test2va-1.0.7/test2va/parser/structs/
--rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/structs/EspressoDeclElement.py
--rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/structs/UiAutomator1ExprElement.py
--rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/structs/UiAutomator2ExprElement.py
--rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/structs/XMLElement.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/parser/structs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.648176 test2va-1.0.7/test2va/parser/structs/__pycache__/
--rw-rw-rw-   0        0        0    20149 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc
--rw-rw-rw-   0        0        0    19514 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc
--rw-rw-rw-   0        0        0    15481 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc
--rw-rw-rw-   0        0        0     9641 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc
--rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/structs/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.650175 test2va-1.0.7/test2va/parser/types/
--rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.7/test2va/parser/types/LibTypes.py
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/parser/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.652175 test2va-1.0.7/test2va/parser/types/__pycache__/
--rw-rw-rw-   0        0        0     2987 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc
--rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/types/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.658629 test2va-1.0.7/test2va/parser/util/
--rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.7/test2va/parser/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.665483 test2va-1.0.7/test2va/parser/util/__pycache__/
--rw-rw-rw-   0        0        0      167 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/util/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1930 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc
--rw-rw-rw-   0        0        0     1917 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc
--rw-rw-rw-   0        0        0     2097 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc
--rw-rw-rw-   0        0        0     1949 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc
--rw-rw-rw-   0        0        0     1202 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc
--rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/util/find_all_test_methods.py
--rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/util/find_setup_method.py
--rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.7/test2va/parser/util/literal_format_check.py
--rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.7/test2va/parser/util/modify_srcml.py
--rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/parser/util/traverse_elements.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.671483 test2va-1.0.7/test2va/util/
--rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.7/test2va/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.677835 test2va-1.0.7/test2va/util/__pycache__/
--rw-rw-rw-   0        0        0      301 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/util/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      487 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/util/__pycache__/camel_to_snake.cpython-312.pyc
--rw-rw-rw-   0        0        0      539 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/util/__pycache__/filter_list.cpython-312.pyc
--rw-rw-rw-   0        0        0      545 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/util/__pycache__/map_list.cpython-312.pyc
--rw-rw-rw-   0        0        0      538 2024-05-30 14:05:53.000000 test2va-1.0.7/test2va/util/__pycache__/write_json.cpython-312.pyc
--rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.7/test2va/util/camel_to_snake.py
--rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.7/test2va/util/filter_list.py
--rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.7/test2va/util/map_list.py
--rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.7/test2va/util/write_json.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:32:53.533345 test2va-1.0.7/test2va.egg-info/
--rw-rw-rw-   0        0        0      260 2024-05-30 14:32:53.000000 test2va-1.0.7/test2va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6487 2024-05-30 14:32:53.000000 test2va-1.0.7/test2va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:32:53.000000 test2va-1.0.7/test2va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-30 14:32:53.000000 test2va-1.0.7/test2va.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-05-30 14:32:53.000000 test2va-1.0.7/test2va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-30 14:32:53.000000 test2va-1.0.7/test2va.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.347462 test2va-1.0.8/
+-rw-rw-rw-   0        0        0     1065 2024-05-30 13:32:00.000000 test2va-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-05-30 14:32:50.000000 test2va-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      189 2024-05-30 14:36:05.346456 test2va-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-28 14:00:53.000000 test2va-1.0.8/README.md
+-rw-rw-rw-   0        0        0       91 2024-05-30 13:33:54.000000 test2va-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:36:05.347462 test2va-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      563 2024-05-30 14:35:59.000000 test2va-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.190975 test2va-1.0.8/test2va/
+-rw-rw-rw-   0        0        0       58 2024-05-29 17:50:22.000000 test2va-1.0.8/test2va/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.205515 test2va-1.0.8/test2va/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.208519 test2va-1.0.8/test2va/const/
+-rw-rw-rw-   0        0        0       96 2024-05-29 17:59:06.000000 test2va-1.0.8/test2va/const/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.210514 test2va-1.0.8/test2va/const/__pycache__/
+-rw-rw-rw-   0        0        0      275 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/const/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      264 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/const/__pycache__/const.cpython-312.pyc
+-rw-rw-rw-   0        0        0       82 2023-12-06 22:52:35.000000 test2va-1.0.8/test2va/const/const.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.175951 test2va-1.0.8/test2va/examples/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.213515 test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/
+-rw-rw-rw-   0        0        0     2320 2024-05-29 17:38:34.000000 test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java
+-rw-rw-rw-   0        0        0  3860356 2024-03-07 09:41:50.000000 test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.218534 test2va-1.0.8/test2va/generator/
+-rw-rw-rw-   0        0        0       32 2024-05-29 18:19:08.000000 test2va-1.0.8/test2va/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.221533 test2va-1.0.8/test2va/generator/__pycache__/
+-rw-rw-rw-   0        0        0      198 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1344 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/__pycache__/generator.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.228047 test2va-1.0.8/test2va/generator/core/
+-rw-rw-rw-   0        0        0    10649 2024-05-30 13:57:46.000000 test2va-1.0.8/test2va/generator/core/GUI.py
+-rw-rw-rw-   0        0        0     4164 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/generator/core/GUIMethodReader.py
+-rw-rw-rw-   0        0        0    10216 2024-05-30 13:57:46.000000 test2va-1.0.8/test2va/generator/core/Method.py
+-rw-rw-rw-   0        0        0    24640 2024-05-30 13:57:46.000000 test2va-1.0.8/test2va/generator/core/MethodGenerator.py
+-rw-rw-rw-   0        0        0     7055 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/generator/core/Mutant.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/generator/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.235073 test2va-1.0.8/test2va/generator/core/__pycache__/
+-rw-rw-rw-   0        0        0    13039 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/GUI.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4552 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10964 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/Method.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6697 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9389 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc
+-rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/core/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.239075 test2va-1.0.8/test2va/generator/exceptions/
+-rw-rw-rw-   0        0        0       97 2024-05-29 18:14:52.000000 test2va-1.0.8/test2va/generator/exceptions/GUIException.py
+-rw-rw-rw-   0        0        0      100 2024-05-29 18:14:52.000000 test2va-1.0.8/test2va/generator/exceptions/MethodException.py
+-rw-rw-rw-   0        0        0      109 2024-05-29 18:14:52.000000 test2va-1.0.8/test2va/generator/exceptions/MethodGeneratorException.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/generator/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.243580 test2va-1.0.8/test2va/generator/exceptions/__pycache__/
+-rw-rw-rw-   0        0        0      600 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc
+-rw-rw-rw-   0        0        0      609 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc
+-rw-rw-rw-   0        0        0      636 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc
+-rw-rw-rw-   0        0        0      176 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/generator/exceptions/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1306 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/generator/generator.py
+-rw-rw-rw-   0        0        0    19901 2024-05-30 14:35:52.000000 test2va-1.0.8/test2va/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.245586 test2va-1.0.8/test2va/mutator/
+-rw-rw-rw-   0        0        0       30 2024-05-28 14:52:21.000000 test2va-1.0.8/test2va/mutator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.247586 test2va-1.0.8/test2va/mutator/__pycache__/
+-rw-rw-rw-   0        0        0      194 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6037 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/__pycache__/mutator.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.249585 test2va-1.0.8/test2va/mutator/mappings/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/mutator/mappings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.251090 test2va-1.0.8/test2va/mutator/mappings/__pycache__/
+-rw-rw-rw-   0        0        0      172 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/mappings/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      910 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc
+-rw-rw-rw-   0        0        0      844 2024-05-29 18:05:43.000000 test2va-1.0.8/test2va/mutator/mappings/maps.py
+-rw-rw-rw-   0        0        0     7080 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/mutator/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.260439 test2va-1.0.8/test2va/mutator/structs/
+-rw-rw-rw-   0        0        0     1325 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/EspressoActions.py
+-rw-rw-rw-   0        0        0     1085 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/EspressoCorrelations.py
+-rw-rw-rw-   0        0        0     6252 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/EspressoCriteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator1Actions.py
+-rw-rw-rw-   0        0        0     1816 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator1Criteria.py
+-rw-rw-rw-   0        0        0      454 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator2Actions.py
+-rw-rw-rw-   0        0        0       43 2024-02-08 02:56:34.000000 test2va-1.0.8/test2va/mutator/structs/UiAutomator2Criteria.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/mutator/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.270030 test2va-1.0.8/test2va/mutator/structs/__pycache__/
+-rw-rw-rw-   0        0        0     2743 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2036 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc
+-rw-rw-rw-   0        0        0    11035 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3580 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1147 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc
+-rw-rw-rw-   0        0        0      365 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator2Criteria.cpython-312.pyc
+-rw-rw-rw-   0        0        0      171 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/structs/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.284050 test2va-1.0.8/test2va/mutator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/mutator/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.299569 test2va-1.0.8/test2va/mutator/util/__pycache__/
+-rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2661 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc
+-rw-rw-rw-   0        0        0      792 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc
+-rw-rw-rw-   0        0        0      422 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/clear_user_data.cpython-312.pyc
+-rw-rw-rw-   0        0        0      864 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2008 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2890 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1450 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3207 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc
+-rw-rw-rw-   0        0        0      869 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1898 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2608 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2061 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2265 2024-05-29 18:07:44.000000 test2va-1.0.8/test2va/mutator/util/base_test.py
+-rw-rw-rw-   0        0        0      431 2024-03-13 20:47:41.000000 test2va-1.0.8/test2va/mutator/util/build_xpath_from_element.py
+-rw-rw-rw-   0        0        0      178 2024-03-28 13:26:27.000000 test2va-1.0.8/test2va/mutator/util/clear_user_data.py
+-rw-rw-rw-   0        0        0      474 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/execute_action.py
+-rw-rw-rw-   0        0        0     1850 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/execute_assertion.py
+-rw-rw-rw-   0        0        0     3220 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/find_assertion_correlations.py
+-rw-rw-rw-   0        0        0      956 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/find_element.py
+-rw-rw-rw-   0        0        0     2741 2024-05-29 18:49:14.000000 test2va-1.0.8/test2va/mutator/util/find_xml_element.py
+-rw-rw-rw-   0        0        0      491 2024-03-20 14:59:40.000000 test2va-1.0.8/test2va/mutator/util/get_element_info.py
+-rw-rw-rw-   0        0        0      787 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/get_true_page_source.py
+-rw-rw-rw-   0        0        0     1844 2024-03-28 14:14:24.000000 test2va-1.0.8/test2va/mutator/util/grant_permissions.py
+-rw-rw-rw-   0        0        0     1497 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/populate_mutators.py
+-rw-rw-rw-   0        0        0     1821 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/mutator/util/setup_test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.301075 test2va-1.0.8/test2va/output/
+-rw-rw-rw-   0        0        0        4 2024-05-30 14:13:40.000000 test2va-1.0.8/test2va/output/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.302081 test2va-1.0.8/test2va/parser/
+-rw-rw-rw-   0        0        0       28 2024-05-28 14:46:44.000000 test2va-1.0.8/test2va/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.305591 test2va-1.0.8/test2va/parser/__pycache__/
+-rw-rw-rw-   0        0        0      192 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4093 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/__pycache__/parser.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3416 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.310838 test2va-1.0.8/test2va/parser/structs/
+-rw-rw-rw-   0        0        0    16620 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/EspressoDeclElement.py
+-rw-rw-rw-   0        0        0    15901 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/UiAutomator1ExprElement.py
+-rw-rw-rw-   0        0        0    12582 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/UiAutomator2ExprElement.py
+-rw-rw-rw-   0        0        0     6324 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/structs/XMLElement.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/parser/structs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.315934 test2va-1.0.8/test2va/parser/structs/__pycache__/
+-rw-rw-rw-   0        0        0    20149 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0    19514 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0    15481 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9641 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc
+-rw-rw-rw-   0        0        0      170 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/structs/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.318444 test2va-1.0.8/test2va/parser/types/
+-rw-rw-rw-   0        0        0     1400 2024-03-14 13:00:19.000000 test2va-1.0.8/test2va/parser/types/LibTypes.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/parser/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.320444 test2va-1.0.8/test2va/parser/types/__pycache__/
+-rw-rw-rw-   0        0        0     2987 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc
+-rw-rw-rw-   0        0        0      168 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/types/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.326868 test2va-1.0.8/test2va/parser/util/
+-rw-rw-rw-   0        0        0        0 2024-05-29 18:48:54.000000 test2va-1.0.8/test2va/parser/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.334370 test2va-1.0.8/test2va/parser/util/__pycache__/
+-rw-rw-rw-   0        0        0      167 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1930 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1917 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2097 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1949 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1202 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1010 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/util/find_all_test_methods.py
+-rw-rw-rw-   0        0        0     1025 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/util/find_setup_method.py
+-rw-rw-rw-   0        0        0     1486 2024-05-29 18:12:22.000000 test2va-1.0.8/test2va/parser/util/literal_format_check.py
+-rw-rw-rw-   0        0        0     1237 2023-11-27 23:10:33.000000 test2va-1.0.8/test2va/parser/util/modify_srcml.py
+-rw-rw-rw-   0        0        0      769 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/parser/util/traverse_elements.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.339375 test2va-1.0.8/test2va/util/
+-rw-rw-rw-   0        0        0      150 2024-05-29 18:03:17.000000 test2va-1.0.8/test2va/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.345457 test2va-1.0.8/test2va/util/__pycache__/
+-rw-rw-rw-   0        0        0      301 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      487 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/camel_to_snake.cpython-312.pyc
+-rw-rw-rw-   0        0        0      539 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/filter_list.cpython-312.pyc
+-rw-rw-rw-   0        0        0      545 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/map_list.cpython-312.pyc
+-rw-rw-rw-   0        0        0      538 2024-05-30 14:05:53.000000 test2va-1.0.8/test2va/util/__pycache__/write_json.cpython-312.pyc
+-rw-rw-rw-   0        0        0      144 2024-02-22 05:30:14.000000 test2va-1.0.8/test2va/util/camel_to_snake.py
+-rw-rw-rw-   0        0        0      240 2023-07-24 05:23:56.000000 test2va-1.0.8/test2va/util/filter_list.py
+-rw-rw-rw-   0        0        0      244 2023-07-24 05:23:56.000000 test2va-1.0.8/test2va/util/map_list.py
+-rw-rw-rw-   0        0        0      180 2024-05-30 13:57:45.000000 test2va-1.0.8/test2va/util/write_json.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:36:05.204514 test2va-1.0.8/test2va.egg-info/
+-rw-rw-rw-   0        0        0      189 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6487 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 14:36:05.000000 test2va-1.0.8/test2va.egg-info/top_level.txt
```

### Comparing `test2va-1.0.7/LICENSE` & `test2va-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/setup.py` & `test2va-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='test2va',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     install_requires=['appium-python-client==3.1.1', 'pylibsrcml'],
     license='MIT',
     author='Anon',
     include_package_data=True,
     description='Test2VA',
     long_description=open('README.md').read(),
```

### Comparing `test2va-1.0.7/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java` & `test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/NOTES_SetLeftSwipeToDelete.java`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk` & `test2va-1.0.8/test2va/examples/NOTES_SetLeftSwipeToDelete/another-notes-app.apk`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/__pycache__/generator.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/__pycache__/generator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/GUI.py` & `test2va-1.0.8/test2va/generator/core/GUI.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/GUIMethodReader.py` & `test2va-1.0.8/test2va/generator/core/GUIMethodReader.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/Method.py` & `test2va-1.0.8/test2va/generator/core/Method.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/MethodGenerator.py` & `test2va-1.0.8/test2va/generator/core/MethodGenerator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/Mutant.py` & `test2va-1.0.8/test2va/generator/core/Mutant.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/__pycache__/GUI.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/core/__pycache__/GUI.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/core/__pycache__/GUIMethodReader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/__pycache__/Method.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/core/__pycache__/Method.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/core/__pycache__/MethodGenerator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/core/__pycache__/Mutant.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/exceptions/__pycache__/GUIException.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodException.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc` & `test2va-1.0.8/test2va/generator/exceptions/__pycache__/MethodGeneratorException.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/generator/generator.py` & `test2va-1.0.8/test2va/generator/generator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/gui.py` & `test2va-1.0.8/test2va/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
             print(file_name)
 
             start = time.time()
             self.out("ℹ️ Parsing input...",)
             data = None
 
             try:
-                data = parser.parser(file_name, self)
+                data = parser(file_name, self)
             except Exception as e:
                 self.out(f"⛔ Unknown parsing error {e}", True)
                 self.driver.quit()
                 self.started = False
                 self.start_button.config(text="Start")
                 self.driver = None
                 return
@@ -401,15 +401,15 @@
             self.out(f"⏳ Waiting for the app to load...")
             time.sleep(3)
 
             self.out("ℹ️ Attempting possible mutable paths...")
             auto_grant_perms = self.perm_var.get() == 1
 
             try:
-                paths = mutator.mutator(self.driver, data[0], auto_grant_perms)
+                paths = mutator(self.driver, data[0], auto_grant_perms)
             except Exception as e:
                 self.out(f"⛔ Unknown mutator error {e}", True)
                 self.driver.quit()
                 self.started = False
                 self.start_button.config(text="Start")
                 self.driver = None
                 return
@@ -423,15 +423,15 @@
             self.out(f"✔️ Mutation results saved to {output_path}")
 
             self.out("ℹ️ Generating task methods...")
 
             input_path = os.path.join(os.path.dirname(__file__), "output")
 
             try:
-                generator.generator(input_path)
+                generator(input_path)
             except Exception as e:
                 self.out(f"⛔ Unknown generator error {e}", True)
                 self.driver.quit()
                 self.started = False
                 self.start_button.config(text="Start")
                 self.driver = None
                 return
```

### Comparing `test2va-1.0.7/test2va/mutator/__pycache__/mutator.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/__pycache__/mutator.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/mappings/__pycache__/maps.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/mappings/maps.py` & `test2va-1.0.8/test2va/mutator/mappings/maps.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/mutator.py` & `test2va-1.0.8/test2va/mutator/mutator.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/EspressoActions.py` & `test2va-1.0.8/test2va/mutator/structs/EspressoActions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/EspressoCorrelations.py` & `test2va-1.0.8/test2va/mutator/structs/EspressoCorrelations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/EspressoCriteria.py` & `test2va-1.0.8/test2va/mutator/structs/EspressoCriteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/UiAutomator1Criteria.py` & `test2va-1.0.8/test2va/mutator/structs/UiAutomator1Criteria.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoActions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCorrelations.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/structs/__pycache__/EspressoCriteria.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Actions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator1Criteria.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/structs/__pycache__/UiAutomator2Actions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/base_test.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/build_xpath_from_element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/execute_action.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/execute_assertion.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/find_assertion_correlations.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/find_element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/find_xml_element.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/get_element_info.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/grant_permissions.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/populate_mutators.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc` & `test2va-1.0.8/test2va/mutator/util/__pycache__/setup_test.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/base_test.py` & `test2va-1.0.8/test2va/mutator/util/base_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/execute_assertion.py` & `test2va-1.0.8/test2va/mutator/util/execute_assertion.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/find_assertion_correlations.py` & `test2va-1.0.8/test2va/mutator/util/find_assertion_correlations.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/find_element.py` & `test2va-1.0.8/test2va/mutator/util/find_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/find_xml_element.py` & `test2va-1.0.8/test2va/mutator/util/find_xml_element.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/get_true_page_source.py` & `test2va-1.0.8/test2va/mutator/util/get_true_page_source.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/grant_permissions.py` & `test2va-1.0.8/test2va/mutator/util/grant_permissions.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/populate_mutators.py` & `test2va-1.0.8/test2va/mutator/util/populate_mutators.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/mutator/util/setup_test.py` & `test2va-1.0.8/test2va/mutator/util/setup_test.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/__pycache__/parser.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/__pycache__/parser.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/parser.py` & `test2va-1.0.8/test2va/parser/parser.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/EspressoDeclElement.py` & `test2va-1.0.8/test2va/parser/structs/EspressoDeclElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/UiAutomator1ExprElement.py` & `test2va-1.0.8/test2va/parser/structs/UiAutomator1ExprElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/UiAutomator2ExprElement.py` & `test2va-1.0.8/test2va/parser/structs/UiAutomator2ExprElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/XMLElement.py` & `test2va-1.0.8/test2va/parser/structs/XMLElement.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/structs/__pycache__/EspressoDeclElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator1ExprElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/structs/__pycache__/UiAutomator2ExprElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/structs/__pycache__/XMLElement.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/types/LibTypes.py` & `test2va-1.0.8/test2va/parser/types/LibTypes.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/types/__pycache__/LibTypes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/util/__pycache__/find_all_test_methods.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/util/__pycache__/find_setup_method.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/util/__pycache__/literal_format_check.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/util/__pycache__/modify_srcml.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc` & `test2va-1.0.8/test2va/parser/util/__pycache__/traverse_elements.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/find_all_test_methods.py` & `test2va-1.0.8/test2va/parser/util/find_all_test_methods.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/find_setup_method.py` & `test2va-1.0.8/test2va/parser/util/find_setup_method.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/literal_format_check.py` & `test2va-1.0.8/test2va/parser/util/literal_format_check.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/modify_srcml.py` & `test2va-1.0.8/test2va/parser/util/modify_srcml.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/parser/util/traverse_elements.py` & `test2va-1.0.8/test2va/parser/util/traverse_elements.py`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/util/__pycache__/filter_list.cpython-312.pyc` & `test2va-1.0.8/test2va/util/__pycache__/filter_list.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/util/__pycache__/map_list.cpython-312.pyc` & `test2va-1.0.8/test2va/util/__pycache__/map_list.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va/util/__pycache__/write_json.cpython-312.pyc` & `test2va-1.0.8/test2va/util/__pycache__/write_json.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `test2va-1.0.7/test2va.egg-info/SOURCES.txt` & `test2va-1.0.8/test2va.egg-info/SOURCES.txt`

 * *Files identical despite different names*

