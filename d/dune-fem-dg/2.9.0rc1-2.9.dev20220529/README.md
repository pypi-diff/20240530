# Comparing `tmp/dune-fem-dg-2.9.0rc1.tar.gz` & `tmp/dune-fem-dg-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-fem-dg-2.9.0rc1.tar", last modified: Fri Oct 21 08:16:59 2022, max compression
+gzip compressed data, was "dune-fem-dg-2.9.dev20220529.tar", last modified: Sun May 29 21:03:37 2022, max compression
```

## Comparing `dune-fem-dg-2.9.0rc1.tar` & `dune-fem-dg-2.9.dev20220529.tar`

### file list

```diff
@@ -1,592 +1,592 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3917 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.983975 dune-fem-dg-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.987975 dune-fem-dg-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/modules/Codegen.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     6716 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/modules/DuneFemDgMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/modules/FindNETCDF.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/modules/TargetDistclean.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.987975 dune-fem-dg-2.9.0rc1/cmake/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/scripts/RunGenerate.cmake
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/cmake/scripts/parameter.in
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.987975 dune-fem-dg-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/concept
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.987975 dune-fem-dg-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/modules.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.987975 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/advectiondiffusion.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/docrules.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/euler.txt
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/examples.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/incompnavierstokes.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5097 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/navierstokes.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13603 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/notation.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/parameters.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/poisson.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/problemstructure.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/doxygen/pages/stokes.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.991975 dune-fem-dg-2.9.0rc1/doc/pics/
--rw-r--r--   0 runner    (1001) docker     (121)    35615 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/advectiondiffusion.png
--rw-r--r--   0 runner    (1001) docker     (121)   173215 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/algorithms_scheme.png
--rw-r--r--   0 runner    (1001) docker     (121)    73378 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container1.png
--rw-r--r--   0 runner    (1001) docker     (121)    91159 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container2.png
--rw-r--r--   0 runner    (1001) docker     (121)   100989 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container3.png
--rw-r--r--   0 runner    (1001) docker     (121)    52131 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container3_1.png
--rw-r--r--   0 runner    (1001) docker     (121)    92349 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container3_2.png
--rw-r--r--   0 runner    (1001) docker     (121)   138952 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container4.png
--rw-r--r--   0 runner    (1001) docker     (121)   106698 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container5.png
--rw-r--r--   0 runner    (1001) docker     (121)   111808 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container6.png
--rw-r--r--   0 runner    (1001) docker     (121)   127296 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/container7.png
--rw-r--r--   0 runner    (1001) docker     (121)    27147 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/euler.png
--rw-r--r--   0 runner    (1001) docker     (121)    92525 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/incompnavierstokes.png
--rw-r--r--   0 runner    (1001) docker     (121)    51100 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_.png
--rw-r--r--   0 runner    (1001) docker     (121)    92036 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_b.png
--rw-r--r--   0 runner    (1001) docker     (121)    41405 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_i.png
--rw-r--r--   0 runner    (1001) docker     (121)    79419 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_ib.png
--rw-r--r--   0 runner    (1001) docker     (121)    17669 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_q.png
--rw-r--r--   0 runner    (1001) docker     (121)    30078 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_qb.png
--rw-r--r--   0 runner    (1001) docker     (121)    33535 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_qi.png
--rw-r--r--   0 runner    (1001) docker     (121)    61858 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_qib.png
--rw-r--r--   0 runner    (1001) docker     (121)    34379 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/navierstokes.png
--rw-r--r--   0 runner    (1001) docker     (121)    29343 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/poisson.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.995975 dune-fem-dg-2.9.0rc1/doc/pics/source/
--rw-r--r--   0 runner    (1001) docker     (121)     6289 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/advectiondiffusion.svg
--rw-r--r--   0 runner    (1001) docker     (121)    60903 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/algorithms_scheme.svg
--rw-r--r--   0 runner    (1001) docker     (121)    35358 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/algorithms_scheme_base.svg
--rw-r--r--   0 runner    (1001) docker     (121)   238170 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container1.svg
--rw-r--r--   0 runner    (1001) docker     (121)   183612 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container2.svg
--rw-r--r--   0 runner    (1001) docker     (121)   220956 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container3.svg
--rw-r--r--   0 runner    (1001) docker     (121)   169762 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container3_1.svg
--rw-r--r--   0 runner    (1001) docker     (121)   219778 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container3_2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    66773 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container4.svg
--rw-r--r--   0 runner    (1001) docker     (121)    44038 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container5.svg
--rw-r--r--   0 runner    (1001) docker     (121)   194000 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container6.svg
--rw-r--r--   0 runner    (1001) docker     (121)   222929 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/container7.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/euler.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12728 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/incompnavierstokes.svg
--rw-r--r--   0 runner    (1001) docker     (121)    26283 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_.svg
--rw-r--r--   0 runner    (1001) docker     (121)    67432 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_b.svg
--rw-r--r--   0 runner    (1001) docker     (121)    70634 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_i.svg
--rw-r--r--   0 runner    (1001) docker     (121)   147825 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_ib.svg
--rw-r--r--   0 runner    (1001) docker     (121)    25285 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_q.svg
--rw-r--r--   0 runner    (1001) docker     (121)    65383 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_qb.svg
--rw-r--r--   0 runner    (1001) docker     (121)    68549 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_qi.svg
--rw-r--r--   0 runner    (1001) docker     (121)   147037 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_qib.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6250 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/navierstokes.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6220 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/poisson.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7841 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/source/stokes.svg
--rw-r--r--   0 runner    (1001) docker     (121)    41946 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/doc/pics/stokes.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.995975 dune-fem-dg-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.995975 dune-fem-dg-2.9.0rc1/dune/fem-dg/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.995975 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10373 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/base.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.995975 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17287 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/adapt.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10404 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/checkpoint.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8974 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/datawriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/eocwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/interface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/postprocessing.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5841 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/solvermonitor.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9650 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/adapt.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10181 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/datawriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/solvermonitor.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13979 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/containers.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/createsubalgorithms.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18435 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/evolution.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/gridinitializer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4251 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/monitor.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/steadystate.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4727 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/advection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/advectiondiffusion.hh
--rw-r--r--   0 runner    (1001) docker     (121)    34166 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/containers.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26025 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12784 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/evolution.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/interface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11284 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/steadystate.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/assemble/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/assemble/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/assemble/assemblertraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)    37386 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/assemble/primalmatrix.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9001 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/models.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/deformationalflow.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7688 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/problem.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/problemQuasiHeatEqn.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/pulse.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/sin.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_heat
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_hierarchic_legendre
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_legendre
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_orthonormal
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_pulse
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_quasi
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff_sin
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiffall
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder1
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder2
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder3
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder4
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/parameter
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7747 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/checkedcheckpointcaller.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/checkpointing.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7550 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/dataconvert.cc
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/models.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7558 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/problem.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:58.999975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/checkpointing
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/dataio
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/parameter
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8145 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6353 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/chorjo.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20180 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/generatedmodel_sod_2d.hh
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13688 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/models.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/problems/
--rw-r--r--   0 runner    (1001) docker     (121)    31030 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/problems/problems.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/problems.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/euler
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/euler_effcomp
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/euler_effcomp_ufl
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/eulerall
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/parameter
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner3d_nonaffine.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner_cube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner_green.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner_red.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/grid2d_nonaffine.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/grid2d_str1d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/nswaves_1d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/nswaves_2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/nswaves_2d_unstr.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/nswaves_3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/square2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/unitcube1.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/unitcube2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/unitcube2_per.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/unitcube2_unstr.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/unitcube3.dgf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5333 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/incompnavierstokesalgorithm.hh
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12165 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/models.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/problems/
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/problems/operatorsplitting.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12685 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/problems/problem.hh
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/problems.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14393 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/stokesmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5148 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/subnavierstokesalgorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5393 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/subpoissonalgorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/substokesalgorithmcreator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/BuildTests.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokes
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokesall
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/parameter
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.003975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7093 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/models.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/navierstokesflux.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7256 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems/nssmooth.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10356 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems/nswaves.hh
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/navierstokes
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/navierstokesall
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/parameter
--rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/thermodynamics.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/test/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/test/parameter
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/test/parameters/netcdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/paramBase
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/paramPhysicalConstants
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/paramSolver
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5002 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/gridinitializer.hh
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15091 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/models.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/problems/
--rw-r--r--   0 runner    (1001) docker     (121)    60726 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/problems/benchmarkproblems.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7721 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/problems/poissonproblem.hh
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/problems.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/poisson
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/poissonall
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13026 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/algorithmcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13718 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/models.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/problems/
--rw-r--r--   0 runner    (1001) docker     (121)     9450 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/problems/corner.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16582 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/problems/problem.hh
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/problems.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21897 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/stokesalgorithm.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24673 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/stokesassembler.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/tensorhelper.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.007975 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/stokes
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/stokesall
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/femdgtest.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4052 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/algorithmcreatorenums.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26716 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/algorithmcreatorselector.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11287 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/configurator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/cons2prim.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/covarianttuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/crs.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11969 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/dgnorm.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14685 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/diagnostics.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/dgeocerror.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/eocerrorlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/h1eocerror.hh
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/l1eocerror.hh
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/l2eocerror.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6858 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/evaluatecaller.hh
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/functioncheck.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5792 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/integral_constant.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/interpolatethreaded.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/matrixutils.hh
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/optional.hh
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/parameterkey.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9662 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/simulator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/static_warning.hh
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/streams.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/timesteppingparameter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    44302 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/tupleutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/typedefcheck.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/uniquefunctionname.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/models/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/models/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    24763 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/models/defaultmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14598 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/models/defaultprobleminterfaces.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20010 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/models/modelwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/models/stokesprobleminterfaces.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/adaptation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8076 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/adaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16169 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/estimator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/estimatorbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)    39726 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/poissonestimator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/stokesestimator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/utility.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/common/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/common/orderreduction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11047 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/dgpyoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19465 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/discretemodelcommon.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17104 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/fluxdiscretemodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20905 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/fluxoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9330 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/operatorbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/operatortraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20366 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/primaldiscretemodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20835 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/primaloperator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.011975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/fluxbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/fluxes.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/llfadvflux.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/noflux.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/parameters.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/python.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/upwindflux.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/userdefined.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8058 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/analyticaleulerflux.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    41181 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/dgprimalfluxes.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15449 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/fluxbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10996 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/fluxes.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11878 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/ldgflux.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9851 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/parameters.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16783 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/eulerflux_impl.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6144 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/fluxes.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4615 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/llfadv.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/parameters.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)   101072 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.cc
--rw-r--r--   0 runner    (1001) docker     (121)   101428 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.hh
--rw-r--r--   0 runner    (1001) docker     (121)   145908 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.cc
--rw-r--r--   0 runner    (1001) docker     (121)    89675 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhdfluxes.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/rotator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/indicatorbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limiter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16904 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limiterdiscretemodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11109 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limitermodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    32535 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limiterutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)    65792 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limitpass.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9816 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/lpreconstruction.hh
--rw-r--r--   0 runner    (1001) docker     (121)    30836 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/scalinglimitpass.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/smoothness.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    36249 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/context.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8079 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dginversemass.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19502 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dgmasspass.hh
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dgmodelcaller.hh
--rw-r--r--   0 runner    (1001) docker     (121)    35987 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dgpass.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22857 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/discretemodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6527 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/insertfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/insertoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13278 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/localfunctiontuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20671 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/modelcaller.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18209 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/pass.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/selector.hh
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/threadhandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25987 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/threadpass.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.015975 dune-fem-dg-2.9.0rc1/dune/fem-dg/python/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/python/operator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8859 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/dghelmholtzinverse.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21030 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/rungekuttasolver.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7838 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/uzawa.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/optim/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5176 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/activeindexmapper.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/optim/common/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/axisalignedreferencefaces.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/densesubvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/fieldmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/getreference.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/integerrange.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14342 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/matrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/common/smallobject.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/optim/constraint/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/constraint/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/constraint/linear.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5391 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/lp.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8398 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/minimize.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/optim/qp/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/qp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/qp/combinedgauss.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/qp/gradient.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/qp/reducedgauss.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/qp.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/optim/solver/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/solver/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9956 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/solver/fullydynmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/solver/gauss.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/solver/gaussjordan.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/solver/rowrefvector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/dune/optim/std/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/std/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/std/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6728 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune/optim/std/subarray.hh
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune-fem-dg.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/dune.module
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/lib/dunefemdgam2cmake.lib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/pydemo/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.019975 dune-fem-dg-2.9.0rc1/pydemo/adrsolver/
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/adrsolver/adrsolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/adrsolver/scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/adrsolver/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/advection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/advection_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/chemical.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/chemical_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/euler_kh.py
--rw-r--r--   0 runner    (1001) docker     (121)     7272 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/euler_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/euler_sb.py
--rw-r--r--   0 runner    (1001) docker     (121)     6680 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/evolve.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/kh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/modalindicator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/ns_kh.py
--rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/ns_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/residual.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/shockvortex2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/shockvortex_naffine.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/shockvortex_poly.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/sw.py
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/sw_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/sw_wb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/triangle.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/unitsquare.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/utility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/camc-paper/wb.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemesh.geo
--rw-r--r--   0 runner    (1001) docker     (121)    72754 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)   303147 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemeshfine.msh
--rw-r--r--   0 runner    (1001) docker     (121)     4694 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemeshquad.msh
--rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/micap.py
--rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/micap1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/paper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/cpptest/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/cpptest/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/cpptest/advection.ufl
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/cpptest/advectiondiffusion.ufl
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/cpptest/diffusion.ufl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/euler/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/chorin.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     8133 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/euler.py
--rw-r--r--   0 runner    (1001) docker     (121)     6116 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/euler_effcomp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/llf.hh
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/llf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     4799 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/paper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/rk.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/sod.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/testdg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/testfv0.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/testfv1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/testpolyfv1.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/euler/triangle.dgf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/eulerufl/
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/eulerufl/dolfin_dg.patch
--rw-r--r--   0 runner    (1001) docker     (121)     5395 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/eulerufl/euler_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/fulltest.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/paramSolver
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/paramThreading
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/parameter
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/rk/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/rk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/rk/euler.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/rk/llf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/rk/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/rk/scheme.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/rk/shock_tube_fast.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.023975 dune-fem-dg-2.9.0rc1/pydemo/scalar/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/scalar/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/scalar/rk.py
--rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/scalar/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/pydemo/shallowWater/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/shallowWater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/shallowWater/llf.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/shallowWater/llfwb.hh
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/shallowWater/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pydemo/shallowWater/shallowwater.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/python/dune/femdg/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30697 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)    18031 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)    21792 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/rk.py
--rw-r--r--   0 runner    (1001) docker     (121)     6949 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune/femdg/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3917 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19183 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5854 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/build-dune-fem-dg.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2960 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/check-dist.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1222 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/check-header.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1067 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/check-headers.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3078 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/check-opts.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1260 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/check-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      976 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/fullcheck.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1222 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/mpiexec.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/scripts/opts/
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/opts/ci-gcc.opts
--rwxr-xr-x   0 runner    (1001) docker     (121)      712 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/update-dune-modules.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      337 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/scripts/version.sh
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:16:59.027974 dune-fem-dg-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:16:58.000000 dune-fem-dg-2.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.275720 dune-fem-dg-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.279719 dune-fem-dg-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/modules/Codegen.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     6716 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/modules/DuneFemDgMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/modules/FindNETCDF.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/modules/TargetDistclean.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.279719 dune-fem-dg-2.9.dev20220529/cmake/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/scripts/RunGenerate.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/cmake/scripts/parameter.in
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.279719 dune-fem-dg-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/concept
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.279719 dune-fem-dg-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/modules.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.283720 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/advectiondiffusion.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/docrules.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/euler.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/incompnavierstokes.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5097 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/navierstokes.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13603 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/notation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/parameters.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/poisson.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/problemstructure.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/stokes.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.283720 dune-fem-dg-2.9.dev20220529/doc/pics/
+-rw-r--r--   0 runner    (1001) docker     (121)    35615 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/advectiondiffusion.png
+-rw-r--r--   0 runner    (1001) docker     (121)   173215 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/algorithms_scheme.png
+-rw-r--r--   0 runner    (1001) docker     (121)    73378 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container1.png
+-rw-r--r--   0 runner    (1001) docker     (121)    91159 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container2.png
+-rw-r--r--   0 runner    (1001) docker     (121)   100989 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container3.png
+-rw-r--r--   0 runner    (1001) docker     (121)    52131 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container3_1.png
+-rw-r--r--   0 runner    (1001) docker     (121)    92349 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container3_2.png
+-rw-r--r--   0 runner    (1001) docker     (121)   138952 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container4.png
+-rw-r--r--   0 runner    (1001) docker     (121)   106698 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container5.png
+-rw-r--r--   0 runner    (1001) docker     (121)   111808 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container6.png
+-rw-r--r--   0 runner    (1001) docker     (121)   127296 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/container7.png
+-rw-r--r--   0 runner    (1001) docker     (121)    27147 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/euler.png
+-rw-r--r--   0 runner    (1001) docker     (121)    92525 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/incompnavierstokes.png
+-rw-r--r--   0 runner    (1001) docker     (121)    51100 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_.png
+-rw-r--r--   0 runner    (1001) docker     (121)    92036 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_b.png
+-rw-r--r--   0 runner    (1001) docker     (121)    41405 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_i.png
+-rw-r--r--   0 runner    (1001) docker     (121)    79419 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_ib.png
+-rw-r--r--   0 runner    (1001) docker     (121)    17669 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_q.png
+-rw-r--r--   0 runner    (1001) docker     (121)    30078 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_qb.png
+-rw-r--r--   0 runner    (1001) docker     (121)    33535 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_qi.png
+-rw-r--r--   0 runner    (1001) docker     (121)    61858 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_qib.png
+-rw-r--r--   0 runner    (1001) docker     (121)    34379 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/navierstokes.png
+-rw-r--r--   0 runner    (1001) docker     (121)    29343 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/poisson.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.287720 dune-fem-dg-2.9.dev20220529/doc/pics/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     6289 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/advectiondiffusion.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    60903 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/algorithms_scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    35358 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/algorithms_scheme_base.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   238170 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container1.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   183612 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container2.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   220956 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container3.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   169762 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container3_1.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   219778 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container3_2.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    66773 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container4.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    44038 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container5.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   194000 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container6.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   222929 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/container7.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     6214 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/euler.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    12728 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/incompnavierstokes.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    26283 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    67432 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_b.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    70634 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_i.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   147825 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_ib.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    25285 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_q.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    65383 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_qb.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    68549 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_qi.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   147037 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_qib.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     6250 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/navierstokes.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     6220 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/poisson.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7841 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/source/stokes.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    41946 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/doc/pics/stokes.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.287720 dune-fem-dg-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10373 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/base.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17287 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/adapt.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10404 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/checkpoint.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8974 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/datawriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4815 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/eocwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/interface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/postprocessing.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5841 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/solvermonitor.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9650 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/adapt.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10181 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/datawriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/solvermonitor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13979 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/containers.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/createsubalgorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18435 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/evolution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/gridinitializer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4251 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/monitor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/steadystate.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4727 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/advection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/advectiondiffusion.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    34166 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/containers.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26025 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12784 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/evolution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/interface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11284 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/steadystate.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/assemble/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/assemble/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/assemble/assemblertraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    37386 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/assemble/primalmatrix.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9001 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/models.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/deformationalflow.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7688 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/problem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/problemQuasiHeatEqn.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/pulse.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/sin.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.291720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_heat
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_hierarchic_legendre
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_legendre
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_orthonormal
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_pulse
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_quasi
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff_sin
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiffall
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder1
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder2
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder3
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiffall_polorder4
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/parameter
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7747 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/checkedcheckpointcaller.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8126 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/checkpointing.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7550 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/dataconvert.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/models.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7558 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/problem.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/checkpointing
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/dataio
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/parameter
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8145 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6353 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/chorjo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20180 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/generatedmodel_sod_2d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13688 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/models.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)    31030 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/problems/problems.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/problems.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.295720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/euler
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/euler_effcomp
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/euler_effcomp_ufl
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/eulerall
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/parameter
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner3d_nonaffine.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner_cube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner_green.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner_red.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/grid2d_nonaffine.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/grid2d_str1d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/nswaves_1d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/nswaves_2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/nswaves_2d_unstr.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/nswaves_3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/square2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/unitcube1.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/unitcube2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/unitcube2_per.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/unitcube2_unstr.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/unitcube3.dgf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5333 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/incompnavierstokesalgorithm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12165 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/models.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/problems/operatorsplitting.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12685 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/problems/problem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/problems.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14393 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/stokesmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5148 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/subnavierstokesalgorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5393 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/subpoissonalgorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/substokesalgorithmcreator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/BuildTests.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokes
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokesall
+-rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/parameter
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7093 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/models.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/navierstokesflux.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7256 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems/nssmooth.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10356 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems/nswaves.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/navierstokes
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/navierstokesall
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/thermodynamics.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/test/parameter
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/test/parameters/netcdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/
+-rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/paramBase
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/paramPhysicalConstants
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/paramSolver
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5002 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/gridinitializer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15091 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/models.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.299720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)    60726 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/problems/benchmarkproblems.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7721 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/problems/poissonproblem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/problems.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/poisson
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/poissonall
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13026 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/algorithmcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13718 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/models.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)     9450 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/problems/corner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16582 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/problems/problem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/problems.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21897 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/stokesalgorithm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24673 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/stokesassembler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/tensorhelper.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/stokes
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/stokesall
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/femdgtest.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4052 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/algorithmcreatorenums.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26716 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/algorithmcreatorselector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11287 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/configurator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/cons2prim.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/covarianttuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/crs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11969 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/dgnorm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14695 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/diagnostics.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.303720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/dgeocerror.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/eocerrorlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/h1eocerror.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/l1eocerror.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/l2eocerror.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6858 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/evaluatecaller.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/functioncheck.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5792 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/integral_constant.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/interpolatethreaded.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/matrixutils.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/optional.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/parameterkey.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9662 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/simulator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/static_warning.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/streams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/timesteppingparameter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    44302 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/tupleutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/typedefcheck.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/uniquefunctionname.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    24533 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/defaultmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14598 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/defaultprobleminterfaces.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19084 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/modelwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/stokesprobleminterfaces.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/adaptation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8076 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/adaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16169 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/estimator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/estimatorbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    39726 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/poissonestimator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/stokesestimator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8287 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/utility.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/common/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/common/orderreduction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11022 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/dgpyoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19465 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/discretemodelcommon.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17104 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/fluxdiscretemodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20905 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/fluxoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9330 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/operatorbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/operatortraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20366 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/primaldiscretemodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20835 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/primaloperator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/fluxbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/fluxes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/llfadvflux.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/noflux.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/parameters.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/python.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/upwindflux.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/userdefined.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8058 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/analyticaleulerflux.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    41181 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/dgprimalfluxes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15449 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/fluxbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10996 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/fluxes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11878 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/ldgflux.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9851 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/parameters.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.307720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16051 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/eulerflux_impl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5435 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/fluxes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4615 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/llfadv.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/parameters.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.311720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   101072 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.cc
+-rw-r--r--   0 runner    (1001) docker     (121)   101428 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.hh
+-rw-r--r--   0 runner    (1001) docker     (121)   145908 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    89675 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhdfluxes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/rotator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.311720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/indicatorbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12150 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limiter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16904 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limiterdiscretemodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11109 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limitermodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    32535 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limiterutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    65792 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limitpass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9816 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/lpreconstruction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    30836 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/scalinglimitpass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/smoothness.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.311720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    36249 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/context.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8079 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dginversemass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19502 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dgmasspass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dgmodelcaller.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    35987 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dgpass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22857 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/discretemodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6527 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/insertfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/insertoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13278 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/localfunctiontuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20671 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/modelcaller.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18209 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/pass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/selector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/threadhandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25940 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/threadpass.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.311720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/python/operator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.311720 dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8706 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/dghelmholtzinverse.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21060 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/rungekuttasolver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7838 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/uzawa.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.311720 dune-fem-dg-2.9.dev20220529/dune/optim/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5176 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/activeindexmapper.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/dune/optim/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/axisalignedreferencefaces.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/densesubvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/fieldmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/getreference.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/integerrange.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14342 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/matrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/common/smallobject.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/dune/optim/constraint/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/constraint/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/constraint/linear.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5391 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/lp.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8398 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/minimize.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/dune/optim/qp/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/qp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/qp/combinedgauss.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/qp/gradient.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/qp/reducedgauss.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/qp.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/dune/optim/solver/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/solver/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9956 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/solver/fullydynmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/solver/gauss.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/solver/gaussjordan.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/solver/rowrefvector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/dune/optim/std/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/std/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/std/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6728 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune/optim/std/subarray.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune-fem-dg.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/dune.module
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/lib/dunefemdgam2cmake.lib
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/pydemo/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.315720 dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/
+-rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/adrsolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/advection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/advection_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/chemical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/chemical_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/euler_kh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7272 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/euler_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/euler_sb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6680 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/kh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/modalindicator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/ns_kh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8475 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/ns_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/residual.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/shockvortex2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/shockvortex_naffine.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/shockvortex_poly.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/sw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/sw_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/sw_wb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/triangle.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/unitsquare.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/utility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4134 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/wb.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemesh.geo
+-rw-r--r--   0 runner    (1001) docker     (121)    72754 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)   303147 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemeshfine.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     4694 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemeshquad.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     3570 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/micap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8556 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/micap1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/paper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/cpptest/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/cpptest/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/cpptest/advection.ufl
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/cpptest/advectiondiffusion.ufl
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/cpptest/diffusion.ufl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/euler/
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/chorin.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/compare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8133 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/euler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6116 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/euler_effcomp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/llf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/llf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4799 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/paper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/rk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      915 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/sod.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/testdg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/testfv0.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/testfv1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/testpolyfv1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/euler/triangle.dgf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/eulerufl/
+-rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/eulerufl/dolfin_dg.patch
+-rw-r--r--   0 runner    (1001) docker     (121)     5395 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/eulerufl/euler_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/fulltest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/paramSolver
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/paramThreading
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/parameter
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/rk/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/rk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/rk/euler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/rk/llf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/rk/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/rk/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/rk/shock_tube_fast.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.319720 dune-fem-dg-2.9.dev20220529/pydemo/scalar/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/scalar/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/scalar/rk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/scalar/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/llf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/llfwb.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/shallowwater.py
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/python/dune/femdg/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30521 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17558 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21792 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/rk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6949 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/python/dune/femdg/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-05-29 21:03:37.000000 dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19183 2022-05-29 21:03:37.000000 dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:37.000000 dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-29 21:03:37.000000 dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:37.000000 dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5854 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/build-dune-fem-dg.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2960 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/check-dist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1222 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/check-header.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1067 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/check-headers.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3078 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/check-opts.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1260 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/check-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      976 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/fullcheck.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1222 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/mpiexec.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/scripts/opts/
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/opts/ci-gcc.opts
+-rwxr-xr-x   0 runner    (1001) docker     (121)      711 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/update-dune-modules.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      337 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/scripts/version.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:37.323720 dune-fem-dg-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:36.000000 dune-fem-dg-2.9.dev20220529/setup.py
```

### Comparing `dune-fem-dg-2.9.0rc1/.gitignore` & `dune-fem-dg-2.9.dev20220529/.gitignore`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/.gitlab-ci.yml` & `dune-fem-dg-2.9.dev20220529/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/AUTHORS` & `dune-fem-dg-2.9.dev20220529/AUTHORS`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/PKG-INFO` & `dune-fem-dg-2.9.dev20220529/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-fem-dg
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: The Dune FEM module: Discontinuous Galerkin for evolution equations
 Home-page: https://www.dune-project.org/modules/dune-fem-dg/
 Author: Andreas Dedner, Tobias Malkmus, Robert Kloefkorn, Stefan Wierling (geb. Girke)
 Author-email: dune-fem@lists.dune-project.org
 License: UNKNOWN
 Description: DUNE-FEM-DG
         ===========
