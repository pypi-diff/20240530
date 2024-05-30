# Comparing `tmp/nglui-3.0.2.tar.gz` & `tmp/nglui-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nglui-3.0.2.tar", last modified: Fri Jan 19 23:59:15 2024, max compression
+gzip compressed data, was "nglui-3.0.3.tar", last modified: Tue Apr 30 23:27:04 2024, max compression
```

## Comparing `nglui-3.0.2.tar` & `nglui-3.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.553857 nglui-3.0.2/
--rw-r--r--   0 caseysm    (501) staff       (20)    11356 2022-11-16 18:20:30.000000 nglui-3.0.2/LICENSE.license
--rw-r--r--   0 caseysm    (501) staff       (20)       73 2022-11-16 18:20:30.000000 nglui-3.0.2/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     1782 2024-01-19 23:59:15.553771 nglui-3.0.2/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1190 2023-12-22 01:48:42.000000 nglui-3.0.2/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.540947 nglui-3.0.2/examples/
--rw-r--r--   0 caseysm    (501) staff       (20)  1130416 2022-11-16 18:20:30.000000 nglui-3.0.2/examples/dash_example_data.h5
--rw-r--r--   0 caseysm    (501) staff       (20)     1867 2022-11-16 18:20:30.000000 nglui-3.0.2/examples/dash_with_statebuilder.py
--rw-r--r--   0 caseysm    (501) staff       (20)  3747792 2022-11-16 18:20:30.000000 nglui-3.0.2/examples/example_data.h5
--rw-r--r--   0 caseysm    (501) staff       (20)    29998 2023-01-30 22:58:07.000000 nglui-3.0.2/examples/statebuilder_examples.ipynb
--rw-r--r--   0 caseysm    (501) staff       (20)      103 2024-01-19 18:54:12.000000 nglui-3.0.2/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      126 2024-01-19 23:59:15.554121 nglui-3.0.2/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1406 2022-11-16 18:20:30.000000 nglui-3.0.2/setup.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.532627 nglui-3.0.2/src/
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.541400 nglui-3.0.2/src/nglui/
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2024-01-19 23:59:06.000000 nglui-3.0.2/src/nglui/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.542246 nglui-3.0.2/src/nglui/easyviewer/
--rw-r--r--   0 caseysm    (501) staff       (20)      433 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.545431 nglui-3.0.2/src/nglui/easyviewer/ev_base/
--rw-r--r--   0 caseysm    (501) staff       (20)       81 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1915 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/annotation_compatibility.py
--rw-r--r--   0 caseysm    (501) staff       (20)     8857 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/base.py
--rw-r--r--   0 caseysm    (501) staff       (20)    10584 2024-01-19 23:52:43.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/mainline.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.548435 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/
--rw-r--r--   0 caseysm    (501) staff       (20)      909 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4927 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/annotation.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6226 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/equivalence_map.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1623 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/json_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9861 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/json_wrappers.py
--rw-r--r--   0 caseysm    (501) staff       (20)      753 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/random_token.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2958 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/skeleton.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4758 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/trackable_state.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3944 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/url_state.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1574 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6920 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6866 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer_config_state.py
--rw-r--r--   0 caseysm    (501) staff       (20)    30305 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer_state.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.549075 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite_compatibility/
--rw-r--r--   0 caseysm    (501) staff       (20)      350 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite_compatibility/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)      101 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite_compatibility/base.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15251 2024-01-19 18:39:34.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/seunglab.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2078 2024-01-19 23:49:14.000000 nglui-3.0.2/src/nglui/easyviewer/ev_base/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.550097 nglui-3.0.2/src/nglui/parser/
--rw-r--r--   0 caseysm    (501) staff       (20)       20 2022-11-16 18:20:30.000000 nglui-3.0.2/src/nglui/parser/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    18969 2023-12-22 09:11:05.000000 nglui-3.0.2/src/nglui/parser/base.py
--rw-r--r--   0 caseysm    (501) staff       (20)      434 2023-12-21 03:04:46.000000 nglui-3.0.2/src/nglui/parser/info.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.552466 nglui-3.0.2/src/nglui/statebuilder/
--rw-r--r--   0 caseysm    (501) staff       (20)      351 2023-05-16 22:19:13.000000 nglui-3.0.2/src/nglui/statebuilder/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    30248 2023-12-22 09:06:45.000000 nglui-3.0.2/src/nglui/statebuilder/helpers.py
--rw-r--r--   0 caseysm    (501) staff       (20)    17089 2023-12-22 02:48:43.000000 nglui-3.0.2/src/nglui/statebuilder/layers.py
--rw-r--r--   0 caseysm    (501) staff       (20)    32489 2023-12-22 03:01:24.000000 nglui-3.0.2/src/nglui/statebuilder/mappers.py
--rw-r--r--   0 caseysm    (501) staff       (20)    10966 2024-01-19 23:50:18.000000 nglui-3.0.2/src/nglui/statebuilder/statebuilder.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2807 2023-12-29 01:45:09.000000 nglui-3.0.2/src/nglui/statebuilder/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.553489 nglui-3.0.2/src/nglui.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     1782 2024-01-19 23:59:15.000000 nglui-3.0.2/src/nglui.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1839 2024-01-19 23:59:15.000000 nglui-3.0.2/src/nglui.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-01-19 23:59:15.000000 nglui-3.0.2/src/nglui.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      104 2024-01-19 23:59:15.000000 nglui-3.0.2/src/nglui.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        6 2024-01-19 23:59:15.000000 nglui-3.0.2/src/nglui.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      124 2022-11-16 18:20:30.000000 nglui-3.0.2/test_requirements.txt
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-01-19 23:59:15.553140 nglui-3.0.2/tests/
--rw-r--r--   0 caseysm    (501) staff       (20)     1423 2022-11-16 18:20:30.000000 nglui-3.0.2/tests/test_parser.py
--rw-r--r--   0 caseysm    (501) staff       (20)    12670 2024-01-19 23:57:50.000000 nglui-3.0.2/tests/test_statebuilder.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5117 2023-12-21 03:04:46.000000 nglui-3.0.2/tests/test_viewer.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.213481 nglui-3.0.3/
+-rw-r--r--   0 caseysm    (501) staff       (20)    11356 2024-03-08 20:04:52.000000 nglui-3.0.3/LICENSE.license
+-rw-r--r--   0 caseysm    (501) staff       (20)       73 2022-11-16 18:20:30.000000 nglui-3.0.3/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)     1782 2024-04-30 23:27:04.213341 nglui-3.0.3/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1190 2023-12-22 01:48:42.000000 nglui-3.0.3/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.194862 nglui-3.0.3/examples/
+-rw-r--r--   0 caseysm    (501) staff       (20)  1130416 2022-11-16 18:20:30.000000 nglui-3.0.3/examples/dash_example_data.h5
+-rw-r--r--   0 caseysm    (501) staff       (20)     1867 2022-11-16 18:20:30.000000 nglui-3.0.3/examples/dash_with_statebuilder.py
+-rw-r--r--   0 caseysm    (501) staff       (20)  3747792 2022-11-16 18:20:30.000000 nglui-3.0.3/examples/example_data.h5
+-rw-r--r--   0 caseysm    (501) staff       (20)    29998 2023-01-30 22:58:07.000000 nglui-3.0.3/examples/statebuilder_examples.ipynb
+-rw-r--r--   0 caseysm    (501) staff       (20)      103 2024-03-08 23:44:33.000000 nglui-3.0.3/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      126 2024-04-30 23:27:04.213802 nglui-3.0.3/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1406 2022-11-16 18:20:30.000000 nglui-3.0.3/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.186057 nglui-3.0.3/src/
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.197321 nglui-3.0.3/src/nglui/
+-rw-r--r--   0 caseysm    (501) staff       (20)      112 2024-04-30 23:26:50.000000 nglui-3.0.3/src/nglui/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.198393 nglui-3.0.3/src/nglui/easyviewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)      433 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.201813 nglui-3.0.3/src/nglui/easyviewer/ev_base/
+-rw-r--r--   0 caseysm    (501) staff       (20)       81 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1915 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/annotation_compatibility.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     8857 2024-02-27 02:56:31.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    10584 2024-01-19 23:52:43.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/mainline.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.205180 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/
+-rw-r--r--   0 caseysm    (501) staff       (20)      909 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4927 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/annotation.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6226 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/equivalence_map.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1623 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/json_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9865 2024-03-08 19:54:38.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/json_wrappers.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      753 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/random_token.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2958 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/skeleton.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4758 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/trackable_state.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3944 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/url_state.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1574 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6920 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6866 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer_config_state.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    30178 2024-04-30 23:22:34.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer_state.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.205888 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite_compatibility/
+-rw-r--r--   0 caseysm    (501) staff       (20)      350 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite_compatibility/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      101 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite_compatibility/base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15166 2024-04-30 23:22:36.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/seunglab.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2078 2024-01-19 23:49:14.000000 nglui-3.0.3/src/nglui/easyviewer/ev_base/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.207969 nglui-3.0.3/src/nglui/parser/
+-rw-r--r--   0 caseysm    (501) staff       (20)       20 2022-11-16 18:20:30.000000 nglui-3.0.3/src/nglui/parser/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    18969 2023-12-22 09:11:05.000000 nglui-3.0.3/src/nglui/parser/base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      434 2023-12-21 03:04:46.000000 nglui-3.0.3/src/nglui/parser/info.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.211586 nglui-3.0.3/src/nglui/statebuilder/
+-rw-r--r--   0 caseysm    (501) staff       (20)      351 2023-05-16 22:19:13.000000 nglui-3.0.3/src/nglui/statebuilder/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    30248 2024-02-27 02:56:31.000000 nglui-3.0.3/src/nglui/statebuilder/helpers.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    17089 2024-02-27 02:56:31.000000 nglui-3.0.3/src/nglui/statebuilder/layers.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    32498 2024-03-08 19:55:08.000000 nglui-3.0.3/src/nglui/statebuilder/mappers.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    10966 2024-01-19 23:50:18.000000 nglui-3.0.3/src/nglui/statebuilder/statebuilder.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2807 2023-12-29 01:45:09.000000 nglui-3.0.3/src/nglui/statebuilder/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.212902 nglui-3.0.3/src/nglui.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1782 2024-04-30 23:27:04.000000 nglui-3.0.3/src/nglui.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1839 2024-04-30 23:27:04.000000 nglui-3.0.3/src/nglui.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-30 23:27:04.000000 nglui-3.0.3/src/nglui.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      104 2024-04-30 23:27:04.000000 nglui-3.0.3/src/nglui.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        6 2024-04-30 23:27:04.000000 nglui-3.0.3/src/nglui.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      124 2022-11-16 18:20:30.000000 nglui-3.0.3/test_requirements.txt
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-30 23:27:04.212485 nglui-3.0.3/tests/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1423 2022-11-16 18:20:30.000000 nglui-3.0.3/tests/test_parser.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    12806 2024-04-30 23:22:54.000000 nglui-3.0.3/tests/test_statebuilder.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5117 2023-12-21 03:04:46.000000 nglui-3.0.3/tests/test_viewer.py
```

### Comparing `nglui-3.0.2/LICENSE.license` & `nglui-3.0.3/LICENSE.license`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/PKG-INFO` & `nglui-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nglui
-Version: 3.0.2
+Version: 3.0.3
 Summary: Framework for data-driven generation of neuroglancer states.
 Home-page: https://github.com/seung-lab/NeuroglancerAnnotationUI
 Author: Derrick Brittain, Casey Schneider-Mizell, Forrest Collman
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.license
 Requires-Dist: numpy>=1.11.0
```

