# Comparing `tmp/xurpas_data_quality-0.0.8.tar.gz` & `tmp/xurpas_data_quality-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurpas_data_quality-0.0.8.tar", last modified: Thu May 16 07:16:35 2024, max compression
+gzip compressed data, was "xurpas_data_quality-1.0.0.tar", last modified: Thu May 30 03:37:20 2024, max compression
```

## Comparing `xurpas_data_quality-0.0.8.tar` & `xurpas_data_quality-1.0.0.tar`

### file list

```diff
@@ -1,68 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.106199 xurpas_data_quality-0.0.8/
--rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2079 2024-05-16 07:16:35.105199 xurpas_data_quality-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.8/README.md
--rw-rw-rw-   0        0        0      841 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 07:16:35.106199 xurpas_data_quality-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1147 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.029200 xurpas_data_quality-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.049625 xurpas_data_quality-0.0.8/src/xurpas_data_quality/
--rw-rw-rw-   0        0        0       59 2024-05-16 07:15:52.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.072697 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/
--rw-rw-rw-   0        0        0        0 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.073697 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/alerts/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/alerts/__init__.py
--rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/alerts/alerts.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.076225 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/algorithms/
--rw-rw-rw-   0        0        0       54 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/algorithms/__init__.py
--rw-rw-rw-   0        0        0      598 2024-05-16 06:58:18.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/algorithms/algorithms.py
--rw-rw-rw-   0        0        0     1282 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/dataframe.py
--rw-rw-rw-   0        0        0     6756 2024-05-16 06:35:50.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/describe.py
--rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/descriptions.py
--rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/pandas_dataframe.py
--rw-rw-rw-   0        0        0     2322 2024-05-16 07:07:06.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/data_report.py
--rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.080753 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/
--rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/__init__.py
--rw-rw-rw-   0        0        0      221 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/render.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.081860 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/render_types/
--rw-rw-rw-   0        0        0        0 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/render_types/render_numerical.py
--rw-rw-rw-   0        0        0      474 2024-05-15 01:55:13.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/render_variable.py
--rw-rw-rw-   0        0        0     4417 2024-05-14 05:05:46.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/renderer.py
--rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/template_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.091148 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.094248 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/assets/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/assets/__init__.py
--rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/assets/script.js
--rw-rw-rw-   0        0        0      600 2024-05-06 05:56:54.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/assets/style.css
--rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/base.html
--rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/collapse.html
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.099437 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/__init__.py
--rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/box.html
--rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/column.html
--rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/default.html
--rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/sections.html
--rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/tabs.html
--rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/test.html
--rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/dropdown.html
--rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/navigation.html
--rw-rw-rw-   0        0        0      279 2024-05-02 01:11:31.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/plot.html
--rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/script.html
--rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/style.html
--rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/table.html
--rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/toggle.html
--rw-rw-rw-   0        0        0      454 2024-05-06 05:58:21.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/variable.html
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.101916 xurpas_data_quality-0.0.8/src/xurpas_data_quality/report/
--rw-rw-rw-   0        0        0       30 2024-04-30 02:52:09.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/report/__init__.py
--rw-rw-rw-   0        0        0     7914 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/report/report.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.103947 xurpas_data_quality-0.0.8/src/xurpas_data_quality/visuals/
--rw-rw-rw-   0        0        0      141 2024-05-06 02:32:12.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/visuals/__init__.py
--rw-rw-rw-   0        0        0     2279 2024-05-16 06:42:23.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality/visuals/plots.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:16:35.105199 xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/
--rw-rw-rw-   0        0        0     2079 2024-05-16 07:16:34.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2024-05-16 07:16:35.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:16:34.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-16 07:16:34.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-16 07:16:34.000000 xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.611879 xurpas_data_quality-1.0.0/
+-rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2375 2024-05-30 03:37:20.610867 xurpas_data_quality-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2024-05-30 03:36:27.000000 xurpas_data_quality-1.0.0/README.md
+-rw-rw-rw-   0        0        0      871 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 03:37:20.611879 xurpas_data_quality-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.207502 xurpas_data_quality-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.217753 xurpas_data_quality-1.0.0/src/xurpas_data_quality/
+-rw-rw-rw-   0        0        0       59 2024-05-30 03:32:02.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.309576 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/
+-rw-rw-rw-   0        0        0      306 2024-05-24 06:43:35.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.317790 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/
+-rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/__init__.py
+-rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/alerts.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.338537 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/
+-rw-rw-rw-   0        0        0      105 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      598 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/algorithms.py
+-rw-rw-rw-   0        0        0      344 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/summary_algorithms.py
+-rw-rw-rw-   0        0        0      117 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/correlations.py
+-rw-rw-rw-   0        0        0     1370 2024-05-24 06:13:00.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/dataframe.py
+-rw-rw-rw-   0        0        0     6756 2024-05-24 06:45:08.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe.py
+-rw-rw-rw-   0        0        0     2697 2024-05-27 02:20:43.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe_new.py
+-rw-rw-rw-   0        0        0     1736 2024-05-27 01:54:23.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describer.py
+-rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/descriptions.py
+-rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/pandas_dataframe.py
+-rw-rw-rw-   0        0        0     1238 2024-05-27 02:20:32.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/series_describe.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.382861 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/
+-rw-rw-rw-   0        0        0      150 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/__init__.py
+-rw-rw-rw-   0        0        0     1681 2024-05-27 07:17:52.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py
+-rw-rw-rw-   0        0        0      772 2024-05-27 01:44:26.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_date.py
+-rw-rw-rw-   0        0        0      989 2024-05-27 01:57:05.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_generic.py
+-rw-rw-rw-   0        0        0     3192 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py
+-rw-rw-rw-   0        0        0      831 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/typeset.py
+-rw-rw-rw-   0        0        0      570 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/utils.py
+-rw-rw-rw-   0        0        0     3196 2024-05-27 01:05:35.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data_report.py
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.439047 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/__init__.py
+-rw-rw-rw-   0        0        0      801 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/handler.py
+-rw-rw-rw-   0        0        0     5621 2024-05-24 06:52:30.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.500994 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/
+-rw-rw-rw-   0        0        0      181 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.529405 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/
+-rw-rw-rw-   0        0        0        0 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-27 07:28:54.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py
+-rw-rw-rw-   0        0        0      518 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py
+-rw-rw-rw-   0        0        0     1571 2024-05-27 00:41:33.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py
+-rw-rw-rw-   0        0        0     1158 2024-05-27 05:11:03.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_categorical.py
+-rw-rw-rw-   0        0        0     1174 2024-05-27 00:26:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_date.py
+-rw-rw-rw-   0        0        0      586 2024-05-27 00:26:47.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_generic.py
+-rw-rw-rw-   0        0        0     1757 2024-05-27 00:46:11.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_numerical.py
+-rw-rw-rw-   0        0        0     4608 2024-05-27 02:18:47.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/renderer.py
+-rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/template_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.547690 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.551934 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/__init__.py
+-rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/script.js
+-rw-rw-rw-   0        0        0      684 2024-05-27 00:34:57.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/style.css
+-rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/base.html
+-rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/collapse.html
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.568879 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/box.html
+-rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/column.html
+-rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/default.html
+-rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/sections.html
+-rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/tabs.html
+-rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/test.html
+-rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/dropdown.html
+-rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/navigation.html
+-rw-rw-rw-   0        0        0      407 2024-05-27 02:32:44.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/plot.html
+-rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/script.html
+-rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/style.html
+-rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/table.html
+-rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/toggle.html
+-rw-rw-rw-   0        0        0      510 2024-05-27 00:51:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/variable.html
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.588646 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/
+-rw-rw-rw-   0        0        0       73 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/__init__.py
+-rw-rw-rw-   0        0        0      817 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/empty_report.py
+-rw-rw-rw-   0        0        0     8076 2024-05-24 06:38:14.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/report.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.607574 xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/
+-rw-rw-rw-   0        0        0      170 2024-05-27 01:58:12.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/__init__.py
+-rw-rw-rw-   0        0        0     2833 2024-05-27 02:28:35.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/plots.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.609575 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/
+-rw-rw-rw-   0        0        0     2375 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3696 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/top_level.txt
```

### Comparing `xurpas_data_quality-0.0.8/PKG-INFO` & `xurpas_data_quality-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 0.0.8
+Version: 1.0.0
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -13,31 +13,36 @@
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: jinja2
 Requires-Dist: openpyxl
 Requires-Dist: pyarrow