@@ -83,15 +83,15 @@
         
         A documentation for the 2.4 release can be found in
         
         * A. Dedner, S. Girke, R. Klöfkorn, T. Malkmus. 2017. The DUNE-FEM-DG module.
         Archive of Numerical Software 5(1): 21--61. http://dx.doi.org/10.11588/ans.2017.1.28602
         
         
-        git-8685c1f074de90182ab41cda4d4836a8f903b30d
+        git-3b4ad3b8d6449914d9b2aa333457451b45ab81cb
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-fem-dg-2.9.0rc1/README.md` & `dune-fem-dg-2.9.dev20220529/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -75,8 +75,8 @@
 
 A documentation for the 2.4 release can be found in
 
 * A. Dedner, S. Girke, R. Klöfkorn, T. Malkmus. 2017. The DUNE-FEM-DG module.
 Archive of Numerical Software 5(1): 21--61. http://dx.doi.org/10.11588/ans.2017.1.28602
 
 
-git-8685c1f074de90182ab41cda4d4836a8f903b30d
+git-3b4ad3b8d6449914d9b2aa333457451b45ab81cb
```

### Comparing `dune-fem-dg-2.9.0rc1/cmake/modules/Codegen.cmake` & `dune-fem-dg-2.9.dev20220529/cmake/modules/Codegen.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/cmake/modules/DuneFemDgMacros.cmake` & `dune-fem-dg-2.9.dev20220529/cmake/modules/DuneFemDgMacros.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/cmake/modules/FindNETCDF.cmake` & `dune-fem-dg-2.9.dev20220529/cmake/modules/FindNETCDF.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/config.h.cmake` & `dune-fem-dg-2.9.dev20220529/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/concept` & `dune-fem-dg-2.9.dev20220529/doc/concept`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/Doxylocal` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/Doxylocal`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/modules.txt` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/modules.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/pages/docrules.txt` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/docrules.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/pages/mainpage.txt` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/mainpage.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/pages/notation.txt` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/notation.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/pages/parameters.txt` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/parameters.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/doxygen/pages/poisson.txt` & `dune-fem-dg-2.9.dev20220529/doc/doxygen/pages/poisson.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/advectiondiffusion.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/advectiondiffusion.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/algorithms_scheme.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/algorithms_scheme.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container1.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container1.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container2.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container2.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container3.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container3.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container3_1.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container3_1.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container3_2.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container3_2.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container4.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container4.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container5.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container5.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container6.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container6.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/container7.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/container7.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/euler.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/euler.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/incompnavierstokes.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/incompnavierstokes.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_b.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_b.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_i.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_i.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_ib.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_ib.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_q.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_q.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_qb.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_qb.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_qi.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_qi.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/local_eval_structure_qib.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/local_eval_structure_qib.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/navierstokes.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/navierstokes.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/poisson.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/poisson.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/advectiondiffusion.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/advectiondiffusion.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/algorithms_scheme.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/algorithms_scheme.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/algorithms_scheme_base.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/algorithms_scheme_base.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container1.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container1.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container2.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container2.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container3.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container3.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container3_1.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container3_1.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container3_2.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container3_2.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container4.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container4.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container5.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container5.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container6.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container6.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/container7.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/container7.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/euler.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/euler.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/incompnavierstokes.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/incompnavierstokes.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_b.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_b.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_i.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_i.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_ib.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_ib.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_q.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_q.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_qb.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_qb.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_qi.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_qi.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/local_eval_structure_qib.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/local_eval_structure_qib.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/navierstokes.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/navierstokes.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/poisson.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/poisson.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/source/stokes.svg` & `dune-fem-dg-2.9.dev20220529/doc/pics/source/stokes.svg`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/doc/pics/stokes.png` & `dune-fem-dg-2.9.dev20220529/doc/pics/stokes.png`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/base.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/base.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/adapt.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/adapt.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/checkpoint.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/checkpoint.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/datawriter.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/datawriter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/diagnostics.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/diagnostics.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/eocwriter.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/eocwriter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/interface.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/interface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/postprocessing.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/postprocessing.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/solvermonitor.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/solvermonitor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/adapt.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/adapt.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/datawriter.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/datawriter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/diagnostics.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/diagnostics.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/caller/sub/solvermonitor.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/caller/sub/solvermonitor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/containers.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/containers.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/createsubalgorithms.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/createsubalgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/evolution.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/evolution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/gridinitializer.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/gridinitializer.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/monitor.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/monitor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/steadystate.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/steadystate.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/advection.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/advection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/advectiondiffusion.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/advectiondiffusion.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/containers.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/containers.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/elliptic.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/evolution.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/evolution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/interface.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/interface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/algorithm/sub/steadystate.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/algorithm/sub/steadystate.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/assemble/assemblertraits.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/assemble/assemblertraits.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/assemble/primalmatrix.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/assemble/primalmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/deformationalflow.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/deformationalflow.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/problem.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/problem.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/problemQuasiHeatEqn.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/problemQuasiHeatEqn.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/pulse.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/pulse.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems/sin.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems/sin.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/problems.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/problems.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiff` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiff`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/advdiffall` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/advdiffall`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/advdiff/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/advdiff/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/checkedcheckpointcaller.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/checkedcheckpointcaller.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/checkpointing.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/checkpointing.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/dataconvert.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/dataconvert.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/problem.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/problem.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/checkpointing` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/checkpointing`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/dataio` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/dataio`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/dataio/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/dataio/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/chorjo.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/chorjo.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/generatedmodel_sod_2d.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/generatedmodel_sod_2d.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/problems/problems.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/problems/problems.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/problems.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/problems.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/euler` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/euler`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/euler_effcomp` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/euler_effcomp`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/euler_effcomp_ufl` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/euler_effcomp_ufl`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/eulerall` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/eulerall`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/euler/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/euler/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/corner3d_nonaffine.dgf` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/corner3d_nonaffine.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/grids/grid2d_nonaffine.dgf` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/grids/grid2d_nonaffine.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/incompnavierstokesalgorithm.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/incompnavierstokesalgorithm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/problems/operatorsplitting.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/problems/operatorsplitting.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/problems/problem.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/problems/problem.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/stokesmodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/stokesmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/subnavierstokesalgorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/subnavierstokesalgorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/subpoissonalgorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/subpoissonalgorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/substokesalgorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/substokesalgorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokes` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokes`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokesall` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/incompnavierstokesall`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/incompnavierstokes/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/incompnavierstokes/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/navierstokesflux.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/navierstokesflux.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems/nssmooth.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems/nssmooth.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/problems/nswaves.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/problems/nswaves.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/navierstokes` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/navierstokes`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/navierstokesall` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/navierstokesall`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/navierstokes/thermodynamics.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/navierstokes/thermodynamics.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/netcdf/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/netcdf/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/paramBase` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/paramBase`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/paramPhysicalConstants` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/paramPhysicalConstants`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/parameter/paramSolver` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/parameter/paramSolver`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/gridinitializer.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/gridinitializer.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/problems/benchmarkproblems.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/problems/benchmarkproblems.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/problems/poissonproblem.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/problems/poissonproblem.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/poisson` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/poisson`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/poisson/test/parameters/poissonall` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/poisson/test/parameters/poissonall`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/algorithmcreator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/algorithmcreator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/main.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/models.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/models.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/problems/corner.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/problems/corner.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/problems/problem.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/problems/problem.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/stokesalgorithm.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/stokesalgorithm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/stokesassembler.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/stokesassembler.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/tensorhelper.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/tensorhelper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/parameter` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/stokes` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/stokes`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/examples/stokes/test/parameters/stokesall` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/examples/stokes/test/parameters/stokesall`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/algorithmcreatorenums.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/algorithmcreatorenums.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/algorithmcreatorselector.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/algorithmcreatorselector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/configurator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/configurator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/cons2prim.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/cons2prim.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/covarianttuple.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/covarianttuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/crs.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/crs.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/dgnorm.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/dgnorm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/diagnostics.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 {
 namespace Fem
 {
 
   class Diagnostics
     : public Fem::AutoPersistentObject
   {
-    typedef Fem :: MPIManager :: Communication CommunicatorType;
+    typedef Fem :: MPIManager :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all diagnosticss
                              // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnostics_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/dgeocerror.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/dgeocerror.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/eocerrorlist.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/eocerrorlist.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/h1eocerror.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/h1eocerror.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/l1eocerror.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/l1eocerror.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/error/l2eocerror.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/error/l2eocerror.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/evaluatecaller.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/evaluatecaller.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/functioncheck.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/functioncheck.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/integral_constant.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/integral_constant.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/interpolatethreaded.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/interpolatethreaded.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/matrixutils.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/matrixutils.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/optional.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/optional.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/parameterkey.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/parameterkey.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/simulator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/simulator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/static_warning.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/static_warning.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/streams.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/streams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/timesteppingparameter.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/timesteppingparameter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/tupleutility.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/tupleutility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/typedefcheck.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/typedefcheck.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/misc/uniquefunctionname.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/misc/uniquefunctionname.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/models/defaultmodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/defaultmodel.hh`

 * *Files 1% similar despite different names*

