# Comparing `tmp/dune-istl-2.9.0rc1.tar.gz` & `tmp/dune-istl-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-istl-2.9.0rc1.tar", last modified: Fri Oct 21 08:16:45 2022, max compression
+gzip compressed data, was "dune-istl-2.9.dev20220529.tar", last modified: Sun May 29 21:03:25 2022, max compression
```

## Comparing `dune-istl-2.9.0rc1.tar` & `dune-istl-2.9.dev20220529.tar`

### file list

```diff
@@ -1,230 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9167 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20628 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)    20628 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.728019 dune-istl-2.9.0rc1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    19036 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.728019 dune-istl-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.728019 dune-istl-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/AddARPACKPPFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/AddSuperLUFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/DuneIstlMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/FindARPACK.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/FindARPACKPP.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/cmake/modules/FindSuperLU.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.732019 dune-istl-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)   859026 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/blockstructure.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/blockstructure.eps.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.732019 dune-istl-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/doxygen/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/doxygen/modules.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5154 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/istl.bib
--rw-r--r--   0 runner    (1001) docker     (121)    34346 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/doc/istl.tex
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.732019 dune-istl-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.736019 dune-istl-2.9.0rc1/dune/istl/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/allocator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13066 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/basearray.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/bccsmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9592 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/bccsmatrixinitializer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    78085 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/bcrsmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/bdmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5801 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/blocklevel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6963 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/btdmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    32872 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/bvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12825 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/cholmod.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.736019 dune-istl-2.9.0rc1/dune/istl/common/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/common/counter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/common/registry.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.736019 dune-istl-2.9.0rc1/dune/istl/eigenvalue/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/eigenvalue/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    41726 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/eigenvalue/arpackpp.hh
--rw-r--r--   0 runner    (1001) docker     (121)    43279 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/eigenvalue/poweriteration.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.736019 dune-istl-2.9.0rc1/dune/istl/eigenvalue/test/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/eigenvalue/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/eigenvalue/test/cond2test.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15062 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/eigenvalue/test/matrixinfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6513 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/foreach.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21815 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/gsetc.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6718 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/ildl.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14277 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/ilu.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7344 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/ilusubdomainsolver.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28842 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/io.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/istlexception.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12982 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/ldl.hh
--rw-r--r--   0 runner    (1001) docker     (121)    30524 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/matrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/matrixindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    41062 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/matrixmarket.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19721 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/matrixmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29297 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/matrixredistribute.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13692 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/matrixutils.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22647 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/multitypeblockmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11164 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/multitypeblockvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13717 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/novlpschwarz.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5510 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/operators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    52405 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/overlappingschwarz.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23489 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/owneroverlapcopy.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.736019 dune-istl-2.9.0rc1/dune/istl/paamg/
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    85259 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/aggregates.hh
--rw-r--r--   0 runner    (1001) docker     (121)    54601 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/amg.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/combinedfunctor.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4951 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/construction.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11342 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/dependency.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28690 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/fastamg.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/fastamgsmoother.hh
--rw-r--r--   0 runner    (1001) docker     (121)    27403 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/galerkin.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8127 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/globalaggregates.hh
--rw-r--r--   0 runner    (1001) docker     (121)    75294 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/graph.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3049 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/graphcreator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12140 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/hierarchy.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15055 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/indicescoarsener.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12469 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/kamg.hh
--rw-r--r--   0 runner    (1001) docker     (121)    37670 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/matrixhierarchy.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14909 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/parameters.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/pinfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/properties.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/renumberer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26347 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/smoother.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.740019 dune-istl-2.9.0rc1/dune/istl/paamg/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6207 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/amgtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6001 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/anisotropic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3969 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/fastamg.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/galerkintest.cc
--rw-r--r--   0 runner    (1001) docker     (121)   124630 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/gr_30_30.mm
--rw-r--r--   0 runner    (1001) docker     (121)    14635 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/graphtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/hierarchytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5718 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/kamgtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/pamgmmtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6208 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/parallelamgtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/pthreadamgtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/pthreadtwoleveltest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/transfertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/test/twolevelmethodtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8225 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/transfer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17483 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/paamg/twolevelmethod.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/preconditioner.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29700 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/preconditioners.hh
--rw-r--r--   0 runner    (1001) docker     (121)    64799 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/repartition.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8060 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/scalarproducts.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13644 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/scaledidmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12605 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/schwarz.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19859 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/solver.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/solvercategory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/solverfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3468 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/solverregistry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    62633 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/solvers.hh
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/solvertype.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13309 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/spqr.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24827 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/superlu.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/superlufunctions.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9838 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/supermatrix.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/dune/istl/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/bcrsassigntest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/bcrsbuild.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9952 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/bcrsimplicitbuild.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/bcrsmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/bcrsnormtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/blocklevel.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5647 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/bvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/cgconditiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4558 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/cholmodtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15923 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/complexdata.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5690 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/complexmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8931 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/complexrhstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6160 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/dotproducttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/fieldvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3918 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/foreachtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/hilbertmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/iluildltest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/inverseoperator2prectest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5680 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/iotest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/laplacian.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/ldltest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixiteratortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixmarkettest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixnormtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixredisttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    20914 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixtest.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/matrixutilstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/mmtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/multirhstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6803 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/multirhstest.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10810 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/multitypeblockmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/multitypeblockvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/mv.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8723 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/overlappingschwarztest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/preconditionerstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/registrytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/scalarproductstest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/scaledidmatrixtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3844 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/solveraborttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/solverfactorytest.cc.in
--rw-r--r--   0 runner    (1001) docker     (121)     6142 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/solverfactorytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/solvertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/spqrtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/superlutest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/umfpacktest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/vbvectortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4971 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/vectorcommtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8486 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/test/vectortest.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22555 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/umfpack.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19834 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/istl/vbvector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/dune/python/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/dune/python/istl/
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18229 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/bcrsmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9551 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/bvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5667 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/matrixindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/operators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7707 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/preconditioners.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/slice.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11507 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/istl/solvers.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/dune/python/test/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/test/bcrsmatrix.mm
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/test/bcrsmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/test/bcrsmatrix.txt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune/python/test/bcrsmatrix.txt.license
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune-istl.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/dune.module
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/python/dune/istl/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune/istl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune/istl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune/istl/_istl.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/python/dune_istl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune_istl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune_istl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune_istl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune_istl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/python/dune_istl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:45.744019 dune-istl-2.9.0rc1/src/
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6945 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/src/istl-solver-playground.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/src/istl-solver-playground.hh
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-21 08:16:45.000000 dune-istl-2.9.0rc1/src/playground.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     8837 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20628 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)    20628 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.371631 dune-istl-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.375631 dune-istl-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/AddARPACKPPFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/AddSuperLUFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/DuneIstlMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/FindARPACK.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4747 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/FindARPACKPP.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/cmake/modules/FindSuperLU.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.375631 dune-istl-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   859026 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/blockstructure.eps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.375631 dune-istl-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/doxygen/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/doxygen/modules.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4965 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/istl.bib
+-rw-r--r--   0 runner    (1001) docker     (121)    34172 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/doc/istl.tex
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.375631 dune-istl-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.379631 dune-istl-2.9.dev20220529/dune/istl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12891 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/basearray.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3715 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/bccsmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9417 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/bccsmatrixinitializer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    77910 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/bcrsmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/bdmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/blocklevel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6788 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/btdmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    32697 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/bvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12650 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/cholmod.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.379631 dune-istl-2.9.dev20220529/dune/istl/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/common/counter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/common/registry.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.379631 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    41551 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/arpackpp.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    43104 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/poweriteration.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.383631 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/test/cond2test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14887 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/eigenvalue/test/matrixinfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6338 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/foreach.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21640 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/gsetc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/ildl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14102 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/ilu.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7169 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/ilusubdomainsolver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28297 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/io.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/istlexception.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12807 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/ldl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    30349 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/matrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/matrixindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    40887 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/matrixmarket.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19546 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/matrixmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    29122 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/matrixredistribute.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13517 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/matrixutils.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22472 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/multitypeblockmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10989 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/multitypeblockvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13676 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/novlpschwarz.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5335 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/operators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    52230 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/overlappingschwarz.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23314 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/owneroverlapcopy.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.383631 dune-istl-2.9.dev20220529/dune/istl/paamg/
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    85084 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/aggregates.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    54426 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/amg.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/combinedfunctor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/construction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11167 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/dependency.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28515 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/fastamg.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/fastamgsmoother.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27228 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/galerkin.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7952 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/globalaggregates.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    75119 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/graph.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/graphcreator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11965 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/hierarchy.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14880 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/indicescoarsener.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12294 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/kamg.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    37495 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/matrixhierarchy.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14734 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/parameters.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/pinfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/properties.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/renumberer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26172 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/smoother.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.383631 dune-istl-2.9.dev20220529/dune/istl/paamg/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/amgtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5826 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/anisotropic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/fastamg.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6312 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/galerkintest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)   124457 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/gr_30_30.mm
+-rw-r--r--   0 runner    (1001) docker     (121)    14460 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/graphtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2598 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/hierarchytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/kamgtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/pamgmmtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/parallelamgtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/pthreadamgtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6320 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/pthreadtwoleveltest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/transfertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/test/twolevelmethodtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8050 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/transfer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17308 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/paamg/twolevelmethod.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/preconditioner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    29525 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/preconditioners.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    64624 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/repartition.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7885 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/scalarproducts.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13469 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/scaledidmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12564 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/schwarz.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19684 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/solver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/solvercategory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9557 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/solverfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/solverregistry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    62458 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/solvers.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/solvertype.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13089 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/spqr.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24652 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/superlu.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/superlufunctions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9663 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/supermatrix.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.387632 dune-istl-2.9.dev20220529/dune/istl/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/bcrsassigntest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/bcrsbuild.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9777 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/bcrsimplicitbuild.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/bcrsmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/bcrsnormtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/blocklevel.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/bvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2879 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/cgconditiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/cholmodtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15748 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/complexdata.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5515 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/complexmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8756 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/complexrhstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/dotproducttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/fieldvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/foreachtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/hilbertmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/iluildltest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/inverseoperator2prectest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5505 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/iotest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/laplacian.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/ldltest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixiteratortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixmarkettest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixnormtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4204 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixredisttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    20739 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixtest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/matrixutilstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/mmtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/multirhstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6628 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/multirhstest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/multitypeblockmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/multitypeblockvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/mv.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/overlappingschwarztest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/preconditionerstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/registrytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/scalarproductstest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/scaledidmatrixtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/solveraborttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/solverfactorytest.cc.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5968 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/solverfactorytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/solvertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/spqrtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/superlutest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/umfpacktest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/vbvectortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4796 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/vectorcommtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/test/vectortest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22380 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/umfpack.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19659 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/istl/vbvector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.387632 dune-istl-2.9.dev20220529/dune/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/dune/python/istl/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18054 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/bcrsmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9376 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/bvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/matrixindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/operators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7532 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/preconditioners.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/slice.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11332 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/istl/solvers.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/dune/python/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/test/bcrsmatrix.mm
+-rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/test/bcrsmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune/python/test/bcrsmatrix.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune-istl.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/dune.module
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/python/dune/istl/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/python/dune/istl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/python/dune/istl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/python/dune/istl/_istl.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/python/dune_istl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/python/dune_istl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/python/dune_istl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/python/dune_istl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/python/dune_istl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/python/dune_istl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:25.000000 dune-istl-2.9.dev20220529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:25.391631 dune-istl-2.9.dev20220529/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/src/istl-solver-playground.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/src/istl-solver-playground.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-05-29 21:03:24.000000 dune-istl-2.9.dev20220529/src/playground.ini
```

### Comparing `dune-istl-2.9.0rc1/.gitlab-ci.yml` & `dune-istl-2.9.dev20220529/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 ---
 include:
   - project: 'core/ci-config'
     ref: master
