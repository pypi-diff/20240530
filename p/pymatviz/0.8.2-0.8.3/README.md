# Comparing `tmp/pymatviz-0.8.2.tar.gz` & `tmp/pymatviz-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatviz-0.8.2.tar", last modified: Sat May 11 16:39:51 2024, max compression
+gzip compressed data, was "pymatviz-0.8.3.tar", last modified: Thu May 30 17:20:56 2024, max compression
```

## Comparing `pymatviz-0.8.2.tar` & `pymatviz-0.8.3.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.610679 pymatviz-0.8.2/
--rw-r--r--   0 janosh     (501) wheel        (0)    20665 2024-05-11 16:39:51.610417 pymatviz-0.8.2/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.8.2/license
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.602909 pymatviz-0.8.2/pymatviz/
--rw-r--r--   0 janosh     (501) wheel        (0)     3791 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/__init__.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3874 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3181 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.8.2/pymatviz/elements.csv
--rw-r--r--   0 janosh     (501) wheel        (0)     4251 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/enums.py
--rw-r--r--   0 janosh     (501) wheel        (0)    14974 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)    16227 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/io.py
--rw-r--r--   0 janosh     (501) wheel        (0)    13297 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)    20943 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/phonons.py
--rw-r--r--   0 janosh     (501) wheel        (0)    16587 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/powerups.py
--rw-r--r--   0 janosh     (501) wheel        (0)    71398 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2967 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2220 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)    17490 2024-05-10 13:08:51.000000 pymatviz-0.8.2/pymatviz/structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2981 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)    10628 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)    17211 2024-05-10 13:08:51.000000 pymatviz-0.8.2/pymatviz/utils.py
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.609516 pymatviz-0.8.2/pymatviz.egg-info/
--rw-r--r--   0 janosh     (501) wheel        (0)    20665 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)      908 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/SOURCES.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        1 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/dependency_links.txt
--rw-r--r--   0 janosh     (501) wheel        (0)      327 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/requires.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        9 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/top_level.txt
--rw-r--r--   0 janosh     (501) wheel        (0)     3332 2024-05-11 16:29:23.000000 pymatviz-0.8.2/pyproject.toml
--rw-r--r--   0 janosh     (501) wheel        (0)    17586 2024-05-11 16:29:46.000000 pymatviz-0.8.2/readme.md
--rw-r--r--   0 janosh     (501) wheel        (0)       38 2024-05-11 16:39:51.610720 pymatviz-0.8.2/setup.cfg
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.609114 pymatviz-0.8.2/tests/
--rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.8.2/tests/test_correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.8.2/tests/test_cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2642 2024-03-17 14:44:01.000000 pymatviz-0.8.2/tests/test_histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)      859 2024-05-11 16:28:36.000000 pymatviz-0.8.2/tests/test_init.py
--rw-r--r--   0 janosh     (501) wheel        (0)     8672 2024-05-06 00:10:06.000000 pymatviz-0.8.2/tests/test_io.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3049 2023-12-26 18:26:44.000000 pymatviz-0.8.2/tests/test_parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)     7585 2024-03-31 18:45:17.000000 pymatviz-0.8.2/tests/test_phonons.py
--rw-r--r--   0 janosh     (501) wheel        (0)    11203 2024-03-22 14:01:49.000000 pymatviz-0.8.2/tests/test_powerups.py
--rw-r--r--   0 janosh     (501) wheel        (0)    20065 2024-05-11 16:28:36.000000 pymatviz-0.8.2/tests/test_ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)      457 2024-05-02 15:22:30.000000 pymatviz-0.8.2/tests/test_readme.py
--rw-r--r--   0 janosh     (501) wheel        (0)     1378 2023-05-24 19:03:32.000000 pymatviz-0.8.2/tests/test_relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)      599 2023-12-26 10:57:39.000000 pymatviz-0.8.2/tests/test_sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2677 2024-05-10 13:08:51.000000 pymatviz-0.8.2/tests/test_structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)      999 2023-05-19 14:05:47.000000 pymatviz-0.8.2/tests/test_sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2383 2023-12-26 10:56:52.000000 pymatviz-0.8.2/tests/test_uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)    12483 2024-05-05 13:32:56.000000 pymatviz-0.8.2/tests/test_utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-30 17:20:56.398566 pymatviz-0.8.3/
+-rw-r--r--   0 janosh     (501) wheel        (0)    21494 2024-05-30 17:20:56.398323 pymatviz-0.8.3/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.8.3/license
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-30 17:20:56.391472 pymatviz-0.8.3/pymatviz/
+-rw-r--r--   0 janosh     (501) wheel        (0)     3933 2024-05-17 22:30:30.000000 pymatviz-0.8.3/pymatviz/__init__.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     8555 2024-05-30 12:25:27.000000 pymatviz-0.8.3/pymatviz/_preprocess_data.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3881 2024-05-16 13:57:26.000000 pymatviz-0.8.3/pymatviz/correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3181 2024-05-04 22:48:32.000000 pymatviz-0.8.3/pymatviz/cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.8.3/pymatviz/elements.csv
+-rw-r--r--   0 janosh     (501) wheel        (0)     6027 2024-05-19 16:02:31.000000 pymatviz-0.8.3/pymatviz/enums.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    15331 2024-05-19 16:02:31.000000 pymatviz-0.8.3/pymatviz/histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    16264 2024-05-27 08:44:03.000000 pymatviz-0.8.3/pymatviz/io.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    13325 2024-05-16 13:57:26.000000 pymatviz-0.8.3/pymatviz/parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    21346 2024-05-30 12:22:35.000000 pymatviz-0.8.3/pymatviz/phonons.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    16937 2024-05-30 12:22:35.000000 pymatviz-0.8.3/pymatviz/powerups.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    72518 2024-05-30 17:01:29.000000 pymatviz-0.8.3/pymatviz/ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2967 2024-05-04 22:48:32.000000 pymatviz-0.8.3/pymatviz/relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2227 2024-05-16 13:57:26.000000 pymatviz-0.8.3/pymatviz/sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    17552 2024-05-23 16:55:13.000000 pymatviz-0.8.3/pymatviz/structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2988 2024-05-16 13:57:26.000000 pymatviz-0.8.3/pymatviz/sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    10642 2024-05-16 13:57:26.000000 pymatviz-0.8.3/pymatviz/uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    17295 2024-05-27 08:44:03.000000 pymatviz-0.8.3/pymatviz/utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-30 17:20:56.397477 pymatviz-0.8.3/pymatviz.egg-info/
+-rw-r--r--   0 janosh     (501) wheel        (0)    21494 2024-05-30 17:20:56.000000 pymatviz-0.8.3/pymatviz.egg-info/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)      987 2024-05-30 17:20:56.000000 pymatviz-0.8.3/pymatviz.egg-info/SOURCES.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        1 2024-05-30 17:20:56.000000 pymatviz-0.8.3/pymatviz.egg-info/dependency_links.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)      327 2024-05-30 17:20:56.000000 pymatviz-0.8.3/pymatviz.egg-info/requires.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        9 2024-05-30 17:20:56.000000 pymatviz-0.8.3/pymatviz.egg-info/top_level.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)     3479 2024-05-30 17:01:36.000000 pymatviz-0.8.3/pyproject.toml
+-rw-r--r--   0 janosh     (501) wheel        (0)    18415 2024-05-14 20:47:56.000000 pymatviz-0.8.3/readme.md
+-rw-r--r--   0 janosh     (501) wheel        (0)       38 2024-05-30 17:20:56.398608 pymatviz-0.8.3/setup.cfg
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-30 17:20:56.397161 pymatviz-0.8.3/tests/
+-rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.8.3/tests/test_correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.8.3/tests/test_cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      363 2024-05-16 13:57:26.000000 pymatviz-0.8.3/tests/test_enums.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3070 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      859 2024-05-11 16:28:36.000000 pymatviz-0.8.3/tests/test_init.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     8751 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_io.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3049 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     8542 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_phonons.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    12196 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_powerups.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     9879 2024-05-30 12:25:27.000000 pymatviz-0.8.3/tests/test_preprocess_data.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    20131 2024-05-30 17:01:29.000000 pymatviz-0.8.3/tests/test_ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      457 2024-05-02 15:22:30.000000 pymatviz-0.8.3/tests/test_readme.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     1378 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      629 2024-05-17 22:30:30.000000 pymatviz-0.8.3/tests/test_sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3407 2024-05-27 08:45:42.000000 pymatviz-0.8.3/tests/test_structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      999 2023-05-19 14:05:47.000000 pymatviz-0.8.3/tests/test_sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2383 2024-05-27 08:45:46.000000 pymatviz-0.8.3/tests/test_uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    12563 2024-05-30 17:01:28.000000 pymatviz-0.8.3/tests/test_utils.py
```

### Comparing `pymatviz-0.8.2/PKG-INFO` & `pymatviz-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.8.2
+Version: 0.8.3
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -104,44 +104,46 @@
 
 ## Usage
 
 See the Jupyter notebooks under [`examples/`](examples) for how to use `pymatviz`. PRs with additional examples are welcome! 🙏
 
 |                                                                                                                        |                                                                                                                                       |                                      |
 | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