```diff
@@ -215,24 +215,14 @@
     void obtainBounds( RangeType& globalMin, RangeType& globalMax ) const
     {
       globalMin =  1e308;
       globalMax = -1e308;
     }
 
     /**
-     *  \brief compute pressure and temperature for compressible flow
-     */
-    template <class State>
-    void pressureTemperatur( const State& u, double& p, double& T ) const
-    {
-      p = 0.0;
-      T = 0.0;
-    }
-
-    /**
      * \brief returns the mass factor term \f$ R \f$
      *
      * \param[in]  local local evaluation
      * \param[in]  u evaluation of the local function, i.e. \f$ u_E( \hat{x} ) \f$
      * \param[out] diagonal of the mass term, i.e. the result \f$ R(u) \f$
      *
      */
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/models/defaultprobleminterfaces.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/defaultprobleminterfaces.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/models/modelwrapper.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/modelwrapper.hh`

 * *Files 2% similar despite different names*

```diff
@@ -222,17 +222,17 @@
     }
 
     double gamma () const { return problem_.gamma(); }
 
     template <class Entity>
     void setEntity( const Entity& entity ) const
     {
-      if constexpr ( hasAdvection )
+      if( hasAdvection )
         advection().init( entity );
-      if constexpr ( hasDiffusion )
+      if( hasDiffusion )
         diffusion().init( entity );
     }
 
     inline bool hasStiffSource() const { return AdditionalType::hasStiffSource; }
     inline bool hasNonStiffSource() const { return AdditionalType::hasNonStiffSource; }
     inline bool hasFlux() const { return AdditionalType::hasFlux; }
 
@@ -245,36 +245,14 @@
     }
 
     bool isConstant( const RangeType& min, const RangeType& max ) const
     {
       return (min - max).infinity_norm() < 1e-10;
     }
 
-    template <class State> // double[dim+2]
-    void pressureTemperature( const State& u, double& p, double& T ) const
-    {
-      if constexpr ( hasAdvection )
-      {
-        const auto pT = advection().pressureTemperature( u );
-        p = pT[0];
-        T = pT[1];
-        return ;
-      }
-
-      if constexpr ( hasDiffusion )
-      {
-        const auto pT = diffusion().pressureTemperature( u );
-        p = pT[0];
-        T = pT[1];
-        return ;
-      }
-
-      p = 0.0;
-      T = 0.0;
-    }
 
     template <class LocalEvaluation>
     inline double stiffSource( const LocalEvaluation& local,
                                const RangeType& u,
                                const JacobianRangeType& du,
                                RangeType & s) const
     {
@@ -306,15 +284,15 @@
     }
 
     template <class LocalEvaluation>
     inline void eigenValues(const LocalEvaluation& local,
                             const RangeType& u,
                             RangeType& maxValue) const
     {
-      if constexpr ( hasDiffusion )
+      if( hasDiffusion )
       {
         maxValue = diffusion().diffusionTimeStep( local.entity(), local.quadraturePoint(), u );
       }
     }
 
     template <class LocalEvaluation>
     inline double diffusionTimeStep( const LocalEvaluation& local,
@@ -391,18 +369,14 @@
     template <class LocalEvaluation>
     void diffusion( const LocalEvaluation& local,
                     const RangeType& u,
                     const JacobianRangeType& du,
                     JacobianRangeType& diff ) const
     {
       assert( hasDiffusion );
-      // TODO: This should be done outside when calling setEntity,
-      // however, this seems not to work and will trigger the assertion
-      diffusion().init( local.entity() );
-      //assert( &(diffusion().entity()) == &(local.entity()) );
       diffusion().flux( local.quadraturePoint(), u, du, diff);
     }
 
 
     /** \brief boundary flux for the diffusion part
      */
     template <class LocalEvaluation>
@@ -550,19 +524,14 @@
 
     // default constructor called by DGOperator
     AdvectionModelWrapper( const AdvectionModelType& advModel )
       : BaseType( advModel, advModel, *(new ProblemType() )),
         problemPtr_( &this->problem_ )
     {}
 
-    // copy constructor
-    AdvectionModelWrapper( const AdvectionModelWrapper& other )
-      : AdvectionModelWrapper( other.advection() )
-    {}
-
   protected:
     std::unique_ptr< const ProblemType > problemPtr_;
   };
 
 } // end namespace Fem
 } // end namespace Dune
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/models/stokesprobleminterfaces.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/models/stokesprobleminterfaces.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/adaptation.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/adaptation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/adaptation.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/estimator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/estimator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/estimatorbase.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/estimatorbase.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/poissonestimator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/poissonestimator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/stokesestimator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/stokesestimator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/adaptation/utility.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/adaptation/utility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/common/orderreduction.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/common/orderreduction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/dgpyoperator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/dgpyoperator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 #include <dune/fem-dg/algorithm/evolution.hh>
 
 // dune-fem-dg includes
 #include <dune/fem-dg/algorithm/evolution.hh>
 #include <dune/fem-dg/operator/fluxes/advection/fluxes.hh>
-#include <dune/fem-dg/operator/fluxes/euler/fluxes.hh>
 #include <dune/fem-dg/operator/dg/operatortraits.hh>
 #include <dune/fem-dg/operator/dg/primaloperator.hh>
 #include <dune/fem-dg/models/modelwrapper.hh>
 #include <dune/fem-dg/misc/algorithmcreatorselector.hh>
 #include <dune/fem-dg/operator/adaptation/estimator.hh>
 
 // this is part of dune-fem now
@@ -55,16 +54,16 @@
     typedef typename DestinationType :: DiscreteFunctionSpaceType    DiscreteFunctionSpaceType;
     typedef typename DiscreteFunctionSpaceType :: FunctionSpaceType  FunctionSpaceType;
     static const int polynomialOrder = DiscreteFunctionSpaceType :: polynomialOrder ;
 
     typedef typename DiscreteFunctionSpaceType :: GridPartType    GridPartType;
     typedef typename GridPartType::GridType                       GridType;
 
-    typedef typename GridType :: Communication          CommunicationType;
-    typedef TimeProvider< CommunicationType >           TimeProviderType;
+    typedef typename GridType :: CollectiveCommunication          CollectiveCommunicationType;
+    typedef TimeProvider< CollectiveCommunicationType >           TimeProviderType;
 
     typedef typename AdvectionLimiterFunctionSelector<
       typename FunctionSpaceType::DomainFieldType, limiterFunctionId > :: type
       LimiterFunctionType;
 
 
     typedef detail::EmptyProblem< AdvectionModel > ProblemType;
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/discretemodelcommon.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/discretemodelcommon.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/fluxdiscretemodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/fluxdiscretemodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/fluxoperator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/fluxoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/operatorbase.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/operatorbase.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/operatortraits.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/operatortraits.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/primaldiscretemodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/primaldiscretemodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/dg/primaloperator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/dg/primaloperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/fluxbase.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/fluxbase.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/fluxes.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/fluxes.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/llfadvflux.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/llfadvflux.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/noflux.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/noflux.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/parameters.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/parameters.hh`

 * *Files 9% similar despite different names*