-    file: 'config/common/releases/2.9.yml'
+    file: 'config/common/master.yml'
   - project: 'core/ci-config'
     ref: master
-    file: 'jobs/common/releases/2.9.yml'
+    file: 'jobs/common/master.yml'
 
 before_script:
   - duneci-install-module https://gitlab.dune-project.org/core/dune-common.git
 
 variables:
 # Suitesparse, as installed with Debian, is thread-parallel using OpenMP.
 # OpenMP silently assumes, it can spawn as many threads as there are cores.
@@ -44,17 +41,7 @@
   image: registry.dune-project.org/docker/ci/ubuntu:18.04
   script: duneci-standard-test
   stage: test
   variables:
     DUNECI_TOOLCHAIN: clang-5-17
     DUNECI_CMAKE_FLAGS: "-DDUNE_ENABLE_PYTHONBINDINGS=OFF"
   tags: [duneci]
-
-reuse:
-  stage: .pre
-  image:
-    name: docker.io/fsfe/reuse:latest
-    entrypoint: [""]
-  tags: [duneci]
-  before_script: ""
-  script:
-    - reuse lint
```

### Comparing `dune-istl-2.9.0rc1/CHANGELOG.md` & `dune-istl-2.9.dev20220529/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 # Master (will become release 2.9)
 
 - Add `const` qualifier to `LinearOperator` and `ScalarProduct` in
   `IterativeSolver`. In particular, the constructors of iterative solvers have
   changed.
 
 - Solvers are more robust if used with multiple right-hand sides and one lane starts with the exact solution.
@@ -31,17 +26,14 @@
 
 - You can now multiply objects of type `ScaledIdentityMatrix` by scalars
   using `operator*`.
 
 - You can now use `std::tuple_element` to get the types of `MultiTypeBlockVector` entries
   and `MultiTypeBlockMatrix` rows.
 
-- The SPQR solver can now work with non-square matrices (a bug which caused a segfault when previously
-  attempting to do it was found and resolved).
-
 ## Deprecations and removals
 
 - The deprecated ILU functions `bilu_backsolve`, `bilu0_decomposition`, `bilu_backsolve`,
   `firstmatrixelement`, and `bilu_decomposition` are removed. Use their camel case
   replacements.
 
 - Remove deprecated `ImplicitModeOverflowExhausted`, use
```

### Comparing `dune-istl-2.9.0rc1/CMakeLists.txt` & `dune-istl-2.9.dev20220529/CMakeLists.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # set up project
 project(dune-istl C CXX)
 
 # general stuff
 cmake_minimum_required(VERSION 3.13)
 
 # guess build tree of dune-common
```

### Comparing `dune-istl-2.9.0rc1/COPYING` & `dune-istl-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-istl-2.9.0rc1/INSTALL` & `dune-istl-2.9.dev20220529/INSTALL`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-<!--
-SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 Installation Instructions
 =========================
 
 For a full explanation of the DUNE installation process please read
 the installation notes [0]. The following introduction is meant for
 the impatient.
```

