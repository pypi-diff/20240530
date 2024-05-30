# Comparing `tmp/erlab-2.5.4.tar.gz` & `tmp/erlab-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.5.4.tar", last modified: Thu May 23 07:37:12 2024, max compression
+gzip compressed data, was "erlab-2.6.1.tar", last modified: Thu May 30 18:00:17 2024, max compression
```

## Comparing `erlab-2.5.4.tar` & `erlab-2.6.1.tar`

### file list

```diff
@@ -1,200 +1,207 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.394111 erlab-2.5.4/
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-23 07:37:02.000000 erlab-2.5.4/.codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.342112 erlab-2.5.4/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.350112 erlab-2.5.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-05-23 07:37:02.000000 erlab-2.5.4/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-23 07:37:02.000000 erlab-2.5.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-23 07:37:02.000000 erlab-2.5.4/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.350112 erlab-2.5.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1668 2024-05-23 07:37:02.000000 erlab-2.5.4/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     2535 2024-05-23 07:37:02.000000 erlab-2.5.4/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-23 07:37:02.000000 erlab-2.5.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1022 2024-05-23 07:37:02.000000 erlab-2.5.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-05-23 07:37:02.000000 erlab-2.5.4/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   129560 2024-05-23 07:37:08.000000 erlab-2.5.4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-05-23 07:37:02.000000 erlab-2.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48973 2024-05-23 07:37:12.390112 erlab-2.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-05-23 07:37:02.000000 erlab-2.5.4/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5552 2024-05-23 07:37:02.000000 erlab-2.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.350112 erlab-2.5.4/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.354112 erlab-2.5.4/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    18220 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15203 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     5039 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.362112 erlab-2.5.4/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.362112 erlab-2.5.4/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.366112 erlab-2.5.4/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    42435 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)    12039 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54817 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    27572 2024-05-23 07:37:02.000000 erlab-2.5.4/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-23 07:37:02.000000 erlab-2.5.4/environment.yml
--rw-r--r--   0 root         (0) root         (0)     5938 2024-05-23 07:37:02.000000 erlab-2.5.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-23 07:37:02.000000 erlab-2.5.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 07:37:12.394111 erlab-2.5.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.346112 erlab-2.5.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.366112 erlab-2.5.4/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-23 07:37:08.000000 erlab-2.5.4/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.366112 erlab-2.5.4/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26366 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    30007 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)    14898 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.370112 erlab-2.5.4/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.370112 erlab-2.5.4/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.370112 erlab-2.5.4/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10779 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9594 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12774 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20223 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    27520 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    14968 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.370112 erlab-2.5.4/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5397 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8505 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.370112 erlab-2.5.4/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.374112 erlab-2.5.4/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14181 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21371 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23038 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11816 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19376 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.374112 erlab-2.5.4/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    17433 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.374112 erlab-2.5.4/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52053 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114641 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27909 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    57841 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    14551 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25642 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16014 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19321 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    56647 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.378112 erlab-2.5.4/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2194 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.378112 erlab-2.5.4/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    43727 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12460 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.378112 erlab-2.5.4/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     6987 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/plugins/maestro.py
--rw-r--r--   0 root         (0) root         (0)     8167 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7667 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     7123 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1522 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.382112 erlab-2.5.4/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.382112 erlab-2.5.4/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30848 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18686 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4420 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39811 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    38540 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-23 07:37:02.000000 erlab-2.5.4/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.390112 erlab-2.5.4/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48973 2024-05-23 07:37:12.000000 erlab-2.5.4/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5297 2024-05-23 07:37:12.000000 erlab-2.5.4/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 07:37:12.000000 erlab-2.5.4/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      667 2024-05-23 07:37:12.000000 erlab-2.5.4/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-23 07:37:12.000000 erlab-2.5.4/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-23 07:37:02.000000 erlab-2.5.4/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-23 07:37:02.000000 erlab-2.5.4/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-23 07:37:02.000000 erlab-2.5.4/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4150 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/tests/analysis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/tests/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/fit/test_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/fit/test_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/fit/test_minuit.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/fit/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_gold.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     3909 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_image_savgol.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.386112 erlab-2.5.4/tests/interactive/
--rw-r--r--   0 root         (0) root         (0)     4374 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/interactive/test_imagetool.py
--rw-r--r--   0 root         (0) root         (0)     4352 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/interactive/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.390112 erlab-2.5.4/tests/io/
--rw-r--r--   0 root         (0) root         (0)    10032 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/io/test_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:37:12.390112 erlab-2.5.4/tests/plotting/
--rw-r--r--   0 root         (0) root         (0)     1305 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/plotting/test_annotations.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/plotting/test_atoms.py
--rw-r--r--   0 root         (0) root         (0)     2015 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/plotting/test_colors.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/plotting/test_general.py
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-23 07:37:02.000000 erlab-2.5.4/tests/test_constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.658880 erlab-2.6.1/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-30 18:00:07.000000 erlab-2.6.1/.codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.606880 erlab-2.6.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.610880 erlab-2.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.610880 erlab-2.6.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-05-30 18:00:07.000000 erlab-2.6.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 18:00:07.000000 erlab-2.6.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-30 18:00:07.000000 erlab-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-30 18:00:07.000000 erlab-2.6.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   133751 2024-05-30 18:00:13.000000 erlab-2.6.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-05-30 18:00:07.000000 erlab-2.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48973 2024-05-30 18:00:17.658880 erlab-2.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-05-30 18:00:07.000000 erlab-2.6.1/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5552 2024-05-30 18:00:07.000000 erlab-2.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.614880 erlab-2.6.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.618880 erlab-2.6.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    18220 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/erlab.utils.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.622880 erlab-2.6.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)  1014848 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   986936 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.626880 erlab-2.6.1/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.626880 erlab-2.6.1/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    42487 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    13061 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54813 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27572 2024-05-30 18:00:07.000000 erlab-2.6.1/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-30 18:00:07.000000 erlab-2.6.1/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5938 2024-05-30 18:00:07.000000 erlab-2.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-30 18:00:07.000000 erlab-2.6.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 18:00:17.658880 erlab-2.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.606880 erlab-2.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.626880 erlab-2.6.1/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-30 18:00:13.000000 erlab-2.6.1/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.630880 erlab-2.6.1/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26568 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    16387 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.630880 erlab-2.6.1/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.630880 erlab-2.6.1/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.634880 erlab-2.6.1/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12774 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20221 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    27488 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.634880 erlab-2.6.1/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     8795 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     5435 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/analysis/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.634880 erlab-2.6.1/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      721 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23034 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19370 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    17431 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114637 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    29113 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    58013 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    26142 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16010 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19321 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2745 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)      257 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/utilities.py
+-rw-r--r--   0 root         (0) root         (0)    57036 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/interactive/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.638880 erlab-2.6.1/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.642880 erlab-2.6.1/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    45761 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12460 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.642880 erlab-2.6.1/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     6985 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/maestro.py
+-rw-r--r--   0 root         (0) root         (0)     8373 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7647 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     7123 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/io/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/lattice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.642880 erlab-2.6.1/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.646880 erlab-2.6.1/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30848 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39811 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    38592 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.646880 erlab-2.6.1/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.646880 erlab-2.6.1/src/erlab/utils/
+-rw-r--r--   0 root         (0) root         (0)      177 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/utils/array.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-05-30 18:00:07.000000 erlab-2.6.1/src/erlab/utils/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.654880 erlab-2.6.1/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48973 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5458 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-30 18:00:17.000000 erlab-2.6.1/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-30 18:00:07.000000 erlab-2.6.1/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-30 18:00:07.000000 erlab-2.6.1/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-30 18:00:07.000000 erlab-2.6.1/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/analysis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_minuit.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/fit/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_gold.py
+-rw-r--r--   0 root         (0) root         (0)     5791 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_image_savgol.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_mask.py
+-rw-r--r--   0 root         (0) root         (0)      714 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/analysis/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.650880 erlab-2.6.1/tests/interactive/
+-rw-r--r--   0 root         (0) root         (0)     4375 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/interactive/test_imagetool.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/interactive/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.654880 erlab-2.6.1/tests/io/
+-rw-r--r--   0 root         (0) root         (0)    10028 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:00:17.654880 erlab-2.6.1/tests/plotting/
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_annotations.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_atoms.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_colors.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/plotting/test_general.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-30 18:00:07.000000 erlab-2.6.1/tests/test_constants.py
```

### Comparing `erlab-2.5.4/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.6.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.6.1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/.github/workflows/pr.yml` & `erlab-2.6.1/.github/workflows/pr.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Test
 
 on:
   pull_request:
 
+env:
+  FORCE_COLOR: 1
+
 jobs:
   test:
     name: Python ${{ matrix.python-version }} tests
     runs-on: ubuntu-latest
     env:
       DISPLAY: ':99.0'
       PYTHONDONTWRITEBYTECODE : 1
@@ -35,19 +38,19 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install -v .[complete] pyqt6
 
       - name: Test with pytest
         if: matrix.python-version != '3.12'
         run: |
-          pytest -v -n 2 --dist worksteal
+          pytest
 
       - name: Test with pytest with coverage
         if: matrix.python-version == '3.12'
         run: |
-          pytest --cov erlab --cov-report xml -v -n 2 --dist worksteal
+          pytest --cov erlab --cov-report xml
 
       - name: Upload coverage to Codecov
         if: matrix.python-version == '3.12'
         uses: codecov/codecov-action@v4.0.1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `erlab-2.5.4/.github/workflows/release.yml` & `erlab-2.6.1/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 name: Release
 
 on:
   push:
     branches: [ "main" ]
   workflow_dispatch:
 
+env:
+  FORCE_COLOR: 1
+
 jobs:
   test:
     name: Python ${{ matrix.python-version }} tests
     runs-on: ubuntu-latest
     env:
       DISPLAY: ':99.0'
       PYTHONDONTWRITEBYTECODE : 1
@@ -34,20 +37,20 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install -v .[complete] pyqt6
 
       - name: Test with pytest
         if: matrix.python-version != '3.12'
         run: |
-          pytest -v -n 2 --dist worksteal
+          pytest
 
       - name: Test with pytest with coverage
         if: matrix.python-version == '3.12'
         run: |
-          pytest --cov erlab --cov-report xml -v -n 2 --dist worksteal
+          pytest --cov erlab --cov-report xml
 
       - name: Upload coverage to Codecov
         if: matrix.python-version == '3.12'
         uses: codecov/codecov-action@v4.0.1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `erlab-2.5.4/.gitignore` & `erlab-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/.pre-commit-config.yaml` & `erlab-2.6.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,14 @@
       - id: check-merge-conflict
       - id: mixed-line-ending
       - id: check-ast
 
   # Lint and format with ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.4.4
+    rev: v0.4.5
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
```

### Comparing `erlab-2.5.4/.readthedocs.yaml` & `erlab-2.6.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/CHANGELOG.md` & `erlab-2.6.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,78 @@
 # CHANGELOG
 
 
 
