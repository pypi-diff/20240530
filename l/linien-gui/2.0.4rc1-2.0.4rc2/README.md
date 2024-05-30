# Comparing `tmp/linien_gui-2.0.4rc1.tar.gz` & `tmp/linien_gui-2.0.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien_gui-2.0.4rc1.tar", last modified: Thu May 30 05:57:22 2024, max compression
+gzip compressed data, was "linien_gui-2.0.4rc2.tar", last modified: Thu May 30 06:18:40 2024, max compression
```

## Comparing `linien_gui-2.0.4rc1.tar` & `linien_gui-2.0.4rc2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:57:22.038356 linien_gui-2.0.4rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 05:57:22.038356 linien_gui-2.0.4rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:57:22.030356 linien_gui-2.0.4rc1/linien_gui/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:57:22.038356 linien_gui-2.0.4rc1/linien_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/device_manager.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/general_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    26298 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/general_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/lock_status_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/locking_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/locking_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/logging_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/logging_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    42559 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/modulation_sweep_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/modulation_sweep_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/new_device_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/new_device_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/optimization_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/optimization_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/psd_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/psd_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/psd_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/psd_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/right_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/spectroscopy_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/spectroscopy_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/spin_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/sweep_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/view_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/ui/view_panel.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/linien_gui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:57:22.038356 linien_gui-2.0.4rc1/linien_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 05:57:22.000000 linien_gui-2.0.4rc1/linien_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-30 05:57:22.000000 linien_gui-2.0.4rc1/linien_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:57:22.000000 linien_gui-2.0.4rc1/linien_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 05:57:22.000000 linien_gui-2.0.4rc1/linien_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 05:57:22.000000 linien_gui-2.0.4rc1/linien_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 05:57:22.000000 linien_gui-2.0.4rc1/linien_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-30 05:57:02.000000 linien_gui-2.0.4rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:57:22.038356 linien_gui-2.0.4rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:18:40.894053 linien_gui-2.0.4rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 06:18:40.894053 linien_gui-2.0.4rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:18:40.886052 linien_gui-2.0.4rc2/linien_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   410598 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:18:40.894053 linien_gui-2.0.4rc2/linien_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/device_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9626 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/general_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26298 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/general_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/lock_status_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/locking_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39236 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/locking_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/logging_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/logging_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42559 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/modulation_sweep_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/modulation_sweep_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/new_device_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/new_device_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/optimization_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/optimization_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/psd_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/psd_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/psd_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/psd_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/right_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/spectroscopy_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/spectroscopy_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/spin_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/sweep_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/view_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/ui/view_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/linien_gui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:18:40.894053 linien_gui-2.0.4rc2/linien_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 06:18:40.000000 linien_gui-2.0.4rc2/linien_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-30 06:18:40.000000 linien_gui-2.0.4rc2/linien_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:18:40.000000 linien_gui-2.0.4rc2/linien_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 06:18:40.000000 linien_gui-2.0.4rc2/linien_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 06:18:40.000000 linien_gui-2.0.4rc2/linien_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 06:18:40.000000 linien_gui-2.0.4rc2/linien_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-30 06:18:21.000000 linien_gui-2.0.4rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:18:40.894053 linien_gui-2.0.4rc2/setup.cfg
```

### Comparing `linien_gui-2.0.4rc1/PKG-INFO` & `linien_gui-2.0.4rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 2.0.4rc1
+Version: 2.0.4rc2
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click<9.0,>=8.1.7
 Requires-Dist: pyqtgraph>=0.10.0
 Requires-Dist: PyQt5<6.0,>=5.12.0
 Requires-Dist: requests<3.0,>=2.31.0
 Requires-Dist: superqt>=0.2.3