### Comparing `dune-istl-2.9.0rc1/LICENSE.md` & `dune-istl-2.9.dev20220529/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dune-istl-2.9.0rc1/PKG-INFO` & `dune-istl-2.9.dev20220529/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-istl
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Iterative solver template library which provides generic sparse matrix/vector classes and a variety of solvers based on these classes
 Home-page: https://gitlab.dune-project.org/core/dune-istl
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
@@ -33,15 +28,15 @@
         More information
         ----------------
         
         Check dune-common for more details concerning dependencies, known bugs,
         license and installation.
         
         
-        git-1b0e7e623bef2665fe0139670df809d403c61389
+        git-927da16f4c0d665a2ceba923aecb36a04133656d
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-istl-2.9.0rc1/README.md` & `dune-istl-2.9.dev20220529/README.md`

 * *Files 25% similar despite different names*

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
@@ -25,8 +20,8 @@
 More information
 ----------------
 
 Check dune-common for more details concerning dependencies, known bugs,
 license and installation.
 
 
-git-1b0e7e623bef2665fe0139670df809d403c61389
+git-927da16f4c0d665a2ceba923aecb36a04133656d
```

### Comparing `dune-istl-2.9.0rc1/cmake/modules/AddSuperLUFlags.cmake` & `dune-istl-2.9.dev20220529/cmake/modules/AddSuperLUFlags.cmake`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Defines the functions to use SuperLU
 #
 # .. cmake_function:: add_dune_superlu_flags
 #
 #    .. cmake_param:: targets
 #       :positional:
 #       :single:
```

### Comparing `dune-istl-2.9.0rc1/cmake/modules/FindARPACK.cmake` & `dune-istl-2.9.dev20220529/cmake/modules/FindARPACK.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    Module that checks whether ARPACK is available and usable.
 #
 #    Variables used by this module which you may want to set:
 #
 #    :ref:`ARPACK_ROOT`
```

### Comparing `dune-istl-2.9.0rc1/cmake/modules/FindARPACKPP.cmake` & `dune-istl-2.9.dev20220529/cmake/modules/FindARPACKPP.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    Module that checks whether ARPACK++ is available and usable.
 #
 #    Variables used by this module which you may want to set:
 #
 #    :ref:`ARPACKPP_ROOT`
```

### Comparing `dune-istl-2.9.0rc1/cmake/modules/FindSuperLU.cmake` & `dune-istl-2.9.dev20220529/cmake/modules/FindSuperLU.cmake`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    Module that checks whether SuperLU is available and usable.
 #
 #    Sets the following variables:
 #
 #    :code:`SuperLU_FOUND`
```

### Comparing `dune-istl-2.9.0rc1/config.h.cmake` & `dune-istl-2.9.dev20220529/config.h.cmake`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /* begin dune-istl
    put the definitions for config.h specific to
    your project here. Everything above will be
    overwritten
 */
 
 /* begin private */