+Requires-Dist: pytest
+Requires-Dist: pytest
 
 # Xurpas Data Quality Report
 
 ## How to Use
 - Load the data to be analyzed (so far only csv files supported)
 - Import the DataReport class
 - Save the report to html File
 
 ## DataReport
 Creates and saves to file the data report.
 
 **Args**
 >**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist.  
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats.  
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Only supports .csv, .xlsx, .parquet, and .orc file formats.  
 >**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.  
->**report_name**: &emsp;Name of the report. Defaults to 'Data Report'.  
->**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
+>**report_name**: &emsp;&emsp;Name of the report. Defaults to 'Data Report'.  
+>**file_path**:&emsp;&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
+>**data_types**:&emsp;&emsp;&emsp; A dict containing the column names and column type to specify column data type.
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Data Types currently allowed "Categorical, Float, Integer, Date, String"
+
 
 **Returns**
 >HTML File of data quality Report
 
 #### Sample Usage using pandas DataFrame
 ```python
 import pandas as pd
@@ -54,7 +59,8 @@
 ```python
 from xurpas_data_quality import DataReport
 report = DataReport(file="manhour_utilization_summary.csv",
                     report_name="Manhour Utilization Summary", 
                     file_path="test_reports/test.html")
 report.to_file()
 ```
+
```