-Requires-Dist: linien_client==2.0.4rc1
+Requires-Dist: linien_client==2.0.4rc2
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien_gui-2.0.4rc1/linien_gui/__init__.py` & `linien_gui-2.0.4rc2/linien_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/app.py` & `linien_gui-2.0.4rc2/linien_gui/app.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/config.py` & `linien_gui-2.0.4rc2/linien_gui/config.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/dialogs.py` & `linien_gui-2.0.4rc2/linien_gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/threads.py` & `linien_gui-2.0.4rc2/linien_gui/threads.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/device_manager.py` & `linien_gui-2.0.4rc2/linien_gui/ui/device_manager.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/device_manager.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/device_manager.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/general_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/general_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/general_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/general_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/lock_status_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/lock_status_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/locking_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/locking_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/locking_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/locking_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/logging_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/logging_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/logging_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/logging_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/main_window.py` & `linien_gui-2.0.4rc2/linien_gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/main_window.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/modulation_sweep_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/modulation_sweep_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/modulation_sweep_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/modulation_sweep_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/new_device_dialog.py` & `linien_gui-2.0.4rc2/linien_gui/ui/new_device_dialog.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/new_device_dialog.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/new_device_dialog.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/optimization_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/optimization_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/optimization_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/optimization_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/plot_widget.py` & `linien_gui-2.0.4rc2/linien_gui/ui/plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/psd_plot_widget.py` & `linien_gui-2.0.4rc2/linien_gui/ui/psd_plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/psd_table_widget.py` & `linien_gui-2.0.4rc2/linien_gui/ui/psd_table_widget.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/psd_window.py` & `linien_gui-2.0.4rc2/linien_gui/ui/psd_window.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/psd_window.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/psd_window.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/right_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/right_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/spectroscopy_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/spectroscopy_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/spectroscopy_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/spectroscopy_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/spin_box.py` & `linien_gui-2.0.4rc2/linien_gui/ui/spin_box.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/sweep_control.py` & `linien_gui-2.0.4rc2/linien_gui/ui/sweep_control.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/version_checker.py` & `linien_gui-2.0.4rc2/linien_gui/ui/version_checker.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/view_panel.py` & `linien_gui-2.0.4rc2/linien_gui/ui/view_panel.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/ui/view_panel.ui` & `linien_gui-2.0.4rc2/linien_gui/ui/view_panel.ui`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui/utils.py` & `linien_gui-2.0.4rc2/linien_gui/utils.py`

 * *Files identical despite different names*

### Comparing `linien_gui-2.0.4rc1/linien_gui.egg-info/PKG-INFO` & `linien_gui-2.0.4rc2/linien_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 2.0.4rc1
+Version: 2.0.4rc2
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click<9.0,>=8.1.7
 Requires-Dist: pyqtgraph>=0.10.0
 Requires-Dist: PyQt5<6.0,>=5.12.0
 Requires-Dist: requests<3.0,>=2.31.0
 Requires-Dist: superqt>=0.2.3
-Requires-Dist: linien_client==2.0.4rc1
+Requires-Dist: linien_client==2.0.4rc2
 
 Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.
```

### Comparing `linien_gui-2.0.4rc1/linien_gui.egg-info/SOURCES.txt` & `linien_gui-2.0.4rc2/linien_gui.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pyproject.toml
 linien_gui/__init__.py
 linien_gui/app.py
 linien_gui/config.py
 linien_gui/dialogs.py
+linien_gui/icon.ico
 linien_gui/threads.py
 linien_gui/utils.py
 linien_gui.egg-info/PKG-INFO
 linien_gui.egg-info/SOURCES.txt
 linien_gui.egg-info/dependency_links.txt
 linien_gui.egg-info/entry_points.txt
 linien_gui.egg-info/requires.txt
```

### Comparing `linien_gui-2.0.4rc1/pyproject.toml` & `linien_gui-2.0.4rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-gui"
-version = "2.0.4rc1"
+version = "2.0.4rc2"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
@@ -24,15 +24,15 @@
 requires-python = ">=3.8"
 dependencies = [
     "click>=8.1.7,<9.0",
     "pyqtgraph>=0.10.0",
     "PyQt5>=5.12.0,<6.0",
     "requests>=2.31.0,<3.0",
     "superqt>=0.2.3",
-    "linien_client==2.0.4rc1",
+    "linien_client==2.0.4rc2",
 ]
 
 [project.readme]
 text = "Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions."
 content-type = "text/markdown"
 
 [project.urls]
@@ -45,7 +45,8 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 namespaces = false
 
 [tool.setuptools.package-data]
 "linien_gui.ui" = ["*.ui"]
+linien_gui = ["icon.ico"]
```