```

### Comparing `dune-istl-2.9.0rc1/doc/blockstructure.eps` & `dune-istl-2.9.dev20220529/doc/blockstructure.eps`

 * *Files identical despite different names*

### Comparing `dune-istl-2.9.0rc1/doc/doxygen/modules.txt` & `dune-istl-2.9.dev20220529/doc/doxygen/modules.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 /**
   @defgroup ISTL Iterative Solvers Template Library (ISTL)
 
    @brief Iterative Solvers supporting block recursive matrix and
    vector classes at compile time.
 
    The Iterative Solver Template Library applies generic programming
```

### Comparing `dune-istl-2.9.0rc1/doc/istl.bib` & `dune-istl-2.9.dev20220529/doc/istl.bib`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-@Comment SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-@Comment SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 @String{ap =     "Ann. der Physik"}
 @String{as =     "Acta Stereol."}
 @String{awr =    "Adv. Water Res."}
 @String{ces =    "Chem. Eng. Sci."}
 @String{mdbg =   "Mitteilgn. Dtsch. Bodenkundl. Gesellsch."}
 @String{pre =    "Phys. Rev. E"}
 @String{rg =     "Reviews of Geophysics"}
@@ -155,8 +152,8 @@
   volume = 	 {47},
   OPTnumber = 	 {},
   pages = 	 {137--151},
   OPTmonth = 	 {},
   OPTnote = 	 {},
   OPTannote = 	 {},
  publisher = {Springer-Verlag Wien}
-}
+}
```

### Comparing `dune-istl-2.9.0rc1/doc/istl.tex` & `dune-istl-2.9.dev20220529/doc/istl.tex`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-% SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 \documentclass[11pt]{article}
 \usepackage{multicol}
 \usepackage{amsmath}
 \usepackage{amsfonts}
 \usepackage{color}
 \usepackage{hyperref}
 \usepackage[dvips]{epsfig}
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/CMakeLists.txt` & `dune-istl-2.9.dev20220529/dune/istl/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_subdirectory("common")
 add_subdirectory("eigenvalue")
 add_subdirectory("paamg")
 add_subdirectory(test)
 
 #install headers
 install(FILES
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/allocator.hh` & `dune-istl-2.9.dev20220529/dune/istl/allocator.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ISTL_ALLOCATOR_HH
 #define DUNE_ISTL_ALLOCATOR_HH
 
 #include <memory>
 #include <type_traits>
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/basearray.hh` & `dune-istl-2.9.dev20220529/dune/istl/basearray.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_BASEARRAY_HH
 #define DUNE_ISTL_BASEARRAY_HH
 
 #include "assert.h"
 #include <cmath>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/bccsmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/bccsmatrix.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_BCCSMATRIX_HH
 #define DUNE_ISTL_BCCSMATRIX_HH
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/bccsmatrixinitializer.hh` & `dune-istl-2.9.dev20220529/dune/istl/bccsmatrixinitializer.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_BCCSMATRIX_INITIALIZER_HH
 #define DUNE_ISTL_BCCSMATRIX_INITIALIZER_HH
 
 #include <limits>
 #include <set>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/bcrsmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/bcrsmatrix.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_BCRSMATRIX_HH
 #define DUNE_ISTL_BCRSMATRIX_HH
 
 #include <cmath>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/bdmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/bdmatrix.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_BDMATRIX_HH
 #define DUNE_ISTL_BDMATRIX_HH
 
 #include <memory>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/blocklevel.hh` & `dune-istl-2.9.dev20220529/dune/istl/blocklevel.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_BLOCKLEVEL_HH
 #define DUNE_ISTL_BLOCKLEVEL_HH
 
 #include <algorithm>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/btdmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/btdmatrix.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_BTDMATRIX_HH
 #define DUNE_ISTL_BTDMATRIX_HH
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/scalarvectorview.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/bvector.hh` & `dune-istl-2.9.dev20220529/dune/istl/bvector.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_BVECTOR_HH
 #define DUNE_ISTL_BVECTOR_HH
 
 #include <algorithm>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/cholmod.hh` & `dune-istl-2.9.dev20220529/dune/istl/cholmod.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #pragma once
 
 #if HAVE_SUITESPARSE_CHOLMOD
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
 #include <dune/istl/bcrsmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/common/counter.hh` & `dune-istl-2.9.dev20220529/dune/istl/common/counter.hh`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ISTL_COMMON_COUNTER_HH
 #define DUNE_ISTL_COMMON_COUNTER_HH
 
 #include <cassert>
 #include <typeinfo>
 #include <iostream>
 #include <memory>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/common/registry.hh` & `dune-istl-2.9.dev20220529/dune/istl/common/registry.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ISTL_COMMON_REGISTRY_HH
 #define DUNE_ISTL_COMMON_REGISTRY_HH
 
 #include <cstddef>
 #include <iostream>
 #include <memory>
 #include <string>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/eigenvalue/arpackpp.hh` & `dune-istl-2.9.dev20220529/dune/istl/eigenvalue/arpackpp.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_EIGENVALUE_ARPACKPP_HH
 #define DUNE_ISTL_EIGENVALUE_ARPACKPP_HH
 
 #if HAVE_ARPACKPP || defined DOXYGEN
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/eigenvalue/poweriteration.hh` & `dune-istl-2.9.dev20220529/dune/istl/eigenvalue/poweriteration.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_EIGENVALUE_POWERITERATION_HH
 #define DUNE_ISTL_EIGENVALUE_POWERITERATION_HH
 
 #include <cstddef>  // provides std::size_t
 #include <cmath>    // provides std::sqrt, std::abs
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/eigenvalue/test/cond2test.cc` & `dune-istl-2.9.dev20220529/dune/istl/eigenvalue/test/cond2test.cc`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/timer.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/eigenvalue/test/matrixinfo.hh` & `dune-istl-2.9.dev20220529/dune/istl/eigenvalue/test/matrixinfo.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_EIGENVALUE_TEST_MATRIXINFO_HH
 #define DUNE_ISTL_EIGENVALUE_TEST_MATRIXINFO_HH
 
 #include <cmath>    // provides std::abs and std::sqrt
 #include <cassert>  // provides assert
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/foreach.hh` & `dune-istl-2.9.dev20220529/dune/istl/foreach.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #pragma once
 
 #include<type_traits>
 #include<utility>
 #include<cassert>
 
 #include<dune/common/std/type_traits.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/gsetc.hh` & `dune-istl-2.9.dev20220529/dune/istl/gsetc.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_GSETC_HH
 #define DUNE_ISTL_GSETC_HH
 
 #include <cmath>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/ildl.hh` & `dune-istl-2.9.dev20220529/dune/istl/ildl.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_ISTL_ILDL_HH
 #define DUNE_ISTL_ILDL_HH
 
 #include <dune/common/scalarvectorview.hh>
 #include <dune/common/scalarmatrixview.hh>
 #include "ilu.hh"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/ilu.hh` & `dune-istl-2.9.dev20220529/dune/istl/ilu.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_ILU_HH
 #define DUNE_ISTL_ILU_HH
 
 #include <cmath>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/ilusubdomainsolver.hh` & `dune-istl-2.9.dev20220529/dune/istl/ilusubdomainsolver.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_ILUSUBDOMAINSOLVER_HH
 #define DUNE_ISTL_ILUSUBDOMAINSOLVER_HH
 
 #include <map>
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/io.hh` & `dune-istl-2.9.dev20220529/dune/istl/io.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_IO_HH
 #define DUNE_ISTL_IO_HH
 
 #include <cmath>
 #include <complex>
@@ -588,38 +586,35 @@
                             {x_off, y_off, block_size, block_size});
         });
         col_offset += cols * (block_size + interspace);
         row_offset += rows * (block_size + interspace);
       } else {
         // before we write anything, we need to calculate the
         // offset for every {row,col} index
-        const auto null_offset = std::numeric_limits<std::size_t>::max();
-        std::vector<std::size_t> col_offsets(cols + 1, null_offset);
-        std::vector<std::size_t> row_offsets(rows + 1, null_offset);
+        std::vector<std::size_t> col_offsets(cols + 1, 0);
+        std::vector<std::size_t> row_offsets(rows + 1, 0);
         for_each_entry([&](const auto &row, const auto &col, const auto &val) {
           NullStream dev0;
           // get size of sub-block
           auto sub_size =
               writeSVGMatrix(val, dev0, opts, row_prefix, col_prefix);
 
           // if we didn't see col size before
-          if (col_offsets[col + 1] == null_offset) // write it in the offset vector
+          if (col_offsets[col + 1] == 0) // write it in the offset vector
             col_offsets[col + 1] = sub_size.first;
+          else // check that is the same we saw before
+            assert(col_offsets[col + 1] == sub_size.first);
 
           // repeat proces for row sizes
-          if (row_offsets[row + 1] == null_offset)
+          if (row_offsets[row + 1] == 0)
             row_offsets[row + 1] = sub_size.second;
+          else
+            assert(row_offsets[row + 1] == sub_size.second);
         });
 
-        // if some rows/cols were not visited, make an educated guess with the minimum offset
-        auto min_row_offset = *std::min_element(begin(row_offsets), end(row_offsets));
-        std::replace(begin(row_offsets), end(row_offsets), null_offset, min_row_offset);
-        auto min_col_offset = *std::min_element(begin(col_offsets), end(col_offsets));
-        std::replace(begin(col_offsets), end(col_offsets), null_offset, min_col_offset);
-
         // we have sizes for every block: to get offsets we make a partial sum
         col_offsets[0] = interspace;
         row_offsets[0] = interspace;
         for (std::size_t i = 1; i < col_offsets.size(); i++)
           col_offsets[i] += col_offsets[i - 1] + interspace;
         for (std::size_t i = 1; i < row_offsets.size(); i++)
           row_offsets[i] += row_offsets[i - 1] + interspace;
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/istlexception.hh` & `dune-istl-2.9.dev20220529/dune/istl/istlexception.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_ISTLEXCEPTION_HH
 #define DUNE_ISTL_ISTLEXCEPTION_HH
 
 #include <dune/common/exceptions.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/ldl.hh` & `dune-istl-2.9.dev20220529/dune/istl/ldl.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_LDL_HH
 #define DUNE_ISTL_LDL_HH
 
 #if HAVE_SUITESPARSE_LDL || defined DOXYGEN
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/matrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/matrix.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MATRIX_HH
 #define DUNE_ISTL_MATRIX_HH
 
 /** \file
     \brief A dynamic dense block matrix class
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/matrixindexset.hh` & `dune-istl-2.9.dev20220529/dune/istl/matrixindexset.hh`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MATRIXINDEXSET_HH
 #define DUNE_ISTL_MATRIXINDEXSET_HH
 
 #include <vector>
 #include <set>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/matrixmarket.hh` & `dune-istl-2.9.dev20220529/dune/istl/matrixmarket.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MATRIXMARKET_HH
 #define DUNE_ISTL_MATRIXMARKET_HH
 
 #include <algorithm>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/matrixmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/matrixmatrix.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MATRIXMATRIX_HH
 #define DUNE_ISTL_MATRIXMATRIX_HH
 
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/matrixredistribute.hh` & `dune-istl-2.9.dev20220529/dune/istl/matrixredistribute.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MATRIXREDISTRIBUTE_HH
 #define DUNE_ISTL_MATRIXREDISTRIBUTE_HH
 #include <memory>
 #include "repartition.hh"
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/matrixutils.hh` & `dune-istl-2.9.dev20220529/dune/istl/matrixutils.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MATRIXUTILS_HH
 #define DUNE_ISTL_MATRIXUTILS_HH
 
 #include <set>
 #include <vector>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/multitypeblockmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/multitypeblockmatrix.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MULTITYPEBLOCKMATRIX_HH
 #define DUNE_ISTL_MULTITYPEBLOCKMATRIX_HH
 
 #include <cmath>
 #include <iostream>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/multitypeblockvector.hh` & `dune-istl-2.9.dev20220529/dune/istl/multitypeblockvector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_MULTITYPEBLOCKVECTOR_HH
 #define DUNE_ISTL_MULTITYPEBLOCKVECTOR_HH
 
 #include <cmath>
 #include <iostream>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/novlpschwarz.hh` & `dune-istl-2.9.dev20220529/dune/istl/novlpschwarz.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_NOVLPSCHWARZ_HH
 #define DUNE_ISTL_NOVLPSCHWARZ_HH
 
 #include <iostream>              // for input/output to shell
 #include <fstream>               // for input/output to files
@@ -43,14 +41,17 @@
    *
    * The \ref ISTL_Solvers "solvers" can easily be turned into parallel solvers
    * initializing them with matching parallel subclasses of the base classes
    * ScalarProduct, Preconditioner and LinearOperator.
    *
    * The information of the data distribution is provided by OwnerOverlapCopyCommunication
    * of \ref ISTL_Comm "communication API".
+   *
+   * Currently only data parallel versions are shipped with dune-istl. Domain
+   * decomposition can be found in module dune-dd.
    */
   /**
      @addtogroup ISTL_Operators
      @{
    */
 
   /**
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/operators.hh` & `dune-istl-2.9.dev20220529/dune/istl/operators.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_OPERATORS_HH
 #define DUNE_ISTL_OPERATORS_HH
 
 #include <cmath>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/overlappingschwarz.hh` & `dune-istl-2.9.dev20220529/dune/istl/overlappingschwarz.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_OVERLAPPINGSCHWARZ_HH
 #define DUNE_ISTL_OVERLAPPINGSCHWARZ_HH
 #include <cassert>
 #include <algorithm>
 #include <functional>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/owneroverlapcopy.hh` & `dune-istl-2.9.dev20220529/dune/istl/owneroverlapcopy.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_OWNEROVERLAPCOPY_HH
 #define DUNE_ISTL_OWNEROVERLAPCOPY_HH
 
 #include <new>
 #include <iostream>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/aggregates.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/aggregates.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_AGGREGATES_HH
 #define DUNE_AMG_AGGREGATES_HH
 
 
 #include "parameters.hh"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/amg.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/amg.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_AMG_HH
 #define DUNE_AMG_AMG_HH
 
 #include <memory>
 #include <sstream>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/combinedfunctor.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/combinedfunctor.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_COMBINEDFUNCTOR_HH
 #define DUNE_AMG_COMBINEDFUNCTOR_HH
 
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/construction.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/construction.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMGCONSTRUCTION_HH
 #define DUNE_AMGCONSTRUCTION_HH
 
 #include <dune/istl/bvector.hh>
 #include <dune/istl/operators.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/dependency.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/dependency.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_DEPENDENCY_HH
 #define DUNE_AMG_DEPENDENCY_HH
 
 
 #include <bitset>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/fastamg.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/fastamg.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_FASTAMG_HH
 #define DUNE_ISTL_FASTAMG_HH
 
 #include <memory>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/fastamgsmoother.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/fastamgsmoother.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_FASTAMGSMOOTHER_HH
 #define DUNE_ISTL_FASTAMGSMOOTHER_HH
 
 #include <cstddef>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/galerkin.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/galerkin.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GALERKIN_HH
 #define DUNE_GALERKIN_HH
 
 #include "aggregates.hh"
 #include "pinfo.hh"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/globalaggregates.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/globalaggregates.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GLOBALAGGREGATES_HH
 #define DUNE_GLOBALAGGREGATES_HH
 
 /**
  * @addtogroup ISTL_PAAMG
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/graph.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/graph.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_GRAPH_HH
 #define DUNE_AMG_GRAPH_HH
 
 #include <cstddef>
 #include <algorithm>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/graphcreator.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/graphcreator.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_GRAPHCREATOR_HH
 #define DUNE_AMG_GRAPHCREATOR_HH
 
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/hierarchy.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/hierarchy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMGHIERARCHY_HH
 #define DUNE_AMGHIERARCHY_HH
 
 #include <list>
 #include <memory>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/indicescoarsener.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/indicescoarsener.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_INDICESCOARSENER_HH
 #define DUNE_AMG_INDICESCOARSENER_HH
 
 #include <dune/common/parallel/indicessyncer.hh>
 #include <vector>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/kamg.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/kamg.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_KAMG_HH
 #define DUNE_AMG_KAMG_HH
 
 #include <dune/istl/preconditioners.hh>
 #include "amg.hh"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/matrixhierarchy.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/matrixhierarchy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_MATRIXHIERARCHY_HH
 #define DUNE_AMG_MATRIXHIERARCHY_HH
 
 #include <algorithm>
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/parameters.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/parameters.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_PARAMETERS_HH
 #define DUNE_AMG_PARAMETERS_HH
 
 #include <cstddef>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/pinfo.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/pinfo.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_PINFO_HH
 #define DUNE_AMG_PINFO_HH
 
 #include <dune/common/parallel/communication.hh>
 #include <dune/common/enumset.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/properties.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/properties.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_AMG_PROPERTIES_HH
 #define DUNE_ISTL_AMG_PROPERTIES_HH
 
 #include <dune/common/propertymap.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/renumberer.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/renumberer.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMG_RENUMBERER_HH
 #define DUNE_AMG_RENUMBERER_HH
 
 #include "aggregates.hh"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/smoother.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/smoother.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMGSMOOTHER_HH
 #define DUNE_AMGSMOOTHER_HH
 
 #include <dune/istl/paamg/construction.hh>
 #include <dune/istl/paamg/aggregates.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/CMakeLists.txt` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 find_package(Threads)
 if(CMAKE_USE_PTHREADS_INIT)
   dune_add_test(NAME pthreadamgtest SOURCES pthreadamgtest.cc
     LINK_LIBRARIES ${CMAKE_THREAD_LIBS_INIT}
     COMPILE_DEFINITIONS MYAMG=Dune::Amg::AMG<Operator,Vector,Smoother>)
   add_dune_mpi_flags(pthreadamgtest)
   add_dune_parmetis_flags(pthreadamgtest)
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/amgtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/amgtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 /*#include"xreal.h"
 
    namespace std
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/anisotropic.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/anisotropic.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef ANISOTROPIC_HH
 #define  ANISOTROPIC_HH
 #include <dune/common/fmatrix.hh>
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/plocalindex.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/fastamg.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/fastamg.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include "anisotropic.hh"
 #include <dune/common/timer.hh>
 #include <dune/common/parallel/indexset.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/galerkintest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/galerkintest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <iostream>
 #include <tuple>
 #include <dune/common/enumset.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/gr_30_30.mm` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/gr_30_30.mm`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 %%MatrixMarket matrix coordinate real symmetric
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 900 900 4322
 1 1  8.0000000000000e+00
 2 1 -1.0000000000000e+00
 31 1 -1.0000000000000e+00
 32 1 -1.0000000000000e+00
 2 2  8.0000000000000e+00
 3 2 -1.0000000000000e+00
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/graphtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/graphtest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 // start with including some headers
 #include "config.h"
 #include <iostream>               // for input/output to shell
 
 #include <dune/istl/paamg/graph.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/hierarchytest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/hierarchytest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/parallel/mpicommunication.hh>
 #include <dune/istl/paamg/matrixhierarchy.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/kamgtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/kamgtest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include "anisotropic.hh"
 #include <dune/common/timer.hh>
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/communication.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/pamgmmtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/pamgmmtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <memory>
 #include <dune/common/parallel/mpihelper.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/parallelamgtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/parallelamgtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #ifdef TEST_AGGLO
 #define UNKNOWNS 10
 #endif
 #include "anisotropic.hh"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/pthreadamgtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/pthreadamgtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 /*#include"xreal.h"
 
    namespace std
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/pthreadtwoleveltest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/pthreadtwoleveltest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include"config.h"
 #include "anisotropic.hh"
 #include <dune/common/timer.hh>
 #include <dune/common/shared_ptr.hh>
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/communication.hh>
 #include <dune/istl/paamg/twolevelmethod.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/transfertest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/transfertest.cc`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/bvector.hh>
 #include <dune/common/fvector.hh>
 #include <dune/istl/paamg/aggregates.hh>
 #include <dune/istl/paamg/pinfo.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/test/twolevelmethodtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/paamg/test/twolevelmethodtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include"config.h"
 #include "anisotropic.hh"
 #include <dune/common/timer.hh>
 #include <dune/common/shared_ptr.hh>
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/communication.hh>
 #include <dune/istl/paamg/twolevelmethod.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/transfer.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/transfer.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_AMGTRANSFER_HH
 #define DUNE_AMGTRANSFER_HH
 
 #include <dune/istl/bvector.hh>
 #include <dune/istl/matrixredistribute.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/paamg/twolevelmethod.hh` & `dune-istl-2.9.dev20220529/dune/istl/paamg/twolevelmethod.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_TWOLEVELMETHOD_HH
 #define DUNE_ISTL_TWOLEVELMETHOD_HH
 
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/preconditioner.hh` & `dune-istl-2.9.dev20220529/dune/istl/preconditioner.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_PRECONDITIONER_HH
 #define DUNE_ISTL_PRECONDITIONER_HH
 
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/preconditioners.hh` & `dune-istl-2.9.dev20220529/dune/istl/preconditioners.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_PRECONDITIONERS_HH
 #define DUNE_ISTL_PRECONDITIONERS_HH
 
 #include <cmath>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/repartition.hh` & `dune-istl-2.9.dev20220529/dune/istl/repartition.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_REPARTITION_HH
 #define DUNE_ISTL_REPARTITION_HH
 
 #include <cassert>
 #include <map>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/scalarproducts.hh` & `dune-istl-2.9.dev20220529/dune/istl/scalarproducts.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SCALARPRODUCTS_HH
 #define DUNE_ISTL_SCALARPRODUCTS_HH
 
 #include <cmath>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/scaledidmatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/scaledidmatrix.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SCALEDIDMATRIX_HH
 #define DUNE_ISTL_SCALEDIDMATRIX_HH
 
 /*! \file
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/schwarz.hh` & `dune-istl-2.9.dev20220529/dune/istl/schwarz.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SCHWARZ_HH
 #define DUNE_ISTL_SCHWARZ_HH
 
 #include <iostream>              // for input/output to shell
 #include <fstream>               // for input/output to files
@@ -41,14 +39,17 @@
    *
    * The \ref ISTL_Solvers "solvers" can easily be turned into parallel solvers
    * initializing them with matching parallel subclasses of the base classes
    * ScalarProduct, Preconditioner and LinearOperator.
    *
    * The information of the data distribution is provided by OwnerOverlapCopyCommunication
    * of \ref ISTL_Comm "communication API".
+   *
+   * Currently only data parallel versions are shipped with dune-istl. Domain
+   * decomposition can be found in module dune-dd.
    */
   /**
      @addtogroup ISTL_Operators
      @{
    */
 
   /**
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/solver.hh` & `dune-istl-2.9.dev20220529/dune/istl/solver.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_SOLVER_HH
 #define DUNE_ISTL_SOLVER_HH
 
 #include <iomanip>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/solvercategory.hh` & `dune-istl-2.9.dev20220529/dune/istl/solvercategory.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SOLVERCATEGORY_HH
 #define DUNE_ISTL_SOLVERCATEGORY_HH
 
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/solverfactory.hh` & `dune-istl-2.9.dev20220529/dune/istl/solverfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_SOLVERFACTORY_HH
 #define DUNE_ISTL_SOLVERFACTORY_HH
 
 #include <unordered_map>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/solverregistry.hh` & `dune-istl-2.9.dev20220529/dune/istl/solverregistry.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_SOLVERREGISTRY_HH
 #define DUNE_ISTL_SOLVERREGISTRY_HH
 
 #include <dune/istl/common/registry.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/solvers.hh` & `dune-istl-2.9.dev20220529/dune/istl/solvers.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_SOLVERS_HH
 #define DUNE_ISTL_SOLVERS_HH
 
 #include <array>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/spqr.hh` & `dune-istl-2.9.dev20220529/dune/istl/spqr.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SPQR_HH
 #define DUNE_ISTL_SPQR_HH
 
 #if HAVE_SUITESPARSE_SPQR || defined DOXYGEN
 
@@ -282,33 +280,28 @@
     friend class SeqOverlappingSchwarz;
 
     friend struct SeqOverlappingSchwarzAssemblerHelper<SPQR<Matrix>,true>;
 
     /** @brief Computes the QR decomposition. */
     void decompose()
     {
-      const std::size_t nrows(spqrMatrix_.N());
-      const std::size_t ncols(spqrMatrix_.M());
-      const std::size_t nnz(spqrMatrix_.getColStart()[ncols]);
-
+      const std::size_t dimMat(spqrMatrix_.N());
+      const std::size_t nnz(spqrMatrix_.getColStart()[dimMat]);
       // initialise the matrix A (sorted, packed, unsymmetric, real entries)
-      A_ = cholmod_l_allocate_sparse(nrows, ncols, nnz, 1, 1, 0, 1, cc_);
-
+      A_ = cholmod_l_allocate_sparse(dimMat, dimMat, nnz, 1, 1, 0, 1, cc_);
       // copy all the entries of Ap, Ai, Ax
-      for(std::size_t k = 0; k != (ncols+1); ++k)
+      for(std::size_t k = 0; k != (dimMat+1); ++k)
         (static_cast<long int *>(A_->p))[k] = spqrMatrix_.getColStart()[k];
-
       for(std::size_t k = 0; k != nnz; ++k)
       {
         (static_cast<long int*>(A_->i))[k] = spqrMatrix_.getRowIndex()[k];
         (static_cast<T*>(A_->x))[k] = spqrMatrix_.getValues()[k];
       }
-
       // initialise the vector B
-      B_ = cholmod_l_allocate_dense(nrows, 1, nrows, A_->xtype, cc_);
+      B_ = cholmod_l_allocate_dense(dimMat, 1, dimMat, A_->xtype, cc_);
       // compute factorization of A
       spqrfactorization_=SuiteSparseQR_factorize<T>(SPQR_ORDERING_DEFAULT,SPQR_DEFAULT_TOL,A_,cc_);
     }
 
     SPQRMatrix spqrMatrix_;
     bool matrixIsLoaded_;
     int verbose_;
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/superlu.hh` & `dune-istl-2.9.dev20220529/dune/istl/superlu.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SUPERLU_HH
 #define DUNE_ISTL_SUPERLU_HH
 
 #if HAVE_SUPERLU
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/superlufunctions.hh` & `dune-istl-2.9.dev20220529/dune/istl/superlufunctions.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SUPERLUFUNCTIONS_HH
 #define DUNE_ISTL_SUPERLUFUNCTIONS_HH
 #if HAVE_SUPERLU
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/supermatrix.hh` & `dune-istl-2.9.dev20220529/dune/istl/supermatrix.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_SUPERMATRIX_HH
 #define DUNE_ISTL_SUPERMATRIX_HH
 
 #if HAVE_SUPERLU
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/CMakeLists.txt` & `dune-istl-2.9.dev20220529/dune/istl/test/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # install the test tools as we want to support testing 3rd-party vectors and matrices with an installed dune-istl
 install(FILES
         matrixtest.hh
         vectortest.hh
         laplacian.hh
         multirhstest.hh
         DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/dune/istl/test)
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/bcrsbuild.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/bcrsbuild.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/bcrsmatrix.hh>
 #include <dune/common/fmatrix.hh>
 #include <dune/common/exceptions.hh>
 #include <dune/common/test/testsuite.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/bcrsimplicitbuild.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/bcrsimplicitbuild.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include "config.h"
 
 #undef NDEBUG // make sure assert works
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/bcrsmatrixtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/bcrsmatrixtest.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/float_cmp.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/bcrsnormtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/bcrsnormtest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <complex>
 #include <memory>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/istl/bcrsmatrix.hh>
 
 template <class V>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/blocklevel.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/blocklevel.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /**
  * \file
  * \brief Test block level function
  */
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/bvectortest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/bvectortest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 // hack to ensure assert() does something
 // really, assert() should not be used in unit tests.
 #ifdef NDEBUG
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/cgconditiontest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/cgconditiontest.cc`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <dune/istl/preconditioners.hh>
 #include <dune/istl/solvers.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/cholmodtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/cholmodtest.cc`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/complexdata.hh` & `dune-istl-2.9.dev20220529/dune/istl/test/complexdata.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 /**
  * \author: Marian Piatkowski, Steffen Müthing
  * \file
  * \brief Test data for complexmatrixtest.
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/complexmatrixtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/complexmatrixtest.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /**
  * \author: Marian Piatkowski, Steffen Müthing
  * \file
  * \brief Test MINRES and GMRes for complex matrices and complex rhs.
  */
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/complexrhstest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/complexrhstest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /**
  * \author: Matthias Wohlmuth
  * \file
  * \brief Test different solvers and preconditioners for
  *        \f$A*x = b\f$ with \f$A\f$ being a \f$N^2 \times N^2\f$
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/dotproducttest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/dotproducttest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/bvector.hh>
 #include <dune/istl/vbvector.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/classname.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/fieldvectortest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/fieldvectortest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 /** \file
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/foreachtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/foreachtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/common/bitsetvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/iluildltest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/iluildltest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <iostream>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/inverseoperator2prectest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/inverseoperator2prectest.cc`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include<dune/istl/bvector.hh>
 #include<dune/istl/superlu.hh>
 #include<dune/istl/preconditioners.hh>
 #include<dune/istl/solvers.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/iotest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/iotest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/common/fmatrix.hh>
 #include <dune/common/diagonalmatrix.hh>
 #include <dune/istl/scaledidmatrix.hh>
 #include <dune/istl/bcrsmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/ldltest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/ldltest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <iostream>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/timer.hh>
 #include <dune/istl/bvector.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/matrixmarkettest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/matrixmarkettest.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <iterator>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/matrixnormtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/matrixnormtest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <complex>
 #include <memory>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/classname.hh>
 #include <dune/istl/matrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/matrixredisttest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/matrixredisttest.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #define DEBUG_REPART
 
 #include <dune/istl/matrixredistribute.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/matrixtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/matrixtest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
     \brief Unit tests for the different dynamic matrices provided by ISTL
  */
 #include "config.h"
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/matrixtest.hh` & `dune-istl-2.9.dev20220529/dune/istl/test/matrixtest.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_TEST_MATRIXTEST_HH
 #define DUNE_ISTL_TEST_MATRIXTEST_HH
 
 /** \file
  * \brief Infrastructure for testing the dune-istl matrix interface
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/matrixutilstest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/matrixutilstest.cc`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/matrixutils.hh>
 #include <dune/istl/bcrsmatrix.hh>
 #include <dune/common/fmatrix.hh>
 #include <dune/common/stdstreams.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/multirhstest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/multirhstest.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 // start with including some headers
 #include "config.h"
 
 #define DISABLE_AMG_DIRECTSOLVER 1
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/multirhstest.hh` & `dune-istl-2.9.dev20220529/dune/istl/test/multirhstest.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ISTL_TEST_MULTIRHSTEST_HH
 #define DUNE_ISTL_TEST_MULTIRHSTEST_HH
 
 #define DISABLE_AMG_DIRECTSOLVER 1
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/multitypeblockmatrixtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/multitypeblockmatrixtest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /**
  * \file
  * \brief Test the MultiTypeBlockMatrix data structure
  */
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/multitypeblockvectortest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/multitypeblockvectortest.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /**
  * \file
  * \brief Test the MultiTypeBlockVector data structure
  */
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/mv.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/mv.cc`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/bvector.hh>
 #include <dune/istl/operators.hh>
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/overlappingschwarztest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/overlappingschwarztest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/istl/io.hh>
 #include <dune/istl/bvector.hh>
 #include <dune/istl/operators.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/preconditionerstest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/preconditionerstest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 /** \file \brief Test the preconditioners in the file `preconditioners.hh`
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/registrytest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/registrytest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #if HAVE_CONFIG_H
 #include <config.h>
 #endif
 
 #include <cassert>
 
 #ifndef DISABLE_CXA_DEMANGLE
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/scalarproductstest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/scalarproductstest.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <dune/common/fvector.hh>
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/test/testsuite.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/scaledidmatrixtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/scaledidmatrixtest.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 // include this first to see whether it includes all necessary headers itself
 #include <dune/istl/scaledidmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/solveraborttest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/solveraborttest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include "config.h"
 
 #include <iostream>
 #include <limits>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/solverfactorytest.cc.in` & `dune-istl-2.9.dev20220529/dune/istl/test/solverfactorytest.cc.in`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 // If we test with simd we need to deactivate the direct solver.
 // In that case we use a define to do this in the next line.
 @DEFINE_DEACTIVATE_AMG_DIRECTSOLVER@
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/solverfactorytest.ini` & `dune-istl-2.9.dev20220529/dune/istl/test/solverfactorytest.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 [sequential]
 N = 20
 
 [sequential.CGWithRichardson]
 type = cgsolver
 verbose = 1
 maxit = 1000
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/solvertest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/solvertest.cc`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/io.hh>
 #include <dune/istl/bvector.hh>
 #include <dune/istl/operators.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/spqrtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/spqrtest.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 #include <complex>
 #include <iostream>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/timer.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/superlutest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/superlutest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <complex>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/umfpacktest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/umfpacktest.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <iostream>
 
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/vbvectortest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/vbvectortest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/istl/vbvector.hh>
 #include <dune/common/fvector.hh>
 #include <dune/common/typetraits.hh>
 #include <dune/common/test/testsuite.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/vectorcommtest.cc` & `dune-istl-2.9.dev20220529/dune/istl/test/vectorcommtest.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <dune/common/parallel/indexset.hh>
 #include <dune/common/parallel/communicator.hh>
 #include <dune/common/parallel/remoteindices.hh>
 #include <vector>
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/test/vectortest.hh` & `dune-istl-2.9.dev20220529/dune/istl/test/vectortest.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_TEST_VECTORTEST_HH
 #define DUNE_ISTL_TEST_VECTORTEST_HH
 
 /** \file
  * \brief Infrastructure for testing the dune-istl vector interface
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/umfpack.hh` & `dune-istl-2.9.dev20220529/dune/istl/umfpack.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_UMFPACK_HH
 #define DUNE_ISTL_UMFPACK_HH
 
 #if HAVE_SUITESPARSE_UMFPACK || defined DOXYGEN
```