### Comparing `xurpas_data_quality-0.0.8/README.md` & `xurpas_data_quality-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 - Save the report to html File
 
 ## DataReport
 Creates and saves to file the data report.
 
 **Args**
 >**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist.  
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats.  
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Only supports .csv, .xlsx, .parquet, and .orc file formats.  
 >**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.  
->**report_name**: &emsp;Name of the report. Defaults to 'Data Report'.  
->**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
+>**report_name**: &emsp;&emsp;Name of the report. Defaults to 'Data Report'.  
+>**file_path**:&emsp;&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
+>**data_types**:&emsp;&emsp;&emsp; A dict containing the column names and column type to specify column data type.
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Data Types currently allowed "Categorical, Float, Integer, Date, String"
+
 
 **Returns**
 >HTML File of data quality Report
 
 #### Sample Usage using pandas DataFrame
 ```python
 import pandas as pd
@@ -33,8 +36,9 @@
 #### Sample Usage using filepath
 ```python
 from xurpas_data_quality import DataReport
 report = DataReport(file="manhour_utilization_summary.csv",
                     report_name="Manhour Utilization Summary", 
                     file_path="test_reports/test.html")
 report.to_file()
-```
+```
+
```

### Comparing `xurpas_data_quality-0.0.8/pyproject.toml` & `xurpas_data_quality-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 description='XAIL Data quality'
 dependencies = [
     "matplotlib",
     "pandas",
     "numpy",
     "jinja2",
     "openpyxl",
-    "pyarrow"
+    "pyarrow",
+    "pytest",
+    "pytest"
 ]
 requires-python = ">=3.10"
 authors = [
     {name="Neil Ortaliz", email="neil.ortaliz@xurpas.com"}
 ]
 readme = "README.md"
 license= {text = "MIT License"}
```

### Comparing `xurpas_data_quality-0.0.8/setup.py` & `xurpas_data_quality-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,10 +31,11 @@
     description='XAIL Data quality',
     install_requires=[
         'pandas',
         'numpy',
         'matplotlib',
         'jinja2',
         'openpyxl',
-        'pyarrow'
+        'pyarrow',
+        'pytest'
     ]
 )
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/alerts/alerts.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/algorithms/algorithms.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/dataframe.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/dataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import functools
+import warnings
 
 import pandas as pd
 
 
 def load_csv(file_path, **kwargs):
     return pd.read_csv(file_path)
 
@@ -11,27 +11,31 @@
     return pd.read_excel(file_path, **kwargs)
 
 def load_parquet(file_path, **kwargs):
     return pd.read_parquet(file_path, **kwargs)
 
 def load_orc(file_path, **kwargs):
     return pd.read_orc(file_path, **kwargs)