```diff
@@ -34,16 +34,14 @@
       general,
 
       /////////////// euler fluxes //////////////////////////////
       //! the local Lax-Friedrichs flux (with wellbalance option)
       euler_llf,
       //! the Harten, Lax and van Leer (HLL) flux
       euler_hll,
-      //! the Harten, Lax and van Leer (HLL) flux with potential temperature formulation
-      euler_hll_pt,
       //! the HLLC flux
       euler_hllc,
       //! general flux: Parameter selection is done via parameter file!
       euler_general,
 
       /////////////// mhd fluxes //////////////////////////////
       mhd_dw,
@@ -53,20 +51,20 @@
       //! a flux implemented by the user and provided to the python code
       //! for C++ just add another enum id
       userdefined
     };
 
     //! Contains all known enums for advection fluxes which can be chosen via parameter file.
     const Enum        _enums[] = { Enum::none, Enum::upwind, Enum::llf,
-                                   Enum::euler_llf, Enum::euler_hll, Enum::euler_hll_pt, Enum::euler_hllc,
+                                   Enum::euler_llf, Enum::euler_hll, Enum::euler_hllc,
                                    Enum::mhd_dw, Enum::mhd_hllem
                                    };
     //! Contains all known names of advection fluxes which can be chosen via parameter file.
     const std::string _strings[] = { "NONE", "UPWIND" , "LLF",
-                                     "EULER-LLF", "EULER-HLL" , "EULER-HLL-PT", "EULER-HLLC",
+                                     "EULER-LLF", "EULER-HLL" , "EULER-HLLC",
                                      "MHD-DW", "MHD-HLLEM"
                                      };
     //! Number of known advection fluxes which can be chosen via parameter file.
     static const int  _size = 8;
 
   }
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/python.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/python.hh`

 * *Files 12% similar despite different names*