### Comparing `dune-istl-2.9.0rc1/dune/istl/vbvector.hh` & `dune-istl-2.9.dev20220529/dune/istl/vbvector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ISTL_VBVECTOR_HH
 #define DUNE_ISTL_VBVECTOR_HH
 
 #include <cmath>
 #include <complex>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/bcrsmatrix.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/bcrsmatrix.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_BCRSMATRIX_HH
 #define DUNE_PYTHON_ISTL_BCRSMATRIX_HH
 
 #include <memory>
 #include <stdexcept>
 #include <string>
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/bvector.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/bvector.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_BVECTOR_HH
 #define DUNE_PYTHON_ISTL_BVECTOR_HH
 
 #include <cstddef>
 
 #include <stdexcept>
 #include <string>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/iterator.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/iterator.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_ITERATOR_HH
 #define DUNE_PYTHON_ISTL_ITERATOR_HH
 
 #include <tuple>
 
 #include <dune/common/visibility.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/matrixindexset.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/matrixindexset.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_BCRSMATRIX_HH
 #define DUNE_PYTHON_ISTL_BCRSMATRIX_HH
 
 #include <memory>
 #include <stdexcept>
 #include <string>
 #include <tuple>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/preconditioners.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/preconditioners.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_PRECONDITIONER_HH
 #define DUNE_PYTHON_ISTL_PRECONDITIONER_HH
 
 #include <dune/common/typeutilities.hh>
 #include <dune/common/version.hh>
 
 #include <dune/istl/operators.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/slice.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/slice.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_SLICE_HH
 #define DUNE_PYTHON_ISTL_SLICE_HH
 
 #include <cassert>
 
 #include <type_traits>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/istl/solvers.hh` & `dune-istl-2.9.dev20220529/dune/python/istl/solvers.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_ISTL_SOLVER_HH
 #define DUNE_PYTHON_ISTL_SOLVER_HH
 
 #include <dune/common/typeutilities.hh>
 #include <dune/common/version.hh>
 
 #include <dune/istl/solver.hh>
