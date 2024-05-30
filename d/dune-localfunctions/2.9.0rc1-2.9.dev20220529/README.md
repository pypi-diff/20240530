# Comparing `tmp/dune-localfunctions-2.9.0rc1.tar.gz` & `tmp/dune-localfunctions-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-localfunctions-2.9.0rc1.tar", last modified: Fri Oct 21 08:16:51 2022, max compression
+gzip compressed data, was "dune-localfunctions-2.9.dev20220529.tar", last modified: Sun May 29 21:03:30 2022, max compression
```

## Comparing `dune-localfunctions-2.9.0rc1.tar` & `dune-localfunctions-2.9.dev20220529.tar`

### file list

```diff
@@ -1,373 +1,359 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6057 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20262 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)    20262 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    19036 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/doc/doxygen/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/doc/doxygen/modules.txt
--rw-r--r--   0 runner    (1001) docker     (121)    59202 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/doc/dune-localfunctions-manual.tex
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/localfunctions/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/bdfmcube.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11700 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/localcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8172 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/localinterpolation.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.960005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11766 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     5131 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalbasis.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1342 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalcoefficients.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3661 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalinterpolation.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2461 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10904 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9446 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinicube.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinisimplex.hh
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10296 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/interface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/interfaceswitch.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localfiniteelementtraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localfiniteelementvariant.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4907 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localfiniteelementvariantcache.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localkey.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11203 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localtoglobaladaptors.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10809 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/virtualinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9645 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/common/virtualwrappers.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/crouzeixraviart.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/dualp1localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/dualp1localcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/dualp1localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualpq1factory.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4166 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/dualq1localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/dualq1localcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/dualq1localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7178 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/test/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9109 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/test/test-biorthogonality.cc
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11779 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15950 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/hierarchicalsimplexp2withelementbubble.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.964005 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8637 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2.hh
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/emptypoints.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6987 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/equidistantpoints.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangebasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangecoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23531 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangecube.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5249 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangelfecache.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28034 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangeprism.hh
--rw-r--r--   0 runner    (1001) docker     (121)    33578 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangepyramid.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28663 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangesimplex.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/p0localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/p0localcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/p0localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0.hh
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p1.hh
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p2.hh
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p23d.hh
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pk.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5833 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pk1d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pk2d.hh
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pk3d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pq22d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5505 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pqkfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/prismp1.hh
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/prismp2.hh
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pyramidp1.hh
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pyramidp2.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/q1.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/q2.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/qk.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3376 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3949 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/basis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/coefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4585 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/mimetic/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/mimetic/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/mimetic/mimeticall.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/mimetic.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9371 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/monomiallocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/monomiallocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/monomiallocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18142 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelec1stkindcube.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14848 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelec1stkindsimplex.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23309 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexprebasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal/orthonormalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5537 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal/orthonormalcompute.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.968005 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek2d/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3969 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek2d/rannacherturek2dlocalbasis.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek3d/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek3d/rannacherturek3dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannachertureklocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannachertureklocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannachertureklocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6073 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube2d/raviartthomas0cube2dall.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube3d/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8273 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube3d/raviartthomas0cube3dall.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube3d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2663 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7102 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    24935 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6222 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.972005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17407 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20117 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6004 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    28131 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6280 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomascube.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomaslfecache.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15013 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6219 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexprebasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/common/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/common/refinedsimplexlocalbasis.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/refinedp0localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/refinedp0localcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/refinedp0localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5386 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp1/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    24729 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp1/refinedp1localbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp1.hh
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/refined.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.976005 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/bdfmelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/brezzidouglasmarinielementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/crouzeixraviartelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/dualmortarelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6164 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/geometries.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/globalmonomialfunctionstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/hierarchicalelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9673 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/lagrangeshapefunctiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3601 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/monomialshapefunctiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/nedelec1stkindelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/rannacherturekelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6232 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/raviartthomaselementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/refinedelementtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-edges0.5.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10811 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-fe.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-finiteelementcache.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-lagrange.cc
--rw-r--r--   0 runner    (1001) docker     (121)    32209 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-localfe.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-nedelecsimplex.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-orthonormal.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-pk2d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-power-monomial.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-q1.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-q2.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-raviartthomassimplex.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/testgenericfem.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6867 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/test/virtualshapefunctiontest.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4654 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/basisevaluator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6400 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/basismatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/basisprint.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/coeffmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/defaultbasisfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/dglocalcoefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7616 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/field.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/interpolationhelper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8133 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/l2interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/lfematrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6153 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/localfiniteelement.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23277 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/monomialbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11396 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/multiindex.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13309 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/polynomialbasis.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29598 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/tensor.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6613 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/basis.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/coefficients.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/common.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4738 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/dune/python/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/dune/python/localfunctions/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/python/localfunctions/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune/python/localfunctions/localfiniteelement.hh
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune-localfunctions.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/dune.module
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/python/dune/localfunctions/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune/localfunctions/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune/localfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune/localfunctions/_localfunctions.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17828 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:16:51.980005 dune-localfunctions-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:16:51.000000 dune-localfunctions-2.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.951673 dune-localfunctions-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20262 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)    20262 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-05-29 21:03:30.951673 dune-localfunctions-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.927672 dune-localfunctions-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.927672 dune-localfunctions-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/doc/doxygen/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/doc/doxygen/modules.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    59028 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/doc/dune-localfunctions-manual.tex
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.927672 dune-localfunctions-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.927672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.927672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/bdfmcube.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.927672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11525 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/localcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7997 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/localinterpolation.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5849 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11591 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4956 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalbasis.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1167 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalcoefficients.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3486 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalinterpolation.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2286 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10729 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9271 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4640 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinicube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinisimplex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10121 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/interface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10161 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/interfaceswitch.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localfiniteelementtraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13205 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localfiniteelementvariant.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localfiniteelementvariantcache.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localkey.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11028 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localtoglobaladaptors.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10634 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/virtualinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9470 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/virtualwrappers.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7182 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/crouzeixraviart.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.931672 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/dualp1localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/dualp1localcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/dualp1localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualpq1factory.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/dualq1localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/dualq1localcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/dualq1localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7003 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8934 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/test/test-biorthogonality.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11604 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15775 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/hierarchicalsimplexp2withelementbubble.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8462 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/emptypoints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6811 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/equidistantpoints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4258 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangebasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangecoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23356 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangecube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5074 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangelfecache.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27859 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangeprism.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    33403 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangepyramid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28488 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangesimplex.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/p0localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/p0localcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/p0localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p2.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p23d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk1d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5593 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk2d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk3d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pq22d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5330 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pqkfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/prismp1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/prismp2.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pyramidp1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pyramidp2.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/q1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/q2.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/qk.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.935673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3774 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/basis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/coefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4410 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/mimetic/
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/mimetic/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/mimetic/mimeticall.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/mimetic.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9196 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/monomiallocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/monomiallocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/monomiallocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17967 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelec1stkindcube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14673 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelec1stkindsimplex.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23134 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8581 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexprebasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal/orthonormalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5362 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal/orthonormalcompute.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek2d/rannacherturek2dlocalbasis.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek3d/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek3d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek3d/rannacherturek3dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannachertureklocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannachertureklocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannachertureklocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3017 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.939673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5898 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube2d/raviartthomas0cube2dall.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube3d/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube3d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8098 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube3d/raviartthomas0cube3dall.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube3d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6927 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3503 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    24760 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17232 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19942 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5829 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    27956 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6105 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomascube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomaslfecache.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14838 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexprebasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10576 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/common/refinedsimplexlocalbasis.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/refinedp0localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/refinedp0localcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/refinedp0localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5211 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.943673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp1/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    24554 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp1/refinedp1localbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/bdfmelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/brezzidouglasmarinielementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/crouzeixraviartelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/dualmortarelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5989 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/geometries.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/globalmonomialfunctionstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/hierarchicalelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9498 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/lagrangeshapefunctiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3426 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/monomialshapefunctiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/nedelec1stkindelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/rannacherturekelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/raviartthomaselementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/refinedelementtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-edges0.5.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10636 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-fe.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-finiteelementcache.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-lagrange.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    32034 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-localfe.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3816 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-nedelecsimplex.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-orthonormal.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-pk2d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-power-monomial.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-q1.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-q2.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-raviartthomassimplex.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/testgenericfem.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6692 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/virtualshapefunctiontest.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4479 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/basisevaluator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6225 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/basismatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/basisprint.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7610 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/coeffmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/defaultbasisfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/dglocalcoefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7441 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/field.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/interpolationhelper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7958 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/l2interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/lfematrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5978 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/localfiniteelement.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23102 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/monomialbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11221 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/multiindex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13134 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/polynomialbasis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    29419 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/tensor.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6438 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/basis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/coefficients.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/common.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/dune/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/dune/python/localfunctions/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/python/localfunctions/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune/python/localfunctions/localfiniteelement.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune-localfunctions.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/dune.module
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.947673 dune-localfunctions-2.9.dev20220529/python/dune/localfunctions/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune/localfunctions/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune/localfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune/localfunctions/_localfunctions.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:30.951673 dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16951 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:30.951673 dune-localfunctions-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:30.000000 dune-localfunctions-2.9.dev20220529/setup.py
```

### Comparing `dune-localfunctions-2.9.0rc1/CHANGELOG.md` & `dune-localfunctions-2.9.dev20220529/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-<!--
-SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 # Master (will become release 2.9)
 
-* The implementation of the Raviart-Thomas element now also includes 0th order shape functions on prisms and pyramids.
-
 ## Deprecations and removals
 
 - Deprecated many of the Lagrange headers, use
   `lagrange(cube|prism|pyramid|simplex).hh` instead.
 
 # Release 2.8
```

### Comparing `dune-localfunctions-2.9.0rc1/CMakeLists.txt` & `dune-localfunctions-2.9.dev20220529/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # set up project
 project("dune-localfunctions" C CXX)
 
 # general stuff
 cmake_minimum_required(VERSION 3.13)
 
 # guess dune-common build dir
```

### Comparing `dune-localfunctions-2.9.0rc1/COPYING` & `dune-localfunctions-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-localfunctions-2.9.0rc1/INSTALL` & `dune-localfunctions-2.9.dev20220529/INSTALL`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 Installation Instructions
 =========================
 
 For a full explanation of the DUNE installation process please read
 the installation notes [0]. The following introduction is meant for
 the impatient.
```

### Comparing `dune-localfunctions-2.9.0rc1/LICENSE.md` & `dune-localfunctions-2.9.dev20220529/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dune-localfunctions-2.9.0rc1/PKG-INFO` & `dune-localfunctions-2.9.dev20220529/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-localfunctions
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Provides interface and implementation for shape functions defined on the DUNE reference elements
 Home-page: https://gitlab.dune-project.org/core/dune-localfunctions
 Author: The Dune Core developers
 Author-email: dune-devel@lists.dune-project.org
 License: UNKNOWN
-Description: <!--
-        SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-        SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-        -->
-        
-        DUNE-library
+Description: DUNE-library
         ============
         
         DUNE, the Distributed and Unified Numerics Environment is a modular toolbox
         for solving partial differential equations with grid-based methods.
         
         The main intention is to create slim interfaces allowing an efficient use of
         legacy and/or new libraries. Using C++ techniques DUNE allows to use very
@@ -35,15 +30,15 @@
         More information
         ----------------
         
         Check dune-common for more details concerning dependencies, known bugs,
         license and installation.
         
         
-        git-f610b1b0035edeb445499e1db70ace8f062b9067
+        git-e93e57d677b10bb963b4c41cb610c6f250398433
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-localfunctions-2.9.0rc1/README.md` & `dune-localfunctions-2.9.dev20220529/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 DUNE-library
 ============
 
 DUNE, the Distributed and Unified Numerics Environment is a modular toolbox
 for solving partial differential equations with grid-based methods.
 
 The main intention is to create slim interfaces allowing an efficient use of
@@ -27,8 +22,8 @@
 More information
 ----------------
 
 Check dune-common for more details concerning dependencies, known bugs,
 license and installation.
 
 
-git-f610b1b0035edeb445499e1db70ace8f062b9067
+git-e93e57d677b10bb963b4c41cb610c6f250398433
```

### Comparing `dune-localfunctions-2.9.0rc1/config.h.cmake` & `dune-localfunctions-2.9.dev20220529/config.h.cmake`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /* begin dune-localfunctions
    put the definitions for config.h specific to
    your project here. Everything above will be
    overwritten
 */
 /* begin private */
 /* Name of package */
```

### Comparing `dune-localfunctions-2.9.0rc1/doc/doxygen/modules.txt` & `dune-localfunctions-2.9.dev20220529/doc/doxygen/modules.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 /**
  * \defgroup LocalFunctions LocalFunctions
  */
 
 /**
  * \defgroup BrezziDouglasFortinMarini Brezzi-Douglas-Fortin-Marini elements
  * \ingroup LocalFunctions
```

### Comparing `dune-localfunctions-2.9.0rc1/doc/dune-localfunctions-manual.tex` & `dune-localfunctions-2.9.dev20220529/doc/dune-localfunctions-manual.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-% SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 \documentclass[a4paper,11pt]{article}
 \usepackage{multicol}
 \usepackage{amsmath}
 \usepackage{amsfonts}
 \usepackage{xspace}
 \usepackage[body={148mm,240mm,nohead}]{geometry}
 \usepackage[ansinew]{inputenc}
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/bdfmcube.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/bdfmcube.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_BDFMCUBE_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_BDFMCUBE_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/localbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_CUBE_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_CUBE_LOCALBASIS_HH
 
 #include <algorithm>
 #include <array>
 #include <bitset>
 #include <numeric>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/localcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/localcoefficients.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_CUBE_LOCALCOEFFICIENTS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_CUBE_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include <dune/common/math.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasfortinmarini/cube/localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasfortinmarini/cube/localinterpolation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_CUBE_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASFORTINMARINI_CUBE_LOCALINTERPOLATION_HH
 
 #include <algorithm>
 #include <array>
 #include <bitset>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalbasis.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALBASIS_HH
 
 #include <array>
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalcoefficients.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
 
   /**
-   * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Brezzi-Douglas-Marini-1 elements on quadrilaterals
+   * \brief Layout map for Brezzi-Douglas-Marini-2 elements on triangles.
    *
+   * \ingroup LocalLayoutImplementation
    * \nosubgrouping
    * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class BDM1Cube2DLocalCoefficients
+  class BDM2Simplex2DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    BDM1Cube2DLocalCoefficients () : li(8)
+    BDM2Simplex2DLocalCoefficients() : li(12)
     {
-      for (std::size_t i = 0; i < 4; ++i)
+      for (std::size_t i = 0; i < 3; ++i)
       {
-        li[2*i] = LocalKey(i,1,0);
-        li[2*i + 1] = LocalKey(i,1,1);
+        li[3 * i] = LocalKey(i,1,0);
+        li[3 * i + 1] = LocalKey(i,1,1);
+        li[3 * i + 2] = LocalKey(i,1,2);
       }
+
+      // last DOFs are associated with the cell (codim=0)
+      li[9]  = LocalKey(0,0,0);
+      li[10] = LocalKey(0,0,1);
+      li[11] = LocalKey(0,0,2);
     }
 
     //! \brief number of coefficients
-    std::size_t size () const
+    std::size_t size() const
     {
-      return 8;
+      return 12;
     }
 
     //! \brief get i'th index
-    const LocalKey& localKey (std::size_t i) const
+    const LocalKey& localKey(std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
-}
-#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALCOEFFICIENTS_HH
+} // end namespace Dune
+#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalinterpolation.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE2D_LOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
 #include "brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalbasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALBASIS_HH
 
 #include <array>
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d/brezzidouglasmarini1cube2dlocalcoefficients.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
 
   /**
    * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Brezzi-Douglas-Marini-1 elements on hexahedra
+   * \brief Layout map for Brezzi-Douglas-Marini-1 elements on quadrilaterals
    *
    * \nosubgrouping
    * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class BDM1Cube3DLocalCoefficients
+  class BDM1Cube2DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    BDM1Cube3DLocalCoefficients() : li(18)
+    BDM1Cube2DLocalCoefficients () : li(8)
     {
-      for (std::size_t i = 0; i < 6; ++i)
+      for (std::size_t i = 0; i < 4; ++i)
       {
-        li[i] = LocalKey(i,1,0);
-        li[i + 6] = LocalKey(i,1,1);
-        li[i + 12] = LocalKey(i,1,2);
+        li[2*i] = LocalKey(i,1,0);
+        li[2*i + 1] = LocalKey(i,1,1);
       }
     }
 
     //! \brief number of coefficients
-    std::size_t size() const
+    std::size_t size () const
     {
-      return 18;
+      return 8;
     }
 
     //! \brief get i'th index
-    const LocalKey& localKey(std::size_t i) const
+    const LocalKey& localKey (std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
-} // end namespace Dune
-#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALCOEFFICIENTS_HH
+}
+#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE2D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalinterpolation.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,79 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE3D_LOCALFINITEELEMENT_HH
-#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE3D_LOCALFINITEELEMENT_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
-#include "brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalbasis.hh"
-#include "brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalcoefficients.hh"
-#include "brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalinterpolation.hh"
+#include "raviartthomas1cube3d/raviartthomas1cube3dlocalbasis.hh"
+#include "raviartthomas1cube3d/raviartthomas1cube3dlocalcoefficients.hh"
+#include "raviartthomas1cube3d/raviartthomas1cube3dlocalinterpolation.hh"
 
 namespace Dune
 {
   /**
-   * \brief First order Brezzi-Douglas-Marini shape functions on hexahedron.
+   * \brief First order Raviart-Thomas shape functions on cubes.
    *
-   * \ingroup BrezziDouglasMarini
+   * \ingroup RaviartThomas
    *
    * \tparam D Type to represent the field in the domain.
    * \tparam R Type to represent the field in the range.
    */
   template<class D, class R>