-    
 
-def validate_dataframe(func):
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        df = func(*args, **kwargs)
-        if df.empty:
-            raise ValueError("DataFrame is empty!")
-        else:
-            return df
-    return wrapper
+def validate_dataframe(df: pd.DataFrame) -> bool:
+    """
+    Checks if dataframe is empty.
+
+    Args
+        df: dataframe to validate
+
+    Returns
+        A boolean. False if the dataframe is empty, True if otherwise
+    """
+    if df.empty:
+        warnings.warn("DataFrame is empty! Generating Empty Report")
+        return False
+    else:
+        return True
 
-@validate_dataframe
 def load_dataframe(file_path: str) -> pd.DataFrame:
     load_methods = {
     '.csv': load_csv,
     '.xlsx': load_excel,
     '.parquet': load_parquet,
     '.orc': load_orc
     }
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/data/describe.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/data_report.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,75 @@
 import os
 import warnings
 from pathlib import Path
 
 import pandas as pd
 
-from xurpas_data_quality.data.dataframe import load_dataframe, validate_dataframe
-from xurpas_data_quality.data.describe import describe
-from xurpas_data_quality.report import get_report
+from xurpas_data_quality.report import get_report, get_empty_report
+from xurpas_data_quality.data import check_dtypes, describe, load_dataframe,validate_dataframe ,check_col_names
 
 
 class DataReport:
-    def __init__(self, file:str=None, df:pd.DataFrame=None, report_name:str="Data Report", file_path:str="report.html"):
+    def __init__(self, file:str=None, 
+                 df:pd.DataFrame=None, 
+                 report_name:str="Data Report", 
+                 file_path:str="report.html",
+                 data_types:dict=None):
         """
         Initializes the DataReport object
         Args
             file:        The path of the file you want to analyze. If empty, df parameter must exist.
                          Only supports .csv, .xlsx, .parquet, and .orc file formats
             df:          Pandas DataFrame object of data to be analyzed, If using df, file must be empty.
             report_name: Name of the report. Defaults to 'Data Report'
             file_path:   Path/ directory of where the report is to be saved
+            data_types:  A dictionary containing the column names and their corresponding data types.
+                         If empty, then the data types will be inferred.
         """
 
+        if file is not None and df is None:
+            self.df = df
+        elif file is None and df is not None:
+            self.df = df
+        elif file is not None and df is not None:
+            raise KeyError("Only 'file' or 'df' should be used one at a time!")
+        elif file is None and df is None:
+            raise ValueError("Please provide your data in 'file' or 'df' parameters!")
+
+        self.render_empty = True if not validate_dataframe(df) else False # checks if dataframe is empty
         self.report_name = report_name
 
+        if data_types is not None:
+            self.data_types = check_dtypes(check_col_names(data_types, df.columns))
+
         def has_extension(file_path:str):
             return os.path.splitext(file_path)[1] != '' 
         if has_extension(file_path):
             self.save_path = file_path
         else:
             self.save_path = '/'.join([file_path,"report.html"])
             warnings.warn("File name not provided, saving as {file_path}/report.html")
-            
-        if file is not None and df is None:
-            self.df = load_dataframe(df)
-        elif file is None and df is not None:
-            self.df = df
-        elif file is not None and df is not None:
-            raise KeyError("Only 'file' or 'df' should be used one at a time!")
-        elif file is None and df is None:
-            raise ValueError("Please provide your data in 'file' or 'df' parameters!")
-        
+
     def describe_dataframe(self):
-        self.description = describe(self.df)
+        self.description = describe(self.df, self.data_types)
 
-    def get_data_quality_report(self, name=None):
+    def get_data_quality_report(self, report_name=None):
         self.describe_dataframe()
-        report = get_report(self.description, name=name)
+        report = get_report(self.description, name=report_name)
+        return report.render()
+    
+    def _render_empty_report(self, name=None):
+        report = get_empty_report(self.df, name)
         return report.render()
     
     def to_file(self, report_name:str=None, file_name:str="report.html"):
         output = Path(self.save_path)