```

### Comparing `dune-istl-2.9.0rc1/dune/python/test/bcrsmatrix.py` & `dune-istl-2.9.dev20220529/dune/python/test/bcrsmatrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import dune.common
 from dune.istl import blockVector, BlockVector, bcrsMatrix, BCRSMatrix, SeqJacobi, CGSolver, BuildMode
 
 def identity(n, buildMode=BuildMode.random):
     if buildMode is BuildMode.random:
         mat = bcrsMatrix((n, n), n, BuildMode.random)
         for i in range(n):
```

### Comparing `dune-istl-2.9.0rc1/pyproject.toml` & `dune-istl-2.9.dev20220529/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # This is uses the `Python-Requires` field in the `dune.modules` file to
 # populate the `requires` entry. Additional packages needed for the package
 # build should be added in the `dune.modules`. These packages will then also be
 # included in the package install from source.
 #
 [build-system]
-requires = ['cmake>=3.13', 'dune-common<=v2.9.0rc1', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
+requires = ['cmake>=3.13', 'dune-common<=2.9.dev20220529', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
```

### Comparing `dune-istl-2.9.0rc1/python/dune/istl/__init__.py` & `dune-istl-2.9.dev20220529/python/dune/istl/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import dune.common
 
 from ._istl import BCRSMatrix as BCRSMatrix11
 from ._istl import BlockVector as BlockVector1
 from ._istl import *
 
 from dune.generator.generator import SimpleGenerator
```

### Comparing `dune-istl-2.9.0rc1/python/dune/istl/_istl.cc` & `dune-istl-2.9.dev20220529/python/dune/istl/_istl.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/common/fmatrix.hh>
 
 #include <dune/istl/bcrsmatrix.hh>
```

### Comparing `dune-istl-2.9.0rc1/python/dune_istl.egg-info/PKG-INFO` & `dune-istl-2.9.dev20220529/python/dune_istl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-istl
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Iterative solver template library which provides generic sparse matrix/vector classes and a variety of solvers based on these classes
 Home-page: https://gitlab.dune-project.org/core/dune-istl
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
@@ -33,15 +28,15 @@
         More information
         ----------------
         
         Check dune-common for more details concerning dependencies, known bugs,
         license and installation.
         
         
-        git-1b0e7e623bef2665fe0139670df809d403c61389
+        git-927da16f4c0d665a2ceba923aecb36a04133656d
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-istl-2.9.0rc1/python/dune_istl.egg-info/SOURCES.txt` & `dune-istl-2.9.dev20220529/python/dune_istl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 LICENSE.md
 README.md
 config.h.cmake
 dune-istl.pc.in
 dune.module
 pyproject.toml
 setup.py
-LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
 cmake/modules/AddARPACKPPFlags.cmake
 cmake/modules/AddSuperLUFlags.cmake
 cmake/modules/CMakeLists.txt
 cmake/modules/DuneIstlMacros.cmake
 cmake/modules/FindARPACK.cmake
 cmake/modules/FindARPACKPP.cmake
 cmake/modules/FindSuperLU.cmake
 doc/CMakeLists.txt
 doc/blockstructure.eps
-doc/blockstructure.eps.license
 doc/istl.bib
 doc/istl.tex
 doc/doxygen/CMakeLists.txt
 doc/doxygen/Doxylocal
 doc/doxygen/mainpage.txt
 doc/doxygen/modules.txt
 dune/CMakeLists.txt
@@ -185,15 +183,14 @@
 dune/python/istl/preconditioners.hh
 dune/python/istl/slice.hh
 dune/python/istl/solvers.hh
 dune/python/test/CMakeLists.txt
 dune/python/test/bcrsmatrix.mm
 dune/python/test/bcrsmatrix.py
 dune/python/test/bcrsmatrix.txt
-dune/python/test/bcrsmatrix.txt.license
 python/CMakeLists.txt
 python/dune/CMakeLists.txt
 python/dune/istl/CMakeLists.txt
 python/dune/istl/__init__.py
 python/dune/istl/_istl.cc
 python/dune_istl.egg-info/PKG-INFO
 python/dune_istl.egg-info/SOURCES.txt
```

### Comparing `dune-istl-2.9.0rc1/src/istl-solver-playground.cc` & `dune-istl-2.9.dev20220529/src/istl-solver-playground.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 // Uncomment the following line if you want to use direct solvers, but have MPI installed on you system
 //#undef HAVE_MPI
```

### Comparing `dune-istl-2.9.0rc1/src/istl-solver-playground.hh` & `dune-istl-2.9.dev20220529/src/istl-solver-playground.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef BIN_SOLVE_MM_HH
 #define BIN_SOLVE_MM_HH
 
 #include <dune/common/parametertree.hh>
```