### Comparing `nglui-3.0.2/README.md` & `nglui-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/examples/dash_example_data.h5` & `nglui-3.0.3/examples/dash_example_data.h5`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/examples/dash_with_statebuilder.py` & `nglui-3.0.3/examples/dash_with_statebuilder.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/examples/example_data.h5` & `nglui-3.0.3/examples/example_data.h5`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/examples/statebuilder_examples.ipynb` & `nglui-3.0.3/examples/statebuilder_examples.ipynb`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/setup.py` & `nglui-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/annotation_compatibility.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/annotation_compatibility.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/base.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/base.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/mainline.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/mainline.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/__init__.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/__init__.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/annotation.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/annotation.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/equivalence_map.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/equivalence_map.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/json_utils.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/json_utils.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/json_wrappers.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/json_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         def __setitem__(self, key, value):
             if self._readonly:
                 raise AttributeError
             if isinstance(key, slice):
                 values = [validator(x) for x in value]
                 self._data[key] = values
             else:
-                value = validator(x)
+                value = validator(value)
                 self._data[key] = value
 
         def __iter__(self):
             return iter(self._data)
 
         def append(self, x):
             if self._readonly:
```

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/random_token.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/random_token.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/skeleton.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/skeleton.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/trackable_state.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/trackable_state.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/url_state.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/url_state.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer_base.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer_base.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer_config_state.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer_config_state.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/nglite/viewer_state.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/nglite/viewer_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,15 @@
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
         super(PointAnnotationLayer, self).__init__(
             *args, type="pointAnnotation", **kwargs
         )
 
-    points = wrapped_property(
-        "points", typed_list(array_wrapper(np.float32, 3)))
+    points = wrapped_property("points", typed_list(array_wrapper(np.float32, 3)))
 
 
 def volume_source(x):
     if not isinstance(x, six.string_types):
         raise TypeError
     return text_type(x)
 
@@ -240,46 +239,44 @@
 
 
 @export
 class SegmentationLayer(Layer, _AnnotationLayerOptions):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
-        super(SegmentationLayer, self).__init__(
-            *args, type="segmentation", **kwargs)
+        super(SegmentationLayer, self).__init__(*args, type="segmentation", **kwargs)
 
     source = wrapped_property("source", optional(volume_source))
     mesh = wrapped_property("mesh", optional(text_type))
     skeletons = wrapped_property("skeletons", optional(text_type))
     segments = wrapped_property("segments", typed_set(np.uint64))
     equivalences = wrapped_property("equivalences", uint64_equivalence_map)
-    timestamp = wrapped_property('timestamp', optional(text_type))
+    timestamp = wrapped_property("timestamp", optional(text_type))
 
     hide_segment_zero = hideSegmentZero = wrapped_property(
         "hideSegmentZero", optional(bool, True)
     )
     selected_alpha = selectedAlpha = wrapped_property(
         "selectedAlpha", optional(float, 0.5)
     )
     not_selected_alpha = notSelectedAlpha = wrapped_property(
         "notSelectedAlpha", optional(float, 0)
     )
-    object_alpha = objectAlpha = wrapped_property(
-        "objectAlpha", optional(float, 1.0))
-    skeleton_shader = skeletonShader = wrapped_property(
-        "skeletonShader", text_type)
+    object_alpha = objectAlpha = wrapped_property("objectAlpha", optional(float, 1.0))
+    skeleton_shader = skeletonShader = wrapped_property("skeletonShader", text_type)
     color_seed = colorSeed = wrapped_property("colorSeed", optional(int, 0))
     cross_section_render_scale = crossSectionRenderScale = wrapped_property(
         "crossSectionRenderScale", optional(float, 1)
     )
     mesh_render_scale = meshRenderScale = wrapped_property(
         "meshRenderScale", optional(float, 10)
     )
     segment_colors = segmentColors = wrapped_property(
-        'segmentColors', optional(typed_string_map(str)))
+        "segmentColors", optional(typed_string_map(str))
+    )
 
     @staticmethod
     def interpolate(a, b, t):
         c = copy.deepcopy(a)
         for k in ["selected_alpha", "not_selected_alpha", "object_alpha"]:
             setattr(c, k, interpolate_linear(getattr(a, k), getattr(b, k), t))
         return c
@@ -320,16 +317,15 @@
         "vertexAttributeNames", optional(typed_list(optional(text_type)))
     )
 
 
 class AnnotationBase(JsonObjectWrapper):
     __slots__ = ()
 
-    id = wrapped_property("id", optional(text_type)
-                          )  # pylint: disable=invalid-name
+    id = wrapped_property("id", optional(text_type))  # pylint: disable=invalid-name
     type = wrapped_property("type", text_type)
     description = wrapped_property("description", optional(text_type))
     segments = wrapped_property("segments", optional(typed_list(np.uint64)))
     parent_id = wrapped_property("parentId", optional(text_type))
     tag_ids = wrapped_property("tagIds", optional(list))
 
 
@@ -368,28 +364,26 @@
 
 
 @export
 class EllipsoidAnnotation(AnnotationBase):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
-        super(EllipsoidAnnotation, self).__init__(
-            *args, type="ellipsoid", **kwargs)
+        super(EllipsoidAnnotation, self).__init__(*args, type="ellipsoid", **kwargs)
 
     center = wrapped_property("center", array_wrapper(np.float32, 3))
     radii = wrapped_property("radii", array_wrapper(np.float32, 3))
 
 
 @export
 class CollectionAnnotation(AnnotationBase):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
-        super(CollectionAnnotation, self).__init__(
-            *args, type="collection", **kwargs)
+        super(CollectionAnnotation, self).__init__(*args, type="collection", **kwargs)
 
     source = wrapped_property("source", array_wrapper(np.float32, 3))
     entries = wrapped_property("entries", array_wrapper(list))
     children_visible = wrapped_property("childrenVisible", array_wrapper(bool))
 
 
 annotation_types = {
@@ -405,16 +399,15 @@
 
 
 @export
 class AnnotationLayer(Layer, _AnnotationLayerOptions):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
-        super(AnnotationLayer, self).__init__(
-            *args, type="annotation", **kwargs)
+        super(AnnotationLayer, self).__init__(*args, type="annotation", **kwargs)
 
     source = wrapped_property("source", optional(volume_source))
     voxel_size = voxelSize = wrapped_property(
         "voxelSize", optional(array_wrapper(np.float32, 3))
     )
     annotations = wrapped_property("annotations", typed_list(annotation))
     linked_segmentation_layer = linkedSegmentationLayer = wrapped_property(
@@ -422,16 +415,19 @@
     )
     filter_by_segmentation = filterBySegmentation = wrapped_property(
         "filterBySegmentation", optional(bool, False)
     )
     brackets_show_segmentation = bracketShowSegmentation = wrapped_property(
         "bracketShortcutsShowSegmentation", optional(bool, True)
     )
-    selection_shows_segmentation = annotationSelectionShowsSegmentation = wrapped_property(
-        "annotationSelectionShowsSegmentation", optional(bool, True)
+    selection_shows_segmentation = annotationSelectionShowsSegmentation = (
+        wrapped_property("annotationSelectionShowsSegmentation", optional(bool, True))
+    )
+    annotation_tags = annotationTags = wrapped_property(
+        "annotationTags", optional(list)
     )
 
     @staticmethod
     def interpolate(a, b, t):
         del b
         del t
         return a
@@ -481,16 +477,15 @@
             if layer is None:
                 json_data = collections.OrderedDict()
             else:
                 json_data = layer
             layer = make_layer(json_data, _readonly=_readonly)
 
         object.__setattr__(self, "layer", layer)
-        super(ManagedLayer, self).__init__(
-            json_data, _readonly=_readonly, **kwargs)
+        super(ManagedLayer, self).__init__(json_data, _readonly=_readonly, **kwargs)
 
     visible = wrapped_property("visible", optional(bool))
 
     def __getattr__(self, key):
         return getattr(self.layer, key)
 
     def __setattr__(self, key, value):
@@ -498,15 +493,15 @@
             raise AttributeError
         if key in ["name", "visible", "layer"]:
             object.__setattr__(self, key, value)
         else:
             return setattr(self.layer, key, value)
 
     def __repr__(self):
-        return u"ManagedLayer(%s,%s)" % (
+        return "ManagedLayer(%s,%s)" % (
             encode_json_for_repr(self.name),
             encode_json_for_repr(self.to_json()),
         )
 
     def to_json(self):
         r = self.layer.to_json()
         r["name"] = self.name
@@ -632,40 +627,37 @@
     def interpolate(a, b, t):
         c = copy.deepcopy(a)
         for layer in c:
             index = b.index(layer.name)
             if index == -1:
                 continue
             other_layer = b[index]
-            if type(other_layer.layer) is not type(
-                layer.layer
-            ):  # pylint: disable=unidiomatic-typecheck
+            if type(other_layer.layer) is not type(layer.layer):  # pylint: disable=unidiomatic-typecheck
                 continue
             layer.layer = type(layer.layer).interpolate(
                 layer.layer, other_layer.layer, t
             )
         return c
 
 
 def navigation_link_type(x):
     x = six.text_type(x)
     x = x.lower()
-    if x not in [u"linked", u"unlinked", u"relative"]:
+    if x not in ["linked", "unlinked", "relative"]:
         raise ValueError("Invalid navigation link type: %r" % x)
     return x
 
 
 def make_linked_navigation_type(value_type, interpolate_function=None):
     if interpolate_function is None:
         interpolate_function = value_type.interpolate
 
     class LinkedType(JsonObjectWrapper):
         __slots__ = ()
-        link = wrapped_property("link", optional(
-            navigation_link_type, u"linked"))
+        link = wrapped_property("link", optional(navigation_link_type, "linked"))
         value = wrapped_property("value", optional(value_type))
 
         @staticmethod
         def interpolate(a, b, t):
             c = copy.deepcopy(a)
             c.link = a.link
             if a.link == b.link and a.link != "linked":
@@ -704,16 +696,15 @@
     zoom = wrapped_property("zoom", LinkedZoomFactor)
 
     @staticmethod
     def interpolate(a, b, t):
         c = copy.deepcopy(a)
         c.width = interpolate_linear(a.width, b.width, t)
         c.height = interpolate_linear(a.height, b.height, t)
-        c.position = LinkedSpatialPosition.interpolate(
-            a.position, b.position, t)
+        c.position = LinkedSpatialPosition.interpolate(a.position, b.position, t)
         c.orientation = LinkedOrientationState.interpolate(
             a.orientation, b.orientation, t
         )
         c.zoom = LinkedZoomFactor.interpolate(a.zoom, b.zoom, t)
         return c
 
 
@@ -728,25 +719,23 @@
         return c
 
 
 @export
 class DataPanelLayout(JsonObjectWrapper):
     __slots__ = ()
     type = wrapped_property("type", text_type)
-    cross_sections = crossSections = wrapped_property(
-        "crossSections", CrossSectionMap)
+    cross_sections = crossSections = wrapped_property("crossSections", CrossSectionMap)
     orthographic_projection = orthographicProjection = wrapped_property(
         "orthographicProjection", optional(bool, False)
     )
 
     def __init__(self, json_data=None, _readonly=False, **kwargs):
         if isinstance(json_data, six.string_types):
             json_data = {"type": six.text_type(json_data)}
-        super(DataPanelLayout, self).__init__(
-            json_data, _readonly=_readonly, **kwargs)
+        super(DataPanelLayout, self).__init__(json_data, _readonly=_readonly, **kwargs)
 
     def to_json(self):
         if len(self.cross_sections) == 0 and not self.orthographic_projection:
             return self.type
         return super(DataPanelLayout, self).to_json()
 
     @staticmethod
@@ -867,15 +856,15 @@
     def __init__(self, *args, **kwargs):
         super(LayerGroupViewer, self).__init__(*args, **kwargs)
         self.type = "viewer"
 
     def __repr__(self):
         j = self.to_json()
         j.pop("type", None)
-        return u"%s(%s)" % (type(self).__name__, encode_json_for_repr(j))
+        return "%s(%s)" % (type(self).__name__, encode_json_for_repr(j))
 
     @staticmethod
     def interpolate(a, b, t):
         c = copy.deepcopy(a)
         for k in (
             "layout",
             "position",
@@ -924,16 +913,15 @@
     navigation = wrapped_property("navigation", NavigationState)
     perspective_zoom = perspectiveZoom = wrapped_property(
         "perspectiveZoom", optional(float)
     )
     perspective_orientation = perspectiveOrientation = wrapped_property(
         "perspectiveOrientation", optional(array_wrapper(np.float32, 4))
     )
-    show_slices = showSlices = wrapped_property(
-        "showSlices", optional(bool, True))
+    show_slices = showSlices = wrapped_property("showSlices", optional(bool, True))
     show_axis_lines = showAxisLines = wrapped_property(
         "showAxisLines", optional(bool, True)
     )
     show_scale_bar = showScaleBar = wrapped_property(
         "showScaleBar", optional(bool, True)
     )
     show_default_annotations = showDefaultAnnotations = wrapped_property(
@@ -949,17 +937,17 @@
         "concurrentDownloads", optional(int)
     )
     layers = wrapped_property("layers", Layers)
     layout = wrapped_property("layout", layout_specification)
     cross_section_background_color = crossSectionBackgroundColor = wrapped_property(
         "crossSectionBackgroundColor", optional(text_type)
     )
-    perspective_view_background_color = (
-        perspectiveViewBackgroundColor
-    ) = wrapped_property("perspectiveViewBackgroundColor", optional(text_type))
+    perspective_view_background_color = perspectiveViewBackgroundColor = (
+        wrapped_property("perspectiveViewBackgroundColor", optional(text_type))
+    )
     selected_layer = selectedLayer = wrapped_property(
         "selectedLayer", SelectedLayerState
     )
     statistics = wrapped_property("statistics", StatisticsDisplayState)
 
     @property
     def position(self):
@@ -984,17 +972,15 @@
     @voxel_size.setter
     def voxel_size(self, v):
         self.navigation.voxel_size = v
 
     @staticmethod
     def interpolate(a, b, t):
         c = copy.deepcopy(a)
-        c.navigation = NavigationState.interpolate(
-            a.navigation, b.navigation, t)
-        c.perspective_zoom = interpolate_zoom(
-            a.perspective_zoom, b.perspective_zoom, t)
+        c.navigation = NavigationState.interpolate(a.navigation, b.navigation, t)
+        c.perspective_zoom = interpolate_zoom(a.perspective_zoom, b.perspective_zoom, t)
         c.perspective_orientation = quaternion_slerp(
             a.perspective_orientation, b.perspective_orientation, t
         )
         c.layers = Layers.interpolate(a.layers, b.layers, t)
         c.layout = interpolate_layout(a.layout, b.layout, t)
         return c
```

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/seunglab.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/seunglab.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from . import utils
 import re
 from . import nglite as neuroglancer
 from typing import Union, List, Dict, Tuple, Optional
 from numpy import issubdtype, integer, uint64, vstack
 from collections import OrderedDict
 