-  class BDM1Cube3DLocalFiniteElement
+  class RT1Cube3DLocalFiniteElement
   {
 
   public:
     typedef LocalFiniteElementTraits<
-        BDM1Cube3DLocalBasis<D,R>,
-        BDM1Cube3DLocalCoefficients,
-        BDM1Cube3DLocalInterpolation<BDM1Cube3DLocalBasis<D,R> > > Traits;
+        RT1Cube3DLocalBasis<D,R>,
+        RT1Cube3DLocalCoefficients,
+        RT1Cube3DLocalInterpolation<RT1Cube3DLocalBasis<D,R> > > Traits;
 
     //! \brief Standard constructor
-    BDM1Cube3DLocalFiniteElement()
+    RT1Cube3DLocalFiniteElement ()
     {}
 
     /**
      * \brief Make set number s, where 0 <= s < 64
      *
      * \param s Edge orientation indicator
      */
-    BDM1Cube3DLocalFiniteElement(int s)
-      : basis(s)
-      , interpolation(s)
+    RT1Cube3DLocalFiniteElement (int s) :
+      basis(s),
+      interpolation(s)
     {}
 
-    const typename Traits::LocalBasisType& localBasis() const
+    const typename Traits::LocalBasisType& localBasis () const
     {
       return basis;
     }
 
-    const typename Traits::LocalCoefficientsType& localCoefficients() const
+    const typename Traits::LocalCoefficientsType& localCoefficients () const
     {
       return coefficients;
     }
 
-    const typename Traits::LocalInterpolationType& localInterpolation() const
+    const typename Traits::LocalInterpolationType& localInterpolation () const
     {
       return interpolation;
     }
 
     /** \brief Number of shape functions in this finite element */
     unsigned int size () const
     {
       return basis.size();
     }
 
-    static constexpr GeometryType type()
+    static constexpr GeometryType type ()
     {
       return GeometryTypes::hexahedron;
     }
 
   private:
-    BDM1Cube3DLocalBasis<D,R> basis;
-    BDM1Cube3DLocalCoefficients coefficients;
-    BDM1Cube3DLocalInterpolation<BDM1Cube3DLocalBasis<D,R> > interpolation;
+    RT1Cube3DLocalBasis<D,R> basis;
+    RT1Cube3DLocalCoefficients coefficients;
+    RT1Cube3DLocalInterpolation<RT1Cube3DLocalBasis<D,R> > interpolation;
   };