```diff
@@ -96,24 +96,14 @@
      */
     DGAdvectionFluxPythonUserDefine (const ModelType& model,
                                      const ParameterType& parameter )
       : BaseType( model, parameter )
     {
     }
 
-    /**
-     * \brief Copy Constructor
-     *
-     * \param[in] other  object to copy
-     */
-    DGAdvectionFluxPythonUserDefine (const DGAdvectionFluxPythonUserDefine& other )
-      : BaseType( other.model_ )
-    {
-    }
-
   protected:
     std::unique_ptr< const ModelType > modelPtr_;
   };
 
 } // end namespace Fem
 } // end namespace Dune
 #endif
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/upwindflux.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/upwindflux.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/advection/userdefined.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/advection/userdefined.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/analyticaleulerflux.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/analyticaleulerflux.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/dgprimalfluxes.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/dgprimalfluxes.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/fluxbase.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/fluxbase.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/fluxes.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/fluxes.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/ldgflux.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/ldgflux.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/diffusion/parameters.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/diffusion/parameters.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/eulerflux_impl.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/eulerflux_impl.hh`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 {
   ////////////////////////////////////////////////////////
   //
   // Implementation of Euler fluxes from Dennis Diehl.
   //
   ////////////////////////////////////////////////////////
 
-  typedef enum {LLF, HLL, HLL_PT, HLLC} EulerFluxType;
+  typedef enum {LLF, HLL, HLLC} EulerFluxType;
   const EulerFluxType std_flux_type = HLL;
 
   /**
   *  \brief Advection flux for the euler problem.
   *
   *  \ingroups AdvectionFluxes
   */
@@ -70,22 +70,19 @@
       }
 
     }
 
     FieldType num_flux(const FieldType Uj[dim+2], const FieldType Un[dim+2],
                        const FieldType normal[dim], FieldType gj[dim+2]) const
     {
-      if constexpr (flux_type == LLF) return num_flux_LLF(Uj, Un, normal, gj);
+      if (flux_type == LLF) return num_flux_LLF(Uj, Un, normal, gj);
 
-      if constexpr (flux_type == HLL) return num_flux_HLL(Uj, Un, normal, gj, std::false_type());
+      if (flux_type == HLL) return num_flux_HLL(Uj, Un, normal, gj);
 
-      // potential temperature
-      if constexpr (flux_type == HLL_PT) return num_flux_HLL(Uj, Un, normal, gj, std::true_type());
-
-      if constexpr (flux_type == HLLC) return num_flux_HLLC(Uj, Un, normal, gj);
+      if (flux_type == HLLC) return num_flux_HLLC(Uj, Un, normal, gj);
 
       DUNE_THROW( Dune::NotImplemented, "Numerical flux not implemented" );
     }
 
     const Model& model_;
     const FieldType _gamma;
 