+
 class EasyViewerSeunglab(neuroglancer.UnsynchronizedViewer, EasyViewerBase):
     def __init__(self, **kwargs):
         super(neuroglancer.UnsynchronizedViewer, self).__init__(**kwargs)
         super(EasyViewerBase, self).__init__(**kwargs)
 
     def load_url(self, url) -> None:
         "Parse a neuroglancer state based on URL and load it into the state"
@@ -24,24 +25,20 @@
     def _AnnotationLayer(self, **kwargs):
         return neuroglancer.AnnotationLayer(
             **kwargs,
         )
 
     def _SegmentationLayer(self, source, **kwargs):
         if re.search(r"^graphene://", source) is not None:
-            source = utils.parse_graphene_header(source, 'seunglab')
-            return neuroglancer.ChunkedgraphSegmentationLayer(
-                source=source, **kwargs
-            )
+            source = utils.parse_graphene_header(source, "seunglab")
+            return neuroglancer.ChunkedgraphSegmentationLayer(source=source, **kwargs)
         elif re.search(r"^precomputed://", source) is not None:
-            return neuroglancer.SegmentationLayer(
-                source=source, **kwargs
-            )
+            return neuroglancer.SegmentationLayer(source=source, **kwargs)
         else:
-            raise ValueError('Source must be either graphene:// or precomputed://')
+            raise ValueError("Source must be either graphene:// or precomputed://")
 
     def set_resolution(self, resolution) -> None:
         with self.txn() as s:
             s.voxel_size = resolution
 
     def set_state_server(self, state_server) -> None:
         with self.txn() as s:
@@ -74,57 +71,55 @@
             s.layers.append(name=layer_name, layer=new_layer)
             if color is not None:
                 s.layers[layer_name].annotationColor = utils.parse_color(color)
 
         if tags is not None:
             self.add_annotation_tags(layer_name=layer_name, tags=tags)
 
-    def _convert_annotations(
-        self,
-        annotations: List) -> List:
+    def _convert_annotations(self, annotations: List) -> List:
         """Pass through annotations, currently defaulting to seung lab format already"""
         return annotations
 
     def add_annotation_tags(self, layer_name, tags):
         if layer_name not in self.layer_names:
             raise ValueError("Layer is not an annotation layer")
         tag_list = [
             OrderedDict({"id": tag_id + 1, "label": label})
             for tag_id, label in enumerate(tags)
         ]
         with self.txn() as s:
-            s.layers[layer_name]._json_data["annotationTags"] = tag_list
+            s.layers[layer_name].annotationTags = tag_list
 
     def as_url(
         self,
         prefix: Optional[str] = None,
         as_html: Optional[bool] = False,
         link_text: Optional[str] = "Neuroglancer Link",
     ) -> str:
-        prefix = utils.neuroglancer_url(prefix, 'seunglab') # 'seunglab' hard-coded because of file.
+        prefix = utils.neuroglancer_url(
+            prefix, "seunglab"
+        )  # 'seunglab' hard-coded because of file.
         ngl_url = neuroglancer.to_url(self.state, prefix=prefix)
         if as_html:
             return '<a href="{}" target="_blank">{}</a>'.format(ngl_url, link_text)
         else:
             return ngl_url
 