-        print(f"saving as {self.save_path}")
-        output.write_text(self.get_data_quality_report(self.report_name), encoding='utf-8')
-        print(f"saved!")
+
+        if self.render_empty:
+            print(f"saving empty report as {self.save_path}")
+            output.write_text(self._render_empty_report(self.report_name), encoding='utf-8')
+            print("saved!")
+
+        else:
+            print(f"saving as {self.save_path}")
+            output.write_text(self.get_data_quality_report(self.report_name), encoding='utf-8')
+            print(f"saved!")
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/renderer.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict,List
+from visions import VisionsBaseType
 
 from xurpas_data_quality.render.template_loader import template
 
 class BaseRenderer(ABC):
-    def __init__(self, content: Dict[str, Any], name: str = None, id:str=None, **kwargs):
+    def __init__(self, content: Dict[str, Any], name: str = None, id:str=None, type:VisionsBaseType=None,**kwargs):
         self.content = content
 
         if name is not None:
             self.content['name'] = name
         
         if id is not None:
             self.content['id'] = id
 
+        if type is not None:
+            self.type = type
+
     @property
     def name(self) -> str:
         return self.content.get('name', None)
     
     @property
     def id(self) -> str:
         return self.content.get('id', None)
@@ -48,21 +52,21 @@
         return template("collapse.html").render(**self.content)
     
 class HTMLVariable(BaseRenderer):
     def __init__(self, name, body, bottom=None, **kwargs):
         super().__init__({"variable_name":name, "variable_body": body, "variable_bottom": bottom}, **kwargs)
 
     def render(self):
-        return template("variable.html").render(name = self.content['variable_name'], bottom=self.content['variable_bottom'],**self.content['variable_body'])
+        return template("variable.html").render(name = self.content['variable_name'], bottom=self.content['variable_bottom'], content = self.content['variable_body'], type=self.type)
     
 class HTMLPlot(BaseRenderer):
     def __init__(self, plot:Any, type="small", **kwargs):
         super().__init__({"plot": plot}, **kwargs)
-        if type !="small" and type !="large":
-            raise ValueError("Plot type should be either 'small' or 'large'")
+        if type !="small" and type !="large" and type!='categorical':
+            raise ValueError("Plot type should be either 'small' or 'large' or 'categorical'")
         else:
             self.type=type
 
     def render(self):
         return template("plot.html").render(**self.content, type=self.type)
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/template_loader.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/template_loader.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/assets/script.js` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/script.js`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/assets/style.css` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/style.css`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     margin-left: -15px;
 }
 
 .variable{
     padding: 2em 2em;
     margin-right: -15px;
     margin-left: -15px;
+    border: 1px solid #e1e1e8;
+    border-right: hidden;
+    border-left:hidden;
 }
 .cont-padding{
     position: relative;
     min-height: 1px;
     padding-right: 15px;
     padding-left: 15px;
     float: left;
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/render/templates/containers/tabs.html` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/tabs.html`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/report/report.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from xurpas_data_quality.data.descriptions import TableDescription
 from xurpas_data_quality.render.renderer import HTMLBase, HTMLContainer, HTMLTable, HTMLVariable, HTMLPlot, HTMLToggle, HTMLCollapse, HTMLDropdown
 from xurpas_data_quality.visuals import plot_to_base64, create_tiny_histogram, create_histogram, create_distribution_plot, create_heatmap, create_interaction_plot
+from xurpas_data_quality.render.render import render_report
 
 from dataclasses import fields
 
 def get_detailed_variable_info(df, key:str, variables:dict):
     details = variables['details']
     bottom = [            
         HTMLContainer(
@@ -24,15 +25,14 @@
                 HTMLContainer(
                     type="column",
                     container_items=
                         HTMLTable(
                             data=details[0],
                             name="Descriptive Statistics"
                         )
-                    
                 )
             ]
         ),
         HTMLPlot(
             name="Histogram",
             type="large",
             id="histo",
@@ -124,15 +124,20 @@
                 name = column,
                 id = f"{column}-interaction-outer",
                 container_items = inner_tabs
             )
         )
     return outer_tabs
 
