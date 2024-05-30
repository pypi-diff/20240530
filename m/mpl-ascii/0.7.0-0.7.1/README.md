# Comparing `tmp/mpl_ascii-0.7.0.tar.gz` & `tmp/mpl_ascii-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.7.0.tar", last modified: Sun May 26 14:11:05 2024, max compression
+gzip compressed data, was "mpl_ascii-0.7.1.tar", last modified: Thu May 30 17:22:51 2024, max compression
```

## Comparing `mpl_ascii-0.7.0.tar` & `mpl_ascii-0.7.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.957542 mpl_ascii-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.941542 mpl_ascii-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.941542 mpl_ascii-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-26 14:11:05.957542 mpl_ascii-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.953542 mpl_ascii-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_chart.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_label_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/bar_stacked.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/barh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/barh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/box_plot_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/box_plot_basic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/broken_line_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/broken_line_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/categorical_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/categorical_variables.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/cohere.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/color_bar_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/color_bar_scatter.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/csd_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/csd_demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/double_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/double_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/errorbars_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/hist_best_fit_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/hist_best_fit_line.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/hist_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/hist_simple.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/hist_simple_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/hist_simple_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/line_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/line_markers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/lines_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/lines_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/scatter_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/scatter_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/simple_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/simple_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/violin_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/examples/violin_plot.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.953542 mpl_ascii-0.7.0/mpl_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/ascii_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/ax.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/mpl_ascii/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.957542 mpl_ascii-0.7.0/mpl_ascii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-26 14:11:05.000000 mpl_ascii-0.7.0/mpl_ascii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-26 14:11:05.000000 mpl_ascii-0.7.0/mpl_ascii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:11:05.000000 mpl_ascii-0.7.0/mpl_ascii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 14:11:05.000000 mpl_ascii-0.7.0/mpl_ascii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 14:11:05.000000 mpl_ascii-0.7.0/mpl_ascii.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:11:05.957542 mpl_ascii-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:05.957542 mpl_ascii-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-26 14:11:01.000000 mpl_ascii-0.7.0/tests/test_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.440119 mpl_ascii-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.428119 mpl_ascii-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.428119 mpl_ascii-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-30 17:22:51.440119 mpl_ascii-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.436119 mpl_ascii-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_chart.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_label_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/bar_stacked.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/barh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/barh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/box_plot_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/box_plot_basic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/broken_line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/broken_line_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/categorical_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/categorical_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/cohere.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/color_bar_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/color_bar_scatter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/csd_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/csd_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/double_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/double_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/errorbars_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/hist_best_fit_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/hist_best_fit_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/hist_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/hist_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/hist_simple_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/hist_simple_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/line_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/line_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/lines_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/lines_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/scatter_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/scatter_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/simple_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/simple_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/violin_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/examples/violin_plot.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.440119 mpl_ascii-0.7.1/mpl_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/ascii_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/ax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/mpl_ascii/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.440119 mpl_ascii-0.7.1/mpl_ascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-30 17:22:51.000000 mpl_ascii-0.7.1/mpl_ascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-30 17:22:51.000000 mpl_ascii-0.7.1/mpl_ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:22:51.000000 mpl_ascii-0.7.1/mpl_ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 17:22:51.000000 mpl_ascii-0.7.1/mpl_ascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 17:22:51.000000 mpl_ascii-0.7.1/mpl_ascii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:22:51.440119 mpl_ascii-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:51.440119 mpl_ascii-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-30 17:22:46.000000 mpl_ascii-0.7.1/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.7.0/.github/workflows/python-package.yml` & `mpl_ascii-0.7.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/.gitignore` & `mpl_ascii-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/CHANGELOG.md` & `mpl_ascii-0.7.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
 ### Added
 
-- Add support for colour bars on scatter plots.
 - Add support for contour plots without colors.
 - Add support for text objects in plot.
 
+## [0.7.1] 2024-05-30
+
+### Fixed
+
+- Fix position of yaxis labels on colorbar axis so they are on the right side instead of the left side.
+
 ## [0.7.0] 2024-05-26
 
 ### Added
 
 - Add support for color bars on scatter plots
 
 ## [0.6.4] 2024-05-26