-} // end namespace Dune
-#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE3D_LOCALFINITEELEMENT_HH
+}
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalbasis.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALBASIS_HH
 
 #include <array>
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalcoefficients.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALCOEFFICIENTS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalinterpolation.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALFINITEELEMENT_HH
-#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALFINITEELEMENT_HH
+#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
-#include "brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalbasis.hh"
-#include "brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalcoefficients.hh"
-#include "brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalinterpolation.hh"
+#include "brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalbasis.hh"
+#include "brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalcoefficients.hh"
+#include "brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalinterpolation.hh"
 
 namespace Dune
 {
-
   /**
-   * \brief First order Brezzi-Douglas-Marini shape functions on triangles.
+   * \brief Second order Brezzi-Douglas-Marini shape functions on triangles.
    *
    * \ingroup BrezziDouglasMarini
    *
    * \tparam D Type to represent the field in the domain.
    * \tparam R Type to represent the field in the range.
    */
   template<class D, class R>
-  class BDM1Simplex2DLocalFiniteElement
+  class BDM2Simplex2DLocalFiniteElement
   {
 
   public:
     typedef LocalFiniteElementTraits<
-        BDM1Simplex2DLocalBasis<D,R>,
-        BDM1Simplex2DLocalCoefficients,
-        BDM1Simplex2DLocalInterpolation<BDM1Simplex2DLocalBasis<D,R> > > Traits;
+        BDM2Simplex2DLocalBasis<D,R>,
+        BDM2Simplex2DLocalCoefficients,
+        BDM2Simplex2DLocalInterpolation<BDM2Simplex2DLocalBasis<D,R> > > Traits;
 
     //! \brief Standard constructor
-    BDM1Simplex2DLocalFiniteElement ()
+    BDM2Simplex2DLocalFiniteElement ()
     {}
 
     /**
      * \brief Make set number s, where 0 <= s < 8
      *
      * \param s Edge orientation indicator
      */
-    BDM1Simplex2DLocalFiniteElement (int s) :
+    BDM2Simplex2DLocalFiniteElement (int s) :
       basis(s),
       interpolation(s)
     {}
 
     const typename Traits::LocalBasisType& localBasis () const
     {
       return basis;
@@ -70,13 +67,13 @@
 
     static constexpr GeometryType type ()
     {
       return GeometryTypes::triangle;
     }
 
   private:
-    BDM1Simplex2DLocalBasis<D,R> basis;
-    BDM1Simplex2DLocalCoefficients coefficients;
-    BDM1Simplex2DLocalInterpolation<BDM1Simplex2DLocalBasis<D,R> > interpolation;
+    BDM2Simplex2DLocalBasis<D,R> basis;
+    BDM2Simplex2DLocalCoefficients coefficients;
+    BDM2Simplex2DLocalInterpolation<BDM2Simplex2DLocalBasis<D,R> > interpolation;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALFINITEELEMENT_HH
+#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalbasis.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_CUBE2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_CUBE2D_LOCALBASIS_HH
 
 #include <array>
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalcoefficients.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_CUBE2D_LOCALCOEFFICIENTS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_CUBE2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalinterpolation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_CUBE2D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_CUBE2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_QUBE2D_LOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_QUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
 #include "brezzidouglasmarini2cube2d/brezzidouglasmarini2cube2dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalbasis.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALBASIS_HH
 
 #include <array>
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalcoefficients.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
 
   /**
-   * \brief Layout map for Brezzi-Douglas-Marini-2 elements on triangles.
+   * @ingroup LocalLayoutImplementation
+   * \brief Layout map for Raviart-Thomas-1 elements on the reference triangle.
    *
-   * \ingroup LocalLayoutImplementation
    * \nosubgrouping
-   * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class BDM2Simplex2DLocalCoefficients
+  class RT12DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    BDM2Simplex2DLocalCoefficients() : li(12)
+    RT12DLocalCoefficients () : li(8)
     {
-      for (std::size_t i = 0; i < 3; ++i)
+      for (std::size_t i = 0; i < 3; i++)
       {
-        li[3 * i] = LocalKey(i,1,0);
-        li[3 * i + 1] = LocalKey(i,1,1);
-        li[3 * i + 2] = LocalKey(i,1,2);
+        li[i] = LocalKey(i,1,0);
+        li[3 + i] = LocalKey(i,1,1);
       }
 
-      // last DOFs are associated with the cell (codim=0)
-      li[9]  = LocalKey(0,0,0);
-      li[10] = LocalKey(0,0,1);
-      li[11] = LocalKey(0,0,2);
+      // last two DOF are associated with the cell (codim = 0)
+      li[6] = LocalKey(0,0,0);
+      li[7] = LocalKey(0,0,1);
     }
 
     //! \brief number of coefficients
-    std::size_t size() const
+    std::size_t size () const
     {
-      return 12;
+      return 8;
     }
 
     //! \brief get i'th index
-    const LocalKey& localKey(std::size_t i) const
+    const LocalKey& localKey (std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
-} // end namespace Dune
-#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALCOEFFICIENTS_HH
+}
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalinterpolation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALFINITEELEMENT_HH
-#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALFINITEELEMENT_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
-#include "brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalbasis.hh"
-#include "brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalcoefficients.hh"
-#include "brezzidouglasmarini2simplex2d/brezzidouglasmarini2simplex2dlocalinterpolation.hh"
+#include "raviartthomas3cube2d/raviartthomas3cube2dlocalbasis.hh"
+#include "raviartthomas3cube2d/raviartthomas3cube2dlocalcoefficients.hh"
+#include "raviartthomas3cube2d/raviartthomas3cube2dlocalinterpolation.hh"
 
 namespace Dune
 {
   /**
-   * \brief Second order Brezzi-Douglas-Marini shape functions on triangles.
+   * \brief Second order Raviart-Thomas shape functions on cubes.
    *
-   * \ingroup BrezziDouglasMarini
+   * \note The Jacobian is not implemented.
+   *
+   * \ingroup RaviartThomas
    *
    * \tparam D Type to represent the field in the domain.
    * \tparam R Type to represent the field in the range.
    */
   template<class D, class R>
-  class BDM2Simplex2DLocalFiniteElement
+  class RT3Cube2DLocalFiniteElement
   {
 
   public:
     typedef LocalFiniteElementTraits<
-        BDM2Simplex2DLocalBasis<D,R>,
-        BDM2Simplex2DLocalCoefficients,
-        BDM2Simplex2DLocalInterpolation<BDM2Simplex2DLocalBasis<D,R> > > Traits;
+        RT3Cube2DLocalBasis<D,R>,
+        RT3Cube2DLocalCoefficients,
+        RT3Cube2DLocalInterpolation<RT3Cube2DLocalBasis<D,R> > > Traits;
 
     //! \brief Standard constructor
-    BDM2Simplex2DLocalFiniteElement ()
+    RT3Cube2DLocalFiniteElement ()
     {}
 
     /**
-     * \brief Make set number s, where 0 <= s < 8
+     * \brief Make set number s, where 0 <= s < 16
      *
      * \param s Edge orientation indicator
      */
-    BDM2Simplex2DLocalFiniteElement (int s) :
+    RT3Cube2DLocalFiniteElement (int s) :
       basis(s),
       interpolation(s)
     {}
 
     const typename Traits::LocalBasisType& localBasis () const
     {
       return basis;
@@ -65,17 +65,17 @@
     unsigned int size () const
     {
       return basis.size();
     }
 
     static constexpr GeometryType type ()
     {
-      return GeometryTypes::triangle;
+      return GeometryTypes::quadrilateral;
     }
 
   private:
-    BDM2Simplex2DLocalBasis<D,R> basis;
-    BDM2Simplex2DLocalCoefficients coefficients;
-    BDM2Simplex2DLocalInterpolation<BDM2Simplex2DLocalBasis<D,R> > interpolation;
+    RT3Cube2DLocalBasis<D,R> basis;
+    RT3Cube2DLocalCoefficients coefficients;
+    RT3Cube2DLocalInterpolation<RT3Cube2DLocalBasis<D,R> > interpolation;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI2_SIMPLEX2D_LOCALFINITEELEMENT_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinicube.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinicube.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI_BREZZIDOUGLASMARINICUBE_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI_BREZZIDOUGLASMARINICUBE_HH
 
 #include <dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube2d.hh>
 #include <dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d.hh>
 #include <dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2cube2d.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinisimplex.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarinisimplex.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI_BREZZIDOUGLASMARINISIMPLEX_HH
 #define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI_BREZZIDOUGLASMARINISIMPLEX_HH
 
 #include <dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d.hh>
 #include <dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini2simplex2d.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/interface.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/interface.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_INTERFACE_HH
 #define DUNE_LOCALFUNCTIONS_INTERFACE_HH
 
 #ifndef HEADERCHECK
 #error This header exists for documentation purposes only and should never be included directly.
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/interfaceswitch.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/interfaceswitch.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_INTERFACESWITCH_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_INTERFACESWITCH_HH
 
 #include <cstddef>
 #include <memory>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localbasis.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_LOCALBASIS_HH
 
 namespace Dune
 {
 
   /**@ingroup LocalBasisInterface
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localfiniteelementvariant.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localfiniteelementvariant.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_LOCALFINITEELEMENTVARIANT_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_LOCALFINITEELEMENTVARIANT_HH
 
 #include <cstddef>
 #include <type_traits>
 #include <variant>
 
@@ -28,15 +26,15 @@
   // Since a generic lambda will in most cases not compile
   // for monostate, we add special empty overloads for monostate.
   // Hence visitIf will simply do nothing in the case of a
   // monostate value.
   template<class Visitor, class Variant>
   void visitIf(Visitor&& visitor, Variant&& variant)
   {
-    auto visitorWithFallback = overload([&](std::monostate&) {},  [&](const std::monostate&) {}, visitor);
+    auto visitorWithFallback = overload([&](std::monostate& impl) {},  [&](const std::monostate& impl) {}, visitor);
     std::visit(visitorWithFallback, variant);
   }
 
   template<class... Implementations>
   class LocalBasisVariant
   {
 
@@ -160,15 +158,15 @@
     {
       // We can't use visitIf since we have to return something
       // even for a monostate value. Since the return type is
       // an l-value reference, we use a default constructed
       // dummy LocalKey value.
       static const Dune::LocalKey dummyLocalKey;
       return std::visit(overload(
-          [&](const std::monostate&) -> decltype(auto) { return (dummyLocalKey);},
+          [&](const std::monostate& impl) -> decltype(auto) { return (dummyLocalKey);},
           [&](const auto* impl) -> decltype(auto) { return impl->localKey(i); }), impl_);
     }
 
   private:
     std::variant<std::monostate, const Implementations*...> impl_;
     std::size_t size_;
   };
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localfiniteelementvariantcache.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localfiniteelementvariantcache.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_LOCALFINITEELEMENTVARIANTCACHE_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_LOCALFINITEELEMENTVARIANTCACHE_HH
 
 #include <vector>
 #include <tuple>
 #include <utility>
 #include <type_traits>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localinterpolation.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_LOCALINTERPOLATION_HH
 
 #include <functional>
 
 #include <dune/common/concept.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localkey.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localkey.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALKEY_HH
 #define DUNE_LOCALKEY_HH
 
 #include <array>
 #include <cstddef>
 #include <ostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/localtoglobaladaptors.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/localtoglobaladaptors.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_LOCALTOGLOBALADAPTORS_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_LOCALTOGLOBALADAPTORS_HH
 
 #include <cstddef>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/virtualinterface.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/virtualinterface.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_VIRTUALINTERFACE_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_VIRTUALINTERFACE_HH
 
 #include <type_traits>
 #include <array>
 #include <vector>
 #include <functional>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/common/virtualwrappers.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/common/virtualwrappers.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_COMMON_VIRTUALWRAPPERS_HH
 #define DUNE_LOCALFUNCTIONS_COMMON_VIRTUALWRAPPERS_HH
 
 #include <array>
 
 #include <dune/localfunctions/common/localbasis.hh>
 #include <dune/localfunctions/common/localkey.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/crouzeixraviart.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/crouzeixraviart.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_CROUZEIXRAVIART_HH
 #define DUNE_LOCALFUNCTIONS_CROUZEIXRAVIART_HH
 
 #include <array>
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/dualp1localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/dualp1localbasis.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DUAL_P1_LOCALBASIS_HH
 #define DUNE_DUAL_P1_LOCALBASIS_HH
 
 #include <numeric>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/dualp1localcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/p0localcoefficients.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_DUAL_P1_LOCALCOEFFICIENTS_HH
-#define DUNE_DUAL_P1_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_P0LOCALCOEFFICIENTS_HH
+#define DUNE_P0LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
+#include <iostream>
 #include <vector>
 
 #include <dune/localfunctions/common/localkey.hh>
 
 namespace Dune
 {
 
-  /** \brief Local coefficients for dual simplex P1 elements
+  /**@ingroup LocalLayoutImplementation
+         \brief Layout map for P0 elements
 
-     \nosubgrouping
+         \nosubgrouping
      \implements Dune::LocalCoefficientsVirtualImp
    */
-  template <int dim>
-  class DualP1LocalCoefficients
+  class P0LocalCoefficients
   {
   public:
     //! \brief Standard constructor
-    DualP1LocalCoefficients () : li(size())
-    {
-      for (std::size_t i=0; i<size(); i++)
-        li[i] = LocalKey(i,dim,0);
-    }
+    P0LocalCoefficients () : index(0,0,0)
+    {}
 
     //! number of coefficients
     std::size_t size () const
     {
-      return dim+1;
+      return 1;
     }
 
     //! get i'th index
-    const LocalKey& localKey (std::size_t i) const
+    const LocalKey& localKey ([[maybe_unused]] std::size_t i) const
     {
-      return li[i];
+      return index;
     }
 
   private:
-    std::vector<LocalKey> li;
+    LocalKey index;
   };
 
 }
-
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1/dualp1localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1/dualp1localinterpolation.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DUAL_P1_LOCALINTERPOLATION_HH
 #define DUNE_DUAL_P1_LOCALINTERPOLATION_HH
 
 #include <vector>
 #include <dune/localfunctions/common/localinterpolation.hh>
 
 namespace Dune
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualp1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualp1.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_DUALMORTARBASIS_DUALP1_HH
 #define DUNE_LOCALFUNCTIONS_DUALMORTARBASIS_DUALP1_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include "dualp1/dualp1localbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualpq1factory.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualpq1factory.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_DUAL_P1_Q1_FACTORY_HH
 #define DUNE_LOCALFUNCTIONS_DUAL_P1_Q1_FACTORY_HH
 
 #include <map>
 
 #include <dune/localfunctions/common/virtualinterface.hh>
 #include <dune/localfunctions/common/virtualwrappers.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/dualq1localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/dualq1localbasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DUAL_Q1_LOCALBASIS_HH
 #define DUNE_DUAL_Q1_LOCALBASIS_HH
 
 #include <array>
 #include <numeric>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/dualq1localcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/dualq1localcoefficients.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DUAL_Q1_LOCALCOEFFICIENTS_HH
 #define DUNE_DUAL_Q1_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <iostream>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1/dualq1localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1/dualq1localinterpolation.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DUAL_Q1_LOCALINTERPOLATION_HH
 #define DUNE_DUAL_Q1_LOCALINTERPOLATION_HH
 
 #include <array>
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/dualq1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/dualq1.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DUAL_Q1_LOCALFINITEELEMENT_HH
 #define DUNE_DUAL_Q1_LOCALFINITEELEMENT_HH
 
 #include <array>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/dualmortarbasis/test/test-biorthogonality.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/dualmortarbasis/test/test-biorthogonality.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <algorithm>
 
 #include <dune/common/fvector.hh>
 
 #include <dune/geometry/quadraturerules.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localbasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_SIMPLEX_P2_LOCALBASIS_HH
 #define DUNE_HIERARCHICAL_SIMPLEX_P2_LOCALBASIS_HH
 
 /** \file
     \brief Hierarchical p2 shape functions for the simplex
  */
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2/hierarchicalsimplexp2localinterpolation.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_SIMPLEX_P2_LOCALINTERPOLATION_HH
 #define DUNE_HIERARCHICAL_SIMPLEX_P2_LOCALINTERPOLATION_HH
 
 #include <vector>
 #include <dune/localfunctions/common/localinterpolation.hh>
 
 namespace Dune
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_P2_LOCALFINITEELEMENT_HH
 #define DUNE_HIERARCHICAL_P2_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include <dune/localfunctions/lagrange/lagrangesimplex.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/hierarchicalsimplexp2withelementbubble.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalp2withelementbubble/hierarchicalsimplexp2withelementbubble.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_SIMPLEX_P2_WITH_ELEMENT_BUBBLE_LOCALBASIS_HH
 #define DUNE_HIERARCHICAL_SIMPLEX_P2_WITH_ELEMENT_BUBBLE_LOCALBASIS_HH
 
 /** \file
     \brief Hierarchical p2 shape functions for the simplex
  */
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_PRISM_P2_LOCALBASIS_HH
 #define DUNE_HIERARCHICAL_PRISM_P2_LOCALBASIS_HH
 
 /** \file
     \brief Hierarchical prism p2 shape functions for the simplex
  */
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2/hierarchicalprismp2localinterpolation.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_PRISM_P2_LOCALINTERPOLATION_HH
 #define DUNE_HIERARCHICAL_PRISM_P2_LOCALINTERPOLATION_HH
 
 #include <vector>
 #include <dune/localfunctions/common/localinterpolation.hh>
 
 namespace Dune
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/hierarchical/hierarchicalprismp2.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/hierarchical/hierarchicalprismp2.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HIERARCHICAL_PRISM_P2_LOCALFINITEELEMENT_HH
 #define DUNE_HIERARCHICAL_PRISM_P2_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include <dune/localfunctions/lagrange/lagrangeprism.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/emptypoints.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/emptypoints.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LAGRANGE_EMPTYPOINTS_HH
 #define DUNE_LAGRANGE_EMPTYPOINTS_HH
 
 #include <vector>
 
 #include <dune/common/fvector.hh>
 #include <dune/localfunctions/common/localkey.hh>
@@ -39,17 +37,17 @@
     }
 
     const Field weight () const
     {
       return weight_;
     }
 
-    Vector point_ = {};
-    LocalKey localKey_ = {};
-    Field weight_ = {};
+    Vector point_;
+    LocalKey localKey_;
+    Field weight_;
   };
 
   // EmptyPointSet
   // --------------
 
   template< class F, unsigned int dim >
   class EmptyPointSet
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/equidistantpoints.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/equidistantpoints.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_EQUIDISTANTPOINTS_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_EQUIDISTANTPOINTS_HH
 
 #include <cstddef>
 
 #include <algorithm>
 #include <vector>
@@ -194,15 +192,15 @@
     }
 
     bool buildCube ()
     {
       return build< GeometryTypes::cube(dim) > ();
     }
 
-    static bool supports ( GeometryType, std::size_t /*order*/ ) { return true; }
+    static bool supports ( GeometryType gt, std::size_t order ) { return true; }
     template< GeometryType::Id geometryId>
     static bool supports ( std::size_t order ) {
       return supports( GeometryType( geometryId ), order );
     }
 
   private:
     using Base::points_;
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/interpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/interpolation.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LAGRANGEBASIS_INTERPOLATION_HH
 #define DUNE_LAGRANGEBASIS_INTERPOLATION_HH
 
 #include <type_traits>
 #include <utility>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangecoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangecoefficients.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LAGRANGECOEFFICIENTS_HH
 #define DUNE_LAGRANGECOEFFICIENTS_HH
 
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangecube.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangecube.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGECUBE_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGECUBE_HH
 
 #include <array>
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangelfecache.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangelfecache.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGELFECACHE_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGELFECACHE_HH
 
 #include <tuple>
 #include <utility>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangeprism.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangeprism.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGEPRISM_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGEPRISM_HH
 
 #include <array>
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangepyramid.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangepyramid.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGEPYRAMID_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGEPYRAMID_HH
 
 #include <array>
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/lagrangesimplex.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/lagrangesimplex.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGESIMPLEX_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_LAGRANGESIMPLEX_HH
 
 #include <array>
 #include <numeric>
 
 #include <dune/common/deprecated.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/p0localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/p0localbasis.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_P0LOCALBASIS_HH
 #define DUNE_P0LOCALBASIS_HH
 
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/p0localcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/refinedp0localcoefficients.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_P0LOCALCOEFFICIENTS_HH
-#define DUNE_P0LOCALCOEFFICIENTS_HH
+#ifndef DUNE_REFINED_P0_LOCALCOEFFICIENTS_HH
+#define DUNE_REFINED_P0_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <iostream>
 #include <vector>
 
 #include <dune/localfunctions/common/localkey.hh>
 
 namespace Dune
 {
 
   /**@ingroup LocalLayoutImplementation
-         \brief Layout map for P0 elements
+     \brief Layout map for RefinedP0 elements
 
-         \nosubgrouping
+     \nosubgrouping
      \implements Dune::LocalCoefficientsVirtualImp
    */
-  class P0LocalCoefficients
+  template<unsigned int k>
+  class RefinedP0LocalCoefficients
   {
+    // 2 to the k-th power
+    constexpr static int N = 1<<k;
+
   public:
-    //! \brief Standard constructor
-    P0LocalCoefficients () : index(0,0,0)
-    {}
+    RefinedP0LocalCoefficients () :
+      localKeys_(N)
+    {
+      // All functions are associated to the element
+      for (int i = 0; i < N; ++i)
+        localKeys_[i] = LocalKey(0,0,i);
+    }
 
     //! number of coefficients
     std::size_t size () const
     {
-      return 1;
+      return N;
     }
 
     //! get i'th index
-    const LocalKey& localKey ([[maybe_unused]] std::size_t i) const
+    const LocalKey& localKey (std::size_t i) const
     {
-      return index;
+      return localKeys_[i];
     }
 
   private:
-    LocalKey index;
+    std::vector<LocalKey> localKeys_;
+
   };
 
 }
+
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0/p0localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0/p0localinterpolation.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_P0LOCALINTERPOLATION_HH
 #define DUNE_P0LOCALINTERPOLATION_HH
 
 #include <vector>
 #include <dune/geometry/referenceelements.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p0.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p0.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_P0LOCALFINITEELEMENT_HH
 #define DUNE_P0LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include "p0/p0localbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk3d.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_P1LOCALFINITEELEMENT_HH
-#define DUNE_P1LOCALFINITEELEMENT_HH
+#ifndef DUNE_Pk3DLOCALFINITEELEMENT_HH
+#define DUNE_Pk3DLOCALFINITEELEMENT_HH
 
 #include <dune/localfunctions/lagrange/lagrangesimplex.hh>
 
 #warning This header is deprecated
 
 namespace Dune
 {
 
-  /** \brief The local p1 finite element on simplices
-      \tparam D Domain data type
-      \tparam R Range data type
-      \tparam dim Dimension of the simplex
+  /** \todo Please doc me !
 
       \deprecated This class is obsolete. Please use LagrangeSimplexLocalFiniteElement instead!
    */
-  template<class D, class R, int dim>
-  using P1LocalFiniteElement
+  template<class D, class R, unsigned int k>
+  using Pk3DLocalFiniteElement
     [[deprecated("use LagrangeSimplexLocalFiniteElement instead")]]
-    = LagrangeSimplexLocalFiniteElement<D,R,dim,1>;
+    = LagrangeSimplexLocalFiniteElement<D,R,3,k>;
 
 }
 
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/p23d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/qk.hh`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_P2_3DLOCALFINITEELEMENT_HH
-#define DUNE_P2_3DLOCALFINITEELEMENT_HH
 
-#include <dune/localfunctions/lagrange/lagrangesimplex.hh>
+#ifndef DUNE_LOCALFUNCTIONS_QK_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_QK_LOCALFINITEELEMENT_HH
+
+#include <dune/localfunctions/lagrange/lagrangecube.hh>
 
 #warning This header is deprecated
 
 namespace Dune
 {
-
-  /** \brief Second-order Lagrange local finite element on the reference tetrahedron
+  /** \brief General Lagrange finite element for cubes with arbitrary dimension and polynomial order
+   *   \note The general class QkLocalCoefficients is available for k>0 in dimensions 2 and 3 only
    *
-   * \tparam D Number type used for domain coordinates
-   * \tparam R Number type used for shape function values
+   * \tparam D type used for domain coordinates
+   * \tparam R type used for function values
+   * \tparam d dimension of the reference element
+   * \tparam k polynomial order
    *
-   * \deprecated This class is obsolete. Please use LagrangeSimplexLocalFiniteElement instead!
+   * \deprecated This class is deprecated!  Please use LagrangeCubeLocalFiniteElement instead.
    */
-  template<class D, class R>
-  using P23DLocalFiniteElement
-    [[deprecated("use LagrangeSimplexLocalFiniteElement instead")]]
-    = LagrangeSimplexLocalFiniteElement<D,R,3,2>;
+  template<class D, class R, int d, int k>
+  using QkLocalFiniteElement
+    [[deprecated("use LagrangeCubeLocalFiniteElement instead")]]
+    = LagrangeCubeLocalFiniteElement<D,R,d,k>;
 
 }
 
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pk1d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk1d.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PK1DLOCALFINITEELEMENT_HH
 #define DUNE_PK1DLOCALFINITEELEMENT_HH
 
 #include <cstddef>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pk2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pk2d.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PK2DLOCALFINITEELEMENT_HH
 #define DUNE_PK2DLOCALFINITEELEMENT_HH
 
 #include <cstddef>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pq22d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pq22d.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PQ22DLOCALFINITEELEMENT_HH
 #define DUNE_PQ22DLOCALFINITEELEMENT_HH
 
 #include <dune/common/fmatrix.hh>
 
 #include <dune/localfunctions/common/localfiniteelementvariant.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pqkfactory.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pqkfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_PQKFACTORY_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_PQKFACTORY_HH
 
 #include <map>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/prismp1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p23d.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_P13DLOCALFINITEELEMENT_HH
-#define DUNE_P13DLOCALFINITEELEMENT_HH
+#ifndef DUNE_P2_3DLOCALFINITEELEMENT_HH
+#define DUNE_P2_3DLOCALFINITEELEMENT_HH
 
-#include <dune/localfunctions/lagrange/lagrangeprism.hh>
+#include <dune/localfunctions/lagrange/lagrangesimplex.hh>
 
 #warning This header is deprecated
 
 namespace Dune
 {
 
-  /** \brief First-order Lagrangian finite element on a prism
+  /** \brief Second-order Lagrange local finite element on the reference tetrahedron
    *
-   * \deprecated Please use LagrangePrismLocalFiniteElement<D,R,2> instead!
+   * \tparam D Number type used for domain coordinates
+   * \tparam R Number type used for shape function values
+   *
+   * \deprecated This class is obsolete. Please use LagrangeSimplexLocalFiniteElement instead!
    */
   template<class D, class R>
-  using PrismP1LocalFiniteElement
-    [[deprecated("use LagrangePrismLocalFiniteElement instead")]]
-    = LagrangePrismLocalFiniteElement<D,R,1>;
+  using P23DLocalFiniteElement
+    [[deprecated("use LagrangeSimplexLocalFiniteElement instead")]]
+    = LagrangeSimplexLocalFiniteElement<D,R,3,2>;
 
 }
 
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/prismp2.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/pyramidp2.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_PRISM2_3DLOCALFINITEELEMENT_HH
-#define DUNE_PRISM2_3DLOCALFINITEELEMENT_HH
+#ifndef DUNE_PYRAMIDP2_3DLOCALFINITEELEMENT_HH
+#define DUNE_PYRAMIDP2_3DLOCALFINITEELEMENT_HH
 
-#include <dune/localfunctions/lagrange/lagrangeprism.hh>
+#include <dune/localfunctions/lagrange/lagrangepyramid.hh>
 
 #warning This header is deprecated
 
 namespace Dune
 {
 
-  /** \brief Second-order Lagrange finite element on a three-dimensional prism
+  /** \brief Second-order Lagrangian finite element on a three-dimensional pyramid
    *
-   * \deprecated Please use LagrangePrismLocalFiniteElement<D,R,2> instead!
+   * \deprecated Please use LagrangePyramidLocalFiniteElement<D,R,2> instead!
    */
   template<class D, class R>
-  using PrismP2LocalFiniteElement
-    [[deprecated("use LagrangePrismLocalFiniteElement instead")]]
-    = LagrangePrismLocalFiniteElement<D,R,2>;
+  using PyramidP2LocalFiniteElement
+    [[deprecated("use LagrangePyramidLocalFiniteElement instead")]]
+    = LagrangePyramidLocalFiniteElement<D,R,2>;
 
 }
 
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/pyramidp1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/p2.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
+#ifndef DUNE_P2_LOCALFINITEELEMENT_HH
+#define DUNE_P2_LOCALFINITEELEMENT_HH
 
-#ifndef DUNE_PYRAMID_P1_LOCALFINITEELEMENT_HH
-#define DUNE_PYRAMID_P1_LOCALFINITEELEMENT_HH
-
-#include <dune/localfunctions/lagrange/lagrangepyramid.hh>
+#include <dune/localfunctions/lagrange/lagrangesimplex.hh>
 
 #warning This header is deprecated
 
 namespace Dune
 {
 
-  /** \brief First-order Lagrangian finite element on a three-dimensional pyramid
-   *
-   * \deprecated Please use LagrangePyramidLocalFiniteElement<D,R,1> instead!
+  /** \brief Second-order Lagrange finite element on the reference simplex with compile-time dimension
+
+      \deprecated This class is obsolete. Please use LagrangeSimplexLocalFiniteElement instead!
    */
-  template<class D, class R>
-  using PyramidP1LocalFiniteElement
-    [[deprecated("use LagrangePyramidLocalFiniteElement instead")]]
-    = LagrangePyramidLocalFiniteElement<D,R,1>;
+  template<class D, class R, int d>
+  using P2LocalFiniteElement
+    [[deprecated("use LagrangeSimplexLocalFiniteElement instead")]]
+    = LagrangeSimplexLocalFiniteElement<D,R,d,2>;
 
 }
 
 #endif
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/q1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/q1.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_Q1_LOCALFINITEELEMENT_HH
 #define DUNE_Q1_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange/q2.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange/q2.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_Q2_LOCALFINITEELEMENT_HH
 #define DUNE_Q2_LOCALFINITEELEMENT_HH
 
 #include <dune/common/typetraits.hh>
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/lagrange.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/lagrange.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_LAGRANGE_HH
 #define DUNE_LOCALFUNCTIONS_LAGRANGE_HH
 
 /** \file
  * \brief Convenience header that includes all implementations of Lagrange finite elements
  */
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/basis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/basis.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_META_POWER_BASIS_HH
 #define DUNE_LOCALFUNCTIONS_META_POWER_BASIS_HH
 
 #include <numeric>
 #include <cstddef>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/coefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/coefficients.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_META_POWER_COEFFICIENTS_HH
 #define DUNE_LOCALFUNCTIONS_META_POWER_COEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power/interpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power/interpolation.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_META_POWER_INTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_META_POWER_INTERPOLATION_HH
 
 #include <algorithm>
 #include <cassert>
 #include <cstddef>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/meta/power.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/meta/power.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_META_POWER_HH
 #define DUNE_LOCALFUNCTIONS_META_POWER_HH
 
 #include <cstddef>
 #include <memory>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/mimetic/mimeticall.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/mimetic/mimeticall.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MIMETIC_ALL_HH
 #define DUNE_MIMETIC_ALL_HH
 
 #include <cstddef>
 
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/mimetic.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/mimetic.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MIMETICLOCALFINITEELEMENT_HH
 #define DUNE_MIMETICLOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "common/localfiniteelementtraits.hh"
 #include "mimetic/mimeticall.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/monomiallocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/monomiallocalbasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_MONOMIAL_MONOMIALLOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_MONOMIAL_MONOMIALLOCALBASIS_HH
 
 #include <array>
 #include <cassert>
 #include <numeric>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/monomiallocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/monomiallocalcoefficients.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_MONOMIAL_MONOMIALLOCALCOEFFICIENTS_HH
 #define DUNE_LOCALFUNCTIONS_MONOMIAL_MONOMIALLOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../common/localkey.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial/monomiallocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial/monomiallocalinterpolation.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_MONOMIAL_MONOMIALLOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_MONOMIAL_MONOMIALLOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/monomial.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/monomial.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_MONOMIAL_HH
 #define DUNE_LOCALFUNCTIONS_MONOMIAL_HH
 
 #include <cassert>
 #include <cstddef>
 #include <cstdlib>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelec1stkindcube.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelec1stkindcube.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_NEDELEC_NEDELEC1STKINDCUBE_HH
 #define DUNE_LOCALFUNCTIONS_NEDELEC_NEDELEC1STKINDCUBE_HH
 
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelec1stkindsimplex.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelec1stkindsimplex.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_NEDELEC_NEDELEC1STKINDSIMPLEX_HH
 #define DUNE_LOCALFUNCTIONS_NEDELEC_NEDELEC1STKINDSIMPLEX_HH
 
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexbasis.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_NEDELEC_NEDELECSIMPLEX_NEDELECSIMPLEXBASIS_HH
 
 #define DUNE_LOCALFUNCTIONS_NEDELEC_NEDELECSIMPLEX_NEDELECSIMPLEXBASIS_HH
 
 #include <fstream>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexinterpolation.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_NEDELEC_NEDELECSIMPLEX_NEDELECSIMPLEXINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_NEDELEC_NEDELECSIMPLEX_NEDELECSIMPLEXINTERPOLATION_HH
 
 #include <fstream>
 #include <utility>
 #include <numeric>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexprebasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexprebasis.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_NEDELEC_NEDELECSIMPLEX_NEDELECSIMPLEXPREBASIS_HH
 #define DUNE_LOCALFUNCTIONS_NEDELEC_NEDELECSIMPLEX_NEDELECSIMPLEXPREBASIS_HH
 
 #include <fstream>
 #include <utility>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal/orthonormalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal/orthonormalbasis.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ORTHONORMALBASIS_HH
 #define DUNE_ORTHONORMALBASIS_HH
 
 #include <sstream>
 
 #include <dune/localfunctions/utility/polynomialbasis.hh>
 #include <dune/localfunctions/orthonormal/orthonormalcompute.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal/orthonormalcompute.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal/orthonormalcompute.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ORTHONORMALCOMPUTE_HH
 #define DUNE_ORTHONORMALCOMPUTE_HH
 
 #include <cassert>
 #include <iostream>
 #include <fstream>
 #include <iomanip>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/orthonormal.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/orthonormal.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ORTHONORMALFINITEELEMENT_HH
 #define DUNE_ORTHONORMALFINITEELEMENT_HH
 
 #include <dune/localfunctions/utility/localfiniteelement.hh>
 #include <dune/localfunctions/utility/dglocalcoefficients.hh>
 #include <dune/localfunctions/utility/l2interpolation.hh>
 #include <dune/localfunctions/orthonormal/orthonormalbasis.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RANNACHER_TUREK_LOCALFINITEELEMENT_HH
 #define DUNE_RANNACHER_TUREK_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek2d/rannacherturek2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek2d/rannacherturek2dlocalbasis.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RANNACHER_TUREK_2D_LOCALBASIS_HH
 #define DUNE_RANNACHER_TUREK_2D_LOCALBASIS_HH
 
 #include <numeric>
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannacherturek3d/rannacherturek3dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannacherturek3d/rannacherturek3dlocalbasis.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RANNACHER_TUREK_3D_LOCALBASIS_HH
 #define DUNE_RANNACHER_TUREK_3D_LOCALBASIS_HH
 
 #include <numeric>
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannachertureklocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannachertureklocalbasis.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RANNACHER_TUREK_LOCALBASIS_HH
 #define DUNE_RANNACHER_TUREK_LOCALBASIS_HH
 
 #include "rannacherturek2d/rannacherturek2dlocalbasis.hh"
 #include "rannacherturek3d/rannacherturek3dlocalbasis.hh"
 
 namespace Dune
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannachertureklocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannachertureklocalcoefficients.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RANNACHER_TUREK_LOCALCOEFFICIENTS_HH
 #define DUNE_RANNACHER_TUREK_LOCALCOEFFICIENTS_HH
 
 #include <algorithm>
 #include <array>
 #include <cassert>
 #include <cstddef>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/rannacherturek/rannachertureklocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/rannacherturek/rannachertureklocalinterpolation.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RANNACHER_TUREK_LOCALINTERPOLATION_HH
 #define DUNE_RANNACHER_TUREK_LOCALINTERPOLATION_HH
 
 #include <cassert>
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalbasis.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RT0TRIANGLELOCALBASIS_HH
 #define DUNE_RT0TRIANGLELOCALBASIS_HH
 
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalcoefficients.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RT0TRIANGLELOCALCOEFFICIENTS_HH
 #define DUNE_RT0TRIANGLELOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <iostream>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d/raviartthomas02dlocalinterpolation.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RT02DLOCALINTERPOLATION_HH
 #define DUNE_RT02DLOCALINTERPOLATION_HH
 
 #include <cmath>
 #include <array>
 #include <bitset>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas02d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas02d.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RAVIARTTHOMAS02DLOCALFINITEELEMENT_HH
 #define DUNE_RAVIARTTHOMAS02DLOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include "raviartthomas02d/raviartthomas02dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalbasis.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_RAVIARTTHOMAS03DLOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_RAVIARTTHOMAS03DLOCALBASIS_HH
 
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalcoefficients.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_RAVIARTTHOMAS03DLOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_RAVIARTTHOMAS03DLOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
-#include <iostream>
 #include <vector>
 
-#include <dune/localfunctions/common/localkey.hh>
+#include "../../common/localkey.hh"
 
 namespace Dune
 {
 
-  /**@ingroup LocalLayoutImplementation
-         \brief Layout map for RT0 elements
-
-         \nosubgrouping
-     \implements Dune::LocalCoefficientsVirtualImp
+  /**
+   * \ingroup LocalLayoutImplementation
+   * \brief Layout map for Raviart-Thomas-1 elements on quadrilaterals.
+   *
+   * \nosubgrouping
+   * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class RT03DLocalCoefficients
+  class RT1Cube3DLocalCoefficients
   {
+
   public:
     //! \brief Standard constructor
-    RT03DLocalCoefficients () : li(4)
+    RT1Cube3DLocalCoefficients () : li(36)
     {
-      for (std::size_t i=0; i<4; i++)
+      for (std::size_t i = 0; i < 6; i++)
+      {
         li[i] = LocalKey(i,1,0);
+        li[i + 6]  = LocalKey(i,1,1);
+        li[i + 12] = LocalKey(i,1,2);
+        li[i + 18] = LocalKey(i,1,3);
+      }
+
+      for (std::size_t i = 0; i < 12; i++)
+      {
+        li[i + 24] = LocalKey(0,0,i);
+      }
     }
 
-    //! number of coefficients
+    //! \brief number of coefficients
     std::size_t size () const
     {
-      return 4;
+      return 36;
     }
 
-    //! get i'th index
+    //! \brief get i'th index
     const LocalKey& localKey (std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
-
 }
-
-#endif
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalinterpolation.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_RAVIARTTHOMAS03DLOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_RAVIARTTHOMAS03DLOCALINTERPOLATION_HH
 
 #include <cmath>
 #include <array>
 #include <bitset>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas03d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas03d.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMAS03D_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include "raviartthomas03d/raviartthomas03dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube2d/raviartthomas0cube2dall.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube2d/raviartthomas0cube2dall.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE2D_ALL_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE2D_ALL_HH
 
 #include <cstddef>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube2d.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE2D_LOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include "raviartthomas0cube2d/raviartthomas0cube2dall.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube3d/raviartthomas0cube3dall.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube3d/raviartthomas0cube3dall.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE3D_ALL_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE3D_ALL_HH
 
 #include <cstddef>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0cube3d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas0cube3d.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE3D_LOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_CUBE3D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include "raviartthomas0cube3d/raviartthomas0cube3dall.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalinterpolation.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,114 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALBASIS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALBASIS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALINTERPOLATION_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALINTERPOLATION_HH
 
-#include <numeric>
 #include <vector>
 
-#include <dune/common/fmatrix.hh>
+#include <dune/geometry/quadraturerules.hh>
+#include <dune/localfunctions/common/localinterpolation.hh>
 
-#include "../../common/localbasis.hh"
 
 namespace Dune
 {
+
   /**
-   * \ingroup LocalBasisImplementation
-   * \brief First order Raviart-Thomas shape functions on the reference prism.
+   * \ingroup LocalInterpolationImplementation
+   * \brief First order Raviart-Thomas shape functions on the reference quadrilateral.
    *
-   * \tparam D Type to represent the field in the domain.
-   * \tparam R Type to represent the field in the range.
+   * \tparam LB corresponding LocalBasis giving traits
    *
    * \nosubgrouping
    */
-  template<class D, class R>
-  class RT0PrismLocalBasis
+  template<class LB>
+  class RT1Cube2DLocalInterpolation
   {
 
   public:
-    typedef LocalBasisTraits<D,3,Dune::FieldVector<D,3>,R,3,Dune::FieldVector<R,3>,
-        Dune::FieldMatrix<R,3,3> > Traits;
-
     /**
-     * \brief Make set number s, where 0 <= s < 32
+     * \brief Make set number s, where 0 <= s < 16
      *
      * \param s Edge orientation indicator
      */
-    RT0PrismLocalBasis (std::bitset<5> s = 0)
+    RT1Cube2DLocalInterpolation (std::bitset<4> s = 0)
     {
-      for (size_t i=0; i<size(); i++)
-        sign[i] = s[i] ? -1.0 : 1.0;
-    }
+      for (size_t i=0; i<4; i++)
+        sign_[i] = (s[i]) ? -1.0 : 1.0;
 
-    //! \brief number of shape functions
-    unsigned int size () const
-    {
-      return 5;
+      n_[0] = {-1.0,  0.0};
+      n_[1] = { 1.0,  0.0};
+      n_[2] = { 0.0, -1.0};
+      n_[3] = { 0.0,  1.0};
     }
 
     /**
-     * \brief Evaluate all shape functions
+     * \brief Interpolate a given function with shape functions
      *
-     * \param in Position
-     * \param out return value
+     * \tparam F Function type for function which should be interpolated
+     * \tparam C Coefficient type
+     * \param ff function which should be interpolated
+     * \param out return value, vector of coefficients
      */
-    inline void evaluateFunction (const typename Traits::DomainType& in,
-                                  std::vector<typename Traits::RangeType>& out) const
+    template<class F, class C>
+    void interpolate (const F& ff, std::vector<C>& out) const
     {
-      out.resize(5);
-
-      out[0] = {        in[0], -1.0 + in[1],              0.0};
-
-      out[1] = { -1.0 + in[0],        in[1],              0.0};
-
-      out[2] = {        in[0],        in[1],              0.0};
-
-      out[3] = {          0.0,          0.0, -2.0 + 2.0*in[2]};
-
-      out[4] = {          0.0,          0.0,        2.0*in[2]};
-
-      for (std::size_t i=0; i<out.size(); i++)
-        out[i] *= sign[i];
-
-    }
-
-    /**
-     * \brief Evaluate Jacobian of all shape functions
-     *
-     * \param in Position
-     * \param out return value
-     */
-    inline void evaluateJacobian (const typename Traits::DomainType& in,
-                                  std::vector<typename Traits::JacobianType>& out) const
-    {
-      out.resize(5);
-
-      for(int i=0; i<size(); i++)
-        for(int j=0; j<3; j++)
-            out[i][j] = {0.0, 0.0, 0.0};
-
-      out[0][0][0] = sign[0];
-      out[0][1][1] = sign[0];
-
-      out[1][0][0] = sign[1];
-      out[1][1][1] = sign[1];
-
-      out[2][0][0] = sign[2];
-      out[2][1][1] = sign[2];
-
-      out[3][2][2] = sign[3]*(2.0);
+      // f gives v*outer normal at a point on the edge!
+      typedef typename LB::Traits::RangeFieldType Scalar;
+      typedef typename LB::Traits::DomainFieldType Vector;
+
+      auto&& f = Impl::makeFunctionWithCallOperator<typename LB::Traits::DomainType>(ff);
+
+      out.resize(12);
+      fill(out.begin(), out.end(), 0.0);
+
+      const int qOrder = 3;
+      const auto& rule1 = QuadratureRules<Scalar,1>::rule(GeometryTypes::cube(1), qOrder);
+
+      for (auto&& qp : rule1)
+      {
+        Scalar qPos = qp.position();
+        typename LB::Traits::DomainType localPos = {0.0, qPos};
+
+        auto y = f(localPos);
+        out[0] += (y[0]*n_[0][0] + y[1]*n_[0][1])*qp.weight()*sign_[0];
+        out[1] += (y[0]*n_[0][0] + y[1]*n_[0][1])*(2.0*qPos - 1.0)*qp.weight();
+
+        localPos = {1.0, qPos};
+        y = f(localPos);
+        out[2] += (y[0]*n_[1][0] + y[1]*n_[1][1])*qp.weight()*sign_[1];
+        out[3] += (y[0]*n_[1][0] + y[1]*n_[1][1])*(1.0 - 2.0*qPos)*qp.weight();
+
+        localPos = {qPos, 0.0};
+        y = f(localPos);
+        out[4] += (y[0]*n_[2][0] + y[1]*n_[2][1])*qp.weight()*sign_[2];
+        out[5] += (y[0]*n_[2][0] + y[1]*n_[2][1])*(1.0 - 2.0*qPos)*qp.weight();
+
+        localPos = {qPos, 1.0};
+        y = f(localPos);
+        out[6] += (y[0]*n_[3][0] + y[1]*n_[3][1])*qp.weight()*sign_[3];
+        out[7] += (y[0]*n_[3][0] + y[1]*n_[3][1])*(2.0*qPos - 1.0)*qp.weight();
+      }
 
-      out[4][2][2] = sign[4]*(2.0);
-    }
+      const auto& rule2 = QuadratureRules<Vector,2>::rule(GeometryTypes::cube(2), qOrder);
 
-    //! \brief Evaluate partial derivatives of all shape functions
-    void partial (const std::array<unsigned int, 3>& order,
-                  const typename Traits::DomainType& in,         // position
-                  std::vector<typename Traits::RangeType>& out) const      // return value
-    {
-      auto totalOrder = std::accumulate(order.begin(), order.end(), 0);
-      if (totalOrder == 0) {
-        evaluateFunction(in, out);
-      } else {
-        DUNE_THROW(NotImplemented, "Desired derivative order is not implemented");
+      for (auto&& qp : rule2)
+      {
+        auto qPos = qp.position();
+
+        auto y = f(qPos);
+        out[8] += y[0]*qp.weight();
+        out[9] += y[1]*qp.weight();
+        out[10] += y[0]*qPos[1]*qp.weight();
+        out[11] += y[1]*qPos[0]*qp.weight();
       }
     }
 
-    //! \brief Polynomial order of the shape functions
-    unsigned int order () const
-    {
-      return 1;
-    }
-
   private:
-    std::array<R,5> sign;
+    // Edge orientations
+    std::array<typename LB::Traits::RangeFieldType, 4> sign_;
+
+    // Edge normals
+    std::array<typename LB::Traits::DomainType, 4>     n_;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALBASIS_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALINTERPOLATION_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalcoefficients.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
 
   /**
    * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Raviart-Thomas-1 elements on prisms.
+   * \brief Layout map for Brezzi-Douglas-Marini-1 elements on hexahedra
    *
    * \nosubgrouping
    * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class RT0PrismLocalCoefficients
+  class BDM1Cube3DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    RT0PrismLocalCoefficients () : li(size())
+    BDM1Cube3DLocalCoefficients() : li(18)
     {
-      for(int i=0; i< size(); i++)
+      for (std::size_t i = 0; i < 6; ++i)
+      {
         li[i] = LocalKey(i,1,0);
+        li[i + 6] = LocalKey(i,1,1);
+        li[i + 12] = LocalKey(i,1,2);
+      }
     }
 
     //! \brief number of coefficients
-    std::size_t size () const
+    std::size_t size() const
     {
-      return 5;
+      return 18;
     }
 
     //! \brief get i'th index
-    const LocalKey& localKey (std::size_t i) const
+    const LocalKey& localKey(std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
-}
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALCOEFFICIENTS_HH
+} // end namespace Dune
+#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_CUBE3D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/interpolation.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALINTERPOLATION_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALINTERPOLATION_HH
 
+#ifndef DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_INTERPOLATION_HH
+#define DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_INTERPOLATION_HH
+
+#include <cstddef>
 #include <vector>
 
+#include <dune/localfunctions/whitney/edges0.5/common.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
 
-namespace Dune
-{
+namespace Dune {
+
+  //////////////////////////////////////////////////////////////////////
+  //
+  // Interpolation
+  //
+
+  //! Interpolation for lowest order edge elements on simplices
   /**
-   * \ingroup LocalInterpolationImplementation
-   * \brief First order Raviart-Thomas shape functions on the reference prism.
-   *
-   * \tparam LB corresponding LocalBasis giving traits
+   * \tparam Geometry Type of the local-to-global map.
+   * \tparam RF       Type to represent the field in the range.
    *
    * \nosubgrouping
    */
-  template<class LB>
-  class RT0PrismLocalInterpolation
+  template<class Geometry, class Traits_>
+  class EdgeS0_5Interpolation :
+    private EdgeS0_5Common<Traits_::dimDomainLocal,
+        typename Traits_::DomainField>
   {
-
   public:
+    typedef Traits_ Traits;
 
+  private:
+    static const std::size_t dim = Traits::dimDomainLocal;
+    typedef EdgeS0_5Common<dim, typename Traits::DomainField> Base;
+    using Base::refelem;
+    using Base::s;
+
+    std::vector<typename Traits::DomainGlobal> edgev;
+
+  public:
+    //! constructor
     /**
-     * \brief Make set number s, where 0 <= s < 32
-     *
-     * \param s Face orientation indicator
+     * \param geo         Geometry of the element to contruct a local basis
+     *                    for.
+     * \param vertexOrder Vertex ordering information.  Only the vertex order
+     *                    on the dim=1 sub-entities (edges) is required.
      */
-    RT0PrismLocalInterpolation (std::bitset<5> s = 0)
+    template<typename VertexOrder>
+    EdgeS0_5Interpolation(const Geometry& geo,
+                          const VertexOrder& vertexOrder) :
+      edgev(s)
     {
-      typedef typename LB::Traits::RangeFieldType Scalar;
+      for(std::size_t i = 0; i < s; ++i) {
+        const std::size_t i0 = refelem.subEntity(i,dim-1,0,dim);
+        const std::size_t i1 = refelem.subEntity(i,dim-1,1,dim);
+
+        edgev[i] = geo.corner(i1);
+        edgev[i] -= geo.corner(i0);
+        edgev[i] /= edgev[i].two_norm();
+
+        const typename VertexOrder::iterator& edgeVertexOrder =
+          vertexOrder.begin(dim-1, i);
+        if(edgeVertexOrder[0] > edgeVertexOrder[1])
+          edgev[i] *= -1;
+      }
+    }
 
-      for (size_t i=0; i<5; i++)
-        sign[i] = (s[i]) ? -1.0 : 1.0;
+    //! Interpolation of a function
+    template<typename F, typename C>
+    void interpolate(const F& ff, std::vector<C>& out) const {
+      typename Traits::Range y;
 
-      Scalar r = 1/std::sqrt(2);
+      auto&& f = Impl::makeFunctionWithCallOperator<std::decay_t<decltype(refelem.position(0,dim-1))>>(ff);
 
-      n[0] = { 0.0, -1.0,  0.0};
-      n[1] = {-1.0,  0.0,  0.0};
-      n[2] = {   r,    r,  0.0};
-      n[3] = { 0.0,  0.0, -1.0};
-      n[4] = { 0.0,  0.0,  1.0};
-
-      c[0] = 1.0;
-      c[1] = 1.0;
-      c[2] = std::sqrt(2);
-      c[3] = 1/2.0;
-      c[4] = 1/2.0;
-
-      m[0] = {   0.5,   0.0, 0.5};
-      m[1] = {   0.0,   0.5, 0.5};
-      m[2] = {   0.5,   0.5, 0.5};
-      m[3] = { 1/3.0, 1/3.0, 0.0};
-      m[4] = { 1/3.0, 1/3.0, 1.0};
-    }
+      out.resize(s);
 
-    /**
-     * \brief Interpolate a given function with shape functions
-     *
-     * \tparam F Function type for function which should be interpolated
-     * \tparam C Coefficient type
-     * \param ff function which should be interpolated
-     * \param out return value, vector of coefficients
-     */
-    template<class F, class C>
-    void interpolate (const F& ff, std::vector<C>& out) const
-    {
-      auto&& f = Impl::makeFunctionWithCallOperator<typename LB::Traits::DomainType>(ff);
+      for(std::size_t i = 0; i < s; ++i) {
+        y = f(refelem.position(i,dim-1));
 
-      out.resize(5);
-      for(int i=0; i<5; i++)
-        out[i] = f(m[i]).dot(n[i]) * c[i] * sign[i];
+        out[i] = y * edgev[i];
+      }
     }
-
-  private:
-    // Facet orientations
-    std::array<typename LB::Traits::RangeFieldType, 5> sign;
-    // Facet area
-    std::array<typename LB::Traits::RangeFieldType, 5> c;
-
-    // Facet normals
-    std::array<typename LB::Traits::DomainType, 5> n;
-    // Facet midpoints
-    std::array<typename LB::Traits::DomainType, 5> m;
   };
-}
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_LOCALINTERPOLATION_HH
+
+} // namespace Dune
+
+#endif // DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_INTERPOLATION_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0prism.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1cube3d.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_HH
+#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE3D_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE3D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
-#include "raviartthomas0prism/raviartthomas0prismlocalbasis.hh"
-#include "raviartthomas0prism/raviartthomas0prismlocalcoefficients.hh"
-#include "raviartthomas0prism/raviartthomas0prismlocalinterpolation.hh"
+#include "brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalbasis.hh"
+#include "brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalcoefficients.hh"
+#include "brezzidouglasmarini1cube3d/brezzidouglasmarini1cube3dlocalinterpolation.hh"
 
 namespace Dune
 {
   /**
-   * \brief First order Raviart-Thomas shape functions on prisms.
+   * \brief First order Brezzi-Douglas-Marini shape functions on hexahedron.
    *
-   * \ingroup RaviartThomas
+   * \ingroup BrezziDouglasMarini
    *
    * \tparam D Type to represent the field in the domain.
    * \tparam R Type to represent the field in the range.
    */
   template<class D, class R>
-  class RT0PrismLocalFiniteElement
+  class BDM1Cube3DLocalFiniteElement
   {
 
   public:
     typedef LocalFiniteElementTraits<
-        RT0PrismLocalBasis<D,R>,
-        RT0PrismLocalCoefficients,
-        RT0PrismLocalInterpolation<RT0PrismLocalBasis<D,R> > > Traits;
-
+        BDM1Cube3DLocalBasis<D,R>,
+        BDM1Cube3DLocalCoefficients,
+        BDM1Cube3DLocalInterpolation<BDM1Cube3DLocalBasis<D,R> > > Traits;
 
     //! \brief Standard constructor
-    RT0PrismLocalFiniteElement ()
+    BDM1Cube3DLocalFiniteElement()
     {}
 
     /**
-     * \brief Make set number s, where 0 <= s < 32
+     * \brief Make set number s, where 0 <= s < 64
      *
-     * \param s Face orientation indicator
+     * \param s Edge orientation indicator
      */
-    RT0PrismLocalFiniteElement (int s) :
-      basis(s),
-      interpolation(s)
+    BDM1Cube3DLocalFiniteElement(int s)
+      : basis(s)
+      , interpolation(s)
     {}
 
-    const typename Traits::LocalBasisType& localBasis () const
+    const typename Traits::LocalBasisType& localBasis() const
     {
       return basis;
     }
 
-    const typename Traits::LocalCoefficientsType& localCoefficients () const
+    const typename Traits::LocalCoefficientsType& localCoefficients() const
     {
       return coefficients;
     }
 
-    const typename Traits::LocalInterpolationType& localInterpolation () const
+    const typename Traits::LocalInterpolationType& localInterpolation() const
     {
       return interpolation;
     }
 
     /** \brief Number of shape functions in this finite element */
     unsigned int size () const
     {
       return basis.size();
     }
 
-    static constexpr GeometryType type ()
+    static constexpr GeometryType type()
     {
-      return GeometryTypes::prism;
+      return GeometryTypes::hexahedron;
     }
 
   private:
-    RT0PrismLocalBasis<D,R> basis;
-    RT0PrismLocalCoefficients coefficients;
-    RT0PrismLocalInterpolation<RT0PrismLocalBasis<D,R> > interpolation;
+    BDM1Cube3DLocalBasis<D,R> basis;
+    BDM1Cube3DLocalCoefficients coefficients;
+    BDM1Cube3DLocalInterpolation<BDM1Cube3DLocalBasis<D,R> > interpolation;
   };
-}
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PRISM_HH
+} // end namespace Dune
+#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_QUBE3D_LOCALFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalinterpolation.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,115 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PYRAMID_LOCALBASIS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PYRAMID_LOCALBASIS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALINTERPOLATION_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALINTERPOLATION_HH
 
-#include <numeric>
 #include <vector>
 
-#include <dune/common/fmatrix.hh>
-
-#include "../../common/localbasis.hh"
+#include <dune/geometry/quadraturerules.hh>
+#include <dune/localfunctions/common/localinterpolation.hh>
 
 namespace Dune
 {
+
   /**
-   * \ingroup LocalBasisImplementation
-   * \brief First order Raviart-Thomas shape functions on the reference pyramid.
+   * @ingroup LocalInterpolationImplementation
+   * \brief First order Raviart-Thomas shape functions on the reference quadrilateral.
    *
-   * \tparam D Type to represent the field in the domain.
-   * \tparam R Type to represent the field in the range.
+   * \tparam LB corresponding LocalBasis giving traits
    *
    * \nosubgrouping
    */
-  template<class D, class R>
-  class RT0PyramidLocalBasis
+  template<class LB>
+  class RT12DLocalInterpolation
   {
 
   public:
-    typedef LocalBasisTraits<D,3,Dune::FieldVector<D,3>,R,3,Dune::FieldVector<R,3>,
-        Dune::FieldMatrix<R,3,3> > Traits;
 
     /**
-     * \brief Make set number s, where 0 <= s < 32
+     * \brief Make set number s, where 0 <= s < 8
      *
      * \param s Edge orientation indicator
      */
-    RT0PyramidLocalBasis (std::bitset<5> s = 0)
-    {
-      for (size_t i=0; i<size(); i++)
-        sign[i] = s[i] ? -1.0 : 1.0;
-    }
-
-    //! \brief number of shape functions
-    unsigned int size () const
+    RT12DLocalInterpolation (std::bitset<3> s = 0)
     {
-      return 5;
+      using std::sqrt;
+      for (size_t i=0; i<3; i++)
+        sign_[i] = (s[i]) ? -1.0 : 1.0;
+
+      n_[0] = { 0.0, -1.0};
+      n_[1] = {-1.0,  0.0};
+      n_[2] = { 1.0/sqrt(2.0), 1.0/sqrt(2.0)};
+
+      c_ = { 0.5*n_[0][0] - 1.0*n_[0][1],
+            -1.0*n_[1][0] + 0.5*n_[1][1],
+             0.5*n_[2][0] + 0.5*n_[2][1]};
     }
 
     /**
-     * \brief Evaluate all shape functions
+     * \brief Interpolate a given function with shape functions
      *
-     * \param in Position
-     * \param out return value
+     * \tparam F Function type for function which should be interpolated
+     * \tparam C Coefficient type
+     * \param ff function which should be interpolated
+     * \param out return value, vector of coefficients
      */
-    inline void evaluateFunction (const typename Traits::DomainType& in,
-                                  std::vector<typename Traits::RangeType>& out) const
+    template<typename F, typename C>
+    void interpolate (const F& ff, std::vector<C>& out) const
     {
-      out.resize(5);
-      for (std::size_t i=0; i<out.size(); i++)
-        out[i] = {0.0,0.0,0.0};
-
-      out[0][0] = 1.5*in[0];
-      out[0][1] = 1.5*in[1];
-      out[0][2] = -1.0;
-
-      out[1][0] = -2.0 + 3.0*in[0];
-
-      out[2][0] = 3.0*in[0];
-
-      out[3][1] = -2.0 + 3.0*in[1];
-
-      out[4][1] = 3.0*in[1];
-
-      for (std::size_t i=0; i<out.size(); i++)
-        out[i] *= sign[i];
-
-    }
-
-    /**
-     * \brief Evaluate Jacobian of all shape functions
-     *
-     * \param in Position
-     * \param out return value
-     */
-    inline void evaluateJacobian (const typename Traits::DomainType& in,
-                                  std::vector<typename Traits::JacobianType>& out) const
-    {
-      out.resize(5);
-
-      for(int i=0; i<size(); i++)
-        for(int j=0; j<3; j++)
-            out[i][j] = {0.0, 0.0, 0.0};
-
-      out[0][0][0] = sign[0]*(1.5);
-      out[0][1][1] = sign[0]*(1.5);
-
-      out[1][0][0] = sign[1]*(3.0);
-
-      out[2][0][0] = sign[2]*(3.0);
+      // f gives v*outer normal at a point on the edge!
+      typedef typename LB::Traits::RangeFieldType Scalar;
+      typedef typename LB::Traits::DomainFieldType Vector;
+
+      auto&& f = Impl::makeFunctionWithCallOperator<typename LB::Traits::DomainType>(ff);
+
+      out.resize(8);
+      fill(out.begin(), out.end(), 0.0);
+
+      const int qOrder1 = 4;
+      const auto& rule1 = Dune::QuadratureRules<Scalar,1>::rule(Dune::GeometryTypes::simplex(1), qOrder1);
+
+      for (auto&& qp : rule1)
+      {
+        Scalar qPos = qp.position();
+        typename LB::Traits::DomainType localPos;
+
+        localPos = {qPos, 0.0};
+        auto y = f(localPos);
+        out[0] += (y[0]*n_[0][0] + y[1]*n_[0][1])*qp.weight()*sign_[0]/c_[0];
+        out[3] += (y[0]*n_[0][0] + y[1]*n_[0][1])*(2.0*qPos - 1.0)*qp.weight()/c_[0];
+
+        localPos = {0.0, qPos};
+        y = f(localPos);
+        out[1] += (y[0]*n_[1][0] + y[1]*n_[1][1])*qp.weight()*sign_[1]/c_[1];
+        out[4] += (y[0]*n_[1][0] + y[1]*n_[1][1])*(1.0 - 2.0*qPos)*qp.weight()/c_[1];
+
+        localPos = {1.0 - qPos, qPos};
+        y = f(localPos);
+        out[2] += (y[0]*n_[2][0] + y[1]*n_[2][1])*qp.weight()*sign_[2]/c_[2];
+        out[5] += (y[0]*n_[2][0] + y[1]*n_[2][1])*(2.0*qPos - 1.0)*qp.weight()/c_[2];
+      }
 
-      out[3][1][1] = sign[3]*(3.0);
+      const int qOrder2 = 8;
+      const auto& rule2 = Dune::QuadratureRules<Vector,2>::rule(Dune::GeometryTypes::simplex(2), qOrder2);
 
-      out[4][1][1] = sign[4]*(3.0);
-    }
-
-    //! \brief Evaluate partial derivatives of all shape functions
-    void partial (const std::array<unsigned int, 3>& order,
-                  const typename Traits::DomainType& in,         // position
-                  std::vector<typename Traits::RangeType>& out) const      // return value
-    {
-      auto totalOrder = std::accumulate(order.begin(), order.end(), 0);
-      if (totalOrder == 0) {
-        evaluateFunction(in, out);
-      } else {
-        DUNE_THROW(NotImplemented, "Desired derivative order is not implemented");
+      for (auto&& qp : rule2)
+      {
+        auto qPos = qp.position();
+
+        auto y = f(qPos);
+        out[6] += y[0]*qp.weight();
+        out[7] += y[1]*qp.weight();
       }
     }
 
-    //! \brief Polynomial order of the shape functions
-    unsigned int order () const
-    {
-      return 1;
-    }
-
   private:
-    std::array<R,5> sign;
+    // Edge orientations
+    std::array<typename LB::Traits::RangeFieldType, 3> sign_;
+
+    // Edge normals
+    std::array<typename LB::Traits::DomainType, 3>     n_;
+
+    std::array<typename LB::Traits::RangeFieldType, 3> c_;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PYRAMID_LOCALBASIS_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALINTERPOLATION_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalcoefficients.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PYRAMID_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PYRAMID_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
-
   /**
    * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Raviart-Thomas-1 elements on pyramids.
+   * \brief Layout map for Raviart-Thomas-3 elements on quadrilaterals
    *
    * \nosubgrouping
    * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class RT0PyramidLocalCoefficients
+  class RT3Cube2DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    RT0PyramidLocalCoefficients () : li(size())
+    RT3Cube2DLocalCoefficients () : li(40)
     {
-      for(int i=0; i< size(); i++)
-        li[i] = LocalKey(i,1,0);
+      for (std::size_t i = 0; i < 4; i++)
+      {
+        li[4*i] = LocalKey(i,1,0);
+        li[4*i + 1] = LocalKey(i,1,1);
+        li[4*i + 2] = LocalKey(i,1,2);
+        li[4*i + 3] = LocalKey(i,1,3);
+      }
+
+      for (std::size_t i=0; i<24; i++)
+      {
+        li[16 + i] = LocalKey(0,0,i);
+      }
     }
 
     //! \brief number of coefficients
     std::size_t size () const
     {
-      return 5;
+      return 40;
     }
 
     //! \brief get i'th index
     const LocalKey& localKey (std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS0_PYRAMID_LOCALCOEFFICIENTS_HH
+
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalbasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALBASIS_HH
 
 #include <numeric>
 #include <vector>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalcoefficients.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
-
   /**
-   * @ingroup LocalLayoutImplementation
-   * \brief Layout map for Raviart-Thomas-1 elements on the reference triangle.
+   * \ingroup LocalLayoutImplementation
+   * \brief Layout map for Raviart-Thomas-2 elements on quadrilaterals
    *
    * \nosubgrouping
+   * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class RT12DLocalCoefficients
+  class RT2Cube2DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    RT12DLocalCoefficients () : li(8)
+    RT2Cube2DLocalCoefficients () : li(24)
     {
-      for (std::size_t i = 0; i < 3; i++)
+      for (std::size_t i = 0; i < 4; i++)
       {
-        li[i] = LocalKey(i,1,0);
-        li[3 + i] = LocalKey(i,1,1);
+        li[3*i] = LocalKey(i,1,0);
+        li[3*i + 1] = LocalKey(i,1,1);
+        li[3*i + 2] = LocalKey(i,1,2);
       }
 
-      // last two DOF are associated with the cell (codim = 0)
-      li[6] = LocalKey(0,0,0);
-      li[7] = LocalKey(0,0,1);
+      for (std::size_t i=0; i<12; i++)
+      {
+        li[12 + i] = LocalKey(0,0,i);
+      }
     }
 
     //! \brief number of coefficients
     std::size_t size () const
     {
-      return 8;
+      return 24;
     }
 
     //! \brief get i'th index
     const LocalKey& localKey (std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALCOEFFICIENTS_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalinterpolation.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALINTERPOLATION_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALINTERPOLATION_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALINTERPOLATION_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
 
 namespace Dune
 {
 
   /**
-   * @ingroup LocalInterpolationImplementation
-   * \brief First order Raviart-Thomas shape functions on the reference quadrilateral.
+   * \ingroup LocalInterpolationImplementation
+   * \brief Second order Raviart-Thomas shape functions on the reference triangle.
    *
    * \tparam LB corresponding LocalBasis giving traits
    *
    * \nosubgrouping
    */
   template<class LB>
-  class RT12DLocalInterpolation
+  class RT2Cube2DLocalInterpolation
   {
 
   public:
 
     /**
-     * \brief Make set number s, where 0 <= s < 8
+     * \brief Make set number s, where 0 <= s < 16
      *
      * \param s Edge orientation indicator
      */
-    RT12DLocalInterpolation (std::bitset<3> s = 0)
+    RT2Cube2DLocalInterpolation (std::bitset<4> s = 0)
     {
-      using std::sqrt;
-      for (size_t i=0; i<3; i++)
+      for (size_t i=0; i<4; i++)
         sign_[i] = (s[i]) ? -1.0 : 1.0;
 
-      n_[0] = { 0.0, -1.0};
-      n_[1] = {-1.0,  0.0};
-      n_[2] = { 1.0/sqrt(2.0), 1.0/sqrt(2.0)};
-
-      c_ = { 0.5*n_[0][0] - 1.0*n_[0][1],
-            -1.0*n_[1][0] + 0.5*n_[1][1],
-             0.5*n_[2][0] + 0.5*n_[2][1]};
+      n_[0] = {-1.0,  0.0};
+      n_[1] = { 1.0,  0.0};
+      n_[2] = { 0.0, -1.0};
+      n_[3] = { 0.0,  1.0};
     }
 
     /**
      * \brief Interpolate a given function with shape functions
      *
      * \tparam F Function type for function which should be interpolated
      * \tparam C Coefficient type
@@ -60,58 +54,74 @@
     {
       // f gives v*outer normal at a point on the edge!
       typedef typename LB::Traits::RangeFieldType Scalar;
       typedef typename LB::Traits::DomainFieldType Vector;
 
       auto&& f = Impl::makeFunctionWithCallOperator<typename LB::Traits::DomainType>(ff);
 
-      out.resize(8);
+      out.resize(24);
       fill(out.begin(), out.end(), 0.0);
 
-      const int qOrder1 = 4;
-      const auto& rule1 = Dune::QuadratureRules<Scalar,1>::rule(Dune::GeometryTypes::simplex(1), qOrder1);
+      const int qOrder = 6;
+      const auto& rule1 = QuadratureRules<Scalar,1>::rule(GeometryTypes::cube(1), qOrder);
 
       for (auto&& qp : rule1)
       {
         Scalar qPos = qp.position();
         typename LB::Traits::DomainType localPos;
 
-        localPos = {qPos, 0.0};
+        localPos = {0.0, qPos};
         auto y = f(localPos);
-        out[0] += (y[0]*n_[0][0] + y[1]*n_[0][1])*qp.weight()*sign_[0]/c_[0];
-        out[3] += (y[0]*n_[0][0] + y[1]*n_[0][1])*(2.0*qPos - 1.0)*qp.weight()/c_[0];
+        out[0] += (y[0]*n_[0][0] + y[1]*n_[0][1])*qp.weight()*sign_[0];
+        out[1] += (y[0]*n_[0][0] + y[1]*n_[0][1])*(2.0*qPos - 1.0)*qp.weight();
+        out[2] += (y[0]*n_[0][0] + y[1]*n_[0][1])*(6.0*qPos*qPos - 6.0*qPos + 1.0)*qp.weight()*sign_[0];
 
-        localPos = {0.0, qPos};
+        localPos = {1.0, qPos};
         y = f(localPos);
-        out[1] += (y[0]*n_[1][0] + y[1]*n_[1][1])*qp.weight()*sign_[1]/c_[1];
-        out[4] += (y[0]*n_[1][0] + y[1]*n_[1][1])*(1.0 - 2.0*qPos)*qp.weight()/c_[1];
+        out[3] += (y[0]*n_[1][0] + y[1]*n_[1][1])*qp.weight()*sign_[1];
+        out[4] += (y[0]*n_[1][0] + y[1]*n_[1][1])*(1.0 - 2.0*qPos)*qp.weight();
+        out[5] += (y[0]*n_[1][0] + y[1]*n_[1][1])*(6.0*qPos*qPos - 6.0*qPos + 1.0)*qp.weight()*sign_[1];
 
-        localPos = {1.0 - qPos, qPos};
+        localPos = {qPos, 0.0};
         y = f(localPos);
-        out[2] += (y[0]*n_[2][0] + y[1]*n_[2][1])*qp.weight()*sign_[2]/c_[2];
-        out[5] += (y[0]*n_[2][0] + y[1]*n_[2][1])*(2.0*qPos - 1.0)*qp.weight()/c_[2];
+        out[6] += (y[0]*n_[2][0] + y[1]*n_[2][1])*qp.weight()*sign_[2];
+        out[7] += (y[0]*n_[2][0] + y[1]*n_[2][1])*(1.0 - 2.0*qPos)*qp.weight();
+        out[8] += (y[0]*n_[2][0] + y[1]*n_[2][1])*(6.0*qPos*qPos - 6.0*qPos + 1.0)*qp.weight()*sign_[2];
+
+        localPos = {qPos, 1.0};
+        y = f(localPos);
+        out[9]  += (y[0]*n_[3][0] + y[1]*n_[3][1])*qp.weight()*sign_[3];
+        out[10] += (y[0]*n_[3][0] + y[1]*n_[3][1])*(2.0*qPos - 1.0)*qp.weight();
+        out[11] += (y[0]*n_[3][0] + y[1]*n_[3][1])*(6.0*qPos*qPos - 6.0*qPos + 1.0)*qp.weight()*sign_[3];
       }
 
-      const int qOrder2 = 8;
-      const auto& rule2 = Dune::QuadratureRules<Vector,2>::rule(Dune::GeometryTypes::simplex(2), qOrder2);
+      const auto& rule2 = QuadratureRules<Vector,2>::rule(GeometryTypes::cube(2), qOrder);
 
       for (auto&& qp : rule2)
       {
-        auto qPos = qp.position();
+        FieldVector<double,2> qPos = qp.position();
 
         auto y = f(qPos);
-        out[6] += y[0]*qp.weight();
-        out[7] += y[1]*qp.weight();
+        out[12] += y[0]*qp.weight();
+        out[13] += y[1]*qp.weight();
+        out[14] += y[0]*qPos[0]*qp.weight();
+        out[15] += y[1]*qPos[0]*qp.weight();
+        out[16] += y[0]*qPos[1]*qp.weight();
+        out[17] += y[1]*qPos[1]*qp.weight();
+        out[18] += y[0]*qPos[0]*qPos[1]*qp.weight();
+        out[19] += y[1]*qPos[0]*qPos[1]*qp.weight();
+        out[20] += y[0]*qPos[1]*qPos[1]*qp.weight();
+        out[21] += y[1]*qPos[0]*qPos[0]*qp.weight();
+        out[22] += y[0]*qPos[0]*qPos[1]*qPos[1]*qp.weight();
+        out[23] += y[1]*qPos[0]*qPos[0]*qPos[1]*qp.weight();
       }
     }
 
   private:
     // Edge orientations
-    std::array<typename LB::Traits::RangeFieldType, 3> sign_;
+    std::array<typename LB::Traits::RangeFieldType, 4> sign_;
 
     // Edge normals
-    std::array<typename LB::Traits::DomainType, 3>     n_;
-
-    std::array<typename LB::Traits::RangeFieldType, 3> c_;
+    std::array<typename LB::Traits::DomainType, 4>     n_;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALINTERPOLATION_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALINTERPOLATION_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas12d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas12d.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS12DLOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
 #include "raviartthomas12d/raviartthomas12dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalbasis.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALBASIS_HH
 
 #include <numeric>
 #include <vector>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalcoefficients.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALCOEFFICIENTS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube2d.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
 #include "raviartthomas1cube2d/raviartthomas1cube2dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALBASIS_HH
 
 #include <numeric>
 #include <vector>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalcoefficients.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALCOEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALCOEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
 #include "../../common/localkey.hh"
 
 namespace Dune
 {
-
   /**
    * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Raviart-Thomas-1 elements on quadrilaterals.
+   * \brief Layout map for Raviart-Thomas-4 elements on quadrilaterals
    *
    * \nosubgrouping
    * \implements Dune::LocalCoefficientsVirtualImp
    */
-  class RT1Cube3DLocalCoefficients
+  class RT4Cube2DLocalCoefficients
   {
 
   public:
     //! \brief Standard constructor
-    RT1Cube3DLocalCoefficients () : li(36)
+    RT4Cube2DLocalCoefficients () : li(60)
     {
-      for (std::size_t i = 0; i < 6; i++)
+      for (std::size_t i = 0; i < 4; i++)
       {
-        li[i] = LocalKey(i,1,0);
-        li[i + 6]  = LocalKey(i,1,1);
-        li[i + 12] = LocalKey(i,1,2);
-        li[i + 18] = LocalKey(i,1,3);
+        li[5*i] = LocalKey(i,1,0);
+        li[5*i + 1] = LocalKey(i,1,1);
+        li[5*i + 2] = LocalKey(i,1,2);
+        li[5*i + 3] = LocalKey(i,1,3);
+        li[5*i + 4] = LocalKey(i,1,4);
       }
 
-      for (std::size_t i = 0; i < 12; i++)
+      for (std::size_t i=0; i<40; i++)
       {
-        li[i + 24] = LocalKey(0,0,i);
+        li[20 + i] = LocalKey(0,0,i);
       }
     }
 
     //! \brief number of coefficients
     std::size_t size () const
     {
-      return 36;
+      return 60;
     }
 
     //! \brief get i'th index
     const LocalKey& localKey (std::size_t i) const
     {
       return li[i];
     }
 
   private:
     std::vector<LocalKey> li;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALCOEFFICIENTS_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas1cube3d/raviartthomas1cube3dlocalinterpolation.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas1cube3d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d.hh`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALFINITEELEMENT_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALFINITEELEMENT_HH
+#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
-#include "raviartthomas1cube3d/raviartthomas1cube3dlocalbasis.hh"
-#include "raviartthomas1cube3d/raviartthomas1cube3dlocalcoefficients.hh"
-#include "raviartthomas1cube3d/raviartthomas1cube3dlocalinterpolation.hh"
+#include "raviartthomas4cube2d/raviartthomas4cube2dlocalbasis.hh"
+#include "raviartthomas4cube2d/raviartthomas4cube2dlocalcoefficients.hh"
+#include "raviartthomas4cube2d/raviartthomas4cube2dlocalinterpolation.hh"
 
 namespace Dune
 {
   /**
-   * \brief First order Raviart-Thomas shape functions on cubes.
+   * \brief Second order Raviart-Thomas shape functions on cubes.
+   *
+   * \note The Jacobian is not implemented.
    *
    * \ingroup RaviartThomas
    *
    * \tparam D Type to represent the field in the domain.
    * \tparam R Type to represent the field in the range.
    */
   template<class D, class R>
-  class RT1Cube3DLocalFiniteElement
+  class RT4Cube2DLocalFiniteElement
   {
 
   public:
     typedef LocalFiniteElementTraits<
-        RT1Cube3DLocalBasis<D,R>,
-        RT1Cube3DLocalCoefficients,
-        RT1Cube3DLocalInterpolation<RT1Cube3DLocalBasis<D,R> > > Traits;
+        RT4Cube2DLocalBasis<D,R>,
+        RT4Cube2DLocalCoefficients,
+        RT4Cube2DLocalInterpolation<RT4Cube2DLocalBasis<D,R> > > Traits;
 
     //! \brief Standard constructor
-    RT1Cube3DLocalFiniteElement ()
+    RT4Cube2DLocalFiniteElement ()
     {}
 
     /**
-     * \brief Make set number s, where 0 <= s < 64
+     * \brief Make set number s, where 0 <= s < 16
      *
      * \param s Edge orientation indicator
      */
-    RT1Cube3DLocalFiniteElement (int s) :
+    RT4Cube2DLocalFiniteElement (int s) :
       basis(s),
       interpolation(s)
     {}
 
     const typename Traits::LocalBasisType& localBasis () const
     {
       return basis;
@@ -65,17 +65,17 @@
     unsigned int size () const
     {
       return basis.size();
     }
 
     static constexpr GeometryType type ()
     {
-      return GeometryTypes::hexahedron;
+      return GeometryTypes::quadrilateral;
     }
 
   private:
-    RT1Cube3DLocalBasis<D,R> basis;
-    RT1Cube3DLocalCoefficients coefficients;
-    RT1Cube3DLocalInterpolation<RT1Cube3DLocalBasis<D,R> > interpolation;
+    RT4Cube2DLocalBasis<D,R> basis;
+    RT4Cube2DLocalCoefficients coefficients;
+    RT4Cube2DLocalInterpolation<RT4Cube2DLocalBasis<D,R> > interpolation;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS1_CUBE3D_LOCALFINITEELEMENT_HH
+#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALBASIS_HH
 
 #include <numeric>
 #include <vector>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d/raviartthomas2cube2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/coefficients.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,49 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALCOEFFICIENTS_HH
+
+#ifndef DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_COEFFICIENTS_HH
+#define DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_COEFFICIENTS_HH
 
 #include <cstddef>
 #include <vector>
 
-#include "../../common/localkey.hh"
+#include <dune/localfunctions/common/localkey.hh>
+#include <dune/localfunctions/whitney/edges0.5/common.hh>
+
+namespace Dune {
 
-namespace Dune
-{
+  //////////////////////////////////////////////////////////////////////
+  //
+  // Coefficients
+  //
+
+  //! Coefficients for lowest order edge elements on simplices
   /**
-   * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Raviart-Thomas-2 elements on quadrilaterals
-   *
    * \nosubgrouping
-   * \implements Dune::LocalCoefficientsVirtualImp
+   * \implements CoefficientsInterface
+   *
+   * \tparam dim Dimension of both domain and range.
    */
-  class RT2Cube2DLocalCoefficients
-  {
+  template<std::size_t dim>
+  class EdgeS0_5Coefficients : private EdgeS0_5Common<dim> {
+    using EdgeS0_5Common<dim>::s;
 
-  public:
-    //! \brief Standard constructor
-    RT2Cube2DLocalCoefficients () : li(24)
-    {
-      for (std::size_t i = 0; i < 4; i++)
-      {
-        li[3*i] = LocalKey(i,1,0);
-        li[3*i + 1] = LocalKey(i,1,1);
-        li[3*i + 2] = LocalKey(i,1,2);
-      }
-
-      for (std::size_t i=0; i<12; i++)
-      {
-        li[12 + i] = LocalKey(0,0,i);
-      }
-    }
+    std::vector<LocalKey> li;
 
-    //! \brief number of coefficients
-    std::size_t size () const
-    {
-      return 24;
+  public:
+    //! Standard constructor
+    EdgeS0_5Coefficients() : li(s) {
+      for(std::size_t i = 0; i < s; i++)
+        li[i] = LocalKey(i, dim-1, 0);
     }
 
-    //! \brief get i'th index
-    const LocalKey& localKey (std::size_t i) const
-    {
-      return li[i];
-    }
+    //! number of coefficients
+    std::size_t size () const { return s; }
 
-  private:
-    std::vector<LocalKey> li;
+    //! get i'th index
+    const LocalKey& localKey(std::size_t i) const { return li[i]; }
   };
-}
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALCOEFFICIENTS_HH
+
+} // namespace Dune
+
+#endif // DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_COEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas2cube2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas2cube2d.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALFINITEELEMENT_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS2_CUBE2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
 #include "raviartthomas2cube2d/raviartthomas2cube2dlocalbasis.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalbasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALBASIS_HH
 
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas3cube2d/raviartthomas3cube2dlocalinterpolation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS3_CUBE2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALBASIS_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALBASIS_HH
 
 #include <bitset>
 #include <numeric>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/dglocalcoefficients.hh`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,76 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALCOEFFICIENTS_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALCOEFFICIENTS_HH
+#ifndef DUNE_DGLOCALCOEFFICIENTS_HH
+#define DUNE_DGLOCALCOEFFICIENTS_HH
 
-#include <cstddef>
+#include <cassert>
 #include <vector>
 
-#include "../../common/localkey.hh"
+#include <dune/localfunctions/common/localkey.hh>
 
 namespace Dune
 {
+
+  // DGLocalCoefficients
+  // -------------------
+
   /**
-   * \ingroup LocalLayoutImplementation
-   * \brief Layout map for Raviart-Thomas-4 elements on quadrilaterals
-   *
-   * \nosubgrouping
-   * \implements Dune::LocalCoefficientsVirtualImp
-   */
-  class RT4Cube2DLocalCoefficients
+   * @brief A class providing local coefficients for dg spaces
+   **/
+  class DGLocalCoefficients
   {
+    typedef DGLocalCoefficients This;
 
   public:
-    //! \brief Standard constructor
-    RT4Cube2DLocalCoefficients () : li(60)
+    //! construct local keys for n basis functions
+    DGLocalCoefficients ( const unsigned int n )
+      : localKey_( n )
     {
-      for (std::size_t i = 0; i < 4; i++)
-      {
-        li[5*i] = LocalKey(i,1,0);
-        li[5*i + 1] = LocalKey(i,1,1);
-        li[5*i + 2] = LocalKey(i,1,2);
-        li[5*i + 3] = LocalKey(i,1,3);
-        li[5*i + 4] = LocalKey(i,1,4);
-      }
-
-      for (std::size_t i=0; i<40; i++)
-      {
-        li[20 + i] = LocalKey(0,0,i);
-      }
+      for( unsigned i = 0; i < n; ++i )
+        localKey_[ i ] = LocalKey( 0, 0, i );
     }
 
-    //! \brief number of coefficients
-    std::size_t size () const
+    const LocalKey &localKey ( const unsigned int i ) const
     {
-      return 60;
+      assert( i < size() );
+      return localKey_[ i ];
     }
 
-    //! \brief get i'th index
-    const LocalKey& localKey (std::size_t i) const
+    unsigned int size () const
     {
-      return li[i];
+      return localKey_.size();
     }
 
   private:
-    std::vector<LocalKey> li;
+    std::vector< LocalKey > localKey_;
   };
+
+
+
+  // DGLocalCoefficientsFactory
+  // --------------------------
+  /**
+   * @brief A factory class for the dg local coefficients.
+   **/
+  template< class BasisFactory >
+  struct DGLocalCoefficientsFactory
+  {
+    static const unsigned int dimension = BasisFactory::dimension;
+    typedef typename BasisFactory::Key Key;
+    typedef const DGLocalCoefficients Object;
+
+    template< GeometryType::Id geometryId >
+    static Object *create ( const Key &key )
+    {
+      const typename BasisFactory::Object *basis
+        = BasisFactory::template create< geometryId >( key );
+      Object *coefficients = new Object( basis->size() );
+      BasisFactory::release( basis );
+      return coefficients;
+    }
+    static void release( Object *object ) { delete object; }
+  };
+
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALCOEFFICIENTS_HH
+
+#endif // #ifndef DUNE_DGLOCALCOEFFICIENTS_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomas4cube2d/raviartthomas4cube2dlocalinterpolation.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALINTERPOLATION_HH
 
 #include <vector>
 
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomas4cube2d.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/brezzidouglasmarini/brezzidouglasmarini1simplex2d.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALFINITEELEMENT_HH
-#define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALFINITEELEMENT_HH
+#ifndef DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALFINITEELEMENT_HH
+#define DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include "../common/localfiniteelementtraits.hh"
-#include "raviartthomas4cube2d/raviartthomas4cube2dlocalbasis.hh"
-#include "raviartthomas4cube2d/raviartthomas4cube2dlocalcoefficients.hh"
-#include "raviartthomas4cube2d/raviartthomas4cube2dlocalinterpolation.hh"
+#include "brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalbasis.hh"
+#include "brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalcoefficients.hh"
+#include "brezzidouglasmarini1simplex2d/brezzidouglasmarini1simplex2dlocalinterpolation.hh"
 
 namespace Dune
 {
+
   /**
-   * \brief Second order Raviart-Thomas shape functions on cubes.
-   *
-   * \note The Jacobian is not implemented.
+   * \brief First order Brezzi-Douglas-Marini shape functions on triangles.
    *
-   * \ingroup RaviartThomas
+   * \ingroup BrezziDouglasMarini
    *
    * \tparam D Type to represent the field in the domain.
    * \tparam R Type to represent the field in the range.
    */
   template<class D, class R>
-  class RT4Cube2DLocalFiniteElement
+  class BDM1Simplex2DLocalFiniteElement
   {
 
   public:
     typedef LocalFiniteElementTraits<
-        RT4Cube2DLocalBasis<D,R>,
-        RT4Cube2DLocalCoefficients,
-        RT4Cube2DLocalInterpolation<RT4Cube2DLocalBasis<D,R> > > Traits;
+        BDM1Simplex2DLocalBasis<D,R>,
+        BDM1Simplex2DLocalCoefficients,
+        BDM1Simplex2DLocalInterpolation<BDM1Simplex2DLocalBasis<D,R> > > Traits;
 
     //! \brief Standard constructor
-    RT4Cube2DLocalFiniteElement ()
+    BDM1Simplex2DLocalFiniteElement ()
     {}
 
     /**
-     * \brief Make set number s, where 0 <= s < 16
+     * \brief Make set number s, where 0 <= s < 8
      *
      * \param s Edge orientation indicator
      */
-    RT4Cube2DLocalFiniteElement (int s) :
+    BDM1Simplex2DLocalFiniteElement (int s) :
       basis(s),
       interpolation(s)
     {}
 
     const typename Traits::LocalBasisType& localBasis () const
     {
       return basis;
@@ -67,17 +64,17 @@
     unsigned int size () const
     {
       return basis.size();
     }
 
     static constexpr GeometryType type ()
     {
-      return GeometryTypes::quadrilateral;
+      return GeometryTypes::triangle;
     }
 
   private:
-    RT4Cube2DLocalBasis<D,R> basis;
-    RT4Cube2DLocalCoefficients coefficients;
-    RT4Cube2DLocalInterpolation<RT4Cube2DLocalBasis<D,R> > interpolation;
+    BDM1Simplex2DLocalBasis<D,R> basis;
+    BDM1Simplex2DLocalCoefficients coefficients;
+    BDM1Simplex2DLocalInterpolation<BDM1Simplex2DLocalBasis<D,R> > interpolation;
   };
 }
-#endif // DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS4_CUBE2D_LOCALFINITEELEMENT_HH
+#endif // DUNE_LOCALFUNCTIONS_BREZZIDOUGLASMARINI1_SIMPLEX2D_LOCALFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomascube.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomascube.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_CUBE_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_CUBE_HH
 
 #include "raviartthomas0cube2d.hh"
 #include "raviartthomas0cube3d.hh"
 #include "raviartthomas1cube2d.hh"
 #include "raviartthomas1cube3d.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomaslfecache.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomaslfecache.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMASLFECACHE_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMASLFECACHE_HH
 
 #include <tuple>
 #include <utility>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexbasis.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RAVIARTTHOMASBASIS_HH
 #define DUNE_RAVIARTTHOMASBASIS_HH
 
 #include <fstream>
 #include <dune/common/exceptions.hh>
 
 #include <dune/localfunctions/utility/defaultbasisfactory.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexinterpolation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMASSIMPLEX_RAVIARTTHOMASSIMPLEXINTERPOLATION_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_RAVIARTTHOMASSIMPLEX_RAVIARTTHOMASSIMPLEXINTERPOLATION_HH
 
 #include <fstream>
 #include <utility>
 
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexprebasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexprebasis.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RAVIARTTHOMASPREBASIS_HH
 #define DUNE_RAVIARTTHOMASPREBASIS_HH
 
 #include <fstream>
 #include <utility>
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas/raviartthomassimplex.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas/raviartthomassimplex.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_SIMPLEX_HH
 #define DUNE_LOCALFUNCTIONS_RAVIARTTHOMAS_SIMPLEX_HH
 
 #include <dune/localfunctions/utility/localfiniteelement.hh>
 #include "raviartthomassimplex/raviartthomassimplexbasis.hh"
 
 /**
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/raviartthomas.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/raviartthomas.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_RAVIARTTHOMASFINITEELEMENT_HH
 #define DUNE_RAVIARTTHOMASFINITEELEMENT_HH
 
 // Raviart-Thomas implementations with run-time order
 #include <dune/localfunctions/raviartthomas/raviartthomascube.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomassimplex.hh>
 
@@ -15,11 +13,9 @@
 #include <dune/localfunctions/raviartthomas/raviartthomas03d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas0cube2d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas1cube2d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas2cube2d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas3cube2d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas0cube3d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas1cube3d.hh>
-#include <dune/localfunctions/raviartthomas/raviartthomas0pyramid.hh>
-#include <dune/localfunctions/raviartthomas/raviartthomas0prism.hh>
 
 #endif // #ifndef DUNE_RAVIARTTHOMASFINITEELEMENT_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/common/refinedsimplexlocalbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/common/refinedsimplexlocalbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_REFINED_SIMPLEX_LOCALBASIS_HH
 #define DUNE_REFINED_SIMPLEX_LOCALBASIS_HH
 
 /** \file
     \brief Contains a base class for LocalBasis classes based on uniform refinement
  */
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/refinedp0localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/refinedp0localbasis.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_REFINED_P0_LOCALBASIS_HH
 #define DUNE_REFINED_P0_LOCALBASIS_HH
 
 #include <numeric>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/refinedp0localcoefficients.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-edges0.5.cc`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-#ifndef DUNE_REFINED_P0_LOCALCOEFFICIENTS_HH
-#define DUNE_REFINED_P0_LOCALCOEFFICIENTS_HH
+
+#ifdef HAVE_CONFIG_H
+#include "config.h"
+#endif
 
 #include <cstddef>
 #include <iostream>
-#include <vector>
+#include <ostream>
+
+#include <dune/common/exceptions.hh>
+#include <dune/common/fvector.hh>
+
+#include <dune/geometry/type.hh>
+#include <dune/geometry/generalvertexorder.hh>
+
+#include <dune/localfunctions/whitney/edges0.5.hh>
 
-#include <dune/localfunctions/common/localkey.hh>
+#include "geometries.hh"
+#include "test-fe.hh"
 
-namespace Dune
-{
+template<std::size_t dim>
+void testEdgeS0_5(int &result) {
+  // tolerance for floating-point comparisons
+  static const double eps = 1e-9;
+  // stepsize for numerical differentiation
+  static const double delta = 1e-5;
 
-  /**@ingroup LocalLayoutImplementation
-     \brief Layout map for RefinedP0 elements
-
-     \nosubgrouping
-     \implements Dune::LocalCoefficientsVirtualImp
-   */
-  template<unsigned int k>
-  class RefinedP0LocalCoefficients
-  {
-    // 2 to the k-th power
-    constexpr static int N = 1<<k;
-
-  public:
-    RefinedP0LocalCoefficients () :
-      localKeys_(N)
-    {
-      // All functions are associated to the element
-      for (int i = 0; i < N; ++i)
-        localKeys_[i] = LocalKey(0,0,i);
-    }
-
-    //! number of coefficients
-    std::size_t size () const
-    {
-      return N;
-    }
-
-    //! get i'th index
-    const LocalKey& localKey (std::size_t i) const
-    {
-      return localKeys_[i];
-    }
+  std::cout << "== Checking global-valued EdgeS0_5 elements (with "
+            << "dim=" << dim << ")" << std::endl;
 
-  private:
-    std::vector<LocalKey> localKeys_;
+  Dune::GeometryType gt(Dune::GeometryTypes::simplex(dim));
 
-  };
+  typedef TestGeometries<double, dim> TestGeos;
+  static const TestGeos testGeos;
 
+  typedef typename TestGeos::Geometry Geometry;
+  const Geometry &geo = testGeos.get(gt);
+
+  static_assert(dim <= 3, "Need to update vertexIds array for dim > 3");
+  std::size_t vertexIds[] = {0, 1, 2, 3};
+  Dune::GeneralVertexOrder<dim, std::size_t>
+  vo(gt, vertexIds+0, vertexIds+dim+1);
+
+  Dune::EdgeS0_5FiniteElementFactory<Geometry, double> feFactory;
+  bool success = testFE(geo, feFactory.make(geo, vo), eps, delta);
+
+  if(success && result != 1)
+    result = 0;
+  else
+    result = 1;
 }
 
-#endif
+int main(int argc, char** argv) {
+  try {
+    int result = 77;
+
+    testEdgeS0_5<2>(result);
+    testEdgeS0_5<3>(result);
+
+    return result;
+  }
+  catch (const Dune::Exception& e) {
+    std::cout << e << std::endl;
+    throw;
+  }
+}
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0/refinedp0localinterpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0/refinedp0localinterpolation.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_REFINED_P0_LOCALINTERPOLATION_HH
 #define DUNE_REFINED_P0_LOCALINTERPOLATION_HH
 
 #include <dune/localfunctions/refined/refinedp0/refinedp0localbasis.hh>
 #include <dune/localfunctions/common/localinterpolation.hh>
 
 namespace Dune
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp0.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp0.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_REFINED_P0_LOCALFINITEELEMENT_HH
 #define DUNE_REFINED_P0_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include <dune/localfunctions/lagrange/p0.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp1/refinedp1localbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp1/refinedp1localbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_REFINED_P1_LOCALBASIS_HH
 #define DUNE_REFINED_P1_LOCALBASIS_HH
 
 /** \file
     \brief Linear Lagrange shape functions on a uniformly refined reference element
  */
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/refined/refinedp1.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/refined/refinedp1.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_REFINED_REFINEDP1_HH
 #define DUNE_LOCALFUNCTIONS_REFINED_REFINEDP1_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
 #include <dune/localfunctions/lagrange/p0.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/CMakeLists.txt` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_definitions(-DDUNE_DEPRECATED_INTERPOLATE_CHECK=1)
 
 dune_add_test(SOURCES bdfmelementtest.cc)
 
 dune_add_test(SOURCES brezzidouglasmarinielementtest.cc)
 
 dune_add_test(SOURCES crouzeixraviartelementtest.cc)
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/bdfmelementtest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/bdfmelementtest.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/localfunctions/brezzidouglasfortinmarini/bdfmcube.hh>
 
 #include <dune/localfunctions/test/test-localfe.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/brezzidouglasmarinielementtest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/brezzidouglasmarinielementtest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/localfunctions/brezzidouglasmarini.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/geometries.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/geometries.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 // This header is not part of the official Dune API and might be subject
 // to change.  You can use this header to test external finite element
 // implementations, but be warned that your tests might break with future
 // Dune versions.
 
 #ifndef DUNE_LOCALFUNCTIONS_TEST_GEOMETRIES_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/globalmonomialfunctionstest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/globalmonomialfunctionstest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstddef>
 #include <iostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/hierarchicalelementtest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/hierarchicalelementtest.cc`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/localfunctions/hierarchical.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/lagrangeshapefunctiontest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/lagrangeshapefunctiontest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <iostream>
 #include <typeinfo>
 #include <fenv.h>
 
 #include <dune/localfunctions/lagrange/p0.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/monomialshapefunctiontest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/monomialshapefunctiontest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/geometry/quadraturerules.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/nedelec1stkindelementtest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/nedelec1stkindelementtest.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include "config.h"
 
 #include <dune/localfunctions/nedelec/nedelec1stkindsimplex.hh>
 #include <dune/localfunctions/nedelec/nedelec1stkindcube.hh>
 
 #include <dune/localfunctions/test/test-localfe.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/rannacherturekelementtest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/rannacherturekelementtest.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <iostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/raviartthomaselementtest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/raviartthomaselementtest.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/localfunctions/raviartthomas/raviartthomassimplex.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomascube.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas02d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas03d.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomaslfecache.hh>
 #include <dune/localfunctions/raviartthomas/raviartthomas12d.hh>
-#include <dune/localfunctions/raviartthomas.hh>
 
 #include <dune/localfunctions/test/test-localfe.hh>
 
 int main(int argc, char** argv)
 {
   bool success = true;
 
@@ -138,31 +135,14 @@
   TEST_FE(rt1cube3dlfemDedicated);
   for (unsigned int s = 0; s < 64; s++)
   {
     Dune::RT1Cube3DLocalFiniteElement<double,double> rt1cube3dlfemDedicated(s);
     TEST_FE(rt1cube3dlfemDedicated);
   }
 
-  Dune::RT0PyramidLocalFiniteElement<double,double> rt0pyramidlfemDedicated;
-  TEST_FE(rt0pyramidlfemDedicated);
-  for (unsigned int s = 0; s < 32; s++)
-  {
-    Dune::RT0PyramidLocalFiniteElement<double,double> rt0pyramidlfemDedicated(s);
-    TEST_FE(rt0pyramidlfemDedicated);
-  }
-
-  Dune::RT0PrismLocalFiniteElement<double,double> rt0prismlfemDedicated;
-  TEST_FE(rt0prismlfemDedicated);
-  for (unsigned int s = 0; s < 32; s++)
-  {
-    Dune::RT0PrismLocalFiniteElement<double,double> rt0prismlfemDedicated(s);
-    TEST_FE(rt0prismlfemDedicated);
-  }
-
-
   // Test the RaviartThomasLocalFiniteElementCache
   Dune::RaviartThomasLocalFiniteElementCache<double,double,2,0> lagrangeLFECache;
   TEST_FE(lagrangeLFECache.get(Dune::GeometryTypes::simplex(2)));
   TEST_FE(lagrangeLFECache.get(Dune::GeometryTypes::cube(2)));
 
   // Test whether asking the cache for an element of the wrong dimension throws an exception
   bool lagrangeLFESuccess = false;
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-edges0.5.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-pk2d.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstddef>
 #include <iostream>
 #include <ostream>
+#include <utility>
 
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
+#include <dune/common/hybridutilities.hh>
 
 #include <dune/geometry/type.hh>
 #include <dune/geometry/generalvertexorder.hh>
 
-#include <dune/localfunctions/whitney/edges0.5.hh>
+#include <dune/localfunctions/lagrange/pk2d.hh>
 
 #include "geometries.hh"
 #include "test-fe.hh"
 
-template<std::size_t dim>
-void testEdgeS0_5(int &result) {
-  // tolerance for floating-point comparisons
-  static const double eps = 1e-9;
-  // stepsize for numerical differentiation
-  static const double delta = 1e-5;
-
-  std::cout << "== Checking global-valued EdgeS0_5 elements (with "
-            << "dim=" << dim << ")" << std::endl;
-
-  Dune::GeometryType gt(Dune::GeometryTypes::simplex(dim));
-
-  typedef TestGeometries<double, dim> TestGeos;
-  static const TestGeos testGeos;
-
-  typedef typename TestGeos::Geometry Geometry;
-  const Geometry &geo = testGeos.get(gt);
-
-  static_assert(dim <= 3, "Need to update vertexIds array for dim > 3");
-  std::size_t vertexIds[] = {0, 1, 2, 3};
-  Dune::GeneralVertexOrder<dim, std::size_t>
-  vo(gt, vertexIds+0, vertexIds+dim+1);
-
-  Dune::EdgeS0_5FiniteElementFactory<Geometry, double> feFactory;
-  bool success = testFE(geo, feFactory.make(geo, vo), eps, delta);
-
-  if(success && result != 1)
-    result = 0;
-  else
-    result = 1;
+// tolerance for floating-point comparisons
+static const double eps = 1e-9;
+// stepsize for numerical differentiation
+static const double delta = 1e-5;
+
+template<int k>
+static void test(int &result)
+{
+    std::cout << "== Checking global-valued Pk2D elements (with k=" << k << ")"
+              << std::endl;
+
+    Dune::GeometryType gt(Dune::GeometryTypes::triangle);
+
+    typedef TestGeometries<double, 2> TestGeos;
+    static const TestGeos testGeos;
+
+    typedef TestGeos::Geometry Geometry;
+    const Geometry &geo = testGeos.get(gt);
+
+    std::size_t vertexIds[] = {0, 1, 2};
+    Dune::GeneralVertexOrder<2, std::size_t>
+    vo(gt, vertexIds+0, vertexIds+3);
+
+    Dune::Pk2DFiniteElementFactory<Geometry, double, k> feFactory;
+    bool success = testFE(geo, feFactory.make(geo, vo), eps, delta);
+
+    if(success && result != 1)
+      result = 0;
+    else
+      result = 1;
 }
 
 int main(int argc, char** argv) {
   try {
     int result = 77;
 
-    testEdgeS0_5<2>(result);
-    testEdgeS0_5<3>(result);
+    static constexpr std::size_t max_k = 20;
+    Dune::Hybrid::forEach(std::make_index_sequence<max_k+1>{},[&](auto i){test<i>(result);});
 
     return result;
   }
   catch (const Dune::Exception& e) {
-    std::cout << e << std::endl;
+    std::cerr << e << std::endl;
     throw;
   }
 }
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-fe.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-fe.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 // This header is not part of the official Dune API and might be subject
 // to change.  You can use this header to test external finite element
 // implementations, but be warned that your tests might break with future
 // Dune versions.
 
 #ifndef DUNE_LOCALFUNCTIONS_TEST_TEST_FE_HH
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-finiteelementcache.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-finiteelementcache.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <utility>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-lagrange.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-lagrange.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/utility/field.hh>
 #include <dune/localfunctions/utility/basisprint.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-localfe.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-localfe.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_TEST_TEST_LOCALFE_HH
 #define DUNE_LOCALFUNCTIONS_TEST_TEST_LOCALFE_HH
 
 /** \file \brief Unit tests for LocalFiniteElement objects
  *
  * \note This header is not part of the official Dune API and might be subject
  *  to change.  You can use this header to test external finite element
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-nedelecsimplex.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-nedelecsimplex.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <dune/localfunctions/nedelec/nedelecsimplex/nedelecsimplexbasis.hh>
 #include <dune/localfunctions/utility/field.hh>
 #include <dune/localfunctions/utility/basisprint.hh>
 
 /**
  * \file
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-orthonormal.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-orthonormal.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <dune/geometry/type.hh>
 #include <dune/geometry/quadraturerules.hh>
 
 #include <dune/localfunctions/utility/field.hh>
 #include <dune/localfunctions/utility/basisprint.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-pk2d.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-q2.cc`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,61 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstddef>
 #include <iostream>
 #include <ostream>
-#include <utility>
 
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
-#include <dune/common/hybridutilities.hh>
 
 #include <dune/geometry/type.hh>
-#include <dune/geometry/generalvertexorder.hh>
 
-#include <dune/localfunctions/lagrange/pk2d.hh>
+#include <dune/localfunctions/lagrange/q2.hh>
 
 #include "geometries.hh"
 #include "test-fe.hh"
 
-// tolerance for floating-point comparisons
-static const double eps = 1e-9;
-// stepsize for numerical differentiation
-static const double delta = 1e-5;
-
-template<int k>
-static void test(int &result)
+template <int dim>
+void test(const double& eps, const double& delta, int& result)
 {
-    std::cout << "== Checking global-valued Pk2D elements (with k=" << k << ")"
-              << std::endl;
+  std::cout << "== Checking global-valued Q2 " << dim << "D elements" << std::endl;
 
-    Dune::GeometryType gt(Dune::GeometryTypes::triangle);
+  Dune::GeometryType gt(Dune::GeometryTypes::cube(dim));
 
-    typedef TestGeometries<double, 2> TestGeos;
-    static const TestGeos testGeos;
+  typedef TestGeometries<double, dim> TestGeos;
+  static const TestGeos testGeos;
 
-    typedef TestGeos::Geometry Geometry;
-    const Geometry &geo = testGeos.get(gt);
+  typedef typename TestGeos::Geometry Geometry;
+  const Geometry &geo = testGeos.get(gt);
 
-    std::size_t vertexIds[] = {0, 1, 2};
-    Dune::GeneralVertexOrder<2, std::size_t>
-    vo(gt, vertexIds+0, vertexIds+3);
+  Dune::Q2FiniteElementFactory<Geometry, double> feFactory;
+  bool success = testFE(geo, feFactory.make(geo), eps, delta);
 
-    Dune::Pk2DFiniteElementFactory<Geometry, double, k> feFactory;
-    bool success = testFE(geo, feFactory.make(geo, vo), eps, delta);
-
-    if(success && result != 1)
-      result = 0;
-    else
-      result = 1;
+  if(success && result != 1)
+    result = 0;
+  else
+    result = 1;
 }
 
 int main(int argc, char** argv) {
   try {
+    // tolerance for floating-point comparisons
+    static const double eps = 1e-9;
+    // stepsize for numerical differentiation
+    static const double delta = 1e-5;
+
     int result = 77;
 
-    static constexpr std::size_t max_k = 20;
-    Dune::Hybrid::forEach(std::make_index_sequence<max_k+1>{},[&](auto i){test<i>(result);});
+    test<1>(eps, delta, result);
+    test<2>(eps, delta, result);
+    test<3>(eps, delta, result);
 
     return result;
   }
   catch (const Dune::Exception& e) {
     std::cerr << e << std::endl;
     throw;
   }
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-power-monomial.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-power-monomial.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstddef>
 #include <iostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-q1.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-q1.cc`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstddef>
 #include <iostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/test-raviartthomassimplex.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/test-raviartthomassimplex.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <dune/localfunctions/raviartthomas/raviartthomassimplex/raviartthomassimplexbasis.hh>
 #include <dune/localfunctions/utility/field.hh>
 #include <dune/localfunctions/utility/basisprint.hh>
 
 /**
  * \file
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/testgenericfem.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/testgenericfem.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cstddef>
 #include <iostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/test/virtualshapefunctiontest.cc` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/test/virtualshapefunctiontest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #undef DUNE_VIRTUAL_SHAPEFUNCTIONS
 
 #include <array>
 #include <cstddef>
 #include <iostream>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/basisevaluator.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/basisevaluator.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_BASISEVALUATOR_HH
 #define DUNE_BASISEVALUATOR_HH
 
 #include <vector>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/basismatrix.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/basismatrix.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_BASISMATRIX_HH
 #define DUNE_BASISMATRIX_HH
 
 #include <fstream>
 #include <dune/common/exceptions.hh>
 
 #include <dune/localfunctions/utility/lfematrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/basisprint.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/basisprint.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef BASISPRINT
 #define BASISPRINT
 #include <dune/localfunctions/utility/multiindex.hh>
 #include <dune/localfunctions/utility/polynomialbasis.hh>
 namespace Dune {
   /**********************************************
   * Methods for printing a PolynomialBasis.
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/coeffmatrix.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/coeffmatrix.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_COEFFMATRIX_HH
 #define DUNE_COEFFMATRIX_HH
 #include <cassert>
 #include <iostream>
 #include <vector>
 #include <dune/common/fvector.hh>
 #include <dune/localfunctions/utility/field.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/defaultbasisfactory.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/defaultbasisfactory.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DEFAULTBASISFACTORY_HH
 #define DUNE_DEFAULTBASISFACTORY_HH
 
 #include <fstream>
 #include <dune/common/exceptions.hh>
 
 #include <dune/localfunctions/utility/basismatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/field.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/field.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_UTILITY_FIELD_HH
 #define DUNE_LOCALFUNCTIONS_UTILITY_FIELD_HH
 
 #include <dune/common/gmpfield.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/interpolationhelper.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/interpolationhelper.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef GENERIC_INTERPOLATIONHELPER_HH
 #define GENERIC_INTERPOLATIONHELPER_HH
 
 #include <vector>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/concept.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/l2interpolation.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/l2interpolation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_L2INTERPOLATION_HH
 #define DUNE_L2INTERPOLATION_HH
 
 #include <dune/common/concept.hh>
 
 #include <dune/geometry/quadraturerules.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/lfematrix.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/lfematrix.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_LOCALFUNCTIONS_UTILITY_LFEMATRIX_HH
 #define DUNE_LOCALFUNCTIONS_UTILITY_LFEMATRIX_HH
 
 #include <cassert>
 #include <vector>
 
 #include "field.hh"
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/localfiniteelement.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/localfiniteelement.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GENERIC_LOCALFINITEELEMENT_HH
 #define DUNE_GENERIC_LOCALFINITEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 #include <dune/geometry/typeindex.hh>
 
 #include <dune/localfunctions/common/localfiniteelementtraits.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/monomialbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/monomialbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MONOMIALBASIS_HH
 #define DUNE_MONOMIALBASIS_HH
 
 #include <vector>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/multiindex.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/multiindex.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_MULTIINDEX_HH
 #define DUNE_MULTIINDEX_HH
 
 #include <vector>
 #include <ostream>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/polynomialbasis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/polynomialbasis.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_POLYNOMIALBASIS_HH
 #define DUNE_POLYNOMIALBASIS_HH
 
 #include <fstream>
 #include <numeric>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/utility/tensor.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/utility/tensor.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_TENSOR_HH
 #define DUNE_TENSOR_HH
 
 #include <ostream>
 #include <vector>
 
@@ -835,15 +833,15 @@
   template <int dimD,
       class F1,unsigned int deriv,
       class F2>
   struct DerivativeAssign<Derivatives<F1,dimD,1,deriv,DerivativeLayoutNS::derivative>,FieldVector<F2,1> >
   {
     typedef Derivatives<F1,dimD,1,deriv,DerivativeLayoutNS::derivative> Vec1;
     typedef FieldVector<F2,1> Vec2;
-    static void apply(unsigned int /*r*/,const Vec1 &vec1,Vec2 &vec2)
+    static void apply(unsigned int r,const Vec1 &vec1,Vec2 &vec2)
     {
       field_cast(vec1[0].template tensor<0>()[0].block(),vec2);
     }
   };
 
   // ***********************************************
   // IO ********************************************
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/basis.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/basis.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_BASIS_HH
 #define DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_BASIS_HH
 
 #include <cstddef>
 #include <vector>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5/common.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5/common.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_COMMON_HH
 #define DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_COMMON_HH
 
 #include <cstddef>
 
 #include <dune/geometry/dimension.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/localfunctions/whitney/edges0.5.hh` & `dune-localfunctions-2.9.dev20220529/dune/localfunctions/whitney/edges0.5.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_HH
 #define DUNE_LOCALFUNCTIONS_WHITNEY_EDGES0_5_HH
 
 #include <dune/geometry/type.hh>
 
 #include <dune/localfunctions/whitney/edges0.5/basis.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/dune/python/localfunctions/localfiniteelement.hh` & `dune-localfunctions-2.9.dev20220529/dune/python/localfunctions/localfiniteelement.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_LOCALFUNCTIONS_LOCALFINITEELEMENT_HH
 #define DUNE_PYTHON_LOCALFUNCTIONS_LOCALFINITEELEMENT_HH
 
 #include <dune/python/pybind11/pybind11.h>
 
 #include <dune/common/visibility.hh>
 #include <dune/localfunctions/common/localkey.hh>
```

### Comparing `dune-localfunctions-2.9.0rc1/pyproject.toml` & `dune-localfunctions-2.9.dev20220529/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # This is uses the `Python-Requires` field in the `dune.modules` file to
 # populate the `requires` entry. Additional packages needed for the package
 # build should be added in the `dune.modules`. These packages will then also be
 # included in the package install from source.
 #
 [build-system]
-requires = ['cmake>=3.13', 'dune-geometry<=v2.9.0rc1', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
+requires = ['cmake>=3.13', 'dune-geometry<=2.9.dev20220529', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
```

### Comparing `dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/PKG-INFO` & `dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-localfunctions
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Provides interface and implementation for shape functions defined on the DUNE reference elements
 Home-page: https://gitlab.dune-project.org/core/dune-localfunctions
 Author: The Dune Core developers
 Author-email: dune-devel@lists.dune-project.org
 License: UNKNOWN
-Description: <!--
-        SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-        SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-        -->
-        
-        DUNE-library
+Description: DUNE-library
         ============
         
         DUNE, the Distributed and Unified Numerics Environment is a modular toolbox
         for solving partial differential equations with grid-based methods.
         
         The main intention is to create slim interfaces allowing an efficient use of
         legacy and/or new libraries. Using C++ techniques DUNE allows to use very
@@ -35,15 +30,15 @@
         More information
         ----------------
         
         Check dune-common for more details concerning dependencies, known bugs,
         license and installation.
         
         
-        git-f610b1b0035edeb445499e1db70ace8f062b9067
+        git-e93e57d677b10bb963b4c41cb610c6f250398433
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-localfunctions-2.9.0rc1/python/dune_localfunctions.egg-info/SOURCES.txt` & `dune-localfunctions-2.9.dev20220529/python/dune_localfunctions.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 LICENSE.md
 README.md
 config.h.cmake
 dune-localfunctions.pc.in
 dune.module
 pyproject.toml
 setup.py
-LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
 doc/CMakeLists.txt
 doc/dune-localfunctions-manual.tex
 doc/doxygen/CMakeLists.txt
 doc/doxygen/Doxylocal
 doc/doxygen/mainpage.txt
 doc/doxygen/modules.txt
 dune/CMakeLists.txt
@@ -168,16 +167,14 @@
 dune/localfunctions/rannacherturek/rannacherturek3d/CMakeLists.txt
 dune/localfunctions/rannacherturek/rannacherturek3d/rannacherturek3dlocalbasis.hh
 dune/localfunctions/raviartthomas/CMakeLists.txt
 dune/localfunctions/raviartthomas/raviartthomas02d.hh
 dune/localfunctions/raviartthomas/raviartthomas03d.hh
 dune/localfunctions/raviartthomas/raviartthomas0cube2d.hh
 dune/localfunctions/raviartthomas/raviartthomas0cube3d.hh
-dune/localfunctions/raviartthomas/raviartthomas0prism.hh
-dune/localfunctions/raviartthomas/raviartthomas0pyramid.hh
 dune/localfunctions/raviartthomas/raviartthomas12d.hh
 dune/localfunctions/raviartthomas/raviartthomas1cube2d.hh
 dune/localfunctions/raviartthomas/raviartthomas1cube3d.hh
 dune/localfunctions/raviartthomas/raviartthomas2cube2d.hh
 dune/localfunctions/raviartthomas/raviartthomas3cube2d.hh
 dune/localfunctions/raviartthomas/raviartthomas4cube2d.hh
 dune/localfunctions/raviartthomas/raviartthomascube.hh
@@ -191,22 +188,14 @@
 dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalbasis.hh
 dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalcoefficients.hh
 dune/localfunctions/raviartthomas/raviartthomas03d/raviartthomas03dlocalinterpolation.hh
 dune/localfunctions/raviartthomas/raviartthomas0cube2d/CMakeLists.txt
 dune/localfunctions/raviartthomas/raviartthomas0cube2d/raviartthomas0cube2dall.hh
 dune/localfunctions/raviartthomas/raviartthomas0cube3d/CMakeLists.txt
 dune/localfunctions/raviartthomas/raviartthomas0cube3d/raviartthomas0cube3dall.hh
-dune/localfunctions/raviartthomas/raviartthomas0prism/CMakeLists.txt
-dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalbasis.hh
-dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalcoefficients.hh
-dune/localfunctions/raviartthomas/raviartthomas0prism/raviartthomas0prismlocalinterpolation.hh
-dune/localfunctions/raviartthomas/raviartthomas0pyramid/CMakeLists.txt
-dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalbasis.hh
-dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalcoefficients.hh
-dune/localfunctions/raviartthomas/raviartthomas0pyramid/raviartthomas0pyramidlocalinterpolation.hh
 dune/localfunctions/raviartthomas/raviartthomas12d/CMakeLists.txt
 dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalbasis.hh
 dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalcoefficients.hh
 dune/localfunctions/raviartthomas/raviartthomas12d/raviartthomas12dlocalinterpolation.hh
 dune/localfunctions/raviartthomas/raviartthomas1cube2d/CMakeLists.txt
 dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalbasis.hh
 dune/localfunctions/raviartthomas/raviartthomas1cube2d/raviartthomas1cube2dlocalcoefficients.hh
```