@@ -141,42 +138,36 @@
       }
       gj[dim+1] = 0.5 * (gj[dim+1] - alpha*(En - Ej));
 
       return alpha;
     }
 
 
-    template <bool pottemp>
     FieldType num_flux_HLL(const FieldType Uj[dim+2], const FieldType Un[dim+2],
-                           const FieldType normal[dim], FieldType gj[dim+2],
-                           const std::integral_constant<bool, pottemp> ) const
+                           const FieldType normal[dim], FieldType gj[dim+2]) const
     {
-      static constexpr bool potentialTemperature = pottemp;
-
       const FieldType rhoj = Uj[0];
       FieldType Ej = Uj[dim+1];
       const FieldType rhon = Un[0];
       FieldType En = Un[dim+1];
-
-      if constexpr (potentialTemperature)
-      {
-        FieldType pressj, tempj;
-        FieldType pressn, tempn;
-        model_.pressureTemperature( Uj, pressj, tempj );
-        model_.pressureTemperature( Un, pressn, tempn );
-
-        FieldType Ekinj = 0;
-        FieldType Ekinn = 0;
-        for(int i=1; i<dim+1; i++){
-          Ekinj += (0.5/rhoj) * Uj[i] * Uj[i];
-          Ekinn += (0.5/rhon) * Un[i] * Un[i];
-        }
-        Ej = pressj/(_gamma-1.) + Ekinj;
-        En = pressn/(_gamma-1.) + Ekinn;
-      }
+#ifdef POTTEMP
+      FieldType pressj, tempj;
+      FieldType pressn, tempn;
+      model_.pressAndTemp( Uj, pressj, tempj );
+      model_.pressAndTemp( Un, pressn, tempn );
+
+      FieldType Ekinj = 0;
+      FieldType Ekinn = 0;
+      for(int i=1; i<dim+1; i++){
+        Ekinj += (0.5/rhoj) * Uj[i] * Uj[i];
+        Ekinn += (0.5/rhon) * Un[i] * Un[i];
+      }
+      Ej = pressj/(_gamma-1.) + Ekinj;
+      En = pressn/(_gamma-1.) + Ekinn;
+#endif
 
       FieldType rho_uj[dim], rho_un[dim], uj[dim], un[dim];
       FieldType Ekin2j=0.0, Ekin2n=0.0;
       rotate(normal, Uj+1, rho_uj);
       rotate(normal, Un+1, rho_un);
       for(int i=0; i<dim; i++){
         uj[i] = (1.0/rhoj) * rho_uj[i];
@@ -209,77 +200,74 @@
       if (u_star > 0.0){
         if (sj >= 0.0){
           gj[0] = rho_uj[0];
 
           for(int i=0; i<dim; i++) guj[i] = rho_uj[i]*uj[0];
           guj[0] += pj;
 
-          if constexpr (potentialTemperature)
-            gj[dim+1] = Uj[dim+1]*uj[0];
-          else
-            gj[dim+1] = (Ej+pj)*uj[0];
+#ifdef POTTEMP
+          gj[dim+1] = Uj[dim+1]*uj[0];
+#else
+          gj[dim+1] = (Ej+pj)*uj[0];
+#endif
         }
         else{
           const FieldType tmp1 = sj * sn;
           const FieldType tmp2 = 1.0/(sn - sj);
           gj[0] = tmp2 * ( sn*rho_uj[0] - sj*rho_un[0] + tmp1*(rhon - rhoj) );
 
           for(int i=0; i<dim; i++){
             guj[i] = tmp2*((sn*uj[0]-tmp1)*rho_uj[i] - (sj*un[0]-tmp1)*rho_un[i]);
           }
           guj[0] += tmp2 * (sn*pj - sj*pn);
 
-          if constexpr(potentialTemperature)
-          {
-            const FieldType Etmpj = Uj[dim+1]*uj[0];
-            const FieldType Etmpn = Un[dim+1]*un[0];
-            gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(Un[dim+1] - Uj[dim+1]));
-          }
-          else
-          {
-            const FieldType Etmpj = (Ej+pj)*uj[0];
-            const FieldType Etmpn = (En+pn)*un[0];
-            gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(En - Ej));
-          }
+#ifdef POTTEMP
+          const FieldType Etmpj = Uj[dim+1]*uj[0];
+          const FieldType Etmpn = Un[dim+1]*un[0];
+          gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(Un[dim+1] - Uj[dim+1]));
+#else
+          const FieldType Etmpj = (Ej+pj)*uj[0];
+          const FieldType Etmpn = (En+pn)*un[0];
+          gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(En - Ej));
+#endif
         }
       }
       else{
         if (sn <= 0.0){
           gj[0] = rho_un[0];
 
           for(int i=0; i<dim; i++) guj[i] = rho_un[i]*un[0];
           guj[0] += pn;
 
-          if constexpr(potentialTemperature)
-            gj[dim+1] = Uj[dim+1]*un[0];
-          else
-            gj[dim+1] = (En+pn)*un[0];
+#ifdef POTTEMP
+          gj[dim+1] = Uj[dim+1]*un[0];
+#else
+          gj[dim+1] = (En+pn)*un[0];
+#endif
         }
         else{
           const FieldType tmp1 = sj * sn;
           const FieldType tmp2 = 1.0/(sn - sj);
           gj[0] = tmp2 * ( sn*rho_uj[0] - sj*rho_un[0] + tmp1*(rhon - rhoj) );
 
           for(int i=0; i<dim; i++){
             guj[i] = tmp2*((sn*uj[0]-tmp1)*rho_uj[i] - (sj*un[0]-tmp1)*rho_un[i]);
           }
           guj[0] += tmp2 * (sn*pj - sj*pn);
 
-          if constexpr(potentialTemperature)
-          {
-            const FieldType Etmpj = Uj[dim+1]*uj[0];
-            const FieldType Etmpn = Un[dim+1]*un[0];
-            gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(Un[dim+1] - Uj[dim+1]));
-          }
-          else
-          {
-            const FieldType Etmpj = (Ej+pj)*uj[0];
-            const FieldType Etmpn = (En+pn)*un[0];
-            gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(En - Ej));
-          }
+#ifdef POTTEMP
+          const FieldType Etmpj = Uj[dim+1]*uj[0];
+          const FieldType Etmpn = Un[dim+1]*un[0];
+          gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(Un[dim+1] - Uj[dim+1]));
+#else
+          const FieldType Etmpj = (Ej+pj)*uj[0];
+          const FieldType Etmpn = (En+pn)*un[0];
+          gj[dim+1] = tmp2 * (sn*Etmpj-sj*Etmpn + tmp1*(En - Ej));
+#endif
+
         }
       }
 
       rotate_inv(normal, guj, gj+1);
       return (std::abs(sj) > std::abs(sn))? std::abs(sj): std::abs(sn);
     }
 