-
     def select_annotation(self, layer_name, anno_id):
         if layer_name in self.layer_names:
             with self.txn() as s:
                 s.layers[layer_name]._json_data["selectedAnnotation"] = id
         self.set_selected_layer(layer_name)
 
     def set_selected_layer(self, layer_name):
         with self.txn() as s:
             s.selectedLayer.layer = layer_name
-        
 
     def add_selected_objects(
-        self, 
+        self,
         segmentation_layer: str,
         oids: List[int],
         colors: Optional[Union[List, Dict]] = None,
     ) -> None:
         if issubdtype(type(oids), integer):
             oids = [oids]
 
@@ -138,15 +133,14 @@
         if colors is not None:
             if isinstance(colors, dict):
                 self.assign_colors(segmentation_layer, colors)
             elif len(colors) == len(oids):
                 seg_colors = {str(oid): clr for oid, clr in zip(oids, colors)}
                 self.assign_colors(segmentation_layer, seg_colors)
 
-
     def assign_colors(self, layer_name, seg_colors):
         """Assign colors to root ids in a segmentation layer
 
         Parameters
         ----------
         layer_name : str,
             Segmentation layer name
@@ -158,28 +152,26 @@
                 seg_colors = {
                     str(oid): utils.parse_color(k)
                     for oid, k in seg_colors.items()
                     if k is not None
                 }
                 s.layers[layer_name].segmentColors = seg_colors
 
- 
-
     def set_view_options(
         self,
         show_slices: Optional[bool] = None,
-        layout: Optional[str]=None,
+        layout: Optional[str] = None,
         show_axis_lines: Optional[bool] = None,
         show_scale_bar: Optional[bool] = None,
         orthographic: Optional[bool] = None,
         position: Optional[Tuple[float]] = None,
         zoom_image: Optional[float] = None,
         zoom_3d: Optional[float] = None,
         background_color: Optional[Tuple[float]] = None,
-    )->None:
+    ) -> None:
         """Set options relating to the neuroglancer view state. Only changes the values of the parameters provided.
 
         Parameters
         ----------
         show_slices : bool, optional
             Show slice cutout in the 3d view, by default None
         layout : str, optional
