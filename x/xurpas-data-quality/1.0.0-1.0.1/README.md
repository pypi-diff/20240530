# Comparing `tmp/xurpas_data_quality-1.0.0.tar.gz` & `tmp/xurpas_data_quality-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurpas_data_quality-1.0.0.tar", last modified: Thu May 30 03:37:20 2024, max compression
+gzip compressed data, was "xurpas_data_quality-1.0.1.tar", last modified: Thu May 30 06:25:54 2024, max compression
```

## Comparing `xurpas_data_quality-1.0.0.tar` & `xurpas_data_quality-1.0.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.611879 xurpas_data_quality-1.0.0/
--rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2375 2024-05-30 03:37:20.610867 xurpas_data_quality-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1745 2024-05-30 03:36:27.000000 xurpas_data_quality-1.0.0/README.md
--rw-rw-rw-   0        0        0      871 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 03:37:20.611879 xurpas_data_quality-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1166 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.207502 xurpas_data_quality-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.217753 xurpas_data_quality-1.0.0/src/xurpas_data_quality/
--rw-rw-rw-   0        0        0       59 2024-05-30 03:32:02.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.309576 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/
--rw-rw-rw-   0        0        0      306 2024-05-24 06:43:35.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.317790 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/
--rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/__init__.py
--rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/alerts.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.338537 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/
--rw-rw-rw-   0        0        0      105 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/__init__.py
--rw-rw-rw-   0        0        0      598 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/algorithms.py
--rw-rw-rw-   0        0        0      344 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/summary_algorithms.py
--rw-rw-rw-   0        0        0      117 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/correlations.py
--rw-rw-rw-   0        0        0     1370 2024-05-24 06:13:00.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/dataframe.py
--rw-rw-rw-   0        0        0     6756 2024-05-24 06:45:08.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe.py
--rw-rw-rw-   0        0        0     2697 2024-05-27 02:20:43.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe_new.py
--rw-rw-rw-   0        0        0     1736 2024-05-27 01:54:23.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describer.py
--rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/descriptions.py
--rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/pandas_dataframe.py
--rw-rw-rw-   0        0        0     1238 2024-05-27 02:20:32.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/series_describe.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.382861 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/
--rw-rw-rw-   0        0        0      150 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/__init__.py
--rw-rw-rw-   0        0        0     1681 2024-05-27 07:17:52.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py
--rw-rw-rw-   0        0        0      772 2024-05-27 01:44:26.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_date.py
--rw-rw-rw-   0        0        0      989 2024-05-27 01:57:05.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_generic.py
--rw-rw-rw-   0        0        0     3192 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py
--rw-rw-rw-   0        0        0      831 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/typeset.py
--rw-rw-rw-   0        0        0      570 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/utils.py
--rw-rw-rw-   0        0        0     3196 2024-05-27 01:05:35.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/data_report.py
--rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.439047 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/
--rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/__init__.py
--rw-rw-rw-   0        0        0      801 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/handler.py
--rw-rw-rw-   0        0        0     5621 2024-05-24 06:52:30.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.500994 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/
--rw-rw-rw-   0        0        0      181 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.529405 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/
--rw-rw-rw-   0        0        0        0 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-05-27 07:28:54.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py
--rw-rw-rw-   0        0        0      518 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py
--rw-rw-rw-   0        0        0     1571 2024-05-27 00:41:33.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py
--rw-rw-rw-   0        0        0     1158 2024-05-27 05:11:03.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_categorical.py
--rw-rw-rw-   0        0        0     1174 2024-05-27 00:26:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_date.py
--rw-rw-rw-   0        0        0      586 2024-05-27 00:26:47.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_generic.py
--rw-rw-rw-   0        0        0     1757 2024-05-27 00:46:11.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_numerical.py
--rw-rw-rw-   0        0        0     4608 2024-05-27 02:18:47.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/renderer.py
--rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/template_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.547690 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.551934 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/__init__.py
--rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/script.js
--rw-rw-rw-   0        0        0      684 2024-05-27 00:34:57.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/style.css
--rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/base.html
--rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/collapse.html
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.568879 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/__init__.py
--rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/box.html
--rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/column.html
--rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/default.html
--rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/sections.html
--rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/tabs.html
--rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/test.html
--rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/dropdown.html
--rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/navigation.html
--rw-rw-rw-   0        0        0      407 2024-05-27 02:32:44.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/plot.html
--rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/script.html
--rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/style.html
--rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/table.html
--rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/toggle.html
--rw-rw-rw-   0        0        0      510 2024-05-27 00:51:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/variable.html
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.588646 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/
--rw-rw-rw-   0        0        0       73 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/__init__.py
--rw-rw-rw-   0        0        0      817 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/empty_report.py
--rw-rw-rw-   0        0        0     8076 2024-05-24 06:38:14.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/report.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.607574 xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/
--rw-rw-rw-   0        0        0      170 2024-05-27 01:58:12.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/__init__.py
--rw-rw-rw-   0        0        0     2833 2024-05-27 02:28:35.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/plots.py
-drwxrwxrwx   0        0        0        0 2024-05-30 03:37:20.609575 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/
--rw-rw-rw-   0        0        0     2375 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3696 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-30 03:37:20.000000 xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.026063 xurpas_data_quality-1.0.1/
+-rw-rw-rw-   0        0        0      110 2024-05-07 06:47:23.000000 xurpas_data_quality-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2375 2024-05-30 06:25:54.024177 xurpas_data_quality-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2024-05-30 03:36:27.000000 xurpas_data_quality-1.0.1/README.md
+-rw-rw-rw-   0        0        0      871 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:25:54.026063 xurpas_data_quality-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.881181 xurpas_data_quality-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.904677 xurpas_data_quality-1.0.1/src/xurpas_data_quality/
+-rw-rw-rw-   0        0        0       59 2024-05-30 06:24:56.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.926531 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/
+-rw-rw-rw-   0        0        0      306 2024-05-24 06:43:35.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.928617 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/
+-rw-rw-rw-   0        0        0        0 2024-05-03 07:10:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/__init__.py
+-rw-rw-rw-   0        0        0      953 2024-05-06 00:02:03.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/alerts.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.931098 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/
+-rw-rw-rw-   0        0        0      105 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      598 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/algorithms.py
+-rw-rw-rw-   0        0        0      344 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/summary_algorithms.py
+-rw-rw-rw-   0        0        0      117 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/correlations.py
+-rw-rw-rw-   0        0        0     1370 2024-05-24 06:13:00.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/dataframe.py
+-rw-rw-rw-   0        0        0     6756 2024-05-24 06:45:08.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe.py
+-rw-rw-rw-   0        0        0     2697 2024-05-27 02:20:43.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe_new.py
+-rw-rw-rw-   0        0        0     2041 2024-05-30 06:23:27.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describer.py
+-rw-rw-rw-   0        0        0      224 2024-05-06 01:15:30.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/descriptions.py
+-rw-rw-rw-   0        0        0      350 2024-04-26 07:12:37.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/pandas_dataframe.py
+-rw-rw-rw-   0        0        0     1238 2024-05-30 06:09:15.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/series_describe.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.938825 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/
+-rw-rw-rw-   0        0        0      192 2024-05-30 06:14:41.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/__init__.py
+-rw-rw-rw-   0        0        0     1681 2024-05-27 07:17:52.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py
+-rw-rw-rw-   0        0        0      899 2024-05-30 06:23:13.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_date.py
+-rw-rw-rw-   0        0        0      989 2024-05-27 01:57:05.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_generic.py
+-rw-rw-rw-   0        0        0     3192 2024-05-30 06:22:46.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py
+-rw-rw-rw-   0        0        0      831 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/typeset.py
+-rw-rw-rw-   0        0        0      570 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/utils.py
+-rw-rw-rw-   0        0        0     3247 2024-05-30 06:02:21.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/data_report.py
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:51:12.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.945254 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/
+-rw-rw-rw-   0        0        0        0 2024-05-07 05:20:40.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/__init__.py
+-rw-rw-rw-   0        0        0      801 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/handler.py
+-rw-rw-rw-   0        0        0     5621 2024-05-24 06:52:30.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.962697 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/
+-rw-rw-rw-   0        0        0      181 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.973332 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/
+-rw-rw-rw-   0        0        0        0 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-05-27 07:28:54.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py
+-rw-rw-rw-   0        0        0      518 2024-05-24 01:53:29.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py
+-rw-rw-rw-   0        0        0     1571 2024-05-27 00:41:33.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py
+-rw-rw-rw-   0        0        0     1158 2024-05-27 05:11:03.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_categorical.py
+-rw-rw-rw-   0        0        0     1148 2024-05-30 06:23:58.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_date.py
+-rw-rw-rw-   0        0        0      586 2024-05-27 00:26:47.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_generic.py
+-rw-rw-rw-   0        0        0     1757 2024-05-27 00:46:11.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_numerical.py
+-rw-rw-rw-   0        0        0     4608 2024-05-27 02:18:47.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/renderer.py
+-rw-rw-rw-   0        0        0      569 2024-05-14 04:40:10.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/template_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.995211 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:20:52.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:53.995211 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:04.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/__init__.py
+-rw-rw-rw-   0        0        0      594 2024-05-06 06:23:01.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/script.js
+-rw-rw-rw-   0        0        0      684 2024-05-27 00:34:57.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/style.css
+-rw-rw-rw-   0        0        0      249 2024-05-06 06:04:16.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/base.html
+-rw-rw-rw-   0        0        0      106 2024-05-01 16:04:49.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/collapse.html
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.012350 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:21:13.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-04-30 07:01:56.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/box.html
+-rw-rw-rw-   0        0        0       78 2024-05-03 02:13:15.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/column.html
+-rw-rw-rw-   0        0        0      141 2024-05-03 02:44:57.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/default.html
+-rw-rw-rw-   0        0        0      340 2024-05-01 12:08:46.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/sections.html
+-rw-rw-rw-   0        0        0      835 2024-05-01 16:36:14.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/tabs.html
+-rw-rw-rw-   0        0        0       72 2024-05-06 02:07:52.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/test.html
+-rw-rw-rw-   0        0        0      277 2024-05-06 05:58:23.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/dropdown.html
+-rw-rw-rw-   0        0        0      268 2024-04-29 06:44:51.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/navigation.html
+-rw-rw-rw-   0        0        0      407 2024-05-27 02:32:44.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/plot.html
+-rw-rw-rw-   0        0        0      449 2024-05-06 06:03:50.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/script.html
+-rw-rw-rw-   0        0        0      267 2024-05-06 06:03:51.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/style.html
+-rw-rw-rw-   0        0        0      390 2024-05-06 00:49:14.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/table.html
+-rw-rw-rw-   0        0        0      300 2024-05-02 00:52:44.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/toggle.html
+-rw-rw-rw-   0        0        0      510 2024-05-27 00:51:20.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/variable.html
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.016525 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/
+-rw-rw-rw-   0        0        0       73 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/__init__.py
+-rw-rw-rw-   0        0        0      817 2024-05-24 06:08:48.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/empty_report.py
+-rw-rw-rw-   0        0        0     8076 2024-05-24 06:38:14.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/report.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.020032 xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/
+-rw-rw-rw-   0        0        0      170 2024-05-27 01:58:12.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/__init__.py
+-rw-rw-rw-   0        0        0     2833 2024-05-27 02:28:35.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/plots.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:25:54.020032 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/
+-rw-rw-rw-   0        0        0     2375 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3696 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 06:25:53.000000 xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/top_level.txt
```

### Comparing `xurpas_data_quality-1.0.0/PKG-INFO` & `xurpas_data_quality-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 1.0.0
+Version: 1.0.1
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `xurpas_data_quality-1.0.0/README.md` & `xurpas_data_quality-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/pyproject.toml` & `xurpas_data_quality-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/setup.py` & `xurpas_data_quality-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/alerts/alerts.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/algorithms/algorithms.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/dataframe.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describe_new.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describe_new.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/describer.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/describer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 from dataclasses import dataclass
-from visions import VisionsTypeset, Generic, Float, Integer, Categorical
+from visions import VisionsTypeset, Generic, Float, Integer, Categorical, Date, DateTime
 from typing import Dict, List, Callable
 
-from xurpas_data_quality.data.type_descriptions import describe_numeric, describe_categorical, describe_generic
+from xurpas_data_quality.data.type_descriptions import describe_numeric, describe_categorical, describe_generic, describe_date
 
 @dataclass
 class TableDescription:
     df: pd.DataFrame
     dataset_statistics: Dict
     variable_types: Dict
     variables: Dict
@@ -29,24 +29,30 @@
                      Integer : [
                          describe_generic,
                          describe_numeric
                      ],
                      Categorical : [
                          describe_generic,
                          describe_categorical
+                     ],
+                     Date: [
+                        describe_generic,
+                        describe_date
+                     ],
+                     DateTime: [
+                        describe_generic,
+                        describe_date
                      ]}):
-
         self.mapping = type_mapping
     
     def summarize(self, dtype, series, **kwargs)-> dict:
         # give the series and typeset
         # for every applicable type apply the function to the series
         # update the summary dict with the new
         summary = {}
-
         if dtype in self.mapping:
             for func in self.mapping[dtype]:
                 summary.update(func(series,summary))
         else:
             for func in self.mapping[Generic]:
                 summary.update(func(series,summary))
```

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/series_describe.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/series_describe.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_categorical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_date.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_date.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     Args:
         series: series to describe
         summary: dict containing the descriptions of the series so far
 
     Return:
         The series and the updated summary dict
         """
-    
-    min_date = series.min()
-    max_date = series.max()
-    mid_date = series.median()
-    time_range = (max_date - min_date).dt.days
-    histogram_counts = series.value_counts.to_dict()
-
-    return summary.update(
+    min_date = pd.to_datetime(series.min())
+    max_date = pd.to_datetime(series.max())
+    med_date = pd.to_datetime(min_date + (max_date-min_date))
+    time_range = (max_date - min_date).days
+    histogram_counts = series.value_counts().to_dict()
+    summary.update(
             {'min_date': min_date,
+             'median_date': med_date,
             'max_date': max_date,
-            'mid_date': mid_date,
-            'time_range': time_range})
+            'time_range': time_range,
+            'histogram_counts':histogram_counts})
+    
+    return summary
```

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_generic.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_generic.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/type_descriptions/describe_numeric.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/typeset.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/typeset.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data/utils.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data/utils.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/data_report.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/data_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
             raise ValueError("Please provide your data in 'file' or 'df' parameters!")
 
         self.render_empty = True if not validate_dataframe(df) else False # checks if dataframe is empty
         self.report_name = report_name
 
         if data_types is not None:
             self.data_types = check_dtypes(check_col_names(data_types, df.columns))
+        else:
+            self.data_types = None
 
         def has_extension(file_path:str):
             return os.path.splitext(file_path)[1] != '' 
         if has_extension(file_path):
             self.save_path = file_path
         else:
             self.save_path = '/'.join([file_path,"report.html"])
```

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/handler.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/handler.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_categorical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_date.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/bottom/render_bottom_numerical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_categorical.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_categorical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_date.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_date.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,23 @@
         "Distinct (%)": "{:0.2f}%".format(data['distinct_perc']),
         "Missing": data['missing'],
         "Missing (%)": "{:0.2f}%".format(data["missing_perc"]),
         "Memory size": "{} bytes".format(data['memory'])
     }
 
     table_2 = {
-        "Minimum": data['max_date'],
-        "Median": data['mid_date'],
+        "Minimum": data['min_date'],
         "Maximum": data['max_date'],
-        "Time range": data['time_range']
+        "Time range": f"{data['time_range']} days"
     }
 
     variable_body = {
         'table_1': HTMLTable(table_1),
         'table_2': HTMLTable(table_2),
-        'plot': HTMLPlot(plot=plot_to_base64(create_tiny_histogram(data['histogram'])))
+        #'plot': HTMLPlot(plot=plot_to_base64(create_tiny_histogram(data['histogram'])))
     }
 
     return HTMLVariable(
         name = name,
         type = data['type'],
         body = variable_body
     )
```

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_generic.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_generic.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/render_types/render_numerical.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/render_types/render_numerical.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/renderer.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/renderer.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/template_loader.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/template_loader.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/script.js` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/script.js`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/assets/style.css` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/assets/style.css`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/render/templates/containers/tabs.html` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/render/templates/containers/tabs.html`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/empty_report.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/empty_report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/report/report.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/report/report.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality/visuals/plots.py` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality/visuals/plots.py`

 * *Files identical despite different names*

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/PKG-INFO` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xurpas_data_quality
-Version: 1.0.0
+Version: 1.0.1
 Summary: XAIL Data quality
 Author: Neil Ortaliz
 Author-email: Neil Ortaliz <neil.ortaliz@xurpas.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `xurpas_data_quality-1.0.0/src/xurpas_data_quality.egg-info/SOURCES.txt` & `xurpas_data_quality-1.0.1/src/xurpas_data_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

