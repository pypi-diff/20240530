# Comparing `tmp/parallax_app-0.37.8.tar.gz` & `tmp/parallax_app-0.37.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallax_app-0.37.8.tar", last modified: Tue May 28 22:58:48 2024, max compression
+gzip compressed data, was "parallax_app-0.37.9.tar", last modified: Thu May 30 01:10:07 2024, max compression
```

## Comparing `parallax_app-0.37.8.tar` & `parallax_app-0.37.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.394233 parallax_app-0.37.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.378233 parallax_app-0.37.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.378233 parallax_app-0.37.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-28 22:58:11.000000 parallax_app-0.37.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 22:58:11.000000 parallax_app-0.37.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-28 22:58:48.394233 parallax_app-0.37.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-28 22:58:11.000000 parallax_app-0.37.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.382233 parallax_app-0.37.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/ReadMe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/parallax.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 22:58:11.000000 parallax_app-0.37.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.382233 parallax_app-0.37.8/img/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-28 22:58:11.000000 parallax_app-0.37.8/img/target.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.386233 parallax_app-0.37.8/parallax/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/axis_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/calibration_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27905 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/coords_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/curr_bg_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/curr_prev_cmp_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/main_window_wip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/mask_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6058 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/no_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16261 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/probe_fine_tip_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/recording_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/reticle_detect_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/reticle_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/reticle_detection_coords_interests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13577 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/screen_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/stage_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/stage_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    39642 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/stage_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/user_setting_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-28 22:58:11.000000 parallax_app-0.37.8/parallax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/parallax_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 22:58:48.000000 parallax_app-0.37.8/parallax_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-28 22:58:11.000000 parallax_app-0.37.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 22:58:48.394233 parallax_app-0.37.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 22:58:11.000000 parallax_app-0.37.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-28 22:58:11.000000 parallax_app-0.37.8/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 22:58:11.000000 parallax_app-0.37.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-28 22:58:11.000000 parallax_app-0.37.8/tests/test_screen_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/ui/
--rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/ParallaxReadME.JPG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/ui/font/
--rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/font/FiraCode-VariableFont_wght.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/mainWindow.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/probe_calib.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:58:48.390233 parallax_app-0.37.8/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/check.png
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/recordingButton.png
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/recordingButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/sextant.png
--rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/snapshotButton_disabled.png
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/snapshotButton_green.png
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/snapshotButton_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/stop-sign.png
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/target.png
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/resources/x.png
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/reticle_calib.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/settingPopUpMenu.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-28 22:58:11.000000 parallax_app-0.37.8/ui/stage_info.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.234795 parallax_app-0.37.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.218795 parallax_app-0.37.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.218795 parallax_app-0.37.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 01:09:27.000000 parallax_app-0.37.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-30 01:09:27.000000 parallax_app-0.37.9/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-30 01:09:27.000000 parallax_app-0.37.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-30 01:09:27.000000 parallax_app-0.37.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 01:09:27.000000 parallax_app-0.37.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-30 01:10:07.234795 parallax_app-0.37.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-30 01:09:27.000000 parallax_app-0.37.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.222795 parallax_app-0.37.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/ReadMe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/parallax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 01:09:27.000000 parallax_app-0.37.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.222795 parallax_app-0.37.9/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-30 01:09:27.000000 parallax_app-0.37.9/img/target.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.226795 parallax_app-0.37.9/parallax/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/axis_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20382 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/calibration_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27905 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/coords_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/curr_bg_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/curr_prev_cmp_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32369 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/main_window_wip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/mask_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6058 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/no_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/probe_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/probe_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/probe_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/probe_fine_tip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/recording_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/reticle_detect_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23325 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/reticle_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/reticle_detection_coords_interests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13577 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/screen_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/stage_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/stage_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39644 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/stage_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/user_setting_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-30 01:09:27.000000 parallax_app-0.37.9/parallax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.230795 parallax_app-0.37.9/parallax_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-30 01:10:07.000000 parallax_app-0.37.9/parallax_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-30 01:10:07.000000 parallax_app-0.37.9/parallax_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:10:07.000000 parallax_app-0.37.9/parallax_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-30 01:10:07.000000 parallax_app-0.37.9/parallax_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 01:10:07.000000 parallax_app-0.37.9/parallax_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-30 01:09:27.000000 parallax_app-0.37.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:10:07.234795 parallax_app-0.37.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 01:09:27.000000 parallax_app-0.37.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.226795 parallax_app-0.37.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-30 01:09:27.000000 parallax_app-0.37.9/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 01:09:27.000000 parallax_app-0.37.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-30 01:09:27.000000 parallax_app-0.37.9/tests/test_screen_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.230795 parallax_app-0.37.9/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   192973 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/ParallaxReadME.JPG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.230795 parallax_app-0.37.9/ui/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   259308 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/font/FiraCode-VariableFont_wght.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/mainWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/probe_calib.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:10:07.230795 parallax_app-0.37.9/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/check.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/recordingButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/recordingButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/sextant.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/snapshotButton_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/snapshotButton_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/snapshotButton_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/stop-sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/target.png
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/resources/x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/reticle_calib.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/settingPopUpMenu.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-30 01:09:27.000000 parallax_app-0.37.9/ui/stage_info.ui
```

### Comparing `parallax_app-0.37.8/.github/workflows/ci.yml` & `parallax_app-0.37.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/.github/workflows/tag_and_publish.yml` & `parallax_app-0.37.9/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/LICENSE` & `parallax_app-0.37.9/LICENSE`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/PKG-INFO` & `parallax_app-0.37.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.8
+Version: 0.37.9
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parallax_app-0.37.8/README.md` & `parallax_app-0.37.9/README.md`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/docs/Makefile` & `parallax_app-0.37.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/docs/ReadMe.rst` & `parallax_app-0.37.9/docs/ReadMe.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/docs/conf.py` & `parallax_app-0.37.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/docs/make.bat` & `parallax_app-0.37.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/docs/parallax.rst` & `parallax_app-0.37.9/docs/parallax.rst`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/arrow-right.png` & `parallax_app-0.37.9/img/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/gear.png` & `parallax_app-0.37.9/img/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/recordingButton.png` & `parallax_app-0.37.9/img/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/sextant.png` & `parallax_app-0.37.9/img/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/snapshotButton_white.png` & `parallax_app-0.37.9/img/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/stop-sign.png` & `parallax_app-0.37.9/img/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/img/target.png` & `parallax_app-0.37.9/img/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/__main__.py` & `parallax_app-0.37.9/parallax/__main__.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/axis_filter.py` & `parallax_app-0.37.9/parallax/axis_filter.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/calibration_camera.py` & `parallax_app-0.37.9/parallax/calibration_camera.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/camera.py` & `parallax_app-0.37.9/parallax/camera.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/coords_transformation.py` & `parallax_app-0.37.9/parallax/coords_transformation.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/curr_bg_cmp_processor.py` & `parallax_app-0.37.9/parallax/curr_bg_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/curr_prev_cmp_processor.py` & `parallax_app-0.37.9/parallax/curr_prev_cmp_processor.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/main_window_wip.py` & `parallax_app-0.37.9/parallax/main_window_wip.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/mask_generator.py` & `parallax_app-0.37.9/parallax/mask_generator.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/model.py` & `parallax_app-0.37.9/parallax/model.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/no_filter.py` & `parallax_app-0.37.9/parallax/no_filter.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/probe_calibration.py` & `parallax_app-0.37.9/parallax/probe_calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import os
 
 import numpy as np
 import pandas as pd
 from PyQt5.QtCore import QObject, pyqtSignal
 from sklearn.linear_model import LinearRegression
-from coords_transformation import RotationTransformation
+from .coords_transformation import RotationTransformation
 
 # Set logger name
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 # Set the logging level for PyQt5.uic.uiparser/properties to WARNING, to ignore DEBUG messages
 logging.getLogger("PyQt5.uic.uiparser").setLevel(logging.WARNING)
 logging.getLogger("PyQt5.uic.properties").setLevel(logging.WARNING)
```