```

### Comparing `mpl_ascii-0.7.0/LICENSE` & `mpl_ascii-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/Makefile` & `mpl_ascii-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/PKG-INFO` & `mpl_ascii-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.7.0
+Version: 0.7.1
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.7.0/README.md` & `mpl_ascii-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_chart.py` & `mpl_ascii-0.7.1/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_chart.txt` & `mpl_ascii-0.7.1/examples/bar_chart.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_color.py` & `mpl_ascii-0.7.1/examples/bar_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_color.txt` & `mpl_ascii-0.7.1/examples/bar_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_1.py` & `mpl_ascii-0.7.1/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_1.txt` & `mpl_ascii-0.7.1/examples/bar_label_1.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_2.py` & `mpl_ascii-0.7.1/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_2.txt` & `mpl_ascii-0.7.1/examples/bar_label_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_3.py` & `mpl_ascii-0.7.1/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_3.txt` & `mpl_ascii-0.7.1/examples/bar_label_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_4.py` & `mpl_ascii-0.7.1/examples/bar_label_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_4.txt` & `mpl_ascii-0.7.1/examples/bar_label_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_5.py` & `mpl_ascii-0.7.1/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_label_5.txt` & `mpl_ascii-0.7.1/examples/bar_label_5.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_stacked.py` & `mpl_ascii-0.7.1/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/bar_stacked.txt` & `mpl_ascii-0.7.1/examples/bar_stacked.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/barh.py` & `mpl_ascii-0.7.1/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/barh.txt` & `mpl_ascii-0.7.1/examples/barh.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/box_plot_basic.py` & `mpl_ascii-0.7.1/examples/box_plot_basic.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/box_plot_basic.txt` & `mpl_ascii-0.7.1/examples/box_plot_basic.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/broken_line_plot.txt` & `mpl_ascii-0.7.1/examples/broken_line_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/categorical_variables.py` & `mpl_ascii-0.7.1/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/categorical_variables.txt` & `mpl_ascii-0.7.1/examples/categorical_variables.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/cohere.py` & `mpl_ascii-0.7.1/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/cohere.txt` & `mpl_ascii-0.7.1/examples/cohere.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/color_bar_scatter.py` & `mpl_ascii-0.7.1/examples/color_bar_scatter.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/color_bar_scatter.txt` & `mpl_ascii-0.7.1/examples/color_bar_scatter.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-                                                                               Scatter Plot with Color Bar                                                                     
-                                                                                                                                                                               
-      +------------------------------------------------------------------------------------------------------------------------------------------------------+     +----------+
-  100--                                                                                                                                                      |     |>>>>>>>>>>|
-      |                                                                                                                                                      |     |>>>>>>>>>>|
-      |                                                        ?  @                                                   ?                                      |     |>>>>>>>>>>|
-      |                                                                                                          $                                           |  14--<<<<<<<<<<|
-      |                                                        @    @   %                                      %                =            =               |     |<<<<<<<<<<|
-      |                                          @                              ?                         =            $                                     |     |<<<<<<<<<<|
-      |                                     <     <               %                                    @              < >                                    |     |<<<<<<<<<<|
-      |             %       @   @          =                                        ?                                                                        |     |<<<<<<<<<<|
-   80--                                                                                    $                                                                 |  12--??????????|
-      |                                                                     <                                                                                |     |??????????|
-      |                                                                        #                                                      #                      |     |??????????|
-      |                                       %                     <#                                                                                       |     |??????????|
-      |                                                 =                                        % #                                                         |     |??????????|
-      |                                                 $                                           #                                        @               |  10--==========|
-      |          @  ?                                                                                               $=                                       |     |==========|
-   60--                                          <                    ?                                                                                      |     |==========|
-      |       %         %                                                                                                   $                                |     |==========|
-      |          ?                                       <                         ?           $                                                             |     |==========|
-      |                     @                                                        %                                                                       |   8--$$$$$$$$$$|
-      |                                                               >                                                          <                           |     |$$$$$$$$$$|
-Y     |                                                          ?                                                                                           |I    |$$$$$$$$$$|
-      |                                                                                                                                                      |n    |$$$$$$$$$$|
-a  40--                                                                 $                                                     ?                              |t    |$$$$$$$$$$|
-x     |                                                                                                                                                      |e  6--@@@@@@@@@@|
-i     |                                @                                                                                                                     |n    |@@@@@@@@@@|
-s     |                                                                       ?                                                                              |s    |@@@@@@@@@@|
-      |           %    &                                             $                                                                                       |i    |@@@@@@@@@@|
-      |                                                                  <    ?     ?        <            @     <                                            |t    |@@@@@@@@@@|
-      |                                                                          %                                                                           |y    |@@@@@@@@@@|
-      |                          >                                                                                 &                                         |   4--&&&&&&&&&&|
-   20--                                                                               $                                     =                      $         |     |&&&&&&&&&&|
-      |                                                                         %           %                   =                      ?                     |     |&&&&&&&&&&|
-      |                >                                =                                   =         &                                                      |     |&&&&&&&&&&|
-      |             #                                                                                                                                        |     |&&&&&&&&&&|
-      |                                  &                                          $                                                            <   %       |   2--%%%%%%%%%%|
-      |                                                            &                 $                $               $           =                          |     |%%%%%%%%%%|
-      |                                     @                                                                                   ?                            |     |%%%%%%%%%%|
-    0--                                                                               $         @   &                                        #    =          |     |%%%%%%%%%%|
-      |                                                                                                                                                      |     |%%%%%%%%%%|
-      |                                                                                                                                                      |   0--%%%%%%%%%%|
-      +----|---------------------------|--------------------------|---------------------------|---------------------------|--------------------------|-------+     +----------+
-           0                          20                         40                          60                          80                        100                         
-                                                                                  X axis                                                                                       
+                                                                               Scatter Plot with Color Bar                                                                    
+                                                                                                                                                                              
+      +------------------------------------------------------------------------------------------------------------------------------------------------------++----------+    
+  100--                                                                                                                                                      ||>>>>>>>>>>|    
+      |                                                                                                                                                      ||>>>>>>>>>>|    
+      |                                                        ?  @                                                   ?                                      ||>>>>>>>>>>|    
+      |                                                                                                          $                                           ||<<<<<<<<<<--14 
+      |                                                        @    @   %                                      %                =            =               ||<<<<<<<<<<|    
+      |                                          @                              ?                         =            $                                     ||<<<<<<<<<<|    
+      |                                     <     <               %                                    @              < >                                    ||<<<<<<<<<<|    
+      |             %       @   @          =                                        ?                                                                        ||<<<<<<<<<<|    
+   80--                                                                                    $                                                                 ||??????????--12 
+      |                                                                     <                                                                                ||??????????|    
+      |                                                                        #                                                      #                      ||??????????|    
+      |                                       %                     <#                                                                                       ||??????????|    
+      |                                                 =                                        % #                                                         ||??????????|    
+      |                                                 $                                           #                                        @               ||==========--10 
+      |          @  ?                                                                                               $=                                       ||==========|    
+   60--                                          <                    ?                                                                                      ||==========|    
+      |       %         %                                                                                                   $                                ||==========|    
+      |          ?                                       <                         ?           $                                                             ||==========|    
+      |                     @                                                        %                                                                       ||$$$$$$$$$$--8  
+      |                                                               >                                                          <                           ||$$$$$$$$$$|    
+Y     |                                                          ?                                                                                           ||$$$$$$$$$$|   I
+      |                                                                                                                                                      ||$$$$$$$$$$|   n
+a  40--                                                                 $                                                     ?                              ||$$$$$$$$$$|   t
+x     |                                                                                                                                                      ||@@@@@@@@@@--6 e
+i     |                                @                                                                                                                     ||@@@@@@@@@@|   n
+s     |                                                                       ?                                                                              ||@@@@@@@@@@|   s
+      |           %    &                                             $                                                                                       ||@@@@@@@@@@|   i
+      |                                                                  <    ?     ?        <            @     <                                            ||@@@@@@@@@@|   t
+      |                                                                          %                                                                           ||@@@@@@@@@@|   y
+      |                          >                                                                                 &                                         ||&&&&&&&&&&--4  
+   20--                                                                               $                                     =                      $         ||&&&&&&&&&&|    
+      |                                                                         %           %                   =                      ?                     ||&&&&&&&&&&|    
+      |                >                                =                                   =         &                                                      ||&&&&&&&&&&|    
+      |             #                                                                                                                                        ||&&&&&&&&&&|    
+      |                                  &                                          $                                                            <   %       ||%%%%%%%%%%--2  
+      |                                                            &                 $                $               $           =                          ||%%%%%%%%%%|    
+      |                                     @                                                                                   ?                            ||%%%%%%%%%%|    
+    0--                                                                               $         @   &                                        #    =          ||%%%%%%%%%%|    
+      |                                                                                                                                                      ||%%%%%%%%%%|    
+      |                                                                                                                                                      ||%%%%%%%%%%--0  
+      +----|---------------------------|--------------------------|---------------------------|---------------------------|--------------------------|-------++----------+    
+           0                          20                         40                          60                          80                        100                        
+                                                                                  X axis
```

### Comparing `mpl_ascii-0.7.0/examples/csd_demo.py` & `mpl_ascii-0.7.1/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/csd_demo.txt` & `mpl_ascii-0.7.1/examples/csd_demo.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/double_plot.py` & `mpl_ascii-0.7.1/examples/double_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/double_plot.txt` & `mpl_ascii-0.7.1/examples/double_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars.txt` & `mpl_ascii-0.7.1/examples/errorbars.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars_2.py` & `mpl_ascii-0.7.1/examples/errorbars_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars_2.txt` & `mpl_ascii-0.7.1/examples/errorbars_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars_3.py` & `mpl_ascii-0.7.1/examples/errorbars_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars_3.txt` & `mpl_ascii-0.7.1/examples/errorbars_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars_4.py` & `mpl_ascii-0.7.1/examples/errorbars_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/errorbars_4.txt` & `mpl_ascii-0.7.1/examples/errorbars_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/hist_best_fit_line.py` & `mpl_ascii-0.7.1/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/hist_best_fit_line.txt` & `mpl_ascii-0.7.1/examples/hist_best_fit_line.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/hist_simple.py` & `mpl_ascii-0.7.1/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/hist_simple.txt` & `mpl_ascii-0.7.1/examples/hist_simple.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/hist_simple_colors.py` & `mpl_ascii-0.7.1/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/hist_simple_colors.txt` & `mpl_ascii-0.7.1/examples/hist_simple_colors.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/line_markers.py` & `mpl_ascii-0.7.1/examples/line_markers.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/line_markers.txt` & `mpl_ascii-0.7.1/examples/line_markers.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/lines_multi_color.py` & `mpl_ascii-0.7.1/examples/lines_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/lines_multi_color.txt` & `mpl_ascii-0.7.1/examples/lines_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/scatter_multi_color.py` & `mpl_ascii-0.7.1/examples/scatter_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/scatter_multi_color.txt` & `mpl_ascii-0.7.1/examples/scatter_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/simple_plot.py` & `mpl_ascii-0.7.1/examples/simple_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/simple_plot.txt` & `mpl_ascii-0.7.1/examples/simple_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/violin_plot.py` & `mpl_ascii-0.7.1/examples/violin_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/examples/violin_plot.txt` & `mpl_ascii-0.7.1/examples/violin_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/__init__.py` & `mpl_ascii-0.7.1/mpl_ascii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         fig_color_map = FigureColorMap(all_axes_plots)
 
         image_canvas = AsciiCanvas()
         for ax_plot in all_axes_plots:
             color_map = fig_color_map(ax_plot)
             ax_plot.draw_canvas(color_map)
             if ax_plot.is_colorbar():