+## v2.6.1 (2024-05-30)
+
+### Fix
+
+* re-trigger due to CI failure ([`b6d69b5`](https://github.com/kmnhan/erlabpy/commit/b6d69b556e3d0dbe6d8d71596e32d9d7cfdc5267))
+
+
+## v2.6.0 (2024-05-30)
+
+### Ci
+
+* (**github**) disable parallel testing ([`fd024f5`](https://github.com/kmnhan/erlabpy/commit/fd024f5f1d6870ff6c30ee32ee8c3a708245a958))
+
+* (**github**) enable color output ([`44071db`](https://github.com/kmnhan/erlabpy/commit/44071db669e66a39d025d23d63962399c59d9e1b))
+
+* (**pre-commit**) pre-commit autoupdate ([`acb9c1c`](https://github.com/kmnhan/erlabpy/commit/acb9c1c31cfa8595512f30820b713c6bd1205983))
+
+  updates: - [github.com/astral-sh/ruff-pre-commit: v0.4.4 → v0.4.5](https://github.com/astral-sh/ruff-pre-commit/compare/v0.4.4...v0.4.5)
+
+### Documentation
+
+* add `qsel.around` to indexing guide ([`1f95659`](https://github.com/kmnhan/erlabpy/commit/1f95659ae30a432d2fd91ec8c669c39a33b41f15))
+
+### Feature
+
+* (**interactive.imagetool**) add bin amount label to binning controls ([`7a7a692`](https://github.com/kmnhan/erlabpy/commit/7a7a692b881e4cc1bd49342f31f3fe50407d72b5))
+
+* add accessor for selecting around a point ([`aa24457`](https://github.com/kmnhan/erlabpy/commit/aa244576fcfa17f71be0a765be8f270a6ae28080))
+
+* (**accessors.fit**) add support for background models ([`550be2d`](https://github.com/kmnhan/erlabpy/commit/550be2deebf54fab77bef591ccbe059b5b219937))
+
+  If one coordinate is given but there are two independent variables are present in the model,  the second one will be treated as the data. This makes the accessor compatible with y-dependent background models, such as the Shirley background provided in `lmfitxps`.
+
+* (**io**) make the dataloader behavior more customizable ([`4824127`](https://github.com/kmnhan/erlabpy/commit/4824127181b4383788f6dbe5cbeae4b2060f1f4f))
+
+  Now, a new `average_attrs` class attribute exists for attributes that would be averaged over multiple file scans. The current default just takes the attributes from the first file. This also works when you wish to demote a coordinate to an attribute while averaging over its values.
+  For more fine-grained control of the resulting data attributes, a new method `combine_attrs` can be overridden to take care of attributes for scans over multiple files. The default behavior is to just use the attributes from the first file.
+
+### Fix
+
+* (**plotting**) make `gradient_fill` keep axis scaling ([`51507dd`](https://github.com/kmnhan/erlabpy/commit/51507dd966a0ce2db4aabff2aac8222bee184cf8))
+
+### Refactor
+
+* (**analysis.image**) add check for 2D and uniform inputs ([`22bb02d`](https://github.com/kmnhan/erlabpy/commit/22bb02dd8dfbd5eb6b5d577abe9138a769a079b3))
+
+* try to fix synced itool garbage collection ([`932cc5a`](https://github.com/kmnhan/erlabpy/commit/932cc5a690dcebc92c65ea3f17081ac9f9c3ef8f))
+
+  This only happens in GH actions, and it doesn&#39;t happen every time so it&#39;s hard to debug.
+
+* create utils subpackage to host internal methods ([`3fa2873`](https://github.com/kmnhan/erlabpy/commit/3fa287386fc0e94e8a558e2f0e5520be869acb43))
+
+  The parallel module is now part of utils, without a compatibiliity layer or deprecation warning since nobody is using the functions from parallel anyway.
+
+* add deprecation warnings for utilities ([`5d375b8`](https://github.com/kmnhan/erlabpy/commit/5d375b8fe0766ea3f2c5fe2421937ce7309e3da5))
+
+  All submodules named `utilities.py` have been renamed to `utils.py` for consistency. The old call to `utilities.py` will still work but will raise a warning. The modules will be removed on 3.0 release.
+
+* rename `erlab.interactive.utilities` to `erlab.interactive.utils` ([`d9f1fb0`](https://github.com/kmnhan/erlabpy/commit/d9f1fb081be8d2e8710ec08421780f927341b71a))
+
+* rename `erlab.analysis.utilities` to `erlab.analysis.utils` ([`ed81b62`](https://github.com/kmnhan/erlabpy/commit/ed81b6234bd2960da785875e0aaaf2e9e5e48f15))
+
+* rename `erlab.io.utilities` to `erlab.io.utils` ([`6e0813d`](https://github.com/kmnhan/erlabpy/commit/6e0813d3873b09593ec9d539d72c7512fac77c70))
+
+* (**io.plugins.merlin**) regard temperature as coordinate ([`2fda047`](https://github.com/kmnhan/erlabpy/commit/2fda04781961f2384c711a3b1c3c00ddaecaa617))
+
+
 ## v2.5.4 (2024-05-23)
 
 ### Fix
 
 * (**io.plugins.maestro**) load correct beta for non deflector scans ([`5324c36`](https://github.com/kmnhan/erlabpy/commit/5324c362d7bdd1dcf0c21303f370fd2e77f12448))
```

### Comparing `erlab-2.5.4/LICENSE` & `erlab-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/PKG-INFO` & `erlab-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.5.4
+Version: 2.6.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.5.4/PythonInterface.ipf` & `erlab-2.6.1/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/README.md` & `erlab-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/Makefile` & `erlab-2.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/environment.yml` & `erlab-2.6.1/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/make.bat` & `erlab-2.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/conf.py` & `erlab-2.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/contributing.rst` & `erlab-2.6.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/getting-started.rst` & `erlab-2.6.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/images/flowchart_multiple.pdf` & `erlab-2.6.1/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/images/flowchart_single.pdf` & `erlab-2.6.1/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/images/ktool_1_dark.png` & `erlab-2.6.1/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/images/ktool_1_light.png` & `erlab-2.6.1/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/images/ktool_2_dark.png` & `erlab-2.6.1/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/images/ktool_2_light.png` & `erlab-2.6.1/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/index.rst` & `erlab-2.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/pyplots/norms.py` & `erlab-2.6.1/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/reference.rst` & `erlab-2.6.1/docs/source/reference.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 Subpackage                 Description
 ========================   ========================
 `erlab.analysis`           Routines for analyzing ARPES data.
 `erlab.io`                 Reading and writing data.
 `erlab.plotting`           Functions related to static plotting with matplotlib.
 `erlab.interactive`        Interactive tools and widgets based on Qt and pyqtgraph
 `erlab.accessors`          `xarray accessors <https://docs.xarray.dev/en/stable/internals/extending-xarray.html>`_. You will not need to import this module directly.
+`erlab.utils`              Utility functions and classes, typically used internally.
 ========================   ========================
 
 .. currentmodule:: erlab
 
 .. toctree::
    :hidden:
 
    erlab.analysis
    erlab.io
    erlab.plotting
    erlab.interactive
    erlab.accessors
+   erlab.utils
 
 Submodules
 ==========
 
 ==================  ==================
 Submodule           Description
 ==================  ==================
 `erlab.lattice`     Tools for working with real and reciprocal lattices.
 `erlab.constants`   Physical constants and functions for unit conversion.
-`erlab.parallel`    Helpers for parallel processing.
 ==================  ==================
 
 .. toctree::
    :hidden:
 
    erlab.lattice
    erlab.constants
-   erlab.parallel
```

### Comparing `erlab-2.5.4/docs/source/refs.bib` & `erlab-2.6.1/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.6.1/docs/source/user-guide/curve-fitting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998831601979904%*

 * *Differences: {"'cells'": "{35: {'source': {insert: [(8, '\\n'), (9, '.. note::\\n'), (10, '\\n'), (11, '    "*

 * *            "There is a dedicated module for Fermi edge fitting and correction, described\\n'), "*

 * *            "(12, '    :ref:`here <fermi edge fitting>`. The following example is for illustrative "*

 * *            "purposes.\\n')]}}, 56: {'source': {delete: [4, 3, 2, 1, 0]}}}"}*

```diff
@@ -512,14 +512,19 @@
                 "``modelfit_stderr``, respectively. The `goodness-of-fit statistics\n",
                 "<https://lmfit.github.io/lmfit-py/fitting.html#goodness-of-fit-statistics>`_ are stored\n",
                 "in ``modelfit_stats``. \n",
                 "\n",
                 "Fitting across multiple dimensions\n",
                 "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n",
                 "\n",
+                ".. note::\n",
+                "\n",
+                "    There is a dedicated module for Fermi edge fitting and correction, described\n",
+                "    :ref:`here <fermi edge fitting>`. The following example is for illustrative purposes.\n",
+                "\n",
                 "The accessor comes in handy when you have to fit a single model to multiple data points\n",
                 "across arbitrary dimensions. Let's demonstrate this with a simulated cut that represents\n",
                 "a curved Fermi edge at 100 K, with an energy broadening of 20 meV."
             ]
         },
         {
             "cell_type": "code",
@@ -843,19 +848,14 @@
                 },
                 "tags": [],
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
-                ".. note::\n",
-                "\n",
-                "    There is a dedicated module for Fermi edge fitting and correction, described\n",
-                "    :ref:`here <fermi edge fitting>`.\n",
-                "\n",
                 "Parallelization\n",
                 "~~~~~~~~~~~~~~~\n",
                 "\n",
                 "The accessors are tightly integrated with `xarray`, so passing a dask array will\n",
                 "parallelize the fitting process. See `Parallel Computing with Dask\n",
                 "<https://docs.xarray.dev/en/stable/user-guide/dask.html>`_ for more information.\n",
                 "\n",
```

### Comparing `erlab-2.5.4/docs/source/user-guide/imagetool.rst` & `erlab-2.6.1/docs/source/user-guide/imagetool.rst`

 * *Files 12% similar despite different names*

```diff
@@ -26,45 +26,50 @@
 - Easy and intuitive plot size adjustment with splitters
 - Advanced colormap control
 
 ImageTool can be used to display *image-like* :class:`xarray.DataArray`\ s ranging from
 2 to 4 dimensions. If a coordinate of the input data happens to be non-uniform, it will
 automatically be converted to an index array so that the data can be displayed.
 
-There are two main ways to invoke the ImageTool. First is to call the :func:`itool
-<erlab.interactive.imagetool.itool>` convenience function, which will create a new
-ImageTool instance and handle the event loop execution: ::
+There are two main ways to invoke the ImageTool. The first way is to call the
+:func:`itool <erlab.interactive.imagetool.itool>` convenience function, which will
+create a new ImageTool instance and handle the event loop execution: ::
 
     import erlab.interactive as eri
     eri.itool(data)
 
 Another way is to use the ``qshow`` accessor: ::
 
     data.qshow()
 
 Tips
 ----
 
-- If you don't know what a button does, many buttons have tooltips that will appear when you hover over them.
+- If you don't know what a button does, many buttons have tooltips that will appear when
+  you hover over them.
 
 - Right-clicking on each plot will bring up a context menu with various options. One
-  useful option is ``Copy selection code`` that copies the selection code which can be
-  quickly pasted to a Python script or Jupyter notebook to reproduce the sliced data.
-  You can also save the data corresponding to each slice as a HDF5 file.
+  useful menu is ``Copy selection code`` that copies the selection code which can be
+  quickly pasted to a Python script or Jupyter notebook to reproduce the data in the
+  clicked region.
 
 - ImageTool is also very extensible. At our home lab, we use a modified version of
   ImageTool to plot data as it is being collected in real-time!
 
 Keyboard shortcuts
 ------------------
 
 Hints for most keyboard shortcuts are displayed in the menu bar. Here, some shortcuts
 that are not found in the menu bar are listed. Mac users must replace :kbd:`Ctrl` with
 :kbd:`⌘` and :kbd:`Alt` with :kbd:`⌥`.
 
+The rule of thumb is that if you can do something that applies to a single cursor, you
+can do it to all cursors by holding :kbd:`Alt`. Also, keyboard shortcuts that are
+related to 'shifting' a cursor usually involves holding :kbd:`Shift`.
+
 .. list-table::
     :header-rows: 1
 
     * - Shortcut
       - Description
     * - :kbd:`LMB` Drag
       - Pan around
```

### Comparing `erlab-2.5.4/docs/source/user-guide/index.rst` & `erlab-2.6.1/docs/source/user-guide/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 core features.
 
 If you are new to programming with python, `Scientific Python Lectures
 <https://github.com/jrjohansson/scientific-python-lectures>`_ is a great place to start.
 
 Data structures in ERLabPy are represented using `xarray <https://docs.xarray.dev/>`_\
 :cite:p:`hoyer2017xarray`, which provides a powerful data structure for working with
-multi-dimensional arrays. Visit the `xarray tutorial <https://tutorial.xarray.dev/>`_
+multi-dimensional arrays. Check out the `xarray tutorial <https://tutorial.xarray.dev/>`_
 and the `xarray user guide <https://docs.xarray.dev/en/stable/index.html>`_ to get
 familiar with xarray.
 
 .. toctree::
    :caption: Table of Contents
    :maxdepth: 2
```

### Comparing `erlab-2.5.4/docs/source/user-guide/indexing.ipynb` & `erlab-2.6.1/docs/source/user-guide/indexing.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820105166572558%*

 * *Differences: {"'cells'": "{4: {'cell_type': 'markdown', 'id': '046a132c', 'metadata': {replace: OrderedDict()}, "*

 * *            '\'source\': ["We can see that the generated data is a three-dimensional DataArray. '*

 * *            'Now, let\'s extract a cut along $k_y = 0.3$."]}, 8: {\'cell_type\': \'markdown\', '*

 * *            "'id': '987121ee', 'metadata': {replace: OrderedDict()}, 'source': ['In many "*

 * *            'scenarios, it is necessary to perform integration across multiple array slices. This '*

 * *            'can be done  […]*

```diff
@@ -63,26 +63,19 @@
             },
             "outputs": [],
             "source": [
                 "dat"
             ]
         },
         {
-            "cell_type": "raw",
-            "id": "0d36f0c0",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
+            "cell_type": "markdown",
+            "id": "046a132c",
+            "metadata": {},
             "source": [
-                "We can see that the generated data is a three-dimensional :class:`xarray.DataArray` . Now, let's extract a cut along :math:`k_y = 0.3`."
+                "We can see that the generated data is a three-dimensional DataArray. Now, let's extract a cut along $k_y = 0.3$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c00a34a2",
             "metadata": {
@@ -112,26 +105,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "dat.sel(eV=0.0, method=\"nearest\")"
             ]
         },
         {
-            "cell_type": "raw",
-            "id": "41bac675",
-            "metadata": {
-                "editable": true,
-                "raw_mimetype": "text/restructuredtext",
-                "slideshow": {
-                    "slide_type": ""
-                },
-                "tags": []
-            },
+            "cell_type": "markdown",
+            "id": "987121ee",
+            "metadata": {},
             "source": [
-                "In many scenarios, it is necessary to perform integration across multiple array slices. This can be done by slicing and averaging. The following code integrates the intensity over a window of 50 meV centered at :math:`E_F`."
+                "In many scenarios, it is necessary to perform integration across multiple array slices. This can be done by slicing and averaging. The following code integrates the intensity over a window of 50 meV centered at $E_F$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b495a686",
             "metadata": {},
@@ -151,15 +137,19 @@
                 },
                 "tags": [],
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
-                "However, doing this every time is cumbersome, and we have lost the coordinate `eV`. ERLabPy provides a callable accessor :class:`qsel <erlab.accessors.utils.SelectionAccessor>` to streamline this process."
+                "However, doing this every time is cumbersome, and we have lost the coordinate `eV`. \n",
+                "\n",
+                "The ``qsel`` accessor\n",
+                "---------------------\n",
+                "ERLabPy provides a callable accessor :class:`qsel <erlab.accessors.utils.SelectionAccessor>` to streamline this process."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "00d3b00f",
             "metadata": {},
@@ -179,32 +169,58 @@
                 },
                 "tags": [],
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
-                "Note that the averaged coordinate is automatically added to the data array. This is useful for plotting and further analysis.\n",
+                "Note that the averaged coordinate is automatically added to the data array. This is\n",
+                "useful for plotting and further analysis.\n",
+                "\n",
+                "- If the width is not specified, :class:`qsel <erlab.accessors.utils.SelectionAccessor>`\n",
+                "  behaves like passing ``method='nearest'`` to :meth:`sel <xarray.DataArray.sel>`.\n",
                 "\n",
-                "If the width is not specified, :class:`qsel <erlab.accessors.utils.SelectionAccessor>` behaves like passing `method='nearest'` to `sel`. If a slice is given instead of a single value, no integration is performed. All of these methods can be combined:"
+                "- If a `slice` object is given instead of a single value, no integration is performed.\n",
+                "\n",
+                "- All of these methods can be combined:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e3bdd1ba",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dat.qsel(kx=slice(-0.3, 0.3), ky=0.3, eV=0.0, eV_width=0.05)"
             ]
         },
         {
             "cell_type": "raw",
-            "id": "761eafa9",
+            "id": "0d36f0c0",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
+            },
+            "source": [
+                "The :class:`qsel <erlab.accessors.utils.SelectionAccessor>` accessor also provides a\n",
+                "method :meth:`qsel.around <erlab.accessors.utils.SelectionAccessor.around>` to average\n",
+                "over points within a certain distance of a given point."
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "id": "41bac675",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": [],
@@ -219,16 +235,32 @@
                 "In some cases, it is necessary to mask the data. Although basic masks are supported by :mod:`xarray`, ERLabPy provides a way to mask data with arbitrary polygons.\n",
                 "\n",
                 ".. admonition:: Work in Progress\n",
                 "   :class: warning\n",
                 "\n",
                 "   This part of the user guide is still under construction. For now, see\n",
                 "   :mod:`erlab.analysis.mask`. For the full list of packages and modules provided by\n",
-                "   ERLabPy, see :doc:`../reference`.\n",
-                "\n",
+                "   ERLabPy, see :doc:`../reference`."
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "id": "761eafa9",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
+            },
+            "source": [
                 "Interpolation\n",
                 "-------------\n",
                 "\n",
                 "In addition to the `powerful interpolation methods\n",
                 "<https://docs.xarray.dev/en/latest/user-guide/interpolation.html>`_ provided by\n",
                 ":mod:`xarray`, ERLabPy provides a convenient way to interpolate data along an arbitrary\n",
                 "path.\n",
```

### Comparing `erlab-2.5.4/docs/source/user-guide/io.ipynb` & `erlab-2.6.1/docs/source/user-guide/io.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999901960784314%*

 * *Differences: {"'cells'": "{18: {'source': {insert: [(7, '        for path in erlab.io.utils.get_files(data_dir, "*

 * *            'extensions=[".h5"]):\\n\')], delete: [7]}}}'}*

```diff
@@ -825,15 +825,15 @@
                 "class ExampleLoaderComplete(ExampleLoader):\n",
                 "    name = \"example_complete\"\n",
                 "    aliases = [\"ExC\"]\n",
                 "\n",
                 "    def generate_summary(self, data_dir):\n",
                 "        # Get all valid data files in directory\n",
                 "        files = {}\n",
-                "        for path in erlab.io.utilities.get_files(data_dir, extensions=[\".h5\"]):\n",
+                "        for path in erlab.io.utils.get_files(data_dir, extensions=[\".h5\"]):\n",
                 "            # Base name\n",
                 "            data_name = os.path.splitext(os.path.basename(path))[0]\n",
                 "\n",
                 "            # If multiple scans, strip the _S### part\n",
                 "            name_match = re.match(r\"(.*?_\\d{3})_(?:_S\\d{3})?\", data_name)\n",
                 "            if name_match is not None:\n",
                 "                data_name = name_match.group(1)\n",
```

### Comparing `erlab-2.5.4/docs/source/user-guide/kconv.ipynb` & `erlab-2.6.1/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/docs/source/user-guide/plotting.ipynb` & `erlab-2.6.1/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/pyproject.toml` & `erlab-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/accessors/__init__.py` & `erlab-2.6.1/src/erlab/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/accessors/fit.py` & `erlab-2.6.1/src/erlab/accessors/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import xarray as xr
 
 from erlab.accessors.utils import (
     _THIS_ARRAY,
     ERLabDataArrayAccessor,
     ERLabDatasetAccessor,
 )
-from erlab.parallel import joblib_progress
+from erlab.utils.parallel import joblib_progress
 
 if TYPE_CHECKING:
     from xarray.core.types import Dims
 
 
 def _nested_dict_vals(d):
     for v in d.values():
@@ -386,14 +386,17 @@
                 mask = np.full_like(y, True)
 
             x = np.squeeze(x)
 
             if model.independent_vars is not None:
                 if n_coords == 1:
                     indep_var_kwargs = {model.independent_vars[0]: x}
+                    if len(model.independent_vars) == 2:
+                        # Y-dependent data, like background models
+                        indep_var_kwargs[model.independent_vars[1]] = y
                 else:
                     indep_var_kwargs = dict(
                         zip(model.independent_vars[:n_coords], x, strict=True)
                     )
             else:
                 raise ValueError("Independent variables not defined in model")
```

### Comparing `erlab-2.5.4/src/erlab/accessors/kspace.py` & `erlab-2.6.1/src/erlab/accessors/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/accessors/utils.py` & `erlab-2.6.1/src/erlab/accessors/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -445,7 +445,45 @@
 
         if verbose:
             print(
                 f"Selected data with {scalars} and {slices}, averaging over {avg_dims}"
             )
 
         return out
+
+    def around(self, radius: float | dict[Hashable, float], **sel_kw) -> xr.DataArray:
+        """
+        Average data within a specified radius of a specified point.
+
+        For instance, consider an ARPES map with dimensions ``kx``, ``ky``, and ``eV``.
+        Providing ``kx`` and ``ky`` points will average the data within a cylindrical
+        region centered at that point. The radius of the cylinder is specified by the
+        ``radius`` parameter. If different radii is given for ``kx`` and ``ky``, the
+        region will be an elliptic cylinder.
+
+        Parameters
+        ----------
+        radius
+            The radius of the region. If a single number, the same radius is used for
+            all dimensions. If a dictionary, each value
+        **sel_kw
+            The center of the spherical region. Must be a mapping of valid dimension
+            names to coordinate values.
+
+        Returns
+        -------
+        xr.DataArray
+            The mean value of the data within the region.
+
+        Note
+        ----
+        The region is defined by a spherical mask, which is generated with
+        `erlab.analysis.mask.spherical_mask`. Depending on the radius and dimensions
+        provided, the mask will be hyperellipsoid in the dimensions specified in
+        `sel_kw`.
+
+        """
+        import erlab.analysis
+
+        return self._obj.where(
+            erlab.analysis.mask.spherical_mask(self._obj, radius, **sel_kw), drop=True
+        ).mean(sel_kw.keys())
```

### Comparing `erlab-2.5.4/src/erlab/analysis/__init__.py` & `erlab-2.6.1/src/erlab/analysis/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,34 +13,23 @@
    mask
    correlation
    gold
    image
    interpolate
    kspace
    transform
-   utilities
+   utils
 
 """
 
 __all__ = [
     "correct_with_edge",
-    "mask_with_hex_bz",
-    "mask_with_polygon",
-    "polygon_mask",
-    "polygon_mask_points",
     "rotateinplane",
     "rotatestackinplane",
     "shift",
     "slice_along_path",
 ]
 
-from erlab.analysis import fit, gold, image, interpolate, mask  # noqa: F401
+from erlab.analysis import fit, gold, image, interpolate, mask, transform  # noqa: F401
 from erlab.analysis.gold import correct_with_edge
 from erlab.analysis.interpolate import slice_along_path
-from erlab.analysis.mask import (
-    mask_with_hex_bz,
-    mask_with_polygon,
-    polygon_mask,
-    polygon_mask_points,
-)
-from erlab.analysis.transform import rotateinplane, rotatestackinplane
-from erlab.analysis.utilities import shift
+from erlab.analysis.utils import shift
```

### Comparing `erlab-2.5.4/src/erlab/analysis/correlation.py` & `erlab-2.6.1/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.6.1/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.6.1/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/fit/functions/general.py` & `erlab-2.6.1/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/fit/minuit.py` & `erlab-2.6.1/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/fit/models.py` & `erlab-2.6.1/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/fit/spline.py` & `erlab-2.6.1/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/gold.py` & `erlab-2.6.1/src/erlab/analysis/gold.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
 from erlab.analysis.fit.models import (
     FermiEdge2dModel,
     FermiEdgeModel,
     PolynomialModel,
     StepEdgeModel,
 )
-from erlab.analysis.utilities import shift
-from erlab.parallel import joblib_progress
+from erlab.analysis.utils import shift
 from erlab.plotting.colors import proportional_colorbar
 from erlab.plotting.general import autoscale_to, figwh, plot_array
+from erlab.utils.parallel import joblib_progress
 
 
 def correct_with_edge(
     darr: xr.DataArray,
     modelresult: lmfit.model.ModelResult | npt.NDArray[np.floating] | Callable,
     shift_coords: bool = True,
     plot: bool = False,
@@ -64,15 +64,15 @@
         shape of the original data will be retained, and only the data will be shifted.
         Defaults to `False`.
     plot
         Whether to plot the original and corrected data arrays. Defaults to `False`.
     plot_kw
         Additional keyword arguments for the plot. Defaults to `None`.
     **shift_kwargs
-        Additional keyword arguments to `erlab.analysis.utilities.shift`.
+        Additional keyword arguments to `erlab.analysis.utils.shift`.
 
     Returns
     -------
     corrected : xarray.DataArray
         The edge corrected data.
     """
     if plot_kw is None:
```

### Comparing `erlab-2.5.4/src/erlab/analysis/image.py` & `erlab-2.6.1/src/erlab/analysis/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 import numpy as np
 import numpy.typing as npt
 import scipy
 import scipy.ndimage
 import xarray as xr
 from numba import carray, cfunc, types
 
+from erlab.utils.array import (
+    check_arg_2d_darr,
+    check_arg_uniform_dims,
+    is_uniform_spaced,
+)
+
 
 def _parse_dict_arg(
     dims: Sequence[Hashable],
     sigma: float | Collection[float] | Mapping[Hashable, float],
     arg_name: str,
     reference_name: str,
     allow_subset: bool = False,
@@ -179,14 +185,18 @@
         radius_pix: tuple[int, ...] | None = tuple(
             round(r / (darr[d].values[1] - darr[d].values[0]))
             for d, r in radius_dict.items()
         )
     else:
         radius_pix = None
 
+    for d in sigma_dict.keys():
+        if not is_uniform_spaced(darr[d].values):
+            raise ValueError(f"Dimension `{d}` is not uniformly spaced")
+
     # Calculate sigma in pixels
     sigma_pix: tuple[float, ...] = tuple(
         val / (darr[d].values[1] - darr[d].values[0]) for d, val in sigma_dict.items()
     )
 
     return darr.copy(
         data=scipy.ndimage.gaussian_filter(
@@ -612,14 +622,16 @@
     :func:`scipy.ndimage.laplace` : The underlying function used to apply the filter.
     """
     if isinstance(mode, dict):
         mode = tuple(mode[d] for d in darr.dims)
     return darr.copy(data=scipy.ndimage.laplace(darr.values, mode=mode, cval=cval))
 
 
+@check_arg_2d_darr
+@check_arg_uniform_dims
 def minimum_gradient(
     darr: xr.DataArray, mode: str = "nearest", cval: float = 0.0
 ) -> xr.DataArray:
     """Minimum gradient method for detecting dispersive features in 2D data.
 
     The minimum gradient is calculated by dividing the input DataArray by the gradient
     magnitude. See Ref. :cite:p:`he2017mingrad`.
@@ -644,33 +656,31 @@
     Raises
     ------
     ValueError
         If the input DataArray is not 2D.
 
     Note
     ----
-    - The input array is assumed to be regularly spaced.
-    - Any zero gradient values are replaced with NaN.
+    Any zero gradient values are replaced with NaN.
     """
-    if darr.ndim != 2:
-        raise ValueError("DataArray must be 2D")
-
     xvals = darr[darr.dims[1]].values
     yvals = darr[darr.dims[0]].values
 
     dx = abs(xvals[1] - xvals[0])
     dy = abs(yvals[1] - yvals[0])
 
     grad = gradient_magnitude(
         darr.values.astype(np.float64), dx, dy, mode=mode, cval=cval
     )
     grad[np.isclose(grad, 0.0)] = np.nan
     return darr / darr.max(skipna=True) / grad
 
 
+@check_arg_2d_darr
+@check_arg_uniform_dims
 def scaled_laplace(
     darr,
     factor: float = 1.0,
     mode: str | Sequence[str] | dict[str, str] = "nearest",
     cval: float = 0.0,
 ) -> xr.DataArray:
     r"""Calculate the Laplacian of a 2D DataArray with different scaling for each axis.
@@ -705,26 +715,19 @@
         The filtered array with the same shape as the input DataArray.
 
     Raises
     ------
     ValueError
         If the input DataArray is not 2D.
 
-    Note
-    ----
-    The input array is assumed to be regularly spaced.
-
     See Also
     --------
     :func:`scipy.ndimage.generic_laplace` : The underlying function used to apply the
         filter.
     """
-    if darr.ndim != 2:
-        raise ValueError("DataArray must be 2D")
-
     xvals = darr[darr.dims[1]].values
     yvals = darr[darr.dims[0]].values
 
     dx = xvals[1] - xvals[0]
     dy = yvals[1] - yvals[0]
     weight = (dx / dy) ** 2
 
@@ -743,14 +746,16 @@
         return out
 
     return darr.copy(
         data=scipy.ndimage.generic_laplace(darr.values, d2_scaled, mode=mode, cval=cval)
     )
 
 
+@check_arg_2d_darr
+@check_arg_uniform_dims
 def curvature(darr: xr.DataArray, a0: float = 1.0, factor: float = 1.0) -> xr.DataArray:
     """2D curvature method for detecting dispersive features.
 
     The curvature is calculated as defined by :cite:t:`zhang2011curvature`.
 
     Parameters
     ----------
@@ -768,22 +773,15 @@
     curvature : xarray.DataArray
         The 2D curvature of the input DataArray. Has the same shape as :code:`input`.
 
     Raises
     ------
     ValueError
         If the input DataArray is not 2D.
-
-    Note
-    ----
-    The input array is assumed to be regularly spaced.
     """
-    if darr.ndim != 2:
-        raise ValueError("DataArray must be 2D")
-
     xvals = darr[darr.dims[1]].values
     yvals = darr[darr.dims[0]].values
 
     dx = xvals[1] - xvals[0]
     dy = yvals[1] - yvals[0]
     weight = (dx / dy) ** 2
```

### Comparing `erlab-2.5.4/src/erlab/analysis/interpolate.py` & `erlab-2.6.1/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/kspace.py` & `erlab-2.6.1/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/mask/__init__.py` & `erlab-2.6.1/src/erlab/analysis/mask/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,25 +18,33 @@
 
 __all__ = [
     "hex_bz_mask_points",
     "mask_with_hex_bz",
     "mask_with_polygon",
     "polygon_mask",
     "polygon_mask_points",
+    "spherical_mask",
 ]
 
+from collections.abc import Hashable, Iterable
+
 import numba
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 
 from erlab.analysis.mask import polygon
 
 
-def mask_with_polygon(arr, vertices, dims=("kx", "ky"), invert=False):
+def mask_with_polygon(
+    arr: xr.DataArray,
+    vertices: npt.NDArray[np.floating],
+    dims: Iterable[Hashable] = ("kx", "ky"),
+    invert: bool = False,
+):
     mask = xr.DataArray(
         polygon_mask(
             vertices.astype(np.float64), *(arr[d].values for d in dims), invert=invert
         ),
         dims=dims,
         coords={d: arr.coords[d] for d in dims},
     )
@@ -148,18 +156,123 @@
         mask[i] = polygon.bounded_side_bool(vertices, (x[i], y[i]))
     if invert:
         return ~mask
     else:
         return mask
 
 
+def spherical_mask(
+    darr: xr.DataArray,
+    radius: float | dict[Hashable, float],
+    boundary: bool = True,
+    **sel_kw,
+) -> xr.DataArray:
+    """Generate a spherical boolean mask.
+
+    Depending on the radius and dimensions provided, the mask will be hyperellipsoid in
+    the dimensions specified in sel_kw. Points at the boundary are included in the mask.
+
+    The resulting mask can be used with :meth:`xarray.DataArray.where` to mask the data.
+
+    Parameters
+    ----------
+    darr
+        The input DataArray.
+    radius
+        The radius of the spherical mask. If a single number, the same radius is used
+        for all dimensions. If a dictionary, the keys should match the dimensions
+        provided in sel_kw.
+    boundary
+        Whether to consider points on the boundary to be inside the mask. Default is
+        `True`.
+    **sel_kw
+        Keyword arguments for selecting specific dimensions and values. Must be a
+        mapping of valid dimension names to coordinate values.
+
+    Returns
+    -------
+    mask : xr.DataArray
+        A boolean mask indicating whether each point in the data array is within the
+        spherical mask.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import xarray as xr
+    >>> from erlab.analysis.mask import spherical_mask
+    >>> darr = xr.DataArray(np.arange(25).reshape(5, 5), dims=("x", "y"))
+    >>> darr
+    <xarray.DataArray (x: 5, y: 5)> Size: 200B
+    array([[ 0,  1,  2,  3,  4],
+        [ 5,  6,  7,  8,  9],
+        [10, 11, 12, 13, 14],
+        [15, 16, 17, 18, 19],
+        [20, 21, 22, 23, 24]])
+    Dimensions without coordinates: x, y
+    >>> spherical_mask(darr, radius=2, x=2, y=2)
+    <xarray.DataArray (x: 5, y: 5)> Size: 25B
+    array([[False, False,  True, False, False],
+        [False,  True,  True,  True, False],
+        [ True,  True,  True,  True,  True],
+        [False,  True,  True,  True, False],
+        [False, False,  True, False, False]])
+    Dimensions without coordinates: x, y
+    >>> spherical_mask(darr, radius=1, x=2)
+    <xarray.DataArray (x: 5)> Size: 5B
+    array([False,  True,  True,  True, False])
+    Dimensions without coordinates: x
+    """
+    if isinstance(radius, dict):
+        if set(radius.keys()) != set(sel_kw.keys()):
+            raise ValueError("Keys in radius and sel_kw must match")
+
+    if len(sel_kw) == 0:
+        raise ValueError("No dimensions provided for mask")
+
+    delta_squared = xr.DataArray(0.0)
+
+    for k, v in sel_kw.items():
+        if k not in darr.dims:
+            raise ValueError(f"Dimension {k} not found in data")
+
+        if isinstance(radius, dict):
+            r = radius[k]
+        else:
+            r = float(radius)
+
+        delta_squared = delta_squared + ((darr[k] - v) / r) ** 2
+
+    if boundary:
+        return delta_squared <= 1.0
+    else:
+        return delta_squared < 1.0
+
+
 def mask_with_hex_bz(
     kxymap: xr.DataArray, a: float = 3.54, rotate: float = 0.0, invert: bool = False
 ) -> xr.DataArray:
-    """Return map masked with a hexagonal BZ."""
+    """Mask an ARPES map with a hexagonal Brillouin zone.
+
+    Parameters
+    ----------
+    kxymap
+        The input map to be masked.
+    a
+        The lattice constant of the hexagonal BZ. Default is 3.54.
+    rotate
+        The rotation angle of the BZ in degrees. Default is 0.0.
+    invert
+        Whether to invert the mask. Default is False.
+
+    Returns
+    -------
+    masked : xr.DataArray
+        The masked map.
+
+    """
     if "kx" in kxymap.dims or "qx" in kxymap.dims:
         dims = ("kx", "ky")
 
     d = 2 * np.pi / (a * 3)
     ang = rotate + np.array([0, 60, 120, 180, 240, 300])
     vertices = np.array(
         [[2 * d * np.cos(t), 2 * d * np.sin(t)] for t in np.deg2rad(ang)]
```

### Comparing `erlab-2.5.4/src/erlab/analysis/mask/polygon.py` & `erlab-2.6.1/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/transform.py` & `erlab-2.6.1/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/analysis/utilities.py` & `erlab-2.6.1/src/erlab/analysis/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     -------
 
     >>> import xarray as xr
     >>> darr = xr.DataArray(
     ...     np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]).astype(float), dims=["x", "y"]
     ... )
     >>> shift_arr = xr.DataArray([1, 0, 2], dims=["x"])
-    >>> shifted = erlab.analysis.utilities.shift(darr, shift_arr, along="y")
+    >>> shifted = erlab.analysis.utils.shift(darr, shift_arr, along="y")
     >>> print(shifted)
     <xarray.DataArray (x: 3, y: 3)> Size: 72B
     nan 1.0 2.0 4.0 5.0 6.0 nan nan 7.0
     Dimensions without coordinates: x, y
     """
     shift_kwargs.setdefault("order", 1)
     shift_kwargs.setdefault("mode", "constant")
@@ -139,13 +139,13 @@
     return out
 
 
 def correct_with_edge(*args, **kwargs):
     from erlab.analysis.gold import correct_with_edge
 
     warnings.warn(
-        "erlab.analysis.utilities.correct_with_edge is deprecated, "
+        "erlab.analysis.utils.correct_with_edge is deprecated, "
         "use erlab.analysis.gold.correct_with_edge instead",
         DeprecationWarning,
         stacklevel=1,
     )
     return correct_with_edge(*args, **kwargs)
```

### Comparing `erlab-2.5.4/src/erlab/constants.py` & `erlab-2.6.1/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/interactive/__init__.py` & `erlab-2.6.1/src/erlab/interactive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    bzplot
    colors
    curvefittingtool
    fermiedge
    kspace
    masktool
    derivative
-   utilities
+   utils
 
 """
 
 __all__ = ["dtool", "goldtool", "itool", "ktool"]
 
 
 try:
```

### Comparing `erlab-2.5.4/src/erlab/interactive/bzplot.py` & `erlab-2.6.1/src/erlab/interactive/bzplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy.typing as npt
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qtagg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.figure import Figure
 from qtpy import QtCore, QtWidgets
 
 import erlab.plotting.erplot as eplt
-from erlab.interactive.utilities import ParameterGroup
+from erlab.interactive.utils import ParameterGroup
 from erlab.lattice import abc2avec, avec2abc, to_real, to_reciprocal
 
 
 class BZPlotter(QtWidgets.QMainWindow):
     """
     Interactive Brillouin zone plotter.
```

### Comparing `erlab-2.5.4/src/erlab/interactive/colors.py` & `erlab-2.6.1/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/interactive/curvefittingtool.py` & `erlab-2.6.1/src/erlab/interactive/curvefittingtool.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import lmfit
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
 from erlab.analysis.fit.models import MultiPeakModel
-from erlab.interactive.utilities import FittingParameterWidget, ParameterGroup
+from erlab.interactive.utils import FittingParameterWidget, ParameterGroup
 
 # EDCmultiFitting Igor procedure - 2D wave EDC fit along momentum range
 
 # Momentum range to fit
 # Number of bands
 # Initial parameters
 #   const_bkg
```

### Comparing `erlab-2.5.4/src/erlab/interactive/derivative.py` & `erlab-2.6.1/src/erlab/interactive/derivative.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from erlab.analysis.image import (
     curvature,
     gaussian_filter,
     minimum_gradient,
     scaled_laplace,
 )
-from erlab.interactive.utilities import (
+from erlab.interactive.utils import (
     copy_to_clipboard,
     gen_function_code,
     parse_data,
     xImageItem,
 )
 
 if TYPE_CHECKING:
```

### Comparing `erlab-2.5.4/src/erlab/interactive/dtool.ui` & `erlab-2.6.1/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/interactive/fermiedge.py` & `erlab-2.6.1/src/erlab/interactive/fermiedge.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 import pyqtgraph as pg
 import varname
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
 import erlab.analysis
 from erlab.interactive.imagetool import ImageTool
-from erlab.interactive.utilities import (
+from erlab.interactive.utils import (
     AnalysisWindow,
     ParameterGroup,
     ROIControls,
     gen_function_code,
     xImageItem,
 )
-from erlab.parallel import joblib_progress_qt
+from erlab.utils.parallel import joblib_progress_qt
 
 if TYPE_CHECKING:
     import lmfit
     import scipy.interpolate
 
 LMFIT_METHODS = [
     "leastsq",
@@ -104,15 +104,15 @@
         The data to correct with the edge. Defaults to `data`.
     data_name
         Name of the data used in generating the code snipped copied to the clipboard.
         Overrides automatic detection.
     execute
         Whether to execute the tool immediately.
     **kwargs
-        Arguments passed onto `erlab.interactive.utilities.AnalysisWindow`.
+        Arguments passed onto `erlab.interactive.utils.AnalysisWindow`.
 
     Signals
     -------
     sigProgressUpdated(int)
         Signal used to update the progress bar.
     sigAbortFitting()
         Signal used to abort the fitting, emitted when the cancel button is clicked.
@@ -562,15 +562,15 @@
         The data to perform Fermi edge fitting on.
     data_corr
         The data to correct with the edge. Defaults to `data`.
     data_name
         Name of the data used in generating the code snipped copied to the clipboard.
         Overrides automatic detection.
     **kwargs
-        Arguments passed onto `erlab.interactive.utilities.AnalysisWindow`.
+        Arguments passed onto `erlab.interactive.utils.AnalysisWindow`.
     """
     if data_name is None:
         try:
             data_name = varname.argname("data", func=goldtool, vars_only=False)
         except varname.VarnameRetrievingError:
             data_name = "data"
     return GoldTool(data, data_corr, data_name=data_name, **kwargs)
```

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import erlab.io
 from erlab.interactive.imagetool.controls import (
     ItoolBinningControls,
     ItoolColormapControls,
     ItoolCrosshairControls,
 )
 from erlab.interactive.imagetool.core import ImageSlicerArea, SlicerLinkProxy
-from erlab.interactive.utilities import DictMenuBar, copy_to_clipboard
+from erlab.interactive.utils import DictMenuBar, copy_to_clipboard
 from erlab.io.plugins.merlin import MERLINLoader
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Collection
 
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
@@ -139,16 +139,18 @@
 
     if execute:
         qapp.exec()
         del itool_list
         gc.collect()
 
         return None
+
     if len(itool_list) == 1:
         return itool_list[0]
+
     return itool_list
 
 
 class BaseImageTool(QtWidgets.QMainWindow):
     def __init__(self, data=None, parent=None, **kwargs):
         super().__init__(parent=parent)
         self.slicer_area = ImageSlicerArea(self, data, **kwargs)
```

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from qtpy import QtCore, QtGui, QtSvg, QtSvgWidgets, QtWidgets
 
 from erlab.interactive.colors import (
     pg_colormap_names,
     pg_colormap_powernorm,
     pg_colormap_to_QPixmap,
 )
-from erlab.interactive.utilities import parse_data, xImageItem
+from erlab.interactive.utils import parse_data, xImageItem
 
 # pg.setConfigOption('useNumba', True)
 # pg.setConfigOption('background', 'w')
 # pg.setConfigOption('foreground', 'k')
 
 if importlib.util.find_spec("numbagg"):
     import numbagg
```

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/controls.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import pyqtgraph as pg
 import qtawesome as qta
 from qtpy import QtCore, QtGui, QtWidgets
 
 from erlab.interactive.colors import ColorMapComboBox, ColorMapGammaWidget
-from erlab.interactive.utilities import BetterSpinBox
+from erlab.interactive.utils import BetterSpinBox
 
 if TYPE_CHECKING:
     from collections.abc import Mapping
 
     import xarray as xr
 
     from erlab.interactive.imagetool.core import ImageSlicerArea
@@ -672,23 +672,34 @@
 
 
 class ItoolBinningControls(ItoolControlsBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def initialize_layout(self):
-        self.setLayout(QtWidgets.QGridLayout(self))
-
-        layout = cast(QtWidgets.QGridLayout, self.layout())
+        layout = QtWidgets.QHBoxLayout(self)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(3)
 
+        self.gridlayout = QtWidgets.QGridLayout()
+        self.gridlayout.setContentsMargins(0, 0, 0, 0)
+        self.gridlayout.setSpacing(3)
+
+        self.buttonslayout = QtWidgets.QVBoxLayout()
+        self.buttonslayout.setContentsMargins(0, 0, 0, 0)
+        self.buttonslayout.setSpacing(3)
+
+        layout.addLayout(self.gridlayout)
+        layout.addLayout(self.buttonslayout)
+        self.setLayout(layout)
+
     def initialize_widgets(self):
         super().initialize_widgets()
         self.labels = tuple(QtWidgets.QLabel() for _ in range(self.data.ndim))
+        self.val_labels = tuple(QtWidgets.QLabel() for _ in range(self.data.ndim))
         self.spins = tuple(
             BetterSpinBox(
                 self,
                 integer=True,
                 singleStep=2,
                 # minimumWidth=60,
                 value=1,
@@ -703,23 +714,35 @@
 
         self.reset_btn = IconButton("reset", toolTip="Reset bins")
         self.reset_btn.clicked.connect(self.reset)
 
         self.all_btn = IconButton(
             on="all_cursors",
             checkable=True,
-            toolTip="Apply for all cursors",
+            toolTip="When checked, apply bins to all cursors upon change",
         )
 
-        layout = cast(QtWidgets.QGridLayout, self.layout())
+        height = QtGui.QFontMetrics(self.labels[0].font()).height() + 3
+
         for i in range(self.data.ndim):
-            layout.addWidget(self.labels[i], 0, i, 1, 1)
-            layout.addWidget(self.spins[i], 1, i, 1, 1)
-        layout.addWidget(self.reset_btn, 2, 0, 1, 1)
-        layout.addWidget(self.all_btn, 2, 1, 1, 1)
+            self.gridlayout.addWidget(self.labels[i], 0, i, 1, 1)
+            self.gridlayout.addWidget(self.spins[i], 1, i, 1, 1)
+            self.gridlayout.addWidget(self.val_labels[i], 2, i, 1, 1)
+            self.val_labels[i].setMaximumHeight(height)
+            self.spins[i].setToolTip("Number of bins")
+            self.val_labels[i].setToolTip("Value corresponding to number of bins")
+
+        self.reset_btn.setSizePolicy(
+            QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding
+        )
+        self.all_btn.setSizePolicy(
+            QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding
+        )
+        self.buttonslayout.addWidget(self.reset_btn)
+        self.buttonslayout.addWidget(self.all_btn)
         # for spin in self.spins:
         # spin.setMinimumWidth(60)
 
     def _update_bin(self, axis, n):
         if self.all_btn.isChecked():
             self.slicer_area.set_bin_all(axis, n)
         else:
@@ -738,21 +761,25 @@
         self.slicer_area.sigBinChanged.disconnect(self.update)
         self.slicer_area.sigDataChanged.disconnect(self.update)
         self.slicer_area.sigShapeChanged.disconnect(self.update)
 
     def update(self):
         super().update()
 
-        if len(self.labels) != self.data.ndim:
+        if len(self.val_labels) != self.data.ndim:
             clear_layout(self.layout())
             self.initialize_widgets()
 
+        bin_numbers = self.array_slicer.get_bins(self.current_cursor)
+        bin_values = self.array_slicer.get_bin_values(self.current_cursor)
+
         for i in range(self.data.ndim):
             self.spins[i].blockSignals(True)
-            self.labels[i].setText(str(self.data.dims[i]))
+            self.labels[i].setText(f"{self.data.dims[i]!s}")
             self.spins[i].setRange(1, self.data.shape[i] - 1)
-            self.spins[i].setValue(self.array_slicer.get_bins(self.current_cursor)[i])
+            self.spins[i].setValue(bin_numbers[i])
+            self.val_labels[i].setText(f"{bin_values[i]:.3g}")
             self.spins[i].blockSignals(False)
 
     def reset(self):
         for spin in self.spins:
             spin.setValue(1)
```

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/core.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from erlab.interactive.colors import (
     BetterColorBarItem,
     BetterImageItem,
     pg_colormap_powernorm,
 )
 from erlab.interactive.imagetool.slicer import ArraySlicer
-from erlab.interactive.utilities import BetterAxisItem, copy_to_clipboard
+from erlab.interactive.utils import BetterAxisItem, copy_to_clipboard
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Iterable, Sequence
 
     from pyqtgraph.graphicsItems.ViewBox import ViewBoxMenu
     from pyqtgraph.GraphicsScene import mouseEvents
 
@@ -170,39 +170,43 @@
 
 
 class SlicerLinkProxy:
     """Internal class for handling linked `ImageSlicerArea` s.
 
     Parameters
     ----------
-    link_colors
-        Whether to sync color related changes.
     *slicers
         The slicers to link.
+    link_colors
+        Whether to sync color related changes, by default `True`.
 
     """
 
     def __init__(self, *slicers: ImageSlicerArea, link_colors: bool = True):
         self.link_colors = link_colors
-        self._slicers: set[ImageSlicerArea] = set()
+        self._children: set[ImageSlicerArea] = set()
         for s in slicers:
             self.add(s)
 
-    def add(self, slicer: ImageSlicerArea):
-        if slicer.is_linked:
-            if slicer._linking_proxy == self:
+    @property
+    def children(self) -> set[ImageSlicerArea]:
+        return self._children
+
+    def add(self, slicer_area: ImageSlicerArea):
+        if slicer_area.is_linked:
+            if slicer_area._linking_proxy == self:
                 return
             else:
                 raise ValueError("Already linked to another proxy.")
-        self._slicers.add(slicer)
-        slicer._linking_proxy = self
+        self._children.add(slicer_area)
+        slicer_area._linking_proxy = self
 
-    def remove(self, slicer: ImageSlicerArea):
-        self._slicers.remove(slicer)
-        slicer._linking_proxy = None
+    def remove(self, slicer_area: ImageSlicerArea):
+        self._children.remove(slicer_area)
+        slicer_area._linking_proxy = None
 
     def sync(
         self,
         source: ImageSlicerArea,
         funcname: str,
         arguments: dict[str, Any],
         indices: bool,
@@ -224,15 +228,15 @@
             Arguments included in the function call.
         indices, steps, color
             Arguments given to the decorator. See :func:`link_slicer`
 
         """
         if color and not self.link_colors:
             return
-        for target in self._slicers.difference({source}):
+        for target in self._children.difference({source}):
             getattr(target, funcname)(
                 **self.convert_args(source, target, arguments, indices, steps)
             )
 
     def convert_args(
         self,
         source: ImageSlicerArea,
@@ -646,15 +650,15 @@
             del self._data
             self.disconnect_axes_signals()
         else:
             n_cursors_old = 1
 
         if not isinstance(data, xr.DataArray):
             if isinstance(data, xr.Dataset):
-                data = data[next(iter(data.data_vars.keys()))]
+                data = cast(xr.DataArray, data[next(iter(data.data_vars.keys()))])
             else:
                 data = xr.DataArray(np.asarray(data))
         if hasattr(data.data, "flags"):
             if not data.data.flags["WRITEABLE"]:
                 data = data.copy()
 
         if not rad2deg:
```

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.6.1/src/erlab/interactive/imagetool/slicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numba
 import numpy as np
 import numpy.typing as npt
 from qtpy import QtCore
 
 from erlab.interactive.imagetool.fastbinning import fast_nanmean_skipcheck
-from erlab.interactive.utilities import format_kwargs
+from erlab.interactive.utils import format_kwargs
 
 if TYPE_CHECKING:
     from collections.abc import Hashable, Sequence
 
     import xarray as xr
 
 VALID_NDIM = (2, 3, 4)
@@ -393,14 +393,27 @@
             update=update,
         )
 
     @QtCore.Slot(int, result=list)
     def get_bins(self, cursor: int) -> list[int]:
         return self._bins[cursor]
 
+    @QtCore.Slot(int, result=list)
+    def get_bin_values(self, cursor: int) -> list[float | None]:
+        bins = self.get_bins(cursor)
+        if self._nonuniform_axes:
+            return [
+                None if i in self._nonuniform_axes else b * np.abs(inc)
+                for i, (b, inc) in enumerate(zip(bins, self.incs_uniform, strict=True))
+            ]
+        else:
+            return [
+                b * np.abs(inc) for b, inc in zip(bins, self.incs_uniform, strict=True)
+            ]
+
     def set_bins(
         self, cursor: int, value: list[int | None], update: bool = True
     ) -> None:
         if not len(value) == self._obj.ndim:
             raise ValueError("length of bin array must match the number of dimensions.")
         axes: list[int | None] = []
         for i, x in enumerate(value):
```

### Comparing `erlab-2.5.4/src/erlab/interactive/kspace.py` & `erlab-2.6.1/src/erlab/interactive/kspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import erlab.analysis
 from erlab.interactive.colors import (
     BetterColorBarItem,  # noqa: F401
     ColorMapComboBox,  # noqa: F401
     ColorMapGammaWidget,  # noqa: F401
 )
 from erlab.interactive.imagetool import ImageTool
-from erlab.interactive.utilities import copy_to_clipboard, gen_function_code, xImageItem
+from erlab.interactive.utils import copy_to_clipboard, gen_function_code, xImageItem
 from erlab.plotting.bz import get_bz_edge
 
 
 class KspaceToolGUI(
     *uic.loadUiType(os.path.join(os.path.dirname(__file__), "ktool.ui"))  # type: ignore[misc]
 ):
     def __init__(self):
```

### Comparing `erlab-2.5.4/src/erlab/interactive/ktool.ui` & `erlab-2.6.1/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/interactive/masktool.py` & `erlab-2.6.1/src/erlab/interactive/masktool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pyqtgraph as pg
 from pyqtgraph.Qt import QtCore
 
-from erlab.interactive.utilities import AnalysisWindow, ParameterGroup
+from erlab.interactive.utils import AnalysisWindow, ParameterGroup
 
 __all__ = ["masktool"]
 
 
 class PolyLineROIControls(ParameterGroup):
     def __init__(self, roi: pg.PolyLineROI, spinbox_kw=None, **kwargs):
         pass
```

### Comparing `erlab-2.5.4/src/erlab/interactive/utilities.py` & `erlab-2.6.1/src/erlab/interactive/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,28 +246,30 @@
         integer: bool = False,
         compact: bool = True,
         discrete: bool = False,
         decimals: int = 3,
         significant: bool = False,
         scientific: bool = False,
         value: float = 0.0,
+        prefix: str = "",
         **kwargs,
     ):
         self._only_int = integer
         self._is_compact = compact
         self._is_discrete = discrete
         self._is_scientific = scientific
         self._decimal_significant = significant
         self.setDecimals(decimals)
 
         self._value = value
         self._lastvalue: float | None = None
         self._min = -np.inf
         self._max = np.inf
         self._step = 1 if self._only_int else 0.01
+        self._prefix = prefix
 
         kwargs.setdefault("correctionMode", self.CorrectionMode.CorrectToPreviousValue)
         kwargs.setdefault("keyboardTracking", False)
 
         # PyQt6 compatibility: set options with keyword arguments
         set_dict = {}
         for k in ["singleStep", "minimum", "maximum"]:
@@ -288,25 +290,34 @@
         if self.isReadOnly():
             line_edit = self.lineEdit()
             if line_edit is not None:
                 line_edit.setReadOnly(True)
             self.setButtonSymbols(self.ButtonSymbols.NoButtons)
         self.setValue(self.value())
 
-    def setDecimals(self, decimals):
+    @QtCore.Slot(str)
+    def setPrefix(self, prefix: str):
+        self._prefix = prefix
+
+    def prefix(self) -> str:
+        return self._prefix
+
+    @QtCore.Slot(int)
+    def setDecimals(self, decimals: int):
         self._decimals = decimals
 
-    def decimals(self):
+    def decimals(self) -> int:
         return self._decimals
 
     def setRange(self, mn, mx):
         self.setMinimum(min(mn, mx))
         self.setMaximum(max(mn, mx))
 
-    def widthFromText(self, text):
+    @QtCore.Slot(str, result=int)
+    def widthFromText(self, text: str) -> int:
         return QtGui.QFontMetrics(self.font()).boundingRect(text).width()
 
     def widthFromValue(self, value):
         return self.widthFromText(self.textFromValue(value))
 
     def setMaximum(self, mx):
         if self._only_int and np.isfinite(mx):
@@ -340,39 +351,40 @@
 
     def value(self):
         if self._only_int:
             return int(self._value)
         else:
             return self._value
 
-    def text(self):
+    def text(self) -> str:
         return self.textFromValue(self.value())
 
-    def textFromValue(self, value):
+    def textFromValue(self, value) -> str:
         if (not self._only_int) or (not np.isfinite(value)):
             if self._is_scientific:
-                return np.format_float_scientific(
+                return self.prefix() + np.format_float_scientific(
                     value,
                     precision=self.decimals(),
                     unique=False,
                     trim="k",
                     exp_digits=1,
                 )
             else:
-                return np.format_float_positional(
+                return self.prefix() + np.format_float_positional(
                     value,
                     precision=self.decimals(),
                     unique=False,
                     fractional=not self._decimal_significant,
                     trim="k",
                 )
         else:
-            return str(int(value))
+            return self.prefix() + str(int(value))
 
-    def valueFromText(self, text):
+    def valueFromText(self, text: str):
+        text = text[len(self.prefix()) :]
         if text == "":
             return np.nan
         if self._only_int:
             return int(text)
         else:
             return float(text)
 
@@ -485,15 +497,15 @@
             - QtGui.QFontMetrics(spin.font())
             .boundingRect(spin.textFromValue(0.0))
             .width()
         )
         spin.setDisabled(True)
         spin.setVisible(False)
         del spin
-        return w + 10
+        return w
 
     def _updateWidth(self):
         self.setMinimumWidth(
             max(
                 self.widthFromValue(self.maximum()), self.widthFromValue(self.minimum())
             )
             + self._get_offset()
```

### Comparing `erlab-2.5.4/src/erlab/io/__init__.py` & `erlab-2.6.1/src/erlab/io/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 =======
 
 .. autosummary::
    :toctree: generated
 
    plugins
    dataloader
-   utilities
+   utils
    igor
    exampledata
    characterization
 
 
 For a single session, it is very common to use only one type of loader for a single
 folder with all your data. Hence, the module provides a way to set a default loader for
@@ -57,15 +57,15 @@
     "summarize",
 ]
 
 import warnings
 
 from erlab.io.dataloader import LoaderRegistry
 from erlab.io.igor import load_experiment, load_wave
-from erlab.io.utilities import load_hdf5, open_hdf5, save_as_hdf5, save_as_netcdf
+from erlab.io.utils import load_hdf5, open_hdf5, save_as_hdf5, save_as_netcdf
 
 # Import plugins last
 # isort: off
 import erlab.io.plugins  # noqa: F401
 
 loaders = LoaderRegistry.instance()
 """
```

### Comparing `erlab-2.5.4/src/erlab/io/characterization/resistance.py` & `erlab-2.6.1/src/erlab/io/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/io/characterization/xrd.py` & `erlab-2.6.1/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/io/dataloader.py` & `erlab-2.6.1/src/erlab/io/dataloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,34 +23,25 @@
 import itertools
 import os
 import warnings
 from typing import TYPE_CHECKING, Any, ClassVar, Self, cast
 
 import joblib
 import numpy as np
-import numpy.typing as npt
 import pandas
 import xarray as xr
 
+from erlab.utils.array import is_monotonic, is_uniform_spaced
+
 if TYPE_CHECKING:
-    from collections.abc import Iterable, Mapping
+    from collections.abc import Iterable, Mapping, Sequence
 
     DataFromSingleFile = xr.DataArray | xr.Dataset | list[xr.DataArray]
 
 
-def _is_uniform(arr: npt.NDArray) -> bool:
-    dif = np.diff(arr)
-    return np.allclose(dif, dif[0], rtol=3e-05, atol=3e-05, equal_nan=True)
-
-
-def _is_monotonic(arr: npt.NDArray) -> np.bool_:
-    dif = np.diff(arr)
-    return np.all(dif >= 0) or np.all(dif <= 0)
-
-
 class ValidationError(Exception):
     """Raised when the loaded data fails validation checks."""
 
 
 class ValidationWarning(UserWarning):
     """Issued when the loaded data fails validation checks."""
 
@@ -81,21 +72,38 @@
     attribute, the value can be passed as an iterable.
     """
 
     coordinate_attrs: tuple[str, ...] = ()
     """
     Names of attributes (after renaming) that should be treated as coordinates.
 
+    Attributes mentioned here will be moved from attrs to coordinates. This means that
+    it will be propagated when concatenating data from multiple files. If a listed
+    attribute is not found, it will be silently skipped.
+
     Note
     ----
     Although the data loader tries to preserve the original attributes, the attributes
     given here, both before and after renaming, will be removed from attrs for
     consistency.
     """
 
+    average_attrs: tuple[str, ...] = ()
+    """
+    Names of attributes or coordinates (after renaming) that should be averaged over.
+
+    This is useful for attributes that may slightly vary between scans. If a listed
+    attribute is not found, it will be silently skipped.
+
+    Note
+    ----
+    The attributes are just converted to coordinates upon loading and are averaged in
+    the post-processing step.
+    """
+
     additional_attrs: ClassVar[dict[str, str | int | float]] = {}
     """Additional attributes to be added to the data after loading."""
 
     additional_coords: ClassVar[dict[str, str | int | float]] = {}
     """Additional non-dimension coordinates to be added to the data after loading."""
 
     always_single: bool = True
@@ -118,14 +126,19 @@
         """A reversed version of the name_map dictionary.
 
         This property is useful for mapping original names to new names.
 
         """
         return self.reverse_mapping(self.name_map)
 
+    @property
+    def coordinate_and_average_attrs(self) -> tuple[str, ...]:
+        """Return a tuple of coordinate and average attributes."""
+        return self.coordinate_attrs + self.average_attrs
+
     @staticmethod
     def reverse_mapping(mapping: Mapping[str, str | Iterable[str]]) -> dict[str, str]:
         """Reverse the given mapping dictionary to form a one-to-one mapping.
 
         Parameters
         ----------
         mapping
@@ -252,21 +265,21 @@
         if isinstance(val, np.ndarray):
             if val.size == 1:
                 return cls.formatter(val.item())
 
             elif val.squeeze().ndim == 1:
                 val = val.squeeze()
 
-                if _is_uniform(val):
+                if is_uniform_spaced(val):
                     start, end, step = tuple(
                         cls.formatter(v) for v in (val[0], val[-1], val[1] - val[0])
                     )
                     return f"{start}→{end} ({step}, {len(val)})".replace("-", "−")
 
-                elif _is_monotonic(val):
+                elif is_monotonic(val):
                     if val[0] == val[-1]:
                         return cls.formatter(val[0])
 
                     return (
                         f"{cls.formatter(val[0])}→{cls.formatter(val[-1])} ({len(val)})"
                     )
 
@@ -845,25 +858,56 @@
         -------
         pandas.DataFrame
             Summary of the data in the directory.
 
         """
         raise NotImplementedError("This loader does not support folder summaries")
 
+    def combine_attrs(
+        self,
+        variable_attrs: Sequence[dict[str, Any]],
+        context: xr.Context | None = None,
+    ) -> dict[str, Any]:
+        """Combine multiple attributes into a single attribute.
+
+        This method is used as the ``combine_attrs`` argument in :func:`xarray.concat`
+        and :func:`xarray.merge` when combining data from multiple files into a single
+        object. By default, it has the same behavior as specifying
+        `combine_attrs='override'` by taking the first set of attributes.
+
+        The method can be overridden to provide fine-grained control over how the
+        attributes are combined.
+
+        Parameters
+        ----------
+        variable_attrs
+            A sequence of attributes to be combined.
+        context
+            The context in which the attributes are being combined. This has no effect,
+            but is required by xarray.
+
+        Returns
+        -------
+        dict[str, Any]
+            The combined attributes.
+
+        """
+        return dict(variable_attrs[0])
+
     def combine_multiple(
         self,
         data_list: list[xr.DataArray | xr.Dataset | list[xr.DataArray]],
         coord_dict: dict[str, Iterable],
     ) -> (
         xr.DataArray | xr.Dataset | list[xr.DataArray | xr.Dataset | list[xr.DataArray]]
     ):
         if len(coord_dict) == 0:
             try:
                 # Try to merge the data without conflicts
-                return xr.merge(data_list)
+                return xr.merge(data_list, combine_attrs=self.combine_attrs)
             except:  # noqa: E722
                 # On failure, return a list
                 return data_list
         else:
             for i in range(len(data_list)):
                 if isinstance(data_list[i], list):
                     data_list[i] = self.combine_multiple(data_list[i], coord_dict={})
@@ -873,14 +917,15 @@
                         {k: v[i] for k, v in coord_dict.items()}
                     )
             try:
                 return xr.concat(
                     data_list,
                     dim=next(iter(coord_dict.keys())),
                     coords="different",
+                    combine_attrs=self.combine_attrs,
                 )
             except:  # noqa: E722
                 return data_list
 
     def process_keys(
         self, data: xr.DataArray, key_mapping: dict[str, str] | None = None
     ) -> xr.DataArray:
@@ -891,33 +936,42 @@
         data = data.rename({k: v for k, v in key_mapping.items() if k in data.coords})
 
         # For attributes, keep original attribute and add new with renamed keys
         new_attrs = {}
         for k, v in dict(data.attrs).items():
             if k in key_mapping:
                 new_key = key_mapping[k]
-                if new_key in self.coordinate_attrs and new_key in data.coords:
+                if (
+                    new_key in self.coordinate_and_average_attrs
+                    and new_key in data.coords
+                ):
                     # Renamed attribute is already a coordinate, remove
                     del data.attrs[k]
                 else:
                     new_attrs[new_key] = v
         data = data.assign_attrs(new_attrs)
 
         # Move from attrs to coordinate if coordinate is not found
         data = data.assign_coords(
             {
                 a: data.attrs.pop(a)
-                for a in self.coordinate_attrs
+                for a in self.coordinate_and_average_attrs
                 if a in data.attrs and a not in data.coords
             }
         )
         return data
 
     def post_process(self, data: xr.DataArray) -> xr.DataArray:
         data = self.process_keys(data)
+
+        for k in self.average_attrs:
+            if k in data.coords:
+                v = data[k].values.mean()
+                data = data.drop(k).assign_attrs({k: v})
+
         data = data.assign_attrs(
             self.additional_attrs | {"data_loader_name": str(self.name)}
         )
         data = data.assign_coords(self.additional_coords)
         return data
 
     def post_process_general(
@@ -968,15 +1022,15 @@
 
         for c in ("alpha", "beta", "delta", "xi", "hv"):
             if c not in data.coords:
                 cls._raise_or_warn(f"Missing coordinate {c}")
 
         for a in ("configuration", "temp_sample"):
             if a not in data.attrs:
-                cls._raise_or_warn(f"Missing attribute {c}")
+                cls._raise_or_warn(f"Missing attribute {a}")
 
         if data.attrs["configuration"] not in (1, 2):
             if data.attrs["configuration"] not in (3, 4):
                 cls._raise_or_warn(
                     f"Invalid configuration {data.attrs['configuration']}"
                 )
             elif "chi" not in data.coords:
```

### Comparing `erlab-2.5.4/src/erlab/io/exampledata.py` & `erlab-2.6.1/src/erlab/io/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/io/igor.py` & `erlab-2.6.1/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/io/plugins/__init__.py` & `erlab-2.6.1/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/io/plugins/da30.py` & `erlab-2.6.1/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/io/plugins/kriss.py` & `erlab-2.6.1/src/erlab/io/plugins/kriss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Plugin for data acquired at KRISS."""
 
 import os
 import re
 from collections.abc import Iterable
 from typing import ClassVar
 
-import erlab.io.utilities
+import erlab.io.utils
 from erlab.io.plugins.da30 import DA30Loader
 
 
 class KRISSLoader(DA30Loader):
     name = "kriss"
 
     aliases = ("KRISS",)
@@ -21,15 +21,15 @@
     @property
     def name_map(self):
         return super().name_map | {"chi": "ThetaY", "xi": "ThetaX"}
 
     def identify(
         self, num: int, data_dir: str | os.PathLike
     ) -> tuple[list[str], dict[str, Iterable]]:
-        for file in erlab.io.utilities.get_files(data_dir, extensions=(".ibw", ".zip")):
+        for file in erlab.io.utils.get_files(data_dir, extensions=(".ibw", ".zip")):
             if file.endswith(".zip"):
                 match = re.match(r"(.*?)" + str(num).zfill(4) + r".zip", file)
             else:
                 match = re.match(
                     r"(.*?)" + str(num).zfill(4) + str(num).zfill(3) + r".ibw", file
                 )
```

### Comparing `erlab-2.5.4/src/erlab/io/plugins/maestro.py` & `erlab-2.6.1/src/erlab/io/plugins/maestro.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     additional_attrs: ClassVar[dict] = {}
 
     skip_validate: bool = True
     always_single: bool = True
 
     def identify(self, num, data_dir):
         file = None
-        for f in erlab.io.utilities.get_files(data_dir, ".h5"):
+        for f in erlab.io.utils.get_files(data_dir, ".h5"):
             if re.match(rf"(\d+)_{str(num).zfill(5)}.h5", os.path.basename(f)):
                 file = f
 
         if file is None:
             raise ValueError(f"No file found in {data_dir} for {num}")
 
         return [file], {}
@@ -185,15 +185,15 @@
                 data.shape,
                 reversed(data.attrs["unitNames"]),
                 strict=False,
             )
         }
 
         data = data.rename(
-            {f"phony_dim_{i+1}": k for i, k in enumerate(coord_dict.keys())}
+            {f"phony_dim_{i + 1}": k for i, k in enumerate(coord_dict.keys())}
         ).assign_coords(coord_dict)
 
         if len(motors) == 1:
             data = data.rename(phony_dim_3=motors[0]).assign_coords(coords)
         else:
             # Stack and unstack to get the correct n-dimensional data
             data = (
```

### Comparing `erlab-2.5.4/src/erlab/io/plugins/merlin.py` & `erlab-2.6.1/src/erlab/io/plugins/merlin.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, ClassVar
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import xarray as xr
 
-import erlab.io.utilities
+import erlab.io.utils
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
 
 
 class MERLINLoader(LoaderBase):
     name = "merlin"
 
@@ -40,14 +40,15 @@
         "xi",
         "hv",
         "x",
         "y",
         "z",
         "polarization",
         "mesh_current",
+        "temp_sample",
     )
     additional_attrs: ClassVar[dict] = {
         "configuration": 1,
         "sample_workfunction": 4.44,
     }
     always_single = False
 
@@ -124,14 +125,19 @@
 
     def post_process(self, data: xr.DataArray) -> xr.DataArray:
         data = super().post_process(data)
 
         if "eV" in data.coords:
             data = data.assign_coords(eV=-data.eV.values)
 
+        if "temp_sample" in data.coords:
+            # Add temperature to attributes
+            temp = float(data.temp_sample.mean())
+            data = data.assign_attrs(temp_sample=temp)
+
         return data
 
     def load_live(self, filename, data_dir=None):
         wave = load_wave(filename, data_dir)
         wave = wave.rename(
             {
                 k: v
@@ -144,15 +150,15 @@
         return self.post_process(wave)
 
     def generate_summary(
         self, data_dir: str | os.PathLike, exclude_live: bool = False
     ) -> pd.DataFrame:
         files: dict[str, str] = {}
 
-        for path in erlab.io.utilities.get_files(data_dir, extensions=(".pxt",)):
+        for path in erlab.io.utils.get_files(data_dir, extensions=(".pxt",)):
             data_name = os.path.splitext(os.path.basename(path))[0]
             name_match = re.match(r"(.*?_\d{3})_(?:_S\d{3})?", data_name)
             if name_match is not None:
                 data_name = name_match.group(1)
             files[data_name] = path
 
         if not exclude_live:
```

### Comparing `erlab-2.5.4/src/erlab/io/plugins/ssrl52.py` & `erlab-2.6.1/src/erlab/io/plugins/ssrl52.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import ClassVar
 
 import h5netcdf
 import numpy as np
 import pandas as pd
 import xarray as xr
 
-import erlab.io.utilities
+import erlab.io.utils
 from erlab.io.dataloader import LoaderBase
 
 
 class SSRL52Loader(LoaderBase):
     name = "ssrl"
     aliases = ("ssrl52", "bl5-2")
 
@@ -114,19 +114,19 @@
     def identify(
         self,
         num: int,
         data_dir: str | os.PathLike,
         zap: bool = False,
     ):
         if zap:
-            target_files = erlab.io.utilities.get_files(
+            target_files = erlab.io.utils.get_files(
                 data_dir, extensions=(".h5",), contains="zap"
             )
         else:
-            target_files = erlab.io.utilities.get_files(
+            target_files = erlab.io.utils.get_files(
                 data_dir, extensions=(".h5",), notcontains="zap"
             )
 
         for file in target_files:
             match = re.match(r"(.*?)_" + str(num).zfill(4) + r".h5", file)
             if match is not None:
                 return [file], {}
@@ -148,19 +148,19 @@
 
     def generate_summary(
         self, data_dir: str | os.PathLike, exclude_zap: bool = False
     ) -> pd.DataFrame:
         files: dict[str, str] = {}
 
         if exclude_zap:
-            target_files = erlab.io.utilities.get_files(
+            target_files = erlab.io.utils.get_files(
                 data_dir, extensions=(".h5",), notcontains="zap"
             )
         else:
-            target_files = erlab.io.utilities.get_files(data_dir, extensions=(".h5",))
+            target_files = erlab.io.utils.get_files(data_dir, extensions=(".h5",))
 
         for pth in target_files:
             base_name = os.path.splitext(os.path.basename(pth))[0]
             files[base_name] = pth
 
         summary_attrs: dict[str, str] = {
             "Type": "Description",
```

### Comparing `erlab-2.5.4/src/erlab/io/utilities.py` & `erlab-2.6.1/src/erlab/io/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/lattice.py` & `erlab-2.6.1/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/parallel.py` & `erlab-2.6.1/src/erlab/utils/parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""
-Helper functions for parallel processing.
-
-.. currentmodule:: erlab.parallel
-
-"""
+"""Helper functions for parallel processing."""
 
 __all__ = ["joblib_progress", "joblib_progress_qt"]
 
 import contextlib
 import sys
 
 import joblib
```

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.6.1/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.6.1/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/__init__.py` & `erlab-2.6.1/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/annotations.py` & `erlab-2.6.1/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/atoms.py` & `erlab-2.6.1/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/bz.py` & `erlab-2.6.1/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/colors.py` & `erlab-2.6.1/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/erplot.py` & `erlab-2.6.1/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/general.py` & `erlab-2.6.1/src/erlab/plotting/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -689,31 +689,36 @@
 
     x = np.asarray(x)
     xn = np.r_[x[0], x, x[-1]]
     yn = np.r_[y0, y, y0]
     patch = matplotlib.patches.PathPatch(
         matplotlib.path.Path(np.array([xn, yn]).T), edgecolor="none", facecolor="none"
     )
-    ax.add_patch(patch)
 
     im = matplotlib.image.AxesImage(
-        ax, cmap=cmap, interpolation="bicubic", origin="lower", zorder=0, **kwargs
+        ax,
+        cmap=cmap,
+        interpolation="bicubic",
+        origin="lower",
+        zorder=0,
+        extent=(min(xn), max(xn), min(yn), max(yn)),
+        **kwargs,
     )
     im.use_sticky_edges = False  # type: ignore[attr-defined]
 
     if transpose:
         im.set_data(np.linspace(0, 1, 1024).reshape(1024, 1).T)
     else:
         im.set_data(np.linspace(0, 1, 1024).reshape(1024, 1))
 
-    # with autoscale_off(ax):
-    im.set_extent((min(xn), max(xn), min(yn), max(yn)))
-    im.set_clip_path(patch)
-    im.autoscale_None()
-    ax.add_image(im)
+    with autoscale_off(ax):
+        ax.add_patch(patch)
+        im.set_clip_path(patch)
+        im.autoscale_None()
+        ax.add_image(im)
 
     return im
 
 
 def plot_slices(
     maps: xr.DataArray | Sequence[xr.DataArray],
     figsize: tuple[float, float] | None = None,
```

### Comparing `erlab-2.5.4/src/erlab/plotting/plot3d.py` & `erlab-2.6.1/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.6.1/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.6.1/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.6.1/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.6.1/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.6.1/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.6.1/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/src/erlab.egg-info/PKG-INFO` & `erlab-2.6.1/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.5.4
+Version: 2.6.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.5.4/src/erlab.egg-info/SOURCES.txt` & `erlab-2.6.1/src/erlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 docs/source/contributing.rst
 docs/source/erlab.accessors.rst
 docs/source/erlab.analysis.rst
 docs/source/erlab.constants.rst
 docs/source/erlab.interactive.rst
 docs/source/erlab.io.rst
 docs/source/erlab.lattice.rst
-docs/source/erlab.parallel.rst
 docs/source/erlab.plotting.rst
+docs/source/erlab.utils.rst
 docs/source/getting-started.rst
 docs/source/index.rst
 docs/source/reference.rst
 docs/source/refs.bib
 docs/source/images/flowchart_multiple.pdf
 docs/source/images/flowchart_single.pdf
 docs/source/images/imagetool_dark.png
@@ -48,15 +48,14 @@
 docs/source/user-guide/indexing.ipynb
 docs/source/user-guide/io.ipynb
 docs/source/user-guide/kconv.ipynb
 docs/source/user-guide/plotting.ipynb
 src/erlab/__init__.py
 src/erlab/constants.py
 src/erlab/lattice.py
-src/erlab/parallel.py
 src/erlab.egg-info/PKG-INFO
 src/erlab.egg-info/SOURCES.txt
 src/erlab.egg-info/dependency_links.txt
 src/erlab.egg-info/requires.txt
 src/erlab.egg-info/top_level.txt
 src/erlab/accessors/__init__.py
 src/erlab/accessors/fit.py
@@ -66,14 +65,15 @@
 src/erlab/analysis/correlation.py
 src/erlab/analysis/gold.py
 src/erlab/analysis/image.py
 src/erlab/analysis/interpolate.py
 src/erlab/analysis/kspace.py
 src/erlab/analysis/transform.py
 src/erlab/analysis/utilities.py
+src/erlab/analysis/utils.py
 src/erlab/analysis/fit/__init__.py
 src/erlab/analysis/fit/minuit.py
 src/erlab/analysis/fit/models.py
 src/erlab/analysis/fit/spline.py
 src/erlab/analysis/fit/functions/__init__.py
 src/erlab/analysis/fit/functions/dynamic.py
 src/erlab/analysis/fit/functions/general.py
@@ -87,27 +87,29 @@
 src/erlab/interactive/derivative.py
 src/erlab/interactive/dtool.ui
 src/erlab/interactive/fermiedge.py
 src/erlab/interactive/kspace.py
 src/erlab/interactive/ktool.ui
 src/erlab/interactive/masktool.py
 src/erlab/interactive/utilities.py
+src/erlab/interactive/utils.py
 src/erlab/interactive/imagetool/__init__.py
 src/erlab/interactive/imagetool/controls.py
 src/erlab/interactive/imagetool/core.py
 src/erlab/interactive/imagetool/fastbinning.py
 src/erlab/interactive/imagetool/slicer.py
 src/erlab/interactive/imagetool/_deprecated/__init__.py
 src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
 src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
 src/erlab/io/__init__.py
 src/erlab/io/dataloader.py
 src/erlab/io/exampledata.py
 src/erlab/io/igor.py
 src/erlab/io/utilities.py
+src/erlab/io/utils.py
 src/erlab/io/characterization/__init__.py
 src/erlab/io/characterization/resistance.py
 src/erlab/io/characterization/xrd.py
 src/erlab/io/plugins/__init__.py
 src/erlab/io/plugins/da30.py
 src/erlab/io/plugins/kriss.py
 src/erlab/io/plugins/maestro.py
@@ -133,27 +135,31 @@
 src/erlab/plotting/IgorCT/morgenstemning.ibw
 src/erlab/plotting/stylelib/fira.mplstyle
 src/erlab/plotting/stylelib/firalight.mplstyle
 src/erlab/plotting/stylelib/khan.mplstyle
 src/erlab/plotting/stylelib/nature.mplstyle
 src/erlab/plotting/stylelib/poster.mplstyle
 src/erlab/plotting/stylelib/times.mplstyle
+src/erlab/utils/__init__.py
+src/erlab/utils/array.py
+src/erlab/utils/parallel.py
 templates/.macros.j2
 templates/.release_notes.md.j2
 templates/CHANGELOG.md.j2
 tests/test_constants.py
 tests/accessors/test_fit.py
 tests/accessors/test_kspace.py
 tests/analysis/test_fastbinning.py
 tests/analysis/test_gold.py
 tests/analysis/test_image.py
 tests/analysis/test_image_savgol.py
 tests/analysis/test_interpolate.py
 tests/analysis/test_kspace.py
-tests/analysis/test_utilities.py
+tests/analysis/test_mask.py
+tests/analysis/test_utils.py
 tests/analysis/fit/test_functions_dynamic.py
 tests/analysis/fit/test_functions_general.py
 tests/analysis/fit/test_minuit.py
 tests/analysis/fit/test_models.py
 tests/interactive/test_imagetool.py
 tests/interactive/test_tools.py
 tests/io/test_dataloader.py
```

### Comparing `erlab-2.5.4/src/erlab.egg-info/requires.txt` & `erlab-2.6.1/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/templates/.macros.j2` & `erlab-2.6.1/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/accessors/test_fit.py` & `erlab-2.6.1/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/accessors/test_kspace.py` & `erlab-2.6.1/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/fit/test_functions_dynamic.py` & `erlab-2.6.1/tests/analysis/fit/test_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/fit/test_functions_general.py` & `erlab-2.6.1/tests/analysis/fit/test_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/fit/test_minuit.py` & `erlab-2.6.1/tests/analysis/fit/test_minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/fit/test_models.py` & `erlab-2.6.1/tests/analysis/fit/test_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/test_fastbinning.py` & `erlab-2.6.1/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/test_gold.py` & `erlab-2.6.1/tests/analysis/test_gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/test_image.py` & `erlab-2.6.1/tests/analysis/test_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import erlab.analysis as era
 import numpy as np
+import pytest
 import xarray as xr
 
 
 def test_gaussian_filter():
     # Create a test input DataArray
     darr = xr.DataArray(np.arange(50, step=2).reshape((5, 5)), dims=["x", "y"])
 
@@ -119,14 +120,31 @@
 
     # Apply the minimum_gradient function
     result = era.image.minimum_gradient(darr).astype(np.float32)
 
     # Check if the result matches the expected output
     assert np.allclose(result, expected_output)
 
+    # Test decorators that check for input validity
+    darr = xr.DataArray(np.arange(5), dims=["x"])
+    with pytest.raises(
+        ValueError, match="Input must be a 2-dimensional xarray.DataArray"
+    ):
+        era.image.minimum_gradient(darr)
+
+    darr = xr.DataArray(
+        np.arange(50, step=2).reshape((5, 5)),
+        dims=["x", "y"],
+        coords={"x": [0, 1, 2, 4, 5]},
+    )
+    with pytest.raises(
+        ValueError, match="Coordinates for all dimensions must be uniformly spaced"
+    ):
+        era.image.minimum_gradient(darr)
+
 
 def test_scaled_laplace():
     # Create a test input DataArray
     darr = xr.DataArray(
         np.arange(50, step=2).reshape((5, 5)).astype(float), dims=["x", "y"]
     )
```

### Comparing `erlab-2.5.4/tests/analysis/test_image_savgol.py` & `erlab-2.6.1/tests/analysis/test_image_savgol.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/test_interpolate.py` & `erlab-2.6.1/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/test_kspace.py` & `erlab-2.6.1/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/analysis/test_utilities.py` & `erlab-2.6.1/tests/analysis/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import xarray as xr
-from erlab.analysis.utilities import shift
+from erlab.analysis.utils import shift
 
 
 def test_shift():
     # Create a test input DataArray
     darr = xr.DataArray(
         np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]).astype(float), dims=["x", "y"]
     )
```

### Comparing `erlab-2.5.4/tests/interactive/test_imagetool.py` & `erlab-2.6.1/tests/interactive/test_imagetool.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,35 +96,34 @@
         )
     with pytest.raises(ValueError, match="^Data shape does not match.*"):
         win.slicer_area.update_values(np.arange(24).reshape((4, 6)))
 
 
 def test_sync(qtbot):
     data = xr.DataArray(np.arange(25).reshape((5, 5)), dims=["x", "y"])
-    win = itool([data, data], link=True, link_colors=True, execute=False)
-    for w in win:
+    win0, win1 = itool([data, data], link=True, link_colors=True, execute=False)
+    for w in (win0, win1):
         qtbot.addWidget(w)
 
+    for w in (win0, win1):
         with qtbot.waitExposed(w):
             w.show()
             w.activateWindow()
             w.raise_()
 
-    win[1].slicer_area.set_colormap("ColdWarm", gamma=1.5)
-    assert (
-        win[0].slicer_area.colormap_properties == win[1].slicer_area.colormap_properties
-    )
+    win1.slicer_area.set_colormap("ColdWarm", gamma=1.5)
+    assert win0.slicer_area.colormap_properties == win1.slicer_area.colormap_properties
 
-    move_and_compare_values(qtbot, win[0], [12.0, 7.0, 6.0, 11.0], target_win=win[1])
+    move_and_compare_values(qtbot, win0, [12.0, 7.0, 6.0, 11.0], target_win=win1)
 
     # Transpose
-    qtbot.keyClick(win[1], QtCore.Qt.Key.Key_T)
-    move_and_compare_values(qtbot, win[0], [12.0, 11.0, 6.0, 7.0], target_win=win[1])
+    qtbot.keyClick(win1, QtCore.Qt.Key.Key_T)
+    move_and_compare_values(qtbot, win0, [12.0, 11.0, 6.0, 7.0], target_win=win1)
 
     # Set bin
-    win[1].slicer_area.set_bin(0, 2, update=False)
-    win[1].slicer_area.set_bin(1, 2, update=True)
+    win1.slicer_area.set_bin(0, 2, update=False)
+    win1.slicer_area.set_bin(1, 2, update=True)
 
     # Set all bins, same effect as above since we only have 1 cursor
-    win[1].slicer_area.set_bin_all(1, 2, update=True)
+    win1.slicer_area.set_bin_all(1, 2, update=True)
 
-    move_and_compare_values(qtbot, win[0], [9.0, 8.0, 3.0, 4.0], target_win=win[1])
+    move_and_compare_values(qtbot, win0, [9.0, 8.0, 3.0, 4.0], target_win=win1)
```

### Comparing `erlab-2.5.4/tests/interactive/test_tools.py` & `erlab-2.6.1/tests/interactive/test_tools.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/io/test_dataloader.py` & `erlab-2.6.1/tests/io/test_dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 return int(scan_num), {}
             else:
                 return None, None
 
         def generate_summary(self, data_dir):
             # Get all valid data files in directory
             files = {}
-            for path in erlab.io.utilities.get_files(data_dir, extensions=[".h5"]):
+            for path in erlab.io.utils.get_files(data_dir, extensions=[".h5"]):
                 # Base name
                 data_name = os.path.splitext(os.path.basename(path))[0]
 
                 # If multiple scans, strip the _S### part
                 name_match = re.match(r"(.*?_\d{3})_(?:_S\d{3})?", data_name)
                 if name_match is not None:
                     data_name = name_match.group(1)
```

### Comparing `erlab-2.5.4/tests/plotting/test_annotations.py` & `erlab-2.6.1/tests/plotting/test_annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/plotting/test_atoms.py` & `erlab-2.6.1/tests/plotting/test_atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/plotting/test_colors.py` & `erlab-2.6.1/tests/plotting/test_colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.4/tests/plotting/test_general.py` & `erlab-2.6.1/tests/plotting/test_general.py`

 * *Files identical despite different names*