@@ -219,15 +211,15 @@
             if background_color is not None:
                 s.perspectiveViewBackgroundColor = utils.parse_color(background_color)
 
     def set_segmentation_view_options(
         self,
         layer_name: str,
         alpha_selected: Optional[float] = None,
-        alpha_3d: Optional[float] =None,
+        alpha_3d: Optional[float] = None,
         alpha_unselected: Optional[float] = None,
         **kwargs,
     ):
         if self.state.layers[layer_name].type not in SEGMENTATION_LAYER_TYPES:
             raise ValueError("Layer is not a segmentation layer")
         with self.txn() as s:
             l = s.layers[layer_name]
@@ -257,15 +249,14 @@
         with self.txn() as s:
             l = s.layers[layer_name]
             if timestamp is not None:
                 l.timestamp = int(timestamp)
             else:
                 l.timestamp = None
 
-
     def set_multicut_points(
         self,
         layer_name,
         seg_id,
         points_red,
         points_blue,
         supervoxels_red=None,
@@ -348,15 +339,15 @@
         return neuroglancer.point_annotation(
             point=point,
             id=id,
             description=description,
             linked_segmentation=linked_segmentation,
             tag_ids=tag_ids,
         )
-    
+
     @staticmethod
     def line_annotation(
         pointA,
         pointB,
         id=None,
         description=None,
         linked_segmentation=None,
@@ -404,15 +395,15 @@
             point_a=pointA,
             point_b=pointB,
             id=id,
             description=description,
             linked_segmentation=linked_segmentation,
             tag_ids=tag_ids,
         )
-    
+
     @staticmethod
     def group_annotations(
         annotations,
         source=None,
         id=None,
         return_all=True,
         gather_linked_segmentations=True,
@@ -424,8 +415,8 @@
             annotations,
             source=source,
             id=id,
             return_all=return_all,
             gather_linked_segmentations=gather_linked_segmentations,
             share_linked_segmentations=share_linked_segmentations,
             children_visible=children_visible,
-        )
+        )
```

### Comparing `nglui-3.0.2/src/nglui/easyviewer/ev_base/utils.py` & `nglui-3.0.3/src/nglui/easyviewer/ev_base/utils.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/parser/base.py` & `nglui-3.0.3/src/nglui/parser/base.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/statebuilder/helpers.py` & `nglui-3.0.3/src/nglui/statebuilder/helpers.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/statebuilder/layers.py` & `nglui-3.0.3/src/nglui/statebuilder/layers.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/statebuilder/mappers.py` & `nglui-3.0.3/src/nglui/statebuilder/mappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                     data = np.array(data)[0].reshape(1,-1)
         return data
 
     def _process_columns(self, data, skip_columns=[]):
         if self.split_positions is not None:
             split_positions = self.split_positions
         else:
-            is_split = np.bool([is_split(col, data) for col in self.data_columns])
+            is_split = np.bool([is_split_position(col, data) for col in self.data_columns])
             if np.all(~is_split):
                 split_positions = False
             if np.any(is_split):
                 split_positions = True
                 # Check that the split applies the the correct columns, in case multiple are used
                 for col, spl in zip(self.data_columns, is_split):
                     if spl:
```

### Comparing `nglui-3.0.2/src/nglui/statebuilder/statebuilder.py` & `nglui-3.0.3/src/nglui/statebuilder/statebuilder.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui/statebuilder/utils.py` & `nglui-3.0.3/src/nglui/statebuilder/utils.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/src/nglui.egg-info/PKG-INFO` & `nglui-3.0.3/src/nglui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nglui
-Version: 3.0.2
+Version: 3.0.3
 Summary: Framework for data-driven generation of neuroglancer states.
 Home-page: https://github.com/seung-lab/NeuroglancerAnnotationUI
 Author: Derrick Brittain, Casey Schneider-Mizell, Forrest Collman
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.license
 Requires-Dist: numpy>=1.11.0
