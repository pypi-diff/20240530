# Comparing `tmp/mc3-3.1.3.tar.gz` & `tmp/mc3-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc3-3.1.3.tar", last modified: Sat Jun 24 15:32:17 2023, max compression
+gzip compressed data, was "mc3-3.1.4.tar", last modified: Thu May 30 15:04:12 2024, max compression
```

## Comparing `mc3-3.1.3.tar` & `mc3-3.1.4.tar`

### file list

```diff
@@ -1,88 +1,82 @@
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.887901 mc3-3.1.3/
--rw-r--r--   0 pato       (501) staff       (20)      123 2023-04-13 07:59:40.000000 mc3-3.1.3/.readthedocs.yml
--rw-r--r--   0 pato       (501) staff       (20)     2943 2019-08-12 13:25:42.000000 mc3-3.1.3/CONTRIBUTING.md
--rw-r--r--   0 pato       (501) staff       (20)     1085 2022-05-11 13:31:47.000000 mc3-3.1.3/LICENSE
--rw-r--r--   0 pato       (501) staff       (20)      402 2022-05-11 13:31:47.000000 mc3-3.1.3/MANIFEST.in
--rw-r--r--   0 pato       (501) staff       (20)      991 2019-08-12 13:25:42.000000 mc3-3.1.3/Makefile
--rw-r--r--   0 pato       (501) staff       (20)     2422 2023-06-24 15:32:17.887760 mc3-3.1.3/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1779 2023-04-13 07:59:40.000000 mc3-3.1.3/README.md
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.875943 mc3-3.1.3/docs/
--rw-r--r--   0 pato       (501) staff       (20)     7657 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/Makefile
--rw-r--r--   0 pato       (501) staff       (20)    62757 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/api.rst
--rw-r--r--   0 pato       (501) staff       (20)    11541 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/conf.py
--rw-r--r--   0 pato       (501) staff       (20)     2970 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/contributing.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.877684 mc3-3.1.3/docs/figures/
--rw-r--r--   0 pato       (501) staff       (20)    32125 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/figures/quad_bestfit.png
--rw-r--r--   0 pato       (501) staff       (20)    34319 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/figures/quad_fitting.png
--rw-r--r--   0 pato       (501) staff       (20)    46027 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/figures/quad_hist.png
--rw-r--r--   0 pato       (501) staff       (20)   242288 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/figures/quad_pairwise.png
--rw-r--r--   0 pato       (501) staff       (20)   211712 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/figures/quad_trace.png
--rw-r--r--   0 pato       (501) staff       (20)    48970 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/figures/rms-vs-binsize.png
--rw-r--r--   0 pato       (501) staff       (20)     8854 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/fit_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     6915 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/get_started.rst
--rw-r--r--   0 pato       (501) staff       (20)     4370 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/index.rst
--rw-r--r--   0 pato       (501) staff       (20)     1140 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/license.rst
--rw-r--r--   0 pato       (501) staff       (20)     7243 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/make.bat
--rw-r--r--   0 pato       (501) staff       (20)    28030 2023-04-13 07:59:40.000000 mc3-3.1.3/docs/mcmc_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     1691 2019-08-12 13:25:42.000000 mc3-3.1.3/docs/references.rst
--rw-r--r--   0 pato       (501) staff       (20)     1333 2022-05-11 13:31:47.000000 mc3-3.1.3/docs/time_averaging.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.880246 mc3-3.1.3/examples/
--rw-r--r--   0 pato       (501) staff       (20)     1650 2023-04-13 07:59:40.000000 mc3-3.1.3/examples/get_started.py
--rw-r--r--   0 pato       (501) staff       (20)     2243 2019-08-12 13:25:42.000000 mc3-3.1.3/examples/ns_tutorial.py
--rw-r--r--   0 pato       (501) staff       (20)     1148 2023-04-14 13:30:47.000000 mc3-3.1.3/examples/ppf.py
--rw-r--r--   0 pato       (501) staff       (20)     1556 2019-08-12 13:25:42.000000 mc3-3.1.3/examples/timeavg.py
--rw-r--r--   0 pato       (501) staff       (20)     2792 2023-04-13 07:59:40.000000 mc3-3.1.3/examples/tutorial.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.881518 mc3-3.1.3/mc3/
--rw-r--r--   0 pato       (501) staff       (20)      688 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    10937 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/__main__.py
--rw-r--r--   0 pato       (501) staff       (20)    13086 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/chain.py
--rw-r--r--   0 pato       (501) staff       (20)     9288 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/fit_driver.py
--rw-r--r--   0 pato       (501) staff       (20)    13642 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/mcmc_driver.py
--rw-r--r--   0 pato       (501) staff       (20)     6544 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/ns_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.883076 mc3-3.1.3/mc3/plots/
--rw-r--r--   0 pato       (501) staff       (20)      604 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/plots/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     5594 2023-06-24 15:31:48.000000 mc3-3.1.3/mc3/plots/colors.py
--rw-r--r--   0 pato       (501) staff       (20)    23328 2021-01-24 14:25:07.000000 mc3-3.1.3/mc3/plots/mc3_plots.py
--rw-r--r--   0 pato       (501) staff       (20)    10671 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/plots/plot_functions.py
--rw-r--r--   0 pato       (501) staff       (20)    39119 2023-06-02 12:30:58.000000 mc3-3.1.3/mc3/plots/posterior.py
--rw-r--r--   0 pato       (501) staff       (20)    24594 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/sampler_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.884992 mc3-3.1.3/mc3/stats/
--rw-r--r--   0 pato       (501) staff       (20)      638 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     2674 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/gelman.py
--rw-r--r--   0 pato       (501) staff       (20)      811 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/prayer.py
--rw-r--r--   0 pato       (501) staff       (20)    36306 2023-06-24 15:31:48.000000 mc3-3.1.3/mc3/stats/stats.py
--rw-r--r--   0 pato       (501) staff       (20)     1589 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/stats/time_averaging.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.885732 mc3-3.1.3/mc3/utils/
--rw-r--r--   0 pato       (501) staff       (20)      529 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/utils/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     7119 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/utils/log.py
--rw-r--r--   0 pato       (501) staff       (20)    13722 2023-04-13 07:59:40.000000 mc3-3.1.3/mc3/utils/utils.py
--rw-r--r--   0 pato       (501) staff       (20)      275 2023-06-24 15:31:48.000000 mc3-3.1.3/mc3/version.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.882142 mc3-3.1.3/mc3.egg-info/
--rw-r--r--   0 pato       (501) staff       (20)     2422 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1484 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/SOURCES.txt
--rw-r--r--   0 pato       (501) staff       (20)        1 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/dependency_links.txt
--rw-r--r--   0 pato       (501) staff       (20)       43 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/entry_points.txt
--rw-r--r--   0 pato       (501) staff       (20)       45 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/requires.txt
--rw-r--r--   0 pato       (501) staff       (20)        4 2023-06-24 15:32:17.000000 mc3-3.1.3/mc3.egg-info/top_level.txt
--rw-r--r--   0 pato       (501) staff       (20)      144 2022-05-11 13:31:47.000000 mc3-3.1.3/pyproject.toml
--rw-r--r--   0 pato       (501) staff       (20)      150 2019-08-12 13:25:42.000000 mc3-3.1.3/pytest.ini
--rw-r--r--   0 pato       (501) staff       (20)       57 2023-04-13 07:59:40.000000 mc3-3.1.3/requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)       38 2023-06-24 15:32:17.887943 mc3-3.1.3/setup.cfg
--rw-r--r--   0 pato       (501) staff       (20)     1728 2023-06-24 15:31:48.000000 mc3-3.1.3/setup.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.886260 mc3-3.1.3/src_c/
--rw-r--r--   0 pato       (501) staff       (20)     3973 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_binarray.c
--rw-r--r--   0 pato       (501) staff       (20)     7667 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_chisq.c
--rw-r--r--   0 pato       (501) staff       (20)    10514 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_dwt.c
--rw-r--r--   0 pato       (501) staff       (20)     6902 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/_time_averaging.c
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.886631 mc3-3.1.3/src_c/include/
--rw-r--r--   0 pato       (501) staff       (20)      522 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/include/ind.h
--rw-r--r--   0 pato       (501) staff       (20)     6646 2023-06-24 15:31:48.000000 mc3-3.1.3/src_c/include/stats.h
--rw-r--r--   0 pato       (501) staff       (20)     4185 2023-04-13 07:59:40.000000 mc3-3.1.3/src_c/include/wavelet.h
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-06-24 15:32:17.887547 mc3-3.1.3/tests/
--rw-r--r--   0 pato       (501) staff       (20)     5592 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_dynesty.py
--rw-r--r--   0 pato       (501) staff       (20)     3988 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_fit.py
--rw-r--r--   0 pato       (501) staff       (20)     2281 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_logging.py
--rw-r--r--   0 pato       (501) staff       (20)    15975 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_mcmc.py
--rw-r--r--   0 pato       (501) staff       (20)     3790 2023-06-24 15:31:48.000000 mc3-3.1.3/tests/test_plots.py
--rw-r--r--   0 pato       (501) staff       (20)    14911 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_stats.py
--rw-r--r--   0 pato       (501) staff       (20)     8937 2023-04-13 07:59:40.000000 mc3-3.1.3/tests/test_utils.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.344791 mc3-3.1.4/
+-rw-r--r--   0 pato       (501) staff       (20)      123 2024-05-30 15:02:31.000000 mc3-3.1.4/.readthedocs.yml
+-rw-r--r--   0 pato       (501) staff       (20)     2943 2021-03-08 22:07:25.000000 mc3-3.1.4/CONTRIBUTING.md
+-rw-r--r--   0 pato       (501) staff       (20)     1085 2024-05-30 15:02:31.000000 mc3-3.1.4/LICENSE
+-rw-r--r--   0 pato       (501) staff       (20)      365 2024-05-30 15:03:29.000000 mc3-3.1.4/MANIFEST.in
+-rw-r--r--   0 pato       (501) staff       (20)     3486 2024-05-30 15:04:12.344506 mc3-3.1.4/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1779 2024-05-30 15:02:31.000000 mc3-3.1.4/README.md
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.329627 mc3-3.1.4/docs/
+-rw-r--r--   0 pato       (501) staff       (20)     7657 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)    62757 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/api.rst
+-rw-r--r--   0 pato       (501) staff       (20)    11541 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/conf.py
+-rw-r--r--   0 pato       (501) staff       (20)     2970 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/contributing.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.332649 mc3-3.1.4/docs/figures/
+-rw-r--r--   0 pato       (501) staff       (20)    32125 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/figures/quad_bestfit.png
+-rw-r--r--   0 pato       (501) staff       (20)    34319 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/figures/quad_fitting.png
+-rw-r--r--   0 pato       (501) staff       (20)    46027 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/figures/quad_hist.png
+-rw-r--r--   0 pato       (501) staff       (20)   242288 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/figures/quad_pairwise.png
+-rw-r--r--   0 pato       (501) staff       (20)   211712 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/figures/quad_trace.png
+-rw-r--r--   0 pato       (501) staff       (20)    48970 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/figures/rms-vs-binsize.png
+-rw-r--r--   0 pato       (501) staff       (20)     8854 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/fit_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     6737 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/get_started.rst
+-rw-r--r--   0 pato       (501) staff       (20)     4370 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/index.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1140 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/license.rst
+-rw-r--r--   0 pato       (501) staff       (20)     7243 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/make.bat
+-rw-r--r--   0 pato       (501) staff       (20)    28030 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/mcmc_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1691 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/references.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1333 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/time_averaging.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.335390 mc3-3.1.4/examples/
+-rw-r--r--   0 pato       (501) staff       (20)     1650 2024-05-30 15:02:31.000000 mc3-3.1.4/examples/get_started.py
+-rw-r--r--   0 pato       (501) staff       (20)     1556 2021-03-08 22:07:25.000000 mc3-3.1.4/examples/timeavg.py
+-rw-r--r--   0 pato       (501) staff       (20)     2792 2024-05-30 15:02:31.000000 mc3-3.1.4/examples/tutorial.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.336823 mc3-3.1.4/mc3/
+-rw-r--r--   0 pato       (501) staff       (20)      688 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    10897 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/__main__.py
+-rw-r--r--   0 pato       (501) staff       (20)    13086 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/chain.py
+-rw-r--r--   0 pato       (501) staff       (20)     9288 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/fit_driver.py
+-rw-r--r--   0 pato       (501) staff       (20)    13642 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/mcmc_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.340205 mc3-3.1.4/mc3/plots/
+-rw-r--r--   0 pato       (501) staff       (20)      604 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     5594 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/colors.py
+-rw-r--r--   0 pato       (501) staff       (20)    10671 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/plot_functions.py
+-rw-r--r--   0 pato       (501) staff       (20)    39119 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/posterior.py
+-rw-r--r--   0 pato       (501) staff       (20)    23046 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/sampler_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.341333 mc3-3.1.4/mc3/stats/
+-rw-r--r--   0 pato       (501) staff       (20)      638 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     2674 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/gelman.py
+-rw-r--r--   0 pato       (501) staff       (20)      811 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/prayer.py
+-rw-r--r--   0 pato       (501) staff       (20)    36306 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     1589 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/time_averaging.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.341772 mc3-3.1.4/mc3/utils/
+-rw-r--r--   0 pato       (501) staff       (20)      529 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/utils/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     7119 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/utils/log.py
+-rw-r--r--   0 pato       (501) staff       (20)    13722 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/utils/utils.py
+-rw-r--r--   0 pato       (501) staff       (20)      275 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/version.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.344111 mc3-3.1.4/mc3.egg-info/
+-rw-r--r--   0 pato       (501) staff       (20)     3486 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1373 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/SOURCES.txt
+-rw-r--r--   0 pato       (501) staff       (20)        1 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/dependency_links.txt
+-rw-r--r--   0 pato       (501) staff       (20)       42 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/entry_points.txt
+-rw-r--r--   0 pato       (501) staff       (20)       65 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/requires.txt
+-rw-r--r--   0 pato       (501) staff       (20)        4 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/top_level.txt
+-rw-r--r--   0 pato       (501) staff       (20)     1075 2024-05-30 15:02:31.000000 mc3-3.1.4/pyproject.toml
+-rw-r--r--   0 pato       (501) staff       (20)      150 2021-03-08 22:07:25.000000 mc3-3.1.4/pytest.ini
+-rw-r--r--   0 pato       (501) staff       (20)       57 2024-05-30 15:02:31.000000 mc3-3.1.4/requirements.txt
+-rw-r--r--   0 pato       (501) staff       (20)       38 2024-05-30 15:04:12.344832 mc3-3.1.4/setup.cfg
+-rw-r--r--   0 pato       (501) staff       (20)      833 2024-05-30 15:02:31.000000 mc3-3.1.4/setup.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.342362 mc3-3.1.4/src_c/
+-rw-r--r--   0 pato       (501) staff       (20)     3973 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_binarray.c
+-rw-r--r--   0 pato       (501) staff       (20)     7667 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_chisq.c
+-rw-r--r--   0 pato       (501) staff       (20)    10514 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_dwt.c
+-rw-r--r--   0 pato       (501) staff       (20)     6902 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_time_averaging.c
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.342827 mc3-3.1.4/src_c/include/
+-rw-r--r--   0 pato       (501) staff       (20)      522 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/include/ind.h
+-rw-r--r--   0 pato       (501) staff       (20)     6646 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/include/stats.h
+-rw-r--r--   0 pato       (501) staff       (20)     4185 2024-05-30 15:02:32.000000 mc3-3.1.4/src_c/include/wavelet.h
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.343894 mc3-3.1.4/tests/
+-rw-r--r--   0 pato       (501) staff       (20)     3988 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_fit.py
+-rw-r--r--   0 pato       (501) staff       (20)     2281 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_logging.py
+-rw-r--r--   0 pato       (501) staff       (20)    15975 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_mcmc.py
+-rw-r--r--   0 pato       (501) staff       (20)     3790 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_plots.py
+-rw-r--r--   0 pato       (501) staff       (20)    14911 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     8937 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_utils.py
```

### Comparing `mc3-3.1.3/CONTRIBUTING.md` & `mc3-3.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/LICENSE` & `mc3-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/PKG-INFO` & `mc3-3.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,43 @@
-Metadata-Version: 2.1
-Name: mc3
-Version: 3.1.3
-Summary: Multi-core Markov-chain Monte Carlo package.
-Home-page: https://github.com/pcubillos/mc3
-Author: Patricio Cubillos
-Author-email: patricio.cubillos@oeaw.ac.at
-License: MIT
-Description: # mc3: Multi-core Markov-chain Monte Carlo
-        > A Python implementation of the Markov-chain Monte Carlo algorithm.
-        
-        [![Tests](https://github.com/pcubillos/mc3/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/pcubillos/mc3/actions/workflows/python-package.yml)
-        [![Documentation Status](https://readthedocs.org/projects/mc3/badge/?version=latest)](https://mc3.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/mc3.svg)](https://pypi.org/project/mc3)
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/mc3.svg)](https://anaconda.org/conda-forge/mc3)
-        [![GitHub](https://img.shields.io/github/license/pcubillos/mc3.svg?color=blue)](https://mc3.readthedocs.io/en/latest/license.html)
-        
-        ### Install as:
-        ```
-        pip install mc3
-        ```
-        or:
-        ```
-        conda install -c conda-forge mc3
-        ```
-        
-        ### Docs at:
-        <https://mc3.readthedocs.io/en/latest/>
-        
-        ### Cite as:
-        ```bibtex
-        @ARTICLE{CubillosEtal2017apjRednoise,
-               author = {{Cubillos}, Patricio and {Harrington}, Joseph and {Loredo}, Thomas J. and {Lust}, Nate B. and {Blecic}, Jasmina and {Stemm}, Madison},
-                title = "{On Correlated-noise Analyses Applied to Exoplanet Light Curves}",
-              journal = {\aj},
-             keywords = {methods: statistical, planets and satellites: fundamental parameters, techniques: photometric, Astrophysics - Earth and Planetary Astrophysics},
-                 year = 2017,
-                month = jan,
-               volume = {153},
-               number = {1},
-                  eid = {3},
-                pages = {3},
-                  doi = {10.3847/1538-3881/153/1/3},
-        archivePrefix = {arXiv},
-               eprint = {1610.01336},
-         primaryClass = {astro-ph.EP},
-               adsurl = {https://ui.adsabs.harvard.edu/abs/2017AJ....153....3C},
-              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-        }
-        ```
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# mc3: Multi-core Markov-chain Monte Carlo
+> A Python implementation of the Markov-chain Monte Carlo algorithm.
+
+[![Tests](https://github.com/pcubillos/mc3/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/pcubillos/mc3/actions/workflows/python-package.yml)
+[![Documentation Status](https://readthedocs.org/projects/mc3/badge/?version=latest)](https://mc3.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/mc3.svg)](https://pypi.org/project/mc3)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/mc3.svg)](https://anaconda.org/conda-forge/mc3)
+[![GitHub](https://img.shields.io/github/license/pcubillos/mc3.svg?color=blue)](https://mc3.readthedocs.io/en/latest/license.html)
+
+### Install as:
+```
+pip install mc3
+```
+or:
+```
+conda install -c conda-forge mc3
+```
+
+### Docs at:
+<https://mc3.readthedocs.io/en/latest/>
+
+### Cite as:
+```bibtex
+@ARTICLE{CubillosEtal2017apjRednoise,
+       author = {{Cubillos}, Patricio and {Harrington}, Joseph and {Loredo}, Thomas J. and {Lust}, Nate B. and {Blecic}, Jasmina and {Stemm}, Madison},
+        title = "{On Correlated-noise Analyses Applied to Exoplanet Light Curves}",
+      journal = {\aj},
+     keywords = {methods: statistical, planets and satellites: fundamental parameters, techniques: photometric, Astrophysics - Earth and Planetary Astrophysics},
+         year = 2017,
+        month = jan,
+       volume = {153},
+       number = {1},
+          eid = {3},
+        pages = {3},
+          doi = {10.3847/1538-3881/153/1/3},
+archivePrefix = {arXiv},
+       eprint = {1610.01336},
+ primaryClass = {astro-ph.EP},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2017AJ....153....3C},
+      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+}
+```
+
```

### Comparing `mc3-3.1.3/docs/Makefile` & `mc3-3.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/api.rst` & `mc3-3.1.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/conf.py` & `mc3-3.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/contributing.rst` & `mc3-3.1.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/figures/quad_bestfit.png` & `mc3-3.1.4/docs/figures/quad_bestfit.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/figures/quad_fitting.png` & `mc3-3.1.4/docs/figures/quad_fitting.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/figures/quad_hist.png` & `mc3-3.1.4/docs/figures/quad_hist.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/figures/quad_pairwise.png` & `mc3-3.1.4/docs/figures/quad_pairwise.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/figures/quad_trace.png` & `mc3-3.1.4/docs/figures/quad_trace.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/figures/rms-vs-binsize.png` & `mc3-3.1.4/docs/figures/rms-vs-binsize.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/fit_tutorial.rst` & `mc3-3.1.4/docs/fit_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/get_started.rst` & `mc3-3.1.4/docs/get_started.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,16 @@
 
 Getting Started
 ===============
 
 System Requirements
 -------------------
 
-``mc3`` is compatible with Python 3.6+, and has been `tested
-<https://github.com/pcubillos/mc3/actions/workflows/python-package.yml>`_ to work on Unix/Linux and
-OS X machines, with the following software:
-
-* Numpy >= 1.19.5
-* Scipy >= 1.9.3
-* Matplotlib >= 3.3.4
-
-``mc3`` may work with previous versions of these software;
-however, we do not guarantee nor provide support for that.
-
+``mc3`` is compatible with Python 3.7+, and has been `tested
+<https://github.com/pcubillos/mc3/actions/workflows/python-package.yml>`_ to work on Unix/Linux and OS X machines.
 
 Install
 -------
 
 To install ``mc3`` run the following command from the terminal:
 
 .. code-block:: shell
@@ -35,31 +26,35 @@
 
 Alternatively (e.g., for developers), clone the repository to your local machine with the following terminal commands:
 
 .. code-block:: shell
 
     git clone https://github.com/pcubillos/mc3
     cd mc3
+    pip install -r requirements.txt
     pip install -e .
 
 
-``mc3`` provides MCMC and nested-sampling posterior sampling,
+``mc3`` provides MCMC posterior sampling,
 optimization and other lower-level statistical and plotting
 routines. See the full docs in the :ref:`api` or through the Python
 interpreter:
 
 .. code-block:: python
 
     import mc3
     # Bayesian posterior sampling:
     help(mc3.sample)
+
     # Optimization:
     help(mc3.fit)
-    # Assorted stats:
+
+    # Assorted stats utilities:
     help(mc3.stats)
+
     # Plotting utilities:
     help(mc3.plots)
 
 
 Example 1: Interactive Run
 --------------------------
```

### Comparing `mc3-3.1.3/docs/index.rst` & `mc3-3.1.4/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 :Web Site:      https://github.com/pcubillos/mc3
 :Date:          |today|
 
 -------------------------------------------------------------------
 
 .. note::
 
-    Got  Python3.6+? Simply install as: ``pip install mc3``
+    Got  Python3.7+? Simply install as: ``pip install mc3``
 
 
 Features
 ========
 
 ``mc3`` is a Bayesian-statistics tool that offers:
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 |License| .. raw:: html
 ------------------------------------------------------------------- :Author:
 Patricio Cubillos and collaborators (see :ref:`team`) :Contact:
 `patricio.cubillos[at]oeaw.ac.at`_ :Organizations: `Space Research Institute
 (IWF)
 iwf.oeaw.ac.at/>`_ :Web Site: https://github.com/pcubillos/mc3 :Date: |today| -
 ------------------------------------------------------------------ .. note::
-Got Python3.6+? Simply install as: ``pip install mc3`` Features ========
+Got Python3.7+? Simply install as: ``pip install mc3`` Features ========
 ``mc3`` is a Bayesian-statistics tool that offers: - Levenberg-Marquardt least-
 squares optimization. - Markov-chain Monte Carlo (MCMC) posterior-distribution
 sampling following the: - Metropolis-Hastings algorithm with Gaussian proposal
 distribution, - Differential-Evolution MCMC (DEMC), or - DEMCzs (Snooker). .. -
 Nested-sampling via `dynesty
 dynesty.readthedocs.io/en/latest/>`_. The following features are available when
 running ``mc3``: - Execution from the Shell prompt or interactively through the
```

### Comparing `mc3-3.1.3/docs/license.rst` & `mc3-3.1.4/docs/license.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/make.bat` & `mc3-3.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/mcmc_tutorial.rst` & `mc3-3.1.4/docs/mcmc_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/references.rst` & `mc3-3.1.4/docs/references.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/docs/time_averaging.rst` & `mc3-3.1.4/docs/time_averaging.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/examples/get_started.py` & `mc3-3.1.4/examples/get_started.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/examples/ns_tutorial.py` & `mc3-3.1.4/examples/tutorial.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,63 +15,92 @@
     """
     y = p[0] + p[1]*x + p[2]*x**2.0
     return y
 
 # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 # Preamble (create a synthetic dataset, in a real scenario you would
 # get your dataset from your own data analysis pipeline):
-np.random.seed(3)
-x  = np.linspace(0, 10, 100)
+np.random.seed(314)
+x  = np.linspace(0, 10, 1000)
 p0 = [3, -2.4, 0.5]
 y  = quad(p0, x)
+
 uncert = np.sqrt(np.abs(y))
-data   = y + np.random.normal(0, uncert)
+error  = np.random.normal(0, uncert)
+data   = y + error
 # ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
-# Modeling function:
+# Define the modeling function as a callable:
 func = quad
+
 # List of additional arguments of func (if necessary):
 indparams = [x]
 
 # Array of initial-guess values of fitting parameters:
 params = np.array([ 10.0, -2.0, 0.1])
 # Lower and upper boundaries for the MCMC exploration:
 pmin = np.array([-10.0, -20.0, -10.0])
 pmax = np.array([ 40.0,  20.0,  10.0])
 # Parameters' stepping behavior:
 pstep = np.array([1.0, 0.5, 0.1])
 
-# Two-sided Gaussian prior on first parameter, uniform priors on rest:
-prior    = np.array([3.5, 0.0, 0.0])
-priorlow = np.array([0.1, 0.0, 0.0])
-priorup  = np.array([0.3, 0.0, 0.0])
+# Parameter prior probability distributions:
+prior    = np.array([ 0.0, 0.0, 0.0])
+priorlow = np.array([ 0.0, 0.0, 0.0])
+priorup  = np.array([ 0.0, 0.0, 0.0])
 
 # Parameter names:
-pnames   = ['y0', 'alpha', 'beta']
+pnames = ['y0', 'alpha', 'beta']
 texnames = [r'$y_{0}$', r'$\alpha$', r'$\beta$']
 
-# Sampler algorithm, choose from: 'snooker', 'demc', 'mrw', or 'dynesty'.
-sampler = 'dynesty'
+# Sampler algorithm, choose from: 'snooker', 'demc' or 'mrw'.
+sampler = 'snooker'
+
+# MCMC setup:
+nsamples =  1e5
+burnin   = 1000
+nchains  =   14
+ncpu     =    7
+thinning =    1
+
+# MCMC initial draw, choose from: 'normal' or 'uniform'
+kickoff = 'normal'
+# DEMC snooker pre-MCMC sample size:
+hsize = 10
 
 # Optimization before MCMC, choose from: 'lm' or 'trf':
-leastsq    = 'lm'
+leastsq = 'lm'
 chisqscale = False
-# NS setup:
-ncpu     = 7
-thinning = 1
+
+# MCMC Convergence:
+grtest = True
+grbreak = 1.01
+grnmin = 0.5
 
 # Logging:
-log = 'NS_tutorial.log'
+log = 'MCMC_tutorial.log'
 
 # File outputs:
-savefile = 'NS_tutorial.npz'
-plots    = True
-rms      = True
+savefile = 'MCMC_tutorial.npz'
+plots = True
+theme = 'indigo'
+statistics = 'med_central'
+rms = True
+
+# Carter & Winn (2009) Wavelet-likelihood method:
+wlike = False
 
 # Run the MCMC:
-mc3_output = mc3.sample(data=data, uncert=uncert, func=func, params=params,
-     indparams=indparams, pmin=pmin, pmax=pmax, pstep=pstep,
-     pnames=pnames, texnames=texnames,
-     prior=prior, priorlow=priorlow, priorup=priorup,
-     sampler=sampler, ncpu=ncpu, thinning=thinning,
-     leastsq=leastsq, chisqscale=chisqscale,
-     plots=plots, rms=rms, log=log, savefile=savefile)
+output = mc3.sample(
+    data=data, uncert=uncert, func=func, params=params,
+    indparams=indparams, pmin=pmin, pmax=pmax, pstep=pstep,
+    pnames=pnames, texnames=texnames,
+    prior=prior, priorlow=priorlow, priorup=priorup,
+    sampler=sampler, nsamples=nsamples,  nchains=nchains,
+    ncpu=ncpu, burnin=burnin, thinning=thinning,
+    leastsq=leastsq, chisqscale=chisqscale,
+    grtest=grtest, grbreak=grbreak, grnmin=grnmin,
+    hsize=hsize, kickoff=kickoff,
+    wlike=wlike, log=log,
+    plots=plots, theme=theme, statistics=statistics,
+    savefile=savefile, rms=rms,
+)
```

### Comparing `mc3-3.1.3/examples/timeavg.py` & `mc3-3.1.4/examples/timeavg.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/__init__.py` & `mc3-3.1.4/mc3/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/__main__.py` & `mc3-3.1.4/mc3/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 import sys
 import os
 import warnings
 import argparse
 import configparser
 
-import matplotlib as mpl
-if os.environ.get('DISPLAY', '') == '':
-    mpl.use('Agg')
+import matplotlib
 import matplotlib.pyplot as plt
 
 import mc3
 import mc3.utils as mu
 
 
 def main():
@@ -232,10 +230,11 @@
         default=None,
         help="Filename or array with prior upper uncertainties "
              "[default: %(default)s]")
     return parser
 
 
 if __name__ == "__main__":
+    matplotlib.use('Agg')
     plt.ioff()
     warnings.simplefilter("ignore", RuntimeWarning)
     main()
```

### Comparing `mc3-3.1.3/mc3/chain.py` & `mc3-3.1.4/mc3/chain.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/fit_driver.py` & `mc3-3.1.4/mc3/fit_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/mcmc_driver.py` & `mc3-3.1.4/mc3/mcmc_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/plots/__init__.py` & `mc3-3.1.4/mc3/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/plots/colors.py` & `mc3-3.1.4/mc3/plots/colors.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/plots/plot_functions.py` & `mc3-3.1.4/mc3/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/plots/posterior.py` & `mc3-3.1.4/mc3/plots/posterior.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/sampler_driver.py` & `mc3-3.1.4/mc3/sampler_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,18 @@
 import os
 import sys
 import importlib
 import multiprocessing as mpr
 from datetime import date
 
 import numpy as np
-import matplotlib as mpl
-if os.environ.get('DISPLAY', '') == '':
-    mpl.use('Agg')
 import matplotlib.pyplot as plt
 
 from .fit_driver import fit
 from .mcmc_driver import mcmc
-from .ns_driver import nested_sampling
 from . import utils as mu
 from . import stats as ms
 from . import plots as mp
 from .version import __version__
 
 
 def sample(
@@ -87,15 +83,14 @@
     priorup: 1D ndarray
         Upper prior uncertainty values.
     sampler: String
         Sampling algorithm:
         - 'mrw':  Metropolis random walk.
         - 'demc': Differential Evolution Markov chain.
         - 'snooker': DEMC-z with snooker update.
-        - 'dynesty': DynamicNestedSampler() sampler from dynesty.
     ncpu: Integer
         Number of processors for the MCMC chains (mc3 defaults to
         one CPU for each chain plus a CPU for the central hub).
     leastsq: String
         If not None, perform a least-square optimization before the MCMC run.
         Select from:
             'lm': Levenberg-Marquardt (most efficient, but doesn't obey bounds)
@@ -249,24 +244,16 @@
     >>> # MCMC sampling:
     >>> mcmc_output = mc3.sample(
     >>>     data, uncert, func, params, indparams=indparams,
     >>>     sampler='snooker', pstep=pstep, ncpu=ncpu, pmin=pmin, pmax=pmax,
     >>>     prior=prior, priorlow=priorlow, priorup=priorup,
     >>>     leastsq='lm', nsamples=1e5, burnin=1000, plots=True)
 
-    >>> # Nested sampling:
-    >>> ns_output = mc3.sample(
-    >>>     data, uncert, func, params, indparams=indparams,
-    >>>     sampler='dynesty', pstep=pstep, ncpu=ncpu, pmin=pmin, pmax=pmax,
-    >>>     prior=prior, priorlow=priorlow, priorup=priorup,
-    >>>     leastsq='lm', plots=True)
-
     >>> # See more examples and details at:
     >>> # https://mc3.readthedocs.io/en/latest/mcmc_tutorial.html
-    >>> # https://mc3.readthedocs.io/en/latest/ns_tutorial.html
     """
     # Logging object:
     if isinstance(log, str):
         log = mu.Log(log, append=resume)
         closelog = True
     else:
         closelog = False
@@ -341,16 +328,14 @@
     elif not callable(func):
         log.error(
             "'func' must be either a callable or an iterable of strings "
             "with the model function, file, and path names")
 
     if ncpu is None and sampler in ['snooker', 'demc', 'mrw']:
         ncpu = nchains
-    elif ncpu is None and sampler == 'dynesty':
-        ncpu = 1
     # Cap the number of processors:
     if ncpu >= mpr.cpu_count():
         log.warning(
             f"The number of requested CPUs ({ncpu}) is >= than the number "
             f"of available CPUs ({mpr.cpu_count()}).  "
             f"Enforced ncpu to {mpr.cpu_count()-1}.")
         ncpu = mpr.cpu_count() - 1
@@ -370,18 +355,14 @@
 
     if pmin is None:
         pmin = np.tile(-np.inf, nparams)
     if pmax is None:
         pmax = np.tile( np.inf, nparams)
     pmin = np.asarray(pmin)
     pmax = np.asarray(pmax)
-    if (np.any(np.isinf(pmin)) or np.any(np.isinf(pmax))) \
-            and sampler=='dynesty':
-        log.error('Parameter space must be constrained by pmin and pmax')
-
     if pstep is None:
         pstep = 0.1 * np.abs(params)
     pstep = np.asarray(pstep)
 
     # Set prior parameter indices:
     if prior is None or priorup is None or priorlow is None:
         prior = priorup = priorlow = np.zeros(nparams)
@@ -424,19 +405,14 @@
         if not os.path.exists(fpath):
             log.warning(
                 f"Output folder path: '{fpath}' does not exist. "
                 "Creating new folder."
             )
             os.makedirs(fpath)
 
-    # At the moment, skip optimization when these dynesty inputs exist:
-    if sampler == 'dynesty' \
-            and ('loglikelihood' in kwargs or 'prior_transform' in kwargs):
-        leastsq = None
-
     # Least-squares minimization:
     chisq_factor = 1.0
     if leastsq is not None:
         fit_output = fit(
             data, uncert, func, np.copy(params),
             indparams, indparams_dict,
             pstep, pmin, pmax, prior, priorlow, priorup, leastsq)
@@ -475,20 +451,14 @@
             params, indparams, indparams_dict,
             pmin, pmax, pstep,
             prior, priorlow, priorup, nchains, ncpu, nsamples, sampler,
             wlike, fit_output, grtest, grbreak, grnmin, burnin, thinning,
             fgamma, fepsilon, hsize, kickoff, savefile, resume, log,
             pnames, texnames,
         )
-    elif sampler == 'dynesty':
-        output = nested_sampling(
-            data, uncert, func, params, indparams, indparams_dict,
-            pmin, pmax, pstep, prior, priorlow, priorup, ncpu,
-            thinning, resume, log, **kwargs,
-        )
 
     # Get some stats:
     output['chisq_factor'] = chisq_factor
 
     if leastsq is not None:
         delta_log_post = output['best_log_post'] - fit_output['best_log_post']
         delta_pars = output['bestp'] - fit_output['bestp']
@@ -506,15 +476,14 @@
         Z=output['posterior'], zchain=output['zchain'], burnin=output['burnin'])
 
     bestp = output['bestp']
     post = mp.Posterior(
         posterior, pnames=texnames[ifree], theme=theme,
         bestp=bestp[ifree], statistics=statistics,
     )
-    print(post.statistics)
     # Let Posterior to turn the theme into a Theme() object:
     theme = post.theme
 
     # Parameter statistics:
     sample_stats = ms.calc_sample_statistics(
         post.posterior, bestp, pstep, calc_hpd=True,
     )
@@ -587,21 +556,16 @@
         '\nFor a detailed summary with all parameter posterior statistics '
         f'see {stats_file}',
     )
 
     log.msg("\nOutput sampler files:")
     log.msg(stats_file, indent=2)
 
-    # Save results (pop unpickables before saving, then put back):
     if savefile is not None:
-        unpickables = ['dynesty_sampler']
-        unpickables = np.intersect1d(unpickables, list(output.keys()))
-        tmp_outputs = {key: output.pop(key) for key in unpickables}
         np.savez(savefile, **output)
-        output.update(tmp_outputs)
         log.msg(savefile, indent=2)
 
     if plots:
         # Trace plot:
         savefile = f'{savefile_root}_trace.png'
         mp.trace(
             output['posterior'], zchain=output['zchain'],
```

### Comparing `mc3-3.1.3/mc3/stats/__init__.py` & `mc3-3.1.4/mc3/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/stats/gelman.py` & `mc3-3.1.4/mc3/stats/gelman.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/stats/prayer.py` & `mc3-3.1.4/mc3/stats/prayer.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/stats/stats.py` & `mc3-3.1.4/mc3/stats/stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/stats/time_averaging.py` & `mc3-3.1.4/mc3/stats/time_averaging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/utils/__init__.py` & `mc3-3.1.4/mc3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/utils/log.py` & `mc3-3.1.4/mc3/utils/log.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3/utils/utils.py` & `mc3-3.1.4/mc3/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/mc3.egg-info/SOURCES.txt` & `mc3-3.1.4/mc3.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .readthedocs.yml
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
-Makefile
 README.md
 pyproject.toml
 pytest.ini
 requirements.txt
 setup.py
 docs/Makefile
 docs/api.rst
@@ -23,35 +22,31 @@
 docs/figures/quad_bestfit.png
 docs/figures/quad_fitting.png
 docs/figures/quad_hist.png
 docs/figures/quad_pairwise.png
 docs/figures/quad_trace.png
 docs/figures/rms-vs-binsize.png
 examples/get_started.py
-examples/ns_tutorial.py
-examples/ppf.py
 examples/timeavg.py
 examples/tutorial.py
 mc3/__init__.py
 mc3/__main__.py
 mc3/chain.py
 mc3/fit_driver.py
 mc3/mcmc_driver.py
-mc3/ns_driver.py
 mc3/sampler_driver.py
 mc3/version.py
 mc3.egg-info/PKG-INFO
 mc3.egg-info/SOURCES.txt
 mc3.egg-info/dependency_links.txt
 mc3.egg-info/entry_points.txt
 mc3.egg-info/requires.txt
 mc3.egg-info/top_level.txt
 mc3/plots/__init__.py
 mc3/plots/colors.py
-mc3/plots/mc3_plots.py
 mc3/plots/plot_functions.py
 mc3/plots/posterior.py
 mc3/stats/__init__.py
 mc3/stats/gelman.py
 mc3/stats/prayer.py
 mc3/stats/stats.py
 mc3/stats/time_averaging.py
@@ -61,14 +56,13 @@
 src_c/_binarray.c
 src_c/_chisq.c
 src_c/_dwt.c
 src_c/_time_averaging.c
 src_c/include/ind.h
 src_c/include/stats.h
 src_c/include/wavelet.h
-tests/test_dynesty.py
 tests/test_fit.py
 tests/test_logging.py
 tests/test_mcmc.py
 tests/test_plots.py
 tests/test_stats.py
 tests/test_utils.py
```

### Comparing `mc3-3.1.3/src_c/_binarray.c` & `mc3-3.1.4/src_c/_binarray.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/src_c/_chisq.c` & `mc3-3.1.4/src_c/_chisq.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/src_c/_dwt.c` & `mc3-3.1.4/src_c/_dwt.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/src_c/_time_averaging.c` & `mc3-3.1.4/src_c/_time_averaging.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/src_c/include/ind.h` & `mc3-3.1.4/src_c/include/ind.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/src_c/include/stats.h` & `mc3-3.1.4/src_c/include/stats.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/src_c/include/wavelet.h` & `mc3-3.1.4/src_c/include/wavelet.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/tests/test_fit.py` & `mc3-3.1.4/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/tests/test_logging.py` & `mc3-3.1.4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/tests/test_mcmc.py` & `mc3-3.1.4/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/tests/test_plots.py` & `mc3-3.1.4/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/tests/test_stats.py` & `mc3-3.1.4/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.3/tests/test_utils.py` & `mc3-3.1.4/tests/test_utils.py`

 * *Files identical despite different names*

