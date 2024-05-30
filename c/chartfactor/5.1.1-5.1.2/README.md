# Comparing `tmp/chartfactor-5.1.1.tar.gz` & `tmp/chartfactor-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartfactor-5.1.1.tar", last modified: Wed May 29 13:41:34 2024, max compression
+gzip compressed data, was "chartfactor-5.1.2.tar", last modified: Thu May 30 20:58:58 2024, max compression
```

## Comparing `chartfactor-5.1.1.tar` & `chartfactor-5.1.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.511648 chartfactor-5.1.1/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    10759 2022-02-01 20:13:50.000000 chartfactor-5.1.1/LICENSE
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      333 2022-09-08 13:41:06.000000 chartfactor-5.1.1/MANIFEST.in
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1942 2024-05-29 13:41:34.511447 chartfactor-5.1.1/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1191 2022-09-08 13:41:06.000000 chartfactor-5.1.1/README.md
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.490978 chartfactor-5.1.1/chartfactor/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      373 2022-09-15 22:28:11.000000 chartfactor-5.1.1/chartfactor/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       65 2022-02-01 20:13:50.000000 chartfactor-5.1.1/chartfactor/main.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.495359 chartfactor-5.1.1/chartfactor/src/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      432 2022-02-01 20:13:50.000000 chartfactor-5.1.1/chartfactor/src/__init__.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.495488 chartfactor-5.1.1/chartfactor/src/assets/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-24 20:09:31.000000 chartfactor-5.1.1/chartfactor/src/assets/__init__.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.495654 chartfactor-5.1.1/chartfactor/src/assets/css/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-24 20:09:31.000000 chartfactor-5.1.1/chartfactor/src/assets/css/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1291 2022-10-10 15:44:38.000000 chartfactor-5.1.1/chartfactor/src/assets/css/style.css
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.496925 chartfactor-5.1.1/chartfactor/src/assets/js/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-24 20:09:31.000000 chartfactor-5.1.1/chartfactor/src/assets/js/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2454 2022-09-08 13:41:06.000000 chartfactor-5.1.1/chartfactor/src/assets/js/cf-message-event-listener.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     6956 2022-06-22 21:03:10.000000 chartfactor-5.1.1/chartfactor/src/assets/js/execute-python.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      413 2022-09-08 13:41:06.000000 chartfactor-5.1.1/chartfactor/src/assets/js/jupyter-notebook-active-cell-change.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    23114 2022-09-15 22:28:11.000000 chartfactor-5.1.1/chartfactor/src/assets/js/kaggle-specs.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      348 2022-06-22 21:03:10.000000 chartfactor-5.1.1/chartfactor/src/assets/js/send-message.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     4643 2022-06-18 22:07:37.000000 chartfactor-5.1.1/chartfactor/src/attribute.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       23 2024-05-29 13:40:46.000000 chartfactor-5.1.1/chartfactor/src/build_info.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    30554 2023-01-24 23:06:43.000000 chartfactor-5.1.1/chartfactor/src/cf.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    25377 2023-01-24 23:06:43.000000 chartfactor-5.1.1/chartfactor/src/code_generator.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     4552 2022-09-08 13:41:06.000000 chartfactor-5.1.1/chartfactor/src/color.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1119 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/column.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     5016 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/compare_metric.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2025 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/field.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     3203 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/filter.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2485 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/grid.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1291 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/legend.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1223 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/markline.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     4991 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/metric.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    98639 2023-10-16 13:44:45.000000 chartfactor-5.1.1/chartfactor/src/provider.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.499347 chartfactor-5.1.1/chartfactor/src/resources/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-03 21:38:09.000000 chartfactor-5.1.1/chartfactor/src/resources/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1062 2022-02-01 20:13:50.000000 chartfactor-5.1.1/chartfactor/src/resources/commons.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    45605 2022-06-22 21:03:10.000000 chartfactor-5.1.1/chartfactor/src/resources/constants.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     4190 2022-10-10 15:44:38.000000 chartfactor-5.1.1/chartfactor/src/resources/html_template.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      709 2022-06-22 21:03:10.000000 chartfactor-5.1.1/chartfactor/src/resources/static_files_manager.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1103 2022-04-09 21:56:18.000000 chartfactor-5.1.1/chartfactor/src/row.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.511207 chartfactor-5.1.1/chartfactor.egg-info/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1942 2024-05-29 13:41:34.000000 chartfactor-5.1.1/chartfactor.egg-info/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1561 2024-05-29 13:41:34.000000 chartfactor-5.1.1/chartfactor.egg-info/SOURCES.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-29 13:41:34.000000 chartfactor-5.1.1/chartfactor.egg-info/dependency_links.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      156 2024-05-29 13:41:34.000000 chartfactor-5.1.1/chartfactor.egg-info/requires.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       18 2024-05-29 13:41:34.000000 chartfactor-5.1.1/chartfactor.egg-info/top_level.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      103 2022-02-01 20:13:50.000000 chartfactor-5.1.1/pyproject.toml
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-05-29 13:41:34.511681 chartfactor-5.1.1/setup.cfg
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1014 2024-05-29 13:41:29.000000 chartfactor-5.1.1/setup.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.500980 chartfactor-5.1.1/tests/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-01 20:13:50.000000 chartfactor-5.1.1/tests/__init__.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-29 13:41:34.504842 chartfactor-5.1.1/tests/data/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-01 20:13:50.000000 chartfactor-5.1.1/tests/data/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    51698 2022-02-01 20:13:50.000000 chartfactor-5.1.1/tests/data/get_visualization_js_code_data.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)  2109816 2022-09-29 23:56:38.000000 chartfactor-5.1.1/tests/data/provider_comparative_data.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)   563117 2023-10-16 13:44:45.000000 chartfactor-5.1.1/tests/data/provider_data.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    54923 2022-02-01 20:13:50.000000 chartfactor-5.1.1/tests/test_get_visualization_js_code.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)   115376 2023-10-16 13:44:45.000000 chartfactor-5.1.1/tests/test_provider.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)   207995 2023-10-16 13:44:45.000000 chartfactor-5.1.1/tests/test_provider_comparative.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.611177 chartfactor-5.1.2/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    10759 2022-02-01 20:13:50.000000 chartfactor-5.1.2/LICENSE
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      333 2022-09-08 13:41:06.000000 chartfactor-5.1.2/MANIFEST.in
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1942 2024-05-30 20:58:58.610960 chartfactor-5.1.2/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1191 2022-09-08 13:41:06.000000 chartfactor-5.1.2/README.md
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.595425 chartfactor-5.1.2/chartfactor/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      373 2022-09-15 22:28:11.000000 chartfactor-5.1.2/chartfactor/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       65 2022-02-01 20:13:50.000000 chartfactor-5.1.2/chartfactor/main.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.600035 chartfactor-5.1.2/chartfactor/src/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      432 2022-02-01 20:13:50.000000 chartfactor-5.1.2/chartfactor/src/__init__.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.600175 chartfactor-5.1.2/chartfactor/src/assets/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-24 20:09:31.000000 chartfactor-5.1.2/chartfactor/src/assets/__init__.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.600354 chartfactor-5.1.2/chartfactor/src/assets/css/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-24 20:09:31.000000 chartfactor-5.1.2/chartfactor/src/assets/css/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1291 2022-10-10 15:44:38.000000 chartfactor-5.1.2/chartfactor/src/assets/css/style.css
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.601695 chartfactor-5.1.2/chartfactor/src/assets/js/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-24 20:09:31.000000 chartfactor-5.1.2/chartfactor/src/assets/js/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2454 2022-09-08 13:41:06.000000 chartfactor-5.1.2/chartfactor/src/assets/js/cf-message-event-listener.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     6956 2022-06-22 21:03:10.000000 chartfactor-5.1.2/chartfactor/src/assets/js/execute-python.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      413 2022-09-08 13:41:06.000000 chartfactor-5.1.2/chartfactor/src/assets/js/jupyter-notebook-active-cell-change.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    23114 2022-09-15 22:28:11.000000 chartfactor-5.1.2/chartfactor/src/assets/js/kaggle-specs.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      348 2022-06-22 21:03:10.000000 chartfactor-5.1.2/chartfactor/src/assets/js/send-message.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     4643 2022-06-18 22:07:37.000000 chartfactor-5.1.2/chartfactor/src/attribute.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       23 2024-05-30 20:58:43.000000 chartfactor-5.1.2/chartfactor/src/build_info.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    30554 2023-01-24 23:06:43.000000 chartfactor-5.1.2/chartfactor/src/cf.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    25377 2023-01-24 23:06:43.000000 chartfactor-5.1.2/chartfactor/src/code_generator.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     4552 2022-09-08 13:41:06.000000 chartfactor-5.1.2/chartfactor/src/color.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1119 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/column.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     5016 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/compare_metric.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2025 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/field.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     3203 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/filter.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2485 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/grid.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1291 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/legend.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1223 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/markline.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     4991 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/metric.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    98639 2023-10-16 13:44:45.000000 chartfactor-5.1.2/chartfactor/src/provider.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.603162 chartfactor-5.1.2/chartfactor/src/resources/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-01-03 21:38:09.000000 chartfactor-5.1.2/chartfactor/src/resources/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1062 2022-02-01 20:13:50.000000 chartfactor-5.1.2/chartfactor/src/resources/commons.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    45605 2022-06-22 21:03:10.000000 chartfactor-5.1.2/chartfactor/src/resources/constants.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     4190 2022-10-10 15:44:38.000000 chartfactor-5.1.2/chartfactor/src/resources/html_template.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      709 2022-06-22 21:03:10.000000 chartfactor-5.1.2/chartfactor/src/resources/static_files_manager.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1103 2022-04-09 21:56:18.000000 chartfactor-5.1.2/chartfactor/src/row.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.610688 chartfactor-5.1.2/chartfactor.egg-info/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1942 2024-05-30 20:58:58.000000 chartfactor-5.1.2/chartfactor.egg-info/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1561 2024-05-30 20:58:58.000000 chartfactor-5.1.2/chartfactor.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-30 20:58:58.000000 chartfactor-5.1.2/chartfactor.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      156 2024-05-30 20:58:58.000000 chartfactor-5.1.2/chartfactor.egg-info/requires.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       18 2024-05-30 20:58:58.000000 chartfactor-5.1.2/chartfactor.egg-info/top_level.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      103 2022-02-01 20:13:50.000000 chartfactor-5.1.2/pyproject.toml
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-05-30 20:58:58.611219 chartfactor-5.1.2/setup.cfg
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1014 2024-05-30 20:58:55.000000 chartfactor-5.1.2/setup.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.604939 chartfactor-5.1.2/tests/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-01 20:13:50.000000 chartfactor-5.1.2/tests/__init__.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-30 20:58:58.608535 chartfactor-5.1.2/tests/data/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-01 20:13:50.000000 chartfactor-5.1.2/tests/data/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    51698 2022-02-01 20:13:50.000000 chartfactor-5.1.2/tests/data/get_visualization_js_code_data.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)  2109816 2022-09-29 23:56:38.000000 chartfactor-5.1.2/tests/data/provider_comparative_data.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)   563117 2023-10-16 13:44:45.000000 chartfactor-5.1.2/tests/data/provider_data.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    54923 2022-02-01 20:13:50.000000 chartfactor-5.1.2/tests/test_get_visualization_js_code.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)   115376 2023-10-16 13:44:45.000000 chartfactor-5.1.2/tests/test_provider.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)   207995 2023-10-16 13:44:45.000000 chartfactor-5.1.2/tests/test_provider_comparative.py
```

### Comparing `chartfactor-5.1.1/LICENSE` & `chartfactor-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/PKG-INFO` & `chartfactor-5.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor
-Version: 5.1.1
+Version: 5.1.2
 Summary: Integrates ChartFactor with Jupyter Notebooks
 Home-page: https://github.com/Aktiun/chartfactor-py
 Author: Aktiun
 Author-email: juan.dominguez@aktiun.com
 Keywords: aktiun,jupyter,jupyterhub,jupyterlab,chartfactor-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: pandas
 Requires-Dist: pandasql>=0.7.3
 Requires-Dist: pygeohash==1.2.0
 Requires-Dist: jsonschema>=3.2.0
 Requires-Dist: colorama>=0.4.4
 Requires-Dist: importlib-resources>=5.4.0
 Requires-Dist: tzlocal~=4.1