-def get_report(data: TableDescription, name:str=None)-> HTMLBase:
+def get_report(data: TableDescription, name:str=None):
+    report = render_report(data, name)
+    return report
+
+
+def get_report_old(data: TableDescription, name:str=None)-> HTMLBase:
     content = []
     overview_section = HTMLContainer(
         type="box",
         name="Overview",
         container_items = [
             HTMLContainer(
                 type="column",
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality/visuals/plots.py` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,50 @@
 import base64
 
 import pandas as pd
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
-from xurpas_data_quality.data.algorithms import sturges, rice,freedman_diaconis
+def create_tiny_histogram(histogram: tuple):
+    counts, bins = histogram
+    fig, ax = plt.subplots()
 
-def create_tiny_histogram(data: pd.Series):
-    data = data.dropna()
-    fig= plt.figure()
-    plt.hist(data, edgecolor="white")
-    plt.box(False)
+    bin_width = bins[1] - bins[0]
+    bin_centers = bins[:-1] + bin_width / 2
+    ax.bar(bin_centers, counts, width=bin_width)
+
+    ax.set(frame_on=False)
+    ax.set_yticks([])
 
     return fig
 
-def create_histogram(data: pd.Series):
-    data = data.dropna()
-    fig= plt.figure(figsize=(8,4))
-    plt.hist(data, edgecolor="white")
-    plt.box(False)
+def create_horizontal_histogram(value_counts: dict):
+    fig, ax = plt.subplots()
+    ax.barh(list(value_counts.keys()), list(value_counts.values()))
+    ax.set(frame_on=False)
+    ax.set_xticks([])
+
+    return fig
+
+def create_histogram(histogram: tuple):
+    counts, bins = histogram
+    fig, ax = plt.subplots(figsize=(12,4))
+
+    bin_width = bins[1] - bins[0]
+    bin_centers = bins[:-1] + bin_width / 2
+    ax.bar(bin_centers, counts, width=bin_width)
+
+    return fig
+
+def create_tiny_counts(series):
+    # Assuming 'df' is your DataFrame and 'Pclass' is your column
+
+    fig, ax = plt.subplots()
+    series.plot(kind='barh', ax=ax)
 
     return fig
 
 def create_heatmap(df: pd.DataFrame):
     # Create a figure and a set of subplots
     fig, ax = plt.subplots()
     plt.box(False)
```

### Comparing `xurpas_data_quality-0.0.8/src/xurpas_data_quality.egg-info/PKG-INFO` & `xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 0.0.8
+Version: 1.0.0
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -13,31 +13,36 @@
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: jinja2
 Requires-Dist: openpyxl
 Requires-Dist: pyarrow
+Requires-Dist: pytest
+Requires-Dist: pytest
 
 # Xurpas Data Quality Report
 
 ## How to Use
 - Load the data to be analyzed (so far only csv files supported)
 - Import the DataReport class
 - Save the report to html File
 
 ## DataReport
 Creates and saves to file the data report.
 
 **Args**
 >**file**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;The path of the file you want to analyze. If empty, df parameter must exist.  
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;Only supports .csv, .xlsx, .parquet, and .orc file formats.  
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Only supports .csv, .xlsx, .parquet, and .orc file formats.  
 >**df**:&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Pandas DataFrame object of data to be analyzed, If using df, file must be empty.  
->**report_name**: &emsp;Name of the report. Defaults to 'Data Report'.  
->**file_path**:&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
+>**report_name**: &emsp;&emsp;Name of the report. Defaults to 'Data Report'.  
+>**file_path**:&emsp;&emsp;&emsp;&emsp;&nbsp;Path/ directory of where the report is to be saved.  
+>**data_types**:&emsp;&emsp;&emsp; A dict containing the column names and column type to specify column data type.
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; Data Types currently allowed "Categorical, Float, Integer, Date, String"
+
 
 **Returns**
 >HTML File of data quality Report
 
 #### Sample Usage using pandas DataFrame
 ```python
 import pandas as pd
@@ -54,7 +59,8 @@
 ```python
 from xurpas_data_quality import DataReport
 report = DataReport(file="manhour_utilization_summary.csv",
                     report_name="Manhour Utilization Summary", 
                     file_path="test_reports/test.html")
 report.to_file()
 ```
+
```

