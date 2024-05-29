# Comparing `tmp/bec_widgets-0.8.1.tar.gz` & `tmp/bec_widgets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_widgets-0.8.1.tar", last modified: Tue Aug 29 12:53:46 2023, max compression
+gzip compressed data, was "bec_widgets-0.9.0.tar", last modified: Tue Aug 29 14:49:48 2023, max compression
```

## Comparing `bec_widgets-0.8.1.tar` & `bec_widgets-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 12:53:46.031912 bec_widgets-0.8.1/
--rw-r--r--   0 root         (0) root         (0)     1511 2023-07-17 06:21:33.000000 bec_widgets-0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      490 2023-08-29 12:53:46.031912 bec_widgets-0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-11 13:21:08.000000 bec_widgets-0.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 12:53:46.029912 bec_widgets-0.8.1/bec_widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 16:17:29.000000 bec_widgets-0.8.1/bec_widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17154 2023-08-17 13:54:53.000000 bec_widgets-0.8.1/bec_widgets/basic_plot.py
--rw-r--r--   0 root         (0) root         (0)     8084 2023-08-29 12:49:18.000000 bec_widgets-0.8.1/bec_widgets/bec_dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     3963 2023-07-17 06:21:33.000000 bec_widgets-0.8.1/bec_widgets/config_plotter.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/ctrl_c.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/display_ui_file.py
--rw-r--r--   0 root         (0) root         (0)    14694 2023-08-17 14:03:34.000000 bec_widgets-0.8.1/bec_widgets/line_plot.py
--rw-r--r--   0 root         (0) root         (0)    13588 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/line_plot_legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 12:53:46.029912 bec_widgets-0.8.1/bec_widgets/qt_utils/
--rw-r--r--   0 root         (0) root         (0)       33 2023-08-11 12:44:10.000000 bec_widgets-0.8.1/bec_widgets/qt_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9327 2023-08-29 12:49:18.000000 bec_widgets-0.8.1/bec_widgets/qt_utils/crosshair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 12:53:46.030912 bec_widgets-0.8.1/bec_widgets/qtdesigner_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/qtdesigner_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/qtdesigner_plugins/scan2d_plot_plugin.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/qtdesigner_plugins/scan_plot_plugin.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-08-11 06:10:15.000000 bec_widgets-0.8.1/bec_widgets/scan2d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4058 2023-08-17 13:54:53.000000 bec_widgets-0.8.1/bec_widgets/scan_plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 12:53:46.030912 bec_widgets-0.8.1/bec_widgets/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-28 12:09:16.000000 bec_widgets-0.8.1/bec_widgets/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 12:53:46.031912 bec_widgets-0.8.1/bec_widgets.egg-info/
--rw-r--r--   0 root         (0) root         (0)      490 2023-08-29 12:53:45.000000 bec_widgets-0.8.1/bec_widgets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      760 2023-08-29 12:53:45.000000 bec_widgets-0.8.1/bec_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-29 12:53:45.000000 bec_widgets-0.8.1/bec_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-08-29 12:53:45.000000 bec_widgets-0.8.1/bec_widgets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-08-29 12:53:45.000000 bec_widgets-0.8.1/bec_widgets.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      521 2023-08-29 12:53:46.032912 bec_widgets-0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-08-29 12:53:44.000000 bec_widgets-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 14:49:48.009949 bec_widgets-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      490 2023-08-29 14:49:48.009949 bec_widgets-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 14:49:48.008948 bec_widgets-0.9.0/bec_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-29 14:49:38.000000 bec_widgets-0.9.0/bec_widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17154 2023-08-17 13:54:52.000000 bec_widgets-0.9.0/bec_widgets/basic_plot.py
+-rw-r--r--   0 root         (0) root         (0)     8084 2023-08-29 12:50:07.000000 bec_widgets-0.9.0/bec_widgets/bec_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3963 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/config_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/ctrl_c.py
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/display_ui_file.py
+-rw-r--r--   0 root         (0) root         (0)    14694 2023-08-28 12:08:21.000000 bec_widgets-0.9.0/bec_widgets/line_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    13588 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/line_plot_legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 14:49:48.008948 bec_widgets-0.9.0/bec_widgets/qt_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/qt_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9327 2023-08-29 12:50:07.000000 bec_widgets-0.9.0/bec_widgets/qt_utils/crosshair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 14:49:48.008948 bec_widgets-0.9.0/bec_widgets/qtdesigner_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-29 14:49:38.000000 bec_widgets-0.9.0/bec_widgets/qtdesigner_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/qtdesigner_plugins/scan2d_plot_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/qtdesigner_plugins/scan_plot_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-08-13 19:12:00.000000 bec_widgets-0.9.0/bec_widgets/scan2d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4058 2023-08-17 13:54:52.000000 bec_widgets-0.9.0/bec_widgets/scan_plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 14:49:48.008948 bec_widgets-0.9.0/bec_widgets/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-29 14:49:38.000000 bec_widgets-0.9.0/bec_widgets/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-29 14:49:48.009949 bec_widgets-0.9.0/bec_widgets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      490 2023-08-29 14:49:47.000000 bec_widgets-0.9.0/bec_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      760 2023-08-29 14:49:47.000000 bec_widgets-0.9.0/bec_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-29 14:49:47.000000 bec_widgets-0.9.0/bec_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-08-29 14:49:47.000000 bec_widgets-0.9.0/bec_widgets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-29 14:49:47.000000 bec_widgets-0.9.0/bec_widgets.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-08-29 14:49:48.010949 bec_widgets-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      287 2023-08-29 14:49:46.000000 bec_widgets-0.9.0/setup.py
```

### Comparing `bec_widgets-0.8.1/LICENSE` & `bec_widgets-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/basic_plot.py` & `bec_widgets-0.9.0/bec_widgets/basic_plot.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/bec_dispatcher.py` & `bec_widgets-0.9.0/bec_widgets/bec_dispatcher.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/config_plotter.py` & `bec_widgets-0.9.0/bec_widgets/config_plotter.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/ctrl_c.py` & `bec_widgets-0.9.0/bec_widgets/ctrl_c.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/display_ui_file.py` & `bec_widgets-0.9.0/bec_widgets/display_ui_file.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/line_plot.py` & `bec_widgets-0.9.0/bec_widgets/line_plot.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/line_plot_legacy.py` & `bec_widgets-0.9.0/bec_widgets/line_plot_legacy.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/qt_utils/crosshair.py` & `bec_widgets-0.9.0/bec_widgets/qt_utils/crosshair.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/qtdesigner_plugins/scan2d_plot_plugin.py` & `bec_widgets-0.9.0/bec_widgets/qtdesigner_plugins/scan2d_plot_plugin.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/qtdesigner_plugins/scan_plot_plugin.py` & `bec_widgets-0.9.0/bec_widgets/qtdesigner_plugins/scan_plot_plugin.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/scan2d_plot.py` & `bec_widgets-0.9.0/bec_widgets/scan2d_plot.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets/scan_plot.py` & `bec_widgets-0.9.0/bec_widgets/scan_plot.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/bec_widgets.egg-info/SOURCES.txt` & `bec_widgets-0.9.0/bec_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.8.1/setup.cfg` & `bec_widgets-0.9.0/setup.cfg`

 * *Files identical despite different names*