@@ -490,15 +478,15 @@
   public:
     typedef typename BaseType::ModelType          ModelType;
     typedef typename BaseType::ParameterType      ParameterType;
 
     /**
      * \copydoc DGAdvectionFluxBase::DGAdvectionFluxBase()
      */
-    EulerFluxImpl (const ModelImp& mod, const ParameterType& parameter = ParameterType() )
+    EulerFluxImpl (const ModelImp& mod )
       : BaseType( mod ),
         numFlux_( mod )
     {}
 
     /**
      * \copydoc DGAdvectionFluxBase::numericalFlux()
      */
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/fluxes.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/fluxes.hh`

 * *Files 5% similar despite different names*

```diff
@@ -56,33 +56,14 @@
   /**
    * \brief class specialization for the HLLC flux.
    *
    * The purpose of this class is to allow the selection of an Euler flux
    * via an enum given in AdvectionFlux::Enum.
    */
   template< class Model >
-  class DGAdvectionFlux< Model, AdvectionFlux::Enum::euler_hll_pt >
-    : public EulerFluxImpl< Model, EulerNumFlux::EulerFlux<Model,EulerNumFlux::EulerFluxType::HLL_PT > >
-  {
-    typedef EulerFluxImpl< Model, EulerNumFlux::EulerFlux<Model,EulerNumFlux::EulerFluxType::HLL_PT > > BaseType ;
-  public:
-    template< class ... Args>
-    DGAdvectionFlux(  Args&&... args )
-      : BaseType( std::forward<Args>(args)... )
-    {}
-    static std::string name () { return "HLL_PT (Dennis)"; }
-  };
-
-  /**
-   * \brief class specialization for the HLLC flux.
-   *
-   * The purpose of this class is to allow the selection of an Euler flux
-   * via an enum given in AdvectionFlux::Enum.
-   */
-  template< class Model >
   class DGAdvectionFlux< Model, AdvectionFlux::Enum::euler_hllc >
     : public EulerFluxImpl< Model, EulerNumFlux::EulerFlux<Model,EulerNumFlux::EulerFluxType::HLLC > >
   {
     typedef EulerFluxImpl< Model, EulerNumFlux::EulerFlux<Model,EulerNumFlux::EulerFluxType::HLLC > > BaseType ;
   public:
     template< class ... Args>
     DGAdvectionFlux(  Args&&... args )
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/llfadv.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/llfadv.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/euler/parameters.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/euler/parameters.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_eqns.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.cc` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhd_fluxes.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/mhd/mhdfluxes.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/mhd/mhdfluxes.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/fluxes/rotator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/fluxes/rotator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limiter.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limiter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limiterdiscretemodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limiterdiscretemodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limitermodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limitermodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limiterutility.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limiterutility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/limitpass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/limitpass.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/lpreconstruction.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/lpreconstruction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/scalinglimitpass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/scalinglimitpass.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/operator/limiter/smoothness.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/operator/limiter/smoothness.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/context.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/context.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dginversemass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dginversemass.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dgmasspass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dgmasspass.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/dgpass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/dgpass.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/discretemodel.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/discretemodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/insertfunction.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/insertfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/insertoperator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/insertoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/localfunctiontuple.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/localfunctiontuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/modelcaller.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/modelcaller.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/pass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/pass.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/selector.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/selector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/pass/threadpass.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/pass/threadpass.hh`

 * *Files 1% similar despite different names*

```diff
@@ -546,20 +546,16 @@
         this->numberOfElements_ = pass( 0 ).numberOfElements();
       }
 
       // if useNonBlockingComm_ is disabled then communicate here if communication is required
       if( requireCommunication_ && ! nonBlockingComm_.nonBlockingCommunication() )
       {
         assert( dest_ );
-
-        if( dest_ )
-        {
-          // communicate calculated function
-          dest_->communicate();
-        }
+        // communicate calculated function
+        dest.communicate();
       }
 
       // remove pointers
       arg_  = 0;
       dest_ = 0;
     }
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/python/operator.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/python/operator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/dghelmholtzinverse.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/dghelmholtzinverse.hh`

 * *Files 2% similar despite different names*

```diff
@@ -119,21 +119,20 @@
 
       typedef Dune::Fem::DGHelmholtzOperatorWithUpdate< SpaceOperatorType >     HelmholtzOperatorType;
       typedef Dune::Fem::NewtonInverseOperator< typename HelmholtzOperatorType::JacobianOperatorType,
                                                 LinearInverseOperatorType >     NonlinearInverseOperatorType;
 
       struct SolverInfo
       {
-        SolverInfo ( bool converged, int linearIterations, int nonlinearIterations, double residualNorm )
-          : converged( converged ), linearIterations( linearIterations ), nonlinearIterations( nonlinearIterations ), residualNorm( residualNorm )
+        SolverInfo ( bool converged, int linearIterations, int nonlinearIterations )
+          : converged( converged ), linearIterations( linearIterations ), nonlinearIterations( nonlinearIterations )
         {}
 
         bool converged;
         int linearIterations, nonlinearIterations;
-        double residualNorm;
       };
 
       // class wrapping a Python function to look like a Fem::Operator
       class PreconditionerWrapper : public virtual Operator< DestinationType, DestinationType >
       {
         const PreconditionerType& pre_; // function given from Python side
       public:
@@ -168,15 +167,14 @@
 
       /** \brief set Newton tolerance */
       void setTolerance( const double tol )
       {
         typedef DestinationType RangeFunctionType;
         auto finished = [ tol ] ( const RangeFunctionType &w, const RangeFunctionType &dw, double res ) { return res < tol; };
         invOp_.setErrorMeasure( finished );
-        invOp_.eisenstatWalker().setTolerance( tol );
       }
 
       /** solve
        *
        * @f[
        * L[\bar{u} + \lambda u ] = rhs
        * @f]
@@ -205,15 +203,15 @@
       {
         helmholtzOp_.setLambda( lambda );
 
         // apply inv op
         (*this)( rhs, u );
 
         helmholtzOp_.unbind();
-        return SolverInfo( invOp_.converged(), invOp_.linearIterations(), invOp_.iterations(), invOp_.residual() );
+        return SolverInfo( invOp_.converged(), invOp_.linearIterations(), invOp_.iterations() );
       }
 
       /** \brief Preconditioned solve
        *
        * @f[
        * L[\bar{u} + \lambda u ] = rhs
        * @f]
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/rungekuttasolver.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/rungekuttasolver.hh`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
       }
     };
 
   public:
     typedef typename OperatorType :: DestinationType DestinationType ;
     typedef DestinationType  DiscreteFunctionType;
     typedef typename DiscreteFunctionType :: DiscreteFunctionSpaceType :: GridType GridType;
-    typedef typename GridType :: Communication            CommunicationType;
-    typedef Dune::Fem::TimeProvider< CommunicationType >  TimeProviderType;
+    typedef typename GridType :: CollectiveCommunication            CollectiveCommunicationType;
+    typedef Dune::Fem::TimeProvider< CollectiveCommunicationType >  TimeProviderType;
 
     typedef DuneODE :: OdeSolverInterface< DestinationType >        OdeSolverInterfaceType;
     typedef typename OdeSolverInterfaceType :: MonitorType MonitorType;
 
     typedef DiscreteFunctionType DomainFunctionType;
     typedef DiscreteFunctionType RangeFunctionType;
