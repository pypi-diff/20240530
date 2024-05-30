# Comparing `tmp/prettypyplot-0.8.0.tar.gz` & `tmp/prettypyplot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prettypyplot-0.8.0.tar", last modified: Sun Apr  3 14:48:58 2022, max compression
+gzip compressed data, was "prettypyplot-0.9.0.tar", last modified: Thu Apr 28 08:54:54 2022, max compression
```

## Comparing `prettypyplot-0.8.0.tar` & `prettypyplot-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,35 @@
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-03 14:48:58.271046 prettypyplot-0.8.0/
--rw-r--r--   0 braniii   (1000) braniii   (1001)       42 2020-02-04 21:26:50.000000 prettypyplot-0.8.0/MANIFEST.in
--rw-r--r--   0 braniii   (1000) braniii   (1001)     9163 2022-04-03 14:48:58.271046 prettypyplot-0.8.0/PKG-INFO
--rw-r--r--   0 braniii   (1000) braniii   (1001)     6970 2021-09-22 14:55:53.000000 prettypyplot-0.8.0/README.md
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-03 14:48:58.267713 prettypyplot-0.8.0/prettypyplot/
--rw-r--r--   0 braniii   (1000) braniii   (1001)      243 2022-04-03 14:32:14.000000 prettypyplot-0.8.0/prettypyplot/__init__.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-03 14:48:58.267713 prettypyplot-0.8.0/prettypyplot/cmaps/
--rw-r--r--   0 braniii   (1000) braniii   (1001)       49 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/cmaps/__init__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    11225 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/cmaps/_bownair.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     2484 2021-03-15 19:25:39.000000 prettypyplot-0.8.0/prettypyplot/cmaps/_discrete.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    11235 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/cmaps/_macaw.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1628 2021-09-22 18:42:03.000000 prettypyplot-0.8.0/prettypyplot/cmaps/_tol_discrete.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     8948 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/cmaps/_turbo.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     9766 2021-09-22 18:46:47.000000 prettypyplot-0.8.0/prettypyplot/colors.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)      147 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/gallery.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    13168 2022-03-29 07:00:40.000000 prettypyplot-0.8.0/prettypyplot/plot.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    12935 2021-06-18 07:31:26.000000 prettypyplot-0.8.0/prettypyplot/style.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-03 14:48:58.267713 prettypyplot-0.8.0/prettypyplot/stylelib/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1169 2021-03-18 07:32:39.000000 prettypyplot-0.8.0/prettypyplot/stylelib/default.mplstyle
--rw-r--r--   0 braniii   (1000) braniii   (1001)      256 2020-04-21 10:05:44.000000 prettypyplot-0.8.0/prettypyplot/stylelib/latex.mplstyle
--rw-r--r--   0 braniii   (1000) braniii   (1001)      180 2020-04-21 10:04:38.000000 prettypyplot-0.8.0/prettypyplot/stylelib/minimal.mplstyle
--rw-r--r--   0 braniii   (1000) braniii   (1001)     6055 2021-02-18 12:01:20.000000 prettypyplot-0.8.0/prettypyplot/subplots.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4974 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/texts.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4131 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/prettypyplot/tools.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-03 14:48:58.267713 prettypyplot-0.8.0/prettypyplot.egg-info/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     9163 2022-04-03 14:48:58.000000 prettypyplot-0.8.0/prettypyplot.egg-info/PKG-INFO
--rw-r--r--   0 braniii   (1000) braniii   (1001)      823 2022-04-03 14:48:58.000000 prettypyplot-0.8.0/prettypyplot.egg-info/SOURCES.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)        1 2022-04-03 14:48:58.000000 prettypyplot-0.8.0/prettypyplot.egg-info/dependency_links.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)       32 2022-04-03 14:48:58.000000 prettypyplot-0.8.0/prettypyplot.egg-info/requires.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)       13 2022-04-03 14:48:58.000000 prettypyplot-0.8.0/prettypyplot.egg-info/top_level.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)      844 2022-04-03 14:48:58.271046 prettypyplot-0.8.0/setup.cfg
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1120 2022-04-03 14:31:37.000000 prettypyplot-0.8.0/setup.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-03 14:48:58.271046 prettypyplot-0.8.0/test/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1179 2021-03-15 19:25:39.000000 prettypyplot-0.8.0/test/test_cmaps.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     5484 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/test/test_colors.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1542 2021-06-17 13:39:16.000000 prettypyplot-0.8.0/test/test_plot.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     5756 2021-05-12 12:18:18.000000 prettypyplot-0.8.0/test/test_subplots.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     2292 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/test/test_texts.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     3889 2021-02-11 08:45:21.000000 prettypyplot-0.8.0/test/test_tools.py
+drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     1517 2022-04-28 06:57:10.000000 prettypyplot-0.9.0/LICENSE
+-rw-r--r--   0 braniii   (1000) braniii   (1001)       77 2022-04-28 06:57:10.000000 prettypyplot-0.9.0/MANIFEST.in
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     7679 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/PKG-INFO
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     6970 2022-04-28 06:57:10.000000 prettypyplot-0.9.0/README.md
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      280 2022-04-28 06:57:10.000000 prettypyplot-0.9.0/extra-requirements.txt
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      930 2022-04-28 08:54:54.995343 prettypyplot-0.9.0/setup.cfg
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     2061 2022-04-28 08:51:16.000000 prettypyplot-0.9.0/setup.py
+drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/src/
+drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/src/prettypyplot/
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      279 2022-04-28 08:51:27.000000 prettypyplot-0.9.0/src/prettypyplot/__init__.py
+drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/src/prettypyplot/cmaps/
+-rw-r--r--   0 braniii   (1000) braniii   (1001)       49 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/cmaps/__init__.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)    11225 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/cmaps/_bownair.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     2484 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/cmaps/_discrete.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)    11235 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/cmaps/_macaw.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     1628 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/cmaps/_tol_discrete.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     8948 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/cmaps/_turbo.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     9766 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/colors.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      147 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/gallery.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)    12735 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/plot.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)    15509 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/style.py
+drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/src/prettypyplot/stylelib/
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     1169 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/stylelib/default.mplstyle
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      256 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/stylelib/latex.mplstyle
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      180 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/stylelib/minimal.mplstyle
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     6055 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/subplots.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     4974 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/texts.py
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     2378 2022-04-28 06:57:11.000000 prettypyplot-0.9.0/src/prettypyplot/tools.py
+drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2022-04-28 08:54:54.992010 prettypyplot-0.9.0/src/prettypyplot.egg-info/
+-rw-r--r--   0 braniii   (1000) braniii   (1001)     7679 2022-04-28 08:54:54.000000 prettypyplot-0.9.0/src/prettypyplot.egg-info/PKG-INFO
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      825 2022-04-28 08:54:54.000000 prettypyplot-0.9.0/src/prettypyplot.egg-info/SOURCES.txt
+-rw-r--r--   0 braniii   (1000) braniii   (1001)        1 2022-04-28 08:54:54.000000 prettypyplot-0.9.0/src/prettypyplot.egg-info/dependency_links.txt
+-rw-r--r--   0 braniii   (1000) braniii   (1001)      202 2022-04-28 08:54:54.000000 prettypyplot-0.9.0/src/prettypyplot.egg-info/requires.txt
+-rw-r--r--   0 braniii   (1000) braniii   (1001)       13 2022-04-28 08:54:54.000000 prettypyplot-0.9.0/src/prettypyplot.egg-info/top_level.txt
```

### Comparing `prettypyplot-0.8.0/PKG-INFO` & `prettypyplot-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,213 +1,219 @@
 Metadata-Version: 2.1
 Name: prettypyplot