### Comparing `parallax_app-0.37.8/parallax/probe_detect_manager.py` & `parallax_app-0.37.9/parallax/probe_detect_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/probe_detector.py` & `parallax_app-0.37.9/parallax/probe_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/probe_fine_tip_detector.py` & `parallax_app-0.37.9/parallax/probe_fine_tip_detector.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/recording_manager.py` & `parallax_app-0.37.9/parallax/recording_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/reticle_detect_manager.py` & `parallax_app-0.37.9/parallax/reticle_detect_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/reticle_detection.py` & `parallax_app-0.37.9/parallax/reticle_detection.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/reticle_detection_coords_interests.py` & `parallax_app-0.37.9/parallax/reticle_detection_coords_interests.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/screen_widget.py` & `parallax_app-0.37.9/parallax/screen_widget.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/stage_listener.py` & `parallax_app-0.37.9/parallax/stage_listener.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/stage_ui.py` & `parallax_app-0.37.9/parallax/stage_ui.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/stage_widget.py` & `parallax_app-0.37.9/parallax/stage_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,15 @@
                 camA, camB = cam_names[i], cam_names[j]
                 coordsA, coordsB = img_coords[i], img_coords[j]
                 itmxA, itmxB = intrinsics[i], intrinsics[j]
                 
                 err, instance, retval, R_AB, T_AB, E_AB, F_AB = self.get_results_calibrate_stereo(
                     camA, coordsA, itmxA, camB, coordsB, itmxB
                 )