```

### Comparing `dune-fem-dg-2.9.0rc1/dune/fem-dg/solver/uzawa.hh` & `dune-fem-dg-2.9.dev20220529/dune/fem-dg/solver/uzawa.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/activeindexmapper.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/activeindexmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/axisalignedreferencefaces.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/axisalignedreferencefaces.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/densesubvector.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/densesubvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/fieldmatrix.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/fieldmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/getreference.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/getreference.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/integerrange.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/integerrange.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/matrix.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/matrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/common/smallobject.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/common/smallobject.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/constraint/linear.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/constraint/linear.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/lp.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/lp.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/minimize.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/minimize.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/qp/combinedgauss.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/qp/combinedgauss.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/qp/gradient.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/qp/gradient.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/qp/reducedgauss.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/qp/reducedgauss.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/qp.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/qp.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/solver/fullydynmatrix.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/solver/fullydynmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/solver/gauss.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/solver/gauss.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/solver/gaussjordan.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/solver/gaussjordan.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/solver/rowrefvector.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/solver/rowrefvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/std/iterator.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/std/iterator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/dune/optim/std/subarray.hh` & `dune-fem-dg-2.9.dev20220529/dune/optim/std/subarray.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/adrsolver/adrsolver.py` & `dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/adrsolver.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/adrsolver/scalar.py` & `dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/scalar.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/adrsolver/scheme.py` & `dune-fem-dg-2.9.dev20220529/pydemo/adrsolver/scheme.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/advection.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/advection.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/advection_model.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/advection_model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/chemical.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/chemical.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/chemical_model.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/chemical_model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/euler_kh.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/euler_kh.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/euler_model.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/euler_model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/euler_sb.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/euler_sb.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/evolve.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/evolve.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/modalindicator.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/modalindicator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/ns_kh.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/ns_kh.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/ns_model.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/ns_model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/residual.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/residual.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/shockvortex_naffine.dgf` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/shockvortex_naffine.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/sw.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/sw.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/sw_model.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/sw_model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/sw_wb.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/sw_wb.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/test.py` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/test.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/utility.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/utility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/camc-paper/wb.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/camc-paper/wb.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemesh.msh` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemesh.msh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemeshfine.msh` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemeshfine.msh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/circlemeshquad.msh` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/circlemeshquad.msh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/main.py` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/main.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/micap.py` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/micap.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/micap1.py` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/micap1.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/paper.py` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/paper.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/chemicalreaction/test.py` & `dune-fem-dg-2.9.dev20220529/pydemo/chemicalreaction/test.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/CMakeLists.txt` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/chorin.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/chorin.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/compare.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/compare.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/euler.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/euler.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/euler_effcomp.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/euler_effcomp.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/llf.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/llf.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/main.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/main.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/paper.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/paper.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/rk.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/rk.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/sod.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/sod.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/testdg.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/testdg.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/testfv0.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/testfv0.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/testfv1.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/testfv1.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/euler/testpolyfv1.py` & `dune-fem-dg-2.9.dev20220529/pydemo/euler/testpolyfv1.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/eulerufl/dolfin_dg.patch` & `dune-fem-dg-2.9.dev20220529/pydemo/eulerufl/dolfin_dg.patch`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/eulerufl/euler_test.py` & `dune-fem-dg-2.9.dev20220529/pydemo/eulerufl/euler_test.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/fulltest.py` & `dune-fem-dg-2.9.dev20220529/pydemo/fulltest.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/paramSolver` & `dune-fem-dg-2.9.dev20220529/pydemo/paramSolver`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/paramThreading` & `dune-fem-dg-2.9.dev20220529/pydemo/paramThreading`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/rk/euler.py` & `dune-fem-dg-2.9.dev20220529/pydemo/rk/euler.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/rk/main.py` & `dune-fem-dg-2.9.dev20220529/pydemo/rk/main.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/rk/scheme.py` & `dune-fem-dg-2.9.dev20220529/pydemo/rk/scheme.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/rk/shock_tube_fast.py` & `dune-fem-dg-2.9.dev20220529/pydemo/rk/shock_tube_fast.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/scalar/main.py` & `dune-fem-dg-2.9.dev20220529/pydemo/scalar/main.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/scalar/rk.py` & `dune-fem-dg-2.9.dev20220529/pydemo/scalar/rk.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/scalar/scalar.py` & `dune-fem-dg-2.9.dev20220529/pydemo/scalar/scalar.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/shallowWater/llf.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/llf.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/shallowWater/llfwb.hh` & `dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/llfwb.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/shallowWater/main.py` & `dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/main.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pydemo/shallowWater/shallowwater.py` & `dune-fem-dg-2.9.dev20220529/pydemo/shallowWater/shallowwater.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/pyproject.toml` & `dune-fem-dg-2.9.dev20220529/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # This is uses the `Python-Requires` field in the `dune.modules` file to
 # populate the `requires` entry. Additional packages needed for the package
 # build should be added in the `dune.modules`. These packages will then also be
 # included in the package install from source.
 #
 [build-system]
-requires = ['cmake>=3.13', 'dune-fem<=v2.9.0rc1', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
+requires = ['cmake>=3.13', 'dune-fem<=2.9.dev20220529', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
```

### Comparing `dune-fem-dg-2.9.0rc1/python/dune/femdg/__main__.py` & `dune-fem-dg-2.9.dev20220529/python/dune/femdg/__main__.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/python/dune/femdg/_operators.py` & `dune-fem-dg-2.9.dev20220529/python/dune/femdg/_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,14 @@
                                  {
                                    self.setTolerance( tol );
                                    auto info = self.solve(rhs, u, lambda);
                                    pybind11::dict ret;
                                    ret["converged"]  = pybind11::cast(info.converged);
                                    ret["iterations"] = pybind11::cast(info.nonlinearIterations);
                                    ret["linear_iterations"] = pybind11::cast(info.linearIterations);
-                                   ret["residual"] = pybind11::cast(info.residualNorm);
                                    return ret;
                                  }''' )
     # add method solve, combining setLambda and __call__ for efficiency. Also,
     # here some solver diagnostics can be returned
     preCondSolve = Method('_preconditionedSolve', '''[]( DuneType &self,
                                                         const typename DuneType::PreconditionerType& p,
                                                         const typename DuneType::UpdatePreconditionerType& up,
@@ -654,15 +653,14 @@
                                  {
                                    self.setTolerance( tol );
                                    auto info = self.preconditionedSolve(p, up, rhs, u, lambda);
                                    pybind11::dict ret;
                                    ret["converged"]  = pybind11::cast(info.converged);
                                    ret["iterations"] = pybind11::cast(info.nonlinearIterations);
                                    ret["linear_iterations"] = pybind11::cast(info.linearIterations);
-                                   ret["residual"] = pybind11::cast(info.residualNorm);
                                    return ret;
                                  }''' )
 
 
     op = load(includes, typeName, constructor, setLambda, solve, preCondSolve).Operator( op, parameters )
 
     # add method solve with default parameter for tolerance
```

### Comparing `dune-fem-dg-2.9.0rc1/python/dune/femdg/patch.py` & `dune-fem-dg-2.9.dev20220529/python/dune/femdg/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,24 +184,14 @@
     predefined.update( {x: UnformattedExpression('auto', 'entity.geometry().global( Dune::Fem::coordinate( x ) )') })
     arg_n = Variable("const DDomainType &", "normal")
     predefined.update( {n: arg_n} )
     arg_t = Variable("const double &", "t")
     predefined.update( {t: arg_t} )
     self.predefineCoefficients(predefined,'x')
 
-    # pressure and temperature for potential temperature formulation
-    pressureTemperature = getattr(Model,"pressureTemperature",None)
-    if pressureTemperature is not None:
-        pressureTemperature = pressureTemperature(u)
-    self.generateMethod(code, pressureTemperature,
-          'Dune::FieldVector<double, 2>', 'pressureTemperature',
-          args=['const State &u'],
-          targs=['class State'], const=True, inline=True,
-          predefined=predefined)
-
     maxWaveSpeed = getattr(Model,"maxWaveSpeed",None)
     # check for deprecated maxLambda
     if maxWaveSpeed is None:
         maxWaveSpeed = getattr(Model,"maxLambda",None)
         if maxWaveSpeed is not None:
             print("WARNING: maxLambda is deprecated, use maxWaveSpeed instead!")
```

### Comparing `dune-fem-dg-2.9.0rc1/python/dune/femdg/rk.py` & `dune-fem-dg-2.9.dev20220529/python/dune/femdg/rk.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/python/dune/femdg/testing.py` & `dune-fem-dg-2.9.dev20220529/python/dune/femdg/testing.py`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/PKG-INFO` & `dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-fem-dg
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: The Dune FEM module: Discontinuous Galerkin for evolution equations
 Home-page: https://www.dune-project.org/modules/dune-fem-dg/
 Author: Andreas Dedner, Tobias Malkmus, Robert Kloefkorn, Stefan Wierling (geb. Girke)
 Author-email: dune-fem@lists.dune-project.org
 License: UNKNOWN
 Description: DUNE-FEM-DG
         ===========
@@ -83,15 +83,15 @@
         
         A documentation for the 2.4 release can be found in
         
         * A. Dedner, S. Girke, R. Klöfkorn, T. Malkmus. 2017. The DUNE-FEM-DG module.
         Archive of Numerical Software 5(1): 21--61. http://dx.doi.org/10.11588/ans.2017.1.28602
         
         
-        git-8685c1f074de90182ab41cda4d4836a8f903b30d
+        git-3b4ad3b8d6449914d9b2aa333457451b45ab81cb
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-fem-dg-2.9.0rc1/python/dune_fem_dg.egg-info/SOURCES.txt` & `dune-fem-dg-2.9.dev20220529/python/dune_fem_dg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/build-dune-fem-dg.sh` & `dune-fem-dg-2.9.dev20220529/scripts/build-dune-fem-dg.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/check-dist.sh` & `dune-fem-dg-2.9.dev20220529/scripts/check-dist.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/check-header.sh` & `dune-fem-dg-2.9.dev20220529/scripts/check-header.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/check-headers.sh` & `dune-fem-dg-2.9.dev20220529/scripts/check-headers.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/check-opts.sh` & `dune-fem-dg-2.9.dev20220529/scripts/check-opts.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/check-tests.sh` & `dune-fem-dg-2.9.dev20220529/scripts/check-tests.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/fullcheck.sh` & `dune-fem-dg-2.9.dev20220529/scripts/fullcheck.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/mpiexec.sh` & `dune-fem-dg-2.9.dev20220529/scripts/mpiexec.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-dg-2.9.0rc1/scripts/update-dune-modules.sh` & `dune-fem-dg-2.9.dev20220529/scripts/update-dune-modules.sh`

 * *Files 1% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
 # NOTE: if conflicts arise due to diverging repositories then fix these
 # conflicts and re-run the script
 # Optional: clean the build directories of all modules to invoke a build from
 # scratch, i.e.
 # MODULES=`./dune-common/bin/dunecontrol print 2>/dev/null`
 MODULES=
-for MOD in $MODULES; do
+for MOD in MODULES; do
   rm -rf $MOD/build-cmake
 done
 
 # build all DUNE modules using dune-control
 ./dune-common/bin/dunecontrol --opts=config.opts all
```

