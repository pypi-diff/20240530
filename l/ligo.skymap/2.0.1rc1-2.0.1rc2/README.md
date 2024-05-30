# Comparing `tmp/ligo_skymap-2.0.1rc1.tar.gz` & `tmp/ligo_skymap-2.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo_skymap-2.0.1rc1.tar", last modified: Fri May 24 14:10:55 2024, max compression
+gzip compressed data, was "ligo_skymap-2.0.1rc2.tar", last modified: Wed May 29 05:09:17 2024, max compression
```

## Comparing `ligo_skymap-2.0.1rc1.tar` & `ligo_skymap-2.0.1rc2.tar`

### file list

```diff
@@ -1,300 +1,300 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:55.000528 ligo_skymap-2.0.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.959528 ligo_skymap-2.0.1rc1/.gitlab/
--rwxrwxrwx   0 root         (0) root         (0)     2033 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/.gitlab/combine-coverage.py
--rw-rw-rw-   0 root         (0) root         (0)    13538 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    44679 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5187 2024-05-24 14:10:55.000528 ligo_skymap-2.0.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.953528 ligo_skymap-2.0.1rc1/cextern/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.959528 ligo_skymap-2.0.1rc1/cextern/chealpix/
--rw-rw-rw-   0 root         (0) root         (0)    30207 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/cextern/chealpix/chealpix.c
--rw-rw-rw-   0 root         (0) root         (0)     7407 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/cextern/chealpix/chealpix.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.961528 ligo_skymap-2.0.1rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4581 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.962528 ligo_skymap-2.0.1rc1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    34751 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/_static/benchmark.svg
--rw-rw-rw-   0 root         (0) root         (0)   567737 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/_static/coinc.xml
--rw-rw-rw-   0 root         (0) root         (0)   260305 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/_static/localization.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.953528 ligo_skymap-2.0.1rc1/docs/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.963528 ligo_skymap-2.0.1rc1/docs/_templates/autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0 root         (0) root         (0)      252 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.963528 ligo_skymap-2.0.1rc1/docs/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    56171 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/bayestar/eggbox.png
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/bayestar/ez_emcee.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/bayestar/filter.rst
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/bayestar/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/bayestar/interpolation.rst
--rw-rw-rw-   0 root         (0) root         (0)    44679 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/changes.rst
--rw-rw-rw-   0 root         (0) root         (0)     8757 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.964528 ligo_skymap-2.0.1rc1/docs/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/coordinates/detector.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/coordinates/eigenframe.rst
--rw-rw-rw-   0 root         (0) root         (0)     2393 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/develop.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.964528 ligo_skymap-2.0.1rc1/docs/distance/
--rw-rw-rw-   0 root         (0) root         (0)     1243 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/distance/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.964528 ligo_skymap-2.0.1rc1/docs/healpix_tree/
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/healpix_tree/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/help.rst
--rw-rw-rw-   0 root         (0) root         (0)     4582 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    15650 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/interface.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.964528 ligo_skymap-2.0.1rc1/docs/io/
--rw-rw-rw-   0 root         (0) root         (0)     3691 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/io/events.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/io/fits.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/io/hdf5.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.965528 ligo_skymap-2.0.1rc1/docs/kde/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/kde/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4549 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/matplotlibrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.965528 ligo_skymap-2.0.1rc1/docs/moc/
--rw-rw-rw-   0 root         (0) root         (0)      308 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/moc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/performance.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.966528 ligo_skymap-2.0.1rc1/docs/plot/
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/plot/allsky.rst
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/plot/backdrop.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/plot/bayes_factor.rst
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/plot/marker.rst
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/plot/poly.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/plot/pp.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.966528 ligo_skymap-2.0.1rc1/docs/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/postprocess/contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/postprocess/cosmology.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/postprocess/crossmatch.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/postprocess/ellipse.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/postprocess/util.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.967528 ligo_skymap-2.0.1rc1/docs/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     6351 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/quickstart/bayestar-injections.rst
--rw-rw-rw-   0 root         (0) root         (0)     4452 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/quickstart/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     6031 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/testing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.970528 ligo_skymap-2.0.1rc1/docs/tool/
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/bayestar_inject.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/bayestar_localize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/bayestar_localize_lvalert.rst
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/bayestar_mcmc.rst
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/bayestar_realize_coincs.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/bayestar_sample_model_psd.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_combine.rst
--rw-rw-rw-   0 root         (0) root         (0)     3709 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_constellations.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_contour.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_contour_moc.rst
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_flatten.rst
--rw-rw-rw-   0 root         (0) root         (0)     1387 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_from_samples.rst
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_airmass.rst
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_coherence.rst
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_observability.rst
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_volume.rst
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_stats.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_unflatten.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.970528 ligo_skymap-2.0.1rc1/docs/util/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/util/file.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/util/ilwd.rst
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/util/numpy.rst
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/docs/util/sqlite.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.971528 ligo_skymap-2.0.1rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     6360 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/licenses/CHEALPIX_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)    37565 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/licenses/NUMPY_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.955528 ligo_skymap-2.0.1rc1/ligo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.974528 ligo_skymap-2.0.1rc1/ligo/skymap/
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/_astropy_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.974528 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/
--rw-rw-rw-   0 root         (0) root         (0)    20357 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/ez_emcee.py
--rw-rw-rw-   0 root         (0) root         (0)    19685 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10348 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/ptemcee.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.975528 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1545 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4573 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/test_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)     4287 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.976528 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3645 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/detector.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/eigenframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.976528 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/tests/test_detector.py
--rw-rw-rw-   0 root         (0) root         (0)    21354 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/distance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.976528 ligo_skymap-2.0.1rc1/ligo/skymap/extern/
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/extern/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.976528 ligo_skymap-2.0.1rc1/ligo/skymap/extern/numpy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/extern/numpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13938 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/extern/numpy/quantile.py
--rw-rw-rw-   0 root         (0) root         (0)    15264 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/healpix_tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.977528 ligo_skymap-2.0.1rc1/ligo/skymap/io/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.978528 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/detector_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/gracedb.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/hdf.py
--rw-rw-rw-   0 root         (0) root         (0)    11536 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/ligolw.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/magic.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/events/sqlite.py
--rwxrwxrwx   0 root         (0) root         (0)    19227 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/fits.py
--rwxrwxrwx   0 root         (0) root         (0)    10626 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.978528 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.980528 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)   492938 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/2016_subset.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     1699 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G197392_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G211117_psd.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.980528 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/gstlal_reference_psd/
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9120 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/test.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    12825 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/test_io_events.py
--rw-rw-rw-   0 root         (0) root         (0)    17043 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/kde.py
--rw-rw-rw-   0 root         (0) root         (0)     7376 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.982528 ligo_skymap-2.0.1rc1/ligo/skymap/plot/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29444 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/allsky.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/angle.py
--rw-rw-rw-   0 root         (0) root         (0)     7312 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/backdrop.py
--rw-rw-rw-   0 root         (0) root         (0)     3915 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/bayes_factor.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/cmap.py
--rw-rw-rw-   0 root         (0) root         (0)     8720 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/cylon.csv
--rw-rw-rw-   0 root         (0) root         (0)     2131 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/cylon.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/marker.py
--rw-rw-rw-   0 root         (0) root         (0)    63275 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/ne_simplified_coastline.json
--rw-rw-rw-   0 root         (0) root         (0)     7394 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/poly.py
--rw-rw-rw-   0 root         (0) root         (0)     9445 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.983528 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.987528 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/
--rw-rw-rw-   0 root         (0) root         (0)    67688 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    66215 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    65823 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    64266 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    71787 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    71744 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    70520 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    69570 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    65034 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    63912 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    63615 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    61805 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    34054 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
--rw-rw-rw-   0 root         (0) root         (0)    26036 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    25898 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    24279 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png
--rw-rw-rw-   0 root         (0) root         (0)    22175 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png
--rw-rw-rw-   0 root         (0) root         (0)    20330 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_globe_axes.png
--rw-rw-rw-   0 root         (0) root         (0)    15198 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_plot_bayes_factor.png
--rw-rw-rw-   0 root         (0) root         (0)    19023 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
--rw-rw-rw-   0 root         (0) root         (0)    39922 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    19023 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
--rw-rw-rw-   0 root         (0) root         (0)     8797 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_reticle.png
--rw-rw-rw-   0 root         (0) root         (0)    19883 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
--rw-rw-rw-   0 root         (0) root         (0)     6245 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.988528 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2903 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    18290 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)    15257 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/ellipse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.989528 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/tests/test_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/tests/test_crossmatch.py
--rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.989528 ligo_skymap-2.0.1rc1/ligo/skymap/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.989528 ligo_skymap-2.0.1rc1/ligo/skymap/tests/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tests/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tests/plugins/omp.py
--rw-rw-rw-   0 root         (0) root         (0)     5704 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tests/test_moc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.993528 ligo_skymap-2.0.1rc1/ligo/skymap/tool/
--rw-rw-rw-   0 root         (0) root         (0)    15388 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21373 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     7333 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_localize_coincs.py
--rwxrwxrwx   0 root         (0) root         (0)     6682 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_localize_lvalert.py
--rw-rw-rw-   0 root         (0) root         (0)     8071 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_mcmc.py
--rw-rw-rw-   0 root         (0) root         (0)    18761 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_realize_coincs.py
--rw-rw-rw-   0 root         (0) root         (0)     4600 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_sample_model_psd.py
--rw-rw-rw-   0 root         (0) root         (0)     5841 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_constellations.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_contour_moc.py
--rw-rw-rw-   0 root         (0) root         (0)     2288 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     7662 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     6732 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     8353 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_airmass.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_coherence.py
--rw-rw-rw-   0 root         (0) root         (0)     5711 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_observability.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
--rw-rw-rw-   0 root         (0) root         (0)     8048 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     9391 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_volume.py
--rw-rw-rw-   0 root         (0) root         (0)    11830 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_unflatten.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.995528 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3088 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_bayestar.py
--rw-rw-rw-   0 root         (0) root         (0)     4496 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_bayestar_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_combine.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_from_samples.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_help.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_plot_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.996528 ligo_skymap-2.0.1rc1/ligo/skymap/util/
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5170 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/ilwd.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/math.py
--rw-rw-rw-   0 root         (0) root         (0)     2023 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4451 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/stopwatch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.996528 ligo_skymap-2.0.1rc1/ligo/skymap/util/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/ligo/skymap/util/tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo/skymap/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.999528 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5187 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8711 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1550 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-24 14:10:54.000000 ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     6374 2024-05-24 14:10:55.004528 ligo_skymap-2.0.1rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3807 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 14:10:54.999528 ligo_skymap-2.0.1rc1/src/
--rw-rw-rw-   0 root         (0) root         (0)    37062 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/src/bayestar_cosmology.h
--rw-rw-rw-   0 root         (0) root         (0)     4094 2024-05-24 14:10:40.000000 ligo_skymap-2.0.1rc1/src/bayestar_cosmology.py
--rw-rw-rw-   0 root         (0) root         (0)    16209 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/bayestar_distance.c
--rw-rw-rw-   0 root         (0) root         (0)     2067 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/bayestar_distance.h
--rw-rw-rw-   0 root         (0) root         (0)     4231 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/bayestar_moc.c
--rw-rw-rw-   0 root         (0) root         (0)     1512 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/bayestar_moc.h
--rw-rw-rw-   0 root         (0) root         (0)    50371 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/bayestar_sky_map.c
--rw-rw-rw-   0 root         (0) root         (0)     7831 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/bayestar_sky_map.h
--rw-rw-rw-   0 root         (0) root         (0)      218 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/branch_prediction.h
--rw-rw-rw-   0 root         (0) root         (0)    41209 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/core.c
--rw-rw-rw-   0 root         (0) root         (0)     5818 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/cubic_interp.c
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/cubic_interp.h
--rw-rw-rw-   0 root         (0) root         (0)    13016 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/cubic_interp_test.c
--rw-rw-rw-   0 root         (0) root         (0)     6370 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/omp_interruptible.h
--rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/vmath.h
--rw-rw-rw-   0 root         (0) root         (0)     1869 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/src/warnings.h
--rw-rw-rw-   0 root         (0) root         (0)     2696 2024-05-24 14:10:41.000000 ligo_skymap-2.0.1rc1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.884104 ligo_skymap-2.0.1rc2/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.821102 ligo_skymap-2.0.1rc2/.gitlab/
+-rwxrwxrwx   0 root         (0) root         (0)     2033 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/.gitlab/combine-coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)    13658 2024-05-28 19:50:04.000000 ligo_skymap-2.0.1rc2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    44876 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5187 2024-05-29 05:09:17.884104 ligo_skymap-2.0.1rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.813102 ligo_skymap-2.0.1rc2/cextern/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.821102 ligo_skymap-2.0.1rc2/cextern/chealpix/
+-rw-rw-rw-   0 root         (0) root         (0)    30207 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/cextern/chealpix/chealpix.c
+-rw-rw-rw-   0 root         (0) root         (0)     7407 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/cextern/chealpix/chealpix.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.824102 ligo_skymap-2.0.1rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.826102 ligo_skymap-2.0.1rc2/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34751 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/_static/benchmark.svg
+-rw-rw-rw-   0 root         (0) root         (0)   567737 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/_static/coinc.xml
+-rw-rw-rw-   0 root         (0) root         (0)   260305 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/_static/localization.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.814102 ligo_skymap-2.0.1rc2/docs/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.827102 ligo_skymap-2.0.1rc2/docs/_templates/autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/_templates/autosummary/base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0 root         (0) root         (0)      252 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.828102 ligo_skymap-2.0.1rc2/docs/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    56171 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/bayestar/eggbox.png
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/bayestar/ez_emcee.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/bayestar/filter.rst
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/bayestar/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/bayestar/interpolation.rst
+-rw-rw-rw-   0 root         (0) root         (0)    44876 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.829102 ligo_skymap-2.0.1rc2/docs/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/coordinates/detector.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/coordinates/eigenframe.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/develop.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.829102 ligo_skymap-2.0.1rc2/docs/distance/
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/distance/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.829102 ligo_skymap-2.0.1rc2/docs/healpix_tree/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/healpix_tree/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/help.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4582 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15650 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/interface.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.830102 ligo_skymap-2.0.1rc2/docs/io/
+-rw-rw-rw-   0 root         (0) root         (0)     3691 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/io/events.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/io/fits.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/io/hdf5.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.830102 ligo_skymap-2.0.1rc2/docs/kde/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/kde/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/matplotlibrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.831102 ligo_skymap-2.0.1rc2/docs/moc/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/moc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/performance.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.832102 ligo_skymap-2.0.1rc2/docs/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/plot/allsky.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/plot/backdrop.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/plot/bayes_factor.rst
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/plot/marker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/plot/poly.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/plot/pp.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.833102 ligo_skymap-2.0.1rc2/docs/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/postprocess/contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/postprocess/cosmology.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/postprocess/crossmatch.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/postprocess/ellipse.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/postprocess/util.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.834102 ligo_skymap-2.0.1rc2/docs/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/quickstart/bayestar-injections.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4452 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/quickstart/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6031 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/testing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.839102 ligo_skymap-2.0.1rc2/docs/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/bayestar_inject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/bayestar_localize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/bayestar_localize_lvalert.rst
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/bayestar_mcmc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/bayestar_realize_coincs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/bayestar_sample_model_psd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_combine.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_constellations.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_contour.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_contour_moc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_flatten.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_from_samples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_airmass.rst
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_coherence.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_observability.rst
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_volume.rst
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_stats.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_unflatten.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.841102 ligo_skymap-2.0.1rc2/docs/util/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/util/file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/util/ilwd.rst
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/util/numpy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/docs/util/sqlite.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.842103 ligo_skymap-2.0.1rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/licenses/CHEALPIX_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)    37565 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/licenses/NUMPY_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.815102 ligo_skymap-2.0.1rc2/ligo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.845103 ligo_skymap-2.0.1rc2/ligo/skymap/
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/_astropy_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.847103 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/
+-rw-rw-rw-   0 root         (0) root         (0)    20357 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/ez_emcee.py
+-rw-rw-rw-   0 root         (0) root         (0)    19685 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10348 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/ptemcee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.847103 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4573 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/test_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4287 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.848103 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3645 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/detector.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/eigenframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.849103 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/tests/test_detector.py
+-rw-rw-rw-   0 root         (0) root         (0)    21354 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/distance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.849103 ligo_skymap-2.0.1rc2/ligo/skymap/extern/
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/extern/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.849103 ligo_skymap-2.0.1rc2/ligo/skymap/extern/numpy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/extern/numpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13938 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/extern/numpy/quantile.py
+-rw-rw-rw-   0 root         (0) root         (0)    15264 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/healpix_tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.850103 ligo_skymap-2.0.1rc2/ligo/skymap/io/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.852103 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/detector_disabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/gracedb.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/hdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    11536 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/ligolw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/magic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/events/sqlite.py
+-rwxrwxrwx   0 root         (0) root         (0)    19227 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/fits.py
+-rwxrwxrwx   0 root         (0) root         (0)    10626 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.852103 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.854103 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)   492938 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/2016_subset.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G197392_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G197392_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G211117_coinc.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G211117_psd.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.855103 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/gstlal_reference_psd/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/gstlal_reference_psd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9120 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/test.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    13030 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/test_io_events.py
+-rw-rw-rw-   0 root         (0) root         (0)    17043 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/kde.py
+-rw-rw-rw-   0 root         (0) root         (0)     7376 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.858103 ligo_skymap-2.0.1rc2/ligo/skymap/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29444 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/allsky.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/angle.py
+-rw-rw-rw-   0 root         (0) root         (0)     7312 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/backdrop.py
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/bayes_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/cmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8720 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/cylon.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/cylon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/marker.py
+-rw-rw-rw-   0 root         (0) root         (0)    63275 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/ne_simplified_coastline.json
+-rw-rw-rw-   0 root         (0) root         (0)     7394 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/poly.py
+-rw-rw-rw-   0 root         (0) root         (0)     9445 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.858103 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.865103 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/
+-rw-rw-rw-   0 root         (0) root         (0)    67688 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    66215 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    65823 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    64266 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    71787 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    71744 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    70520 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    69570 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    65034 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    63912 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    63615 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    61805 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    34054 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png
+-rw-rw-rw-   0 root         (0) root         (0)    26036 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    25898 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    24279 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png
+-rw-rw-rw-   0 root         (0) root         (0)    22175 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png
+-rw-rw-rw-   0 root         (0) root         (0)    20330 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_globe_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)    15198 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_plot_bayes_factor.png
+-rw-rw-rw-   0 root         (0) root         (0)    19023 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    39922 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    19023 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png
+-rw-rw-rw-   0 root         (0) root         (0)     8797 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_reticle.png
+-rw-rw-rw-   0 root         (0) root         (0)    19883 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_zoom_axes.png
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.867103 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6348 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2903 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    18290 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)    15257 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/ellipse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.867103 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/tests/test_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/tests/test_crossmatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.868103 ligo_skymap-2.0.1rc2/ligo/skymap/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.868103 ligo_skymap-2.0.1rc2/ligo/skymap/tests/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tests/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tests/plugins/omp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5704 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tests/test_moc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.874104 ligo_skymap-2.0.1rc2/ligo/skymap/tool/
+-rw-rw-rw-   0 root         (0) root         (0)    16330 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22383 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     7739 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_localize_coincs.py
+-rwxrwxrwx   0 root         (0) root         (0)     7120 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_localize_lvalert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8653 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_mcmc.py
+-rw-rw-rw-   0 root         (0) root         (0)    19766 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_realize_coincs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4754 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_sample_model_psd.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     2099 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_constellations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_contour_moc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     8090 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7143 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     8353 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_airmass.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_coherence.py
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_observability.py
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)     8666 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)    10148 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_volume.py
+-rw-rw-rw-   0 root         (0) root         (0)    11959 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-29 02:54:19.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_unflatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.876103 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_bayestar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_bayestar_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_combine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_from_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_plot_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.878104 ligo_skymap-2.0.1rc2/ligo/skymap/util/
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5170 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/ilwd.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4451 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/stopwatch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.878104 ligo_skymap-2.0.1rc2/ligo/skymap/util/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 05:09:07.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/ligo/skymap/util/tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo/skymap/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.882104 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5187 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8711 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1550 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-29 05:09:17.000000 ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6477 2024-05-29 05:09:17.885104 ligo_skymap-2.0.1rc2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3807 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:09:17.882104 ligo_skymap-2.0.1rc2/src/
+-rw-rw-rw-   0 root         (0) root         (0)    37062 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_cosmology.h
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_cosmology.py
+-rw-rw-rw-   0 root         (0) root         (0)    16209 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_distance.c
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_distance.h
+-rw-rw-rw-   0 root         (0) root         (0)     4231 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_moc.c
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_moc.h
+-rw-rw-rw-   0 root         (0) root         (0)    50371 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_sky_map.c
+-rw-rw-rw-   0 root         (0) root         (0)     7831 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/bayestar_sky_map.h
+-rw-rw-rw-   0 root         (0) root         (0)      218 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/branch_prediction.h
+-rw-rw-rw-   0 root         (0) root         (0)    41209 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/core.c
+-rw-rw-rw-   0 root         (0) root         (0)     5818 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/cubic_interp.c
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/cubic_interp.h
+-rw-rw-rw-   0 root         (0) root         (0)    13016 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/cubic_interp_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     6370 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/omp_interruptible.h
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/vmath.h
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/src/warnings.h
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2024-05-28 19:20:21.000000 ligo_skymap-2.0.1rc2/tox.ini
```

### Comparing `ligo_skymap-2.0.1rc1/.gitignore` & `ligo_skymap-2.0.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/.gitlab/combine-coverage.py` & `ligo_skymap-2.0.1rc2/.gitlab/combine-coverage.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/.gitlab-ci.yml` & `ligo_skymap-2.0.1rc2/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,16 @@
   script:
     - . /opt/local/share/macports/setupenv.bash
     - PYVERS=3.10
     # Enter virtualenv so that we have a controlled version of Numpy
     - python${PYVERS} -m venv env
     - source env/bin/activate
     - pip install $(echo ${CI_PROJECT_DIR}/*.whl)[test]
+    # FIXME: remove when https://git.ligo.org/computing/helpdesk/-/issues/5983 is fixed
+    - pip install 'healpy<1.17'
     - python -c 'import sys; from ligo.skymap import test; sys.exit(test(args="--doctest-plus --doctest-ufunc --mpl --mpl-results-path '${CI_PROJECT_DIR}'/pytest-mpl-results --mpl-generate-summary=html --omp-get-num-threads --durations=10"))'
   artifacts:
     paths:
       - pytest-mpl-results/
     when: always
 
 test/macos/x86_64:
```

### Comparing `ligo_skymap-2.0.1rc1/CHANGES.rst` & `ligo_skymap-2.0.1rc2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #########
 Changelog
 #########
 
-2.0.1rc1 (2024-04-24)
+2.0.1rc2 (2024-05-29)
 =====================
 
 - Drop support for Python 3.9 because Astropy 6.1.0 dropped Python 3.9 in
   accordance with the Numpy version support policy.
 
 - Require astropy >= 6.0.0.
 
@@ -17,14 +17,18 @@
 
 - Ensure that ``ligo.skymap.distance.conditional_cdf`` and
   ``ligo.skymap.distance.marginal_cdf`` correctly handle corner cases for
   extreme values: both now return 0 for distances that are less than or equal
   to 0, and 1 for a distance of positive infinity (assuming that the
   ``distnorm`` argument does indeed normalize the distribution).
 
+- Ensure that all ligo.skymap command-line tools close any files that they have
+  opened. These command-line tools are used as functions in GWCelery, and were
+  leaking unclosed file descriptors.
+
 2.0.0 (2024-04-15)
 ==================
 
 - Added options to center ``mollweide`` and ``aitoff`` projections. Thanks go
   to Sam Wyatt for this contribution.
 
 - Added support for ``os.PathLike`` filenames when reading ligolw files. Thanks
```

### Comparing `ligo_skymap-2.0.1rc1/CONTRIBUTING.rst` & `ligo_skymap-2.0.1rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/PKG-INFO` & `ligo_skymap-2.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 2.0.1rc1
+Version: 2.0.1rc2
 Summary: Tools for reading, writing, manipulating, and making LIGO/Virgo/KAGRA sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
```

### Comparing `ligo_skymap-2.0.1rc1/README.rst` & `ligo_skymap-2.0.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/cextern/chealpix/chealpix.c` & `ligo_skymap-2.0.1rc2/cextern/chealpix/chealpix.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/cextern/chealpix/chealpix.h` & `ligo_skymap-2.0.1rc2/cextern/chealpix/chealpix.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/Makefile` & `ligo_skymap-2.0.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/_static/benchmark.svg` & `ligo_skymap-2.0.1rc2/docs/_static/benchmark.svg`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/_static/coinc.xml` & `ligo_skymap-2.0.1rc2/docs/_static/coinc.xml`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/_static/localization.svg` & `ligo_skymap-2.0.1rc2/docs/_static/localization.svg`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/bayestar/eggbox.png` & `ligo_skymap-2.0.1rc2/docs/bayestar/eggbox.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/changes.rst` & `ligo_skymap-2.0.1rc2/docs/changes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #########
 Changelog
 #########
 
-2.0.1rc1 (2024-04-24)
+2.0.1rc2 (2024-05-29)
 =====================
 
 - Drop support for Python 3.9 because Astropy 6.1.0 dropped Python 3.9 in
   accordance with the Numpy version support policy.
 
 - Require astropy >= 6.0.0.
 
@@ -17,14 +17,18 @@
 
 - Ensure that ``ligo.skymap.distance.conditional_cdf`` and
   ``ligo.skymap.distance.marginal_cdf`` correctly handle corner cases for
   extreme values: both now return 0 for distances that are less than or equal
   to 0, and 1 for a distance of positive infinity (assuming that the
   ``distnorm`` argument does indeed normalize the distribution).
 
+- Ensure that all ligo.skymap command-line tools close any files that they have
+  opened. These command-line tools are used as functions in GWCelery, and were
+  leaking unclosed file descriptors.
+
 2.0.0 (2024-04-15)
 ==================
 
 - Added options to center ``mollweide`` and ``aitoff`` projections. Thanks go
   to Sam Wyatt for this contribution.
 
 - Added support for ``os.PathLike`` filenames when reading ligolw files. Thanks
```

### Comparing `ligo_skymap-2.0.1rc1/docs/conf.py` & `ligo_skymap-2.0.1rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/contributing.rst` & `ligo_skymap-2.0.1rc2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/develop.rst` & `ligo_skymap-2.0.1rc2/docs/develop.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/distance/index.rst` & `ligo_skymap-2.0.1rc2/docs/distance/index.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/help.rst` & `ligo_skymap-2.0.1rc2/docs/help.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/index.rst` & `ligo_skymap-2.0.1rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/interface.rst` & `ligo_skymap-2.0.1rc2/docs/interface.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/io/events.rst` & `ligo_skymap-2.0.1rc2/docs/io/events.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/make.bat` & `ligo_skymap-2.0.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/performance.rst` & `ligo_skymap-2.0.1rc2/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/quickstart/bayestar-injections.rst` & `ligo_skymap-2.0.1rc2/docs/quickstart/bayestar-injections.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/quickstart/install.rst` & `ligo_skymap-2.0.1rc2/docs/quickstart/install.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/testing.rst` & `ligo_skymap-2.0.1rc2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_combine.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_combine.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_constellations.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_constellations.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_from_samples.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_from_samples.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_airmass.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_airmass.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_coherence.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_coherence.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_observability.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_observability.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/docs/tool/ligo_skymap_plot_volume.rst` & `ligo_skymap-2.0.1rc2/docs/tool/ligo_skymap_plot_volume.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/licenses/CHEALPIX_LICENSE.rst` & `ligo_skymap-2.0.1rc2/licenses/CHEALPIX_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/licenses/LICENSE.rst` & `ligo_skymap-2.0.1rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/licenses/NUMPY_LICENSE.rst` & `ligo_skymap-2.0.1rc2/licenses/NUMPY_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/licenses/TEMPLATE_LICENCE.rst` & `ligo_skymap-2.0.1rc2/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/__init__.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/_astropy_init.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/__init__.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/ez_emcee.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/ez_emcee.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/filter.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/filter.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/interpolation.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/ptemcee.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/ptemcee.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/test_bayestar.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/test_interpolation.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/bayestar/tests/test_signal_amplitude_model.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/conftest.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,18 +44,19 @@
 # To ignore some specific deprecation warning messages for Python version
 # MAJOR.MINOR or later, add:
 #     warnings_to_ignore_by_pyver={(MAJOR, MINOR): ['Message to ignore']}
 # from astropy.tests.helper import enable_deprecations_as_exceptions  # noqa
 # enable_deprecations_as_exceptions()
 
 
-@pytest.fixture(autouse=True)
-def ignore_unclosed_file_warnings():
-    """Ignore unclosed file warnings.
+@pytest.fixture(autouse=True, scope='session')
+def treat_unclosed_files_as_errors():
+    """Treat warnings abnout unclosed files as errors
 
     Many of the command-line tools in :mod:`ligo.skymap.tool` use
-    :class:`arparse.FileType` and therefore leave files opened. Suppress
-    warnings about unclosed files so that other more interesting warning types
-    are more noticable.
+    :class:`arparse.FileType` and therefore might leave files opened. Treat
+    this as an error.
 
     """
-    warnings.filterwarnings('ignore', 'unclosed file .*', ResourceWarning)
+    warnings.filterwarnings('error', 'unclosed file .*', ResourceWarning)
+    warnings.filterwarnings(
+        'error', category=pytest.PytestUnraisableExceptionWarning)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/detector.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/detector.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/eigenframe.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/eigenframe.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/coordinates/tests/test_detector.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/coordinates/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/distance.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/distance.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/extern/numpy/quantile.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/extern/numpy/quantile.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/healpix_tree.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/healpix_tree.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/base.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/base.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/detector_disabled.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/detector_disabled.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/gracedb.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/gracedb.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/hdf.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/hdf.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/ligolw.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/ligolw.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/magic.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/magic.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/events/sqlite.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/events/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/fits.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/fits.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/hdf5.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/2016_subset.xml.gz` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/2016_subset.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G197392_coinc.xml.gz` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G197392_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G197392_psd.xml.gz` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G197392_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G211117_coinc.xml.gz` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G211117_coinc.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/G211117_psd.xml.gz` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/G211117_psd.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/gstlal_reference_psd/H1L1V1-REFERENCE_PSD-967234210-29963.xml.gz`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/data/test.hdf5` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/io/tests/test_io_events.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/io/tests/test_io_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+from contextlib import ExitStack
 import errno
 import gzip
 import os
 from pathlib import Path
 import re
 import subprocess
-from unittest.mock import patch
 
 from ligo.lw.utils import load_filename
 import h5py
 import numpy as np
 import pytest
 
 from .. import events
 from ..events.ligolw import ContentHandler
 from ...util import sqlite
 
 DATA_PATH = os.path.join(os.path.dirname(__file__), 'data')
 
 
-class MockGraceDb:
-    """Mock GraceDB client class that reads local data files."""
-
-    def files(self, graceid, filename):
-        path = os.path.join(DATA_PATH, '{}_{}'.format(graceid, filename))
-        try:
-            return open(path, 'rb')
-        except IOError as e:
-            if e.errno != errno.ENOENT:
-                raise
-            return gzip.GzipFile(path + '.gz', 'rb')
+@pytest.fixture
+def mock_gracedb(monkeypatch):
+    stack = ExitStack()
+
+    class MockGraceDb(ExitStack):
+
+        def files(self, graceid, filename):
+            path = os.path.join(DATA_PATH, '{}_{}'.format(graceid, filename))
+            try:
+                return stack.enter_context(open(path, 'rb'))
+            except IOError as e:
+                if e.errno != errno.ENOENT:
+                    raise
+                return stack.enter_context(gzip.GzipFile(path + '.gz', 'rb'))
+
+    with stack:
+        monkeypatch.setattr('ligo.gracedb.rest.GraceDb', MockGraceDb)
+        yield
 
 
 def raises(expected_exception, msg):
     return pytest.raises(expected_exception, match='^' + re.escape(msg) + '$')
 
 
 def ligolw_assertions(source):
@@ -126,16 +133,15 @@
         ligolw_assertions(source)
 
     with sqlite.open(dbfilename, 'r') as db:
         source = events.open(db)
         ligolw_assertions(source)
 
 
-@patch('ligo.gracedb.rest.GraceDb', MockGraceDb)
-def test_gracedb():
+def test_gracedb(mock_gracedb):
     """Test reading events from GraceDB records."""
     source = events.gracedb.open(['G211117', 'G197392'])
     assert len(source) == 2
     for i, (event_id, event) in enumerate(source.items()):
         if i == 0:
             assert event_id == 'G211117'
             assert (event.singles[0].snr_series is event.singles[1].snr_series
@@ -194,16 +200,15 @@
                 'spin1z': 0.34881824,
                 'spin2x': 0.0,
                 'spin2y': 0.0,
                 'spin2z': -0.53029484,
                 'f_final': 0.0}
 
 
-@patch('ligo.gracedb.rest.GraceDb', MockGraceDb)
-def test_detector_disabled():
+def test_detector_disabled(mock_gracedb):
     """Test reading from event sources with certain detectors disabled."""
     graceids = ('G211117', 'G197392')
     base_source = events.gracedb.open(graceids)
 
     source = events.detector_disabled.open(base_source, ['H1'])
     assert len(source) == 2
     for graceid, (event_id, event) in zip(graceids, source.items()):
@@ -322,8 +327,11 @@
             assert np.all(single.psd.data.data == np.arange(5)**2)
         assert coinc.template_args == {}
 
     # Test reading from h5py.File instances
     events.open(*(h5py.File(filename, 'r') for filename in filenames))
 
     # Test reading from file-like objects
-    events.open(*(open(filename, 'rb') for filename in filenames))
+    with ExitStack() as stack:
+        events.open(*(
+            stack.enter_context(open(filename, 'rb'))
+            for filename in filenames))
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/kde.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/kde.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/moc.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/moc.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/allsky.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/allsky.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/angle.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/angle.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/backdrop.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/backdrop.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/bayes_factor.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/bayes_factor.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/cmap.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/cmap.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/cylon.csv` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/cylon.csv`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/cylon.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/cylon.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/marker.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/marker.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/ne_simplified_coastline.json` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/ne_simplified_coastline.json`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/poly.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/poly.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/pp.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/pp.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_astro-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_galactic-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-degrees-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_axes_geo-hours-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_allsky_obstime.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_197.45d -23.38d-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_None-aitoff.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_center_projections_None-mollweide.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_globe_axes.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_globe_axes.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_plot_bayes_factor.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_plot_bayes_factor.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_pp_plot_default.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_pp_plot_lines.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_pp_plot_steps.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_reticle.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_reticle.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/baseline/test_zoom_axes.png` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/baseline/test_zoom_axes.png`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/tests/test_plot.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/plot/util.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/plot/util.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/contour.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/contour.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/cosmology.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/crossmatch.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/ellipse.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/ellipse.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/tests/test_cosmology.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/tests/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/tests/test_crossmatch.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/tests/test_crossmatch.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/postprocess/util.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/postprocess/util.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tests/plugins/omp.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tests/plugins/omp.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tests/test_moc.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tests/test_moc.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/__init__.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,43 @@
 
 from ..util import sqlite
 from .. import version
 
 version_string = version.__package__ + ' ' + version.version
 
 
+def _try_close(obj):
+    try:
+        obj.close()
+    except AttributeError:
+        pass
+
+
+class Namespace(argparse.Namespace):
+    """A Namespace that can be used in a context to close all open files."""
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        for value in vars(self).values():
+            if isinstance(value, list):
+                for item in value:
+                    _try_close(item)
+            _try_close(value)
+
+
 class FileType(argparse.FileType):
     """Inherit from :class:`argparse.FileType` to enable opening stdin or
     stdout in binary mode.
 
-    This is a workaround for https://bugs.python.org/issue14156.
+    This is a workaround for https://bugs.python.org/issue14156, which is fixed
+    in Python 3.9.12, 3.10.3, and >=3.11.0.
+
+    FIXME: Remove this when we drop support for Python 3.10.
     """
 
     def __call__(self, string):
         if string == '-' and 'b' in self._mode:
             if 'r' in self._mode:
                 return sys.stdin.buffer
             elif 'w' in self._mode:
@@ -258,14 +282,17 @@
     - The description is taken from the docstring of the file in which the
       ArgumentParser is created.
 
     - If the description is taken from the docstring, then whitespace in
       the description is preserved.
 
     - A ``--version`` option is added that prints the version of ligo.skymap.
+
+    - The Namespace object returned by ``parser.parse_args()`` can be used as a
+      context manager, in a ``with::`` statement, to close all opened files.
     """
 
     def __init__(self,
                  prog=None,
                  usage=None,
                  description=None,
                  epilog=None,
@@ -297,14 +324,19 @@
         self.register('action', 'glob', GlobAction)
         self.register('action', 'loglevel', LogLevelAction)
         self.add_argument(
             '--version', action='version', version=version_string)
         self.add_argument(
             '-l', '--loglevel', action='loglevel', default='INFO')
 
+    def parse_known_args(self, args=None, namespace=None):
+        if namespace is None:
+            namespace = Namespace()
+        return super().parse_known_args(args, namespace)
+
 
 class DirType:
     """Factory for directory arguments."""
 
     def __init__(self, create=False):
         self._create = create
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_inject.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_inject.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,275 +275,281 @@
     parser.add_argument(
         '-j', '--jobs', type=int, default=1, const=None, nargs='?',
         help='Number of threads')
     return parser
 
 
 def main(args=None):
-    import warnings
-
-    from astropy.table import Table
-    from ligo.lw import lsctables
-    from ligo.lw import utils as ligolw_utils
-    from ligo.lw import ligolw
-    import lal.series
-    from scipy import stats
-
     p = parser()
-    args = p.parse_args(args)
+    with p.parse_args(args) as args:
+        import warnings
 
-    if args.min_snr is not None:
-        warnings.warn(
-            'The --min-snr threshold option is deprecated. '
-            'Please use the synonymous --snr-threshold option instead.',
-            UserWarning)
-        args.snr_threshold = args.min_snr
-
-    xmldoc = ligolw.Document()
-    xmlroot = xmldoc.appendChild(ligolw.LIGO_LW())
-    process = register_to_xmldoc(xmldoc, p, args)
-
-    # Read PSDs
-    psds = list(
-        lal.series.read_psd_xmldoc(
-            ligolw_utils.load_fileobj(
-                args.reference_psd,
-                contenthandler=lal.series.PSDContentHandler)).values())
-
-    if len(psds) < args.min_triggers:
-        parser.error(
-            f'The number of PSDs ({len(psds)}) must be greater than or equal '
-            f'to the value of --min-triggers ({args.min_triggers}).')
-
-    gwcosmo = GWCosmo(getattr(cosmology, args.cosmology))
-
-    if args.distribution:
-        ns_mass_min = 1.0
-        ns_mass_max = 2.0
-        bh_mass_min = 5.0
-        bh_mass_max = 50.0
-
-        ns_astro_spin_min = -0.05
-        ns_astro_spin_max = +0.05
-        ns_astro_mass_dist = stats.norm(1.33, 0.09)
-        ns_astro_spin_dist = stats.uniform(
-            ns_astro_spin_min, ns_astro_spin_max - ns_astro_spin_min)
-
-        ns_broad_spin_min = -0.4
-        ns_broad_spin_max = +0.4
-        ns_broad_mass_dist = stats.uniform(
-            ns_mass_min, ns_mass_max - ns_mass_min)
-        ns_broad_spin_dist = stats.uniform(
-            ns_broad_spin_min, ns_broad_spin_max - ns_broad_spin_min)
-
-        bh_astro_spin_min = -0.99
-        bh_astro_spin_max = +0.99
-        bh_astro_mass_dist = stats.pareto(b=1.3)
-        bh_astro_spin_dist = stats.uniform(
-            bh_astro_spin_min, bh_astro_spin_max - bh_astro_spin_min)
-
-        bh_broad_spin_min = -0.99
-        bh_broad_spin_max = +0.99
-        bh_broad_mass_dist = stats.reciprocal(bh_mass_min, bh_mass_max)
-        bh_broad_spin_dist = stats.uniform(
-            bh_broad_spin_min, bh_broad_spin_max - bh_broad_spin_min)
-
-        if args.distribution.startswith('bns_'):
-            m1_min = m2_min = ns_mass_min
-            m1_max = m2_max = ns_mass_max
-            if args.distribution.endswith('_astro'):
-                x1_min = x2_min = ns_astro_spin_min
-                x1_max = x2_max = ns_astro_spin_max
-                m1_dist = m2_dist = ns_astro_mass_dist
-                x1_dist = x2_dist = ns_astro_spin_dist
-            elif args.distribution.endswith('_broad'):
-                x1_min = x2_min = ns_broad_spin_min
-                x1_max = x2_max = ns_broad_spin_max
-                m1_dist = m2_dist = ns_broad_mass_dist
-                x1_dist = x2_dist = ns_broad_spin_dist
-            else:  # pragma: no cover
-                assert_not_reached()
-        elif args.distribution.startswith('nsbh_'):
-            m1_min = bh_mass_min
-            m1_max = bh_mass_max
-            m2_min = ns_mass_min
-            m2_max = ns_mass_max
-            if args.distribution.endswith('_astro'):
-                x1_min = bh_astro_spin_min
-                x1_max = bh_astro_spin_max
-                x2_min = ns_astro_spin_min
-                x2_max = ns_astro_spin_max
-                m1_dist = bh_astro_mass_dist
-                m2_dist = ns_astro_mass_dist
-                x1_dist = bh_astro_spin_dist
-                x2_dist = ns_astro_spin_dist
-            elif args.distribution.endswith('_broad'):
-                x1_min = bh_broad_spin_min
-                x1_max = bh_broad_spin_max
-                x2_min = ns_broad_spin_min
-                x2_max = ns_broad_spin_max
-                m1_dist = bh_broad_mass_dist
-                m2_dist = ns_broad_mass_dist
-                x1_dist = bh_broad_spin_dist
-                x2_dist = ns_broad_spin_dist
+        from astropy.table import Table
+        from ligo.lw import lsctables
+        from ligo.lw import utils as ligolw_utils
+        from ligo.lw import ligolw
+        import lal.series
+        from scipy import stats
+
+        if args.min_snr is not None:
+            warnings.warn(
+                'The --min-snr threshold option is deprecated. '
+                'Please use the synonymous --snr-threshold option instead.',
+                UserWarning)
+            args.snr_threshold = args.min_snr
+
+        xmldoc = ligolw.Document()
+        xmlroot = xmldoc.appendChild(ligolw.LIGO_LW())
+        process = register_to_xmldoc(xmldoc, p, args)
+
+        # Read PSDs
+        psds = list(
+            lal.series.read_psd_xmldoc(
+                ligolw_utils.load_fileobj(
+                    args.reference_psd,
+                    contenthandler=lal.series.PSDContentHandler)).values())
+
+        if len(psds) < args.min_triggers:
+            parser.error(
+                f'The number of PSDs ({len(psds)}) must be greater than or '
+                f'equal to the value of --min-triggers ({args.min_triggers}).')
+
+        gwcosmo = GWCosmo(getattr(cosmology, args.cosmology))
+
+        if args.distribution:
+            ns_mass_min = 1.0
+            ns_mass_max = 2.0
+            bh_mass_min = 5.0
+            bh_mass_max = 50.0
+
+            ns_astro_spin_min = -0.05
+            ns_astro_spin_max = +0.05
+            ns_astro_mass_dist = stats.norm(1.33, 0.09)
+            ns_astro_spin_dist = stats.uniform(
+                ns_astro_spin_min, ns_astro_spin_max - ns_astro_spin_min)
+
+            ns_broad_spin_min = -0.4
+            ns_broad_spin_max = +0.4
+            ns_broad_mass_dist = stats.uniform(
+                ns_mass_min, ns_mass_max - ns_mass_min)
+            ns_broad_spin_dist = stats.uniform(
+                ns_broad_spin_min, ns_broad_spin_max - ns_broad_spin_min)
+
+            bh_astro_spin_min = -0.99
+            bh_astro_spin_max = +0.99
+            bh_astro_mass_dist = stats.pareto(b=1.3)
+            bh_astro_spin_dist = stats.uniform(
+                bh_astro_spin_min, bh_astro_spin_max - bh_astro_spin_min)
+
+            bh_broad_spin_min = -0.99
+            bh_broad_spin_max = +0.99
+            bh_broad_mass_dist = stats.reciprocal(bh_mass_min, bh_mass_max)
+            bh_broad_spin_dist = stats.uniform(
+                bh_broad_spin_min, bh_broad_spin_max - bh_broad_spin_min)
+
+            if args.distribution.startswith('bns_'):
+                m1_min = m2_min = ns_mass_min
+                m1_max = m2_max = ns_mass_max
+                if args.distribution.endswith('_astro'):
+                    x1_min = x2_min = ns_astro_spin_min
+                    x1_max = x2_max = ns_astro_spin_max
+                    m1_dist = m2_dist = ns_astro_mass_dist
+                    x1_dist = x2_dist = ns_astro_spin_dist
+                elif args.distribution.endswith('_broad'):
+                    x1_min = x2_min = ns_broad_spin_min
+                    x1_max = x2_max = ns_broad_spin_max
+                    m1_dist = m2_dist = ns_broad_mass_dist
+                    x1_dist = x2_dist = ns_broad_spin_dist
+                else:  # pragma: no cover
+                    assert_not_reached()
+            elif args.distribution.startswith('nsbh_'):
+                m1_min = bh_mass_min
+                m1_max = bh_mass_max
+                m2_min = ns_mass_min
+                m2_max = ns_mass_max
+                if args.distribution.endswith('_astro'):
+                    x1_min = bh_astro_spin_min
+                    x1_max = bh_astro_spin_max
+                    x2_min = ns_astro_spin_min
+                    x2_max = ns_astro_spin_max
+                    m1_dist = bh_astro_mass_dist
+                    m2_dist = ns_astro_mass_dist
+                    x1_dist = bh_astro_spin_dist
+                    x2_dist = ns_astro_spin_dist
+                elif args.distribution.endswith('_broad'):
+                    x1_min = bh_broad_spin_min
+                    x1_max = bh_broad_spin_max
+                    x2_min = ns_broad_spin_min
+                    x2_max = ns_broad_spin_max
+                    m1_dist = bh_broad_mass_dist
+                    m2_dist = ns_broad_mass_dist
+                    x1_dist = bh_broad_spin_dist
+                    x2_dist = ns_broad_spin_dist
+                else:  # pragma: no cover
+                    assert_not_reached()
+            elif args.distribution.startswith('bbh_'):
+                m1_min = m2_min = bh_mass_min
+                m1_max = m2_max = bh_mass_max
+                if args.distribution.endswith('_astro'):
+                    x1_min = x2_min = bh_astro_spin_min
+                    x1_max = x2_max = bh_astro_spin_max
+                    m1_dist = m2_dist = bh_astro_mass_dist
+                    x1_dist = x2_dist = bh_astro_spin_dist
+                elif args.distribution.endswith('_broad'):
+                    x1_min = x2_min = bh_broad_spin_min
+                    x1_max = x2_max = bh_broad_spin_max
+                    m1_dist = m2_dist = bh_broad_mass_dist
+                    x1_dist = x2_dist = bh_broad_spin_dist
+                else:  # pragma: no cover
+                    assert_not_reached()
             else:  # pragma: no cover
                 assert_not_reached()
-        elif args.distribution.startswith('bbh_'):
-            m1_min = m2_min = bh_mass_min
-            m1_max = m2_max = bh_mass_max
-            if args.distribution.endswith('_astro'):
-                x1_min = x2_min = bh_astro_spin_min
-                x1_max = x2_max = bh_astro_spin_max
-                m1_dist = m2_dist = bh_astro_mass_dist
-                x1_dist = x2_dist = bh_astro_spin_dist
-            elif args.distribution.endswith('_broad'):
-                x1_min = x2_min = bh_broad_spin_min
-                x1_max = x2_max = bh_broad_spin_max
-                m1_dist = m2_dist = bh_broad_mass_dist
-                x1_dist = x2_dist = bh_broad_spin_dist
-            else:  # pragma: no cover
-                assert_not_reached()
-        else:  # pragma: no cover
+
+            dists = (m1_dist, m2_dist, x1_dist, x2_dist)
+
+            # Construct mass1, mass2, spin1z, spin2z grid.
+            m1 = np.geomspace(m1_min, m1_max, 10)
+            m2 = np.geomspace(m2_min, m2_max, 10)
+            x1 = np.linspace(x1_min, x1_max, 10)
+            x2 = np.linspace(x2_min, x2_max, 10)
+            params = m1, m2, x1, x2
+
+            # Calculate the maximum distance on the grid.
+            max_z = gwcosmo.get_max_z(
+                psds, args.waveform, args.f_low,
+                args.snr_threshold, args.min_triggers,
+                *np.meshgrid(m1, m2, x1, x2, indexing='ij'), jobs=args.jobs)
+            if args.max_distance is not None:
+                new_max_z = cosmology.z_at_value(
+                    gwcosmo.cosmo.luminosity_distance,
+                    args.max_distance * units.Mpc)
+                max_z[max_z > new_max_z] = new_max_z
+            max_distance = gwcosmo.sensitive_distance(
+                max_z).to_value(units.Mpc)
+
+            # Find piecewise constant approximate upper bound on distance.
+            max_distance = cell_max(max_distance)
+
+            # Calculate V * T in each grid cell
+            cdfs = [dist.cdf(param) for param, dist in zip(params, dists)]
+            cdf_los = [cdf[:-1] for cdf in cdfs]
+            cdfs = [np.diff(cdf) for cdf in cdfs]
+            probs = np.prod(np.meshgrid(*cdfs, indexing='ij'), axis=0)
+            probs /= probs.sum()
+            probs *= 4/3*np.pi*max_distance**3
+            volume = probs.sum()
+            probs /= volume
+            probs = probs.ravel()
+
+            # Draw random grid cells
+            dist = stats.rv_discrete(values=(np.arange(len(probs)), probs))
+            indices = np.unravel_index(
+                dist.rvs(size=args.nsamples), max_distance.shape)
+
+            # Draw random intrinsic params from each cell
+            cols = {}
+            cols['mass1'], cols['mass2'], cols['spin1z'], cols['spin2z'] = [
+                dist.ppf(
+                    stats.uniform(cdf_lo[i], cdf[i]).rvs(size=args.nsamples))
+                for i, dist, cdf_lo, cdf in zip(indices, dists, cdf_los, cdfs)]
+        elif args.distribution_samples:
+            # Load distribution samples.
+            samples = Table.read(args.distribution_samples)
+
+            # Calculate the maximum sensitive distance for each sample.
+            max_z = gwcosmo.get_max_z(
+                psds, args.waveform, args.f_low,
+                args.snr_threshold, args.min_triggers,
+                samples['mass1'], samples['mass2'],
+                samples['spin1z'], samples['spin2z'], jobs=args.jobs)
+            if args.max_distance is not None:
+                new_max_z = cosmology.z_at_value(
+                    gwcosmo.cosmo.luminosity_distance,
+                    args.max_distance * units.Mpc)
+                max_z[max_z > new_max_z] = new_max_z
+            max_distance = gwcosmo.sensitive_distance(
+                max_z).to_value(units.Mpc)
+
+            # Calculate V * T for each sample.
+            probs = 1 / len(max_distance)
+            probs *= 4/3*np.pi*max_distance**3
+            volume = probs.sum()
+            probs /= volume
+
+            # Draw weighted samples for the simulated events.
+            dist = stats.rv_discrete(values=(np.arange(len(probs)), probs))
+            # Note that we do this in small batches because
+            # stats.rv_discrete.rvs has quadratic memory usage, number of
+            # values times number of samples, which might cause us to run out
+            # of memory if we did it all at once.
+            n_batches = max(args.nsamples * len(probs) // 1_000_000_000, 1)
+            batch_sizes = [len(subarray) for subarray in
+                           np.array_split(np.empty(args.nsamples), n_batches)]
+            indices = np.concatenate([dist.rvs(size=batch_size)
+                                      for batch_size in batch_sizes])
+
+            cols = {key: samples[key][indices]
+                    for key in ['mass1', 'mass2', 'spin1z', 'spin2z']}
+        else:
             assert_not_reached()
 
-        dists = (m1_dist, m2_dist, x1_dist, x2_dist)
+        volumetric_rate = (
+            args.nsamples / volume * units.year**-1 * units.Mpc**-3)
 
-        # Construct mass1, mass2, spin1z, spin2z grid.
-        m1 = np.geomspace(m1_min, m1_max, 10)
-        m2 = np.geomspace(m2_min, m2_max, 10)
-        x1 = np.linspace(x1_min, x1_max, 10)
-        x2 = np.linspace(x2_min, x2_max, 10)
-        params = m1, m2, x1, x2
-
-        # Calculate the maximum distance on the grid.
-        max_z = gwcosmo.get_max_z(
-            psds, args.waveform, args.f_low,
-            args.snr_threshold, args.min_triggers,
-            *np.meshgrid(m1, m2, x1, x2, indexing='ij'), jobs=args.jobs)
-        if args.max_distance is not None:
-            new_max_z = cosmology.z_at_value(gwcosmo.cosmo.luminosity_distance,
-                                             args.max_distance * units.Mpc)
-            max_z[max_z > new_max_z] = new_max_z
-        max_distance = gwcosmo.sensitive_distance(max_z).to_value(units.Mpc)
-
-        # Find piecewise constant approximate upper bound on distance.
-        max_distance = cell_max(max_distance)
-
-        # Calculate V * T in each grid cell
-        cdfs = [dist.cdf(param) for param, dist in zip(params, dists)]
-        cdf_los = [cdf[:-1] for cdf in cdfs]
-        cdfs = [np.diff(cdf) for cdf in cdfs]
-        probs = np.prod(np.meshgrid(*cdfs, indexing='ij'), axis=0)
-        probs /= probs.sum()
-        probs *= 4/3*np.pi*max_distance**3
-        volume = probs.sum()
-        probs /= volume
-        probs = probs.ravel()
-
-        # Draw random grid cells
-        dist = stats.rv_discrete(values=(np.arange(len(probs)), probs))
-        indices = np.unravel_index(
-            dist.rvs(size=args.nsamples), max_distance.shape)
-
-        # Draw random intrinsic params from each cell
-        cols = {}
-        cols['mass1'], cols['mass2'], cols['spin1z'], cols['spin2z'] = [
-            dist.ppf(stats.uniform(cdf_lo[i], cdf[i]).rvs(size=args.nsamples))
-            for i, dist, cdf_lo, cdf in zip(indices, dists, cdf_los, cdfs)]
-    elif args.distribution_samples:
-        # Load distribution samples.
-        samples = Table.read(args.distribution_samples)
-
-        # Calculate the maximum sensitive distance for each sample.
-        max_z = gwcosmo.get_max_z(
-            psds, args.waveform, args.f_low,
-            args.snr_threshold, args.min_triggers,
-            samples['mass1'], samples['mass2'],
-            samples['spin1z'], samples['spin2z'], jobs=args.jobs)
-        if args.max_distance is not None:
-            new_max_z = cosmology.z_at_value(gwcosmo.cosmo.luminosity_distance,
-                                             args.max_distance * units.Mpc)
-            max_z[max_z > new_max_z] = new_max_z
-        max_distance = gwcosmo.sensitive_distance(max_z).to_value(units.Mpc)
-
-        # Calculate V * T for each sample.
-        probs = 1 / len(max_distance)
-        probs *= 4/3*np.pi*max_distance**3
-        volume = probs.sum()
-        probs /= volume
-
-        # Draw weighted samples for the simulated events.
-        dist = stats.rv_discrete(values=(np.arange(len(probs)), probs))
-        # Note that we do this in small batches because stats.rv_discrete.rvs
-        # has quadratic memory usage, number of values times number of samples,
-        # which might cause us to run out of memory if we did it all at once.
-        n_batches = max(args.nsamples * len(probs) // 1_000_000_000, 1)
-        batch_sizes = [len(subarray) for subarray in
-                       np.array_split(np.empty(args.nsamples), n_batches)]
-        indices = np.concatenate([dist.rvs(size=batch_size)
-                                  for batch_size in batch_sizes])
-
-        cols = {key: samples[key][indices]
-                for key in ['mass1', 'mass2', 'spin1z', 'spin2z']}
-    else:
-        assert_not_reached()
-
-    volumetric_rate = args.nsamples / volume * units.year**-1 * units.Mpc**-3
-
-    # Swap binary components as needed to ensure that mass1 >= mass2.
-    # Note that the .copy() is important.
-    # See https://github.com/numpy/numpy/issues/14428
-    swap = cols['mass1'] < cols['mass2']
-    cols['mass1'][swap], cols['mass2'][swap] = \
-        cols['mass2'][swap].copy(), cols['mass1'][swap].copy()
-    cols['spin1z'][swap], cols['spin2z'][swap] = \
-        cols['spin2z'][swap].copy(), cols['spin1z'][swap].copy()
-
-    # Draw random extrinsic parameters
-    cols['distance'] = stats.powerlaw(a=3, scale=max_distance[indices]).rvs(
-        size=args.nsamples)
-    cols['longitude'] = stats.uniform(0, 2 * np.pi).rvs(
-        size=args.nsamples)
-    cols['latitude'] = np.arcsin(stats.uniform(-1, 2).rvs(
-        size=args.nsamples))
-    cols['inclination'] = np.arccos(stats.uniform(-1, 2).rvs(
-        size=args.nsamples))
-    cols['polarization'] = stats.uniform(0, 2 * np.pi).rvs(
-        size=args.nsamples)
-    cols['coa_phase'] = stats.uniform(-np.pi, 2 * np.pi).rvs(
-        size=args.nsamples)
-    cols['time_geocent'] = stats.uniform(1e9, units.year.to(units.second)).rvs(
-        size=args.nsamples)
-
-    # Convert from sensitive distance to redshift and comoving distance.
-    # FIXME: Replace this brute-force lookup table with a solver.
-    z = np.linspace(0, max_z.max(), 10000)
-    ds = gwcosmo.sensitive_distance(z).to_value(units.Mpc)
-    dc = gwcosmo.cosmo.comoving_distance(z).to_value(units.Mpc)
-    z_for_ds = interp1d(ds, z, kind='cubic', assume_sorted=True)
-    dc_for_ds = interp1d(ds, dc, kind='cubic', assume_sorted=True)
-    zp1 = 1 + z_for_ds(cols['distance'])
-    cols['distance'] = dc_for_ds(cols['distance'])
-
-    # Apply redshift factor to convert from comoving distance and source frame
-    # masses to luminosity distance and observer frame masses.
-    for key in ['distance', 'mass1', 'mass2']:
-        cols[key] *= zp1
-
-    # Populate sim_inspiral table
-    sims = xmlroot.appendChild(lsctables.New(lsctables.SimInspiralTable))
-    for row in zip(*cols.values()):
-        sims.appendRow(
-            **dict(
-                dict.fromkeys(sims.validcolumns, None),
-                process_id=process.process_id,
-                simulation_id=sims.get_next_id(),
-                waveform=args.waveform,
-                f_lower=args.f_low,
-                **dict(zip(cols.keys(), row))))
-
-    # Record process end time.
-    process.comment = str(volumetric_rate)
-    process.set_end_time_now()
+        # Swap binary components as needed to ensure that mass1 >= mass2.
+        # Note that the .copy() is important.
+        # See https://github.com/numpy/numpy/issues/14428
+        swap = cols['mass1'] < cols['mass2']
+        cols['mass1'][swap], cols['mass2'][swap] = \
+            cols['mass2'][swap].copy(), cols['mass1'][swap].copy()
+        cols['spin1z'][swap], cols['spin2z'][swap] = \
+            cols['spin2z'][swap].copy(), cols['spin1z'][swap].copy()
+
+        # Draw random extrinsic parameters
+        cols['distance'] = stats.powerlaw(
+            a=3, scale=max_distance[indices]).rvs(size=args.nsamples)
+        cols['longitude'] = stats.uniform(0, 2 * np.pi).rvs(
+            size=args.nsamples)
+        cols['latitude'] = np.arcsin(stats.uniform(-1, 2).rvs(
+            size=args.nsamples))
+        cols['inclination'] = np.arccos(stats.uniform(-1, 2).rvs(
+            size=args.nsamples))
+        cols['polarization'] = stats.uniform(0, 2 * np.pi).rvs(
+            size=args.nsamples)
+        cols['coa_phase'] = stats.uniform(-np.pi, 2 * np.pi).rvs(
+            size=args.nsamples)
+        cols['time_geocent'] = stats.uniform(
+            1e9, units.year.to(units.second)).rvs(size=args.nsamples)
+
+        # Convert from sensitive distance to redshift and comoving distance.
+        # FIXME: Replace this brute-force lookup table with a solver.
+        z = np.linspace(0, max_z.max(), 10000)
+        ds = gwcosmo.sensitive_distance(z).to_value(units.Mpc)
+        dc = gwcosmo.cosmo.comoving_distance(z).to_value(units.Mpc)
+        z_for_ds = interp1d(ds, z, kind='cubic', assume_sorted=True)
+        dc_for_ds = interp1d(ds, dc, kind='cubic', assume_sorted=True)
+        zp1 = 1 + z_for_ds(cols['distance'])
+        cols['distance'] = dc_for_ds(cols['distance'])
+
+        # Apply redshift factor to convert from comoving distance and source
+        # frame masses to luminosity distance and observer frame masses.
+        for key in ['distance', 'mass1', 'mass2']:
+            cols[key] *= zp1
+
+        # Populate sim_inspiral table
+        sims = xmlroot.appendChild(lsctables.New(lsctables.SimInspiralTable))
+        for row in zip(*cols.values()):
+            sims.appendRow(
+                **dict(
+                    dict.fromkeys(sims.validcolumns, None),
+                    process_id=process.process_id,
+                    simulation_id=sims.get_next_id(),
+                    waveform=args.waveform,
+                    f_lower=args.f_low,
+                    **dict(zip(cols.keys(), row))))
+
+        # Record process end time.
+        process.comment = str(volumetric_rate)
+        process.set_end_time_now()
 
-    # Write output file.
-    write_fileobj(xmldoc, args.output)
+        # Write output file.
+        write_fileobj(xmldoc, args.output)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_localize_coincs.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_localize_coincs.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,105 +78,109 @@
     parser.add_argument(
         '--condor-submit', action='store_true',
         help='submit to Condor instead of running locally')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
+    with parser().parse_args(args) as opts:
+        import logging
+        log = logging.getLogger('BAYESTAR')
+
+        # BAYESTAR imports.
+        from .. import omp
+        from ..io import fits, events
+        from ..bayestar import localize
+
+        # Other imports.
+        import os
+        import subprocess
+        import sys
+
+        log.info('Using %d OpenMP thread(s)', omp.num_threads)
+
+        # Read coinc file.
+        log.info(
+            '%s:reading input files', ','.join(
+                file.name for file in opts.input))
+        event_source = events.open(*opts.input, sample=opts.pycbc_sample)
+
+        if opts.disable_detector:
+            event_source = events.detector_disabled.open(
+                event_source, opts.disable_detector)
+
+        os.makedirs(opts.output, exist_ok=True)
+
+        if opts.condor_submit:
+            if opts.seed is not None:
+                raise NotImplementedError(
+                    '--seed does not yet work with --condor-submit')
+            if opts.coinc_event_id:
+                raise ValueError(
+                    'must not set --coinc-event-id with --condor-submit')
+            with subprocess.Popen(['condor_submit'],
+                                  text=True, stdin=subprocess.PIPE) as proc:
+                f = proc.stdin
+                print('''
+                    accounting_group = ligo.dev.o4.cbc.pe.bayestar
+                    on_exit_remove = (ExitBySignal == False) && (ExitCode == 0)
+                    on_exit_hold = (ExitBySignal == True) || (ExitCode != 0)
+                    on_exit_hold_reason = (ExitBySignal == True \
+                        ? strcat("The job exited with signal ", ExitSignal) \
+                        : strcat("The job exited with code ", ExitCode))
+                    request_memory = 2000 MB
+                    request_disk = 100 MB
+                    universe = vanilla
+                    getenv = true
+                    executable = /usr/bin/env
+                    JobBatchName = BAYESTAR
+                    environment = "OMP_NUM_THREADS=1"
+                    ''', file=f)
+                print(
+                    'error =', os.path.join(opts.output, '$(cid).err'), file=f)
+                print(
+                    'arguments = "',
+                    *(arg for arg in sys.argv if arg != '--condor-submit'),
+                    '--coinc-event-id $(cid)"', file=f)
+                print('queue cid in', *event_source, file=f)
+            sys.exit(proc.returncode)
 
-    import logging
-    log = logging.getLogger('BAYESTAR')
-
-    # BAYESTAR imports.
-    from .. import omp
-    from ..io import fits, events
-    from ..bayestar import localize
-
-    # Other imports.
-    import os
-    import subprocess
-    import sys
-
-    log.info('Using %d OpenMP thread(s)', omp.num_threads)
-
-    # Read coinc file.
-    log.info(
-        '%s:reading input files', ','.join(file.name for file in opts.input))
-    event_source = events.open(*opts.input, sample=opts.pycbc_sample)
-
-    if opts.disable_detector:
-        event_source = events.detector_disabled.open(
-            event_source, opts.disable_detector)
-
-    os.makedirs(opts.output, exist_ok=True)
-
-    if opts.condor_submit:
-        if opts.seed is not None:
-            raise NotImplementedError(
-                '--seed does not yet work with --condor-submit')
         if opts.coinc_event_id:
-            raise ValueError(
-                'must not set --coinc-event-id with --condor-submit')
-        with subprocess.Popen(['condor_submit'],
-                              text=True, stdin=subprocess.PIPE) as proc:
-            f = proc.stdin
-            print('''
-                  accounting_group = ligo.dev.o4.cbc.pe.bayestar
-                  on_exit_remove = (ExitBySignal == False) && (ExitCode == 0)
-                  on_exit_hold = (ExitBySignal == True) || (ExitCode != 0)
-                  on_exit_hold_reason = (ExitBySignal == True \
-                    ? strcat("The job exited with signal ", ExitSignal) \
-                    : strcat("The job exited with code ", ExitCode))
-                  request_memory = 2000 MB
-                  request_disk = 100 MB
-                  universe = vanilla
-                  getenv = true
-                  executable = /usr/bin/env
-                  JobBatchName = BAYESTAR
-                  environment = "OMP_NUM_THREADS=1"
-                  ''', file=f)
-            print('error =', os.path.join(opts.output, '$(cid).err'), file=f)
-            print('arguments = "',
-                  *(arg for arg in sys.argv if arg != '--condor-submit'),
-                  '--coinc-event-id $(cid)"', file=f)
-            print('queue cid in', *event_source, file=f)
-        sys.exit(proc.returncode)
-
-    if opts.coinc_event_id:
-        event_source = {key: event_source[key] for key in opts.coinc_event_id}
-
-    count_sky_maps_failed = 0
-
-    # Loop over all sngl_inspiral <-> sngl_inspiral coincs.
-    for coinc_event_id, event in event_source.items():
-        # Loop over sky localization methods
-        log.info('%d:computing sky map', coinc_event_id)
-        if opts.chain_dump:
-            chain_dump = f'{coinc_event_id}.hdf5'
-        else:
-            chain_dump = None
-        try:
-            sky_map = localize(
-                event, opts.waveform, opts.f_low, opts.min_distance,
-                opts.max_distance, opts.prior_distance_power,
-                opts.cosmology, mcmc=opts.mcmc, chain_dump=chain_dump,
-                enable_snr_series=opts.enable_snr_series,
-                f_high_truncate=opts.f_high_truncate,
-                rescale_loglikelihood=opts.rescale_loglikelihood)
-            sky_map.meta['objid'] = coinc_event_id
-            sky_map.meta['comment'] = ROW_ID_COMMENT
-
-        except (ArithmeticError, ValueError):
-            log.exception('%d:sky localization failed', coinc_event_id)
-            count_sky_maps_failed += 1
-            if not opts.keep_going:
-                raise
-        else:
-            log.info('%d:saving sky map', coinc_event_id)
-            filename = f'{coinc_event_id}.fits'
-            fits.write_sky_map(
-                os.path.join(opts.output, filename), sky_map, nest=True)
-
-    if count_sky_maps_failed > 0:
-        raise RuntimeError("{0} sky map{1} did not converge".format(
-            count_sky_maps_failed, 's' if count_sky_maps_failed > 1 else ''))
+            event_source = {
+                key: event_source[key] for key in opts.coinc_event_id}
+
+        count_sky_maps_failed = 0
+
+        # Loop over all sngl_inspiral <-> sngl_inspiral coincs.
+        for coinc_event_id, event in event_source.items():
+            # Loop over sky localization methods
+            log.info('%d:computing sky map', coinc_event_id)
+            if opts.chain_dump:
+                chain_dump = f'{coinc_event_id}.hdf5'
+            else:
+                chain_dump = None
+            try:
+                sky_map = localize(
+                    event, opts.waveform, opts.f_low, opts.min_distance,
+                    opts.max_distance, opts.prior_distance_power,
+                    opts.cosmology, mcmc=opts.mcmc, chain_dump=chain_dump,
+                    enable_snr_series=opts.enable_snr_series,
+                    f_high_truncate=opts.f_high_truncate,
+                    rescale_loglikelihood=opts.rescale_loglikelihood)
+                sky_map.meta['objid'] = coinc_event_id
+                sky_map.meta['comment'] = ROW_ID_COMMENT
+
+            except (ArithmeticError, ValueError):
+                log.exception('%d:sky localization failed', coinc_event_id)
+                count_sky_maps_failed += 1
+                if not opts.keep_going:
+                    raise
+            else:
+                log.info('%d:saving sky map', coinc_event_id)
+                filename = f'{coinc_event_id}.fits'
+                fits.write_sky_map(
+                    os.path.join(opts.output, filename), sky_map, nest=True)
+
+        if count_sky_maps_failed > 0:
+            raise RuntimeError("{0} sky map{1} did not converge".format(
+                count_sky_maps_failed,
+                's' if count_sky_maps_failed > 1 else ''))
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_localize_lvalert.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_localize_lvalert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -58,120 +58,122 @@
         'graceid', metavar='G123456', nargs='*',
         help='Run on these GraceDB IDs. If no GraceDB IDs are listed on the '
         'command line, then read newline-separated GraceDB IDs from stdin.')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
-
-    import logging
-    import os
-    import re
-    import sys
-    import tempfile
-    import urllib.parse
-    from ..bayestar import localize, rasterize
-    from ..io import fits
-    from ..io import events
-    from .. import omp
-    from ..util.file import rename
-    import ligo.gracedb.logging
-    import ligo.gracedb.rest
-
-    log = logging.getLogger('BAYESTAR')
-
-    log.info('Using %d OpenMP thread(s)', omp.num_threads)
-
-    # If no GraceDB IDs were specified on the command line, then read them
-    # from stdin line-by-line.
-    graceids = opts.graceid if opts.graceid else iterlines(sys.stdin)
-
-    # Fire up a GraceDb client
-    # FIXME: Mimic the behavior of the GraceDb command line client, where the
-    # environment variable GRACEDB_SERVICE_URL overrides the default service
-    # URL. It would be nice to get this behavior into the gracedb package
-    # itself.
-    gracedb = ligo.gracedb.rest.GraceDb(
-        os.environ.get(
-            'GRACEDB_SERVICE_URL', ligo.gracedb.rest.DEFAULT_SERVICE_URL))
-
-    # Determine the base URL for event pages.
-    scheme, netloc, *_ = urllib.parse.urlparse(gracedb._service_url)
-    base_url = urllib.parse.urlunparse((scheme, netloc, 'events', '', '', ''))
-
-    if opts.chain_dump:
-        chain_dump = re.sub(r'.fits(.gz)?$', r'.hdf5', opts.output)
-    else:
-        chain_dump = None
-
-    tags = ("sky_loc",)
-    if not opts.no_tag:
-        tags += ("lvem",)
-
-    event_source = events.gracedb.open(graceids, gracedb)
-
-    if opts.disable_detector:
-        event_source = events.detector_disabled.open(
-            event_source, opts.disable_detector)
-
-    for graceid in event_source.keys():
-
-        try:
-            event = event_source[graceid]
-        except:  # noqa: E722
-            log.exception('failed to read event %s from GraceDB', graceid)
-            continue
-
-        # Send log messages to GraceDb too
-        if not opts.dry_run:
-            handler = ligo.gracedb.logging.GraceDbLogHandler(gracedb, graceid)
-            handler.setLevel(logging.INFO)
-            logging.root.addHandler(handler)
-
-        # A little bit of Cylon humor
-        log.info('by your command...')
-
-        try:
-            # perform sky localization
-            log.info("starting sky localization")
-            sky_map = localize(
-                event, opts.waveform, opts.f_low, opts.min_distance,
-                opts.max_distance, opts.prior_distance_power, opts.cosmology,
-                mcmc=opts.mcmc, chain_dump=chain_dump,
-                enable_snr_series=opts.enable_snr_series,
-                f_high_truncate=opts.f_high_truncate,
-                rescale_loglikelihood=opts.rescale_loglikelihood)
-            if not opts.enable_multiresolution:
-                sky_map = rasterize(sky_map)
-            sky_map.meta['objid'] = str(graceid)
-            sky_map.meta['url'] = '{}/{}'.format(base_url, graceid)
-            log.info("sky localization complete")
-
-            # upload FITS file
-            with tempfile.TemporaryDirectory() as fitsdir:
-                fitspath = os.path.join(fitsdir, opts.output)
-                fits.write_sky_map(fitspath, sky_map, nest=True)
-                log.debug('wrote FITS file: %s', opts.output)
-                if opts.dry_run:
-                    rename(fitspath, os.path.join('.', opts.output))
-                else:
-                    gracedb.writeLog(
-                        graceid, "BAYESTAR rapid sky localization ready",
-                        filename=fitspath, tagname=tags)
-                log.debug('uploaded FITS file')
-        except KeyboardInterrupt:
-            # Produce log message and then exit if we receive SIGINT (ctrl-C).
-            log.exception("sky localization failed")
-            raise
-        except:  # noqa: E722
-            # Produce log message for any otherwise uncaught exception.
-            # Unless we are in dry-run mode, keep going.
-            log.exception("sky localization failed")
-            if opts.dry_run:
-                # Then re-raise the exception if we are in dry-run mode
+    with parser().parse_args(args) as opts:
+        import logging
+        import os
+        import re
+        import sys
+        import tempfile
+        import urllib.parse
+        from ..bayestar import localize, rasterize
+        from ..io import fits
+        from ..io import events
+        from .. import omp
+        from ..util.file import rename
+        import ligo.gracedb.logging
+        import ligo.gracedb.rest
+
+        log = logging.getLogger('BAYESTAR')
+
+        log.info('Using %d OpenMP thread(s)', omp.num_threads)
+
+        # If no GraceDB IDs were specified on the command line, then read them
+        # from stdin line-by-line.
+        graceids = opts.graceid if opts.graceid else iterlines(sys.stdin)
+
+        # Fire up a GraceDb client
+        # FIXME: Mimic the behavior of the GraceDb command line client, where
+        # the environment variable GRACEDB_SERVICE_URL overrides the default
+        # service URL. It would be nice to get this behavior into the gracedb
+        # package itself.
+        gracedb = ligo.gracedb.rest.GraceDb(
+            os.environ.get(
+                'GRACEDB_SERVICE_URL', ligo.gracedb.rest.DEFAULT_SERVICE_URL))
+
+        # Determine the base URL for event pages.
+        scheme, netloc, *_ = urllib.parse.urlparse(gracedb._service_url)
+        base_url = urllib.parse.urlunparse(
+            (scheme, netloc, 'events', '', '', ''))
+
+        if opts.chain_dump:
+            chain_dump = re.sub(r'.fits(.gz)?$', r'.hdf5', opts.output)
+        else:
+            chain_dump = None
+
+        tags = ("sky_loc",)
+        if not opts.no_tag:
+            tags += ("lvem",)
+
+        event_source = events.gracedb.open(graceids, gracedb)
+
+        if opts.disable_detector:
+            event_source = events.detector_disabled.open(
+                event_source, opts.disable_detector)
+
+        for graceid in event_source.keys():
+
+            try:
+                event = event_source[graceid]
+            except:  # noqa: E722
+                log.exception('failed to read event %s from GraceDB', graceid)
+                continue
+
+            # Send log messages to GraceDb too
+            if not opts.dry_run:
+                handler = ligo.gracedb.logging.GraceDbLogHandler(
+                    gracedb, graceid)
+                handler.setLevel(logging.INFO)
+                logging.root.addHandler(handler)
+
+            # A little bit of Cylon humor
+            log.info('by your command...')
+
+            try:
+                # perform sky localization
+                log.info("starting sky localization")
+                sky_map = localize(
+                    event, opts.waveform, opts.f_low, opts.min_distance,
+                    opts.max_distance, opts.prior_distance_power,
+                    opts.cosmology, mcmc=opts.mcmc, chain_dump=chain_dump,
+                    enable_snr_series=opts.enable_snr_series,
+                    f_high_truncate=opts.f_high_truncate,
+                    rescale_loglikelihood=opts.rescale_loglikelihood)
+                if not opts.enable_multiresolution:
+                    sky_map = rasterize(sky_map)
+                sky_map.meta['objid'] = str(graceid)
+                sky_map.meta['url'] = '{}/{}'.format(base_url, graceid)
+                log.info("sky localization complete")
+
+                # upload FITS file
+                with tempfile.TemporaryDirectory() as fitsdir:
+                    fitspath = os.path.join(fitsdir, opts.output)
+                    fits.write_sky_map(fitspath, sky_map, nest=True)
+                    log.debug('wrote FITS file: %s', opts.output)
+                    if opts.dry_run:
+                        rename(fitspath, os.path.join('.', opts.output))
+                    else:
+                        gracedb.writeLog(
+                            graceid, "BAYESTAR rapid sky localization ready",
+                            filename=fitspath, tagname=tags)
+                    log.debug('uploaded FITS file')
+            except KeyboardInterrupt:
+                # Produce log message and then exit if we receive SIGINT
+                # (ctrl-C).
+                log.exception("sky localization failed")
                 raise
+            except:  # noqa: E722
+                # Produce log message for any otherwise uncaught exception.
+                # Unless we are in dry-run mode, keep going.
+                log.exception("sky localization failed")
+                if opts.dry_run:
+                    # Then re-raise the exception if we are in dry-run mode
+                    raise
 
-        if not opts.dry_run:
-            # Remove old log handler
-            logging.root.removeHandler(handler)
-            del handler
+            if not opts.dry_run:
+                # Remove old log handler
+                logging.root.removeHandler(handler)
+                del handler
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_mcmc.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,133 +65,141 @@
 
 
 def identity(x):
     return x
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
+    with parser().parse_args(args) as opts:
+        import logging
+        log = logging.getLogger('BAYESTAR')
+
+        # BAYESTAR imports.
+        from ..io import events, hdf5
+        from ..bayestar import condition, condition_prior, ez_emcee, log_post
+
+        # Other imports.
+        from astropy.table import Table
+        import numpy as np
+        import os
+        import subprocess
+        import sys
+
+        import lal
+
+        # Read coinc file.
+        log.info(
+            '%s:reading input files', ','.join(
+                file.name for file in opts.input))
+        event_source = events.open(*opts.input, sample=opts.pycbc_sample)
+
+        os.makedirs(opts.output, exist_ok=True)
+
+        if opts.condor_submit:
+            if opts.seed is not None:
+                raise NotImplementedError(
+                    '--seed does not yet work with --condor-submit')
+            if opts.coinc_event_id:
+                raise ValueError(
+                    'must not set --coinc-event-id with --condor-submit')
+            with subprocess.Popen(['condor_submit'],
+                                  text=True, stdin=subprocess.PIPE) as proc:
+                f = proc.stdin
+                print('''
+                    accounting_group = ligo.dev.o4.cbc.pe.bayestar
+                    on_exit_remove = (ExitBySignal == False) && (ExitCode == 0)
+                    on_exit_hold = (ExitBySignal == True) || (ExitCode != 0)
+                    on_exit_hold_reason = (ExitBySignal == True \
+                        ? strcat("The job exited with signal ", ExitSignal) \
+                        : strcat("The job exited with code ", ExitCode))
+                    request_memory = 1000 MB
+                    universe = vanilla
+                    getenv = true
+                    executable = /usr/bin/env
+                    JobBatchName = BAYESTAR
+                    environment = "OMP_NUM_THREADS=1"
+                    ''', file=f)
+                print(
+                    'error =', os.path.join(opts.output, '$(cid).err'), file=f)
+                print('log =', os.path.join(opts.output, '$(cid).log'), file=f)
+                print(
+                    'arguments = "',
+                    *(arg for arg in sys.argv if arg != '--condor-submit'),
+                    '--coinc-event-id $(cid)"', file=f)
+                print('queue cid in', *event_source, file=f)
+            sys.exit(proc.returncode)
 
-    import logging
-    log = logging.getLogger('BAYESTAR')
-
-    # BAYESTAR imports.
-    from ..io import events, hdf5
-    from ..bayestar import condition, condition_prior, ez_emcee, log_post
-
-    # Other imports.
-    from astropy.table import Table
-    import numpy as np
-    import os
-    import subprocess
-    import sys
-
-    import lal
-
-    # Read coinc file.
-    log.info(
-        '%s:reading input files', ','.join(file.name for file in opts.input))
-    event_source = events.open(*opts.input, sample=opts.pycbc_sample)
-
-    os.makedirs(opts.output, exist_ok=True)
-
-    if opts.condor_submit:
-        if opts.seed is not None:
-            raise NotImplementedError(
-                '--seed does not yet work with --condor-submit')
         if opts.coinc_event_id:
-            raise ValueError(
-                'must not set --coinc-event-id with --condor-submit')
-        with subprocess.Popen(['condor_submit'],
-                              text=True, stdin=subprocess.PIPE) as proc:
-            f = proc.stdin
-            print('''
-                  accounting_group = ligo.dev.o4.cbc.pe.bayestar
-                  on_exit_remove = (ExitBySignal == False) && (ExitCode == 0)
-                  on_exit_hold = (ExitBySignal == True) || (ExitCode != 0)
-                  on_exit_hold_reason = (ExitBySignal == True \
-                    ? strcat("The job exited with signal ", ExitSignal) \
-                    : strcat("The job exited with code ", ExitCode))
-                  request_memory = 1000 MB
-                  universe = vanilla
-                  getenv = true
-                  executable = /usr/bin/env
-                  JobBatchName = BAYESTAR
-                  environment = "OMP_NUM_THREADS=1"
-                  ''', file=f)
-            print('error =', os.path.join(opts.output, '$(cid).err'), file=f)
-            print('log =', os.path.join(opts.output, '$(cid).log'), file=f)
-            print('arguments = "',
-                  *(arg for arg in sys.argv if arg != '--condor-submit'),
-                  '--coinc-event-id $(cid)"', file=f)
-            print('queue cid in', *event_source, file=f)
-        sys.exit(proc.returncode)
-
-    if opts.coinc_event_id:
-        event_source = {key: event_source[key] for key in opts.coinc_event_id}
-
-    # Loop over all sngl_inspiral <-> sngl_inspiral coincs.
-    for int_coinc_event_id, event in event_source.items():
-        coinc_event_id = 'coinc_event:coinc_event_id:{}'.format(
-            int_coinc_event_id)
-
-        log.info('%s:preparing', coinc_event_id)
-
-        epoch, sample_rate, epochs, snrs, responses, locations, horizons = \
-            condition(event, waveform=opts.waveform, f_low=opts.f_low,
-                      enable_snr_series=opts.enable_snr_series,
-                      f_high_truncate=opts.f_high_truncate)
-
-        min_distance, max_distance, prior_distance_power, cosmology = \
-            condition_prior(horizons, opts.min_distance, opts.max_distance,
-                            opts.prior_distance_power, opts.cosmology)
-
-        gmst = lal.GreenwichMeanSiderealTime(epoch)
-
-        max_abs_t = 2 * snrs.data.shape[1] / sample_rate
-        xmin = [0, -1, min_distance, -1, 0, 0]
-        xmax = [2 * np.pi, 1, max_distance, 1, 2 * np.pi, 2 * max_abs_t]
-        names = 'ra dec distance inclination twopsi time'.split()
-        transformed_names = 'ra sin_dec distance u twopsi time'.split()
-        forward_transforms = [identity, np.sin, identity,
-                              np.cos, identity, identity]
-        reverse_transforms = [identity, np.arcsin, identity,
-                              np.arccos, identity, identity]
-        kwargs = dict(min_distance=min_distance, max_distance=max_distance,
-                      prior_distance_power=prior_distance_power,
-                      cosmology=cosmology, gmst=gmst, sample_rate=sample_rate,
-                      epochs=epochs, snrs=snrs, responses=responses,
-                      locations=locations, horizons=horizons)
-
-        # Fix parameters
-        for i, key in reversed(list(enumerate(['ra', 'dec', 'distance']))):
-            value = getattr(opts, key)
-            if value is None:
-                continue
-
-            if key in ['ra', 'dec']:
-                # FIXME: figure out a more elegant way to address different
-                # units in command line arguments and posterior samples
-                value = np.deg2rad(value)
-
-            kwargs[transformed_names[i]] = forward_transforms[i](value)
-            del (xmin[i], xmax[i], names[i], transformed_names[i],
-                 forward_transforms[i], reverse_transforms[i])
-
-        log.info('%s:sampling', coinc_event_id)
-
-        # Run MCMC
-        chain = ez_emcee(log_post, xmin, xmax, kwargs=kwargs, vectorize=True)
-
-        # Transform back from sin_dec to dec and cos_inclination to inclination
-        for i, func in enumerate(reverse_transforms):
-            chain[:, i] = func(chain[:, i])
-
-        # Create Astropy table
-        chain = Table(rows=chain, names=names, copy=False)
-
-        log.info('%s:saving posterior samples', coinc_event_id)
-
-        hdf5.write_samples(
-            chain,
-            os.path.join(opts.output, '{}.hdf5'.format(int_coinc_event_id)),
-            path='/bayestar/posterior_samples', overwrite=True)
+            event_source = {
+                key: event_source[key] for key in opts.coinc_event_id}
+
+        # Loop over all sngl_inspiral <-> sngl_inspiral coincs.
+        for int_coinc_event_id, event in event_source.items():
+            coinc_event_id = 'coinc_event:coinc_event_id:{}'.format(
+                int_coinc_event_id)
+
+            log.info('%s:preparing', coinc_event_id)
+
+            epoch, sample_rate, epochs, snrs, responses, locations, horizons \
+                = condition(event, waveform=opts.waveform, f_low=opts.f_low,
+                            enable_snr_series=opts.enable_snr_series,
+                            f_high_truncate=opts.f_high_truncate)
+
+            min_distance, max_distance, prior_distance_power, cosmology \
+                = condition_prior(horizons, opts.min_distance,
+                                  opts.max_distance, opts.prior_distance_power,
+                                  opts.cosmology)
+
+            gmst = lal.GreenwichMeanSiderealTime(epoch)
+
+            max_abs_t = 2 * snrs.data.shape[1] / sample_rate
+            xmin = [0, -1, min_distance, -1, 0, 0]
+            xmax = [2 * np.pi, 1, max_distance, 1, 2 * np.pi, 2 * max_abs_t]
+            names = 'ra dec distance inclination twopsi time'.split()
+            transformed_names = 'ra sin_dec distance u twopsi time'.split()
+            forward_transforms = [identity, np.sin, identity,
+                                  np.cos, identity, identity]
+            reverse_transforms = [identity, np.arcsin, identity,
+                                  np.arccos, identity, identity]
+            kwargs = dict(min_distance=min_distance, max_distance=max_distance,
+                          prior_distance_power=prior_distance_power,
+                          cosmology=cosmology, gmst=gmst,
+                          sample_rate=sample_rate, epochs=epochs, snrs=snrs,
+                          responses=responses, locations=locations,
+                          horizons=horizons)
+
+            # Fix parameters
+            for i, key in reversed(list(enumerate(['ra', 'dec', 'distance']))):
+                value = getattr(opts, key)
+                if value is None:
+                    continue
+
+                if key in ['ra', 'dec']:
+                    # FIXME: figure out a more elegant way to address different
+                    # units in command line arguments and posterior samples
+                    value = np.deg2rad(value)
+
+                kwargs[transformed_names[i]] = forward_transforms[i](value)
+                del (xmin[i], xmax[i], names[i], transformed_names[i],
+                     forward_transforms[i], reverse_transforms[i])
+
+            log.info('%s:sampling', coinc_event_id)
+
+            # Run MCMC
+            chain = ez_emcee(
+                log_post, xmin, xmax, kwargs=kwargs, vectorize=True)
+
+            # Transform back from sin_dec to dec and cos_inclination to
+            # inclination
+            for i, func in enumerate(reverse_transforms):
+                chain[:, i] = func(chain[:, i])
+
+            # Create Astropy table
+            chain = Table(rows=chain, names=names, copy=False)
+
+            log.info('%s:saving posterior samples', coinc_event_id)
+
+            hdf5.write_samples(
+                chain,
+                os.path.join(
+                    opts.output, '{}.hdf5'.format(int_coinc_event_id)),
+                path='/bayestar/posterior_samples', overwrite=True)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_realize_coincs.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_realize_coincs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -215,247 +215,253 @@
             ra, dec, psi, inc, DL, epoch, gmst, H, S, response, location,
             measurement_error=measurement_error)
         for S, response, location in zip(psds, responses, locations)]
 
 
 def main(args=None):
     p = parser()
-    opts = p.parse_args(args)
+    with p.parse_args(args) as opts:
+        # LIGO-LW XML imports.
+        from ligo.lw import ligolw
+        from ligo.lw.param import Param
+        from ligo.lw.utils.search_summary import append_search_summary
+        from ligo.lw import utils as ligolw_utils
+        from ligo.lw.lsctables import (
+            New, CoincDefTable, CoincID, CoincInspiralTable, CoincMapTable,
+            CoincTable, ProcessParamsTable, ProcessTable, SimInspiralTable,
+            SnglInspiralTable, TimeSlideTable)
+
+        # glue, LAL and pylal imports.
+        from ligo import segments
+        import lal
+        import lal.series
+        import lalsimulation
+        from lalinspiral.inspinjfind import InspiralSCExactCoincDef
+        from lalinspiral.thinca import InspiralCoincDef
+        from tqdm import tqdm
+
+        # BAYESTAR imports.
+        from ..io.events.ligolw import ContentHandler
+        from ..bayestar import filter
+        from ..util.progress import progress_map
+
+        # Read PSDs.
+        xmldoc = ligolw_utils.load_fileobj(
+            opts.reference_psd, contenthandler=lal.series.PSDContentHandler)
+        psds = lal.series.read_psd_xmldoc(xmldoc, root_name=None)
+        psds = {
+            key: filter.InterpolatedPSD(filter.abscissa(psd), psd.data.data)
+            for key, psd in psds.items() if psd is not None}
+        psds = [psds[ifo] for ifo in opts.detector]
+
+        # Extract simulation table from injection file.
+        inj_xmldoc = ligolw_utils.load_fileobj(
+            opts.input, contenthandler=ContentHandler)
+        orig_sim_inspiral_table = SimInspiralTable.get_table(inj_xmldoc)
+
+        # Prune injections that are outside distance limits.
+        orig_sim_inspiral_table[:] = [
+            row for row in orig_sim_inspiral_table
+            if opts.min_distance <= row.distance <= opts.max_distance]
+
+        # Open output file.
+        xmldoc = ligolw.Document()
+        xmlroot = xmldoc.appendChild(ligolw.LIGO_LW())
+
+        # Create tables. Process and ProcessParams tables are copied from the
+        # injection file.
+        coinc_def_table = xmlroot.appendChild(New(CoincDefTable))
+        coinc_inspiral_table = xmlroot.appendChild(New(CoincInspiralTable))
+        coinc_map_table = xmlroot.appendChild(New(CoincMapTable))
+        coinc_table = xmlroot.appendChild(New(CoincTable))
+        xmlroot.appendChild(ProcessParamsTable.get_table(inj_xmldoc))
+        xmlroot.appendChild(ProcessTable.get_table(inj_xmldoc))
+        sim_inspiral_table = xmlroot.appendChild(New(SimInspiralTable))
+        sngl_inspiral_table = xmlroot.appendChild(New(SnglInspiralTable))
+        time_slide_table = xmlroot.appendChild(New(TimeSlideTable))
+
+        # Write process metadata to output file.
+        process = register_to_xmldoc(
+            xmldoc, p, opts, instruments=opts.detector,
+            comment="Simulated coincidences")
+
+        # Add search summary to output file.
+        all_time = segments.segment([lal.LIGOTimeGPS(0), lal.LIGOTimeGPS(2e9)])
+        append_search_summary(xmldoc, process, inseg=all_time, outseg=all_time)
+
+        # Create a time slide entry.  Needed for coinc_event rows.
+        time_slide_id = time_slide_table.get_time_slide_id(
+            {ifo: 0 for ifo in opts.detector}, create_new=process)
+
+        # Populate CoincDef table.
+        inspiral_coinc_def = copy.copy(InspiralCoincDef)
+        inspiral_coinc_def.coinc_def_id = coinc_def_table.get_next_id()
+        coinc_def_table.append(inspiral_coinc_def)
+        found_coinc_def = copy.copy(InspiralSCExactCoincDef)
+        found_coinc_def.coinc_def_id = coinc_def_table.get_next_id()
+        coinc_def_table.append(found_coinc_def)
+
+        # Precompute values that are common to all simulations.
+        detectors = [lalsimulation.DetectorPrefixToLALDetector(ifo)
+                     for ifo in opts.detector]
+        responses = [det.response for det in detectors]
+        locations = [det.location for det in detectors]
+
+        func = functools.partial(simulate, psds=psds,
+                                 responses=responses, locations=locations,
+                                 measurement_error=opts.measurement_error,
+                                 f_low=opts.f_low, f_high=opts.f_high,
+                                 waveform=opts.waveform)
+
+        # Make sure that each thread gets a different random number state.
+        # We start by drawing a random integer s in the main thread, and
+        # then the i'th subprocess will seed itself with the integer i + s.
+        #
+        # The seed must be an unsigned 32-bit integer, so if there are n
+        # threads, then s must be drawn from the interval [0, 2**32 - n).
+        #
+        # Note that *we* are thread 0, so there are a total of
+        # n=1+len(sim_inspiral_table) threads.
+        seed = np.random.randint(0, 2 ** 32 - len(sim_inspiral_table) - 1)
+        np.random.seed(seed)
+
+        with tqdm(desc='accepted') as progress:
+            for sim_inspiral, simulation in zip(
+                    orig_sim_inspiral_table,
+                    progress_map(
+                        func,
+                        np.arange(len(orig_sim_inspiral_table)) + seed + 1,
+                        orig_sim_inspiral_table, jobs=opts.jobs)):
+
+                sngl_inspirals = []
+                used_snr_series = []
+                net_snr = 0.0
+                count_triggers = 0
+
+                # Loop over individual detectors and create SnglInspiral
+                # entries.
+                for ifo, (horizon, abs_snr, arg_snr, toa, series) \
+                        in zip(opts.detector, simulation):
+
+                    if np.random.uniform() > opts.duty_cycle:
+                        continue
+                    elif abs_snr >= opts.snr_threshold:
+                        # If SNR < threshold, then the injection is not found.
+                        # Skip it.
+                        count_triggers += 1
+                        net_snr += np.square(abs_snr)
+                    elif not opts.keep_subthreshold:
+                        continue
+
+                    # Create SnglInspiral entry.
+                    used_snr_series.append(series)
+                    sngl_inspirals.append(
+                        sngl_inspiral_table.RowType(**dict(
+                            dict.fromkeys(
+                                sngl_inspiral_table.validcolumns, None),
+                            process_id=process.process_id,
+                            ifo=ifo,
+                            mass1=sim_inspiral.mass1,
+                            mass2=sim_inspiral.mass2,
+                            spin1x=sim_inspiral.spin1x,
+                            spin1y=sim_inspiral.spin1y,
+                            spin1z=sim_inspiral.spin1z,
+                            spin2x=sim_inspiral.spin2x,
+                            spin2y=sim_inspiral.spin2y,
+                            spin2z=sim_inspiral.spin2z,
+                            end=toa,
+                            snr=abs_snr,
+                            coa_phase=arg_snr,
+                            f_final=opts.f_high,
+                            eff_distance=horizon / abs_snr)))
 
-    # LIGO-LW XML imports.
-    from ligo.lw import ligolw
-    from ligo.lw.param import Param
-    from ligo.lw.utils.search_summary import append_search_summary
-    from ligo.lw import utils as ligolw_utils
-    from ligo.lw.lsctables import (
-        New, CoincDefTable, CoincID, CoincInspiralTable, CoincMapTable,
-        CoincTable, ProcessParamsTable, ProcessTable, SimInspiralTable,
-        SnglInspiralTable, TimeSlideTable)
-
-    # glue, LAL and pylal imports.
-    from ligo import segments
-    import lal
-    import lal.series
-    import lalsimulation
-    from lalinspiral.inspinjfind import InspiralSCExactCoincDef
-    from lalinspiral.thinca import InspiralCoincDef
-    from tqdm import tqdm
+                net_snr = np.sqrt(net_snr)
 
-    # BAYESTAR imports.
-    from ..io.events.ligolw import ContentHandler
-    from ..bayestar import filter
-    from ..util.progress import progress_map
+                # If too few triggers were found, then skip this event.
+                if count_triggers < opts.min_triggers:
+                    continue
 
-    # Read PSDs.
-    xmldoc = ligolw_utils.load_fileobj(
-        opts.reference_psd, contenthandler=lal.series.PSDContentHandler)
-    psds = lal.series.read_psd_xmldoc(xmldoc, root_name=None)
-    psds = {
-        key: filter.InterpolatedPSD(filter.abscissa(psd), psd.data.data)
-        for key, psd in psds.items() if psd is not None}
-    psds = [psds[ifo] for ifo in opts.detector]
-
-    # Extract simulation table from injection file.
-    inj_xmldoc = ligolw_utils.load_fileobj(
-        opts.input, contenthandler=ContentHandler)
-    orig_sim_inspiral_table = SimInspiralTable.get_table(inj_xmldoc)
-
-    # Prune injections that are outside distance limits.
-    orig_sim_inspiral_table[:] = [
-        row for row in orig_sim_inspiral_table
-        if opts.min_distance <= row.distance <= opts.max_distance]
-
-    # Open output file.
-    xmldoc = ligolw.Document()
-    xmlroot = xmldoc.appendChild(ligolw.LIGO_LW())
-
-    # Create tables. Process and ProcessParams tables are copied from the
-    # injection file.
-    coinc_def_table = xmlroot.appendChild(New(CoincDefTable))
-    coinc_inspiral_table = xmlroot.appendChild(New(CoincInspiralTable))
-    coinc_map_table = xmlroot.appendChild(New(CoincMapTable))
-    coinc_table = xmlroot.appendChild(New(CoincTable))
-    xmlroot.appendChild(ProcessParamsTable.get_table(inj_xmldoc))
-    xmlroot.appendChild(ProcessTable.get_table(inj_xmldoc))
-    sim_inspiral_table = xmlroot.appendChild(New(SimInspiralTable))
-    sngl_inspiral_table = xmlroot.appendChild(New(SnglInspiralTable))
-    time_slide_table = xmlroot.appendChild(New(TimeSlideTable))
-
-    # Write process metadata to output file.
-    process = register_to_xmldoc(
-        xmldoc, p, opts, instruments=opts.detector,
-        comment="Simulated coincidences")
-
-    # Add search summary to output file.
-    all_time = segments.segment([lal.LIGOTimeGPS(0), lal.LIGOTimeGPS(2e9)])
-    append_search_summary(xmldoc, process, inseg=all_time, outseg=all_time)
-
-    # Create a time slide entry.  Needed for coinc_event rows.
-    time_slide_id = time_slide_table.get_time_slide_id(
-        {ifo: 0 for ifo in opts.detector}, create_new=process)
-
-    # Populate CoincDef table.
-    inspiral_coinc_def = copy.copy(InspiralCoincDef)
-    inspiral_coinc_def.coinc_def_id = coinc_def_table.get_next_id()
-    coinc_def_table.append(inspiral_coinc_def)
-    found_coinc_def = copy.copy(InspiralSCExactCoincDef)
-    found_coinc_def.coinc_def_id = coinc_def_table.get_next_id()
-    coinc_def_table.append(found_coinc_def)
-
-    # Precompute values that are common to all simulations.
-    detectors = [lalsimulation.DetectorPrefixToLALDetector(ifo)
-                 for ifo in opts.detector]
-    responses = [det.response for det in detectors]
-    locations = [det.location for det in detectors]
-
-    func = functools.partial(simulate, psds=psds,
-                             responses=responses, locations=locations,
-                             measurement_error=opts.measurement_error,
-                             f_low=opts.f_low, f_high=opts.f_high,
-                             waveform=opts.waveform)
-
-    # Make sure that each thread gets a different random number state.
-    # We start by drawing a random integer s in the main thread, and
-    # then the i'th subprocess will seed itself with the integer i + s.
-    #
-    # The seed must be an unsigned 32-bit integer, so if there are n
-    # threads, then s must be drawn from the interval [0, 2**32 - n).
-    #
-    # Note that *we* are thread 0, so there are a total of
-    # n=1+len(sim_inspiral_table) threads.
-    seed = np.random.randint(0, 2 ** 32 - len(sim_inspiral_table) - 1)
-    np.random.seed(seed)
+                # If network SNR < threshold, then the injection is not found.
+                # Skip it.
+                if net_snr < opts.net_snr_threshold:
+                    continue
 
-    with tqdm(desc='accepted') as progress:
-        for sim_inspiral, simulation in zip(
-                orig_sim_inspiral_table,
-                progress_map(
-                    func,
-                    np.arange(len(orig_sim_inspiral_table)) + seed + 1,
-                    orig_sim_inspiral_table, jobs=opts.jobs)):
-
-            sngl_inspirals = []
-            used_snr_series = []
-            net_snr = 0.0
-            count_triggers = 0
-
-            # Loop over individual detectors and create SnglInspiral entries.
-            for ifo, (horizon, abs_snr, arg_snr, toa, series) \
-                    in zip(opts.detector, simulation):
+                # Add Coinc table entry.
+                coinc = coinc_table.appendRow(
+                    coinc_event_id=coinc_table.get_next_id(),
+                    process_id=process.process_id,
+                    coinc_def_id=inspiral_coinc_def.coinc_def_id,
+                    time_slide_id=time_slide_id,
+                    insts=opts.detector,
+                    nevents=len(opts.detector),
+                    likelihood=None)
 
-                if np.random.uniform() > opts.duty_cycle:
-                    continue
-                elif abs_snr >= opts.snr_threshold:
-                    # If SNR < threshold, then the injection is not found.
-                    # Skip it.
-                    count_triggers += 1
-                    net_snr += np.square(abs_snr)
-                elif not opts.keep_subthreshold:
-                    continue
+                # Add CoincInspiral table entry.
+                coinc_inspiral_table.appendRow(
+                    coinc_event_id=coinc.coinc_event_id,
+                    instruments=[
+                        sngl_inspiral.ifo for sngl_inspiral in sngl_inspirals],
+                    end=lal.LIGOTimeGPS(1e-9 * np.mean([
+                        sngl_inspiral.end.ns()
+                        for sngl_inspiral in sngl_inspirals
+                        if sngl_inspiral.end is not None])),
+                    mass=sim_inspiral.mass1 + sim_inspiral.mass2,
+                    mchirp=sim_inspiral.mchirp,
+                    combined_far=0.0,  # Not provided
+                    false_alarm_rate=0.0,  # Not provided
+                    minimum_duration=None,  # Not provided
+                    snr=net_snr)
+
+                # Record all sngl_inspiral records and associate them with
+                # coincs.
+                for sngl_inspiral, series in zip(
+                        sngl_inspirals, used_snr_series):
+                    # Give this sngl_inspiral record an id and add it to the
+                    # table.
+                    sngl_inspiral.event_id = sngl_inspiral_table.get_next_id()
+                    sngl_inspiral_table.append(sngl_inspiral)
+
+                    if opts.enable_snr_series:
+                        elem = lal.series.build_COMPLEX8TimeSeries(series)
+                        elem.appendChild(
+                            Param.from_pyvalue(
+                                'event_id', sngl_inspiral.event_id))
+                        xmlroot.appendChild(elem)
+
+                    # Add CoincMap entry.
+                    coinc_map_table.appendRow(
+                        coinc_event_id=coinc.coinc_event_id,
+                        table_name=sngl_inspiral_table.tableName,
+                        event_id=sngl_inspiral.event_id)
+
+                # Record injection
+                if not opts.preserve_ids:
+                    sim_inspiral.simulation_id \
+                        = sim_inspiral_table.get_next_id()
+                sim_inspiral_table.append(sim_inspiral)
 
-                # Create SnglInspiral entry.
-                used_snr_series.append(series)
-                sngl_inspirals.append(
-                    sngl_inspiral_table.RowType(**dict(
-                        dict.fromkeys(sngl_inspiral_table.validcolumns, None),
-                        process_id=process.process_id,
-                        ifo=ifo,
-                        mass1=sim_inspiral.mass1,
-                        mass2=sim_inspiral.mass2,
-                        spin1x=sim_inspiral.spin1x,
-                        spin1y=sim_inspiral.spin1y,
-                        spin1z=sim_inspiral.spin1z,
-                        spin2x=sim_inspiral.spin2x,
-                        spin2y=sim_inspiral.spin2y,
-                        spin2z=sim_inspiral.spin2z,
-                        end=toa,
-                        snr=abs_snr,
-                        coa_phase=arg_snr,
-                        f_final=opts.f_high,
-                        eff_distance=horizon / abs_snr)))
-
-            net_snr = np.sqrt(net_snr)
-
-            # If too few triggers were found, then skip this event.
-            if count_triggers < opts.min_triggers:
-                continue
-
-            # If network SNR < threshold, then the injection is not found.
-            # Skip it.
-            if net_snr < opts.net_snr_threshold:
-                continue
+                progress.update()
 
-            # Add Coinc table entry.
+        # Record coincidence associating injections with events.
+        for i, sim_inspiral in enumerate(sim_inspiral_table):
             coinc = coinc_table.appendRow(
                 coinc_event_id=coinc_table.get_next_id(),
                 process_id=process.process_id,
-                coinc_def_id=inspiral_coinc_def.coinc_def_id,
+                coinc_def_id=found_coinc_def.coinc_def_id,
                 time_slide_id=time_slide_id,
-                insts=opts.detector,
-                nevents=len(opts.detector),
+                instruments=None,
+                nevents=None,
                 likelihood=None)
-
-            # Add CoincInspiral table entry.
-            coinc_inspiral_table.appendRow(
+            coinc_map_table.appendRow(
                 coinc_event_id=coinc.coinc_event_id,
-                instruments=[
-                    sngl_inspiral.ifo for sngl_inspiral in sngl_inspirals],
-                end=lal.LIGOTimeGPS(1e-9 * np.mean([
-                    sngl_inspiral.end.ns()
-                    for sngl_inspiral in sngl_inspirals
-                    if sngl_inspiral.end is not None])),
-                mass=sim_inspiral.mass1 + sim_inspiral.mass2,
-                mchirp=sim_inspiral.mchirp,
-                combined_far=0.0,  # Not provided
-                false_alarm_rate=0.0,  # Not provided
-                minimum_duration=None,  # Not provided
-                snr=net_snr)
-
-            # Record all sngl_inspiral records and associate them with coincs.
-            for sngl_inspiral, series in zip(sngl_inspirals, used_snr_series):
-                # Give this sngl_inspiral record an id and add it to the table.
-                sngl_inspiral.event_id = sngl_inspiral_table.get_next_id()
-                sngl_inspiral_table.append(sngl_inspiral)
-
-                if opts.enable_snr_series:
-                    elem = lal.series.build_COMPLEX8TimeSeries(series)
-                    elem.appendChild(
-                        Param.from_pyvalue('event_id', sngl_inspiral.event_id))
-                    xmlroot.appendChild(elem)
-
-                # Add CoincMap entry.
-                coinc_map_table.appendRow(
-                    coinc_event_id=coinc.coinc_event_id,
-                    table_name=sngl_inspiral_table.tableName,
-                    event_id=sngl_inspiral.event_id)
-
-            # Record injection
-            if not opts.preserve_ids:
-                sim_inspiral.simulation_id = sim_inspiral_table.get_next_id()
-            sim_inspiral_table.append(sim_inspiral)
-
-            progress.update()
-
-    # Record coincidence associating injections with events.
-    for i, sim_inspiral in enumerate(sim_inspiral_table):
-        coinc = coinc_table.appendRow(
-            coinc_event_id=coinc_table.get_next_id(),
-            process_id=process.process_id,
-            coinc_def_id=found_coinc_def.coinc_def_id,
-            time_slide_id=time_slide_id,
-            instruments=None,
-            nevents=None,
-            likelihood=None)
-        coinc_map_table.appendRow(
-            coinc_event_id=coinc.coinc_event_id,
-            table_name=sim_inspiral_table.tableName,
-            event_id=sim_inspiral.simulation_id)
-        coinc_map_table.appendRow(
-            coinc_event_id=coinc.coinc_event_id,
-            table_name=coinc_table.tableName,
-            event_id=CoincID(i))
+                table_name=sim_inspiral_table.tableName,
+                event_id=sim_inspiral.simulation_id)
+            coinc_map_table.appendRow(
+                coinc_event_id=coinc.coinc_event_id,
+                table_name=coinc_table.tableName,
+                event_id=CoincID(i))
 
-    # Record process end time.
-    process.set_end_time_now()
+        # Record process end time.
+        process.set_end_time_now()
 
-    # Write output file.
-    write_fileobj(xmldoc, opts.output)
+        # Write output file.
+        write_fileobj(xmldoc, opts.output)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/bayestar_sample_model_psd.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/bayestar_sample_model_psd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2014-2020  Leo Singer
+# Copyright (C) 2014-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -74,55 +74,54 @@
             help='Scale range for {0} detector'.format(name))
 
     return parser
 
 
 def main(args=None):
     p = parser()
-    opts = p.parse_args(args)
-
-    import lal.series
-    import lalsimulation
-    import numpy as np
-    from ..bayestar.filter import vectorize_swig_psd_func
-
-    # Add basic options.
-
-    psds = {}
-
-    n = int(opts.f_max // opts.df)
-    f = np.arange(n) * opts.df
-
-    detectors = [d.frDetector.prefix for d in lal.CachedDetectors]
-
-    for detector in detectors:
-        psd_name = getattr(opts, detector, None)
-        if psd_name is None:
-            continue
-        scale = 1 / np.square(getattr(opts, detector + '_scale', 1.0))
-        func = getattr(lalsimulation, psd_name_prefix + psd_name)
-        series = lal.CreateREAL8FrequencySeries(
-            psd_name, 0, 0, opts.df, lal.SecondUnit, n)
-        if '(double f) -> double' in func.__doc__:
-            series.data.data = vectorize_swig_psd_func(
-                psd_name_prefix + psd_name)(f)
-        else:
-            func(series, 0.0)
-
-            # Find indices of first and last nonzero samples.
-            nonzero = np.flatnonzero(series.data.data)
-            # FIXME: int cast seems to be needed on old versions of Numpy
-            first_nonzero = int(nonzero[0])
-            last_nonzero = int(nonzero[-1])
-
-            # Truncate
-            series = lal.CutREAL8FrequencySeries(
-                series, first_nonzero, last_nonzero - first_nonzero + 1)
-            series.f0 = first_nonzero * series.deltaF
-
-            series.name = psd_name
-        series.data.data *= scale
-        psds[detector] = series
-
-    xmldoc = lal.series.make_psd_xmldoc(psds)
-    register_to_xmldoc(xmldoc, p, opts)
-    write_fileobj(xmldoc, opts.output)
+    with p.parse_args(args) as opts:
+        import lal.series
+        import lalsimulation
+        import numpy as np
+        from ..bayestar.filter import vectorize_swig_psd_func
+
+        # Add basic options.
+
+        psds = {}
+
+        n = int(opts.f_max // opts.df)
+        f = np.arange(n) * opts.df
+
+        detectors = [d.frDetector.prefix for d in lal.CachedDetectors]
+
+        for detector in detectors:
+            psd_name = getattr(opts, detector, None)
+            if psd_name is None:
+                continue
+            scale = 1 / np.square(getattr(opts, detector + '_scale', 1.0))
+            func = getattr(lalsimulation, psd_name_prefix + psd_name)
+            series = lal.CreateREAL8FrequencySeries(
+                psd_name, 0, 0, opts.df, lal.SecondUnit, n)
+            if '(double f) -> double' in func.__doc__:
+                series.data.data = vectorize_swig_psd_func(
+                    psd_name_prefix + psd_name)(f)
+            else:
+                func(series, 0.0)
+
+                # Find indices of first and last nonzero samples.
+                nonzero = np.flatnonzero(series.data.data)
+                # FIXME: int cast seems to be needed on old versions of Numpy
+                first_nonzero = int(nonzero[0])
+                last_nonzero = int(nonzero[-1])
+
+                # Truncate
+                series = lal.CutREAL8FrequencySeries(
+                    series, first_nonzero, last_nonzero - first_nonzero + 1)
+                series.f0 = first_nonzero * series.deltaF
+
+                series.name = psd_name
+            series.data.data *= scale
+            psds[detector] = series
+
+        xmldoc = lal.series.make_psd_xmldoc(psds)
+        register_to_xmldoc(xmldoc, p, opts)
+        write_fileobj(xmldoc, opts.output)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_combine.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_combine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2018-2020  Tito Dal Canton, Eric Burns, Leo Singer
+# Copyright (C) 2018-2024  Tito Dal Canton, Eric Burns, Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -39,108 +39,108 @@
     parser.add_argument('--origin', type=str,
                         help='Optional tag describing the organization'
                              ' responsible for the combined output')
     return parser
 
 
 def main(args=None):
-    args = parser().parse_args(args)
-
-    from textwrap import wrap
-    import numpy as np
-    import astropy_healpix as ah
-    from astropy.io import fits
-    from astropy.time import Time
-    import healpy as hp
-
-    from ..distance import parameters_to_marginal_moments
-    from ..io import read_sky_map, write_sky_map
-
-    input_skymaps = []
-    dist_mu = dist_sigma = dist_norm = None
-    for input_file in args.input:
-        with fits.open(input_file) as hdus:
-            header = hdus[0].header.copy()
-            header.extend(hdus[1].header)
-            has_distance = 'DISTMU' in hdus[1].columns.names
-            data, meta = read_sky_map(hdus, nest=True,
-                                      distances=has_distance)
-
-        if has_distance:
-            if dist_mu is not None:
-                raise RuntimeError('only one input localization can have'
-                                   ' distance information')
-            dist_mu = data[1]
-            dist_sigma = data[2]
-            dist_norm = data[3]
+    with parser().parse_args(args) as args:
+        from textwrap import wrap
+        import numpy as np
+        import astropy_healpix as ah
+        from astropy.io import fits
+        from astropy.time import Time
+        import healpy as hp
+
+        from ..distance import parameters_to_marginal_moments
+        from ..io import read_sky_map, write_sky_map
+
+        input_skymaps = []
+        dist_mu = dist_sigma = dist_norm = None
+        for input_file in args.input:
+            with fits.open(input_file) as hdus:
+                header = hdus[0].header.copy()
+                header.extend(hdus[1].header)
+                has_distance = 'DISTMU' in hdus[1].columns.names
+                data, meta = read_sky_map(hdus, nest=True,
+                                          distances=has_distance)
+
+            if has_distance:
+                if dist_mu is not None:
+                    raise RuntimeError('only one input localization can have '
+                                       'distance information')
+                dist_mu = data[1]
+                dist_sigma = data[2]
+                dist_norm = data[3]
+            else:
+                data = (data,)
+
+            nside = ah.npix_to_nside(len(data[0]))
+            input_skymaps.append((nside, data[0], meta, header))
+
+        max_nside = max(x[0] for x in input_skymaps)
+
+        # upsample sky posteriors to maximum resolution and combine them
+        combined_prob = None
+        for nside, prob, _, _ in input_skymaps:
+            if nside < max_nside:
+                prob = hp.ud_grade(prob, max_nside, order_in='NESTED',
+                                   order_out='NESTED')
+            if combined_prob is None:
+                combined_prob = np.ones_like(prob)
+            combined_prob *= prob
+
+        # normalize joint posterior
+        norm = combined_prob.sum()
+        if norm == 0:
+            raise RuntimeError('input sky localizations are disjoint')
+        combined_prob /= norm
+
+        out_kwargs = {'gps_creation_time': Time.now().gps,
+                      'nest': True}
+        if args.origin is not None:
+            out_kwargs['origin'] = args.origin
+
+        # average the various input event times
+        input_gps = [
+            x[2]['gps_time'] for x in input_skymaps if 'gps_time' in x[2]]
+        if input_gps:
+            out_kwargs['gps_time'] = np.mean(input_gps)
+
+        # combine instrument tags
+        out_instruments = set()
+        for x in input_skymaps:
+            if 'instruments' in x[2]:
+                out_instruments.update(x[2]['instruments'])
+        out_kwargs['instruments'] = ','.join(out_instruments)
+
+        # update marginal distance posterior, if available
+        if dist_mu is not None:
+            if ah.npix_to_nside(len(dist_mu)) < max_nside:
+                dist_mu = hp.ud_grade(dist_mu, max_nside, order_in='NESTED',
+                                      order_out='NESTED')
+                dist_sigma = hp.ud_grade(dist_sigma, max_nside,
+                                         order_in='NESTED', order_out='NESTED')
+                dist_norm = hp.ud_grade(dist_norm, max_nside,
+                                        order_in='NESTED', order_out='NESTED')
+            distmean, diststd = parameters_to_marginal_moments(combined_prob,
+                                                               dist_mu,
+                                                               dist_sigma)
+            out_data = (combined_prob, dist_mu, dist_sigma, dist_norm)
+            out_kwargs['distmean'] = distmean
+            out_kwargs['diststd'] = diststd
         else:
-            data = (data,)
-
-        nside = ah.npix_to_nside(len(data[0]))
-        input_skymaps.append((nside, data[0], meta, header))
-
-    max_nside = max(x[0] for x in input_skymaps)
+            out_data = combined_prob
 
-    # upsample sky posteriors to maximum resolution and combine them
-    combined_prob = None
-    for nside, prob, _, _ in input_skymaps:
-        if nside < max_nside:
-            prob = hp.ud_grade(prob, max_nside, order_in='NESTED',
-                               order_out='NESTED')
-        if combined_prob is None:
-            combined_prob = np.ones_like(prob)
-        combined_prob *= prob
-
-    # normalize joint posterior
-    norm = combined_prob.sum()
-    if norm == 0:
-        raise RuntimeError('input sky localizations are disjoint')
-    combined_prob /= norm
-
-    out_kwargs = {'gps_creation_time': Time.now().gps,
-                  'nest': True}
-    if args.origin is not None:
-        out_kwargs['origin'] = args.origin
-
-    # average the various input event times
-    input_gps = [x[2]['gps_time'] for x in input_skymaps if 'gps_time' in x[2]]
-    if input_gps:
-        out_kwargs['gps_time'] = np.mean(input_gps)
-
-    # combine instrument tags
-    out_instruments = set()
-    for x in input_skymaps:
-        if 'instruments' in x[2]:
-            out_instruments.update(x[2]['instruments'])
-    out_kwargs['instruments'] = ','.join(out_instruments)
-
-    # update marginal distance posterior, if available
-    if dist_mu is not None:
-        if ah.npix_to_nside(len(dist_mu)) < max_nside:
-            dist_mu = hp.ud_grade(dist_mu, max_nside, order_in='NESTED',
-                                  order_out='NESTED')
-            dist_sigma = hp.ud_grade(dist_sigma, max_nside, order_in='NESTED',
-                                     order_out='NESTED')
-            dist_norm = hp.ud_grade(dist_norm, max_nside, order_in='NESTED',
-                                    order_out='NESTED')
-        distmean, diststd = parameters_to_marginal_moments(combined_prob,
-                                                           dist_mu,
-                                                           dist_sigma)
-        out_data = (combined_prob, dist_mu, dist_sigma, dist_norm)
-        out_kwargs['distmean'] = distmean
-        out_kwargs['diststd'] = diststd
-    else:
-        out_data = combined_prob
-
-    # save input headers in output history
-    out_kwargs['HISTORY'] = []
-    for i, x in enumerate(input_skymaps):
-        out_kwargs['HISTORY'].append('')
-        out_kwargs['HISTORY'].append(
-            'Headers of HDUs 0 and 1 of input file {:d}:'.format(i))
-        out_kwargs['HISTORY'].append('')
-        for line in x[3].tostring(sep='\n',
-                                  endcard=False,
-                                  padding=False).split('\n'):
-            out_kwargs['HISTORY'].extend(wrap(line, 72))
+        # save input headers in output history
+        out_kwargs['HISTORY'] = []
+        for i, x in enumerate(input_skymaps):
+            out_kwargs['HISTORY'].append('')
+            out_kwargs['HISTORY'].append(
+                'Headers of HDUs 0 and 1 of input file {:d}:'.format(i))
+            out_kwargs['HISTORY'].append('')
+            for line in x[3].tostring(sep='\n',
+                                      endcard=False,
+                                      padding=False).split('\n'):
+                out_kwargs['HISTORY'].extend(wrap(line, 72))
 
-    write_sky_map(args.output, out_data, **out_kwargs)
+        write_sky_map(args.output, out_data, **out_kwargs)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_constellations.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_constellations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2019-2020  Leo Singer
+# Copyright (C) 2019-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -31,31 +31,30 @@
     parser.add_argument(
         '-o', '--output', metavar='OUT.dat', type=FileType('w'), default='-',
         help='Name of output file')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
-
-    # Late imports
-
-    from ..io import fits
-    import astropy_healpix as ah
-    from astropy.coordinates import SkyCoord
-    from astropy.table import Table
-    from astropy import units as u
-    import healpy as hp
-    import numpy as np
-
-    prob, meta = fits.read_sky_map(opts.input.name, nest=None)
-    npix = len(prob)
-    nside = ah.npix_to_nside(npix)
-    ipix = np.arange(npix)
-    ra, dec = hp.pix2ang(nside, ipix, lonlat=True, nest=meta['nest'])
-    coord = SkyCoord(ra * u.deg, dec * u.deg)
-    table = Table({'prob': prob, 'constellation': coord.get_constellation()},
-                  copy=False)
-    table = table.group_by('constellation').groups.aggregate(np.sum)
-    table.sort('prob')
-    table.reverse()
-    table.write(opts.output, format='ascii.tab')
+    with parser().parse_args(args) as opts:
+        # Late imports
+        from ..io import fits
+        import astropy_healpix as ah
+        from astropy.coordinates import SkyCoord
+        from astropy.table import Table
+        from astropy import units as u
+        import healpy as hp
+        import numpy as np
+
+        prob, meta = fits.read_sky_map(opts.input.name, nest=None)
+        npix = len(prob)
+        nside = ah.npix_to_nside(npix)
+        ipix = np.arange(npix)
+        ra, dec = hp.pix2ang(nside, ipix, lonlat=True, nest=meta['nest'])
+        coord = SkyCoord(ra * u.deg, dec * u.deg)
+        table = Table(
+            {'prob': prob, 'constellation': coord.get_constellation()},
+            copy=False)
+        table = table.group_by('constellation').groups.aggregate(np.sum)
+        table.sort('prob')
+        table.reverse()
+        table.write(opts.output, format='ascii.tab')
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_contour.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_contour.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2015-2018  Leo Singer
+# Copyright (C) 2015-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -44,53 +44,54 @@
     parser.add_argument(
         'input', metavar='INPUT.fits[.gz]', type=FileType('rb'),
         default='-', nargs='?', help='Input FITS file')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
-
-    import healpy as hp
-    import numpy as np
-    import json
-
-    from ..io import fits
-    from .. import postprocess
-
-    # Read input file
-    prob, _ = fits.read_sky_map(opts.input.name, nest=True)
-
-    # Resample if requested
-    if opts.nside is not None and opts.interpolate in ('nearest', 'nested'):
-        prob = hp.ud_grade(prob, opts.nside, order_in='NESTED', power=-2)
-    elif opts.nside is not None and opts.interpolate == 'bilinear':
-        prob = postprocess.smooth_ud_grade(prob, opts.nside, nest=True)
-    if opts.interpolate == 'nested':
-        prob = postprocess.interpolate_nested(prob, nest=True)
-
-    # Find credible levels
-    i = np.flipud(np.argsort(prob))
-    cumsum = np.cumsum(prob[i])
-    cls = np.empty_like(prob)
-    cls[i] = cumsum * 100
-
-    # Generate contours
-    paths = list(postprocess.contour(
-        cls, opts.contour, nest=True, degrees=True, simplify=opts.simplify))
-
-    json.dump({
-        'type': 'FeatureCollection',
-        'features': [
-            {
-                'type': 'Feature',
-                'properties': {
-                    'credible_level': contour
-                },
-                'geometry': {
-                    'type': 'MultiLineString',
-                    'coordinates': path
+    with parser().parse_args(args) as opts:
+        import healpy as hp
+        import numpy as np
+        import json
+
+        from ..io import fits
+        from .. import postprocess
+
+        # Read input file
+        prob, _ = fits.read_sky_map(opts.input.name, nest=True)
+
+        # Resample if requested
+        if opts.nside is not None and opts.interpolate in (
+                'nearest', 'nested'):
+            prob = hp.ud_grade(prob, opts.nside, order_in='NESTED', power=-2)
+        elif opts.nside is not None and opts.interpolate == 'bilinear':
+            prob = postprocess.smooth_ud_grade(prob, opts.nside, nest=True)
+        if opts.interpolate == 'nested':
+            prob = postprocess.interpolate_nested(prob, nest=True)
+
+        # Find credible levels
+        i = np.flipud(np.argsort(prob))
+        cumsum = np.cumsum(prob[i])
+        cls = np.empty_like(prob)
+        cls[i] = cumsum * 100
+
+        # Generate contours
+        paths = list(postprocess.contour(
+            cls, opts.contour, nest=True, degrees=True,
+            simplify=opts.simplify))
+
+        json.dump({
+            'type': 'FeatureCollection',
+            'features': [
+                {
+                    'type': 'Feature',
+                    'properties': {
+                        'credible_level': contour
+                    },
+                    'geometry': {
+                        'type': 'MultiLineString',
+                        'coordinates': path
+                    }
                 }
-            }
-            for contour, path in zip(opts.contour, paths)
-        ]
-    }, opts.output)
+                for contour, path in zip(opts.contour, paths)
+            ]
+        }, opts.output)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_contour_moc.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_contour_moc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023 Giuseppe Greco, Leo Singer, and CDS team.
+# Copyright (C) 2013-2024  Giuseppe Greco, Leo Singer, and CDS team.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -38,40 +38,39 @@
                                       HEALPix FITS file')
 
     return parser
 
 
 def main(args=None):
     p = parser()
-    opts = parser().parse_args(args)
+    with parser().parse_args(args) as opts:
+        import astropy_healpix as ah
+        import astropy.units as u
+
+        try:
+            from mocpy import MOC
+        except ImportError:
+            p.error('This command-line tool requires mocpy >= 0.8.2. '
+                    'Please install it by running "pip install mocpy".')
+
+        from ..io import read_sky_map
+
+        # Read multi-order sky map
+        skymap = read_sky_map(opts.input.name, moc=True)
+
+        uniq = skymap['UNIQ']
+        probdensity = skymap['PROBDENSITY']
+
+        level, ipix = ah.uniq_to_level_ipix(uniq)
+        area = ah.nside_to_pixel_area(
+            ah.level_to_nside(level)).to_value(u.steradian)
+
+        prob = probdensity * area
+
+        # Create MOC
+        contour_decimal = opts.contour / 100
+        moc = MOC.from_valued_healpix_cells(
+            uniq, prob, max_depth=level.max(),
+            cumul_from=0.0, cumul_to=contour_decimal)
 
-    import astropy_healpix as ah
-    import astropy.units as u
-
-    try:
-        from mocpy import MOC
-    except ImportError:
-        p.error('This command-line tool requires mocpy >= 0.8.2. '
-                'Please install it by running "pip install mocpy".')
-
-    from ..io import read_sky_map
-
-    # Read multi-order sky map
-    skymap = read_sky_map(opts.input.name, moc=True)
-
-    uniq = skymap['UNIQ']
-    probdensity = skymap['PROBDENSITY']
-
-    level, ipix = ah.uniq_to_level_ipix(uniq)
-    area = ah.nside_to_pixel_area(
-        ah.level_to_nside(level)).to_value(u.steradian)
-
-    prob = probdensity * area
-
-    # Create MOC
-    contour_decimal = opts.contour / 100
-    moc = MOC.from_valued_healpix_cells(
-        uniq, prob, max_depth=level.max(),
-        cumul_from=0.0, cumul_to=contour_decimal)
-
-    # Write MOC
-    moc.write(opts.output, format='fits', overwrite=True)
+        # Write MOC
+        moc.write(opts.output, format='fits', overwrite=True)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_flatten.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_flatten.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2018-2020  Leo Singer
+# Copyright (C) 2018-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -28,37 +28,37 @@
     parser.add_argument('output', metavar='OUTPUT.fits',
                         type=FileType('wb'), help='Output FITS file')
     parser.add_argument('--nside', type=int, help='Output HEALPix resolution')
     return parser
 
 
 def main(args=None):
-    args = parser().parse_args(args)
-
-    import logging
-    import warnings
-    import astropy_healpix as ah
-    from astropy.io import fits
-    from ..io import read_sky_map, write_sky_map
-    from ..bayestar import rasterize
-
-    log = logging.getLogger()
-
-    if args.nside is None:
-        order = None
-    else:
-        order = ah.nside_to_level(args.nside)
-
-    log.info('reading FITS file %s', args.input.name)
-    hdus = fits.open(args.input)
-    ordering = hdus[1].header['ORDERING']
-    expected_ordering = 'NUNIQ'
-    if ordering != expected_ordering:
-        msg = 'Expected the FITS file {} to have ordering {}, but it is {}'
-        warnings.warn(msg.format(args.input.name, expected_ordering, ordering))
-    log.debug('converting original FITS file to Astropy table')
-    table = read_sky_map(hdus, moc=True)
-    log.debug('flattening HEALPix tree')
-    table = rasterize(table, order=order)
-    log.info('writing FITS file %s', args.output.name)
-    write_sky_map(args.output.name, table, nest=True)
-    log.debug('done')
+    with parser().parse_args(args) as args:
+        import logging
+        import warnings
+        import astropy_healpix as ah
+        from astropy.io import fits
+        from ..io import read_sky_map, write_sky_map
+        from ..bayestar import rasterize
+
+        log = logging.getLogger()
+
+        if args.nside is None:
+            order = None
+        else:
+            order = ah.nside_to_level(args.nside)
+
+        log.info('reading FITS file %s', args.input.name)
+        hdus = fits.open(args.input)
+        ordering = hdus[1].header['ORDERING']
+        expected_ordering = 'NUNIQ'
+        if ordering != expected_ordering:
+            msg = 'Expected the FITS file {} to have ordering {}, but it is {}'
+            warnings.warn(
+                msg.format(args.input.name, expected_ordering, ordering))
+        log.debug('converting original FITS file to Astropy table')
+        table = read_sky_map(hdus, moc=True)
+        log.debug('flattening HEALPix tree')
+        table = rasterize(table, order=order)
+        log.info('writing FITS file %s', args.output.name)
+        write_sky_map(args.output.name, table, nest=True)
+        log.debug('done')
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_from_samples.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_from_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2011-2023  Will M. Farr <will.farr@ligo.org>
+# Copyright (C) 2011-2024  Will M. Farr <will.farr@ligo.org>
 #                          Leo P. Singer <leo.singer@ligo.org>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -82,105 +82,107 @@
                         'within the HDF5 file. By default, search for '
                         'posterior_samples')
     return parser
 
 
 def main(args=None):
     _parser = parser()
-    args = _parser.parse_args(args)
+    with _parser.parse_args(args) as args:
+        # Late imports
+        from .. import io
+        from ..io.hdf5 import _remap_colnames
+        from ..bayestar import rasterize
+        from .. import version
+        from astropy.table import Table
+        from astropy.time import Time
+        import numpy as np
+        import os
+        import sys
+        import pickle
+        from ..kde import Clustered2Plus1DSkyKDE, Clustered2DSkyKDE
+        import logging
+        from textwrap import wrap
 
-    # Late imports
-    from .. import io
-    from ..io.hdf5 import _remap_colnames
-    from ..bayestar import rasterize
-    from .. import version
-    from astropy.table import Table
-    from astropy.time import Time
-    import numpy as np
-    import os
-    import sys
-    import pickle
-    from ..kde import Clustered2Plus1DSkyKDE, Clustered2DSkyKDE
-    import logging
-    from textwrap import wrap
-
-    log = logging.getLogger()
-
-    log.info('reading samples')
-    try:
-        data = io.read_samples(args.samples.name, path=args.path,
-                               tablename=args.tablename)
-    except IOError:
-        # FIXME: remove this code path once we support only HDF5
-        data = Table.read(args.samples, format='ascii')
-        _remap_colnames(data)
-
-    if args.maxpts is not None and args.maxpts < len(data):
-        log.info('taking random subsample of chain')
-        data = data[np.random.choice(len(data), args.maxpts, replace=False)]
-    try:
-        dist = data['dist']
-    except KeyError:
+        log = logging.getLogger()
+
+        log.info('reading samples')
+        try:
+            data = io.read_samples(args.samples.name, path=args.path,
+                                   tablename=args.tablename)
+        except IOError:
+            # FIXME: remove this code path once we support only HDF5
+            data = Table.read(args.samples, format='ascii')
+            _remap_colnames(data)
+
+        if args.maxpts is not None and args.maxpts < len(data):
+            log.info('taking random subsample of chain')
+            data = data[
+                np.random.choice(len(data), args.maxpts, replace=False)]
         try:
-            dist = data['distance']
+            dist = data['dist']
         except KeyError:
-            dist = None
-
-    if args.loadpost is None:
-        if dist is None:
+            try:
+                dist = data['distance']
+            except KeyError:
+                dist = None
+
+        if args.loadpost is None:
+            if dist is None:
+                if args.enable_distance_map:
+                    _parser.error("The posterior samples file '{}' does not "
+                                  "have a distance column named 'dist' or "
+                                  "'distance'. Cannot generate distance map. "
+                                  "If you do not intend to generate a "
+                                  "distance map, then add the "
+                                  "'--disable-distance-map' command line "
+                                  "argument.".format(args.samples.name))
+                pts = np.column_stack((data['ra'], data['dec']))
+            else:
+                pts = np.column_stack((data['ra'], data['dec'], dist))
             if args.enable_distance_map:
-                _parser.error("The posterior samples file '{}' does not have "
-                              "a distance column named 'dist' or 'distance'. "
-                              "Cannot generate distance map. If you do not "
-                              "intend to generate a distance map, then add "
-                              "the '--disable-distance-map' command line "
-                              "argument.".format(args.samples.name))
-            pts = np.column_stack((data['ra'], data['dec']))
-        else:
-            pts = np.column_stack((data['ra'], data['dec'], dist))
-        if args.enable_distance_map:
-            cls = Clustered2Plus1DSkyKDE
+                cls = Clustered2Plus1DSkyKDE
+            else:
+                cls = Clustered2DSkyKDE
+            skypost = cls(pts, trials=args.trials, jobs=args.jobs)
+
+            log.info('pickling')
+            with open(os.path.join(args.outdir, 'skypost.obj'), 'wb') as out:
+                pickle.dump(skypost, out)
         else:
-            cls = Clustered2DSkyKDE
-        skypost = cls(pts, trials=args.trials, jobs=args.jobs)
+            skypost = pickle.load(args.loadpost)
+            skypost.jobs = args.jobs
 
-        log.info('pickling')
-        with open(os.path.join(args.outdir, 'skypost.obj'), 'wb') as out:
-            pickle.dump(skypost, out)
-    else:
-        skypost = pickle.load(args.loadpost)
-        skypost.jobs = args.jobs
-
-    log.info('making skymap')
-    hpmap = skypost.as_healpix(top_nside=args.top_nside)
-    if not args.enable_multiresolution:
-        hpmap = rasterize(hpmap)
-    hpmap.meta.update(io.fits.metadata_for_version_module(version))
-    hpmap.meta['creator'] = _parser.prog
-    hpmap.meta['origin'] = 'LIGO/Virgo/KAGRA'
-    hpmap.meta['gps_creation_time'] = Time.now().gps
-    hpmap.meta['history'] = [
-        '', 'Generated by running the following script:',
-        *wrap(' '.join([_parser.prog] + sys.argv[1:]), 72)]
-    if args.objid is not None:
-        hpmap.meta['objid'] = args.objid
-    if args.instruments:
-        hpmap.meta['instruments'] = args.instruments
-    if args.enable_distance_map:
-        hpmap.meta['distmean'] = np.mean(dist)
-        hpmap.meta['diststd'] = np.std(dist)
+        log.info('making skymap')
+        hpmap = skypost.as_healpix(top_nside=args.top_nside)
+        if not args.enable_multiresolution:
+            hpmap = rasterize(hpmap)
+        hpmap.meta.update(io.fits.metadata_for_version_module(version))
+        hpmap.meta['creator'] = _parser.prog
+        hpmap.meta['origin'] = 'LIGO/Virgo/KAGRA'
+        hpmap.meta['gps_creation_time'] = Time.now().gps
+        hpmap.meta['history'] = [
+            '', 'Generated by running the following script:',
+            *wrap(' '.join([_parser.prog] + sys.argv[1:]), 72)]
+        if args.objid is not None:
+            hpmap.meta['objid'] = args.objid
+        if args.instruments:
+            hpmap.meta['instruments'] = args.instruments
+        if args.enable_distance_map:
+            hpmap.meta['distmean'] = np.mean(dist)
+            hpmap.meta['diststd'] = np.std(dist)
 
-    keys = ['time', 'time_mean', 'time_maxl']
-    for key in keys:
-        try:
-            time = data[key]
-        except KeyError:
-            continue
+        keys = ['time', 'time_mean', 'time_maxl']
+        for key in keys:
+            try:
+                time = data[key]
+            except KeyError:
+                continue
+            else:
+                hpmap.meta['gps_time'] = time.mean()
+                break
         else:
-            hpmap.meta['gps_time'] = time.mean()
-            break
-    else:
-        log.warning(
-            'Cannot determine the event time from any of the columns %r', keys)
+            log.warning(
+                'Cannot determine the event time from any of the columns %r',
+                keys)
 
-    io.write_sky_map(os.path.join(args.outdir, args.fitsoutname),
-                     hpmap, nest=True)
+        io.write_sky_map(os.path.join(args.outdir, args.fitsoutname),
+                         hpmap, nest=True)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2011-2020  Leo Singer
+# Copyright (C) 2011-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -66,112 +66,113 @@
     parser.add_argument(
         'input', metavar='INPUT.fits[.gz]', type=FileType('rb'),
         default='-', nargs='?', help='Input FITS file')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
-
-    # Late imports
-
-    import numpy as np
-    import matplotlib.pyplot as plt
-    from matplotlib import rcParams
-    from ..io import fits
-    from .. import plot
-    from .. import postprocess
-    import astropy_healpix as ah
-    from astropy.coordinates import SkyCoord
-    from astropy.time import Time
-    from astropy import units as u
-
-    skymap, metadata = fits.read_sky_map(opts.input.name, nest=None)
-    nside = ah.npix_to_nside(len(skymap))
-
-    # Convert sky map from probability to probability per square degree.
-    deg2perpix = ah.nside_to_pixel_area(nside).to_value(u.deg**2)
-    probperdeg2 = skymap / deg2perpix
-
-    axes_args = {}
-    if opts.geo:
-        axes_args['projection'] = 'geo'
-        obstime = Time(metadata['gps_time'], format='gps').utc.isot
-        axes_args['obstime'] = obstime
-    else:
-        axes_args['projection'] = 'astro'
-    axes_args['projection'] += ' ' + opts.projection
-    if opts.projection_center is not None:
-        axes_args['center'] = SkyCoord(opts.projection_center)
-    if opts.zoom_radius is not None:
-        axes_args['radius'] = opts.zoom_radius
-    ax = plt.axes(**axes_args)
-    ax.grid()
-
-    # Plot sky map.
-    vmax = probperdeg2.max()
-    img = ax.imshow_hpx(
-        (probperdeg2, 'ICRS'), nested=metadata['nest'], vmin=0., vmax=vmax)
-
-    # Add colorbar.
-    if opts.colorbar:
-        cb = plot.colorbar(img)
-        cb.set_label(r'prob. per deg$^2$')
-
-    # Add contours.
-    if opts.contour:
-        cls = 100 * postprocess.find_greedy_credible_levels(skymap)
-        cs = ax.contour_hpx(
-            (cls, 'ICRS'), nested=metadata['nest'],
-            colors='k', linewidths=0.5, levels=opts.contour)
-        fmt = r'%g\%%' if rcParams['text.usetex'] else '%g%%'
-        plt.clabel(cs, fmt=fmt, fontsize=6, inline=True)
-
-    # Add continents.
-    if opts.geo:
-        plt.plot(*plot.coastlines(), color='0.5', linewidth=0.5,
-                 transform=ax.get_transform('world'))
-
-    radecs = opts.radec
-    if opts.inj_database:
-        query = '''SELECT DISTINCT longitude, latitude FROM sim_inspiral AS si
-                   INNER JOIN coinc_event_map AS cm1
-                   ON (si.simulation_id = cm1.event_id)
-                   INNER JOIN coinc_event_map AS cm2
-                   ON (cm1.coinc_event_id = cm2.coinc_event_id)
-                   WHERE cm2.event_id = ?
-                   AND cm1.table_name = 'sim_inspiral'
-                   AND cm2.table_name = 'coinc_event'
-                   '''
-        (ra, dec), = opts.inj_database.execute(
-            query, (metadata['objid'],)).fetchall()
-        radecs.append(np.rad2deg([ra, dec]).tolist())
-
-    # Add markers (e.g., for injections or external triggers).
-    for ra, dec in radecs:
-        ax.plot_coord(
-            SkyCoord(ra, dec, unit='deg'), '*',
-            markerfacecolor='white', markeredgecolor='black', markersize=10)
-
-    # Add a white outline to all text to make it stand out from the background.
-    plot.outline_text(ax)
-
-    if opts.annotate:
-        text = []
-        try:
-            objid = metadata['objid']
-        except KeyError:
-            pass
+    with parser().parse_args(args) as opts:
+        # Late imports
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from matplotlib import rcParams
+        from ..io import fits
+        from .. import plot
+        from .. import postprocess
+        import astropy_healpix as ah
+        from astropy.coordinates import SkyCoord
+        from astropy.time import Time
+        from astropy import units as u
+
+        skymap, metadata = fits.read_sky_map(opts.input.name, nest=None)
+        nside = ah.npix_to_nside(len(skymap))
+
+        # Convert sky map from probability to probability per square degree.
+        deg2perpix = ah.nside_to_pixel_area(nside).to_value(u.deg**2)
+        probperdeg2 = skymap / deg2perpix
+
+        axes_args = {}
+        if opts.geo:
+            axes_args['projection'] = 'geo'
+            obstime = Time(metadata['gps_time'], format='gps').utc.isot
+            axes_args['obstime'] = obstime
         else:
-            text.append('event ID: {}'.format(objid))
+            axes_args['projection'] = 'astro'
+        axes_args['projection'] += ' ' + opts.projection
+        if opts.projection_center is not None:
+            axes_args['center'] = SkyCoord(opts.projection_center)
+        if opts.zoom_radius is not None:
+            axes_args['radius'] = opts.zoom_radius
+        ax = plt.axes(**axes_args)
+        ax.grid()
+
+        # Plot sky map.
+        vmax = probperdeg2.max()
+        img = ax.imshow_hpx(
+            (probperdeg2, 'ICRS'), nested=metadata['nest'], vmin=0., vmax=vmax)
+
+        # Add colorbar.
+        if opts.colorbar:
+            cb = plot.colorbar(img)
+            cb.set_label(r'prob. per deg$^2$')
+
+        # Add contours.
         if opts.contour:
-            pp = np.round(opts.contour).astype(int)
-            ii = np.round(np.searchsorted(np.sort(cls), opts.contour) *
-                          deg2perpix).astype(int)
-            for i, p in zip(ii, pp):
-                # FIXME: use Unicode symbol instead of TeX '$^2$'
-                # because of broken fonts on Scientific Linux 7.
-                text.append('{:d}% area: {:,d} deg²'.format(p, i))
-        ax.text(1, 1, '\n'.join(text), transform=ax.transAxes, ha='right')
+            cls = 100 * postprocess.find_greedy_credible_levels(skymap)
+            cs = ax.contour_hpx(
+                (cls, 'ICRS'), nested=metadata['nest'],
+                colors='k', linewidths=0.5, levels=opts.contour)
+            fmt = r'%g\%%' if rcParams['text.usetex'] else '%g%%'
+            plt.clabel(cs, fmt=fmt, fontsize=6, inline=True)
+
+        # Add continents.
+        if opts.geo:
+            plt.plot(*plot.coastlines(), color='0.5', linewidth=0.5,
+                     transform=ax.get_transform('world'))
+
+        radecs = opts.radec
+        if opts.inj_database:
+            query = '''SELECT DISTINCT longitude, latitude
+                       FROM sim_inspiral AS si
+                       INNER JOIN coinc_event_map AS cm1
+                       ON (si.simulation_id = cm1.event_id)
+                       INNER JOIN coinc_event_map AS cm2
+                       ON (cm1.coinc_event_id = cm2.coinc_event_id)
+                       WHERE cm2.event_id = ?
+                       AND cm1.table_name = 'sim_inspiral'
+                       AND cm2.table_name = 'coinc_event'
+                    '''
+            (ra, dec), = opts.inj_database.execute(
+                query, (metadata['objid'],)).fetchall()
+            radecs.append(np.rad2deg([ra, dec]).tolist())
+
+        # Add markers (e.g., for injections or external triggers).
+        for ra, dec in radecs:
+            ax.plot_coord(
+                SkyCoord(ra, dec, unit='deg'), '*',
+                markerfacecolor='white', markeredgecolor='black',
+                markersize=10)
+
+        # Add a white outline to all text to make it stand out from the
+        # background.
+        plot.outline_text(ax)
+
+        if opts.annotate:
+            text = []
+            try:
+                objid = metadata['objid']
+            except KeyError:
+                pass
+            else:
+                text.append('event ID: {}'.format(objid))
+            if opts.contour:
+                pp = np.round(opts.contour).astype(int)
+                ii = np.round(np.searchsorted(np.sort(cls), opts.contour) *
+                              deg2perpix).astype(int)
+                for i, p in zip(ii, pp):
+                    # FIXME: use Unicode symbol instead of TeX '$^2$'
+                    # because of broken fonts on Scientific Linux 7.
+                    text.append('{:d}% area: {:,d} deg²'.format(p, i))
+            ax.text(1, 1, '\n'.join(text), transform=ax.transAxes, ha='right')
 
-    # Show or save output.
-    opts.output()
+        # Show or save output.
+        opts.output()
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_airmass.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_airmass.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_coherence.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_coherence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2011-2023  Leo Singer
+# Copyright (C) 2011-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -28,29 +28,27 @@
         'input', metavar='INPUT.fits[.gz]', type=FileType('rb'),
         default='-', nargs='?', help='Input FITS file')
     parser.set_defaults(colormap='RdYlBu')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
+    with parser().parse_args(args) as opts:
+        # Late imports
+        from astropy.io import fits
+        import numpy as np
+        from ..plot import plot_bayes_factor
+
+        header = fits.getheader(opts.input, 1)
+        logb = header['LOGBCI']
+        objid = header.get('OBJECT')
+
+        title = 'Coherence'
+        if objid:
+            title += f' of {objid}'
+        logb_string = np.format_float_positional(logb, 1, trim='0', sign=True)
+        title += fr' $[\ln\,B = {logb_string}]$'
 
-    # Late imports
+        plot_bayes_factor(logb, title=title, palette=opts.colormap)
 
-    from astropy.io import fits
-    import numpy as np
-    from ..plot import plot_bayes_factor
-
-    header = fits.getheader(opts.input, 1)
-    logb = header['LOGBCI']
-    objid = header.get('OBJECT')
-
-    title = 'Coherence'
-    if objid:
-        title += f' of {objid}'
-    logb_string = np.format_float_positional(logb, 1, trim='0', sign=True)
-    title += fr' $[\ln\,B = {logb_string}]$'
-
-    plot_bayes_factor(logb, title=title, palette=opts.colormap)
-
-    # Show or save output.
-    opts.output()
+        # Show or save output.
+        opts.output()
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_observability.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_observability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2019-2020  Leo Singer
+# Copyright (C) 2019-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -65,84 +65,85 @@
     which we map to infinite airmass.
     """
     return np.where(x <= 0, np.inf, x)
 
 
 def main(args=None):
     p = parser()
-    opts = p.parse_args(args)
+    with p.parse_args(args) as opts:
+        # Late imports
+        from astroplan import (
+            AirmassConstraint, AtNightConstraint, Observer,
+            is_event_observable)
+        from astropy.coordinates import EarthLocation, SkyCoord
+        from astropy.time import Time
+        from astropy import units as u
+        from matplotlib import dates
+        from matplotlib import pyplot as plt
+        from tqdm import tqdm
+
+        from ..io import fits
+        from .. import moc
+        from .. import plot  # noqa
+
+        names = ('name', 'longitude', 'latitude', 'height')
+        length0, *lengths = (
+            len(getattr(opts, 'site_{}'.format(name))) for name in names)
+        if not all(length0 == length for length in lengths):
+            p.error(
+                'these options require equal numbers of arguments: {}'.format(
+                    ', '.join('--site-{}'.format(name) for name in names)))
+
+        observers = [Observer.at_site(site) for site in opts.site]
+        for name, lon, lat, height in zip(
+                opts.site_name, opts.site_longitude, opts.site_latitude,
+                opts.site_height):
+            location = EarthLocation(
+                lon=lon * u.deg,
+                lat=lat * u.deg,
+                height=(height or 0) * u.m)
+            observers.append(Observer(location, name=name))
+        observers = list(reversed(observers))
+
+        m = fits.read_sky_map(opts.input.name, moc=True)
+
+        t0 = Time(opts.time) if opts.time is not None else Time.now()
+        times = t0 + np.linspace(0, 1) * u.day
+
+        theta, phi = moc.uniq2ang(m['UNIQ'])
+        coords = SkyCoord(phi, 0.5 * np.pi - theta, unit='rad')
+        prob = np.asarray(moc.uniq2pixarea(m['UNIQ']) * m['PROBDENSITY'])
+
+        constraints = [
+            getattr(AtNightConstraint, 'twilight_{}'.format(opts.twilight))(),
+            AirmassConstraint(opts.max_airmass)]
+
+        fig = plt.figure()
+        width, height = fig.get_size_inches()
+        fig.set_size_inches(width, (len(observers) + 1) / 16 * width)
+        ax = plt.axes()
+        locator = dates.AutoDateLocator()
+        formatter = dates.DateFormatter('%H:%M')
+        ax.set_xlim([times[0].plot_date, times[-1].plot_date])
+        ax.xaxis.set_major_formatter(formatter)
+        ax.xaxis.set_major_locator(locator)
+        ax.set_xlabel("Time from {0} [UTC]".format(min(times).datetime.date()))
+        plt.setp(ax.get_xticklabels(), rotation=30, ha='right')
+        ax.set_yticks(np.arange(len(observers)))
+        ax.set_yticklabels([observer.name for observer in observers])
+        ax.yaxis.set_tick_params(left=False)
+        ax.grid(axis='x')
+        ax.spines['bottom'].set_visible(False)
+        ax.spines['top'].set_visible(False)
+
+        for i, observer in enumerate(tqdm(observers)):
+            observable = 100 * np.dot(prob, is_event_observable(
+                constraints, observer, coords, times))
+            ax.contourf(
+                times.plot_date, [i - 0.4, i + 0.4],
+                np.tile(observable, (2, 1)), levels=np.arange(10, 110, 10),
+                cmap=plt.get_cmap().reversed())
 
-    # Late imports
-    from astroplan import (
-        AirmassConstraint, AtNightConstraint, Observer, is_event_observable)
-    from astropy.coordinates import EarthLocation, SkyCoord
-    from astropy.time import Time
-    from astropy import units as u
-    from matplotlib import dates
-    from matplotlib import pyplot as plt
-    from tqdm import tqdm
-
-    from ..io import fits
-    from .. import moc
-    from .. import plot  # noqa
-
-    names = ('name', 'longitude', 'latitude', 'height')
-    length0, *lengths = (
-        len(getattr(opts, 'site_{}'.format(name))) for name in names)
-    if not all(length0 == length for length in lengths):
-        p.error('these options require equal numbers of arguments: {}'.format(
-            ', '.join(
-                '--site-{}'.format(name) for name in names)))
-
-    observers = [Observer.at_site(site) for site in opts.site]
-    for name, lon, lat, height in zip(
-            opts.site_name, opts.site_longitude, opts.site_latitude,
-            opts.site_height):
-        location = EarthLocation(
-            lon=lon * u.deg,
-            lat=lat * u.deg,
-            height=(height or 0) * u.m)
-        observers.append(Observer(location, name=name))
-    observers = list(reversed(observers))
-
-    m = fits.read_sky_map(opts.input.name, moc=True)
-
-    t0 = Time(opts.time) if opts.time is not None else Time.now()
-    times = t0 + np.linspace(0, 1) * u.day
-
-    theta, phi = moc.uniq2ang(m['UNIQ'])
-    coords = SkyCoord(phi, 0.5 * np.pi - theta, unit='rad')
-    prob = np.asarray(moc.uniq2pixarea(m['UNIQ']) * m['PROBDENSITY'])
-
-    constraints = [
-        getattr(AtNightConstraint, 'twilight_{}'.format(opts.twilight))(),
-        AirmassConstraint(opts.max_airmass)]
-
-    fig = plt.figure()
-    width, height = fig.get_size_inches()
-    fig.set_size_inches(width, (len(observers) + 1) / 16 * width)
-    ax = plt.axes()
-    locator = dates.AutoDateLocator()
-    formatter = dates.DateFormatter('%H:%M')
-    ax.set_xlim([times[0].plot_date, times[-1].plot_date])
-    ax.xaxis.set_major_formatter(formatter)
-    ax.xaxis.set_major_locator(locator)
-    ax.set_xlabel("Time from {0} [UTC]".format(min(times).datetime.date()))
-    plt.setp(ax.get_xticklabels(), rotation=30, ha='right')
-    ax.set_yticks(np.arange(len(observers)))
-    ax.set_yticklabels([observer.name for observer in observers])
-    ax.yaxis.set_tick_params(left=False)
-    ax.grid(axis='x')
-    ax.spines['bottom'].set_visible(False)
-    ax.spines['top'].set_visible(False)
-
-    for i, observer in enumerate(tqdm(observers)):
-        observable = 100 * np.dot(prob, is_event_observable(
-            constraints, observer, coords, times))
-        ax.contourf(
-            times.plot_date, [i - 0.4, i + 0.4], np.tile(observable, (2, 1)),
-            levels=np.arange(10, 110, 10), cmap=plt.get_cmap().reversed())
+        plt.tight_layout()
 
-    plt.tight_layout()
-
-    # Show or save output.
-    opts.output()
+        # Show or save output.
+        opts.output()
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_pp_samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2017-2019  Leo Singer
+# Copyright (C) 2017-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -52,77 +52,78 @@
         metavar='PERCENT',
         help='Report the areas and volumes within the smallest contours '
         'containing this much probability.')
     return parser
 
 
 def main(args=None):
-    args = parser().parse_args(args)
-
-    # Late imports.
-    from astropy.table import Table
-    from matplotlib import pyplot as plt
-    from scipy.interpolate import interp1d
-    from .. import io
-    from .. import plot as _  # noqa: F401
-    from ..postprocess import find_injection_moc
-
-    # Read input.
-    skymap = io.read_sky_map(args.skymap.name, moc=True)
-    chain = io.read_samples(args.samples.name)
-
-    # If required, downselect to a smaller number of posterior samples.
-    if args.max_points is not None:
-        chain = Table(np.random.permutation(chain)[:args.max_points],
-                      copy=False)
-
-    # Calculate P-P plot.
-    contours = np.asarray(args.contour)
-    result = find_injection_moc(skymap,
-                                chain['ra'], chain['dec'], chain['dist'],
-                                contours=1e-2 * contours)
-
-    # Make Matplotlib figure.
-    fig = plt.figure(figsize=(6, 6))
-    ax = fig.add_subplot(111, projection='pp_plot')
-    ax.add_diagonal()
-    ax.add_series(result.searched_prob, label='R.A., Dec.')
-    searched_area_func = interp1d(np.linspace(0, 1, len(chain)),
-                                  np.sort(result.searched_area),
-                                  bounds_error=False)
-    if 'DISTMU' in skymap.colnames:
-        ax.add_series(result.searched_prob_dist, label='Distance')
-        ax.add_series(result.searched_prob_vol, label='Volume')
-        searched_vol_func = interp1d(np.linspace(0, 1, len(chain)),
-                                     np.sort(result.searched_vol),
-                                     bounds_error=False)
-    for p, area, vol in zip(
-            args.contour, result.contour_areas, result.contour_vols):
-        text = '{:g}%\n{} deg$^2$'.format(p, fmt(area, 2))
-        if 'DISTMU' in skymap.colnames:
-            text += '\n{} Mpc$^3$'.format(fmt(vol, 2, force_scientific=True))
-        ax.annotate(
-            text, (1e-2 * p, 1e-2 * p), (0, -150),
-            xycoords='data', textcoords='offset points',
-            horizontalalignment='right', backgroundcolor='white',
-            arrowprops=dict(connectionstyle='bar,angle=0,fraction=0',
-                            arrowstyle='-|>', linewidth=2, color='black'))
-        area = searched_area_func(1e-2 * p)
-        text = '{:g}%\n{} deg$^2$'.format(p, fmt(area, 2))
+    with parser().parse_args(args) as args:
+        # Late imports.
+        from astropy.table import Table
+        from matplotlib import pyplot as plt
+        from scipy.interpolate import interp1d
+        from .. import io
+        from .. import plot as _  # noqa: F401
+        from ..postprocess import find_injection_moc
+
+        # Read input.
+        skymap = io.read_sky_map(args.skymap.name, moc=True)
+        chain = io.read_samples(args.samples.name)
+
+        # If required, downselect to a smaller number of posterior samples.
+        if args.max_points is not None:
+            chain = Table(np.random.permutation(chain)[:args.max_points],
+                          copy=False)
+
+        # Calculate P-P plot.
+        contours = np.asarray(args.contour)
+        result = find_injection_moc(skymap,
+                                    chain['ra'], chain['dec'], chain['dist'],
+                                    contours=1e-2 * contours)
+
+        # Make Matplotlib figure.
+        fig = plt.figure(figsize=(6, 6))
+        ax = fig.add_subplot(111, projection='pp_plot')
+        ax.add_diagonal()
+        ax.add_series(result.searched_prob, label='R.A., Dec.')
+        searched_area_func = interp1d(np.linspace(0, 1, len(chain)),
+                                      np.sort(result.searched_area),
+                                      bounds_error=False)
         if 'DISTMU' in skymap.colnames:
-            vol = searched_vol_func(1e-2 * p)
-            text += '\n{} Mpc$^3$'.format(fmt(vol, 2, force_scientific=True))
-        ax.annotate(
-            text, (1e-2 * p, 1e-2 * p), (-75, 0),
-            xycoords='data', textcoords='offset points',
-            horizontalalignment='right', verticalalignment='center',
-            backgroundcolor='white',
-            arrowprops=dict(connectionstyle='bar,angle=0,fraction=0',
-                            arrowstyle='-|>', linewidth=2, color='black'))
-    ax.set_xlabel('searched probability')
-    ax.set_ylabel('cumulative fraction of posterior samples')
-    ax.set_title(args.skymap.name)
-    ax.legend()
-    ax.grid()
+            ax.add_series(result.searched_prob_dist, label='Distance')
+            ax.add_series(result.searched_prob_vol, label='Volume')
+            searched_vol_func = interp1d(np.linspace(0, 1, len(chain)),
+                                         np.sort(result.searched_vol),
+                                         bounds_error=False)
+        for p, area, vol in zip(
+                args.contour, result.contour_areas, result.contour_vols):
+            text = '{:g}%\n{} deg$^2$'.format(p, fmt(area, 2))
+            if 'DISTMU' in skymap.colnames:
+                text += '\n{} Mpc$^3$'.format(
+                    fmt(vol, 2, force_scientific=True))
+            ax.annotate(
+                text, (1e-2 * p, 1e-2 * p), (0, -150),
+                xycoords='data', textcoords='offset points',
+                horizontalalignment='right', backgroundcolor='white',
+                arrowprops=dict(connectionstyle='bar,angle=0,fraction=0',
+                                arrowstyle='-|>', linewidth=2, color='black'))
+            area = searched_area_func(1e-2 * p)
+            text = '{:g}%\n{} deg$^2$'.format(p, fmt(area, 2))
+            if 'DISTMU' in skymap.colnames:
+                vol = searched_vol_func(1e-2 * p)
+                text += '\n{} Mpc$^3$'.format(
+                    fmt(vol, 2, force_scientific=True))
+            ax.annotate(
+                text, (1e-2 * p, 1e-2 * p), (-75, 0),
+                xycoords='data', textcoords='offset points',
+                horizontalalignment='right', verticalalignment='center',
+                backgroundcolor='white',
+                arrowprops=dict(connectionstyle='bar,angle=0,fraction=0',
+                                arrowstyle='-|>', linewidth=2, color='black'))
+        ax.set_xlabel('searched probability')
+        ax.set_ylabel('cumulative fraction of posterior samples')
+        ax.set_title(args.skymap.name)
+        ax.legend()
+        ax.grid()
 
-    # Show or save output.
-    args.output()
+        # Show or save output.
+        args.output()
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_stats.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2023  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -44,173 +44,175 @@
         help='Name of input file generated by ligo-skymap-stats')
     parser.add_argument(
         '--output', '-o', default='.', help='output directory')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
-
-    # Imports.
-    from astropy.table import Table
-    import matplotlib
-    matplotlib.use('agg')
-    from matplotlib import pyplot as plt
-    from matplotlib import rcParams
-    import numpy as np
-    from tqdm import tqdm
-    from .. import plot  # noqa
-
-    # Read in all of the datasets listed as positional command line arguments.
-    datasets = [Table.read(file, format='ascii') for file in opts.input]
-
-    # Determine plot colors and labels
-    filenames = [file.name for file in opts.input]
-    labels = [os.path.splitext(os.path.basename(f))[0] for f in filenames]
-    if rcParams['text.usetex']:
-        labels = [r'\verb/' + label + '/' for label in labels]
-    rcParams['savefig.format'] = opts.format
-    metadata = MatplotlibFigureType.get_savefig_metadata(opts.format)
-
-    # Normalize column names
-    for dataset in datasets:
-        if 'p_value' in dataset.colnames:
-            dataset.rename_column('p_value', 'searched_prob')
-
-    if opts.group_by == 'far':
-
-        def key_func(table):
-            return -np.log10(table['far'])
-
-        def key_to_dir(key):
-            return 'far_1e{}'.format(-key)
-
-        def key_to_title(key):
-            return r'$\mathrm{{FAR}} \leq 10^{{{}}}$ Hz'.format(-key)
-
-    elif opts.group_by == 'snr':
-
-        def key_func(table):
-            return table['snr']
-
-        def key_to_dir(key):
-            return 'snr_{}'.format(key)
-
-        def key_to_title(key):
-            return r'$\mathrm{{SNR}} \geq {}$'.format(key)
-
-    else:
-
-        def key_func(table):
-            return np.zeros(len(table))
-
-        def key_to_dir(key):
-            return '.'
-
-        def key_to_title(key):
-            return 'All events'
-
-    if opts.group_by is not None:
-        missing = [filename for filename, dataset in zip(filenames, datasets)
-                   if opts.group_by not in dataset.colnames]
-        if missing:
-            raise RuntimeError(
-                'The following files had no "'
-                + opts.group_by + '" column: ' + ' '.join(missing))
-
-    for dataset in datasets:
-        dataset['key'] = key_func(dataset)
-
-    if opts.group_by is not None:
-        invalid = [filename for filename, dataset in zip(filenames, datasets)
-                   if not np.all(np.isfinite(dataset['key']))]
-        if invalid:
-            raise RuntimeError(
-                'The following files had invalid values in the "'
-                + opts.group_by + '" column: ' + ' '.join(invalid))
-
-    keys = np.concatenate([dataset['key'] for dataset in datasets])
-
-    histlabel = []
-    if opts.cumulative:
-        histlabel.append('cumulative')
-    if opts.normed:
-        histlabel.append('fraction')
-    else:
-        histlabel.append('number')
-    histlabel.append('of injections')
-    histlabel = ' '.join(histlabel)
-
-    pp_plot_settings = [
-        ['', 'searched posterior mass'],
-        ['_dist', 'distance CDF at true distance'],
-        ['_vol', 'searched volumetric probability']]
-    hist_settings = [
-        ['searched_area', 'searched_area (deg$^2$)'],
-        ['searched_vol', 'searched volume (Mpc$^3$)'],
-        ['offset', 'angle from true location and mode of posterior (deg)'],
-        ['runtime', 'run time (s)']]
-
-    keys = range(*np.floor([keys.min(), keys.max()+1]).astype(int))
-    total = len(keys) * (len(pp_plot_settings) + len(hist_settings))
-    with tqdm(total=total) as progress:
-        for key in keys:
-            filtered = [d[d['key'] >= key] for d in datasets]
-            title = key_to_title(key)
-            nsamples = {len(d) for d in filtered}
-            if len(nsamples) == 1:
-                nsamples, = nsamples
-                title += ' ({} events)'.format(nsamples)
-            else:
-                nsamples = None
-
-            subdir = os.path.join(opts.output, key_to_dir(key))
-            os.makedirs(subdir, exist_ok=True)
-
-            # Make several different kinds of P-P plots
-            for suffix, xlabel in pp_plot_settings:
-                colname = 'searched_prob' + suffix
-                fig = plt.figure(figsize=(6, 6))
-                ax = fig.add_subplot(111, projection='pp_plot')
-                fig.subplots_adjust(bottom=0.15)
-                ax.set_xlabel(xlabel)
-                ax.set_ylabel('cumulative fraction of injections')
-                ax.set_title(title)
-                for d, label in zip(filtered, labels):
-                    ax.add_series(d.columns.get(colname, []), label=label)
-                ax.add_diagonal()
-                if nsamples:
-                    ax.add_confidence_band(
-                        nsamples, 0.01 * opts.pp_confidence_interval)
-                ax.grid()
-                if len(filtered) > 1:
-                    ax.legend(loc='lower right')
-                fig.savefig(os.path.join(subdir, colname),
-                            metadata=metadata)
-                plt.close()
-                progress.update()
-
-            # Make several different kinds of histograms
-            for colname, xlabel in hist_settings:
-                fig = plt.figure(figsize=(6, 4.5))
-                ax = fig.add_subplot(111)
-                fig.subplots_adjust(bottom=0.15)
-                ax.set_xscale('log')
-                ax.set_xlabel(xlabel)
-                ax.set_ylabel(histlabel)
-                ax.set_title(title)
-                values = np.concatenate(
-                    [d.columns.get(colname, []) for d in filtered])
-                if len(values) > 0:
-                    bins = np.geomspace(np.min(values), np.max(values),
-                                        1000 if opts.cumulative else 20)
+    with parser().parse_args(args) as opts:
+        # Imports.
+        from astropy.table import Table
+        import matplotlib
+        matplotlib.use('agg')
+        from matplotlib import pyplot as plt
+        from matplotlib import rcParams
+        import numpy as np
+        from tqdm import tqdm
+        from .. import plot  # noqa
+
+        # Read in all of the datasets listed as positional command line
+        # arguments.
+        datasets = [Table.read(file, format='ascii') for file in opts.input]
+
+        # Determine plot colors and labels
+        filenames = [file.name for file in opts.input]
+        labels = [os.path.splitext(os.path.basename(f))[0] for f in filenames]
+        if rcParams['text.usetex']:
+            labels = [r'\verb/' + label + '/' for label in labels]
+        rcParams['savefig.format'] = opts.format
+        metadata = MatplotlibFigureType.get_savefig_metadata(opts.format)
+
+        # Normalize column names
+        for dataset in datasets:
+            if 'p_value' in dataset.colnames:
+                dataset.rename_column('p_value', 'searched_prob')
+
+        if opts.group_by == 'far':
+
+            def key_func(table):
+                return -np.log10(table['far'])
+
+            def key_to_dir(key):
+                return 'far_1e{}'.format(-key)
+
+            def key_to_title(key):
+                return r'$\mathrm{{FAR}} \leq 10^{{{}}}$ Hz'.format(-key)
+
+        elif opts.group_by == 'snr':
+
+            def key_func(table):
+                return table['snr']
+
+            def key_to_dir(key):
+                return 'snr_{}'.format(key)
+
+            def key_to_title(key):
+                return r'$\mathrm{{SNR}} \geq {}$'.format(key)
+
+        else:
+
+            def key_func(table):
+                return np.zeros(len(table))
+
+            def key_to_dir(key):
+                return '.'
+
+            def key_to_title(key):
+                return 'All events'
+
+        if opts.group_by is not None:
+            missing = [filename for filename, dataset
+                       in zip(filenames, datasets)
+                       if opts.group_by not in dataset.colnames]
+            if missing:
+                raise RuntimeError(
+                    'The following files had no "'
+                    + opts.group_by + '" column: ' + ' '.join(missing))
+
+        for dataset in datasets:
+            dataset['key'] = key_func(dataset)
+
+        if opts.group_by is not None:
+            invalid = [filename for filename, dataset
+                       in zip(filenames, datasets)
+                       if not np.all(np.isfinite(dataset['key']))]
+            if invalid:
+                raise RuntimeError(
+                    'The following files had invalid values in the "'
+                    + opts.group_by + '" column: ' + ' '.join(invalid))
+
+        keys = np.concatenate([dataset['key'] for dataset in datasets])
+
+        histlabel = []
+        if opts.cumulative:
+            histlabel.append('cumulative')
+        if opts.normed:
+            histlabel.append('fraction')
+        else:
+            histlabel.append('number')
+        histlabel.append('of injections')
+        histlabel = ' '.join(histlabel)
+
+        pp_plot_settings = [
+            ['', 'searched posterior mass'],
+            ['_dist', 'distance CDF at true distance'],
+            ['_vol', 'searched volumetric probability']]
+        hist_settings = [
+            ['searched_area', 'searched_area (deg$^2$)'],
+            ['searched_vol', 'searched volume (Mpc$^3$)'],
+            ['offset', 'angle from true location and mode of posterior (deg)'],
+            ['runtime', 'run time (s)']]
+
+        keys = range(*np.floor([keys.min(), keys.max()+1]).astype(int))
+        total = len(keys) * (len(pp_plot_settings) + len(hist_settings))
+        with tqdm(total=total) as progress:
+            for key in keys:
+                filtered = [d[d['key'] >= key] for d in datasets]
+                title = key_to_title(key)
+                nsamples = {len(d) for d in filtered}
+                if len(nsamples) == 1:
+                    nsamples, = nsamples
+                    title += ' ({} events)'.format(nsamples)
+                else:
+                    nsamples = None
+
+                subdir = os.path.join(opts.output, key_to_dir(key))
+                os.makedirs(subdir, exist_ok=True)
+
+                # Make several different kinds of P-P plots
+                for suffix, xlabel in pp_plot_settings:
+                    colname = 'searched_prob' + suffix
+                    fig = plt.figure(figsize=(6, 6))
+                    ax = fig.add_subplot(111, projection='pp_plot')
+                    fig.subplots_adjust(bottom=0.15)
+                    ax.set_xlabel(xlabel)
+                    ax.set_ylabel('cumulative fraction of injections')
+                    ax.set_title(title)
                     for d, label in zip(filtered, labels):
-                        ax.hist(d.columns.get(colname, []),
-                                cumulative=opts.cumulative,
-                                density=opts.normed, histtype='step',
-                                bins=bins, label=label)
-                ax.grid()
-                ax.legend(loc='upper left')
-                fig.savefig(os.path.join(subdir, colname + '_hist'),
-                            metadata=metadata)
-                plt.close()
-                progress.update()
+                        ax.add_series(d.columns.get(colname, []), label=label)
+                    ax.add_diagonal()
+                    if nsamples:
+                        ax.add_confidence_band(
+                            nsamples, 0.01 * opts.pp_confidence_interval)
+                    ax.grid()
+                    if len(filtered) > 1:
+                        ax.legend(loc='lower right')
+                    fig.savefig(os.path.join(subdir, colname),
+                                metadata=metadata)
+                    plt.close()
+                    progress.update()
+
+                # Make several different kinds of histograms
+                for colname, xlabel in hist_settings:
+                    fig = plt.figure(figsize=(6, 4.5))
+                    ax = fig.add_subplot(111)
+                    fig.subplots_adjust(bottom=0.15)
+                    ax.set_xscale('log')
+                    ax.set_xlabel(xlabel)
+                    ax.set_ylabel(histlabel)
+                    ax.set_title(title)
+                    values = np.concatenate(
+                        [d.columns.get(colname, []) for d in filtered])
+                    if len(values) > 0:
+                        bins = np.geomspace(np.min(values), np.max(values),
+                                            1000 if opts.cumulative else 20)
+                        for d, label in zip(filtered, labels):
+                            ax.hist(d.columns.get(colname, []),
+                                    cumulative=opts.cumulative,
+                                    density=opts.normed, histtype='step',
+                                    bins=bins, label=label)
+                    ax.grid()
+                    ax.legend(loc='upper left')
+                    fig.savefig(os.path.join(subdir, colname + '_hist'),
+                                metadata=metadata)
+                    plt.close()
+                    progress.update()
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_plot_volume.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_plot_volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,203 +49,206 @@
         '--align-to', metavar='SKYMAP.fits[.gz]', type=FileType('rb'),
         help='Align to the principal axes of this sky map')
     parser.set_defaults(figure_width='3.5', figure_height='3.5')
     return parser
 
 
 def main(args=None):
-    opts = parser().parse_args(args)
+    with parser().parse_args(args) as opts:
+        # Create progress bar.
+        from tqdm import tqdm
+        progress = tqdm()
+        progress.set_description('Starting up')
+
+        # Late imports
+        import astropy_healpix as ah
+        from matplotlib import pyplot as plt
+        from matplotlib import gridspec
+        from matplotlib import transforms
+        from .. import io
+        from ..plot import marker
+        from ..distance import (parameters_to_marginal_moments,
+                                principal_axes, volume_render, marginal_pdf)
+        import healpy as hp
+        import numpy as np
+        import scipy.stats
+
+        # Read input, determine input resolution.
+        progress.set_description('Loading FITS file')
+        (prob, mu, sigma, norm), metadata = io.read_sky_map(
+            opts.input.name, distances=True)
+        npix = len(prob)
+        nside = ah.npix_to_nside(npix)
+
+        progress.set_description('Preparing projection')
+
+        if opts.align_to is None or opts.input.name == opts.align_to.name:
+            prob2, mu2, sigma2, norm2 = prob, mu, sigma, norm
+        else:
+            (prob2, mu2, sigma2, norm2), _ = io.read_sky_map(
+                opts.align_to.name, distances=True)
+        if opts.max_distance is None:
+            mean, std = parameters_to_marginal_moments(prob2, mu2, sigma2)
+            max_distance = mean + 2.5 * std
+        else:
+            max_distance = opts.max_distance
+        rot = np.ascontiguousarray(principal_axes(prob2, mu2, sigma2))
 
-    # Create progress bar.
-    from tqdm import tqdm
-    progress = tqdm()
-    progress.set_description('Starting up')
-
-    # Late imports
-    import astropy_healpix as ah
-    from matplotlib import pyplot as plt
-    from matplotlib import gridspec
-    from matplotlib import transforms
-    from .. import io
-    from ..plot import marker
-    from ..distance import (parameters_to_marginal_moments, principal_axes,
-                            volume_render, marginal_pdf)
-    import healpy as hp
-    import numpy as np
-    import scipy.stats
-
-    # Read input, determine input resolution.
-    progress.set_description('Loading FITS file')
-    (prob, mu, sigma, norm), metadata = io.read_sky_map(
-        opts.input.name, distances=True)
-    npix = len(prob)
-    nside = ah.npix_to_nside(npix)
-
-    progress.set_description('Preparing projection')
-
-    if opts.align_to is None or opts.input.name == opts.align_to.name:
-        prob2, mu2, sigma2, norm2 = prob, mu, sigma, norm
-    else:
-        (prob2, mu2, sigma2, norm2), _ = io.read_sky_map(
-            opts.align_to.name, distances=True)
-    if opts.max_distance is None:
-        mean, std = parameters_to_marginal_moments(prob2, mu2, sigma2)
-        max_distance = mean + 2.5 * std
-    else:
-        max_distance = opts.max_distance
-    rot = np.ascontiguousarray(principal_axes(prob2, mu2, sigma2))
-
-    if opts.chain:
-        chain = io.read_samples(opts.chain.name)
-        chain = np.dot(rot.T, (hp.ang2vec(
-            0.5 * np.pi - chain['dec'], chain['ra']) *
-            np.atleast_2d(chain['dist']).T).T)
-
-    fig = plt.figure()
-    n = 1 if opts.projection else 2
-    gs = gridspec.GridSpec(
-        n, n, left=0.01, right=0.99, bottom=0.01, top=0.99,
-        wspace=0.05, hspace=0.05)
-
-    imgwidth = int(opts.dpi * opts.figure_width / n)
-    s = np.linspace(-max_distance, max_distance, imgwidth)
-    xx, yy = np.meshgrid(s, s)
-
-    truth_marker = marker.reticle(
-        inner=0.5 * np.sqrt(2), outer=1.5 * np.sqrt(2), angle=45)
-
-    for iface, (axis0, axis1, (sp0, sp1)) in enumerate((
-            (1, 0, [0, 0]),
-            (0, 2, [1, 1]),
-            (1, 2, [1, 0]),)):
-
-        if opts.projection and opts.projection != iface + 1:
-            continue
-
-        progress.set_description('Plotting projection {0}'.format(iface + 1))
-
-        # Marginalize onto the given face
-        density = volume_render(
-            xx.ravel(), yy.ravel(), max_distance, axis0, axis1, rot, False,
-            prob, mu, sigma, norm).reshape(xx.shape)
-
-        # Plot heat map
-        ax = fig.add_subplot(
-            gs[0, 0] if opts.projection else gs[sp0, sp1], aspect=1)
-        ax.imshow(
-            density, origin='lower',
-            extent=[-max_distance, max_distance, -max_distance, max_distance],
-            cmap=opts.colormap)
+        if opts.chain:
+            chain = io.read_samples(opts.chain.name)
+            chain = np.dot(rot.T, (hp.ang2vec(
+                0.5 * np.pi - chain['dec'], chain['ra']) *
+                np.atleast_2d(chain['dist']).T).T)
+
+        fig = plt.figure()
+        n = 1 if opts.projection else 2
+        gs = gridspec.GridSpec(
+            n, n, left=0.01, right=0.99, bottom=0.01, top=0.99,
+            wspace=0.05, hspace=0.05)
+
+        imgwidth = int(opts.dpi * opts.figure_width / n)
+        s = np.linspace(-max_distance, max_distance, imgwidth)
+        xx, yy = np.meshgrid(s, s)
+
+        truth_marker = marker.reticle(
+            inner=0.5 * np.sqrt(2), outer=1.5 * np.sqrt(2), angle=45)
+
+        for iface, (axis0, axis1, (sp0, sp1)) in enumerate((
+                (1, 0, [0, 0]),
+                (0, 2, [1, 1]),
+                (1, 2, [1, 0]),)):
+
+            if opts.projection and opts.projection != iface + 1:
+                continue
+
+            progress.set_description(
+                'Plotting projection {0}'.format(iface + 1))
+
+            # Marginalize onto the given face
+            density = volume_render(
+                xx.ravel(), yy.ravel(), max_distance, axis0, axis1, rot, False,
+                prob, mu, sigma, norm).reshape(xx.shape)
+
+            # Plot heat map
+            ax = fig.add_subplot(
+                gs[0, 0] if opts.projection else gs[sp0, sp1], aspect=1)
+            ax.imshow(
+                density, origin='lower',
+                extent=[-max_distance, max_distance,
+                        -max_distance, max_distance],
+                cmap=opts.colormap)
+
+            # Add contours if requested
+            if opts.contour:
+                flattened_density = density.ravel()
+                indices = np.argsort(flattened_density)[::-1]
+                cumsum = np.empty_like(flattened_density)
+                cs = np.cumsum(flattened_density[indices])
+                cumsum[indices] = cs / cs[-1] * 100
+                cumsum = np.reshape(cumsum, density.shape)
+                u, v = np.meshgrid(s, s)
+                contourset = ax.contour(
+                    u, v, cumsum, levels=opts.contour, linewidths=0.5)
+
+            # Mark locations
+            ax._get_lines.get_next_color()  # skip default color
+            for ra, dec, dist in opts.radecdist:
+                theta = 0.5 * np.pi - np.deg2rad(dec)
+                phi = np.deg2rad(ra)
+                xyz = np.dot(rot.T, hp.ang2vec(theta, phi) * dist)
+                ax.plot(
+                    xyz[axis0], xyz[axis1], marker=truth_marker,
+                    markerfacecolor='none', markeredgewidth=1)
+
+            # Plot chain
+            if opts.chain:
+                ax.plot(chain[axis0], chain[axis1], '.k', markersize=0.5)
+
+            # Hide axes ticks
+            ax.set_xticks([])
+            ax.set_yticks([])
+
+            # Set axis limits
+            ax.set_xlim([-max_distance, max_distance])
+            ax.set_ylim([-max_distance, max_distance])
 
-        # Add contours if requested
-        if opts.contour:
-            flattened_density = density.ravel()
-            indices = np.argsort(flattened_density)[::-1]
-            cumsum = np.empty_like(flattened_density)
-            cs = np.cumsum(flattened_density[indices])
-            cumsum[indices] = cs / cs[-1] * 100
-            cumsum = np.reshape(cumsum, density.shape)
-            u, v = np.meshgrid(s, s)
-            contourset = ax.contour(
-                u, v, cumsum, levels=opts.contour, linewidths=0.5)
-
-        # Mark locations
-        ax._get_lines.get_next_color()  # skip default color
-        for ra, dec, dist in opts.radecdist:
-            theta = 0.5 * np.pi - np.deg2rad(dec)
-            phi = np.deg2rad(ra)
-            xyz = np.dot(rot.T, hp.ang2vec(theta, phi) * dist)
+            # Mark origin (Earth)
             ax.plot(
-                xyz[axis0], xyz[axis1], marker=truth_marker,
-                markerfacecolor='none', markeredgewidth=1)
+                [0], [0], marker=marker.earth, markersize=5,
+                markerfacecolor='none', markeredgecolor='black',
+                markeredgewidth=0.75)
 
-        # Plot chain
-        if opts.chain:
-            ax.plot(chain[axis0], chain[axis1], '.k', markersize=0.5)
+            if iface == 2:
+                ax.invert_xaxis()
 
-        # Hide axes ticks
-        ax.set_xticks([])
-        ax.set_yticks([])
-
-        # Set axis limits
-        ax.set_xlim([-max_distance, max_distance])
-        ax.set_ylim([-max_distance, max_distance])
-
-        # Mark origin (Earth)
-        ax.plot(
-            [0], [0], marker=marker.earth, markersize=5,
-            markerfacecolor='none', markeredgecolor='black',
-            markeredgewidth=0.75)
-
-        if iface == 2:
-            ax.invert_xaxis()
-
-    # Add contour labels if contours requested
-    if opts.contour:
-        ax.clabel(contourset, fmt='%d%%', fontsize=7)
-
-    if not opts.projection:
-        # Add scale bar, 1/4 width of the plot
-        ax.plot(
-            [0.0625, 0.3125], [0.0625, 0.0625],
-            color='black', linewidth=1, transform=ax.transAxes)
-        ax.text(
-            0.0625, 0.0625,
-            '{0:d} Mpc'.format(int(np.round(0.5 * max_distance))),
-            fontsize=8, transform=ax.transAxes, verticalalignment='bottom')
-
-        # Create marginal distance plot.
-        progress.set_description('Plotting distance')
-        gs1 = gridspec.GridSpecFromSubplotSpec(5, 5, gs[0, 1])
-        ax = fig.add_subplot(gs1[1:-1, 1:-1])
-
-        # Plot marginal distance distribution, integrated over the whole sky.
-        d = np.linspace(0, max_distance)
-        ax.fill_between(d, marginal_pdf(d, prob, mu, sigma, norm),
-                        alpha=0.5, color=ax._get_lines.get_next_color())
-
-        # Plot conditional distance distribution at true position
-        # and mark true distance.
-        for ra, dec, dist in opts.radecdist:
-            theta = 0.5 * np.pi - np.deg2rad(dec)
-            phi = np.deg2rad(ra)
-            ipix = hp.ang2pix(nside, theta, phi)
-            lines, = ax.plot(
-                [dist], [-0.15], marker=truth_marker,
-                markerfacecolor='none', markeredgewidth=1, clip_on=False,
-                transform=transforms.blended_transform_factory(
-                    ax.transData, ax.transAxes))
-            ax.fill_between(d, scipy.stats.norm(
-                mu[ipix], sigma[ipix]).pdf(d) * norm[ipix] * np.square(d),
-                alpha=0.5, color=lines.get_color())
-            ax.axvline(dist, color='black', linewidth=0.5)
-
-        # Scale axes
-        ax.set_xticks([0, max_distance])
-        ax.set_xticklabels(
-            ['0', "{0:d}\nMpc".format(int(np.round(max_distance)))],
-            fontsize=9)
-        ax.set_yticks([])
-        ax.set_xlim(0, max_distance)
-        ax.set_ylim(0, ax.get_ylim()[1])
-
-        if opts.annotate:
-            text = []
-            try:
-                objid = metadata['objid']
-            except KeyError:
-                pass
-            else:
-                text.append('event ID: {}'.format(objid))
-            try:
-                distmean = metadata['distmean']
-                diststd = metadata['diststd']
-            except KeyError:
-                pass
-            else:
-                text.append('distance: {}±{} Mpc'.format(
-                            int(np.round(distmean)), int(np.round(diststd))))
-            ax.text(0, 1, '\n'.join(text), transform=ax.transAxes, fontsize=7,
-                    ha='left', va='bottom', clip_on=False)
+        # Add contour labels if contours requested
+        if opts.contour:
+            ax.clabel(contourset, fmt='%d%%', fontsize=7)
+
+        if not opts.projection:
+            # Add scale bar, 1/4 width of the plot
+            ax.plot(
+                [0.0625, 0.3125], [0.0625, 0.0625],
+                color='black', linewidth=1, transform=ax.transAxes)
+            ax.text(
+                0.0625, 0.0625,
+                '{0:d} Mpc'.format(int(np.round(0.5 * max_distance))),
+                fontsize=8, transform=ax.transAxes, verticalalignment='bottom')
+
+            # Create marginal distance plot.
+            progress.set_description('Plotting distance')
+            gs1 = gridspec.GridSpecFromSubplotSpec(5, 5, gs[0, 1])
+            ax = fig.add_subplot(gs1[1:-1, 1:-1])
+
+            # Plot marginal distance distribution, integrated over the whole
+            # sky.
+            d = np.linspace(0, max_distance)
+            ax.fill_between(d, marginal_pdf(d, prob, mu, sigma, norm),
+                            alpha=0.5, color=ax._get_lines.get_next_color())
+
+            # Plot conditional distance distribution at true position
+            # and mark true distance.
+            for ra, dec, dist in opts.radecdist:
+                theta = 0.5 * np.pi - np.deg2rad(dec)
+                phi = np.deg2rad(ra)
+                ipix = hp.ang2pix(nside, theta, phi)
+                lines, = ax.plot(
+                    [dist], [-0.15], marker=truth_marker,
+                    markerfacecolor='none', markeredgewidth=1, clip_on=False,
+                    transform=transforms.blended_transform_factory(
+                        ax.transData, ax.transAxes))
+                ax.fill_between(d, scipy.stats.norm(
+                    mu[ipix], sigma[ipix]).pdf(d) * norm[ipix] * np.square(d),
+                    alpha=0.5, color=lines.get_color())
+                ax.axvline(dist, color='black', linewidth=0.5)
+
+            # Scale axes
+            ax.set_xticks([0, max_distance])
+            ax.set_xticklabels(
+                ['0', "{0:d}\nMpc".format(int(np.round(max_distance)))],
+                fontsize=9)
+            ax.set_yticks([])
+            ax.set_xlim(0, max_distance)
+            ax.set_ylim(0, ax.get_ylim()[1])
+
+            if opts.annotate:
+                text = []
+                try:
+                    objid = metadata['objid']
+                except KeyError:
+                    pass
+                else:
+                    text.append('event ID: {}'.format(objid))
+                try:
+                    distmean = metadata['distmean']
+                    diststd = metadata['diststd']
+                except KeyError:
+                    pass
+                else:
+                    text.append('distance: {}±{} Mpc'.format(
+                                int(np.round(distmean)),
+                                int(np.round(diststd))))
+                ax.text(0, 1, '\n'.join(text), transform=ax.transAxes,
+                        fontsize=7, ha='left', va='bottom', clip_on=False)
 
-    progress.set_description('Saving')
-    opts.output()
+        progress.set_description('Saving')
+        opts.output()
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_stats.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2013-2020  Leo Singer
+# Copyright (C) 2013-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -208,37 +208,37 @@
             ret += [searched_modes]
         ret += contour_modes
     return ret
 
 
 def main(args=None):
     p = parser()
-    opts = p.parse_args(args)
+    with p.parse_args(args) as opts:
+        from ..util.progress import progress_map
 
-    from ..util.progress import progress_map
+        if args is None:
+            print('#', *sys.argv, file=opts.output)
+        else:
+            print('#', p.prog, *args, file=opts.output)
 
-    if args is None:
-        print('#', *sys.argv, file=opts.output)
-    else:
-        print('#', p.prog, *args, file=opts.output)
-
-    colnames = ['coinc_event_id']
-    if opts.database is not None:
-        colnames += ['simulation_id', 'far', 'snr', 'searched_area',
-                     'searched_prob', 'searched_prob_dist', 'searched_vol',
-                     'searched_prob_vol', 'offset']
-    colnames += ['runtime', 'distmean', 'diststd', 'log_bci', 'log_bsn']
-    colnames += ['area({0:g})'.format(_) for _ in opts.contour]
-    colnames += ['prob({0:g})'.format(_) for _ in opts.area]
-    colnames += ['dist({0:g})'.format(_) for _ in opts.contour]
-    colnames += ['vol({0:g})'.format(_) for _ in opts.contour]
-    if opts.modes:
+        colnames = ['coinc_event_id']
         if opts.database is not None:
-            colnames += ['searched_modes']
-        colnames += ["modes({0:g})".format(p) for p in opts.contour]
-    print(*colnames, sep="\t", file=opts.output)
-
-    func = partial(process, db=opts.database, contours=opts.contour,
-                   modes=opts.modes, areas=opts.area, cosmology=opts.cosmology)
-    for record in progress_map(func, opts.fitsfilenames, jobs=opts.jobs):
-        if record is not None:
-            print(*record, sep="\t", file=opts.output)
+            colnames += ['simulation_id', 'far', 'snr', 'searched_area',
+                         'searched_prob', 'searched_prob_dist', 'searched_vol',
+                         'searched_prob_vol', 'offset']
+        colnames += ['runtime', 'distmean', 'diststd', 'log_bci', 'log_bsn']
+        colnames += ['area({0:g})'.format(_) for _ in opts.contour]
+        colnames += ['prob({0:g})'.format(_) for _ in opts.area]
+        colnames += ['dist({0:g})'.format(_) for _ in opts.contour]
+        colnames += ['vol({0:g})'.format(_) for _ in opts.contour]
+        if opts.modes:
+            if opts.database is not None:
+                colnames += ['searched_modes']
+            colnames += ["modes({0:g})".format(p) for p in opts.contour]
+        print(*colnames, sep="\t", file=opts.output)
+
+        func = partial(process, db=opts.database, contours=opts.contour,
+                       modes=opts.modes, areas=opts.area,
+                       cosmology=opts.cosmology)
+        for record in progress_map(func, opts.fitsfilenames, jobs=opts.jobs):
+            if record is not None:
+                print(*record, sep="\t", file=opts.output)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/ligo_skymap_unflatten.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/ligo_skymap_unflatten.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2018-2020  Leo Singer
+# Copyright (C) 2018-2024  Leo Singer
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -27,22 +27,21 @@
                         type=FileType('rb'), help='Input FITS file')
     parser.add_argument('output', metavar='OUTPUT.fits[.gz]',
                         type=FileType('wb'), help='Output FITS file')
     return parser
 
 
 def main(args=None):
-    args = parser().parse_args(args)
-
-    import warnings
-    from astropy.io import fits
-    from ..io import read_sky_map, write_sky_map
-
-    hdus = fits.open(args.input)
-    ordering = hdus[1].header['ORDERING']
-    expected_orderings = {'NESTED', 'RING'}
-    if ordering not in expected_orderings:
-        msg = 'Expected the FITS file {} to have ordering {}, but it is {}'
-        warnings.warn(msg.format(
-            args.input.name, ' or '.join(expected_orderings), ordering))
-    table = read_sky_map(hdus, moc=True)
-    write_sky_map(args.output.name, table)
+    with parser().parse_args(args) as args:
+        import warnings
+        from astropy.io import fits
+        from ..io import read_sky_map, write_sky_map
+
+        hdus = fits.open(args.input)
+        ordering = hdus[1].header['ORDERING']
+        expected_orderings = {'NESTED', 'RING'}
+        if ordering not in expected_orderings:
+            msg = 'Expected the FITS file {} to have ordering {}, but it is {}'
+            warnings.warn(msg.format(
+                args.input.name, ' or '.join(expected_orderings), ordering))
+        table = read_sky_map(hdus, moc=True)
+        write_sky_map(args.output.name, table)
```

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/matplotlib.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/matplotlib.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/__init__.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_bayestar.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_bayestar.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_bayestar_inject.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_bayestar_inject.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_combine.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_flatten.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_from_samples.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_from_samples.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_help.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_plot.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/tool/tests/test_plot_stats.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/tool/tests/test_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/file.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/file.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/ilwd.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/ilwd.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/math.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/math.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/numpy.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/numpy.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/progress.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/progress.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/sqlite.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo/skymap/util/stopwatch.py` & `ligo_skymap-2.0.1rc2/ligo/skymap/util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/PKG-INFO` & `ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo.skymap
-Version: 2.0.1rc1
+Version: 2.0.1rc2
 Summary: Tools for reading, writing, manipulating, and making LIGO/Virgo/KAGRA sky maps
 Home-page: https://lscsoft.docs.ligo.org/ligo.skymap/
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 License: GNU GPL v3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/ligo.skymap/issues
 Project-URL: Change Log, https://lscsoft.docs.ligo.org/ligo.skymap/changes.html
```

### Comparing `ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/SOURCES.txt` & `ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/ligo.skymap.egg-info/entry_points.txt` & `ligo_skymap-2.0.1rc2/ligo.skymap.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/setup.cfg` & `ligo_skymap-2.0.1rc2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,17 @@
 
 [tool:pytest]
 testpaths = "ligo/skymap"
 astropy_header = true
 doctest_plus = enabled
 doctest_ufunc = enabled
 omp_get_num_threads = true
+filterwarnings = 
+	error:unclosed file:ResourceWarning
+	error::pytest.PytestUnraisableExceptionWarning
 
 [coverage:run]
 source = {packagename}
 omit = 
 	ligo/skymap/_astropy_init*
 	ligo/skymap/conftest.py
 	ligo/skymap/extern/*
```

### Comparing `ligo_skymap-2.0.1rc1/setup.py` & `ligo_skymap-2.0.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_cosmology.h` & `ligo_skymap-2.0.1rc2/src/bayestar_cosmology.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_cosmology.py` & `ligo_skymap-2.0.1rc2/src/bayestar_cosmology.py`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_distance.c` & `ligo_skymap-2.0.1rc2/src/bayestar_distance.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_distance.h` & `ligo_skymap-2.0.1rc2/src/bayestar_distance.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_moc.c` & `ligo_skymap-2.0.1rc2/src/bayestar_moc.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_moc.h` & `ligo_skymap-2.0.1rc2/src/bayestar_moc.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_sky_map.c` & `ligo_skymap-2.0.1rc2/src/bayestar_sky_map.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/bayestar_sky_map.h` & `ligo_skymap-2.0.1rc2/src/bayestar_sky_map.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/core.c` & `ligo_skymap-2.0.1rc2/src/core.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/cubic_interp.c` & `ligo_skymap-2.0.1rc2/src/cubic_interp.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/cubic_interp.h` & `ligo_skymap-2.0.1rc2/src/cubic_interp.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/cubic_interp_test.c` & `ligo_skymap-2.0.1rc2/src/cubic_interp_test.c`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/omp_interruptible.h` & `ligo_skymap-2.0.1rc2/src/omp_interruptible.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/vmath.h` & `ligo_skymap-2.0.1rc2/src/vmath.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/src/warnings.h` & `ligo_skymap-2.0.1rc2/src/warnings.h`

 * *Files identical despite different names*

### Comparing `ligo_skymap-2.0.1rc1/tox.ini` & `ligo_skymap-2.0.1rc2/tox.ini`

 * *Files identical despite different names*