+| [mlff_phonons.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb)                         | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb)             | [![Launch Codespace]][codespace url] |
 | [matbench_dielectric_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)  | [![Launch Codespace]][codespace url] |
 | [mp_bimodal_e_form.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)               | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)        | [![Launch Codespace]][codespace url] |
 | [matbench_perovskites_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_perovskites_eda.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_perovskites_eda.ipynb) | [![Launch Codespace]][codespace url] |
 | [mprester_ptable.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb)                   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb)          | [![Launch Codespace]][codespace url] |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 [Launch Codespace]: https://img.shields.io/badge/Launch-Codespace-darkblue?logo=github
 [codespace url]: https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=340898532
 
 ## Periodic Table
 
 See [`pymatviz/ptable.py`](pymatviz/ptable.py). Heatmaps of the periodic table can be plotted both with `matplotlib` and `plotly`. `plotly` supports displaying additional data on hover or full interactivity through [Dash](https://plotly.com/dash).
 
-|                        [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                        |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
-| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
-|                                              ![ptable-heatmap]                                               |                        ![ptable-heatmap-ratio]                        |
-|                         [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                         | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
-|                                   ![ptable-heatmap-plotly-more-hover-data]                                   |                     ![ptable-heatmap-plotly-log]                      |
-|                       [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                        |              [`ptable_lines(data)`](pymatviz/ptable.py)               |
-|                                               ![ptable-hists]                                                |                            ![ptable-lines]                            |
-| [`ptable_heatmap_splits(data, colormap="coolwarm", start_angle=135, hide_f_block=True)`](pymatviz/ptable.py) |
-|                                           ![ptable-heatmap-splits]                                           |
+|                    [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                    |                   [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)                    |
+| :--------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------: |
+|                                          ![ptable-heatmap]                                           |                                       ![ptable-heatmap-ratio]                                       |
+|                     [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                     |                [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py)                |
+|                               ![ptable-heatmap-plotly-more-hover-data]                               |                                    ![ptable-heatmap-plotly-log]                                     |
+|                   [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                    |                             [`ptable_lines(data)`](pymatviz/ptable.py)                              |
+|                                           ![ptable-hists]                                            |                                           ![ptable-lines]                                           |
+| [`ptable_heatmap_splits(2_vals_per_elem, colormap="coolwarm", start_angle=135)`](pymatviz/ptable.py) | [`ptable_heatmap_splits(3_vals_per_elem, colormap="coolwarm", start_angle=90)`](pymatviz/ptable.py) |
+|                                      ![ptable-heatmap-splits-2]                                      |                                     ![ptable-heatmap-splits-3]                                      |
 
 [ptable-hists]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-hists.svg
 [ptable-lines]: https://github.com/janosh/pymatviz/raw/main/examples/diatomics/homo-nuclear-mace-medium.svg
-[ptable-heatmap-splits]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits.svg
+[ptable-heatmap-splits-2]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits-2.svg
+[ptable-heatmap-splits-3]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits-3.svg
 
 ## Phonons
 
-See [`pymatviz/phonons.py`](pymatviz/phonons.py).
+See [`examples/mlff_phonons.ipynb`](https://github.com/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb) for usage example.
 
 |           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           |             [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py)             |
 | :------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
 |                              ![phonon-bands]                               |                                ![phonon-dos]                                 |
 | [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) | [`plot_phonon_bands_and_dos(single_bands, single_dos)`](pymatviz/phonons.py) |
 |                      ![phonon-bands-and-dos-mp-2758]                       |                       ![phonon-bands-and-dos-mp-23907]                       |
```

### Comparing `pymatviz-0.8.2/license` & `pymatviz-0.8.3/license`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/pymatviz/__init__.py` & `pymatviz-0.8.3/pymatviz/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,22 +99,29 @@
     zeroline=True,
     linewidth=1,
     showgrid=True,
 )
 white_axis_template = axis_template | dict(linecolor="black", gridcolor="lightgray")
 # inherit from plotly_white template
 pmv_white_template = go.layout.Template(pio.templates["plotly_white"])
+common_layout = dict(margin=dict(l=10, r=10, t=10, b=10))
 
 pio.templates[f"{PKG_NAME}_white"] = pmv_white_template.update(
     layout=dict(
-        xaxis=white_axis_template, yaxis=white_axis_template, font=dict(color="black")
+        xaxis=white_axis_template,
+        yaxis=white_axis_template,
+        font=dict(color="black"),
+        **common_layout,
     )
 )
 dark_axis_template = axis_template | dict(linecolor="white", gridcolor="darkgray")
 # inherit from plotly_dark template
 pmv_dark_template = go.layout.Template(pio.templates["plotly_dark"])
 
 pio.templates[f"{PKG_NAME}_dark"] = pmv_dark_template.update(
     layout=dict(
-        xaxis=dark_axis_template, yaxis=dark_axis_template, font=dict(color="white")
+        xaxis=dark_axis_template,
+        yaxis=dark_axis_template,
+        font=dict(color="white"),
+        **common_layout,
     )
 )
```

### Comparing `pymatviz-0.8.2/pymatviz/correlation.py` & `pymatviz-0.8.3/pymatviz/correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     return pre_fac * root * (0 if unit_step else 1)
 
 
 def marchenko_pastur(
     matrix: ArrayLike,
     gamma: float,
+    *,
     sigma: float = 1,
     filter_high_evals: bool = False,
     ax: plt.Axes | None = None,
 ) -> plt.Axes:
     """Plot the eigenvalue distribution of a symmetric matrix (usually a correlation
     matrix) against the Marchenko Pastur distribution.
```

### Comparing `pymatviz-0.8.2/pymatviz/cumulative.py` & `pymatviz-0.8.3/pymatviz/cumulative.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/pymatviz/elements.csv` & `pymatviz-0.8.3/pymatviz/elements.csv`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/pymatviz/enums.py` & `pymatviz-0.8.3/pymatviz/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,26 +5,59 @@
 from enum import Enum, unique
 from typing import TYPE_CHECKING
 
 from pymatviz.utils import styled_html_tag
 
 
 if TYPE_CHECKING:
-    from typing import Self
+    from typing import Any, Self
 
 
-@unique
-class LabelEnum(Enum):  # migrate to StrEnum once only 3.11+ supported
-    """Enum with optional label and description attributes plus dict() methods."""
+class StrEnum(str, Enum):
+    """Enum where members are also (and must be) strings.
+
+    Copied from std lib due to being 3.11+.
+    """
+
+    def __new__(cls, *values: Any) -> Self:
+        """Values must already be str."""
+        if len(values) > 3:
+            raise TypeError(f"too many arguments for str(): {values!r}")
+        if len(values) == 1 and not isinstance(values[0], str):
+            # it must be a string
+            raise TypeError(f"{values[0]!r} is not a string")
+        if len(values) >= 2 and not isinstance(values[1], str):
+            # check that encoding argument is a string
+            raise TypeError(f"encoding must be a string, not {values[1]!r}")
+        if len(values) == 3 and not isinstance(values[2], str):
+            # check that errors argument is a string
+            raise TypeError(f"errors must be a string, not {values[2]!r}")
+        value = str(*values)
+        member = str.__new__(cls, value)
+        member._value_ = value
+        return member
+
+    def _generate_next_value_(  # type: ignore[override]
+        self,
+        start: int,  # noqa: ARG002
+        count: int,  # noqa: ARG002
+        last_values: list[str],  # noqa: ARG002
+    ) -> str:
+        """Return the lower-cased version of the member name."""
+        return self.lower()
+
+
+class LabelEnum(StrEnum):
+    """StrEnum with optional label and description attributes plus dict() methods."""
 
     def __new__(
         cls, val: str, label: str | None = None, desc: str | None = None
     ) -> Self:
         """Create a new class."""
-        member = object.__new__(cls)
+        member = str.__new__(cls, val)
         member._value_ = val
         member.__dict__ |= dict(label=label, desc=desc)
         return member
 
     @property
     def label(self) -> str:
         """Make label read-only."""
@@ -80,14 +113,18 @@
     e_form_true = "e_form_per_atom_true", f"Actual E<sub>form</sub> {eV_per_atom}"
     each = "energy_above_hull", f"E<sub>hull dist</sub> {eV_per_atom}"
     each_pred = "e_above_hull_pred", f"Predicted E<sub>hull dist</sub> {eV_per_atom}"
     each_true = "e_above_hull_true", f"Actual E<sub>MP hull dist</sub> {eV_per_atom}"
     element = "element", "Element"
     energy = "energy", f"Energy {eV}"
     energy_per_atom = "energy_per_atom", f"Energy {eV_per_atom}"
+    cohesive_energy_per_atom = (
+        "cohesive_energy_per_atom",
+        f"Cohesive Energy {eV_per_atom}",
+    )
     final_struct = "final_structure", "Final Structure"
     forces = "forces", "Forces"
     form_energy = "formation_energy_per_atom", f"Formation Energy {eV_per_atom}"
     formula = "formula", "Formula"
     formula_pretty = "formula_pretty", "Pretty Formula"
     heat_val = "heat_val", "Heatmap Value"  # used by PTableProjector for ptable data
     init_struct = "initial_structure", "Initial Structure"
@@ -99,7 +136,20 @@
     spacegroup_symbol = "spacegroup_symbol", "Spacegroup Symbol"
     stress = "stress", "Stress"
     structure = "structure", "Structure"
     task_id = "task_id", "Task ID"  # unique identifier for a compute task
     task_type = "task_type", "Task Type"
     volume = "volume", "Volume (Å³)"
     wyckoff = "wyckoff", "Aflow-style Wyckoff Label"  # crystallographic site symmetry
+    phonon_bandstructure = "phonon_bandstructure", "Phonon Band Structure"
+    phonon_dos = "phonon_dos", "Phonon Density of States"
+
+
+@unique
+class Model(LabelEnum):
+    """Model names."""
+
+    # key, label, color
+    m3gnet_ms = "m3gnet", "M3GNet-MS", "blue"
+    chgnet_030 = "chgnet-v0.3.0", "CHGNet v0.3.0", "orange"
+    mace_mp = "mace-mp-0-medium", "MACE-MP", "green"
+    pbe = "pbe", "PBE", "gray"
```

### Comparing `pymatviz-0.8.2/pymatviz/histograms.py` & `pymatviz-0.8.3/pymatviz/histograms.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from pymatgen.core import Structure
 from pymatgen.symmetry.groups import SpaceGroup
 
 from pymatviz.enums import Key
 from pymatviz.powerups import annotate_bars
 from pymatviz.ptable import count_elements
 from pymatviz.utils import (
+    PLOTLY_BACKEND,
     Backend,
     crystal_sys_from_spg_num,
     df_to_arrays,
-    plotly_key,
     si_fmt_int,
 )
 
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
 
@@ -104,20 +104,22 @@
     ax.figure.set_size_inches(12, 7)
 
     return ax
 
 
 def spacegroup_hist(
     data: Sequence[int | str | Structure] | pd.Series,
+    *,
     show_counts: bool = True,
     xticks: Literal["all", "crys_sys_edges"] | int = 20,
     show_empty_bins: bool = False,
     ax: plt.Axes | None = None,
     backend: Backend = "plotly",
     text_kwargs: dict[str, Any] | None = None,
+    log: bool = False,
     **kwargs: Any,
 ) -> plt.Axes | go.Figure:
     """Plot a histogram of spacegroups shaded by crystal system.
 
     Args:
         data (list[int | str | Structure] | pd.Series): Space group strings or numbers
             (from 1 - 230) or pymatgen structures.
@@ -132,28 +134,28 @@
             not symbols. Defaults to False.
         ax (Axes, optional): matplotlib Axes on which to plot. Defaults to None.
         backend ("matplotlib" | "plotly", optional): Which backend to use for plotting.
             Defaults to "plotly".
         text_kwargs (dict, optional): Keyword arguments passed to
             matplotlib.Axes.text(). Defaults to None. Has no effect if backend is
             "plotly".
+        log (bool, optional): Whether to log scale the y-axis. Defaults to False.
         kwargs: Keywords passed to pd.Series.plot.bar() or plotly.express.bar().
 
     Returns:
         plt.Axes | go.Figure: matplotlib Axes or plotly Figure depending on backend.
     """
     if isinstance(next(iter(data)), Structure):
         # if 1st sequence item is structure, assume all are
         data = cast(Sequence[Structure], data)
         series = pd.Series(struct.get_space_group_info()[1] for struct in data)
     else:
         series = pd.Series(data)
 
     count_col = "Counts"
-    crys_sys_col = Key.crystal_system.value
     df_data = series.value_counts(sort=False).to_frame(name=count_col)
 
     crystal_sys_colors = {
         "triclinic": "red",
         "monoclinic": "teal",
         "orthorhombic": "blue",
         "tetragonal": "green",
@@ -162,54 +164,60 @@
         "cubic": "darkred",
     }
 
     if df_data.index.inferred_type == "integer":  # assume index is space group numbers
         df_data = df_data.reindex(range(1, 231), fill_value=0).sort_index()
         if not show_empty_bins:
             df_data = df_data.query(f"{count_col} > 0")
-        df_data[crys_sys_col] = [crystal_sys_from_spg_num(x) for x in df_data.index]
+        df_data[Key.crystal_system] = [
+            crystal_sys_from_spg_num(x) for x in df_data.index
+        ]
 
         xlim = (df_data.index.min() - 0.5, df_data.index.max() + 0.5)
         x_label = "International Spacegroup Number"
 
     else:  # assume index is space group symbols
         # TODO: figure how to implement show_empty_bins for space group symbols
         # if show_empty_bins:
         #     idx = [SpaceGroup.from_int_number(x).symbol for x in range(1, 231)]
         #     df = df.reindex(idx, fill_value=0)
         df_data = df_data[df_data[count_col] > 0]
-        df_data[crys_sys_col] = [SpaceGroup(x).crystal_system for x in df_data.index]
+        df_data[Key.crystal_system] = [
+            SpaceGroup(x).crystal_system for x in df_data.index
+        ]
 
         # sort df by crystal system going from smallest to largest spacegroup numbers
         # e.g. triclinic (1-2) comes first, cubic (195-230) last
         sys_order = dict(zip(crystal_sys_colors, range(len(crystal_sys_colors))))
-        df_data = df_data.loc[df_data[crys_sys_col].map(sys_order).sort_values().index]
+        df_data = df_data.loc[
+            df_data[Key.crystal_system].map(sys_order).sort_values().index
+        ]
 
         x_label = "International Spacegroup Symbol"
 
     # count rows per crystal system
-    crys_sys_counts = df_data.groupby(crys_sys_col).sum(count_col)
-    crys_sys_counts["width"] = df_data.value_counts(crys_sys_col)
+    crys_sys_counts = df_data.groupby(Key.crystal_system).sum(count_col)
+    crys_sys_counts["width"] = df_data.value_counts(Key.crystal_system)
     crys_sys_counts["color"] = pd.Series(crystal_sys_colors)
 
     # sort by key order in dict crys_colors
     crys_sys_counts = crys_sys_counts.loc[
         [x for x in crystal_sys_colors if x in crys_sys_counts.index]
     ]
     xlim = (0, len(df_data) - 1)
 
     fig_title = f"{count_col} per crystal system" if show_counts else None
-    if backend == plotly_key:
+    if backend == PLOTLY_BACKEND:
         df_plot = df_data if show_empty_bins else df_data.reset_index()
 
         fig = px.bar(
             df_plot,
             x=df_plot.index,
             y=count_col,
-            color=df_data[crys_sys_col],
+            color=df_data[Key.crystal_system],
             color_discrete_map=crystal_sys_colors,
             **kwargs,
         )
         # add vertical lines between crystal systems and fill area with color
         x0 = x1 = 0
         for idx, (crys_sys, count, width, color) in enumerate(
             crys_sys_counts.itertuples()
@@ -245,16 +253,17 @@
                     yanchor="bottom",
                 )
             x0 += width
 
         fig.update_layout(showlegend=False)
         fig.layout.title.update(text=fig_title, x=0.5)
         fig.layout.xaxis.update(showgrid=False, title=x_label, range=xlim)
-        ylim = (0, int(df_data[count_col].max() * 1.05))
-        fig.layout.yaxis.update(range=ylim)
+        count_max = df_data[count_col].max()
+        y_max = np.log10(count_max * 1.05) if log else count_max * 1.05
+        fig.layout.yaxis.update(range=(0, y_max), type="log" if log else None)
         fig.layout.margin = dict(l=0, r=0, t=40, b=0)
 
         if isinstance(xticks, int):
             # get x_locs of n=xticks tallest bars
             x_indices = df_data.reset_index()[count_col].nlargest(xticks).index
             tick_text = df_data.iloc[x_indices].index
         elif xticks == "crys_sys_edges":
@@ -280,25 +289,25 @@
     defaults = dict(width=0.9)  # set default histogram bar width
     df_data[count_col].plot.bar(figsize=[16, 4], ax=ax, **defaults | kwargs)
 
     ax.set_title(fig_title, fontdict={"fontsize": 18}, pad=30)
     ax.set(xlabel=x_label)
 
     # https://matplotlib.org/3.1.1/gallery/lines_bars_and_markers/fill_between_demo
-    trans = transforms.blended_transform_factory(ax.transData, ax.transAxes)
+    transform = transforms.blended_transform_factory(ax.transData, ax.transAxes)
 
     # add crystal system labels and dividers
     x0 = 0
     for crys_sys, count, width, color in crys_sys_counts.itertuples():
         x1 = x0 + width
 
         for patch in ax.patches[0 if x0 == 1 else x0 : x1 + 1]:
             patch.set_facecolor(color)
 
-        text_kwds = dict(transform=trans, horizontalalignment="center") | (
+        text_kwds = dict(transform=transform, horizontalalignment="center") | (
             text_kwargs or {}
         )
         crys_sys_anno_kwds = dict(
             rotation=90, va="top", ha="right", fontdict={"fontsize": 14}
         )
         ax.text(*[(x0 + x1) / 2, 0.95], crys_sys, **crys_sys_anno_kwds | text_kwds)
         if show_counts:
@@ -309,40 +318,43 @@
             )
 
         ax.fill_between(
             [x0 - 0.5, x1 - 0.5],
             *[0, 1],
             facecolor=color,
             alpha=0.1,
-            transform=trans,
+            transform=transform,
             edgecolor="black",
         )
         x0 += width
 
     ax.yaxis.grid(visible=True)
     ax.xaxis.grid(visible=False)
+    ax.set_ylim(0, None)
+    if log:
+        ax.set_yscale("log")
 
     if xticks == "crys_sys_edges" or isinstance(xticks, int):
         if isinstance(xticks, int):
             # get x_locs of n=xticks tallest bars
             x_indices = df_data.reset_index().sort_values(count_col).tail(xticks).index
         else:
             # add x_locs of n=xticks tallest bars
             x_indices = crys_sys_counts.width.cumsum()
 
         major_loc = FixedLocator(x_indices)
 
         ax.xaxis.set_major_locator(major_loc)
     plt.xticks(rotation=90)
-
     return ax
 
 
 def elements_hist(
     formulas: ElemValues,
+    *,
     count_mode: CountMode = Key.composition,
     log: bool = False,
     keep_top: int | None = None,
     ax: plt.Axes | None = None,
     bar_values: Literal["percent", "count"] | None = "percent",
     h_offset: int = 0,
     v_offset: int = 10,
```

### Comparing `pymatviz-0.8.2/pymatviz/io.py` & `pymatviz-0.8.3/pymatviz/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,21 @@
             variables are set. Defaults to ("CI",).
         pdf_sleep (float, optional): Minimum time in seconds to wait before writing a
             plotly figure to PDF file. Workaround for this plotly issue
             https://github.com/plotly/plotly.py/issues/3469. Defaults to 0.6. Has no
             effect on matplotlib figures.
         style (str, optional): CSS style string to be inserted into the HTML file.
             Defaults to "". Only used if path ends with .svelte or .html.
-        prec (int, optional): Number of significant figures to keep for any float
+        prec (int, optional): Number of significant digits to keep for any float
             in the exported file. Defaults to None (no rounding). Sensible values are
             usually 4, 5, 6.
         template (str, optional): Temporary plotly to apply to the figure before
             saving. Will be reset to the original after. Defaults to "pymatviz_white" if
             path ends with .pdf or .pdfa, else None. Set to None to disable. Only used
             if fig is a plotly figure.
-
         **kwargs: Keyword arguments passed to fig.write_html().
     """
     is_pdf = path.lower().endswith((".pdf", ".pdfa"))
     if template is None and is_pdf:
         template = "pymatviz_white"
 
     if prec is not None:
@@ -147,37 +146,41 @@
 
             fig.layout.template = orig_template
         for trace in hidden_traces:
             trace.visible = "legendonly"
 
 
 def save_and_compress_svg(
-    fig: go.Figure | plt.Figure | plt.Axes, filename: str
+    fig: go.Figure | plt.Figure | plt.Axes,
+    filename: str,
 ) -> None:
-    """Save Plotly figure as SVG and HTML to assets/ folder. Compresses SVG
-    file with svgo CLI if available in PATH.
+    """Save Plotly figure as SVG and HTML to assets/ folder.
+    Compresses SVG file with svgo CLI if available in PATH.
 
     Args:
         fig (Figure): Plotly or matplotlib Figure/Axes instance.
         filename (str): Name of SVG file (w/o extension).
 
     Raises:
         ValueError: If fig is None and plt.gcf() is empty.
     """
-    if filename.endswith(".svg"):
-        raise ValueError(f"{filename=} should not include .svg")
-    filepath = f"{ROOT}/assets/{filename}.svg"
     if isinstance(fig, plt.Axes):
         fig = fig.figure
 
     if isinstance(fig, plt.Figure) and not fig.axes:
         raise ValueError("Passed fig contains no axes. Nothing to plot!")
+
+    if filename.endswith(".svg"):
+        filename = filename.rstrip(".svg")
+
+    filepath = f"{ROOT}/assets/{filename}.svg"
     save_fig(fig, filepath)
     plt.close()
 
+    # Compress SVG if svgo is available
     if (svgo := which("svgo")) is not None:
         subprocess.run([svgo, "--multipass", filepath], check=True)  # noqa: S603
 
 
 DEFAULT_DF_STYLES: Final = {
     "": "font-family: sans-serif; border-collapse: collapse;",
     "td, th": "border: none; padding: 4px 6px; white-space: nowrap;",
@@ -185,14 +188,15 @@
     "th.row_heading": "font-weight: normal; padding: 3pt;",
 }
 
 
 def df_to_pdf(
     styler: Styler,
     file_path: str | Path,
+    *,
     crop: bool = True,
     size: str | None = None,
     style: str = "",
     styler_css: bool | dict[str, str] = True,
     **kwargs: Any,
 ) -> None:
     """Export a pandas Styler to PDF with WeasyPrint.
@@ -312,14 +316,15 @@
 table::-webkit-scrollbar {
     display: none;  /* Safari and Chrome */
 }"""
 
 
 def df_to_html_table(
     styler: Styler,
+    *,
     file_path: str | Path | None = None,
     inline_props: str | None = "",
     script: str | None = "",
     styles: str | None = ALLOW_TABLE_SCROLL + HIDE_SCROLL_BAR,
     styler_css: bool | dict[str, str] = True,
     sortable: bool = True,
     post_process: Callable[[str], str] | None = None,
```

### Comparing `pymatviz-0.8.2/pymatviz/parity.py` & `pymatviz-0.8.3/pymatviz/parity.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     from matplotlib.gridspec import GridSpec
     from numpy.typing import ArrayLike
 
 
 def hist_density(
     x: ArrayLike | str,
     y: ArrayLike | str,
+    *,
     df: pd.DataFrame | None = None,
     sort: bool = True,
     bins: int = 100,
     method: str = "nearest",
 ) -> tuple[ArrayLike, ArrayLike, ArrayLike]:
     """Return an approximate density of 2d points.
 
@@ -65,14 +66,15 @@
 
     return xs, ys, zs
 
 
 def density_scatter(
     x: ArrayLike | str,
     y: ArrayLike | str,
+    *,
     df: pd.DataFrame | None = None,
     ax: plt.Axes | None = None,
     log_density: bool = True,
     hist_density_kwargs: dict[str, Any] | None = None,
     color_bar: bool | dict[str, Any] = True,
     xlabel: str | None = None,
     ylabel: str | None = None,
@@ -147,14 +149,15 @@
 
     return ax
 
 
 def scatter_with_err_bar(
     x: ArrayLike | str,
     y: ArrayLike | str,
+    *,
     df: pd.DataFrame | None = None,
     xerr: ArrayLike | None = None,
     yerr: ArrayLike | None = None,
     ax: plt.Axes | None = None,
     identity_line: bool | dict[str, Any] = True,
     best_fit_line: bool | dict[str, Any] = True,
     xlabel: str = "Actual",
@@ -206,14 +209,15 @@
 
     return ax
 
 
 def density_hexbin(
     x: ArrayLike | str,
     y: ArrayLike | str,
+    *,
     df: pd.DataFrame | None = None,
     ax: plt.Axes | None = None,
     weights: ArrayLike | None = None,
     identity_line: bool | dict[str, Any] = True,
     best_fit_line: bool | dict[str, Any] = True,
     xlabel: str = "Actual",
     ylabel: str = "Predicted",
```

### Comparing `pymatviz-0.8.2/pymatviz/phonons.py` & `pymatviz-0.8.3/pymatviz/phonons.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,24 +193,28 @@
         branches = [branches]
 
     if branch_mode not in get_args(BranchMode):
         raise ValueError(
             f"Invalid {branch_mode=}, must be one of {get_args(BranchMode)}"
         )
 
+    if type(band_structs) not in {PhononBands, dict}:
+        cls_name = PhononBands.__name__
+        raise TypeError(
+            f"Only {cls_name} or dict supported, got {type(band_structs).__name__}"
+        )
+    if isinstance(band_structs, dict) and len(band_structs) == 0:
+        raise ValueError("Empty band structure dict")
+
     if not isinstance(band_structs, dict):  # normalize input to dictionary
         band_structs = {"": band_structs}
 
     # find common branches by normalized branch names
     common_branches: set[str] = set()
     for idx, bs in enumerate(band_structs.values()):
-        if not isinstance(bs, PhononBands):
-            raise TypeError(
-                f"Only {PhononBands.__name__} supported, got {type(bs).__name__}"
-            )
         bs_branches = {branch["name"] for branch in bs.branches}
         common_branches = (
             bs_branches
             if idx == 0
             # calc set union/intersect (& or |) depending on branch_mode
             else getattr(common_branches, branch_mode)(bs_branches)
         )
@@ -313,14 +317,15 @@
     _shaded_range(fig, shaded_ys)
 
     return fig
 
 
 def plot_phonon_dos(
     doses: PhononDos | dict[str, PhononDos],
+    *,
     stack: bool = False,
     sigma: float = 0,
     units: Literal["THz", "eV", "meV", "Ha", "cm-1"] = "THz",
     normalize: Literal["max", "sum", "integral"] | None = None,
     last_peak_anno: str | None = None,
     **kwargs: Any,
 ) -> go.Figure:
@@ -342,14 +347,22 @@
 
     Returns:
         go.Figure: Plotly figure object.
     """
     valid_normalize = (None, "max", "sum", "integral")
     if normalize not in valid_normalize:
         raise ValueError(f"Invalid {normalize=}, must be one of {valid_normalize}.")
+
+    if type(doses) not in {PhononDos, dict}:
+        raise TypeError(
+            f"Only {PhononDos.__name__} or dict supported, got {type(doses).__name__}"
+        )
+    if isinstance(doses, dict) and len(doses) == 0:
+        raise ValueError("Empty DOS dict")
+
     if last_peak_anno == "":
         last_peak_anno = "ω<sub>{key}</sub></span>={last_peak:.1f} {units}"
 
     fig = go.Figure()
     doses = {"": doses} if isinstance(doses, PhononDos) else doses
 
     for key, dos in doses.items():
@@ -361,25 +374,25 @@
         densities = dos.get_smeared_densities(sigma)
 
         # convert frequencies to specified units
         frequencies = convert_frequencies(frequencies, units)
 
         # normalize DOS
         if normalize == "max":
-            densities = densities / densities.max()
+            densities /= densities.max()
         elif normalize == "sum":
-            densities = densities / densities.sum()
+            densities /= densities.sum()
         elif normalize == "integral":
             bin_width = frequencies[1] - frequencies[0]
             densities = densities / densities.sum() / bin_width
 
         defaults = dict(mode="lines")
         if stack:
             if fig.data:  # for stacked plots, accumulate densities
-                densities = densities + fig.data[-1].y
+                densities += fig.data[-1].y
             defaults.setdefault("fill", "tonexty")
 
         fig.add_scatter(x=frequencies, y=densities, name=key, **(defaults | kwargs))
 
     fig.layout.xaxis.update(title=f"Frequency ({units})")
     fig.layout.yaxis.update(title="Density of States")
     fig.layout.margin = dict(t=5, b=5, l=5, r=5)
```

### Comparing `pymatviz-0.8.2/pymatviz/powerups.py` & `pymatviz-0.8.3/pymatviz/powerups.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 import plotly.express as px
 import plotly.graph_objects as go
 import sklearn
 from sklearn.metrics import mean_absolute_percentage_error as mape
 from sklearn.metrics import r2_score
 
 from pymatviz.utils import (
+    MPL_BACKEND,
+    PLOTLY_BACKEND,
     AxOrFig,
     Backend,
     annotate,
     get_fig_xy_range,
-    mpl_key,
-    plotly_key,
     pretty_label,
     validate_fig,
 )
 
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
@@ -80,14 +80,15 @@
     ax_histy.axis("off")
 
     return ax_main
 
 
 def annotate_bars(
     ax: plt.Axes | None = None,
+    *,
     v_offset: float = 10,
     h_offset: float = 0,
     labels: Sequence[str | int | float] | None = None,
     fontsize: int = 14,
     y_max_headroom: float = 1.2,
     adjust_test_pos: bool = False,
     **kwargs: Any,
@@ -121,17 +122,17 @@
     y_max: float = 0
     texts: list[Annotation] = []
     for rect, label in zip(ax.patches, labels):
         y_pos = rect.get_height()
         x_pos = rect.get_x() + rect.get_width() / 2 + h_offset
 
         if ax.get_yscale() == "log":
-            y_pos = y_pos + np.log(max(1, v_offset))
+            y_pos += np.log(max(1, v_offset))
         else:
-            y_pos = y_pos + v_offset
+            y_pos += v_offset
 
         y_max = max(y_max, y_pos)
 
         txt = f"{label:,}" if isinstance(label, (int, float)) else label
         # place label at end of the bar and center horizontally
         anno = ax.annotate(
             txt, (x_pos, y_pos), ha="center", fontsize=fontsize, **kwargs
@@ -188,15 +189,15 @@
     if isinstance(metrics, str):
         metrics = [metrics]
     if not isinstance(metrics, (dict, list, tuple, set)):
         raise TypeError(
             f"metrics must be dict|list|tuple|set, not {type(metrics).__name__}"
         )
 
-    backend: Backend = plotly_key if isinstance(fig, go.Figure) else mpl_key
+    backend: Backend = PLOTLY_BACKEND if isinstance(fig, go.Figure) else MPL_BACKEND
 
     funcs = {
         "MAE": lambda x, y: np.abs(x - y).mean(),
         "RMSE": lambda x, y: (((x - y) ** 2).mean()) ** 0.5,
         "MSE": lambda x, y: ((x - y) ** 2).mean(),
         "MAPE": mape,
         "R2": r2_score,
@@ -208,15 +209,15 @@
     if bad_keys := set(metrics) - set(funcs):
         raise ValueError(f"Unrecognized metrics: {bad_keys}")
 
     nan_mask = np.isnan(xs) | np.isnan(ys)
     xs, ys = xs[~nan_mask], ys[~nan_mask]
 
     text = prefix
-    newline = "\n" if backend == mpl_key else "<br>"
+    newline = "\n" if backend == MPL_BACKEND else "<br>"
 
     if isinstance(metrics, dict):
         for key, val in metrics.items():
             label = pretty_label(key, backend)
             text += f"{label} = {val:{fmt}}{newline}"
     else:
         for key in metrics:
@@ -226,16 +227,18 @@
     text += suffix
 
     return annotate(text, fig, **kwargs)
 
 
 def add_identity_line(
     fig: go.Figure | plt.Figure | plt.Axes,
+    *,
     line_kwds: dict[str, Any] | None = None,
     trace_idx: int = 0,
+    retain_xy_limits: bool = False,
     **kwargs: Any,
 ) -> go.Figure:
     """Add a line shape to the background layer of a plotly figure spanning
     from smallest to largest x/y values in the trace specified by trace_idx.
 
     Args:
         fig (go.Figure | plt.Figure | plt.Axes): plotly/matplotlib figure or axes to
@@ -243,14 +246,16 @@
         line_kwds (dict[str, Any], optional): Keyword arguments for customizing the line
             shape will be passed to fig.add_shape(line=line_kwds). Defaults to
             dict(color="gray", width=1, dash="dash").
         trace_idx (int, optional): Index of the trace to use for measuring x/y limits.
             Defaults to 0. Unused if kaleido package is installed and the figure's
             actual x/y-range can be obtained from fig.full_figure_for_development().
             Applies only to plotly figures.
+        retain_xy_limits (bool, optional): If True, the x/y-axis limits will be retained
+            after adding the identity line. Defaults to False.
         **kwargs: Additional arguments are passed to fig.add_shape().
 
     Raises:
         TypeError: If fig is neither a plotly nor a matplotlib figure or axes.
         ValueError: If fig is a plotly figure and kaleido is not installed and trace_idx
             is out of range.
 
@@ -282,20 +287,24 @@
     fig.add_shape(
         type="line",
         **dict(x0=xy_min, y0=xy_min, x1=xy_max, y1=xy_max),
         layer="below",
         line=line_defaults | (line_kwds or {}),
         **kwargs,
     )
+    if retain_xy_limits:
+        fig.update_xaxes(range=[x_min, x_max])
+        fig.update_yaxes(range=[y_min, y_max])
 
     return fig
 
 
 def add_best_fit_line(
     fig: go.Figure | plt.Figure | plt.Axes,
+    *,
     xs: ArrayLike = (),
     ys: ArrayLike = (),
     trace_idx: int = 0,
     line_kwds: dict[str, Any] | None = None,
     annotate_params: bool | dict[str, Any] = True,
     **kwargs: Any,
 ) -> go.Figure:
@@ -328,15 +337,15 @@
         Figure: Figure with added best fit line.
     """
     valid_types = (go.Figure, plt.Figure, plt.Axes)
     if not isinstance(fig, valid_types):
         type_names = " | ".join(f"{t.__module__}.{t.__qualname__}" for t in valid_types)
         raise TypeError(f"{fig=} must be instance of {type_names}")
 
-    backend = plotly_key if isinstance(fig, go.Figure) else mpl_key
+    backend = PLOTLY_BACKEND if isinstance(fig, go.Figure) else MPL_BACKEND
     kwargs.setdefault("color", "blue")
 
     if 0 in {len(xs), len(ys)}:
         if isinstance(fig, go.Figure):
             if not len(xs) or not len(ys):
                 trace = fig.data[trace_idx]
                 xs, ys = trace.x, trace.y
@@ -353,30 +362,30 @@
 
     x_min = get_fig_xy_range(fig)[0][0]
 
     x0, x1 = x_min, x_min + 1
     y0, y1 = slope * x0 + intercept, slope * x1 + intercept
 
     if annotate_params:
-        if backend == mpl_key:
+        if backend == MPL_BACKEND:
             defaults = dict(loc="lower right", color=kwargs["color"])
         else:
             defaults = dict(
                 xref="paper",
                 yref="paper",
                 x=0.02,
                 y=0.96,
                 showarrow=False,
                 font_color=kwargs["color"],
             )
         if isinstance(annotate_params, dict):
             defaults |= annotate_params
         annotate(f"LS fit: y = {slope:.2}x + {intercept:.2}", fig=fig, **defaults)
 
-    if backend == mpl_key:
+    if backend == MPL_BACKEND:
         ax = fig if isinstance(fig, plt.Axes) else fig.gca()
 
         defaults = dict(alpha=0.7, linestyle="--", zorder=1)
         ax.axline((x0, y0), (x1, y1), **(defaults | (line_kwds or {})) | kwargs)
 
         return fig
```

### Comparing `pymatviz-0.8.2/pymatviz/ptable.py` & `pymatviz-0.8.3/pymatviz/ptable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,116 +1,50 @@
 """Various periodic table heatmaps with matplotlib and plotly."""
 
 from __future__ import annotations
 
-import inspect
 import itertools
 import math
 import warnings
 from collections.abc import Sequence
 from functools import partial
 from typing import TYPE_CHECKING, Literal, Union, get_args
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.figure_factory as ff
-from matplotlib.cm import get_cmap
 from matplotlib.colors import Colormap, LogNorm, Normalize
 from matplotlib.patches import Rectangle
 from pandas.api.types import is_numeric_dtype, is_string_dtype
 from pymatgen.core import Composition, Element
 
+from pymatviz._preprocess_data import (
+    SupportedDataType,
+    SupportedValueType,
+    preprocess_ptable_data,
+)
 from pymatviz.enums import Key
-from pymatviz.utils import df_ptable, pick_bw_for_contrast, si_fmt, si_fmt_int
+from pymatviz.utils import ELEM_TYPE_COLORS, df_ptable, pick_bw_for_contrast, si_fmt
 
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, Final
+    from typing import Any, Callable
 
     import plotly.graph_objects as go
 
 
-# Data types supported by ptable plotters
-SupportedValueType = Union[Sequence[float], np.ndarray]
-
-SupportedDataType = Union[
-    dict[str, Union[float, Sequence[float], np.ndarray]], pd.DataFrame, pd.Series
-]
-
 CountMode = Literal[
     Key.composition, "fractional_composition", "reduced_composition", "occurrence"
 ]
 
 ElemValues = Union[dict[Union[str, int], float], pd.Series, Sequence[str]]
 
-ELEM_CLASS_COLORS: Final = {
-    "Diatomic Nonmetal": "green",
-    "Noble Gas": "purple",
-    "Alkali Metal": "red",
-    "Alkaline Earth Metal": "orange",
-    "Metalloid": "darkgreen",
-    "Polyatomic Nonmetal": "teal",
-    "Transition Metal": "blue",
-    "Post Transition Metal": "cyan",
-    "Lanthanide": "brown",
-    "Actinide": "gray",
-    "Nonmetal": "green",
-    "Halogen": "teal",
-    "Metal": "lightblue",
-    "Alkaline Metal": "magenta",
-    "Transactinide": "olive",
-}
-
-
-def add_element_type_legend(
-    data: pd.DataFrame | pd.Series | dict[str, list[float]],
-    elem_class_colors: dict[str, str] | None = None,
-    legend_kwargs: dict[str, Any] | None = None,
-) -> None:
-    """Add a legend to a matplotlib figure showing the colors of element types.
-
-
-    Args:
-        data (pd.DataFrame | pd.Series | dict[str, list[float]]): Map from element
-            to plot data. Used only to determine which element types are present.
-        elem_class_colors (dict[str, str]): Map from element
-            types to colors. E.g. {"Alkali Metal": "red", "Noble Gas": "blue"}.
-        legend_kwargs (dict): Keyword arguments passed to plt.legend() for customizing
-            legend appearance. Defaults to None.
-    """
-    elem_class_colors = ELEM_CLASS_COLORS | (elem_class_colors or {})
-    # else case list(data) covers dict and DataFrame
-    elems_with_data = data.index if isinstance(data, pd.Series) else list(data)
-    visible_elem_types = df_ptable.loc[elems_with_data, "type"].unique()
-    font_size = 10
-    legend_elements = [
-        plt.Line2D(
-            *([0], [0]),
-            marker="s",
-            color="w",
-            label=elem_class,
-            markerfacecolor=color,
-            markersize=1.2 * font_size,
-        )
-        for elem_class, color in elem_class_colors.items()
-        if elem_class in visible_elem_types
-    ]
-    legend_kwargs = dict(
-        loc="center left",
-        bbox_to_anchor=(0, -42),
-        ncol=6,
-        frameon=False,
-        fontsize=font_size,
-        handlelength=1,  # more compact legend
-    ) | (legend_kwargs or {})
-    plt.legend(handles=legend_elements, **legend_kwargs)
-
 
 def count_elements(
     values: ElemValues,
     count_mode: CountMode = Key.composition,
     exclude_elements: Sequence[str] = (),
     fill_value: float | None = 0,
 ) -> pd.Series:
@@ -214,155 +148,66 @@
             raise ValueError(
                 f"Unexpected symbol(s) {bad_symbols} in {exclude_elements=}"
             ) from exc
 
     return srs
 
 
-def data_preprocessor(data: SupportedDataType) -> pd.DataFrame:
-    """Preprocess input data for ptable plotters, including:
-        - Convert all data types to pd.DataFrame.
-        - Impute missing values.
-        - Handle anomalies such as NaN, infinity.
-        - Write vmin/vmax as metadata into the DataFrame.
-
-    Returns:
-        pd.DataFrame: The preprocessed DataFrame with element names
-            as index and values as columns.
-
-    Example:
-        >>> data_dict: dict = {
-            "H": 1.0,
-            "He": [2.0, 4.0],
-            "Li": [[6.0, 8.0], [10.0, 12.0]],
-        }
-
-        OR
-        >>> data_df: pd.DataFrame = pd.DataFrame(
-            data_dict.items(),
-            columns=["element", "heat_val"]
-            ).set_index("element")
-
-        OR
-        >>> data_series: pd.Series = pd.Series(data_dict)
-
-        >>> preprocess_data(data_dict / df / series)
-
-             Element   Value
-        0    H         [1.0, ]
-        1    He        [2.0, 4.0]
-        2    Li        [[6.0, 8.0], [10.0, 12.0]]
-
-        Metadata:
-            vmin: 1.0
-            vmax: 12.0
-    """
-
-    def set_vmin_vmax(df: pd.DataFrame) -> pd.DataFrame:
-        """Write vmin and vmax to DataFrame metadata."""
-        # flatten up to triple nested lists
-        values = df[Key.heat_val].explode().explode().explode()
-        numeric_values = pd.to_numeric(values, errors="coerce")
-
-        df.attrs["vmin"] = numeric_values.min()  # ignores NaNs
-        df.attrs["vmax"] = numeric_values.max()
-        return df
-
-    # Check and handle different supported data types
-    if isinstance(data, pd.DataFrame):
-        data_df = data
-
-    elif isinstance(data, pd.Series):
-        data_df = data.to_frame(name=Key.heat_val)
-        data_df.index.name = Key.element
-
-    elif isinstance(data, dict):
-        data_df = pd.DataFrame(
-            data.items(), columns=[Key.element, Key.heat_val]
-        ).set_index(Key.element)
-
-    else:
-        raise TypeError(f"Unsupported data type, choose from: {SupportedDataType}.")
-
-    # Convert all values to np.array
-    data_df[Key.heat_val] = data_df[Key.heat_val].map(
-        lambda x: np.array([x]) if isinstance(x, float) else np.array(x)
-    )
-
-    # Handle missing and anomalous values
-    data_df = handle_missing_and_anomaly(data_df)
-
-    # Write vmin/vmax into metadata
-    return set_vmin_vmax(data_df)
-
-
-def handle_missing_and_anomaly(
-    df: pd.DataFrame,
-    # missing_strategy: Literal["zero", "mean"] = "mean",
-) -> pd.DataFrame:
-    """Handle missing value (NaN) and anomaly (infinity).
-
-    Infinity would be replaced by vmax(∞) or vmin(-∞).
-    Missing values would be handled by selected strategy:
-        - zero: impute with zeros
-        - mean: impute with mean value
-
-    TODO: finish this function
-    """
-    return df
-
-
 class PTableProjector:
     """Project (nest) a custom plot into a periodic table.
 
+    Attributes:
+        cmap (Colormap | None): Colormap.
+        data (pd.DataFrame): Data for plotting.
+        norm (Normalize): Data min-max normalizer.
+        hide_f_block (bool): Whether to hide f-block.
+        elem_types (set[str]): Types of elements present.
+        elem_type_colors (dict[str, str]): Element typed based colors.
+        elem_colors (dict): Element based colors.
+
     Scopes mentioned in this plotter:
-        plot: Refers to the global scope.
-        ax: Refers to the axis where child plotter would plot.
-        child: Refers to the child plotter itself, for example, ax.plot().
+        plot: Refers to the global Figure.
+        axis: Refers to the Axis where child plotter would plot.
+        child: Refers to the child plotter, for example, ax.plot().
     """
 
     def __init__(
         self,
         *,
         data: SupportedDataType,
-        colormap: str | Colormap | None,
+        colormap: str | Colormap = "viridis",
         plot_kwargs: dict[str, Any] | None = None,
         hide_f_block: bool | None = None,
+        elem_type_colors: dict[str, str] | None = None,
+        elem_colors: dict[str, Any] | None = None,
     ) -> None:
         """Initialize a ptable projector.
 
         Default figsize is set to (0.75 * n_groups, 0.75 * n_periods),
         and axes would be turned off by default.
 
         Args:
             data (SupportedDataType): The data to be visualized.
-            colormap (str | Colormap | None): The colormap to use.
+            colormap (str | Colormap): The colormap to use. Defaults to "viridis".
             plot_kwargs (dict): Additional keyword arguments to
                 pass to the plt.subplots function call.
-            hide_f_block: Hide f-block (Lanthanum and Actinium series). Defaults to
-                None, meaning hide if no data is provided for f-block elements.
+            hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults
+                to None, meaning hide if no data provided for f-block elements.
+            elem_type_colors (dict | None): Element typed based colors.
+            elem_colors (dict | None): Element-specific colors.
         """
-        # Get colormap
+        # Set colors
         self.cmap: Colormap = colormap
+        self._elem_type_colors = ELEM_TYPE_COLORS | (elem_type_colors or {})
+        self.elem_colors = elem_colors  # type: ignore[assignment]
 
         # Preprocess data
         self.data: pd.DataFrame = data
 
-        if hide_f_block is None:
-            hide_f_block = bool(
-                {
-                    atom_num
-                    for atom_num in [*range(57, 72), *range(89, 104)]  # rare earths
-                    # check if data is present for f-block elements
-                    if (elem := Element.from_Z(atom_num).symbol) in self.data.index  # type: ignore[union-attr]
-                    and self.data.loc[elem, Key.heat_val]  # type: ignore[union-attr]
-                }
-            )
-
-        self.hide_f_block = hide_f_block
+        self.hide_f_block = hide_f_block  # type: ignore[assignment]
 
         # Initialize periodic table canvas
         n_periods = df_ptable.row.max()
         n_groups = df_ptable.column.max()
 
         if self.hide_f_block:
             n_periods -= 3
@@ -392,42 +237,110 @@
         """The preprocessed data."""
         return self._data
 
     @data.setter
     def data(self, data: SupportedDataType) -> None:
         """Set and preprocess the data. Also set normalizer."""
         # Preprocess data
-        self._data: pd.DataFrame = data_preprocessor(data)
+        self._data = preprocess_ptable_data(data)
 
         # Normalize data for colorbar
-        self._norm: Normalize = Normalize(
-            vmin=self._data.attrs["vmin"], vmax=self._data.attrs["vmax"]
-        )
+        vmin = self._data.attrs["vmin"]
+        vmax = self._data.attrs["vmax"]
+        self._norm = Normalize(vmin=vmin, vmax=vmax)
 
     @property
     def norm(self) -> Normalize:
         """Data min-max normalizer."""
         return self._norm
 
+    @property
+    def hide_f_block(self) -> bool:
+        """Whether to hide f-block in plots."""
+        return self._hide_f_block
+
+    @hide_f_block.setter
+    def hide_f_block(self, hide_f_block: bool | None) -> None:
+        """If hide_f_block is None, would detect if data is present."""
+        if hide_f_block is None:
+            f_block_elements_with_data = {
+                atom_num
+                for atom_num in [*range(57, 72), *range(89, 104)]  # rare earths
+                # Check if data is present for f-block elements
+                if (elem := Element.from_Z(atom_num).symbol) in self.data.index
+                and len(self.data.loc[elem, Key.heat_val]) > 0
+            }
+            self._hide_f_block = not bool(f_block_elements_with_data)
+
+        else:
+            self._hide_f_block = hide_f_block
+
+    @property
+    def elem_types(self) -> set[str]:
+        """Element types present in data."""
+        return set(df_ptable.loc[self.data.index, "type"])
+
+    @property
+    def elem_type_colors(self) -> dict[str, str]:
+        """Element type based colors.
+
+        Example:
+            dict(Nonmetal="green", Halogen="teal", Metal="lightblue")
+        """
+        return self._elem_type_colors or {}
+
+    @elem_type_colors.setter
+    def elem_type_colors(self, elem_type_colors: dict[str, str]) -> None:
+        self._elem_type_colors |= elem_type_colors or {}
+
+    @property
+    def elem_colors(self) -> dict[str, Any]:
+        """Element-based colors."""
+        return self._elem_colors
+
+    @elem_colors.setter
+    def elem_colors(self, elem_colors: dict[str, Any] | None) -> None:
+        # TODO: set default colors
+        # TODO: what is the type of values (str, tuple[float, ...] or both)
+        self._elem_colors = elem_colors or {}
+
+    def get_elem_type_color(
+        self,
+        elem_symbol: str,
+        default: str = "white",
+    ) -> str:
+        """Get element type color by element symbol."""
+        elem_type = df_ptable.loc[elem_symbol].get("type", None)
+        return self.elem_type_colors.get(elem_type, default)
+
     def add_child_plots(
         self,
-        child_plotter: Callable[[plt.axes, Any], None],
-        child_args: dict[str, Any],
+        child_plotter: Callable[..., None],
         *,
-        ax_kwargs: dict[str, Any],
+        child_kwargs: dict[str, Any] | None = None,
+        tick_kwargs: dict[str, Any] | None = None,
+        ax_kwargs: dict[str, Any] | None = None,
         on_empty: Literal["hide", "show"] = "hide",
     ) -> None:
         """Add custom child plots to the periodic table grid.
 
         Args:
             child_plotter: A callable for the child plotter.
-            child_args: Arguments to pass to the child plotter call.
+            child_kwargs: Arguments to pass to the child plotter call.
+            tick_kwargs: kwargs to pass to ax.tick_params().
             ax_kwargs: Keyword arguments to pass to ax.set().
             on_empty: Whether to "show" or "hide" tiles for elements without data.
         """
+        # Update kwargs
+        child_kwargs = child_kwargs or {}
+        ax_kwargs = ax_kwargs or {}
+        tick_kwargs = {"axis": "both", "which": "major", "labelsize": 8} | (
+            tick_kwargs or {}
+        )
+
         for element in Element:
             # Hide f-block
             if self.hide_f_block and (element.is_lanthanoid or element.is_actinoid):
                 continue
 
             # Get axis index by element symbol
             symbol: str = element.symbol
@@ -442,122 +355,193 @@
             except KeyError:  # skip element without data
                 plot_data = None
 
             if (plot_data is None or len(plot_data) == 0) and on_empty == "hide":
                 continue
 
             # Call child plotter
-            child_plotter(ax, plot_data, **child_args)
+            child_plotter(ax, plot_data, tick_kwargs=tick_kwargs, **child_kwargs)
 
             # Pass axis kwargs
             if ax_kwargs:
                 ax.set(**ax_kwargs)
 
-    def add_ele_symbols(
+    def add_elem_symbols(
         self,
         text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+        *,
         pos: tuple[float, float] = (0.5, 0.5),
+        text_color: str = "black",
         kwargs: dict[str, Any] | None = None,
     ) -> None:
         """Add element symbols for each tile.
 
         Args:
             text (str | Callable): The text to add to the tile.
-                If a callable, it should accept a pymatgen Element object and return a
+                If a callable, it should accept a pymatgen Element and return a
                 string. If a string, it can contain a format
                 specifier for an `elem` variable which will be replaced by the element.
-            pos: The position of the text relative to the axes.
-            kwargs: Additional keyword arguments to pass to the `ax.text`.
+            pos (tuple): The position of the text relative to the axes.
+            text_color (bool): The color of the text. Defaults to "black".
+                Pass "element-type" to color symbol by self.elem_type_colors.
+            kwargs (dict): Additional keyword arguments to pass to the `ax.text`.
         """
-        # Update symbol args
+        # Update symbol kwargs
         kwargs = kwargs or {}
-        kwargs.setdefault("fontsize", 18)
+        kwargs.setdefault("fontsize", 12)
 
         # Add symbol for each element
         for element in Element:
             # Hide f-block
             if self.hide_f_block and (element.is_lanthanoid or element.is_actinoid):
                 continue
 
             # Get axis index by element symbol
             symbol: str = element.symbol
             row, column = df_ptable.loc[symbol, ["row", "column"]]
             ax: plt.Axes = self.axes[row - 1][column - 1]
 
-            anno = text(element) if callable(text) else text.format(elem=element)
+            content = text(element) if callable(text) else text.format(elem=element)
+
+            elem_type_color = self.get_elem_type_color(symbol, default=text_color)
             ax.text(
-                *pos, anno, ha="center", va="center", transform=ax.transAxes, **kwargs
+                *pos,
+                content,
+                color=elem_type_color if text_color == "element-type" else text_color,
+                ha="center",
+                va="center",
+                transform=ax.transAxes,
+                **kwargs,
             )
 
     def add_colorbar(
         self,
         title: str,
-        coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
         *,
+        coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
         cbar_kwargs: dict[str, Any] | None = None,
         title_kwargs: dict[str, Any] | None = None,
     ) -> None:
         """Add a global colorbar.
 
         Args:
             title: Title for the colorbar.
             coords: Coordinates of the colorbar (left, bottom, width, height).
-                    Defaults to (0.18, 0.8, 0.42, 0.02).
+                Defaults to (0.18, 0.8, 0.42, 0.02).
             cbar_kwargs: Additional keyword arguments to pass to fig.colorbar().
             title_kwargs: Additional keyword arguments for the colorbar title.
         """
-        # Update colorbar args
+        # Update colorbar kwargs
         cbar_kwargs = {"orientation": "horizontal"} | (cbar_kwargs or {})
+        title_kwargs = {"fontsize": 12, "pad": 10, "label": title} | (
+            title_kwargs or {}
+        )
 
         # Check colormap
         if self.cmap is None:
-            raise ValueError("Cannot add colorbar without colormap.")
+            raise ValueError("Cannot add colorbar without a colormap.")
 
         # Add colorbar
         cbar_ax = self.fig.add_axes(coords)
 
         self.fig.colorbar(
             plt.cm.ScalarMappable(norm=self._norm, cmap=self.cmap),
             cax=cbar_ax,
             **cbar_kwargs,
         )
 
         # Set colorbar title
-        title_kwargs = title_kwargs or {}
-        title_kwargs.setdefault("fontsize", 12)
-        title_kwargs.setdefault("pad", 10)
-        title_kwargs["label"] = title
-
         cbar_ax.set_title(**title_kwargs)
 
+    def add_elem_type_legend(
+        self,
+        kwargs: dict[str, Any] | None,
+    ) -> None:
+        """Add a legend to show the colors based on element types.
+
+        Args:
+            kwargs (dict | None): Keyword arguments passed to
+                plt.legend() for customizing legend appearance.
+        """
+        kwargs = kwargs or {}
+
+        font_size = 10
+
+        # Get present elements
+        legend_elements = [
+            plt.Line2D(
+                *([0], [0]),
+                marker="s",
+                color="w",
+                label=elem_class,
+                markerfacecolor=color,
+                markersize=1.2 * font_size,
+            )
+            for elem_class, color in self.elem_type_colors.items()
+            if elem_class in self.elem_types
+        ]
+
+        default_legend_kwargs = dict(
+            loc="center left",
+            bbox_to_anchor=(0, -42),
+            ncol=6,
+            frameon=False,
+            fontsize=font_size,
+            handlelength=1,  # more compact legend
+        )
+        kwargs = default_legend_kwargs | kwargs
+
+        plt.legend(handles=legend_elements, **kwargs)
+
+    def set_elem_background_color(self, alpha: float = 0.1) -> None:
+        """Set element tile background color by element type.
+
+        Args:
+            alpha (float): transparency
+        """
+        for element in Element:
+            # Hide f-block
+            if self.hide_f_block and (element.is_lanthanoid or element.is_actinoid):
+                continue
+
+            # Get element axis
+            symbol = element.symbol
+            row, column = df_ptable.loc[symbol, ["row", "column"]]
+            ax: plt.Axes = self.axes[row - 1][column - 1]
+
+            # Set background color by element type
+            rgb = mpl.colors.to_rgb(self.get_elem_type_color(symbol))
+            ax.set_facecolor((*rgb, alpha))
+
 
 class ChildPlotters:
-    """Collect some pre-defined child plotters."""
+    """Collection of pre-defined child plotters."""
 
     @staticmethod
     def rectangle(
         ax: plt.axes,
         data: SupportedValueType,
         norm: Normalize,
         cmap: Colormap,
         start_angle: float,
+        tick_kwargs: dict[str, Any],  # noqa: ARG004
     ) -> None:
         """Rectangle heatmap plotter, could be evenly split.
 
         Could be evenly split, depending on the
         length of the data (could mix and match).
 
         Args:
             ax (plt.axes): The axis to plot on.
-            data (SupportedValueType): The values for to
-                the child plotter.
+            data (SupportedValueType): The values for the child plotter.
             norm (Normalize): Normalizer for data-color mapping.
             cmap (Colormap): Colormap used for value mapping.
             start_angle (float): The starting angle for the splits in degrees,
                 and the split proceeds counter-clockwise (0 refers to the x-axis).
+            tick_kwargs: For compatibility with other plotters.
         """
         # Map values to colors
         if isinstance(data, (Sequence, np.ndarray)):
             colors = [cmap(norm(value)) for value in data]
         else:
             raise TypeError("Unsupported data type.")
 
@@ -576,66 +560,131 @@
         ax.set_xlim(-0.5, 0.5)
         ax.set_ylim(-0.5, 0.5)
 
     @staticmethod
     def scatter(
         ax: plt.axes,
         data: SupportedValueType,
-        **child_args: Any,
+        tick_kwargs: dict[str, Any],
+        **child_kwargs: Any,
     ) -> None:
         """Scatter plotter.
 
         Args:
             ax (plt.axes): The axis to plot on.
-            data (SupportedValueType): The values for to
-                the child plotter.
-            child_args (dict): args to pass to the child plotter call
+            data (SupportedValueType): The values for the child plotter.
+            child_kwargs (dict): kwargs to pass to the child plotter call.
+            tick_kwargs (dict): kwargs to pass to ax.tick_params().
         """
         # Add scatter
         if len(data) == 2:
-            ax.scatter(x=data[0], y=data[1], **child_args)
+            ax.scatter(x=data[0], y=data[1], **child_kwargs)
         elif len(data) == 3:
-            ax.scatter(x=data[0], y=data[1], c=data[2], **child_args)
+            ax.scatter(x=data[0], y=data[1], c=data[2], **child_kwargs)
 
-        # Adjust tick labels
-        # TODO: how to achieve this from external?
-        ax.tick_params(axis="both", which="major", labelsize=8)
+        # Set tick labels
+        ax.tick_params(**tick_kwargs)
 
         # Hide the right and top spines
         ax.axis("on")  # turned off by default
         ax.spines[["right", "top"]].set_visible(False)
 
     @staticmethod
     def line(
         ax: plt.axes,
         data: SupportedValueType,
-        **child_args: Any,
+        tick_kwargs: dict[str, Any],
+        **child_kwargs: Any,
     ) -> None:
         """Line plotter.
 
         Args:
             ax (plt.axes): The axis to plot on.
-            data (SupportedValueType): The values for to
-                the child plotter.
-            child_args (dict): args to pass to the child plotter call
+            data (SupportedValueType): The values for the child plotter.
+            child_kwargs (dict): kwargs to pass to the child plotter call.
+            tick_kwargs (dict): kwargs to pass to ax.tick_params().
         """
         # Add line
-        ax.plot(data[0], data[1], **child_args)
+        ax.plot(data[0], data[1], **child_kwargs)
 
-        # Adjust tick labels
-        # TODO: how to achieve this from external?
-        ax.tick_params(axis="both", which="major", labelsize=8)
+        # Set tick labels
+        ax.tick_params(**tick_kwargs)
 
         # Hide the right and top spines
         ax.axis("on")  # turned off by default
         ax.spines[["right", "top"]].set_visible(False)
 
+    @staticmethod
+    def histogram(
+        ax: plt.axes,
+        data: SupportedValueType,
+        cmap: Colormap,
+        cbar_axis: Literal["x", "y"],
+        tick_kwargs: dict[str, Any],
+        **child_kwargs: Any,
+    ) -> None:
+        """Histogram plotter.
+
+        Taken from https://stackoverflow.com/questions/23061657/
+        plot-histogram-with-colors-taken-from-colormap
+
+        Args:
+            ax (plt.axes): The axis to plot on.
+            data (SupportedValueType): The values for the child plotter.
+            cmap (Colormap): Colormap.
+            cbar_axis (Literal["x", "y"]): The axis colormap
+                would be based on.
+            child_kwargs: kwargs to pass to the child plotter call.
+            tick_kwargs (dict): kwargs to pass to ax.tick_params().
+        """
+        # Preprocess x_range if only one boundary is given
+        x_range = child_kwargs.pop("range", None)
+
+        if x_range is None or x_range == [None, None]:
+            x_range = [np.min(data), np.max(data)]
+
+        elif x_range[0] is None:
+            x_range = [np.min(data), x_range[1]]
+
+        else:
+            x_range = [x_range[0], np.max(data)]
+
+        # Add histogram
+        n, bins, patches = ax.hist(data, range=x_range, **child_kwargs)
+
+        # Scale values according to axis
+        if cbar_axis == "x":
+            bin_centers = 0.5 * (bins[:-1] + bins[1:])
+
+            cols = bin_centers - min(bin_centers)
+            cols /= max(cols)
+
+        else:
+            cols = (n - n.min()) / (n.max() - n.min())
+
+        # Apply colors
+        for col, patch in zip(cols, patches):
+            plt.setp(patch, "facecolor", cmap(col))
+
+        # Set tick labels
+        ax.tick_params(**tick_kwargs)
+        ax.set_yticklabels([])
+        ax.set_yticks([])
+
+        # Hide the right, left and top spines
+        ax.axis("on")
+        ax.spines[["right", "top", "left"]].set_visible(False)
+
+        # Set x-ticks to min/max only
+        ax.set_xticks([math.floor(x_range[0]), math.ceil(x_range[1])])
+
 
 def ptable_heatmap(
     values: ElemValues,
+    *,
     log: bool | Normalize = False,
     ax: plt.Axes | None = None,
     count_mode: CountMode = Key.composition,
     cbar_title: str = "Element Count",
     cbar_range: tuple[float | None, float | None] | None = None,
     cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.05),
     cbar_kwargs: dict[str, Any] | None = None,
@@ -755,27 +804,28 @@
             "Combining log color scale and heat_mode='fraction'/'percent' unsupported"
         )
     if "cmap" in kwargs:
         colorscale = kwargs.pop("cmap")
         warnings.warn(
             "cmap argument is deprecated, use colorscale instead",
             category=DeprecationWarning,
+            stacklevel=2,
         )
 
     values = count_elements(values, count_mode, exclude_elements)
 
     # replace positive and negative infinities with NaN values, then drop all NaNs
     clean_vals = values.replace([np.inf, -np.inf], np.nan).dropna()
 
     if heat_mode in ("fraction", "percent"):
         # ignore inf values in sum() else all would be set to 0 by normalizing
         values /= clean_vals.sum()
         clean_vals /= clean_vals.sum()  # normalize as well for norm.autoscale() below
 
-    color_map = get_cmap(colorscale)
+    color_map = plt.get_cmap(colorscale)
 
     n_rows = df_ptable.row.max()
     n_columns = df_ptable.column.max()
 
     # TODO can we pass as a kwarg and still ensure aspect ratio respected?
     fig = plt.figure(figsize=(0.75 * n_columns, 0.7 * n_rows), **kwargs)
 
@@ -821,20 +871,15 @@
         elif tile_value == 0:
             color = zero_color
             label = str(zero_symbol)
         else:
             color = color_map(norm(tile_value))
 
             if callable(fmt):
-                if len(inspect.signature(fmt).parameters) == 2:
-                    # 2nd arg=0 needed for matplotlib which always passes 2 positional
-                    # args to fmt()
-                    label = fmt(tile_value, 0)
-                else:
-                    label = fmt(tile_value)
+                label = fmt(tile_value)
 
             elif heat_mode == "percent":
                 label = f"{tile_value:{fmt or '.1f'}}"
             else:
                 fmt = fmt or (".0f" if tile_value > 100 else ".1f")
                 label = f"{tile_value:{fmt}}"
             # replace shortens scientific notation 1e+01 to 1e1 so it fits inside cells
@@ -883,139 +928,145 @@
             )
 
         ax.add_patch(rect)
 
     if heat_mode is not None and show_scale:
         # colorbar position and size: [x, y, width, height]
         # anchored at lower left corner
-        cbar_ax = ax.inset_axes(cbar_coords, transform=ax.transAxes)
+        cbar_kwargs = cbar_kwargs or {}
+        cbar_ax = cbar_kwargs.pop("cax", None) or ax.inset_axes(
+            cbar_coords, transform=ax.transAxes
+        )
         # format major and minor ticks
         # TODO maybe give user direct control over labelsize, instead of hard-coding
         # 8pt smaller than default
         cbar_ax.tick_params(which="both", labelsize=text_style["fontsize"])
 
         mappable = plt.cm.ScalarMappable(norm=norm, cmap=colorscale)
 
         if callable(cbar_fmt):
-            tick_fmt = cbar_fmt
+            # 2nd _pos arg is always passed by matplotlib but we don't need it
+            tick_fmt = lambda val, _pos: cbar_fmt(val)
 
-        cbar_kwargs = cbar_kwargs or {}
         cbar = fig.colorbar(
             mappable,
-            cax=cbar_kwargs.pop("cax", cbar_ax),
+            cax=cbar_ax,
             orientation=cbar_kwargs.pop("orientation", "horizontal"),
             format=cbar_kwargs.pop("format", tick_fmt),
             **cbar_kwargs,
         )
 
         cbar.outline.set_linewidth(1)
+        if text_style.get("color") == "white":
+            text_style.pop("color")  # don't want to apply possibly 'white' default
+            # text color (depending on colorscale) to color bar with white background
         cbar_ax.set_title(cbar_title, pad=10, **text_style)
 
     plt.ylim(0.3, n_rows + 0.1)
     plt.xlim(0.9, n_columns + 1)
 
     plt.axis("off")
     return ax
 
 
 def ptable_heatmap_splits(
     data: pd.DataFrame | pd.Series | dict[str, list[list[float]]],
-    colormap: str | None = None,
+    *,
+    # Heatmap-split specific
     start_angle: float = 135,
-    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
-    symbol_pos: tuple[float, float] = (0.5, 0.5),
-    cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
-    cbar_title: str = "Values",
+    # Figure-scope
+    colormap: str | Colormap = "viridis",
     on_empty: Literal["hide", "show"] = "hide",
     hide_f_block: bool | None = None,
-    ax_kwargs: dict[str, Any] | None = None,
-    symbol_kwargs: dict[str, Any] | None = None,
     plot_kwargs: dict[str, Any]
     | Callable[[Sequence[float]], dict[str, Any]]
     | None = None,
+    # Axis-scope
+    ax_kwargs: dict[str, Any] | None = None,
+    # Symbol
+    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    symbol_pos: tuple[float, float] = (0.5, 0.5),
+    symbol_kwargs: dict[str, Any] | None = None,
+    # Colorbar
+    cbar_title: str = "Values",
     cbar_title_kwargs: dict[str, Any] | None = None,
+    cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
     cbar_kwargs: dict[str, Any] | None = None,
 ) -> plt.Figure:
     """Plot evenly-split heatmaps, nested inside a periodic table.
 
     Args:
         data (pd.DataFrame | pd.Series | dict[str, list[list[float]]]):
             Map from element symbols to plot data. E.g. if dict,
             {"Fe": [1, 2], "Co": [3, 4]}, where the 1st value would
             be plotted on the lower-left corner and the 2nd on the upper-right.
             If pd.Series, index is element symbols and values lists.
             If pd.DataFrame, column names are element symbols,
             plots are created from each column.
-        colormap (str): Matplotlib colormap name to use.
         start_angle (float): The starting angle for the splits in degrees,
                 and the split proceeds counter-clockwise (0 refers to
                 the x-axis). Defaults to 135 degrees.
+        colormap (str): Matplotlib colormap name to use.
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
         ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
             Use to set x/y labels, limits, etc. Defaults to None. Example:
             dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
             ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
             https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
         symbol_text (str | Callable[[Element], str]): Text to display for
             each element symbol. Defaults to lambda elem: elem.symbol.
-        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
-            element symbols. Defaults to None.
         symbol_pos (tuple[float, float]): Position of element symbols
             relative to the lower left corner of each tile.
             Defaults to (0.5, 0.5). (1, 1) is the upper right corner.
-        cbar_coords (tuple[float, float, float, float]): Colorbar
-            position and size: [x, y, width, height] anchored at lower left
-            corner of the bar. Defaults to (0.25, 0.77, 0.35, 0.02).
+        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
+            element symbols. Defaults to None.
+
         cbar_title (str): Colorbar title. Defaults to "Values".
         cbar_title_kwargs (dict): Keyword arguments passed to
             cbar.ax.set_title(). Defaults to dict(fontsize=12, pad=10).
+        cbar_coords (tuple[float, float, float, float]): Colorbar
+            position and size: [x, y, width, height] anchored at lower left
+            corner of the bar. Defaults to (0.25, 0.77, 0.35, 0.02).
         cbar_kwargs (dict): Keyword arguments passed to fig.colorbar().
-        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
-            data. Defaults to "hide".
-        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
-            None, meaning hide if no data is provided for f-block elements.
-        plot_kwargs (dict): Additional keyword arguments to
-                pass to the plt.subplots function call.
 
     Notes:
         Default figsize is set to (0.75 * n_groups, 0.75 * n_periods).
 
     Returns:
         plt.Figure: periodic table with a subplot in each element tile.
     """
-    # Re-initialize kwargs as empty dict if None
-    plot_kwargs = plot_kwargs or {}
-    ax_kwargs = ax_kwargs or {}
-    symbol_kwargs = symbol_kwargs or {}
-    cbar_title_kwargs = cbar_title_kwargs or {}
-    cbar_kwargs = cbar_kwargs or {}
-
     # Initialize periodic table plotter
     plotter = PTableProjector(
         data=data,
         colormap=colormap,
         plot_kwargs=plot_kwargs,  # type: ignore[arg-type]
         hide_f_block=hide_f_block,
     )
 
     # Call child plotter: evenly split rectangle
-    child_args = {
+    child_kwargs = {
         "start_angle": start_angle,
         "cmap": plotter.cmap,
         "norm": plotter.norm,
     }
 
     plotter.add_child_plots(
-        ChildPlotters.rectangle,  # type: ignore[arg-type]
-        child_args=child_args,
+        ChildPlotters.rectangle,
+        child_kwargs=child_kwargs,
         ax_kwargs=ax_kwargs,
         on_empty=on_empty,
     )
 
     # Add element symbols
-    plotter.add_ele_symbols(
+    plotter.add_elem_symbols(
         text=symbol_text,
         pos=symbol_pos,
         kwargs=symbol_kwargs,
     )
 
     # Add colorbar
     plotter.add_colorbar(
@@ -1027,14 +1078,15 @@
 
     return plotter.fig
 
 
 def ptable_heatmap_ratio(
     values_num: ElemValues,
     values_denom: ElemValues,
+    *,
     count_mode: CountMode = Key.composition,
     normalize: bool = False,
     cbar_title: str = "Element Ratio",
     not_in_numerator: tuple[str, str] | None = ("#eff", "gray: not in 1st list"),
     not_in_denominator: tuple[str, str] | None = (
         "lightskyblue",
         "blue: not in 2nd list",
@@ -1093,14 +1145,15 @@
         plt.text(0.8, y_pos, txt, fontsize=10, bbox=bbox)
 
     return ptable_heatmap(values, cbar_title=cbar_title, **kwargs)
 
 
 def ptable_heatmap_plotly(
     values: ElemValues,
+    *,
     count_mode: CountMode = Key.composition,
     colorscale: str | Sequence[str] | Sequence[tuple[float, str]] = "viridis",
     show_scale: bool = True,
     show_values: bool = True,
     heat_mode: Literal["value", "fraction", "percent"] | None = "value",
     fmt: str | None = None,
     hover_props: Sequence[str] | dict[str, str] | None = None,
@@ -1351,381 +1404,364 @@
 
     fig.update_traces(colorbar=dict(lenmode="fraction", thickness=15, **color_bar))
     return fig
 
 
 def ptable_hists(
     data: pd.DataFrame | pd.Series | dict[str, list[float]],
+    *,
+    # Histogram-specific
     bins: int = 20,
-    colormap: str | None = None,
-    hist_kwds: dict[str, Any]
+    x_range: tuple[float | None, float | None] | None = None,
+    log: bool = False,
+    # Figure-scope
+    colormap: str | Colormap | None = "viridis",
+    on_empty: Literal["show", "hide"] = "hide",
+    hide_f_block: bool | None = None,
+    plot_kwargs: dict[str, Any] | None = None,
+    # Axis-scope
+    ax_kwargs: dict[str, Any] | None = None,
+    child_kwargs: dict[str, Any]
     | Callable[[Sequence[float]], dict[str, Any]]
     | None = None,
-    cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
-    x_range: tuple[float | None, float | None] | None = None,
-    symbol_kwargs: Any = None,
-    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    # Colorbar
+    cbar_axis: Literal["x", "y"] = "x",
     cbar_title: str = "Values",
-    cbar_title_kwds: dict[str, Any] | None = None,
-    cbar_kwds: dict[str, Any] | None = None,
+    cbar_title_kwargs: dict[str, Any] | None = None,
+    cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
+    cbar_kwargs: dict[str, Any] | None = None,
+    # Symbol
     symbol_pos: tuple[float, float] = (0.5, 0.8),
-    log: bool = False,
-    anno_kwds: dict[str, Any] | None = None,
-    on_empty: Literal["show", "hide"] = "hide",
-    color_elem_types: Literal["symbol", "background", "both", False]
-    | dict[str, str] = "background",
-    elem_type_legend: bool | dict[str, Any] = True,
-    **kwargs: Any,
+    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    symbol_kwargs: dict[str, Any] | None = None,
+    # Element types based colors and legend
+    color_elem_strategy: Literal["symbol", "background", "both", "off"] = "background",
+    elem_type_colors: dict[str, str] | None = None,
+    add_elem_type_legend: bool = False,
+    elem_type_legend_kwargs: dict[str, Any] | None = None,
 ) -> plt.Figure:
-    """Plot small histograms for each element laid out in a periodic table.
+    """Plot histograms for each element laid out in a periodic table.
 
     Args:
         data (pd.DataFrame | pd.Series | dict[str, list[float]]): Map from element
             symbols to histogram values. E.g. if dict, {"Fe": [1, 2, 3], "O": [4, 5]}.
             If pd.Series, index is element symbols and values lists. If pd.DataFrame,
             column names are element symbols histograms are plotted from each column.
+
         bins (int): Number of bins for the histograms. Defaults to 20.
-        colormap (str): Matplotlib colormap name to use. Defaults to None. See options
-            at https://matplotlib.org/stable/users/explain/colors/colormaps.
-        hist_kwds (dict | Callable): Keywords passed to ax.hist() for each histogram.
+        x_range (tuple[float | None, float | None]): x-axis range for all histograms.
+            Defaults to None.
+        log (bool): Whether to log scale y-axis of each histogram. Defaults to False.
+
+        colormap (str): Matplotlib colormap name to use. Defaults to 'viridis'. See
+            options at https://matplotlib.org/stable/users/explain/colors/colormaps.
+        on_empty ("hide" | "show"): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        plot_kwargs (dict): Additional keyword arguments to
+            pass to the plt.subplots function call.
+
+        ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
+            Use to set x/y labels, limits, etc. Defaults to None. Example:
+            dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
+            ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
+            https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
+        child_kwargs (dict | Callable): Keywords passed to ax.hist() for each histogram.
             If callable, it is called with the histogram values for each element and
             should return a dict of keyword arguments. Defaults to None.
+
+        cbar_axis (Literal["x", "y"]): The axis colormap would be based on.
+        cbar_title (str): Color bar title. Defaults to "Histogram Value".
+        cbar_title_kwargs (dict): Keyword arguments passed to cbar.ax.set_title().
+            Defaults to dict(fontsize=12, pad=10).
         cbar_coords (tuple[float, float, float, float]): Color bar position and size:
             [x, y, width, height] anchored at lower left corner of the bar. Defaults to
             (0.25, 0.77, 0.35, 0.02).
-        x_range (tuple[float | None, float | None]): x-axis range for all histograms.
-            Defaults to None.
+        cbar_kwargs (dict): Keyword arguments passed to fig.colorbar().
+
+        symbol_pos (tuple[float, float]): Position of element symbols relative to the
+            lower left corner of each tile. Defaults to (0.5, 0.8). (1, 1) is the upper
+            right corner.
         symbol_text (str | Callable[[Element], str]): Text to display for each element
             symbol. Defaults to lambda elem: elem.symbol.
         symbol_kwargs (dict): Keyword arguments passed to plt.text() for element
             symbols. Defaults to None.
-        cbar_title (str): Color bar title. Defaults to "Histogram Value".
-        cbar_title_kwds (dict): Keyword arguments passed to cbar.ax.set_title().
-            Defaults to dict(fontsize=12, pad=10).
-        cbar_kwds (dict): Keyword arguments passed to fig.colorbar().
-        symbol_pos (tuple[float, float]): Position of element symbols relative to the
-            lower left corner of each tile. Defaults to (0.5, 0.8). (1, 1) is the upper
-            right corner.
-        log (bool): Whether to log scale y-axis of each histogram. Defaults to False.
-        anno_kwds (dict): Keyword arguments passed to plt.annotate() for element
-            annotations. Defaults to None. Useful for adding e.g. number of data points
-            in each histogram. For that, use
-            anno_kwds=lambda hist_vals: dict(text=len(hist_vals)).
-            Recognized keys are text, xy, xycoords, fontsize, and any other
-            plt.annotate() keywords.
-        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
-            data. Defaults to "hide".
-        color_elem_types ('symbol' | 'background' | 'both' | False | dict): Whether to
+
+        color_elem_strategy ("symbol" | "background" | "both" | "off"): Whether to
             color element symbols, tile backgrounds, or both based on element type.
-            If dict, it should map element types to colors. Defaults to "background".
-        elem_type_legend (bool | dict): Whether to show a legend for element
-            types. Defaults to True. If dict, used as kwargs to plt.legend(), e.g. to
+            Defaults to "background".
+        elem_type_colors (dict | None): dict to map element types to colors.
+            None to use default element type colors.
+        add_elem_type_legend (bool): Whether to show a legend for element
+            types. Defaults to True.
+        elem_type_legend_kwargs (dict): kwargs to plt.legend(), e.g. to
             set the legend title, use {"title": "Element Types"}.
-        **kwargs: Additional keyword arguments passed to plt.subplots(). Defaults to
-            dict(figsize=(0.75 * n_columns, 0.75 * n_rows)) with n_columns/n_rows the
-            number of columns/rows in the periodic table.
 
     Returns:
         plt.Figure: periodic table with a histogram in each element tile.
     """
-    n_rows = df_ptable.row.max()
-    n_columns = df_ptable.column.max()
-
-    kwargs.setdefault("figsize", (0.75 * n_columns, 0.75 * n_rows))
-    fig, axes = plt.subplots(n_rows, n_columns, **kwargs)
-
-    # Use series name as color bar title if available if no title was passed
-    if isinstance(data, pd.Series) and cbar_title == "Values" and data.name:
-        cbar_title = data.name
-        data = data.to_dict()
-
-    elif isinstance(data, pd.DataFrame):
-        data = data.to_dict(orient="list")
-
-    if x_range is not None:
-        vmin, vmax = x_range
-    else:
-        flat_list = [
-            val
-            for sublist in (data.values() if isinstance(data, dict) else data)
-            for val in sublist
-        ]
-        vmin, vmax = min(flat_list), max(flat_list)
-    norm = Normalize(vmin=vmin, vmax=vmax)
+    # Initialize periodic table plotter
+    plotter = PTableProjector(
+        data=data,
+        colormap=colormap,
+        plot_kwargs=plot_kwargs,
+        hide_f_block=hide_f_block,
+        elem_type_colors=elem_type_colors,
+    )
 
-    cmap = None
-    if colormap:
-        cmap = plt.get_cmap(colormap) if isinstance(colormap, str) else colormap
-
-    # Turn off axis of subplots on the grid that don't correspond to elements
-    ax: plt.Axes
-    for ax in axes.flat:
-        ax.axis("off")
+    # Call child plotter: histogram
+    child_kwargs = {
+        "bins": bins,
+        "range": x_range,
+        "log": log,
+        "cbar_axis": cbar_axis,
+        "cmap": plotter.cmap,
+    }
 
-    elem_class_colors = ELEM_CLASS_COLORS | (
-        color_elem_types if isinstance(color_elem_types, dict) else {}
+    plotter.add_child_plots(
+        ChildPlotters.histogram,
+        child_kwargs=child_kwargs,
+        ax_kwargs=ax_kwargs,
+        on_empty=on_empty,
     )
 
-    symbol_kwargs = symbol_kwargs or {}
-    for element in Element:
-        symbol = element.symbol
-        row, group = df_ptable.loc[symbol, ["row", "column"]]
-
-        ax = axes[row - 1][group - 1]
-        symbol_kwargs.setdefault("fontsize", 10)
-        hist_data = data.get(symbol, [])
+    # Add element symbols
+    plotter.add_elem_symbols(
+        text=symbol_text,
+        pos=symbol_pos,
+        text_color="element-types"
+        if color_elem_strategy in {"both", "symbol"}
+        else "black",
+        kwargs=symbol_kwargs,
+    )
 
-        if len(hist_data) == 0 and on_empty == "hide":
-            continue
+    # Color element tile background
+    if color_elem_strategy in {"both", "background"}:
+        plotter.set_elem_background_color()
 
-        if color_elem_types:
-            elem_class = df_ptable.loc[symbol, "type"]
-            if color_elem_types in ("symbol", "both"):
-                symbol_kwargs["color"] = elem_class_colors.get(elem_class, "black")
-            if color_elem_types in ("background", "both"):
-                bg_color = elem_class_colors.get(elem_class, "white")
-                ax.set_facecolor((*mpl.colors.to_rgb(bg_color), 0.07))
-
-        ax.text(
-            *symbol_pos,
-            symbol_text(element)
-            if callable(symbol_text)
-            else symbol_text.format(elem=element),
-            ha="center",
-            va="center",
-            transform=ax.transAxes,
-            **symbol_kwargs,
-        )
-        ax.axis("on")  # re-enable axes of elements that exist
-
-        if anno_kwds:
-            defaults = dict(
-                text=lambda hist_vals: si_fmt_int(len(hist_vals)),
-                xy=(0.8, 0.8),
-                xycoords="axes fraction",
-                fontsize=8,
-                horizontalalignment="center",
-                verticalalignment="center",
-            )
-            if callable(anno_kwds):
-                annotation = anno_kwds(hist_data)
-            else:
-                annotation = anno_kwds
-                anno_text = anno_kwds.get("text")
-                if isinstance(anno_text, dict):
-                    anno_text = anno_text.get(symbol)
-                elif callable(anno_text):
-                    anno_text = anno_text(hist_data)
-                annotation["text"] = anno_text
-            ax.annotate(**(defaults | annotation))
-
-        if hist_data is not None:
-            hist_kwargs = hist_kwds(hist_data) if callable(hist_kwds) else hist_kwds
-            _n, bins_array, patches = ax.hist(
-                hist_data, bins=bins, log=log, range=x_range, **(hist_kwargs or {})
-            )
-            if x_range:
-                ax.set_xlim(x_range)
-            x_min, x_max = math.floor(min(bins_array)), math.ceil(max(bins_array))
-            x_ticks = list(x_range or [x_min, x_max])
-            if x_ticks[0] is None:
-                x_ticks[0] = x_min
-            if x_ticks[1] is None:
-                x_ticks[1] = x_max
-            if x_min < 0 < x_max:
-                # make sure we always show a mark at 0
-                x_ticks.insert(1, 0)
-
-            if cmap:
-                for patch, x_val in zip(patches, bins_array[:-1]):
-                    plt.setp(patch, "facecolor", cmap(norm(x_val)))
-            ax.set_xticks(x_ticks)
-            ax.tick_params(labelsize=8, direction="in")
-        else:  # disable ticks for elements without data
-            ax.set_xticks([])
-        ax.set_yticks([])  # disable y ticks for all elements
-
-        for side in ("left", "right", "top"):
-            ax.spines[side].set_visible(b=False)
-        # Hide y ticks
-        ax.tick_params(axis="y", which="both", length=0)
-
-    # Add color bar
-    if isinstance(cmap, Colormap):
-        cbar_ax = fig.add_axes(cbar_coords)
-        fig.colorbar(
-            plt.cm.ScalarMappable(norm=norm, cmap=cmap),
-            cax=cbar_ax,
-            **{"orientation": "horizontal"} | (cbar_kwds or {}),
+    # Add colorbar
+    if colormap is not None:
+        plotter.add_colorbar(
+            title=cbar_title,
+            coords=cbar_coords,
+            cbar_kwargs=cbar_kwargs,
+            title_kwargs=cbar_title_kwargs,
         )
-        # Set color bar title
-        cbar_title_kwds = cbar_title_kwds or {}
-        cbar_title_kwds.setdefault("fontsize", 12)
-        cbar_title_kwds.setdefault("pad", 10)
-        cbar_title_kwds["label"] = cbar_title
-        cbar_ax.set_title(**cbar_title_kwds)
-
-    if elem_type_legend and color_elem_types:
-        legend_kwargs = elem_type_legend if isinstance(elem_type_legend, dict) else {}
-        add_element_type_legend(
-            data=data, elem_class_colors=elem_class_colors, legend_kwargs=legend_kwargs
+
+    # Add element type legend
+    if add_elem_type_legend:
+        plotter.add_elem_type_legend(
+            kwargs=elem_type_legend_kwargs,
         )
 
-    return fig
+    return plotter.fig
 
 
 def ptable_scatters(
     data: pd.DataFrame | pd.Series | dict[str, list[list[float]]],
-    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
-    symbol_pos: tuple[float, float] = (0.5, 0.8),
+    *,
+    # Figure-scope
     on_empty: Literal["hide", "show"] = "hide",
     hide_f_block: bool | None = None,
     plot_kwargs: dict[str, Any]
     | Callable[[Sequence[float]], dict[str, Any]]
     | None = None,
-    child_args: dict[str, Any] | None = None,
+    # Axis-scope
     ax_kwargs: dict[str, Any] | None = None,
+    child_kwargs: dict[str, Any] | None = None,
+    # Symbol
+    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    symbol_pos: tuple[float, float] = (0.5, 0.8),
     symbol_kwargs: dict[str, Any] | None = None,
+    # Element types based colors and legend
+    color_elem_strategy: Literal["symbol", "background", "both", "off"] = "background",
+    elem_type_colors: dict[str, str] | None = None,
+    add_elem_type_legend: bool = False,
+    elem_type_legend_kwargs: dict[str, Any] | None = None,
 ) -> plt.Figure:
     """Make scatter plots for each element, nested inside a periodic table.
 
     Args:
         data (pd.DataFrame | pd.Series | dict[str, list[list[float]]]):
             Map from element symbols to plot data. E.g. if dict,
             {"Fe": [1, 2], "Co": [3, 4]}, where the 1st value would
             be plotted on the lower-left corner and the 2nd on the upper-right.
             If pd.Series, index is element symbols and values lists.
             If pd.DataFrame, column names are element symbols,
             plots are created from each column.
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
         ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
             Use to set x/y labels, limits, etc. Defaults to None. Example:
             dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
             ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
             https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
+        child_kwargs: Arguments to pass to the child plotter call.
+
         symbol_text (str | Callable[[Element], str]): Text to display for
             each element symbol. Defaults to lambda elem: elem.symbol.
-        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
-            element symbols. Defaults to None.
         symbol_pos (tuple[float, float]): Position of element symbols
             relative to the lower left corner of each tile.
             Defaults to (0.5, 0.5). (1, 1) is the upper right corner.
-        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
-            data. Defaults to "hide".
-        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
-            None, meaning hide if no data is provided for f-block elements.
-        child_args: Arguments to pass to the child plotter call.
-        plot_kwargs (dict): Additional keyword arguments to
-                pass to the plt.subplots function call.
+        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
+            element symbols. Defaults to None.
+
+        color_elem_strategy ("symbol" | "background" | "both" | "off"): Whether to
+            color element symbols, tile backgrounds, or both based on element type.
+            Defaults to "background".
+        elem_type_colors (dict | None): dict to map element types to colors.
+            None to use default element type colors.
+        add_elem_type_legend (bool): Whether to show a legend for element
+            types. Defaults to True.
+        elem_type_legend_kwargs (dict): kwargs to plt.legend(), e.g. to
+            set the legend title, use {"title": "Element Types"}.
 
     TODO: allow colormap with 3rd data dimension
     """
-    # Re-initialize kwargs as empty dict if None
-    plot_kwargs = plot_kwargs or {}
-    ax_kwargs = ax_kwargs or {}
-
-    child_args = child_args or {}
-
-    symbol_kwargs = symbol_kwargs or {}
-    symbol_kwargs.setdefault("fontsize", 12)
-
     # Initialize periodic table plotter
     plotter = PTableProjector(
         data=data,
         colormap=None,
         plot_kwargs=plot_kwargs,  # type: ignore[arg-type]
         hide_f_block=hide_f_block,
+        elem_type_colors=elem_type_colors,
     )
 
     # Call child plotter: Scatter
     plotter.add_child_plots(
         ChildPlotters.scatter,
-        child_args=child_args,
+        child_kwargs=child_kwargs,
         ax_kwargs=ax_kwargs,
         on_empty=on_empty,
     )
 
     # Add element symbols
-    plotter.add_ele_symbols(
+    plotter.add_elem_symbols(
         text=symbol_text,
         pos=symbol_pos,
+        text_color="element-types"
+        if color_elem_strategy in {"both", "symbol"}
+        else "black",
         kwargs=symbol_kwargs,
     )
 
+    # Color element tile background
+    if color_elem_strategy in {"both", "background"}:
+        plotter.set_elem_background_color()
+
+    # Add element type legend
+    if add_elem_type_legend:
+        plotter.add_elem_type_legend(
+            kwargs=elem_type_legend_kwargs,
+        )
+
     return plotter.fig
 
 
 def ptable_lines(
     data: pd.DataFrame | pd.Series | dict[str, list[list[float]]],
-    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
-    symbol_pos: tuple[float, float] = (0.5, 0.8),
+    *,
+    # Figure-scope
     on_empty: Literal["hide", "show"] = "hide",
     hide_f_block: bool | None = None,
     plot_kwargs: dict[str, Any]
     | Callable[[Sequence[float]], dict[str, Any]]
     | None = None,
-    child_args: dict[str, Any] | None = None,
+    # Axis-scope
     ax_kwargs: dict[str, Any] | None = None,
+    child_kwargs: dict[str, Any] | None = None,
+    # Symbol
     symbol_kwargs: dict[str, Any] | None = None,
+    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    symbol_pos: tuple[float, float] = (0.5, 0.8),
+    # Element types based colors and legend
+    color_elem_strategy: Literal["symbol", "background", "both", "off"] = "background",
+    elem_type_colors: dict[str, str] | None = None,
+    add_elem_type_legend: bool = False,
+    elem_type_legend_kwargs: dict[str, Any] | None = None,
 ) -> plt.Figure:
     """Line plots for each element, nested inside a periodic table.
 
     Args:
         data (pd.DataFrame | pd.Series | dict[str, list[list[float]]]):
             Map from element symbols to plot data. E.g. if dict,
             {"Fe": [1, 2], "Co": [3, 4]}, where the 1st value would
             be plotted on the lower-left corner and the 2nd on the upper-right.
             If pd.Series, index is element symbols and values lists.
             If pd.DataFrame, column names are element symbols,
             plots are created from each column.
+
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
+
         ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
             Use to set x/y labels, limits, etc. Defaults to None. Example:
             dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
             ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
             https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
+        child_kwargs: Arguments to pass to the child plotter call.
+
         symbol_text (str | Callable[[Element], str]): Text to display for
             each element symbol. Defaults to lambda elem: elem.symbol.
-        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
-            element symbols. Defaults to None.
         symbol_pos (tuple[float, float]): Position of element symbols
             relative to the lower left corner of each tile.
             Defaults to (0.5, 0.5). (1, 1) is the upper right corner.
-        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
-            data. Defaults to "hide".
-        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
-            None, meaning hide if no data is provided for f-block elements.
-        child_args: Arguments to pass to the child plotter call.
-        plot_kwargs (dict): Additional keyword arguments to
-                pass to the plt.subplots function call.
-    """
-    # Re-initialize kwargs as empty dict if None
-    plot_kwargs = plot_kwargs or {}
-    ax_kwargs = ax_kwargs or {}
-
-    child_args = child_args or {}
-
-    symbol_kwargs = symbol_kwargs or {}
-    symbol_kwargs.setdefault("fontsize", 12)
+        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
+            element symbols. Defaults to None.
 
+        color_elem_strategy ("symbol" | "background" | "both" | "off"): Whether to
+            color element symbols, tile backgrounds, or both based on element type.
+            Defaults to "background".
+        elem_type_colors (dict | None): dict to map element types to colors.
+            None to use default element type colors.
+        add_elem_type_legend (bool): Whether to show a legend for element
+            types. Defaults to True.
+        elem_type_legend_kwargs (dict): kwargs to plt.legend(), e.g. to
+            set the legend title, use {"title": "Element Types"}.
+    """
     # Initialize periodic table plotter
     plotter = PTableProjector(
         data=data,
         colormap=None,
         plot_kwargs=plot_kwargs,  # type: ignore[arg-type]
         hide_f_block=hide_f_block,
+        elem_type_colors=elem_type_colors,
     )
 
     # Call child plotter: line
     plotter.add_child_plots(
         ChildPlotters.line,
-        child_args=child_args,
+        child_kwargs=child_kwargs,
         ax_kwargs=ax_kwargs,
         on_empty=on_empty,
     )
 
     # Add element symbols
-    plotter.add_ele_symbols(
+    plotter.add_elem_symbols(
         text=symbol_text,
         pos=symbol_pos,
+        text_color="element-types"
+        if color_elem_strategy in {"both", "symbol"}
+        else "black",
         kwargs=symbol_kwargs,
     )
 
+    # Color element tile background
+    if color_elem_strategy in {"both", "background"}:
+        plotter.set_elem_background_color()
+
+    # Add element type legend
+    if add_elem_type_legend:
+        plotter.add_elem_type_legend(
+            kwargs=elem_type_legend_kwargs,
+        )
+
     return plotter.fig
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymatviz-0.8.2/pymatviz/relevance.py` & `pymatviz-0.8.3/pymatviz/relevance.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/pymatviz/sankey.py` & `pymatviz-0.8.3/pymatviz/sankey.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if TYPE_CHECKING:
     import pandas as pd
 
 
 def sankey_from_2_df_cols(
     df: pd.DataFrame,
     cols: list[str],
+    *,
     labels_with_counts: bool | Literal["percent"] = True,
     **kwargs: Any,
 ) -> go.Figure:
     """Plot two columns of a dataframe as a Plotly Sankey diagram.
 
     Args:
         df (pd.DataFrame): Pandas dataframe.
```

### Comparing `pymatviz-0.8.2/pymatviz/structure_viz.py` & `pymatviz-0.8.3/pymatviz/structure_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
             n1 = n2
 
     return lines, z_indices, unit_cell_lines
 
 
 def plot_structure_2d(
     struct: Structure,
+    *,
     ax: plt.Axes | None = None,
     rotation: str = "10x,10y,0z",
     atomic_radii: float | dict[str, float] | None = None,
     colors: dict[str, str | list[float]] | None = None,
     scale: float = 1,
     show_unit_cell: bool = True,
     show_bonds: bool | NearNeighbors = False,
@@ -222,16 +223,16 @@
         )
 
     # Default behavior in case of no user input: standardize if any fractional
     # coordinates are negative
     has_sites_outside_unit_cell = any(any(site.frac_coords < 0) for site in struct)
     if standardize_struct is False and has_sites_outside_unit_cell:
         warnings.warn(
-            "your structure has negative fractional coordinates, you may want to set "
-            "standardize=True",
+            "your structure has negative fractional coordinates but you passed "
+            f"{standardize_struct=}, you may want to set standardize_struct=True",
             UserWarning,
         )
     elif standardize_struct is None:
         standardize_struct = has_sites_outside_unit_cell
     if standardize_struct:
         struct = SpacegroupAnalyzer(struct).get_conventional_standard_structure()
 
@@ -243,19 +244,18 @@
     # perfect for disordered sites. Plotting wedges of different radii for disordered
     # sites is handled later.
     elements_at_sites = [str(site.species.elements[0].symbol) for site in struct]
 
     if atomic_radii is None or isinstance(atomic_radii, float):
         # atomic_radii is a scaling factor for the default set of radii
         atomic_radii = 0.7 * covalent_radii * (atomic_radii or 1)
-    else:
+    elif missing := set(elements_at_sites) - set(atomic_radii):
         # atomic_radii is assumed to be a map from element symbols to atomic radii
         # make sure all present elements are assigned a radius
-        if missing := set(elements_at_sites) - set(atomic_radii):
-            raise ValueError(f"atomic_radii is missing keys: {missing}")
+        raise ValueError(f"atomic_radii is missing keys: {missing}")
 
     radii_at_sites = np.array(
         [atomic_radii[el] for el in elements_at_sites]  # type: ignore[index]
     )
 
     # Generate lines for unit cell
     rotation_matrix = _angles_to_rotation_matrix(rotation)
@@ -398,14 +398,15 @@
                 ax.add_patch(path)
 
     if show_bonds:
         warnings.warn(
             "Warning: the show_bonds feature of plot_structure_2d() is experimental. "
             "Issues and PRs with improvements welcome.",
             category=ExperimentalWarning,
+            stacklevel=2,
         )
         if show_bonds is True:
             neighbor_strategy_cls = CrystalNN
         elif issubclass(show_bonds, NearNeighbors):
             neighbor_strategy_cls = show_bonds
         else:
             raise ValueError(
```

### Comparing `pymatviz-0.8.2/pymatviz/sunburst.py` & `pymatviz-0.8.3/pymatviz/sunburst.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     from collections.abc import Sequence
 
     import plotly.graph_objects as go
 
 
 def spacegroup_sunburst(
     data: Sequence[int | str] | pd.Series,
+    *,
     show_counts: Literal["value", "percent", False] = False,
     **kwargs: Any,
 ) -> go.Figure:
     """Generate a sunburst plot with crystal systems as the inner ring for a list of
     international space group numbers.
 
     Hint: To hide very small labels, set a uniformtext minsize and mode='hide'.
```

### Comparing `pymatviz-0.8.2/pymatviz/uncertainty.py` & `pymatviz-0.8.3/pymatviz/uncertainty.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from numpy.typing import ArrayLike
 
 
 def qq_gaussian(
     y_true: ArrayLike | str,
     y_pred: ArrayLike | str,
     y_std: ArrayLike | dict[str, ArrayLike] | str | Sequence[str],
+    *,
     df: pd.DataFrame | None = None,
     ax: plt.Axes | None = None,
     identity_line: bool | dict[str, Any] = True,
 ) -> plt.Axes:
     """Plot the Gaussian quantile-quantile (Q-Q) plot of one (passed as array) or
     multiple (passed as dict) sets of uncertainty estimates for a single pair of ground
     truth targets `y_true` and model predictions `y_pred`.
@@ -197,14 +198,15 @@
     return abs_err[y_std_sort].cumsum() / n_inc
 
 
 def error_decay_with_uncert(
     y_true: ArrayLike | str,
     y_pred: ArrayLike | str,
     y_std: ArrayLike | dict[str, ArrayLike] | str | Sequence[str],
+    *,
     df: pd.DataFrame | None = None,
     n_rand: int = 100,
     percentiles: bool = True,
     ax: plt.Axes | None = None,
 ) -> plt.Axes:
     """Plot for assessing the quality of uncertainty estimates. If a model's uncertainty
     is well calibrated, i.e. strongly correlated with its error, removing the most
```

### Comparing `pymatviz-0.8.2/pymatviz/utils.py` & `pymatviz-0.8.3/pymatviz/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,30 +27,30 @@
     R = TypeVar("R")
 
 PKG_DIR = dirname(__file__)
 ROOT = dirname(PKG_DIR)
 TEST_FILES = f"{ROOT}/tests/files"
 Backend = Literal["matplotlib", "plotly"]
 AxOrFig = Union[plt.Axes, plt.Figure, go.Figure]
-VALID_BACKENDS = mpl_key, plotly_key = get_args(Backend)
+VALID_BACKENDS = MPL_BACKEND, PLOTLY_BACKEND = get_args(Backend)
 CrystalSystem = Literal[
     "triclinic",
     "monoclinic",
     "orthorhombic",
     "tetragonal",
     "trigonal",
     "hexagonal",
     "cubic",
 ]
 
 
 elements_csv = f"{ROOT}/pymatviz/elements.csv"
 df_ptable = pd.read_csv(elements_csv, comment="#").set_index("symbol")
 
-ELEM_CLASS_COLORS: Final = {
+ELEM_TYPE_COLORS: Final = {
     "Diatomic Nonmetal": "green",
     "Noble Gas": "purple",
     "Alkali Metal": "red",
     "Alkaline Earth Metal": "orange",
     "Metalloid": "darkgreen",
     "Polyatomic Nonmetal": "teal",
     "Transition Metal": "blue",
@@ -89,16 +89,19 @@
 
 def pretty_label(key: str, backend: Backend) -> str:
     """Map metric keys to their pretty labels."""
     if backend not in VALID_BACKENDS:
         raise ValueError(f"Unexpected {backend=}, must be one of {VALID_BACKENDS}")
 
     symbol_mapping = {
-        "R2": {mpl_key: "$R^2$", plotly_key: "R<sup>2</sup>"},
-        "R2_adj": {mpl_key: "$R^2_{adj}$", plotly_key: "R<sup>2</sup><sub>adj</sub>"},
+        "R2": {MPL_BACKEND: "$R^2$", PLOTLY_BACKEND: "R<sup>2</sup>"},
+        "R2_adj": {
+            MPL_BACKEND: "$R^2_{adj}$",
+            PLOTLY_BACKEND: "R<sup>2</sup><sub>adj</sub>",
+        },
     }
 
     return symbol_mapping.get(key, {}).get(backend, key)
 
 
 def crystal_sys_from_spg_num(spg: float) -> CrystalSystem:
     """Get the crystal system for an international space group number."""
@@ -184,14 +187,15 @@
 
     return args  # type: ignore[return-value]
 
 
 def bin_df_cols(
     df_in: pd.DataFrame,
     bin_by_cols: Sequence[str],
+    *,
     group_by_cols: Sequence[str] = (),
     n_bins: int | Sequence[int] = 100,
     bin_counts_col: str = "bin_counts",
     kde_col: str = "",
     verbose: bool = True,
 ) -> pd.DataFrame:
     """Bin columns of a DataFrame.
@@ -311,14 +315,15 @@
     """
     light_bg = luminance(color) > text_color_threshold
     return "black" if light_bg else "white"
 
 
 def si_fmt(
     val: float,
+    *,
     fmt: str = ".1f",
     sep: str = "",
     binary: bool = False,
     decimal_threshold: float = 0.01,
 ) -> str:
     """Convert large numbers into human readable format using SI prefixes.
 
@@ -413,17 +418,17 @@
         color (str, optional): The color of the text. Defaults to "black".
         **kwargs: Additional arguments to pass to matplotlib's AnchoredText or plotly's
             fig.add_annotation().
 
     Returns:
         plt.Axes | plt.Figure | go.Figure: The annotated figure.
     """
-    backend = plotly_key if isinstance(fig, go.Figure) else mpl_key
+    backend = PLOTLY_BACKEND if isinstance(fig, go.Figure) else MPL_BACKEND
 
-    if backend == mpl_key:
+    if backend == MPL_BACKEND:
         ax = fig if isinstance(fig, plt.Axes) else plt.gca()
 
         defaults = dict(frameon=False, loc="upper left", prop=dict(color=color))
         text_box = AnchoredText(text, **(defaults | kwargs))
         ax.add_artist(text_box)
     elif isinstance(fig, go.Figure):
         defaults = dict(
```

### Comparing `pymatviz-0.8.2/pymatviz.egg-info/PKG-INFO` & `pymatviz-0.8.3/pymatviz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.8.2
+Version: 0.8.3
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -104,44 +104,46 @@
 
 ## Usage
 
 See the Jupyter notebooks under [`examples/`](examples) for how to use `pymatviz`. PRs with additional examples are welcome! 🙏
 
 |                                                                                                                        |                                                                                                                                       |                                      |
 | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
+| [mlff_phonons.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb)                         | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb)             | [![Launch Codespace]][codespace url] |
 | [matbench_dielectric_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)  | [![Launch Codespace]][codespace url] |
 | [mp_bimodal_e_form.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)               | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)        | [![Launch Codespace]][codespace url] |
 | [matbench_perovskites_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_perovskites_eda.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_perovskites_eda.ipynb) | [![Launch Codespace]][codespace url] |
 | [mprester_ptable.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb)                   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb)          | [![Launch Codespace]][codespace url] |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 [Launch Codespace]: https://img.shields.io/badge/Launch-Codespace-darkblue?logo=github
 [codespace url]: https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=340898532
 
 ## Periodic Table
 
 See [`pymatviz/ptable.py`](pymatviz/ptable.py). Heatmaps of the periodic table can be plotted both with `matplotlib` and `plotly`. `plotly` supports displaying additional data on hover or full interactivity through [Dash](https://plotly.com/dash).
 
-|                        [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                        |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
-| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
-|                                              ![ptable-heatmap]                                               |                        ![ptable-heatmap-ratio]                        |
-|                         [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                         | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
-|                                   ![ptable-heatmap-plotly-more-hover-data]                                   |                     ![ptable-heatmap-plotly-log]                      |
-|                       [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                        |              [`ptable_lines(data)`](pymatviz/ptable.py)               |
-|                                               ![ptable-hists]                                                |                            ![ptable-lines]                            |
-| [`ptable_heatmap_splits(data, colormap="coolwarm", start_angle=135, hide_f_block=True)`](pymatviz/ptable.py) |
-|                                           ![ptable-heatmap-splits]                                           |
+|                    [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                    |                   [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)                    |
+| :--------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------: |
+|                                          ![ptable-heatmap]                                           |                                       ![ptable-heatmap-ratio]                                       |
+|                     [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                     |                [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py)                |
+|                               ![ptable-heatmap-plotly-more-hover-data]                               |                                    ![ptable-heatmap-plotly-log]                                     |
+|                   [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                    |                             [`ptable_lines(data)`](pymatviz/ptable.py)                              |
+|                                           ![ptable-hists]                                            |                                           ![ptable-lines]                                           |
+| [`ptable_heatmap_splits(2_vals_per_elem, colormap="coolwarm", start_angle=135)`](pymatviz/ptable.py) | [`ptable_heatmap_splits(3_vals_per_elem, colormap="coolwarm", start_angle=90)`](pymatviz/ptable.py) |
+|                                      ![ptable-heatmap-splits-2]                                      |                                     ![ptable-heatmap-splits-3]                                      |
 
 [ptable-hists]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-hists.svg
 [ptable-lines]: https://github.com/janosh/pymatviz/raw/main/examples/diatomics/homo-nuclear-mace-medium.svg
-[ptable-heatmap-splits]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits.svg
+[ptable-heatmap-splits-2]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits-2.svg
+[ptable-heatmap-splits-3]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits-3.svg
 
 ## Phonons
 
-See [`pymatviz/phonons.py`](pymatviz/phonons.py).
+See [`examples/mlff_phonons.ipynb`](https://github.com/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb) for usage example.
 
 |           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           |             [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py)             |
 | :------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
 |                              ![phonon-bands]                               |                                ![phonon-dos]                                 |
 | [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) | [`plot_phonon_bands_and_dos(single_bands, single_dos)`](pymatviz/phonons.py) |
 |                      ![phonon-bands-and-dos-mp-2758]                       |                       ![phonon-bands-and-dos-mp-23907]                       |
```

### Comparing `pymatviz-0.8.2/pymatviz.egg-info/SOURCES.txt` & `pymatviz-0.8.3/pymatviz.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 license
 pyproject.toml
 readme.md
 pymatviz/__init__.py
+pymatviz/_preprocess_data.py
 pymatviz/correlation.py
 pymatviz/cumulative.py
 pymatviz/elements.csv
 pymatviz/enums.py
 pymatviz/histograms.py
 pymatviz/io.py
 pymatviz/parity.py
@@ -21,20 +22,22 @@
 pymatviz.egg-info/PKG-INFO
 pymatviz.egg-info/SOURCES.txt
 pymatviz.egg-info/dependency_links.txt
 pymatviz.egg-info/requires.txt
 pymatviz.egg-info/top_level.txt
 tests/test_correlation.py
 tests/test_cumulative.py
+tests/test_enums.py
 tests/test_histograms.py
 tests/test_init.py
 tests/test_io.py
 tests/test_parity.py
 tests/test_phonons.py
 tests/test_powerups.py
+tests/test_preprocess_data.py
 tests/test_ptable.py
 tests/test_readme.py
 tests/test_relevance.py
 tests/test_sankey.py
 tests/test_structure_viz.py
 tests/test_sunburst.py
 tests/test_uncertainty.py
```

### Comparing `pymatviz-0.8.2/pyproject.toml` & `pymatviz-0.8.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-[build-system]
-requires = ["setuptools>=61.2"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "pymatviz"
-version = "0.8.2"
+version = "0.8.3"
 description = "A toolkit for visualizations in materials informatics"
 authors = [{ name = "Janosh Riebesell", email = "janosh.riebesell@gmail.com" }]
 readme = "readme.md"
 license = { file = "license" }
 keywords = [
     "chemistry",
     "data visualization",
@@ -60,14 +56,18 @@
 
 [tool.setuptools.package-data]
 pymatviz = ["*.csv"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
+[build-system]
+requires = ["setuptools>=61.2"]
+build-backend = "setuptools.build_meta"
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-p no:warnings"
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
@@ -83,49 +83,50 @@
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "ANN101",
     "ANN102",
     "ANN401",
-    "B028",   # No explicit stacklevel keyword argument found
-    "C408",   # unnecessary-collection-call
+    "B028",    # No explicit stacklevel keyword argument found
+    "C408",    # unnecessary-collection-call
     "C901",
-    "COM812", # trailing comma missing
-    "D205",   # 1 blank line required between summary line and description
-    "E731",   # do not assign a lambda expression, use a def
+    "COM812",  # trailing comma missing
+    "D205",    # 1 blank line required between summary line and description
+    "E731",    # do not assign a lambda expression, use a def
     "EM101",
     "EM102",
     "ERA001",
-    "FBT001",
-    "FBT002",
     "FIX002",
     "ISC001",
-    "N806",   # non-lowercase-variable-in-function
+    "N806",    # non-lowercase-variable-in-function
     "NPY002",
-    "PLR",    # pylint refactor
-    "PT006",  # pytest-parametrize-names-wrong-type
-    "PT011",  # pytest-raises-too-broad
+    "PLR0911", # too-many-return-statements
+    "PLR0912", # too-many-branches
+    "PLR0913", # function-with-too-many-arguments
+    "PLR0915", # too-many-statements
+    "PLR2004", # magic-number-comparison
+    "PT006",   # pytest-parametrize-names-wrong-type
     "PTH",
-    "RUF001", # ambiguous-unicode-character-string
+    "RUF001",  # ambiguous-unicode-character-string
     "S311",
-    "SIM105", # Use contextlib.suppress() instead of try-except-pass
+    "SIM105",  # Use contextlib.suppress() instead of try-except-pass
     "TD",
     "TRY003",
 ]
 pydocstyle.convention = "google"
 isort.lines-after-imports = 2
 isort.split-on-trailing-comma = false
 
 [tool.ruff.format]
 docstring-code-format = true
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
-"tests/*" = ["D", "S101"]
+"tests/*" = ["D", "FBT001", "FBT002", "PLR2004", "S101"]
 # T201: print found
 # D100: Missing docstring in public module
 "examples/*" = ["D100", "INP001", "T201"]
 "site/*" = ["D", "INP001", "S602"]
 
 [tool.pyright]
 typeCheckingMode = "off"
```

### Comparing `pymatviz-0.8.2/readme.md` & `pymatviz-0.8.3/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,44 +36,46 @@
 
 ## Usage
 
 See the Jupyter notebooks under [`examples/`](examples) for how to use `pymatviz`. PRs with additional examples are welcome! 🙏
 
 |                                                                                                                        |                                                                                                                                       |                                      |
 | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
+| [mlff_phonons.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb)                         | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb)             | [![Launch Codespace]][codespace url] |
 | [matbench_dielectric_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)  | [![Launch Codespace]][codespace url] |
 | [mp_bimodal_e_form.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)               | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)        | [![Launch Codespace]][codespace url] |
 | [matbench_perovskites_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_perovskites_eda.ipynb) | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_perovskites_eda.ipynb) | [![Launch Codespace]][codespace url] |
 | [mprester_ptable.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb)                   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb)          | [![Launch Codespace]][codespace url] |
 
 [Open in Google Colab]: https://colab.research.google.com/assets/colab-badge.svg
 [Launch Codespace]: https://img.shields.io/badge/Launch-Codespace-darkblue?logo=github
 [codespace url]: https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=340898532
 
 ## Periodic Table
 
 See [`pymatviz/ptable.py`](pymatviz/ptable.py). Heatmaps of the periodic table can be plotted both with `matplotlib` and `plotly`. `plotly` supports displaying additional data on hover or full interactivity through [Dash](https://plotly.com/dash).
 
-|                        [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                        |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
-| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
-|                                              ![ptable-heatmap]                                               |                        ![ptable-heatmap-ratio]                        |
-|                         [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                         | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
-|                                   ![ptable-heatmap-plotly-more-hover-data]                                   |                     ![ptable-heatmap-plotly-log]                      |
-|                       [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                        |              [`ptable_lines(data)`](pymatviz/ptable.py)               |
-|                                               ![ptable-hists]                                                |                            ![ptable-lines]                            |
-| [`ptable_heatmap_splits(data, colormap="coolwarm", start_angle=135, hide_f_block=True)`](pymatviz/ptable.py) |
-|                                           ![ptable-heatmap-splits]                                           |
+|                    [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                    |                   [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)                    |
+| :--------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------: |
+|                                          ![ptable-heatmap]                                           |                                       ![ptable-heatmap-ratio]                                       |
+|                     [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                     |                [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py)                |
+|                               ![ptable-heatmap-plotly-more-hover-data]                               |                                    ![ptable-heatmap-plotly-log]                                     |
+|                   [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                    |                             [`ptable_lines(data)`](pymatviz/ptable.py)                              |
+|                                           ![ptable-hists]                                            |                                           ![ptable-lines]                                           |
+| [`ptable_heatmap_splits(2_vals_per_elem, colormap="coolwarm", start_angle=135)`](pymatviz/ptable.py) | [`ptable_heatmap_splits(3_vals_per_elem, colormap="coolwarm", start_angle=90)`](pymatviz/ptable.py) |
+|                                      ![ptable-heatmap-splits-2]                                      |                                     ![ptable-heatmap-splits-3]                                      |
 
 [ptable-hists]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-hists.svg
 [ptable-lines]: https://github.com/janosh/pymatviz/raw/main/examples/diatomics/homo-nuclear-mace-medium.svg
-[ptable-heatmap-splits]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits.svg
+[ptable-heatmap-splits-2]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits-2.svg
+[ptable-heatmap-splits-3]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits-3.svg
 
 ## Phonons
 
-See [`pymatviz/phonons.py`](pymatviz/phonons.py).
+See [`examples/mlff_phonons.ipynb`](https://github.com/janosh/pymatviz/blob/main/examples/mlff_phonons.ipynb) for usage example.
 
 |           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           |             [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py)             |
 | :------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
 |                              ![phonon-bands]                               |                                ![phonon-dos]                                 |
 | [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) | [`plot_phonon_bands_and_dos(single_bands, single_dos)`](pymatviz/phonons.py) |
 |                      ![phonon-bands-and-dos-mp-2758]                       |                       ![phonon-bands-and-dos-mp-23907]                       |
```

### Comparing `pymatviz-0.8.2/tests/test_cumulative.py` & `pymatviz-0.8.3/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/tests/test_histograms.py` & `pymatviz-0.8.3/tests/test_histograms.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, Literal
 
 import matplotlib.pyplot as plt
 import plotly.graph_objects as go
 import pytest
 
 from pymatviz import elements_hist, spacegroup_hist, true_pred_hist
-from pymatviz.utils import VALID_BACKENDS, mpl_key
+from pymatviz.utils import MPL_BACKEND, PLOTLY_BACKEND, VALID_BACKENDS
 from tests.conftest import df_regr, y_pred, y_true
 
 
 if TYPE_CHECKING:
     import pandas as pd
     from numpy.typing import ArrayLike
     from pymatgen.core import Structure
@@ -39,46 +39,59 @@
     bins: int | None,
     cmap: str,
 ) -> None:
     ax = true_pred_hist(y_true, y_pred, y_std, df, bins=bins, cmap=cmap)
     assert isinstance(ax, plt.Axes)
 
 
-@pytest.mark.parametrize("xticks", ["all", "crys_sys_edges", 1, 50])
-@pytest.mark.parametrize("show_counts", [True, False])
-@pytest.mark.parametrize("show_empty_bins", [True, False])
 @pytest.mark.parametrize("backend", VALID_BACKENDS)
+@pytest.mark.parametrize(
+    ("xticks", "show_counts", "show_empty_bins", "log"),
+    [
+        ("all", True, True, True),
+        ("crys_sys_edges", False, False, False),
+        (1, True, False, True),
+        (50, False, True, False),
+    ],
+)
 def test_spacegroup_hist(
     spg_symbols: list[str],
     structures: list[Structure],
     backend: Backend,
     xticks: Literal["all", "crys_sys_edges", 1, 50],
     show_counts: bool,
     show_empty_bins: bool,
+    log: bool,
 ) -> None:
-    # spacegroup numbers
+    # test spacegroups as integers
     fig = spacegroup_hist(
         range(1, 231),
         xticks=xticks,
         show_counts=show_counts,
         show_empty_bins=show_empty_bins,
         backend=backend,
+        log=log,
     )
-    assert isinstance(fig, plt.Axes if backend == mpl_key else go.Figure)
+    assert isinstance(fig, plt.Axes if backend == MPL_BACKEND else go.Figure)
+    y_min, y_max = fig.get_ylim() if backend == MPL_BACKEND else fig.layout.yaxis.range
+    assert y_min == 0
+    assert y_max == pytest.approx(
+        0.02118929 if log and backend == PLOTLY_BACKEND else 1.05
+    ), f"{y_max=} {log=} {backend=}"
 
-    # spacegroup symbols
+    # test spacegroups as symbols
     fig = spacegroup_hist(
         spg_symbols,
         xticks=xticks,
         show_counts=show_counts,
         show_empty_bins=show_empty_bins,
         backend=backend,
     )
 
-    # pmg structures
+    # test spacegroups determined on-the-fly from structures
     spacegroup_hist(
         structures,
         xticks=xticks,
         show_counts=show_counts,
         show_empty_bins=show_empty_bins,
         backend=backend,
     )
```

### Comparing `pymatviz-0.8.2/tests/test_init.py` & `pymatviz-0.8.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/tests/test_io.py` & `pymatviz-0.8.3/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         size=size,
         style=style,
         styler_css=styler_css,
     )
     try:
         df_to_pdf(**kwds)
     except ImportError as exc:
+        # check we're raising helpful error messages on missing deps
         if weasyprint is None:
             assert "weasyprint not installed\n" in str(exc)  # noqa: PT017
             return
         if pdfCropMargins is None:
             assert "cropPdfMargins not installed\n" in str(exc)  # noqa: PT017
             return
 
@@ -214,15 +215,15 @@
         styles=styles,
         inline_props=inline_props,
         styler_css=styler_css,
     )
     assert not file_path.is_file()
     html2 = df_to_html_table(
         df_mixed.style,
-        file_path,
+        file_path=file_path,
         script=script,
         styles=styles,
         inline_props=inline_props,
         styler_css=styler_css,
     )
     assert html1 == html2
```

### Comparing `pymatviz-0.8.2/tests/test_parity.py` & `pymatviz-0.8.3/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/tests/test_phonons.py` & `pymatviz-0.8.3/tests/test_phonons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+import re
 from glob import glob
 from typing import Literal, Union
 
 import plotly.graph_objects as go
 import pytest
 from monty.io import zopen
 from monty.json import MontyDecoder, MSONable
@@ -89,24 +90,24 @@
 
     # test dict of band structures
     fig = plot_phonon_bands(
         phonon_bands_doses_mp_2758["bands"], branch_mode=branch_mode, branches=branches
     )
     assert isinstance(fig, go.Figure)
 
-    with pytest.raises(
-        TypeError, match=f"Only {PhononBands.__name__} supported, got str"
-    ):
-        plot_phonon_bands("invalid input")
-
 
 def test_plot_phonon_bands_raises(
     phonon_bands_doses_mp_2758: BandsDoses, capsys: pytest.CaptureFixture
 ) -> None:
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        TypeError, match=f"Only {PhononBands.__name__} or dict supported, got str"
+    ):
+        plot_phonon_bands("invalid input")
+
+    with pytest.raises(ValueError) as exc:  # noqa: PT011
         plot_phonon_bands(
             phonon_bands_doses_mp_2758["bands"]["DFT"], branches=("foo-bar",)
         )
 
     assert (
         "No common branches with branch_mode='union'.\n"
         "- : GAMMA-X, X-U, K-GAMMA, GAMMA-L, L-W, W-X\n"
@@ -117,14 +118,23 @@
     plot_phonon_bands(
         phonon_bands_doses_mp_2758["bands"]["DFT"], branches=("X-U", "foo-bar")
     )
     stdout, stderr = capsys.readouterr()
     assert stdout == ""
     assert "Warning: missing_branches={'foo-bar'}, available branches:" in stderr
 
+    with pytest.raises(ValueError, match="Invalid branch_mode='invalid'"):
+        plot_phonon_bands(
+            phonon_bands_doses_mp_2758["bands"]["DFT"],
+            branch_mode="invalid",  # type: ignore[arg-type]
+        )
+
+    with pytest.raises(ValueError, match="Empty band structure dict"):
+        plot_phonon_bands({})
+
 
 @pytest.mark.parametrize(
     "sym_point, expected",
     [("Γ", "Γ"), ("Γ|DELTA", "Γ|Δ"), ("GAMMA", "Γ"), ("S_0|SIGMA", "S<sub>0</sub>|Σ")],
 )
 def test_pretty_sym_point(sym_point: str, expected: str) -> None:
     assert pretty_sym_point(sym_point) == expected
@@ -168,14 +178,30 @@
         normalize=normalize,
         units=units,
         last_peak_anno=last_peak_anno,
     )
     assert isinstance(fig, go.Figure)
 
 
+def test_plot_phonon_dos_raises(phonon_bands_doses_mp_2758: BandsDoses) -> None:
+    with pytest.raises(
+        TypeError, match=f"Only {PhononDos.__name__} or dict supported, got str"
+    ):
+        plot_phonon_dos("invalid input")
+
+    with pytest.raises(ValueError, match="Empty DOS dict"):
+        plot_phonon_dos({})
+
+    expected_msg = (
+        "Invalid unit='invalid', must be one of ['THz', 'eV', 'meV', 'Ha', 'cm-1']"
+    )
+    with pytest.raises(ValueError, match=re.escape(expected_msg)):
+        plot_phonon_dos(phonon_bands_doses_mp_2758["doses"], units="invalid")  # type: ignore[arg-type]
+
+
 @pytest.mark.parametrize(
     "units, stack, sigma, normalize, last_peak_anno",
     [
         ("eV", False, 0.01, "max", "{key}={last_peak:.1f}"),
         ("meV", False, 0.05, "sum", "{key}={last_peak:.4} ({units})"),
         ("cm-1", True, 0.1, "integral", None),
         ("THz", True, 0.1, None, ""),
@@ -212,11 +238,11 @@
     # check legend labels
     assert {trace.name for trace in fig.data} == {"DFT", "MACE"}
 
     fig = plot_phonon_bands_and_dos(bands["DFT"], doses["DFT"])
     assert isinstance(fig, go.Figure)
 
     band_keys, dos_keys = set(bands), set(phonon_doses)
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError, match=f"{band_keys=} and {dos_keys=} must be identical"
+    ):
         plot_phonon_bands_and_dos(bands, phonon_doses)
-
-    assert str(exc.value) == f"{band_keys=} and {dos_keys=} must be identical"
```

### Comparing `pymatviz-0.8.2/tests/test_powerups.py` & `pymatviz-0.8.3/tests/test_powerups.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,30 +101,46 @@
 
 def test_annote_metrics_bad_fig() -> None:
     err_msg = "Unexpected type for fig: str, must be one of"
     with pytest.raises(TypeError, match=err_msg):
         annotate_metrics(y_pred, y_true, fig="invalid")
 
 
-@pytest.mark.parametrize("xaxis_type", ["linear", "log"])
-@pytest.mark.parametrize("yaxis_type", ["linear", "log"])
-@pytest.mark.parametrize("trace_idx", [0, 1])
-@pytest.mark.parametrize("line_kwds", [None, {"color": "blue"}])
+@pytest.mark.parametrize(
+    ("xaxis_type", "yaxis_type", "trace_idx", "line_kwds", "retain_xy_limits"),
+    [
+        ("linear", "log", 0, None, True),
+        ("log", "linear", 1, {"color": "red"}, False),
+        ("log", "log", 0, {"color": "green"}, True),
+        ("linear", "linear", 1, None, False),
+    ],
+)
 def test_add_identity_line(
     plotly_scatter: go.Figure,
     xaxis_type: str,
     yaxis_type: str,
     trace_idx: int,
     line_kwds: dict[str, str] | None,
+    retain_xy_limits: bool,
 ) -> None:
     # Set axis types
     plotly_scatter.layout.xaxis.type = xaxis_type
     plotly_scatter.layout.yaxis.type = yaxis_type
 
-    fig = add_identity_line(plotly_scatter, line_kwds=line_kwds, trace_idx=trace_idx)
+    # record initial axis limits
+    dev_fig_pre = plotly_scatter.full_figure_for_development(warn=False)
+    x_range_pre = dev_fig_pre.layout.xaxis.range
+    y_range_pre = dev_fig_pre.layout.yaxis.range
+
+    fig = add_identity_line(
+        plotly_scatter,
+        line_kwds=line_kwds,
+        trace_idx=trace_idx,
+        retain_xy_limits=retain_xy_limits,
+    )
     assert isinstance(fig, go.Figure)
 
     # retrieve identity line
     line = next((shape for shape in fig.layout.shapes if shape.type == "line"), None)
     assert line is not None
 
     assert line.layer == "below"
@@ -132,14 +148,26 @@
     # check line coordinates
     assert line.x0 == line.y0
     assert line.x1 == line.y1
     # check fig axis types
     assert fig.layout.xaxis.type == xaxis_type
     assert fig.layout.yaxis.type == yaxis_type
 
+    if retain_xy_limits:
+        assert dev_fig_pre.layout.xaxis.range == x_range_pre
+        assert dev_fig_pre.layout.yaxis.range == y_range_pre
+    else:
+        dev_fig_post = fig.full_figure_for_development(warn=False)
+        x_range_post = dev_fig_post.layout.xaxis.range
+        y_range_post = dev_fig_post.layout.yaxis.range
+        # this assumes that the x and y axis had different ranges initially which became
+        # equalized by adding an identity line (which is the case for plotly_scatter)
+        assert x_range_post != x_range_pre
+        assert y_range_post != y_range_pre
+
 
 @pytest.mark.parametrize("line_kwds", [None, {"color": "blue"}])
 def test_add_identity_matplotlib(
     matplotlib_scatter: plt.Figure, line_kwds: dict[str, str] | None
 ) -> None:
     expected_line_color = (line_kwds or {}).get("color", "black")
     # test Figure
```

### Comparing `pymatviz-0.8.2/tests/test_ptable.py` & `pymatviz-0.8.3/tests/test_ptable.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,120 +1,116 @@
 from __future__ import annotations
 
 import random
+import re
 from typing import TYPE_CHECKING, Any, Literal
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import pytest
-from numpy.testing import assert_allclose
 from plotly.exceptions import PlotlyError
 from pymatgen.core.periodic_table import Element
 
 from pymatviz import (
     count_elements,
     ptable_heatmap,
     ptable_heatmap_plotly,
     ptable_heatmap_ratio,
     ptable_heatmap_splits,
     ptable_hists,
     ptable_lines,
     ptable_scatters,
 )
 from pymatviz.enums import Key
-from pymatviz.ptable import add_element_type_legend, data_preprocessor
+from pymatviz.ptable import PTableProjector
 from pymatviz.utils import df_ptable, si_fmt, si_fmt_int
 
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
     from typing import Any, ClassVar
 
     from pymatgen.core import Composition
 
     from pymatviz.ptable import CountMode
 
 
-class TestDataPreprocessor:
-    test_dict: ClassVar = {"H": 1.0, "He": [2.0, 4.0], "Li": np.array([6.0, 8.0])}
-
-    @staticmethod
-    def _validate_output_df(output_df: pd.DataFrame) -> None:
-        assert isinstance(output_df, pd.DataFrame)
-
-        assert list(output_df) == [Key.heat_val]
-        assert list(output_df.index) == ["H", "He", "Li"]
-
-        assert_allclose(output_df.loc["H", Key.heat_val], [1.0])
-        assert_allclose(output_df.loc["He", Key.heat_val], [2.0, 4.0])
-        assert_allclose(output_df.loc["Li", Key.heat_val], [6.0, 8.0])
-
-        assert output_df.attrs["vmin"] == 1.0
-        assert output_df.attrs["vmax"] == 8.0
-
-    def test_from_pd_dataframe(self) -> None:
-        input_df: pd.DataFrame = pd.DataFrame(
-            self.test_dict.items(), columns=[Key.element, Key.heat_val]
-        ).set_index(Key.element)
-
-        output_df: pd.DataFrame = data_preprocessor(input_df)
-
-        self._validate_output_df(output_df)
-
-    def test_from_pd_series(self) -> None:
-        input_series: pd.Series = pd.Series(self.test_dict)
-
-        output_df = data_preprocessor(input_series)
-
-        self._validate_output_df(output_df)
-
-    def test_from_dict(self) -> None:
-        input_dict = self.test_dict
-
-        output_df = data_preprocessor(input_dict)
-
-        self._validate_output_df(output_df)
-
-    def test_unsupported_type(self) -> None:
-        invalid_data = [0, 1, 2]
-
-        with pytest.raises(TypeError, match="Unsupported data type"):
-            data_preprocessor(invalid_data)
-
-    def test_get_vmin_vmax(self) -> None:
-        # Test without nested list/array
-        test_dict_0 = {"H": 1, "He": [2, 4], "Li": np.array([6, 8])}
-
-        output_df_0 = data_preprocessor(test_dict_0)
-
-        assert output_df_0.attrs["vmin"] == 1
-        assert output_df_0.attrs["vmax"] == 8
+class TestPTableProjector:
+    test_dict: ClassVar = {
+        "H": 1,  # int
+        "He": [2.0, 4.0],  # float list
+        "Li": np.array([6.0, 8.0]),  # float array
+        "Na": 11.0,  # float
+        "Mg": {"a": -1, "b": 14.0}.values(),  # dict_values
+        "Al": {-1, 2.3},  # mixed int/float set
+    }
 
-        # Test with nested list/array
-        test_dict_1 = {
-            "H": 1,
-            "He": [[2, 3], [4, 5]],
-            "Li": [np.array([6, 7]), np.array([8, 9])],
+    def test_elem_types(self) -> None:
+        projector = PTableProjector(data=self.test_dict)
+        assert projector.elem_types == {
+            "Noble Gas",
+            "Metal",
+            "Alkaline Earth Metal",
+            "Nonmetal",
+            "Alkali Metal",
         }
 
-        output_df_1 = data_preprocessor(test_dict_1)
+    def test_hide_f_block(self) -> None:
+        # check default is True if no f-block elements in data
+        assert PTableProjector(data=self.test_dict).hide_f_block is True
+        assert PTableProjector(data={"H": 1}).hide_f_block is True
+        # check default is False if f-block elements in data
+        assert PTableProjector(data=self.test_dict | {"La": 1}).hide_f_block is False
+        assert PTableProjector(data={"La": 1}).hide_f_block is False
+        # check override
+        assert PTableProjector(data={"La": 1}, hide_f_block=True).hide_f_block is True
+
+    def test_get_elem_type_color(self) -> None:
+        projector = PTableProjector(data=self.test_dict)
+
+        assert projector.get_elem_type_color("H") == "green"
+        assert projector.get_elem_type_color("Fe") == "blue"
+
+    @pytest.mark.parametrize(
+        "data, elem_type_colors",
+        [
+            # data=dict, elem colors=empty dict
+            ({"Li": [1, 2, 3], "Na": [4, 5, 6], "K": [7, 8, 9]}, {}),
+            # data=series, elem colors=dict
+            (
+                pd.Series([1, 2, 3], index=["Fe", "Fe", "Fe"]),
+                {"Transition Metal": "red", "Nonmetal": "blue"},
+            ),
+            # data=dataframe, elem colors=None
+            (pd.DataFrame({"Fe": [1, 2, 3], "O": [4, 5, 6], "P": [7, 8, 9]}), None),
+        ],
+    )
+    def test_add_element_type_legend_data_types(
+        self,
+        data: pd.DataFrame | pd.Series | dict[str, list[float]],
+        elem_type_colors: dict[str, str] | None,
+    ) -> None:
+        projector = PTableProjector(data=data, elem_type_colors=elem_type_colors)
+
+        legend_title = "Element Types"
+        legend_kwargs = dict(loc="upper right", ncol=5, fontsize=12, title=legend_title)
+        projector.add_elem_type_legend(kwargs=legend_kwargs)
+
+        legend = plt.gca().get_legend()
+        assert isinstance(legend, mpl.legend.Legend)
+        assert len(legend.get_texts()) in {1, 2}
+        legend_labels = {text.get_text() for text in legend.get_texts()}
+        assert legend_labels <= {"Transition Metal", "Alkali Metal", "Nonmetal"}
+        assert legend._ncols == 5  # noqa: SLF001
 
-        assert output_df_1.attrs["vmin"] == 1
-        assert output_df_1.attrs["vmax"] == 9
-
-
-class TestMissingAnomalyHandle:
-    def test_handle_missing(self) -> None:
-        pass
-
-    def test_handle_infinity(self) -> None:
-        pass
+        assert legend.get_title().get_text() == legend_title
+        assert legend.get_texts()[0].get_fontsize() == 12
 
 
 @pytest.fixture()
 def glass_elem_counts(glass_formulas: pd.Series[Composition]) -> pd.Series[int]:
     return count_elements(glass_formulas)
 
 
@@ -232,21 +228,26 @@
     ax = ptable_heatmap(glass_elem_counts, cbar_fmt=".3f")
     cbar_labels = [label.get_text() for label in ax.child_axes[0].get_xticklabels()]
     assert cbar_labels[:2] == ["0.000", "50.000"]
 
     # cbar_fmt as function
     ax = ptable_heatmap(glass_elem_counts, fmt=si_fmt)
     ax = ptable_heatmap(
-        glass_elem_counts, fmt=lambda x, _: f"{x:.0f}", cbar_fmt=si_fmt_int
+        glass_elem_counts, fmt=lambda x: f"{x:.0f}", cbar_fmt=si_fmt_int
     )
     ax = ptable_heatmap(glass_elem_counts, cbar_fmt=lambda x, _: f"{x:.3f} kg")
 
     ax = ptable_heatmap(glass_elem_counts, heat_mode="percent", cbar_fmt=".3%")
-    cbar_1st_label = ax.child_axes[0].get_xticklabels()[0].get_text()
+    cbar_ax = ax.child_axes[0]
+    cbar_1st_label = cbar_ax.get_xticklabels()[0].get_text()
     assert cbar_1st_label == "0.000%"
+    cbar_title = cbar_ax.title
+    assert str(cbar_title) == "Text(0.5, 1.0, 'Element Count')"
+    # check colorbar title font color is black and hence visible on white background
+    assert cbar_title.get_color() == "black"
 
     # tile_size
     ptable_heatmap(df_ptable.atomic_mass, tile_size=1)
     ptable_heatmap(df_ptable.atomic_mass, tile_size=(0.9, 1))
 
     # bad colorscale should raise ValueError
     bad_name = "bad color scale"
@@ -260,26 +261,33 @@
     # test text_style
     ptable_heatmap(glass_formulas, text_style=dict(color="red", fontsize=12))
 
     # test show_scale (with heat_mode)
     ptable_heatmap(glass_formulas, heat_mode="percent", show_scale=False)
 
 
-@pytest.mark.parametrize("hide_f_block", [False, True])
+@pytest.mark.parametrize("hide_f_block", [None, False, True])
 def test_ptable_heatmap_splits(hide_f_block: bool) -> None:
     """Test ptable_heatmap_splits with arbitrary data length."""
-    data_dict = {
+    data_dict: dict[str, Any] = {
         elem.symbol: [
             random.randint(0, 10)  # random value for each split
             # random number of 1-4 splits per element
             for _ in range(random.randint(1, 4))
         ]
         for elem in Element
     }
 
+    # Also test different data types
+    data_dict["H"] = {"a": 1, "b": 2}.values()
+    data_dict["He"] = [1, 2]
+    data_dict["Li"] = np.array([1, 2])
+    data_dict["Be"] = 1
+    data_dict["B"] = 2.0
+
     cbar_title = "Periodic Table Evenly-Split Tiles Plots"
     fig = ptable_heatmap_splits(
         data_dict,
         colormap="coolwarm",
         start_angle=135,
         cbar_title=cbar_title,
         hide_f_block=hide_f_block,
@@ -441,17 +449,18 @@
         assert trace["zmax"] == pytest.approx(df_ptable.density.max())
     else:
         assert cscale_range == (trace["zmin"], trace["zmax"])
 
 
 def test_ptable_heatmap_plotly_cscale_range_raises() -> None:
     cscale_range = (0, 10, 20)
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(
+        ValueError, match=re.escape(f"{cscale_range=} should have length 2")
+    ):
         ptable_heatmap_plotly(df_ptable.density, cscale_range=cscale_range)  # type: ignore[arg-type]
-    assert f"{cscale_range=} should have length 2" in str(exc.value)
 
 
 @pytest.mark.parametrize(
     "label_map",
     [None, False, {"1.0": "one", "2.0": "two", "3.0": "three", np.nan: "N/A"}],
 )
 def test_ptable_heatmap_plotly_label_map(
@@ -472,61 +481,70 @@
         assert sum(
             any(val in anno.text for val in label_map.values())
             for anno in fig.layout.annotations
         )
 
 
 @pytest.mark.parametrize(
-    "data, symbol_pos, anno_kwds, hist_kwds",
+    "data, symbol_pos, hist_kwargs",
     [
-        (pd.DataFrame({"H": [1, 2, 3], "He": [4, 5, 6]}), (0, 0), {}, None),
+        ({"H": [1, 2, 3], "He": [4, 5, 6]}, (0, 0), None),
+        (pd.DataFrame({"Fe": [1, 2, 3], "O": [4, 5, 6]}), (0, 0), None),
         (
             dict(H=[1, 2, 3], He=[4, 5, 6]),
             (1, 1),
-            dict(text=lambda x: f"{len(x):,}"),
             {},
         ),
         (
             dict(H=np.array([1, 2, 3]), He=np.array([4, 5, 6])),
             (1, 1),
-            dict(text=lambda x: f"{len(x):,}"),
             {},
         ),
         (
             pd.Series([[1, 2, 3], [4, 5, 6]], index=["H", "He"]),
             (1, 1),
             dict(xy=(0, 0)),
-            lambda _hist_vals: dict(color="red"),
         ),
     ],
 )
 def test_ptable_hists(
     data: pd.DataFrame | pd.Series | dict[str, list[int]],
     symbol_pos: tuple[int, int],
-    anno_kwds: dict[str, Any],
-    hist_kwds: dict[str, Any],
+    hist_kwargs: dict[str, Any],
 ) -> None:
-    fig = ptable_hists(
-        data, symbol_pos=symbol_pos, anno_kwds=anno_kwds, hist_kwds=hist_kwds
+    fig_0 = ptable_hists(
+        data,
+        symbol_pos=symbol_pos,
+        child_kwargs=hist_kwargs,
+    )
+    assert isinstance(fig_0, plt.Figure)
+
+    # Test partial x_range
+    fig_1 = ptable_hists(
+        data,
+        x_range=(2, None),
+        symbol_pos=symbol_pos,
+        child_kwargs=hist_kwargs,
     )
-    assert isinstance(fig, plt.Figure)
+    assert isinstance(fig_1, plt.Figure)
 
 
 @pytest.mark.parametrize("hide_f_block", [False, True])
 def test_ptable_lines(hide_f_block: bool) -> None:
     """Test ptable_lines."""
     fig = ptable_lines(
         data={
             "Fe": [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
             "O": [[10, 11], [12, 13], [14, 15]],
         },
         hide_f_block=hide_f_block,
     )
     assert isinstance(fig, plt.Figure)
-    assert len(fig.axes) == 126 if hide_f_block else 181
+    expected_n_axes = 126 if hide_f_block else 180
+    assert len(fig.axes) == expected_n_axes
 
 
 @pytest.mark.parametrize("hide_f_block", [False, True])
 def test_ptable_scatters(hide_f_block: bool) -> None:
     """Test ptable_scatters."""
     fig = ptable_scatters(
         data={
@@ -548,33 +566,7 @@
             "O": [[10, 11], [12, 13], [14, 15]],
         },
         # colormap="coolwarm",
         # cbar_title="Test ptable_scatters",
     )
     assert isinstance(fig, plt.Figure)
     assert len(fig.axes) == 180
-
-
-@pytest.mark.parametrize(
-    "data",
-    [
-        {"Li": [1, 2, 3], "Na": [4, 5, 6], "K": [7, 8, 9]},
-        pd.DataFrame({"Fe": [1, 2, 3], "O": [4, 5, 6]}),
-        pd.Series([1, 2, 3], index=["Fe", "Fe", "Fe"]),
-    ],
-)
-def test_add_element_type_legend_data_types(
-    data: pd.DataFrame | pd.Series | dict[str, list[float]],
-) -> None:
-    elem_class_colors = {"Transition Metal": "red", "Nonmetal": "blue"}
-    legend_kwargs = dict(loc="upper right", ncol=5, fontsize=12, title="Element Types")
-
-    add_element_type_legend(data, elem_class_colors, legend_kwargs=legend_kwargs)
-    legend = plt.gca().get_legend()
-    assert isinstance(legend, mpl.legend.Legend)
-    assert len(legend.get_texts()) in {1, 2}
-    legend_labels = {text.get_text() for text in legend.get_texts()}
-    assert legend_labels <= {"Transition Metal", "Alkali Metal", "Nonmetal"}
-    assert legend._ncols == 5  # noqa: SLF001
-
-    assert legend.get_title().get_text() == "Element Types"
-    assert legend.get_texts()[0].get_fontsize() == 12
```

### Comparing `pymatviz-0.8.2/tests/test_relevance.py` & `pymatviz-0.8.3/tests/test_relevance.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/tests/test_sankey.py` & `pymatviz-0.8.3/tests/test_sankey.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,13 @@
 import pytest
 
 from pymatviz.sankey import sankey_from_2_df_cols
 
 
 @pytest.mark.parametrize("labels_with_counts", [True, False, "percent"])
 def test_sankey_from_2_df_cols(labels_with_counts: bool | Literal["percent"]) -> None:
-    col_names = "col_a col_b".split()
+    col_names = ["col_a", "col_b"]
     df_rand = pd.DataFrame(np.random.randint(0, 10, size=(100, 2)), columns=col_names)
-    fig = sankey_from_2_df_cols(df_rand, col_names, labels_with_counts)
+    fig = sankey_from_2_df_cols(
+        df_rand, col_names, labels_with_counts=labels_with_counts
+    )
     assert isinstance(fig, go.Figure)
```

### Comparing `pymatviz-0.8.2/tests/test_structure_viz.py` & `pymatviz-0.8.3/tests/test_structure_viz.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     assert y_max > 5
 
     patch_counts = pd.Series(
         [type(patch).__name__ for patch in ax.patches]
     ).value_counts()
     assert patch_counts["Wedge"] == len(disordered_struct.composition)
 
-    assert patch_counts["PathPatch"] > 182
+    min_expected_n_patches = 182
+    assert patch_counts["PathPatch"] > min_expected_n_patches
 
 
 @pytest.mark.parametrize("axis", [True, False, "on", "off", "square", "equal"])
 def test_plot_structure_2d_axis(axis: str | bool) -> None:
     ax = plot_structure_2d(disordered_struct, axis=axis)
     assert ax.axes.axison == (axis not in (False, "off"))
 
@@ -74,7 +75,25 @@
 ) -> None:
     ax = plot_structure_2d(disordered_struct, site_labels=site_labels)
     if site_labels is False:
         assert not ax.axes.texts
     else:
         label = ax.axes.texts[0].get_text()
         assert label in ("Fe", "O", "1.0", "Iron")
+
+
+def test_plot_structure_2d_warns() -> None:
+    # for sites with negative fractional coordinates
+    orig_coords = disordered_struct[0].frac_coords.copy()
+    disordered_struct[0].frac_coords = [-0.1, 0.1, 0.1]
+    standardize_struct = False
+    try:
+        with pytest.warns(
+            UserWarning,
+            match=(
+                "your structure has negative fractional coordinates but you passed "
+                f"{standardize_struct=}, you may want to set standardize_struct=True"
+            ),
+        ):
+            plot_structure_2d(disordered_struct, standardize_struct=standardize_struct)
+    finally:
+        disordered_struct[0].frac_coords = orig_coords
```

### Comparing `pymatviz-0.8.2/tests/test_sunburst.py` & `pymatviz-0.8.3/tests/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/tests/test_uncertainty.py` & `pymatviz-0.8.3/tests/test_uncertainty.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.2/tests/test_utils.py` & `pymatviz-0.8.3/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,16 @@
 ) -> None:
     idx_col = "index"
     df_float.index.name = idx_col
     bin_counts_col = "bin_counts"
     df_binned = bin_df_cols(
         df_float,
         bin_by_cols,
-        group_by_cols,
-        n_bins,
+        group_by_cols=group_by_cols,
+        n_bins=n_bins,
         verbose=verbose,
         bin_counts_col=bin_counts_col,
         kde_col=kde_col,
     )
 
     # ensure binned DataFrame has a minimum set of expected columns
     expected_cols = {bin_counts_col, *df_float, *(f"{col}_bins" for col in bin_by_cols)}
@@ -157,15 +157,15 @@
 
 
 def test_bin_df_cols_raises() -> None:
     df_dummy = pd.DataFrame({"col1": [1, 2, 3, 4], "col2": [2, 3, 4, 5]})
     bin_by_cols = ["col1", "col2"]
 
     # test error when passing n_bins as list but list has wrong length
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(ValueError) as exc:  # noqa: PT011
         bin_df_cols(df_dummy, bin_by_cols, n_bins=[2])
 
     assert "len(bin_by_cols)=2 != len(n_bins)=1" in str(exc.value)
 
 
 sample_dict = {"a": 1, "b": None, "c": [3, 4]}
 ref_sample_dict = deepcopy(sample_dict)
@@ -217,22 +217,24 @@
     with patch_dict(sample_dict, c={"x": 10, "y": 20}) as patched_dict:
         assert patched_dict == {"a": 1, "b": None, "c": {"x": 10, "y": 20}}
     assert sample_dict == ref_sample_dict
 
 
 def test_patch_dict_overlapping_args_kwargs() -> None:
     # kwargs should take precedence over args
-    with patch_dict(sample_dict, {"a": 7}, a=8) as patched_dict:
-        assert patched_dict["a"] == 8
+    a_val = 8
+    with patch_dict(sample_dict, {"a": 7}, a=a_val) as patched_dict:
+        assert patched_dict["a"] == a_val
     assert sample_dict == ref_sample_dict
 
 
 def test_patch_dict_remove_key_inside_context() -> None:
-    with patch_dict(sample_dict, d=7) as patched_dict:
-        assert patched_dict["d"] == 7
+    d_val = 7
+    with patch_dict(sample_dict, d=d_val) as patched_dict:
+        assert patched_dict["d"] == d_val
         del patched_dict["d"]
         assert "d" not in patched_dict
     assert sample_dict == ref_sample_dict
 
 
 assert ref_sample_dict == sample_dict, "sample_dict should not be modified"
```