-Version: 0.8.0
+Version: 0.9.0
 Summary: Wrapper for matplotlib to generate pretty plots.
 Home-page: https://gitlab.com/braniii/prettypyplot
 Author: braniii
 License: BSD 3-Clause License
-Description: <div align="center">
-          <img
-            src="https://gitlab.com/braniii/prettypyplot/-/raw/master/gallery/logo_large.png"
-          />
-        
-          <p>
-            <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide" >
-                <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
-            <a href="https://gitlab.com/braniii/prettypyplot/pipelines" alt="Gitlab pipeline status" >
-                <img src="https://img.shields.io/gitlab/pipeline/braniii/prettypyplot" /></a>
-            <a href="https://gitlab.com/braniii/prettypyplot/-/commits/master">
-                <img alt="coverage report" src="https://gitlab.com/braniii/prettypyplot/badges/master/coverage.svg" /></a>
-            <a href="https://pypi.org/project/prettypyplot" alt="PyPI" >
-                <img src="https://img.shields.io/pypi/v/prettypyplot" /></a>
-            <a href="https://pepy.tech/project/prettypyplot" alt="Downloads" >
-                <img src="https://pepy.tech/badge/prettypyplot" /></a>
-            <a href="https://img.shields.io/pypi/pyversions/prettypyplot" alt="PyPI - Python Version">
-                <img src="https://img.shields.io/pypi/pyversions/prettypyplot" /></a>
-            <a href="https://gitlab.com/braniii/prettypyplot/-/blob/master/LICENSE" alt="PyPI - License" >
-                <img src="https://img.shields.io/pypi/l/prettypyplot" /></a>
-            <a href="https://braniii.gitlab.io/prettypyplot" alt="Doc" >
-                <img src="https://img.shields.io/badge/pdoc3-Documentation-brightgreen" /></a>
-          </p>
-        
-          <p>
-            <a href="https://braniii.gitlab.io/prettypyplot">Docs</a> •
-            <a href="#features">Features</a> •
-            <a href="#Installation">Installation</a> •
-            <a href="#usage">Usage</a>
-          </p>
-        </div>
-        
-        
-        
-        # prettypyplot
-        
-        The documentation including an gallery can be found [here](https://braniii.gitlab.io/prettypyplot).
-        
-        This is a wrapper package for matplotlib to achieve more easily pretty figures.
-        If you are looking for something complete, this project is nothing for you
-        but maybe [seaborn](https://seaborn.pydata.org/). The main aspect of this
-        project is to help me syncing my rcParams files and to stop copy-pasting so
-        much code.
-        
-        The aim of this project is to simplify the generation of some simple
-        pre-defined figures. Almost all code is inspired or taken from the
-        [matplotlib gallery](https://matplotlib.org/gallery/index.html). If you are a
-        power user or interested in generating complex figures, this packages is not
-        ment for you and you should better take a look in the matplotlib gallery
-        directly.
-        
-        This project is in an alpha stage, hence it is neither stable nor ready for
-        production.
-        > **CAUTION**:
-        > Starting from version 1.0.0 (which is far in the future) API-breaking
-        > changes will be made only in major releases. Until then, it can be changed
-        > in every minor release (see [changelog](#changelog)).
-        
-        ## Features
-        
-        The most notable features are:
-        
-        - figsize specifies size of canvas. So labels, ticks or colorbars are not counted.
-        - Nice top-aligned outter legends
-        - New colors
-        
-        ## Usage
-        
-        This package uses an syntax very close to matplotlib. Hence, it should be
-        straight forward to use it. Instead of calling a function on the axes itself,
-        one needs to pass here the axes as an argument (args or kwargs).
-        
-        ### Installation
-        
-        ```python
-        python3 -m pip install --upgrade prettypyplot
-        ```
-        or for the latest dev version
-        ```python
-        python3 -m pip install git+https://gitlab.com/braniii/prettypyplot.git
-        ```
-        
-        ### Usage
-        
-        ```python
-        import matplotlib.pyplot as plt
-        import prettypyplot as pplt
-        
-        pplt.use_style()
-        fig, ax = plt.subplots()
-        ...
-        pplt.plot(ax=ax, x, y)
-        pplt.savefig(output)
-        ```
-        
-        ### Known Bugs
-        
-        - `plt.subplots_adjust()` does not work with `pplt.savefig(use_canvas_size=True)`
-        If you find one, please open an issue.
-        - `pplt.savefig(use_canvas_size=True)` is not compatible with a grid of subplots
-        
-        ### Known Workarounds
-        
-        The method `pyplot.subplots_adjust()` is not compatible with the option
-        `use_canvas_size` in `prettypyplot.plot.savefig`,
-        use instead:
-        ```python
-        # this doesn't work, use instead gridspec
-        fig.subplots_adjust(hspace=0)
-        # use this instead
-        fig, axs = plt.subplots(..., gridspec_kw={'hspace': 0.000})
-        ```
-        
-        ## Comparison to `matplotlib`
-        
-        <table>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.plot</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.plot</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot.png" width="350">
-                </td>
-            </tr>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.legend</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot_legend.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.legend</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot_legend.png" width="350">
-                </td>
-            </tr>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.imshow</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.imshow</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow.png" width="350">
-                </td>
-            </tr>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.colorbar</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow_cbar.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.colorbar</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow_cbar.png" width="350">
-                </td>
-            </tr>
-        </table>
-        
-        ## Roadmap:
-        
-        The following list is sorted from *near future* to *hopefully ever*.
-        
-        - [x] add pytest
-        - [x] add search functionality in doc
-        - [x] refactoring code to improve readabilty
-        - [ ] add more colorpalettes
-        - [ ] add countour line plot
-        - [ ] add [axes_grid](https://matplotlib.org/3.1.1/tutorials/toolkits/axes_grid.html) examples
-        - [ ] add more gallery entries
-        - [ ] add package to conda_forge
-        - [ ] improve `plt.suplots()` behaviour together with `pplt.savefig()`
-        - [ ] setup widths and scaling factors for beamer and poster mode
-        - [ ] tweak all function to enable `STYLE='minimal'`
-        - [ ] implement tufte style
-        
-        ## Building Documentation:
-        
-        The doc is based on [pdoc](https://pdoc3.github.io/pdoc/) and can be created by
-        simply running `bash create_doc.sh` from the docs folder. For dependencies see in the
-        CI action.
-        
-        ## Similar Projects
-        
-        - [seaborn](https://seaborn.pydata.org/)
-        
-        ## Credits:
-        
-        In alphabetical order:
-        
-        - [colorcyclepicker](https://colorcyclepicker.mpetroff.net/)
-        - [coolors](https://coolors.co/)
-        - [matplotlib](https://matplotlib.org/)
-        - [prettyplotlib](https://github.com/olgabot/prettyplotlib)
-        - [realpython](https://realpython.com/)
-        - [viscm](https://github.com/matplotlib/viscm)
-        
 Keywords: matplotlib pyplot
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: docs
+Provides-Extra: all
+License-File: LICENSE
+
+<div align="center">
+  <img
+    src="https://gitlab.com/braniii/prettypyplot/-/raw/master/gallery/logo_large.png"
+  />
+
+  <p>
+    <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide" >
+        <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
+    <a href="https://gitlab.com/braniii/prettypyplot/pipelines" alt="Gitlab pipeline status" >
+        <img src="https://img.shields.io/gitlab/pipeline/braniii/prettypyplot" /></a>
+    <a href="https://gitlab.com/braniii/prettypyplot/-/commits/master">
+        <img alt="coverage report" src="https://gitlab.com/braniii/prettypyplot/badges/master/coverage.svg" /></a>
+    <a href="https://pypi.org/project/prettypyplot" alt="PyPI" >
+        <img src="https://img.shields.io/pypi/v/prettypyplot" /></a>
+    <a href="https://pepy.tech/project/prettypyplot" alt="Downloads" >
+        <img src="https://pepy.tech/badge/prettypyplot" /></a>
+    <a href="https://img.shields.io/pypi/pyversions/prettypyplot" alt="PyPI - Python Version">
+        <img src="https://img.shields.io/pypi/pyversions/prettypyplot" /></a>
+    <a href="https://gitlab.com/braniii/prettypyplot/-/blob/master/LICENSE" alt="PyPI - License" >
+        <img src="https://img.shields.io/pypi/l/prettypyplot" /></a>
+    <a href="https://braniii.gitlab.io/prettypyplot" alt="Doc" >
+        <img src="https://img.shields.io/badge/pdoc3-Documentation-brightgreen" /></a>
+  </p>
+
+  <p>
+    <a href="https://braniii.gitlab.io/prettypyplot">Docs</a> •
+    <a href="#features">Features</a> •
+    <a href="#Installation">Installation</a> •
+    <a href="#usage">Usage</a>
+  </p>
+</div>
+
+
+
+# prettypyplot
+
+The documentation including an gallery can be found [here](https://braniii.gitlab.io/prettypyplot).
+
+This is a wrapper package for matplotlib to achieve more easily pretty figures.
+If you are looking for something complete, this project is nothing for you
+but maybe [seaborn](https://seaborn.pydata.org/). The main aspect of this
+project is to help me syncing my rcParams files and to stop copy-pasting so
+much code.
+
+The aim of this project is to simplify the generation of some simple
+pre-defined figures. Almost all code is inspired or taken from the
+[matplotlib gallery](https://matplotlib.org/gallery/index.html). If you are a
+power user or interested in generating complex figures, this packages is not
+ment for you and you should better take a look in the matplotlib gallery
+directly.
+
+This project is in an alpha stage, hence it is neither stable nor ready for
+production.
+> **CAUTION**:
+> Starting from version 1.0.0 (which is far in the future) API-breaking
+> changes will be made only in major releases. Until then, it can be changed
+> in every minor release (see [changelog](#changelog)).
+
+## Features
+
+The most notable features are:
+
+- figsize specifies size of canvas. So labels, ticks or colorbars are not counted.
+- Nice top-aligned outter legends
+- New colors
+
+## Usage
+
+This package uses an syntax very close to matplotlib. Hence, it should be
+straight forward to use it. Instead of calling a function on the axes itself,
+one needs to pass here the axes as an argument (args or kwargs).
+
+### Installation
+
+```python
+python3 -m pip install --upgrade prettypyplot
+```
+or for the latest dev version
+```python
+python3 -m pip install git+https://gitlab.com/braniii/prettypyplot.git
+```
+
+### Usage
+
+```python
+import matplotlib.pyplot as plt
+import prettypyplot as pplt
+
+pplt.use_style()
+fig, ax = plt.subplots()
+...
+pplt.plot(ax=ax, x, y)
+pplt.savefig(output)
+```
+
+### Known Bugs
+
+- `plt.subplots_adjust()` does not work with `pplt.savefig(use_canvas_size=True)`
+If you find one, please open an issue.
+- `pplt.savefig(use_canvas_size=True)` is not compatible with a grid of subplots
+
+### Known Workarounds
+
+The method `pyplot.subplots_adjust()` is not compatible with the option
+`use_canvas_size` in `prettypyplot.plot.savefig`,
+use instead:
+```python
+# this doesn't work, use instead gridspec
+fig.subplots_adjust(hspace=0)
+# use this instead
+fig, axs = plt.subplots(..., gridspec_kw={'hspace': 0.000})
+```
+
+## Comparison to `matplotlib`
+
+<table>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.plot</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.plot</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot.png" width="350">
+        </td>
+    </tr>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.legend</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot_legend.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.legend</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot_legend.png" width="350">
+        </td>
+    </tr>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.imshow</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.imshow</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow.png" width="350">
+        </td>
+    </tr>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.colorbar</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow_cbar.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.colorbar</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow_cbar.png" width="350">
+        </td>
+    </tr>
+</table>
+
+## Roadmap:
+
+The following list is sorted from *near future* to *hopefully ever*.
+
+- [x] add pytest
+- [x] add search functionality in doc
+- [x] refactoring code to improve readabilty
+- [ ] add more colorpalettes
+- [ ] add countour line plot
+- [ ] add [axes_grid](https://matplotlib.org/3.1.1/tutorials/toolkits/axes_grid.html) examples
+- [ ] add more gallery entries
+- [ ] add package to conda_forge
+- [ ] improve `plt.suplots()` behaviour together with `pplt.savefig()`
+- [ ] setup widths and scaling factors for beamer and poster mode
+- [ ] tweak all function to enable `STYLE='minimal'`
+- [ ] implement tufte style
+
+## Building Documentation:
+
+The doc is based on [pdoc](https://pdoc3.github.io/pdoc/) and can be created by
+simply running `bash create_doc.sh` from the docs folder. For dependencies see in the
+CI action.
+
+## Similar Projects
+
+- [seaborn](https://seaborn.pydata.org/)
+
+## Credits:
+
+In alphabetical order:
+
+- [colorcyclepicker](https://colorcyclepicker.mpetroff.net/)
+- [coolors](https://coolors.co/)
+- [matplotlib](https://matplotlib.org/)
+- [prettyplotlib](https://github.com/olgabot/prettyplotlib)
+- [realpython](https://realpython.com/)
+- [viscm](https://github.com/matplotlib/viscm)
+
+
```

#### html2text {}

```diff
@@ -1,10 +1,17 @@
-Metadata-Version: 2.1 Name: prettypyplot Version: 0.8.0 Summary: Wrapper for
+Metadata-Version: 2.1 Name: prettypyplot Version: 0.9.0 Summary: Wrapper for
 matplotlib to generate pretty plots. Home-page: https://gitlab.com/braniii/
-prettypyplot Author: braniii License: BSD 3-Clause License Description:
+prettypyplot Author: braniii License: BSD 3-Clause License Keywords: matplotlib
+pyplot Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Python: >=3.6 Description-Content-Type:
+text/markdown Provides-Extra: testing Provides-Extra: docs Provides-Extra: all
+License-File: LICENSE
  [https://gitlab.com/braniii/prettypyplot/-/raw/master/gallery/logo_large.png]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_t_y_l_e_-_w_e_m_a_k_e_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _g_i_t_l_a_b_/_p_i_p_e_l_i_n_e_/_b_r_a_n_i_i_i_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_c_o_v_e_r_a_g_e_ _r_e_p_o_r_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
       _p_y_p_i_/_v_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
   _p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_d_o_c_3_-_D_o_c_u_m_e_n_t_a_t_i_o_n_-_b_r_i_g_h_t_g_r_e_e_n_]
                  _D_o_c_s â¢ _F_e_a_t_u_r_e_s â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _U_s_a_g_e
@@ -66,14 +73,8 @@
 Building Documentation: The doc is based on [pdoc](https://pdoc3.github.io/
 pdoc/) and can be created by simply running `bash create_doc.sh` from the docs
 folder. For dependencies see in the CI action. ## Similar Projects - [seaborn]
 (https://seaborn.pydata.org/) ## Credits: In alphabetical order: -
 [colorcyclepicker](https://colorcyclepicker.mpetroff.net/) - [coolors](https://
 coolors.co/) - [matplotlib](https://matplotlib.org/) - [prettyplotlib](https://
 github.com/olgabot/prettyplotlib) - [realpython](https://realpython.com/) -
-[viscm](https://github.com/matplotlib/viscm) Keywords: matplotlib pyplot
-Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Python: >=3.6 Description-Content-Type:
-text/markdown
+[viscm](https://github.com/matplotlib/viscm)
```

### Comparing `prettypyplot-0.8.0/README.md` & `prettypyplot-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/cmaps/_bownair.py` & `prettypyplot-0.9.0/src/prettypyplot/cmaps/_bownair.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/cmaps/_discrete.py` & `prettypyplot-0.9.0/src/prettypyplot/cmaps/_discrete.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/cmaps/_macaw.py` & `prettypyplot-0.9.0/src/prettypyplot/cmaps/_macaw.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/cmaps/_tol_discrete.py` & `prettypyplot-0.9.0/src/prettypyplot/cmaps/_tol_discrete.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/cmaps/_turbo.py` & `prettypyplot-0.9.0/src/prettypyplot/cmaps/_turbo.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/colors.py` & `prettypyplot-0.9.0/src/prettypyplot/colors.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/plot.py` & `prettypyplot-0.9.0/src/prettypyplot/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,16 +196,15 @@
     outside : str or bool
         False, 'top', 'right', 'bottom' or 'left'.
 
     axs : list of mpl.axes.Axes
         List of axes which are used for extracting all labels.
 
     ax : mpl.axes.Axes
-        Axes which is used for placing legend. If none is specified `axs`
-        will be used if not `None` and otherwise the currently active axis
+        Axes which is used for placing legend.
 
     args, kwargs
         See [pyplot.legend()](MPL_DOC.pyplot.legend.html)
 
     Returns
     -------
     leg : matplotlib.legend.Legend
@@ -221,28 +220,14 @@
         raise ValueError(
             'Use for outside one of [False, {0}]'.format(
                 ', '.join(['"{0}"'.format(dr) for dr in default_kwargs]),
             ),
         )
 
     # parse axes
-    if ax is not None:
-        ax = tools.gca(ax)
-        if axs is not None:
-            axs = tools.get_axes(axs)
-        else:
-            axs = [ax]
-    else:
-        if axs is not None:
-            axs = tools.get_axes(axs)
-            ax = tools.get_axes(axs)
-        else:
-            ax = plt.gca()
-            axs = [ax]
-
     args, ax = tools.parse_axes(*args, ax=ax)
 
     # parse axs
     if axs is None:
         axs = [ax]
     else:
         axs = tools.get_axes(axs)
```

### Comparing `prettypyplot-0.8.0/prettypyplot/style.py` & `prettypyplot-0.9.0/src/prettypyplot/style.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,75 +127,93 @@
         If true LaTeX font will be used.
 
     sf : bool, optional
         Use sans-serif font for text and latex math environment.
 
     """
     # set selected mode and style
-    if mode is not None:
-        if isinstance(mode, Mode):
-            pass
-        elif isinstance(mode, str) and mode.upper() in Mode.keys_list():
-            mode = Mode[mode.upper()]
-        else:
-            assert ValueError(
-                'Mode "{mode}" is not supported, use one of {modes}.'.format(
-                    mode=mode,
-                    modes=Mode.keys_list(),
-                ),
-            )
-
-        _pplt.MODE = mode
-
     if style is not None:
         if isinstance(style, Style):
             pass
         elif isinstance(style, str) and style.upper() in Style.keys_list():
             style = Style[style.upper()]
         else:
-            assert ValueError(
+            raise ValueError(
                 'Style "{st}" is not supported, use one of {sts}.'.format(
                     st=style,
                     sts=Style.keys_list(),
                 ),
             )
         _pplt.STYLE = style
 
-        if _pplt.STYLE is Style.NONE:
-            _reset_style()
+    if mode is not None:
+        if isinstance(mode, Mode):
+            pass
+        elif isinstance(mode, str) and mode.upper() in Mode.keys_list():
+            mode = Mode[mode.upper()]
         else:
-            # load static rcParams
-            _apply_style('stylelib/default.mplstyle')
-            if _pplt.STYLE is Style.MINIMAL:
-                _apply_style('stylelib/minimal.mplstyle')
-
-            # set color cycle and cmap
-            _set_rc_colors(
-                colors=colors, cmap=cmap, ncs=ncs, true_black=true_black,
+            raise ValueError(
+                'Mode "{mode}" is not supported, use one of {modes}.'.format(
+                    mode=mode,
+                    modes=Mode.keys_list(),
+                ),
             )
 
-            # set figsize
+        _pplt.MODE = mode
+
+    # set style variables in dictionary
+    for key, val in (
+        ('interactive', interactive),
+        ('colors', colors),
+        ('cmap', cmap),
+        ('ncs', ncs),
+        ('figsize', figsize),
+        ('figratio', figratio),
+        ('ipython', ipython),
+        ('true_black', true_black),
+        ('latex', latex),
+        ('sf', sf),
+    ):
+        if val is not None:
+            _pplt.STYLE_DICT[key] = val
+
+    if _pplt.STYLE is Style.NONE:
+        _reset_style()
+    else:
+        # load static rcParams
+        _apply_style('stylelib/default.mplstyle')
+        if _pplt.STYLE is Style.MINIMAL:
+            _apply_style('stylelib/minimal.mplstyle')
+
+        # set color cycle and cmap
+        _set_rc_colors(
+            colors=colors, cmap=cmap, ncs=ncs, true_black=true_black,
+        )
+
+        # set figsize
+        if figsize is not None:
             _set_rc_figsize(figratio=figratio, figsize=figsize)
 
-            # change widths and fontsize depending on MODE
-            _set_rc_widths(mode)
+        # increase dpi if not in iypthon
+        _set_rc_dpi(ipython)
 
-            # increase dpi if not in iypthon
-            _set_rc_dpi(ipython)
+        # set interactive mode
+        _set_ineractive_mode(interactive=interactive)
 
-    # set interactive mode
-    _set_ineractive_mode(interactive=interactive)
+        # setup LaTeX font
+        # plt.style.use can not be used.
+        if latex:
+            _apply_style('stylelib/latex.mplstyle')
 
-    # setup LaTeX font
-    # plt.style.use can not be used.
-    if latex is not None and latex:
-        _apply_style('stylelib/latex.mplstyle')
+        if sf:
+            _set_rc_sansserif()
 
-    if sf:
-        _set_rc_sansserif()
+    if mode is not None:
+        # change widths and fontsize depending on MODE
+        _set_rc_widths(mode)
 
 
 @copy_doc_params(update_style)
 def use_style(
     interactive=None,
     colors='pastel5',
     cmap='macaw',
@@ -284,28 +302,29 @@
         ipython=ipython,
         true_black=true_black,
         latex=latex,
         sf=False,
     )
 
 
-def _set_rc_colors(colors, cmap, ncs, true_black):
+def _set_rc_colors(colors, cmap, true_black, ncs):
     """Set rcParams colors."""
     # set color cycle and cmap
-    if colors is not None:
-        try:
-            # try if discrete cmap was selected
-            color_cycler = plt.cycler(color=plt.get_cmap(colors).colors)
-        except AttributeError:
-            color_cycler = plt.cycler(
-                color=plt.get_cmap(colors)(np.linspace(0, 1, ncs)),
-            )
-
-        # TODO: refactor following code in private function
-        plt.rcParams['axes.prop_cycle'] = color_cycler
+    if colors is not None or ncs is not None:
+        # use values of previous call in case of None
+        colors = colors if colors is not None else _pplt.STYLE_DICT['colors']
+        ncs = ncs if ncs is not None else _pplt.STYLE_DICT['ncs']
+
+        clrs = plt.get_cmap(colors)
+        plt.rcParams['axes.prop_cycle'] = plt.cycler(
+            color=(
+                clrs.colors if tools.is_discrete_cmap(colors) else
+                clrs(np.linspace(0, 1, ncs))
+            ),
+        )
 
     if cmap is not None:
         plt.rcParams['image.cmap'] = cmap
 
     if true_black is not None:
         # change default colors
         if true_black:
@@ -322,19 +341,16 @@
             'ytick.color': grays.dark,
             'grid.color': grays.light,
         })
 
 
 def _set_rc_figsize(figratio, figsize):
     """Set rcParams figsize."""
-    # convert figratio to value
-    figratio = tools.parse_figratio(figratio)
-
     # setup figsize
-    figsize = tools.parse_figsize(figsize, figratio)
+    figsize = _parse_figsize(figsize, figratio)
 
     if figsize is not None:
         plt.rcParams['figure.figsize'] = figsize
 
 
 def _set_rc_widths(mode):
     """Set rcParams widths and fontsizes according to mode."""
@@ -461,7 +477,82 @@
 def _apply_style(path):
     """Load mplstyle file at given relative path to this file."""
     module_dir = ospath.dirname(__file__)
     path = ospath.join(module_dir, path)
 
     # load and apply style
     plt.style.use(path)
+
+
+def _parse_figratio(figratio):
+    """Parse the figratio value.
+
+    Parameters
+    ----------
+    figratio : float or one of ['sqrt(2)', 'sqrt(3)', 'golden']
+        Parse the figratio to an numeric value.
+
+    Returns
+    -------
+    figratio : float
+        Numeric figratio.
+
+    """
+    if figratio is None:
+        figratio = _pplt.STYLE_DICT['figratio']
+    elif tools.is_number(figratio):
+        figratio = float(figratio)
+    else:
+        figratios = {
+            'sqrt(2)': np.sqrt(2),
+            'sqrt(3)': np.sqrt(3),
+            'golden': (1 + np.sqrt(5)) / 2,
+        }
+        if figratio not in figratios:
+            raise ValueError(
+                'figratio needs to be an numeric value or one of [' +
+                '{0}].'.format(', '.join(figratios.keys())),
+            )
+        figratio = figratios.get(figratio, None)
+    return figratio
+
+
+def _parse_figsize(figsize, figratio):
+    """Parse the figsize value.
+
+    Parameters
+    ----------
+    figsize : float or tuple of floats
+        Parse the figsize (in inches) to an numeric value. If only a single
+        value is given, the figratio will be used for the second dimension.
+    figratio : float or one of ['sqrt(2)', 'sqrt(3)', 'golden'], optional
+        Parse the figratio to an numeric value, see `parse_figsize`.
+
+    Returns
+    -------
+    figsize : tuple
+        Tuple of figsize in inches (x, y).
+
+    """
+    figsize = tuple(np.atleast_1d(figsize))
+    if not all(tools.is_number(size) for size in figsize):
+        sizetuple = None
+    elif len(figsize) == 1 and figratio is None:
+        raise ValueError(
+            'using single value for `figsize` requires `figratio` but was not'
+            ' specified yet.',
+        )
+    elif len(figsize) == 1:
+        figratio = _parse_figratio(figratio)
+        figsize = float(figsize[0])
+        sizetuple = (figsize, figsize / figratio)
+    elif len(figsize) == 2:
+        sizetuple = figsize
+    else:
+        sizetuple = None
+
+    if sizetuple is None:
+        raise ValueError(
+            'figsize needs to be an numeric value or a tuple, not ' +
+            '{0}.'.format(figsize),
+        )
+    return sizetuple
```

### Comparing `prettypyplot-0.8.0/prettypyplot/stylelib/default.mplstyle` & `prettypyplot-0.9.0/src/prettypyplot/stylelib/default.mplstyle`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/subplots.py` & `prettypyplot-0.9.0/src/prettypyplot/subplots.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot/texts.py` & `prettypyplot-0.9.0/src/prettypyplot/texts.py`

 * *Files identical despite different names*

### Comparing `prettypyplot-0.8.0/prettypyplot.egg-info/PKG-INFO` & `prettypyplot-0.9.0/src/prettypyplot.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,213 +1,219 @@
 Metadata-Version: 2.1
 Name: prettypyplot
-Version: 0.8.0
+Version: 0.9.0
 Summary: Wrapper for matplotlib to generate pretty plots.
 Home-page: https://gitlab.com/braniii/prettypyplot
 Author: braniii
 License: BSD 3-Clause License
-Description: <div align="center">
-          <img
-            src="https://gitlab.com/braniii/prettypyplot/-/raw/master/gallery/logo_large.png"
-          />
-        
-          <p>
-            <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide" >
-                <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
-            <a href="https://gitlab.com/braniii/prettypyplot/pipelines" alt="Gitlab pipeline status" >
-                <img src="https://img.shields.io/gitlab/pipeline/braniii/prettypyplot" /></a>
-            <a href="https://gitlab.com/braniii/prettypyplot/-/commits/master">
-                <img alt="coverage report" src="https://gitlab.com/braniii/prettypyplot/badges/master/coverage.svg" /></a>
-            <a href="https://pypi.org/project/prettypyplot" alt="PyPI" >
-                <img src="https://img.shields.io/pypi/v/prettypyplot" /></a>
-            <a href="https://pepy.tech/project/prettypyplot" alt="Downloads" >
-                <img src="https://pepy.tech/badge/prettypyplot" /></a>
-            <a href="https://img.shields.io/pypi/pyversions/prettypyplot" alt="PyPI - Python Version">
-                <img src="https://img.shields.io/pypi/pyversions/prettypyplot" /></a>
-            <a href="https://gitlab.com/braniii/prettypyplot/-/blob/master/LICENSE" alt="PyPI - License" >
-                <img src="https://img.shields.io/pypi/l/prettypyplot" /></a>
-            <a href="https://braniii.gitlab.io/prettypyplot" alt="Doc" >
-                <img src="https://img.shields.io/badge/pdoc3-Documentation-brightgreen" /></a>
-          </p>
-        
-          <p>
-            <a href="https://braniii.gitlab.io/prettypyplot">Docs</a> •
-            <a href="#features">Features</a> •
-            <a href="#Installation">Installation</a> •
-            <a href="#usage">Usage</a>
-          </p>
-        </div>
-        
-        
-        
-        # prettypyplot
-        
-        The documentation including an gallery can be found [here](https://braniii.gitlab.io/prettypyplot).
-        
-        This is a wrapper package for matplotlib to achieve more easily pretty figures.
-        If you are looking for something complete, this project is nothing for you
-        but maybe [seaborn](https://seaborn.pydata.org/). The main aspect of this
-        project is to help me syncing my rcParams files and to stop copy-pasting so
-        much code.
-        
-        The aim of this project is to simplify the generation of some simple
-        pre-defined figures. Almost all code is inspired or taken from the
-        [matplotlib gallery](https://matplotlib.org/gallery/index.html). If you are a
-        power user or interested in generating complex figures, this packages is not
-        ment for you and you should better take a look in the matplotlib gallery
-        directly.
-        
-        This project is in an alpha stage, hence it is neither stable nor ready for
-        production.
-        > **CAUTION**:
-        > Starting from version 1.0.0 (which is far in the future) API-breaking
-        > changes will be made only in major releases. Until then, it can be changed
-        > in every minor release (see [changelog](#changelog)).
-        
-        ## Features
-        
-        The most notable features are:
-        
-        - figsize specifies size of canvas. So labels, ticks or colorbars are not counted.
-        - Nice top-aligned outter legends
-        - New colors
-        
-        ## Usage
-        
-        This package uses an syntax very close to matplotlib. Hence, it should be
-        straight forward to use it. Instead of calling a function on the axes itself,
-        one needs to pass here the axes as an argument (args or kwargs).
-        
-        ### Installation
-        
-        ```python
-        python3 -m pip install --upgrade prettypyplot
-        ```
-        or for the latest dev version
-        ```python
-        python3 -m pip install git+https://gitlab.com/braniii/prettypyplot.git
-        ```
-        
-        ### Usage
-        
-        ```python
-        import matplotlib.pyplot as plt
-        import prettypyplot as pplt
-        
-        pplt.use_style()
-        fig, ax = plt.subplots()
-        ...
-        pplt.plot(ax=ax, x, y)
-        pplt.savefig(output)
-        ```
-        
-        ### Known Bugs
-        
-        - `plt.subplots_adjust()` does not work with `pplt.savefig(use_canvas_size=True)`
-        If you find one, please open an issue.
-        - `pplt.savefig(use_canvas_size=True)` is not compatible with a grid of subplots
-        
-        ### Known Workarounds
-        
-        The method `pyplot.subplots_adjust()` is not compatible with the option
-        `use_canvas_size` in `prettypyplot.plot.savefig`,
-        use instead:
-        ```python
-        # this doesn't work, use instead gridspec
-        fig.subplots_adjust(hspace=0)
-        # use this instead
-        fig, axs = plt.subplots(..., gridspec_kw={'hspace': 0.000})
-        ```
-        
-        ## Comparison to `matplotlib`
-        
-        <table>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.plot</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.plot</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot.png" width="350">
-                </td>
-            </tr>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.legend</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot_legend.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.legend</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot_legend.png" width="350">
-                </td>
-            </tr>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.imshow</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.imshow</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow.png" width="350">
-                </td>
-            </tr>
-            <tr width="700" valign="top">
-                <td>
-                    <code>matplotlib.pyplot.colorbar</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow_cbar.png" width="350">
-                </td>
-                <td>
-                    <code>prettypyplot.colorbar</code><br>
-                    <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow_cbar.png" width="350">
-                </td>
-            </tr>
-        </table>
-        
-        ## Roadmap:
-        
-        The following list is sorted from *near future* to *hopefully ever*.
-        
-        - [x] add pytest
-        - [x] add search functionality in doc
-        - [x] refactoring code to improve readabilty
-        - [ ] add more colorpalettes
-        - [ ] add countour line plot
-        - [ ] add [axes_grid](https://matplotlib.org/3.1.1/tutorials/toolkits/axes_grid.html) examples
-        - [ ] add more gallery entries
-        - [ ] add package to conda_forge
-        - [ ] improve `plt.suplots()` behaviour together with `pplt.savefig()`
-        - [ ] setup widths and scaling factors for beamer and poster mode
-        - [ ] tweak all function to enable `STYLE='minimal'`
-        - [ ] implement tufte style
-        
-        ## Building Documentation:
-        
-        The doc is based on [pdoc](https://pdoc3.github.io/pdoc/) and can be created by
-        simply running `bash create_doc.sh` from the docs folder. For dependencies see in the
-        CI action.
-        
-        ## Similar Projects
-        
-        - [seaborn](https://seaborn.pydata.org/)
-        
-        ## Credits:
-        
-        In alphabetical order:
-        
-        - [colorcyclepicker](https://colorcyclepicker.mpetroff.net/)
-        - [coolors](https://coolors.co/)
-        - [matplotlib](https://matplotlib.org/)
-        - [prettyplotlib](https://github.com/olgabot/prettyplotlib)
-        - [realpython](https://realpython.com/)
-        - [viscm](https://github.com/matplotlib/viscm)
-        
 Keywords: matplotlib pyplot
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: docs
+Provides-Extra: all
+License-File: LICENSE
+
+<div align="center">
+  <img
+    src="https://gitlab.com/braniii/prettypyplot/-/raw/master/gallery/logo_large.png"
+  />
+
+  <p>
+    <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide" >
+        <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
+    <a href="https://gitlab.com/braniii/prettypyplot/pipelines" alt="Gitlab pipeline status" >
+        <img src="https://img.shields.io/gitlab/pipeline/braniii/prettypyplot" /></a>
+    <a href="https://gitlab.com/braniii/prettypyplot/-/commits/master">
+        <img alt="coverage report" src="https://gitlab.com/braniii/prettypyplot/badges/master/coverage.svg" /></a>
+    <a href="https://pypi.org/project/prettypyplot" alt="PyPI" >
+        <img src="https://img.shields.io/pypi/v/prettypyplot" /></a>
+    <a href="https://pepy.tech/project/prettypyplot" alt="Downloads" >
+        <img src="https://pepy.tech/badge/prettypyplot" /></a>
+    <a href="https://img.shields.io/pypi/pyversions/prettypyplot" alt="PyPI - Python Version">
+        <img src="https://img.shields.io/pypi/pyversions/prettypyplot" /></a>
+    <a href="https://gitlab.com/braniii/prettypyplot/-/blob/master/LICENSE" alt="PyPI - License" >
+        <img src="https://img.shields.io/pypi/l/prettypyplot" /></a>
+    <a href="https://braniii.gitlab.io/prettypyplot" alt="Doc" >
+        <img src="https://img.shields.io/badge/pdoc3-Documentation-brightgreen" /></a>
+  </p>
+
+  <p>
+    <a href="https://braniii.gitlab.io/prettypyplot">Docs</a> •
+    <a href="#features">Features</a> •
+    <a href="#Installation">Installation</a> •
+    <a href="#usage">Usage</a>
+  </p>
+</div>
+
+
+
+# prettypyplot
+
+The documentation including an gallery can be found [here](https://braniii.gitlab.io/prettypyplot).
+
+This is a wrapper package for matplotlib to achieve more easily pretty figures.
+If you are looking for something complete, this project is nothing for you
+but maybe [seaborn](https://seaborn.pydata.org/). The main aspect of this
+project is to help me syncing my rcParams files and to stop copy-pasting so
+much code.
+
+The aim of this project is to simplify the generation of some simple
+pre-defined figures. Almost all code is inspired or taken from the
+[matplotlib gallery](https://matplotlib.org/gallery/index.html). If you are a
+power user or interested in generating complex figures, this packages is not
+ment for you and you should better take a look in the matplotlib gallery
+directly.
+
+This project is in an alpha stage, hence it is neither stable nor ready for
+production.
+> **CAUTION**:
+> Starting from version 1.0.0 (which is far in the future) API-breaking
+> changes will be made only in major releases. Until then, it can be changed
+> in every minor release (see [changelog](#changelog)).
+
+## Features
+
+The most notable features are:
+
+- figsize specifies size of canvas. So labels, ticks or colorbars are not counted.
+- Nice top-aligned outter legends
+- New colors
+
+## Usage
+
+This package uses an syntax very close to matplotlib. Hence, it should be
+straight forward to use it. Instead of calling a function on the axes itself,
+one needs to pass here the axes as an argument (args or kwargs).
+
+### Installation
+
+```python
+python3 -m pip install --upgrade prettypyplot
+```
+or for the latest dev version
+```python
+python3 -m pip install git+https://gitlab.com/braniii/prettypyplot.git
+```
+
+### Usage
+
+```python
+import matplotlib.pyplot as plt
+import prettypyplot as pplt
+
+pplt.use_style()
+fig, ax = plt.subplots()
+...
+pplt.plot(ax=ax, x, y)
+pplt.savefig(output)
+```
+
+### Known Bugs
+
+- `plt.subplots_adjust()` does not work with `pplt.savefig(use_canvas_size=True)`
+If you find one, please open an issue.
+- `pplt.savefig(use_canvas_size=True)` is not compatible with a grid of subplots
+
+### Known Workarounds
+
+The method `pyplot.subplots_adjust()` is not compatible with the option
+`use_canvas_size` in `prettypyplot.plot.savefig`,
+use instead:
+```python
+# this doesn't work, use instead gridspec
+fig.subplots_adjust(hspace=0)
+# use this instead
+fig, axs = plt.subplots(..., gridspec_kw={'hspace': 0.000})
+```
+
+## Comparison to `matplotlib`
+
+<table>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.plot</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.plot</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot.png" width="350">
+        </td>
+    </tr>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.legend</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_plot_legend.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.legend</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_plot_legend.png" width="350">
+        </td>
+    </tr>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.imshow</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.imshow</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow.png" width="350">
+        </td>
+    </tr>
+    <tr width="700" valign="top">
+        <td>
+            <code>matplotlib.pyplot.colorbar</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/mpl_imshow_cbar.png" width="350">
+        </td>
+        <td>
+            <code>prettypyplot.colorbar</code><br>
+            <img src="https://braniii.gitlab.io/prettypyplot/gallery/default_imshow_cbar.png" width="350">
+        </td>
+    </tr>
+</table>
+
+## Roadmap:
+
+The following list is sorted from *near future* to *hopefully ever*.
+
+- [x] add pytest
+- [x] add search functionality in doc
+- [x] refactoring code to improve readabilty
+- [ ] add more colorpalettes
+- [ ] add countour line plot
+- [ ] add [axes_grid](https://matplotlib.org/3.1.1/tutorials/toolkits/axes_grid.html) examples
+- [ ] add more gallery entries
+- [ ] add package to conda_forge
+- [ ] improve `plt.suplots()` behaviour together with `pplt.savefig()`
+- [ ] setup widths and scaling factors for beamer and poster mode
+- [ ] tweak all function to enable `STYLE='minimal'`
+- [ ] implement tufte style
+
+## Building Documentation:
+
+The doc is based on [pdoc](https://pdoc3.github.io/pdoc/) and can be created by
+simply running `bash create_doc.sh` from the docs folder. For dependencies see in the
+CI action.
+
+## Similar Projects
+
+- [seaborn](https://seaborn.pydata.org/)
+
+## Credits:
+
+In alphabetical order:
+
+- [colorcyclepicker](https://colorcyclepicker.mpetroff.net/)
+- [coolors](https://coolors.co/)
+- [matplotlib](https://matplotlib.org/)
+- [prettyplotlib](https://github.com/olgabot/prettyplotlib)
+- [realpython](https://realpython.com/)
+- [viscm](https://github.com/matplotlib/viscm)
+
+
```

#### html2text {}

```diff
@@ -1,10 +1,17 @@
-Metadata-Version: 2.1 Name: prettypyplot Version: 0.8.0 Summary: Wrapper for
+Metadata-Version: 2.1 Name: prettypyplot Version: 0.9.0 Summary: Wrapper for
 matplotlib to generate pretty plots. Home-page: https://gitlab.com/braniii/
-prettypyplot Author: braniii License: BSD 3-Clause License Description:
+prettypyplot Author: braniii License: BSD 3-Clause License Keywords: matplotlib
+pyplot Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Python: >=3.6 Description-Content-Type:
+text/markdown Provides-Extra: testing Provides-Extra: docs Provides-Extra: all
+License-File: LICENSE
  [https://gitlab.com/braniii/prettypyplot/-/raw/master/gallery/logo_large.png]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_t_y_l_e_-_w_e_m_a_k_e_-_0_0_0_0_0_0_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _g_i_t_l_a_b_/_p_i_p_e_l_i_n_e_/_b_r_a_n_i_i_i_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_c_o_v_e_r_a_g_e_ _r_e_p_o_r_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
       _p_y_p_i_/_v_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
   _p_r_e_t_t_y_p_y_p_l_o_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_d_o_c_3_-_D_o_c_u_m_e_n_t_a_t_i_o_n_-_b_r_i_g_h_t_g_r_e_e_n_]
                  _D_o_c_s â¢ _F_e_a_t_u_r_e_s â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _U_s_a_g_e
@@ -66,14 +73,8 @@
 Building Documentation: The doc is based on [pdoc](https://pdoc3.github.io/
 pdoc/) and can be created by simply running `bash create_doc.sh` from the docs
 folder. For dependencies see in the CI action. ## Similar Projects - [seaborn]
 (https://seaborn.pydata.org/) ## Credits: In alphabetical order: -
 [colorcyclepicker](https://colorcyclepicker.mpetroff.net/) - [coolors](https://
 coolors.co/) - [matplotlib](https://matplotlib.org/) - [prettyplotlib](https://
 github.com/olgabot/prettyplotlib) - [realpython](https://realpython.com/) -
-[viscm](https://github.com/matplotlib/viscm) Keywords: matplotlib pyplot
-Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Python: >=3.6 Description-Content-Type:
-text/markdown
+[viscm](https://github.com/matplotlib/viscm)
```

### Comparing `prettypyplot-0.8.0/setup.cfg` & `prettypyplot-0.9.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -2,41 +2,42 @@
 addopts = 
 	--strict-markers
 	--doctest-modules
 	--mpl
 	--reruns 5
 	--reruns-delay 1
 	--cov-report term-missing
-	--cov=prettypyplot test/
+	--cov=src/prettypyplot tests/
 
 [flake8]
 format = wemake
 show-source = True
 statistics = True
 doctests = True
 count = True
 max-local-variables = 10
 max-module-members = 14
 rst-roles = class, func, ref
 rst-directives = todo
 max-complexity = 10
 ignore = S101, C101, N, DAR401, DAR402, W504, WPS306, SC
+exclude = .git, src/prettypyplot/__pycache__, docs, build, dist
 per-file-ignores = 
-	prettypyplot/cmaps/*.py:WPS339, E501
-	prettypyplot/*__init__.py:E402, F401, F403, D104, D400
-	prettypyplot/decorators.py:WPS430
+	src/prettypyplot/cmaps/*.py:WPS339, E501
+	src/prettypyplot/*__init__.py:E402, F401, F403, D104, D400
+	src/prettypyplot/decorators.py:WPS430
 	setup.py:D100
-	test/*.py:WPS, DAR101, DAR201
+	tests/*.py:WPS, DAR101, DAR201
 
 [isort]
 include_trailing_comma = true
 multi_line_output = 3
 line_length = 79
 skip = 
-	prettypyplot/__init__.py
+	src/prettypyplot/__init__.py
 
 [darglint]
 strictness = short
 docstring_style = numpy
 ignore_regex = ^_(.*)
 
 [egg_info]
```