-                image_canvas = image_canvas.update(ax_plot.color_canvas, (0, image_canvas.shape[1]))
+                image_canvas = image_canvas.update(ax_plot.color_canvas, (0, image_canvas.shape[1] + 3))
             else:
                 image_canvas = image_canvas.update(ax_plot.color_canvas, (image_canvas.shape[0], 0))
 
         return image_canvas
 
 
     def to_txt(self, sep="\n", tw=240, invert=False, threshold=200):
```

### Comparing `mpl_ascii-0.7.0/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.7.1/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/ax.py` & `mpl_ascii-0.7.1/mpl_ascii/ax.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/bar.py` & `mpl_ascii-0.7.1/mpl_ascii/bar.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/color_map.py` & `mpl_ascii-0.7.1/mpl_ascii/color_map.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/colorbar.py` & `mpl_ascii-0.7.1/mpl_ascii/colorbar.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/draw.py` & `mpl_ascii-0.7.1/mpl_ascii/draw.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/legend.py` & `mpl_ascii-0.7.1/mpl_ascii/legend.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/line.py` & `mpl_ascii-0.7.1/mpl_ascii/line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/overlay.py` & `mpl_ascii-0.7.1/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/poly.py` & `mpl_ascii-0.7.1/mpl_ascii/poly.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/scatter.py` & `mpl_ascii-0.7.1/mpl_ascii/scatter.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii/tools.py` & `mpl_ascii-0.7.1/mpl_ascii/tools.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.7.1/mpl_ascii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.7.0
+Version: 0.7.1
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
```

### Comparing `mpl_ascii-0.7.0/mpl_ascii.egg-info/SOURCES.txt` & `mpl_ascii-0.7.1/mpl_ascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/pyproject.toml` & `mpl_ascii-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.7.0/tests/test_overlay.py` & `mpl_ascii-0.7.1/tests/test_overlay.py`

 * *Files identical despite different names*