-Requires-Dist: chartfactor-jlab-ext==5.1.1
+Requires-Dist: chartfactor-jlab-ext==5.1.2
 
 # ChartFactor for Python
 
 [ChartFactor Py](https://chartfactor.com/doc/latest/cfpy_overview/) is built on top of [ChartFactor](https://chartfactor.com), the lightweight visual analytics platform. It includes [ChartFactor Studio](https://chartfactor.com/doc/latest/studio_intro/) and the [ChartFactor Toolkit](https://chartfactor.com/doc/latest/architecture/) between other components.
 
 # Installing Chartfactor Py
```

### Comparing `chartfactor-5.1.1/README.md` & `chartfactor-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/assets/css/style.css` & `chartfactor-5.1.2/chartfactor/src/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/assets/js/cf-message-event-listener.js` & `chartfactor-5.1.2/chartfactor/src/assets/js/cf-message-event-listener.js`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/assets/js/execute-python.js` & `chartfactor-5.1.2/chartfactor/src/assets/js/execute-python.js`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/assets/js/kaggle-specs.js` & `chartfactor-5.1.2/chartfactor/src/assets/js/kaggle-specs.js`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/attribute.py` & `chartfactor-5.1.2/chartfactor/src/attribute.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/cf.py` & `chartfactor-5.1.2/chartfactor/src/cf.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/code_generator.py` & `chartfactor-5.1.2/chartfactor/src/code_generator.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/color.py` & `chartfactor-5.1.2/chartfactor/src/color.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/column.py` & `chartfactor-5.1.2/chartfactor/src/column.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/compare_metric.py` & `chartfactor-5.1.2/chartfactor/src/compare_metric.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/field.py` & `chartfactor-5.1.2/chartfactor/src/field.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/filter.py` & `chartfactor-5.1.2/chartfactor/src/filter.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/grid.py` & `chartfactor-5.1.2/chartfactor/src/grid.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/legend.py` & `chartfactor-5.1.2/chartfactor/src/legend.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/markline.py` & `chartfactor-5.1.2/chartfactor/src/markline.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/metric.py` & `chartfactor-5.1.2/chartfactor/src/metric.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/provider.py` & `chartfactor-5.1.2/chartfactor/src/provider.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/resources/commons.py` & `chartfactor-5.1.2/chartfactor/src/resources/commons.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/resources/constants.py` & `chartfactor-5.1.2/chartfactor/src/resources/constants.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/resources/html_template.py` & `chartfactor-5.1.2/chartfactor/src/resources/html_template.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/resources/static_files_manager.py` & `chartfactor-5.1.2/chartfactor/src/resources/static_files_manager.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor/src/row.py` & `chartfactor-5.1.2/chartfactor/src/row.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/chartfactor.egg-info/PKG-INFO` & `chartfactor-5.1.2/chartfactor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor
-Version: 5.1.1
+Version: 5.1.2
 Summary: Integrates ChartFactor with Jupyter Notebooks
 Home-page: https://github.com/Aktiun/chartfactor-py
 Author: Aktiun
 Author-email: juan.dominguez@aktiun.com
 Keywords: aktiun,jupyter,jupyterhub,jupyterlab,chartfactor-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: pandas
 Requires-Dist: pandasql>=0.7.3
 Requires-Dist: pygeohash==1.2.0
 Requires-Dist: jsonschema>=3.2.0
 Requires-Dist: colorama>=0.4.4
 Requires-Dist: importlib-resources>=5.4.0
 Requires-Dist: tzlocal~=4.1
-Requires-Dist: chartfactor-jlab-ext==5.1.1
+Requires-Dist: chartfactor-jlab-ext==5.1.2
 
 # ChartFactor for Python
 
 [ChartFactor Py](https://chartfactor.com/doc/latest/cfpy_overview/) is built on top of [ChartFactor](https://chartfactor.com), the lightweight visual analytics platform. It includes [ChartFactor Studio](https://chartfactor.com/doc/latest/studio_intro/) and the [ChartFactor Toolkit](https://chartfactor.com/doc/latest/architecture/) between other components.
 
 # Installing Chartfactor Py
```

### Comparing `chartfactor-5.1.1/chartfactor.egg-info/SOURCES.txt` & `chartfactor-5.1.2/chartfactor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/setup.py` & `chartfactor-5.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='chartfactor',
-    version='5.1.1',
+    version='5.1.2',
     description='Integrates ChartFactor with Jupyter Notebooks',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Aktiun/chartfactor-py',
     author='Aktiun',
     author_email='juan.dominguez@aktiun.com',
     packages=find_packages(),
@@ -21,15 +21,15 @@
         'pandas',
         'pandasql>=0.7.3',
         'pygeohash==1.2.0',
         'jsonschema>=3.2.0',
         'colorama>=0.4.4',
         'importlib-resources>=5.4.0',
         'tzlocal~=4.1',
-        'chartfactor-jlab-ext==5.1.1',
+        'chartfactor-jlab-ext==5.1.2',
     ],
     include_package_data=True,
     keywords=['aktiun', 'jupyter', 'jupyterhub', 'jupyterlab', 'chartfactor-py'],
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

### Comparing `chartfactor-5.1.1/tests/data/get_visualization_js_code_data.py` & `chartfactor-5.1.2/tests/data/get_visualization_js_code_data.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/tests/data/provider_comparative_data.py` & `chartfactor-5.1.2/tests/data/provider_comparative_data.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/tests/data/provider_data.py` & `chartfactor-5.1.2/tests/data/provider_data.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/tests/test_get_visualization_js_code.py` & `chartfactor-5.1.2/tests/test_get_visualization_js_code.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/tests/test_provider.py` & `chartfactor-5.1.2/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `chartfactor-5.1.1/tests/test_provider_comparative.py` & `chartfactor-5.1.2/tests/test_provider_comparative.py`

 * *Files identical despite different names*