-                print(f"camA: {camA} camB: {camB} err: {err}")
+                print(f"camera pair: {camA}-{camB}, err: {err}")
                 if err < min_err:
                     self.calibrationStereo = instance
                     min_err = err
                     R_AB_best, T_AB_best, E_AB_best, F_AB_best = R_AB, T_AB, E_AB, F_AB
                     self.camA_best, self.camB_best = camA, camB
                     coordsA_best, coordsB_best = coordsA, coordsB
                     itmxA_best, itmxB_best = itmxA, itmxB
```

### Comparing `parallax_app-0.37.8/parallax/user_setting_manager.py` & `parallax_app-0.37.9/parallax/user_setting_manager.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax/utils.py` & `parallax_app-0.37.9/parallax/utils.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/parallax_app.egg-info/PKG-INFO` & `parallax_app-0.37.9/parallax_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallax-app
-Version: 0.37.8
+Version: 0.37.9
 Summary: GUI software for photogrammetry-assisted probe targeting in electrophysiology
 Author-email: Hanna Lee <hanna.lee@alleninstitute.org>
 License: MIT
 Keywords: parallax
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parallax_app-0.37.8/parallax_app.egg-info/SOURCES.txt` & `parallax_app-0.37.9/parallax_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/pyproject.toml` & `parallax_app-0.37.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/tests/test_screen_widget.py` & `parallax_app-0.37.9/tests/test_screen_widget.py`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/ParallaxReadME.JPG` & `parallax_app-0.37.9/ui/ParallaxReadME.JPG`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/font/FiraCode-VariableFont_wght.ttf` & `parallax_app-0.37.9/ui/font/FiraCode-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/mainWindow.ui` & `parallax_app-0.37.9/ui/mainWindow.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/probe_calib.ui` & `parallax_app-0.37.9/ui/probe_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/arrow-right.png` & `parallax_app-0.37.9/ui/resources/arrow-right.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/check.png` & `parallax_app-0.37.9/ui/resources/check.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/gear.png` & `parallax_app-0.37.9/ui/resources/gear.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/recordingButton.png` & `parallax_app-0.37.9/ui/resources/recordingButton.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/recordingButton_disabled.png` & `parallax_app-0.37.9/ui/resources/recordingButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/sextant.png` & `parallax_app-0.37.9/ui/resources/sextant.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/snapshotButton_disabled.png` & `parallax_app-0.37.9/ui/resources/snapshotButton_disabled.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/snapshotButton_green.png` & `parallax_app-0.37.9/ui/resources/snapshotButton_green.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/snapshotButton_white.png` & `parallax_app-0.37.9/ui/resources/snapshotButton_white.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/stop-sign.png` & `parallax_app-0.37.9/ui/resources/stop-sign.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/resources/target.png` & `parallax_app-0.37.9/ui/resources/target.png`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/reticle_calib.ui` & `parallax_app-0.37.9/ui/reticle_calib.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/settingPopUpMenu.ui` & `parallax_app-0.37.9/ui/settingPopUpMenu.ui`

 * *Files identical despite different names*

### Comparing `parallax_app-0.37.8/ui/stage_info.ui` & `parallax_app-0.37.9/ui/stage_info.ui`

 * *Files identical despite different names*