```

### Comparing `nglui-3.0.2/src/nglui.egg-info/SOURCES.txt` & `nglui-3.0.3/src/nglui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/tests/test_parser.py` & `nglui-3.0.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `nglui-3.0.2/tests/test_statebuilder.py` & `nglui-3.0.3/tests/test_statebuilder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 import pytest
 import numpy as np
 from collections import OrderedDict
-from nglui.statebuilder import (ImageLayerConfig, SegmentationLayerConfig, AnnotationLayerConfig, StateBuilder, PointMapper, LineMapper, SphereMapper, SplitPointMapper, ChainedStateBuilder)
+from nglui.statebuilder import (
+    ImageLayerConfig,
+    SegmentationLayerConfig,
+    AnnotationLayerConfig,
+    StateBuilder,
+    PointMapper,
+    LineMapper,
+    SphereMapper,
+    SplitPointMapper,
+    ChainedStateBuilder,
+)
 
 
 @pytest.fixture
 def image_layer(img_path):
     img_layer = ImageLayerConfig(
         name="img",
         source=img_path,
@@ -22,15 +32,17 @@
 @pytest.fixture
 def anno_layer_basic():
     anno_layer = AnnotationLayerConfig(name="anno")
     return anno_layer
 
 
 def test_basic(image_layer, seg_layer_basic, anno_layer_basic):
-    sb = StateBuilder([image_layer, seg_layer_basic, anno_layer_basic], target_site='seunglab')
+    sb = StateBuilder(
+        [image_layer, seg_layer_basic, anno_layer_basic], target_site="seunglab"
+    )
     state_url = sb.render_state()
     assert state_url[:4] == "http"
 
     state = sb.render_state(return_as="html")
     # padding for link html plus text
     assert state.data == f'<a href="{state_url}" target="_blank">Neuroglancer Link</a>'
 
@@ -41,15 +53,17 @@
     assert type(state) is str
 
     state = sb.render_state(return_as="viewer")
     assert len(state.layer_names) == 3
 
 
 def test_basic_cave_explorer(image_layer, seg_layer_basic, anno_layer_basic):
-    sb = StateBuilder([image_layer, seg_layer_basic, anno_layer_basic], target_site='cave-explorer')
+    sb = StateBuilder(
+        [image_layer, seg_layer_basic, anno_layer_basic], target_site="cave-explorer"
+    )
     state_url = sb.render_state()
     assert state_url[:4] == "http"
 
     state = sb.render_state(return_as="html")
     # padding for link html plus text
     assert state.data == f'<a href="{state_url}" target="_blank">Neuroglancer Link</a>'
 
@@ -59,15 +73,15 @@
     state = sb.render_state(return_as="json")
     assert type(state) is str
 
     state = sb.render_state(return_as="viewer")
     assert len(state.layer_names) == 3
 
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_segmentation_layer(soma_df, seg_path_precomputed, target_site):
     seg_layer = SegmentationLayerConfig(
         name="seg",
         source=seg_path_precomputed,
         fixed_ids=[1000],
         selected_ids_column="pt_root_id",
     )
@@ -75,183 +89,193 @@
     sb = StateBuilder(layers=[seg_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
     print(state["layers"])
     assert 648518346349538466 in state["layers"][0]["segments"]
     assert 1000 in state["layers"][0]["segments"]
 
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_segmentation_layer_color(soma_df, seg_path_precomputed, target_site):
     soma_df["color"] = ["#fdd4c2", "#fca082", "#fb694a", "#e32f27", "#b11218"]
     seg_layer = SegmentationLayerConfig(
         name="seg",
         source=seg_path_precomputed,
         selected_ids_column="pt_root_id",
         color_column="color",
     )
-    sb = StateBuilder(layers=[seg_layer], target_site=target_site )
+    sb = StateBuilder(layers=[seg_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
-    assert state["layers"][0]['segmentColors']["648518346349538715"] == "#e32f27"
+    assert state["layers"][0]["segmentColors"]["648518346349538715"] == "#e32f27"
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_segmentation_layer_options(soma_df, seg_path_precomputed, target_site):
     segmentation_view_options = {"alpha_selected": 0.6, "alpha_3d": 0.2}
     seg_layer = SegmentationLayerConfig(
         seg_path_precomputed, view_kws=segmentation_view_options
     )
     sb = StateBuilder([seg_layer], target_site=target_site)
     state = sb.render_state(return_as="dict")
     assert state["layers"][0]["selectedAlpha"] == 0.6
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotations(pre_syn_df, target_site):
     points = PointMapper(point_column="pre_pt_position")
     points_2 = PointMapper(point_column="ctr_pt_position")
     anno_layer = AnnotationLayerConfig(name="annos", mapping_rules=[points, points_2])
 
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(pre_syn_df, return_as="dict")
     assert len(state["layers"][0]["annotations"]) == 10
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_array_annotations(target_site):
     data = np.array([[1, 2, 3], [3, 4, 5], [6, 5, 3], [1, 2, 1]])
     anno_layer = AnnotationLayerConfig(
         name="annos", array_data=True, mapping_rules=PointMapper()
     )
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(data, return_as="dict")
     assert len(state["layers"][0]["annotations"]) == 4
 
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotations_line(pre_syn_df, target_site):
     lines = LineMapper(
         point_column_a="pre_pt_position", point_column_b="post_pt_position"
     )
     anno_layer = AnnotationLayerConfig(name="annos", mapping_rules=lines)
 
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(pre_syn_df, return_as="dict")
     assert len(state["layers"][0]["annotations"]) == 5
 
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotations_sphere(soma_df, target_site):
     soma_df["radius"] = 5000
     spheres = SphereMapper(center_column="pt_position", radius_column="radius")
     anno_layer = AnnotationLayerConfig(name="annos", mapping_rules=spheres)
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
     assert len(state["layers"][0]["annotations"]) == 5
 
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotations_description(soma_df, target_site):
     soma_df["desc"] = ["a", "b", "c", "d", "e"]
     points = PointMapper("pt_position", description_column="desc")
     anno_layer = AnnotationLayerConfig(name="annos", mapping_rules=points)
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
     assert state["layers"][0]["annotations"][2]["description"] == "c"
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotations_linked(soma_df, soma_df_Int64, seg_path_precomputed, target_site):
     seg_layer = SegmentationLayerConfig(seg_path_precomputed, name="seg")
 
     points = PointMapper("pt_position", linked_segmentation_column="pt_root_id")
     anno_layer = AnnotationLayerConfig(
         mapping_rules=points, linked_segmentation_layer="seg"
     )
 
     sb = StateBuilder([seg_layer, anno_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
-    assert 648518346349538715 in np.squeeze(state["layers"][1]["annotations"][3]["segments"])
+    assert 648518346349538715 in np.squeeze(
+        state["layers"][1]["annotations"][3]["segments"]
+    )
 
     state = sb.render_state(soma_df_Int64, return_as="dict")
     assert len(np.squeeze(state["layers"][1]["annotations"][0]["segments"])) == 0
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotation_tags(soma_df, target_site):
     tag_list = ["i", "e"]
 
     points = PointMapper("pt_position", tag_column="cell_type")
     anno_layer = AnnotationLayerConfig(mapping_rules=points, tags=tag_list)
 
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
     if target_site == "seunglab":
         assert 2 in state["layers"][0]["annotations"][1]["tagIds"]
     else:
         # Not implemented yet in cave-explorer.
         assert True
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_annotation_groups(pre_syn_df, target_site):
     df = pre_syn_df.copy()
     df["group"] = [1, 1, np.nan, 2.0, 2.0]
     points = PointMapper("ctr_pt_position", group_column="group")
     anno_layer = AnnotationLayerConfig(mapping_rules=[points])
     sb = StateBuilder([anno_layer], target_site=target_site)
     state = sb.render_state(df, return_as="dict")
-    if target_site=="seunglab" or target_site is None:
+    if target_site == "seunglab" or target_site is None:
         assert len(state["layers"][0]["annotations"]) == 7
     else:
         assert len(state["layers"][0]["annotations"]) == 5
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_view_options(soma_df, image_layer, target_site):
     view_options = {
         "layout": "4panel",
         "show_slices": True,
         "zoom_3d": 500,
         "position": [71832, 54120, 1089],
     }
 
     sb = StateBuilder([image_layer], view_kws=view_options, target_site=target_site)
     state = sb.render_state(return_as="dict")
-    if target_site == 'seunglab':
+    if target_site == "seunglab":
         assert state["navigation"]["pose"]["position"]["voxelCoordinates"] == [
             71832,
             54120,
             1089,
         ]
-    elif target_site=='cave-explorer':
-        assert state['position'] == [
+    elif target_site == "cave-explorer":
+        assert state["position"] == [
             71832,
             54120,
             1089,
         ]
 
     points = PointMapper("pt_position", set_position=True)
     anno_layer = AnnotationLayerConfig(mapping_rules=points)
 
     sb = StateBuilder([image_layer, anno_layer], target_site=target_site)
     state = sb.render_state(soma_df, return_as="dict")
-    if target_site == 'seunglab':
+    if target_site == "seunglab":
         assert state["navigation"]["pose"]["position"]["voxelCoordinates"] == list(
             soma_df["pt_position"].loc[0]
         )
-    elif target_site=='cave-explorer':
-        assert state['position'] == list(
-            soma_df["pt_position"].loc[0]
-        )
+    elif target_site == "cave-explorer":
+        assert state["position"] == list(soma_df["pt_position"].loc[0])
+
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_chained(pre_syn_df, post_syn_df, image_layer, target_site):
     # First state builder
 
     postsyn_mapper = LineMapper(
         point_column_a="pre_pt_position", point_column_b="ctr_pt_position"
     )
     postsyn_annos = AnnotationLayerConfig(
         "post", color="#00CCCC", mapping_rules=postsyn_mapper
     )
 
-    postsyn_sb = StateBuilder(layers=[image_layer, postsyn_annos], target_site=target_site)
+    postsyn_sb = StateBuilder(
+        layers=[image_layer, postsyn_annos], target_site=target_site
+    )
 
     # Second state builder
     presyn_mapper = LineMapper(
         point_column_a="ctr_pt_position", point_column_b="post_pt_position"
     )
     presyn_annos = AnnotationLayerConfig(
         "pre", color="#CC1111", mapping_rules=presyn_mapper
@@ -260,51 +284,60 @@
     presyn_sb = StateBuilder(layers=[presyn_annos], target_site=target_site)
 
     # Chained state builder
     chained_sb = ChainedStateBuilder([postsyn_sb, presyn_sb])
     state = chained_sb.render_state([post_syn_df, pre_syn_df], return_as="dict")
     assert len(state["layers"]) == 3
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_mapping_sets(pre_syn_df, post_syn_df, image_layer, target_site):
     postsyn_mapper = LineMapper(
-        point_column_a="pre_pt_position", point_column_b="ctr_pt_position", mapping_set='post',
+        point_column_a="pre_pt_position",
+        point_column_b="ctr_pt_position",
+        mapping_set="post",
     )
     postsyn_annos = AnnotationLayerConfig(
         "post", color="#00CCCC", mapping_rules=postsyn_mapper
     )
 
     presyn_mapper = LineMapper(
-        point_column_a="ctr_pt_position", point_column_b="post_pt_position", mapping_set='pre'
+        point_column_a="ctr_pt_position",
+        point_column_b="post_pt_position",
+        mapping_set="pre",
     )
     presyn_annos = AnnotationLayerConfig(
         "pre", color="#CC1111", mapping_rules=presyn_mapper
     )
 
-    sb = StateBuilder([image_layer, postsyn_annos, presyn_annos], target_site=target_site)
-    state = sb.render_state({'pre': pre_syn_df, 'post': post_syn_df}, return_as='dict')
-    assert len(state['layers'][1]['annotations']) > 0
-    assert len(state['layers'][2]['annotations']) > 0
+    sb = StateBuilder(
+        [image_layer, postsyn_annos, presyn_annos], target_site=target_site
+    )
+    state = sb.render_state({"pre": pre_syn_df, "post": post_syn_df}, return_as="dict")
+    assert len(state["layers"][1]["annotations"]) > 0
+    assert len(state["layers"][2]["annotations"]) > 0
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_split_points(split_point_df, seg_path_graphene, target_site):
     split_mapper = SplitPointMapper(
         id_column="seg_id", point_column="pts", team_column="team", focus=True
     )
     seg = SegmentationLayerConfig(seg_path_graphene, split_point_map=split_mapper)
     sb = StateBuilder([seg], target_site=target_site)
     state = sb.render_state(split_point_df, return_as="dict")
     seg_layer = state["layers"][0]
     if target_site == "seunglab" or target_site is None:
         assert len(seg_layer["graphOperationMarker"][1]["annotations"]) == 2
     else:
         # Not implemented in cave-explorer
         assert True
 
-@pytest.mark.parametrize('target_site', [None, 'seunglab', 'cave-explorer'])
+
+@pytest.mark.parametrize("target_site", [None, "seunglab", "cave-explorer"])
 def test_timestamp(seg_path_graphene, target_site):
     ts = 12345
     seg = SegmentationLayerConfig(seg_path_graphene, timestamp=ts)
     sb = StateBuilder([seg], target_site=target_site)
     state = sb.render_state(return_as="dict")
     seg_layer = state["layers"][0]
     if target_site == "seunglab":
```

### Comparing `nglui-3.0.2/tests/test_viewer.py` & `nglui-3.0.3/tests/test_viewer.py`

 * *Files identical despite different names*

