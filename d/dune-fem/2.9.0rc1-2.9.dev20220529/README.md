# Comparing `tmp/dune-fem-2.9.0rc1.tar.gz` & `tmp/dune-fem-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-fem-2.9.0rc1.tar", last modified: Fri Oct 21 08:17:03 2022, max compression
+gzip compressed data, was "dune-fem-2.9.dev20220529.tar", last modified: Sun May 29 21:03:41 2022, max compression
```

## Comparing `dune-fem-2.9.0rc1.tar` & `dune-fem-2.9.dev20220529.tar`

### file list

```diff
@@ -1,1110 +1,1110 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.955973 dune-fem-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/AddPAPIFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/AddSIONlibFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/CommandLineHacks.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/CorrectWindowsPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     5082 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/DuneFemMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/DuneFempyMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FemShort.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FemTortureTests.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindAmgXSolver.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindPAPI.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    16964 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindPETSc.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindPThreads.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindPackageMultipass.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindSIONlib.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindViennaCL.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/FindXDR.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/ResolveCompilerPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/cmake/modules/UseModelCompiler.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/doxygen/modules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/doc/doxygen/pages/
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/doxygen/pages/docrules.page
--rw-r--r--   0 runner    (1001) docker     (121)     5917 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/doxygen/pages/main.page
--rw-r--r--   0 runner    (1001) docker     (121)     4980 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/doc/operator-concept.tex
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/common/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/bindguard.hh
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/coordinate.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/explicitfieldvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/fmatrixcol.hh
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/forloop.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6143 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/geometrytypemap.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6039 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/hybrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/intersectionside.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/localcontribution.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/memory.hh
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/referencevector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/stackallocator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/common/test/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/test/test-hybrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7363 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/tupletypetraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10566 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/tupleutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/typeindexedtuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/common/utility.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/function/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/function/adaptivefunction/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/adaptivefunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7378 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/adaptivefunction/adaptivefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/adaptivefunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/function/blockvectordiscretefunction/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectordiscretefunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectordiscretefunction/blockvectordiscretefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectordiscretefunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.963974 dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7297 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction/blockvectorfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/blockvectors/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectors/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    22676 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectors/defaultblockvectors.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/blockvectors/referenceblockvector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/combinedfunction/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/combinedfunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18053 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/combinedfunction/combinedfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/combinedfunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/common/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/common.hh
--rw-r--r--   0 runner    (1001) docker     (121)    41635 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/discretefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14727 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/discretefunction_inline.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/dofblock.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7804 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/dofiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/function.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/functionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/functor.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23009 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/gridfunctionadapter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6596 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/instationary.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9267 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/localcontribution.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26218 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/localfunctionadapter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/rangegenerators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/common/scalarproducts.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/hierarchical/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11993 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/hierarchical/dofvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/hierarchical/function.hh
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/hierarchical.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/localfunction/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5487 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/average.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/bindable.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25604 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/const.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8627 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/converter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19881 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/localfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5322 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/localfunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/localfunctionsetadapter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/mutable.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9527 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/localfunction/temporary.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/petscdiscretefunction/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/petscdiscretefunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12306 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/petscdiscretefunction/petscdiscretefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/petscdiscretefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/subfunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/test/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/1dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6745 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/test-df.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/test-filtered-df.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/test-hierarchicalfunction-comm.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3155 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/test-hierarchicalfunction.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/test-lfa.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5948 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/test/test-tuplediscretefunction.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/discretefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/dofvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/functor.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/scalarproducts.hh
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.967974 dune-fem-2.9.0rc1/dune/fem/function/vectorfunction/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/vectorfunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/vectorfunction/managedvectorfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/vectorfunction/vectorfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/function/vectorfunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.971974 dune-fem-2.9.0rc1/dune/fem/gridpart/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19595 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/adaptiveleafgridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)    50309 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/adaptiveleafindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17378 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/codimindexset.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.971974 dune-fem-2.9.0rc1/dune/fem/gridpart/common/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/compositegeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5309 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/deaditerator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/defaultgridpartentity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4889 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/entitysearch.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/extendedentity.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17824 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridpart2gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridpartadapter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8138 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridview2gridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8631 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/localfunctiongeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/metatwistutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5684 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/persistentindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/policies.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/sharedgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/simplegeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/common/unimplementedgeometry.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.971974 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8367 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/basicfilterwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4943 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/domainfilter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/filter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/inversefilter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/radialfilter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4035 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/simple.hh
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/threadfilter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter/voidfilter.hh
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filter.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.971974 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2287 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3990 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14988 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.971974 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10580 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/cornerstorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6957 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5994 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12621 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6694 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7822 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13874 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4516 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8445 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4169 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11845 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/leafgridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/levelgridpart.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/gridpart/test/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/1dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4543 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkgridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8951 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkintersections.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/failure.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/test-gplagrangeinterpolation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12648 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/gridpart/test/test-gridpart.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/io/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/io/file/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/asciiparser.hh
--rw-r--r--   0 runner    (1001) docker     (121)    35314 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/dataoutput.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25975 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/datawriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21392 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/iointerface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/iolock.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15918 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/iotuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11214 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/latextablewriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17010 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/persistencemanager.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/io/file/test/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/backuprestore.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10524 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/dataoutputtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/test/persistencemanagertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    19435 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/file/vtkio.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/io.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/io.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.975973 dune-fem-2.9.0rc1/dune/fem/io/parameter/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20524 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter/container.hh
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter/parametertree.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter/parser.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11090 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter/reader.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29150 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/parameter.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/io/streams/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8186 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/asciistreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/binarystreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10823 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/sionlibstreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8281 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/standardstreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12190 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/streams.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/streams_inline.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/io/streams/test/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6193 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/test/test-streams.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/tuples.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9105 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/virtualstreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/streams/xdrstreams.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/io/test/
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       76 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/bc.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       77 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/date.sh
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/param_DarcyStokes
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/param_NavierStokes
--rw-r--r--   0 runner    (1001) docker     (121)     2503 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/parameterdicttest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/parametertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/test/testparameterfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/io/visual/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/converttemplate.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/dataconvert.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3748 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/datadisp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/errordisplay.hh
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/grcommon.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/printhelp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/programtemplate.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9871 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/readioparams.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/readiotupledata.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3495 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/readtupledata.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.979974 dune-fem-2.9.0rc1/dune/fem/marking/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/marking/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/marking/default.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12635 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/marking/doerfler.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/marking/localerror.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/marking/maximum.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15075 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/alugridwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/bartonnackmaninterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9058 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/boundaryidprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5207 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9161 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/checkgeomaffinity.hh
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/compatibility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/debug.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/debugbreak.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16798 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/domainintegral.hh
--rw-r--r--   0 runner    (1001) docker     (121)    27163 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/double.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26035 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/femeoc.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23850 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/femeoctable.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/femtimer.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13600 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/femtimer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/fieldmatrixhelper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/flops.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12152 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/fmatrixconverter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/functor.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/griddeclaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/gridfunctionview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/gridname.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/gridobjectstreams.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10966 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/gridsolution.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/gridwidth.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7590 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/h1norm.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8171 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/l1norm.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12999 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/l2norm.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8421 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/linesegmentsampler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14883 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/lpnorm.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/mapgeomtype.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/metaprogramming.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18168 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/mpimanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/nonconformitylevel.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/misc/petsc/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/petsc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20031 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/petsc/petsccommon.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10379 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/petsc/petscdofblock.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20752 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/petsc/petscvector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/misc/threads/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9745 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/domainthreaditerator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/threaditerator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3765 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/threaditeratorstorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/threadmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8660 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/threadpartitioner.hh
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/threadpool.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/threads/threadsafevalue.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5571 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/misc/umfpack.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/operator/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/operator/1order/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/1order/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    36862 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/1order/localmassmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/operator/common/
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/automaticdifferenceoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/differentiableoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12503 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/localcontribution.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19578 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/localmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/localmatrixcolumn.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7428 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/localmatrixwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16682 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/localoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13641 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/mapping.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/objpointer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8532 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/operator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8988 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/spaceoperatorif.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14812 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/stencil.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8359 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/temporarylocalmatrix.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.983974 dune-fem-2.9.0rc1/dune/fem/operator/common/test/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/test/mappingtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5137 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/common/tuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/dghelmholtz.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/linear/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14251 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/blockdiagonal.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/denserow.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/eigenoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13641 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/hierarchical.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6085 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/istladapter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/istloperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/numpyoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    37038 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/petscoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/spoperator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/linear/test/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10272 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/test/checklinearoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/test/test-hierarchicallinearoperator.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6180 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/linear/test/test-matrices.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/matrix/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7861 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/blockmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5291 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/colcompspmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/columnobject.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15598 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/densematrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5137 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/eigenmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/functor.hh
--rw-r--r--   0 runner    (1001) docker     (121)    43764 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/istlmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13757 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/istlmatrixadapter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    34090 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/istlpreconditioner.hh
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/preconditionerwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    37242 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/matrix/spmatrix.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/projection/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/dgl2projection.hh
--rw-r--r--   0 runner    (1001) docker     (121)    46069 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/hdivprojection.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6441 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/l2projection.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4272 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/dense.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/localrieszprojection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/orthonormal.hh
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9834 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/projection/vtxprojection.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.987974 dune-fem-2.9.0rc1/dune/fem/operator/test/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8538 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/operator/test/unitrows.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.991973 dune-fem-2.9.0rc1/dune/fem/quadrature/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6631 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/agglomerationquadrature.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.991973 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/cacheprovider.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7552 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/cacheprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/pointmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/pointprovider.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/pointprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/registry.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.991973 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/cache_test.cc
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/cache_test.hh
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6472 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/point_test.cc
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/point_test.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8507 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/twist_test.cc
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/twist_test.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/topology.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/topology.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistprovider.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11000 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistutility.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9930 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14577 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/cachingpointlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8546 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/cachingquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4483 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/cornerpointset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/defaultquadratures.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/dunequadratures.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8603 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/elementpointlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12841 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/elementpointlistbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/elementquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9882 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/femquadratures.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/femquadratures_inline.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/gausspoints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10041 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/gausspoints_implementation.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.991973 dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/gausslegendre.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/quadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/idprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/integrator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8891 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/interpolationquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/intersectionquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3698 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/lumpingquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3853 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature0d.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15939 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature1d.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15710 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature2d.cc
--rw-r--r--   0 runner    (1001) docker     (121)    35191 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature3d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/pyramidpoints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24303 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/quadprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18642 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/quadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/quadratureimp.hh
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/quadratureimp_inline.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.991973 dune-fem-2.9.0rc1/dune/fem/quadrature/test/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/1dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   118558 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/3dcubesimp.dgf
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/agglomerationquadrature.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11408 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/cachingquadrature.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13809 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/checkleafcodim1.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7327 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/elementquadrature.cc
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/quad_test.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/quadrature/test/quad_test.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.995974 dune-fem-2.9.0rc1/dune/fem/schemes/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    23536 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/conservationlawmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    31734 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/dgelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/dgfemscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/diffusionmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23053 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/dirichletwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19868 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9642 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)    70135 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/galerkin.hh
--rw-r--r--   0 runner    (1001) docker     (121)    43025 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/integrands.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6097 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/linearized.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18807 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/schemes/molgalerkin.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.995974 dune-fem-2.9.0rc1/dune/fem/solver/
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    26085 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/amgistl.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7303 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/amgxsolver.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26973 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/cginverseoperator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.995974 dune-fem-2.9.0rc1/dune/fem/solver/communication/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/communication/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5068 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/communication/fem.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7213 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/communication/hierarchical.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6506 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/communication/owneroverlapcopy.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/diagonalpreconditioner.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/eigen.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6986 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/fempreconditioning.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7898 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/inverseoperatorinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    35170 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/istl.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15836 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/istlinverseoperators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11665 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/krylovinverseoperators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12206 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/ldlsolver.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.995974 dune-fem-2.9.0rc1/dune/fem/solver/linear/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/linear/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/linear/bicgstab.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/linear/cg.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7575 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/linear/gmres.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14106 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/multistep.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22797 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/newtoninverseoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/odesolver.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/odesolverinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/oemsolver.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10291 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/parameter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6698 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/parameterdoc.hh
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/pardginverseoperators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19866 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/petscinverseoperators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/preconditionedinverseoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/preconditionfunctionwrapper.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.999974 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/basicimplicit.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12751 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/basicrow.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10700 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/butchertable.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/butchertable.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7471 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/explicit.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/implicit.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/row.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9046 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/semiimplicit.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14590 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/timestepcontrol.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12956 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/spqrsolver.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.999974 dune-fem-2.9.0rc1/dune/fem/solver/test/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/amgxconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)    23433 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/inverseoperatortest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/newtontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11113 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/odetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/test/test-timeprovider.cc
--rw-r--r--   0 runner    (1001) docker     (121)    21099 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/timeprovider.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10426 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/umfpacksolver.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8712 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/solver/viennacl.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.999974 dune-fem-2.9.0rc1/dune/fem/space/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.999974 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5169 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/basisfunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    58351 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/codegen.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21894 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/default.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25877 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/evaluatecaller.hh
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/evaluatecallerdeclaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6803 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/evaluatecallerdefaultimpl.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3869 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/functor.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.999974 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10689 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/anisotropic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/basisfunctionsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/legendre.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10163 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/orthogonal.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6142 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/typeindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/typemap.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/vectorial.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8107 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/piolatransformation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8786 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/simple.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.003974 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/1dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/checkbasisfunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8199 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-cachingbasisfunctionset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4607 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-defaultbasisfunctionset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-generate.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-simplebasisfunctionset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-tuplebasisfunctionset.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13447 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-vectorialbasisfunctionset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/transformation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12031 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/transformed.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28400 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/tuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21060 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/vectorial.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/brezzidouglasmarini.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.003974 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/combineddofstorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5966 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/combinedspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6563 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/generic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/lagrangepointsetexporter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5644 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/powerlocalrestrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11113 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/powermapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9436 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/powerspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/subobjects.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9586 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/tuplelocalrestrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19345 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/tuplemapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15697 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace/tuplespace.hh
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/combinedspace.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.003974 dune-fem-2.9.0rc1/dune/fem/space/common/
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    32076 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/adaptationmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/adaptcallbackhandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/adaptmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5697 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/allgeomtypes.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/auxiliarydofs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9677 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/basesetlocalkeystorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)    48456 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/cachedcommmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/commindexmap.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/commoperations.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13533 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/communicationmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26241 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/datacollector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.007974 dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/dataprojection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7413 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/default.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/tuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6992 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/defaultcommhandler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    41194 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/discretefunctionspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)    49962 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dofmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4961 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/dofstorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11952 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/functionspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/functionspaceinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9692 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/interpolate.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9226 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/loadbalancer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/localrestrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6925 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/restrictprolongfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13765 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/restrictprolonginterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11661 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/restrictprolongtuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/slavedofs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/common/uniquefacetorientation.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.007974 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/basisfunctionsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5873 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/generic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4699 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/hierarchiclegendre.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8045 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/lagrange.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9403 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/legendre.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/localdgmassmatrix.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11003 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/localrestrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/shapefunctionsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7563 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13484 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/tuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.007974 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8355 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/basisfunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/basisfunctionsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/finitevolume.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.007974 dune-fem-2.9.0rc1/dune/fem/space/fourier/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3929 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/dofmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14217 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/functionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/interpolate.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/fourier.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.007974 dune-fem-2.9.0rc1/dune/fem/space/hpdg/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/anisotropic.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22679 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/blockmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6158 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/default.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11928 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/legendre.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/localdofstorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8207 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/orthogonal.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10982 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/hpdg/space.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.007974 dune-fem-2.9.0rc1/dune/fem/space/lagrange/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/adaptmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/dofmappercode.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22293 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/genericbasefunctions.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14977 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/genericgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    30869 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/genericlagrangepoints.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24923 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/lagrangepoints.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/restrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/shapefunctionset.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12558 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/shapefunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14273 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/storage.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.011974 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/basisfunctiontest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/basisfunctiontest.hh
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/cube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/generic.cc
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/mappertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/mappertest.hh
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/onesimplex.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     6799 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/lagrange.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.011974 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7890 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15247 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/dgspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14609 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10730 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/localrestrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/quadratureinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/shapefunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14798 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/space.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.011974 dune-fem-2.9.0rc1/dune/fem/space/mapper/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5181 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/code.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11629 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/codimensionmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5249 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/compile.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9342 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/dofmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11267 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/dynamicnonblockmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (121)    34460 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/genericadaptivedofmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15738 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/ghost.hh
--rw-r--r--   0 runner    (1001) docker     (121)    27918 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/indexsetdofmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/localkey.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10003 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/nonblockmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8980 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/parallel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/mapper/petsc.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17960 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/p1bubble.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.011974 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/adaptmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/discontinuousgalerkin.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14743 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/generic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9028 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/lagrange.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5836 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/mapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/padaptivespace.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/restrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/padaptivespace.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.011974 dune-fem-2.9.0rc1/dune/fem/space/rannacherturek/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/rannacherturek/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/rannacherturek/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5330 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/rannacherturek.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.011974 dune-fem-2.9.0rc1/dune/fem/space/raviartthomas/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/raviartthomas/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15832 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/raviartthomas/localinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8374 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/raviartthomas/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/raviartthomas.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.015974 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14152 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/caching.hh
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/lagrange.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/legendre.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/legendrepolynomials.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/legendrepolynomials.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/localfunctions.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.015974 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_1d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8498 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_1d.hh
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_2d.cc
--rw-r--r--   0 runner    (1001) docker     (121)   248281 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_2d.hh
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_3d.cc
--rw-r--r--   0 runner    (1001) docker     (121)  3902513 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_3d.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9263 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/proxy.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/selectcaching.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/shapefunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5696 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/simple.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13787 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/tensorproduct.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9749 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/tuple.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21674 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/vectorial.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/wrapper.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.019974 dune-fem-2.9.0rc1/dune/fem/space/test/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/1dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_8.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    13507 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_poly-0.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    13507 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_poly-1.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    13507 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_poly-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/3dgrid_8.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     4569 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11937 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/adapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/checklocalinterpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8729 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/combinedspacetest.cc
--rwxr-xr-x   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/dgcomm-4.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      403 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/dgcomm-cached-4.sh
--rw-r--r--   0 runner    (1001) docker     (121)    10093 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/dgcomm.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12417 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/functiontupleadapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/hierarchicspace.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11238 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/interpolation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    20840 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/l2projection.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11302 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/lagrangeadapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/lagrangeglobalrefine.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11993 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/lagrangeinterpolation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/localadapter.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15788 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/padapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-auxiliarydofs.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9990 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-balladapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-fvadaptation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-globalrefine.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-localadaptation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8429 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-raviartthomasinterpolation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9828 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-spaceinterpolation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2774 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-tupledgspace.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/space/test/test-tuplespace.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fem/storage/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11470 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/dynamicarray.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/eigenvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/envelope.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/objectstack.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10492 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/referencecounter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/referencevector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/rowreferencevector.hh
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/singleton.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/singleton.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/singletonlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/subvector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fem/storage/test/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/storage/test/dynamicarray.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fem/test/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/1dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/2dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/3dgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      394 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/adaptation-4.sh
--rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/adaptation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/dfspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11998 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/dgl2projection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/exactsolution.hh
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/fmatrixconverter.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/l2projection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5089 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/lagrangeinterpolation.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/massoperator.hh
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/referencesolution.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4666 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/simpleoperators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/test-hierarchicall2projection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/test-intersectionindexset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/test-periodic.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6193 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/test-tupleoperator.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/testgrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/vtxprojection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/test/weightfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fem/version.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fempy/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fempy/common/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/common/collectivecommunication.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fempy/function/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18172 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/function/simplegridfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19586 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/function/virtualizedgridfunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fempy/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/geometry/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/geometry/edgelength.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fempy/grid/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/grid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5598 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/grid/adaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/grid/discretefunctionmanager.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11685 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/grid/globalmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6477 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/grid/virtualizedrestrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3622 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/parameter.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.023974 dune-fem-2.9.0rc1/dune/fempy/py/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/py/common/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/common/numpyvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22716 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/discretefunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/py/function/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/function/grid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/py/grid/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/grid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/grid/adaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17371 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/grid/function.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/grid/gridpart.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4443 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/grid/numpy.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/grid/restrictprolong.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/integrands.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/integrandsbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13519 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/operator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9939 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/scheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7239 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/space.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/spaceadapt.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/py/ufllocalfunction.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/pybind11/gridfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/pybind11/pybind11.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/pybind11/space.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/quadrature/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/quadrature/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4187 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/quadrature/cachingpoint.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/quadrature/elementpoint.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9273 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/quadrature/fempyquadratures.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/space/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/space/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/space/adaptation.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/dune/fempy/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2068 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/backrest1.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      526 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/backrest2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/fempy-bcrsmatrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/fenics-elasticity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/fenics-heat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3135 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/fenics-poisson.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/filteredgridview.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/interpolate.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1099 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/levelspaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/localcontexttest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/mixed.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6401 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/scheme_assemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/test-quad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/test-tupledf.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3772 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/test_assembly.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/test_quad.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/testd2.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/testnVector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/testoperator.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/testufl2vtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/testvecbackends.py
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune/fempy/test/vtktest.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune-fem.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/dune.module
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/lib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/pydemo/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/pydemo/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     5197 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/pydemo/advectiondiffusion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6272 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/pydemo/testthreading.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.027974 dune-fem-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6028 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6724 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/_fem.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/_spaceadaptation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/_discretefunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/_solvers.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/eigen.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/istl.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/discretefunction/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/function/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6137 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/function/_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/model/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/model/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/model/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/operator/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/operator/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13996 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9417 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/scheme/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/scheme/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16021 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/scheme/_schemes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/scheme/dgmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/space/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/space/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14881 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30074 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/space/_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fem/utility/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/utility/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5440 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fem/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/fenics/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fenics/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fenics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8402 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/fenics/_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/models/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9522 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/formfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    21942 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    16503 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/conservationlaw/ufl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.031974 dune-fem-2.9.0rc1/python/dune/models/integrands/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/formfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    13812 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     5945 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    23467 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/integrands/ufl.py
--rw-r--r--   0 runner    (1001) docker     (121)    14337 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/models/localfunction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/python/dune/source/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/python/dune/source/algorithm/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/algorithm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/algorithm/extractincludes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/algorithm/extractvariables.py
--rw-r--r--   0 runner    (1001) docker     (121)    13176 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/builtin.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    18933 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/cplusplus.py
--rw-r--r--   0 runner    (1001) docker     (121)     7561 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/fem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/python/dune/source/formatter/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/formatter/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7236 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/formatter/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/function.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/source/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/python/dune/ufl/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19641 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/applyrestrictions.py
--rw-r--r--   0 runner    (1001) docker     (121)    40989 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/formfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/gatherderivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/latex.py
--rw-r--r--   0 runner    (1001) docker     (121)     7369 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune/ufl/tensors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/python/dune_fem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune_fem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    38225 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune_fem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune_fem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune_fem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/python/dune_fem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      336 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/addauthors.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1067 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/check-headers.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3165 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/check-opts.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1260 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/check-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/scripts/ci-petsc/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/ci-petsc/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (121)     1234 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/fullcheck.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      119 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/getparameter.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1302 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/mpiexec.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/scripts/opts/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/ci-clang-5.opts
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/ci-clang-6.opts
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/ci-clang.opts
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/ci-gcc.opts
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/ci-gcc7.opts
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/ci-headercheck.opts
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_alberta.opts.unused
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_all.opts
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_alu_cube.opts
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_alu_simplex.opts
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_none.opts
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_spgrid.opts
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/opts/config_spgrid.opts.unused
--rwxr-xr-x   0 runner    (1001) docker     (121)      245 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/replace.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1012 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/scripts/rundocker.sh
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:17:03.035974 dune-fem-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:02.000000 dune-fem-2.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.107748 dune-fem-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-05-29 21:03:41.107748 dune-fem-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3218 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.019747 dune-fem-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/AddPAPIFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/AddSIONlibFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/CommandLineHacks.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/CorrectWindowsPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4920 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/DuneFemMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/DuneFempyMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FemShort.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FemTortureTests.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindAmgXSolver.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindPAPI.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    16964 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindPETSc.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindPThreads.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindPackageMultipass.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindSIONlib.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindViennaCL.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/FindXDR.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/ResolveCompilerPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/cmake/modules/UseModelCompiler.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/doxygen/modules
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/doc/doxygen/pages/
+-rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/doxygen/pages/docrules.page
+-rw-r--r--   0 runner    (1001) docker     (121)     5917 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/doxygen/pages/main.page
+-rw-r--r--   0 runner    (1001) docker     (121)     4980 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/doc/operator-concept.tex
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/bindguard.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/coordinate.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5595 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/explicitfieldvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/fmatrixcol.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/forloop.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6143 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/geometrytypemap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6039 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/hybrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/intersectionside.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/localcontribution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/memory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/referencevector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/stackallocator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/common/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/test/test-hybrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7363 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/tupletypetraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10566 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/tupleutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/typeindexedtuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/common/utility.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/function/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/function/adaptivefunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/adaptivefunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7378 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/adaptivefunction/adaptivefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/adaptivefunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/function/blockvectordiscretefunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectordiscretefunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectordiscretefunction/blockvectordiscretefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectordiscretefunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.027747 dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7297 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction/blockvectorfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/blockvectors/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectors/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21291 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectors/defaultblockvectors.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/blockvectors/referenceblockvector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/combinedfunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/combinedfunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18053 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/combinedfunction/combinedfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/combinedfunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/common.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    41635 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/discretefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14727 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/discretefunction_inline.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3317 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/dofblock.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7804 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/dofiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/function.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/functionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3134 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/functor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23009 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/gridfunctionadapter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6596 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/instationary.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9267 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/localcontribution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26218 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/localfunctionadapter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/rangegenerators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5915 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/common/scalarproducts.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/hierarchical/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11993 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/hierarchical/dofvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/hierarchical/function.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/hierarchical.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5487 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/average.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/bindable.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25604 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/const.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8627 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/converter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19881 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/localfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5322 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/localfunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/localfunctionsetadapter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/mutable.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9527 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/localfunction/temporary.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/petscdiscretefunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/petscdiscretefunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12306 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/petscdiscretefunction/petscdiscretefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/petscdiscretefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/subfunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/1dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6745 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/test-df.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/test-filtered-df.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5834 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/test-hierarchicalfunction-comm.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3155 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/test-hierarchicalfunction.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4626 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/test-lfa.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5948 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/test/test-tuplediscretefunction.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.031747 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/discretefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/dofvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/functor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/scalarproducts.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.035747 dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction/managedvectorfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction/vectorfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.035747 dune-fem-2.9.dev20220529/dune/fem/gridpart/
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19615 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/adaptiveleafgridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    50309 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/adaptiveleafindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17378 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/codimindexset.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.035747 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/compositegeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5309 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/deaditerator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/defaultgridpartentity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4889 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/entitysearch.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/extendedentity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17904 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6668 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridpart2gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridpartadapter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8198 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridview2gridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8631 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/localfunctiongeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/metatwistutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5684 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/persistentindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/policies.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/sharedgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/simplegeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/common/unimplementedgeometry.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.035747 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8367 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/basicfilterwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4943 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/domainfilter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/filter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/inversefilter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/radialfilter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4035 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/simple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/threadfilter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/voidfilter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filter.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.035747 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2287 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3990 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15048 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.039747 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10580 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/cornerstorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6955 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5994 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12527 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.039747 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6497 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13820 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.039747 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7434 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4516 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8445 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4169 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11743 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/leafgridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/levelgridpart.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.039747 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/1dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4543 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkgridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7217 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8951 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkintersections.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/failure.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4399 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/test-gplagrangeinterpolation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12025 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/gridpart/test/test-gridpart.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.039747 dune-fem-2.9.dev20220529/dune/fem/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.039747 dune-fem-2.9.dev20220529/dune/fem/io/file/
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/asciiparser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    35314 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/dataoutput.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25975 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/datawriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21402 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/iointerface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/iolock.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15918 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/iotuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11214 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/latextablewriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17010 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/persistencemanager.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/file/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/backuprestore.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10524 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/dataoutputtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/test/persistencemanagertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    19435 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/file/vtkio.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/io.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/io.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/parameter/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20524 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter/container.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter/parametertree.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11090 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter/reader.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    29150 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/parameter.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/streams/
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8186 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/asciistreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/binarystreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10823 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/sionlibstreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8281 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/standardstreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12190 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/streams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/streams_inline.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/streams/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6193 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/test/test-streams.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/tuples.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9105 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/virtualstreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/streams/xdrstreams.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)       76 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/bc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)       77 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/date.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/param_DarcyStokes
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/param_NavierStokes
+-rw-r--r--   0 runner    (1001) docker     (121)     2503 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/parameterdicttest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/parametertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/test/testparameterfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/visual/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/converttemplate.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/dataconvert.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3748 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/datadisp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/errordisplay.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      828 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/grcommon.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/printhelp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/programtemplate.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9871 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/readioparams.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/readiotupledata.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3495 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/readtupledata.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.043747 dune-fem-2.9.dev20220529/dune/fem/marking/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/marking/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/marking/default.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12635 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/marking/doerfler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/marking/localerror.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/marking/maximum.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.047747 dune-fem-2.9.dev20220529/dune/fem/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15075 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/alugridwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/bartonnackmaninterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8807 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/boundaryidprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5207 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9161 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/checkgeomaffinity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/compatibility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/debug.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/debugbreak.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16808 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/domainintegral.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27163 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/double.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26035 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/femeoc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23850 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/femeoctable.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/femtimer.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13610 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/femtimer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/fieldmatrixhelper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5719 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/flops.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12152 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/fmatrixconverter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/functor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/griddeclaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/gridfunctionview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/gridname.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/gridobjectstreams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10966 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/gridsolution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/gridwidth.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7590 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/h1norm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8171 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/l1norm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12999 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/l2norm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8421 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/linesegmentsampler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14883 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/lpnorm.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/mapgeomtype.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5255 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/metaprogramming.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18238 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/mpimanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5045 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/nonconformitylevel.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.047747 dune-fem-2.9.dev20220529/dune/fem/misc/petsc/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/petsc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20031 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/petsc/petsccommon.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10379 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/petsc/petscdofblock.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20752 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/petsc/petscvector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.047747 dune-fem-2.9.dev20220529/dune/fem/misc/threads/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9745 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/domainthreaditerator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/threaditerator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3765 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/threaditeratorstorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/threadmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8660 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/threadpartitioner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/threadpool.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/threads/threadsafevalue.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5571 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/misc/umfpack.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.047747 dune-fem-2.9.dev20220529/dune/fem/operator/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.047747 dune-fem-2.9.dev20220529/dune/fem/operator/1order/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/1order/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    36862 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/1order/localmassmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.051747 dune-fem-2.9.dev20220529/dune/fem/operator/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/automaticdifferenceoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/differentiableoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12503 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/localcontribution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19578 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/localmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5324 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/localmatrixcolumn.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7428 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/localmatrixwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16682 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/localoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13641 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/mapping.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/objpointer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8532 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/operator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8988 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/spaceoperatorif.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14812 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/stencil.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8359 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/temporarylocalmatrix.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.051747 dune-fem-2.9.dev20220529/dune/fem/operator/common/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/test/mappingtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5137 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/common/tuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/dghelmholtz.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.051747 dune-fem-2.9.dev20220529/dune/fem/operator/linear/
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14251 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/blockdiagonal.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/denserow.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/eigenoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13641 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/hierarchical.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/istladapter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/istloperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/numpyoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    37038 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/petscoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/spoperator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.051747 dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10272 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/checklinearoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/test-hierarchicallinearoperator.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6180 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/test-matrices.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.051747 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7861 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/blockmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5291 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/colcompspmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/columnobject.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15598 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/densematrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5137 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/eigenmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/functor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    41046 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/istlmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13574 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/istlmatrixadapter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    33233 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/istlpreconditioner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/preconditionerwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    34349 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/matrix/spmatrix.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.051747 dune-fem-2.9.dev20220529/dune/fem/operator/projection/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3522 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/dgl2projection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    46069 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/hdivprojection.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.055747 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6441 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/l2projection.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.055747 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4272 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/dense.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/localrieszprojection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/orthonormal.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/projection/vtxprojection.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.055747 dune-fem-2.9.dev20220529/dune/fem/operator/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8538 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/operator/test/unitrows.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.055747 dune-fem-2.9.dev20220529/dune/fem/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6631 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/agglomerationquadrature.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.059748 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/cacheprovider.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7552 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/cacheprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/pointmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/pointprovider.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/pointprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/registry.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.059748 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/cache_test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/cache_test.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6472 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/point_test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/point_test.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8507 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/twist_test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/twist_test.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/topology.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/topology.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistprovider.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11000 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistutility.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9930 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14395 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/cachingpointlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8546 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/cachingquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4483 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/cornerpointset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/defaultquadratures.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/dunequadratures.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8424 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/elementpointlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12841 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/elementpointlistbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/elementquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9882 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/femquadratures.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/femquadratures_inline.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/gausspoints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10041 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/gausspoints_implementation.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.059748 dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/gausslegendre.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/quadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/idprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/integrator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8891 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/interpolationquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5046 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/intersectionquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3698 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/lumpingquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3853 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature0d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15939 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature1d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15710 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature2d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    35191 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature3d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/pyramidpoints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24303 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/quadprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18642 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/quadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10277 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/quadratureimp.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/quadratureimp_inline.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.059748 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/1dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   118558 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/3dcubesimp.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6363 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/agglomerationquadrature.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11408 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/cachingquadrature.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13809 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/checkleafcodim1.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7327 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/elementquadrature.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     9054 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/quad_test.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/quadrature/test/quad_test.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.059748 dune-fem-2.9.dev20220529/dune/fem/schemes/
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    23536 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/conservationlawmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    31734 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/dgelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/dgfemscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/diffusionmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23019 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/dirichletwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19868 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9642 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    70135 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/galerkin.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    42972 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/integrands.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6097 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/linearized.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18807 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/schemes/molgalerkin.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.063748 dune-fem-2.9.dev20220529/dune/fem/solver/
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    26095 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/amgistl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7303 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/amgxsolver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26973 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/cginverseoperator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.063748 dune-fem-2.9.dev20220529/dune/fem/solver/communication/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/communication/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/communication/fem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7223 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/communication/hierarchical.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6506 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/communication/owneroverlapcopy.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/diagonalpreconditioner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/eigen.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6986 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/fempreconditioning.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7898 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/inverseoperatorinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    35170 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/istl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15606 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/istlinverseoperators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11662 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/krylovinverseoperators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12206 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/ldlsolver.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.063748 dune-fem-2.9.dev20220529/dune/fem/solver/linear/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/linear/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/linear/bicgstab.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/linear/cg.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7695 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/linear/gmres.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14126 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/multistep.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22575 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/newtoninverseoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/odesolver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/odesolverinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/oemsolver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10158 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/parameter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6698 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/parameterdoc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/pardginverseoperators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19866 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/petscinverseoperators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/preconditionedinverseoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/preconditionfunctionwrapper.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.063748 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11387 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/basicimplicit.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12751 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/basicrow.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10700 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/butchertable.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/butchertable.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7471 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/explicit.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/implicit.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/row.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9046 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/semiimplicit.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14590 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/timestepcontrol.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12956 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/spqrsolver.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.063748 dune-fem-2.9.dev20220529/dune/fem/solver/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/amgxconfig.json
+-rw-r--r--   0 runner    (1001) docker     (121)    23433 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/inverseoperatortest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/newtontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11153 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/odetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/test/test-timeprovider.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    21337 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/timeprovider.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10426 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/umfpacksolver.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8712 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/solver/viennacl.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.067747 dune-fem-2.9.dev20220529/dune/fem/space/
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.067747 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5169 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/basisfunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    58351 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/codegen.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20391 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/default.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25877 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/evaluatecaller.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/evaluatecallerdeclaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6803 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/evaluatecallerdefaultimpl.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3869 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/functor.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.067747 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10689 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/anisotropic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/basisfunctionsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/legendre.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10163 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/orthogonal.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6142 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/typeindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/typemap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/vectorial.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8107 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/piolatransformation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8786 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/simple.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.067747 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/1dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8410 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/checkbasisfunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8199 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-cachingbasisfunctionset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4607 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-defaultbasisfunctionset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-generate.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2825 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-simplebasisfunctionset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-tuplebasisfunctionset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13447 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-vectorialbasisfunctionset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/transformation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12031 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/transformed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28400 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/tuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21060 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/vectorial.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6960 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/brezzidouglasmarini.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.071748 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/combineddofstorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5966 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/combinedspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6563 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/generic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/lagrangepointsetexporter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5644 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/powerlocalrestrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11113 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/powermapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9436 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/powerspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/subobjects.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9586 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/tuplelocalrestrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19345 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/tuplemapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15697 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/tuplespace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/combinedspace.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.071748 dune-fem-2.9.dev20220529/dune/fem/space/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    32076 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/adaptationmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/adaptcallbackhandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/adaptmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5697 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/allgeomtypes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12963 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/auxiliarydofs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9677 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/basesetlocalkeystorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    48466 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/cachedcommmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6683 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/commindexmap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/commoperations.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13533 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/communicationmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26241 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/datacollector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.071748 dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/dataprojection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7413 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/default.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/tuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6992 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/defaultcommhandler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    40049 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/discretefunctionspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    49962 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dofmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4961 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/dofstorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11952 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/functionspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/functionspaceinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9691 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/interpolate.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9226 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/loadbalancer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/localrestrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6925 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/restrictprolongfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13765 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/restrictprolonginterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11661 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/restrictprolongtuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/slavedofs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/common/uniquefacetorientation.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.075748 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/basisfunctionsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5873 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/generic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4699 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/hierarchiclegendre.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8045 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/lagrange.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9403 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/legendre.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/localdgmassmatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11003 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/localrestrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/shapefunctionsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7563 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13484 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/tuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.075748 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8355 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/basisfunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/basisfunctionsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7826 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/finitevolume.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.075748 dune-fem-2.9.dev20220529/dune/fem/space/fourier/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3929 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/dofmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14217 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/functionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/interpolate.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/fourier.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.075748 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7186 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/anisotropic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22679 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/blockmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6158 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/default.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11826 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/legendre.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/localdofstorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8207 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/orthogonal.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10982 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/hpdg/space.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.075748 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/adaptmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/dofmappercode.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22293 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/genericbasefunctions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14977 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/genericgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    30869 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/genericlagrangepoints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24923 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/lagrangepoints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/restrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/shapefunctionset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12558 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/shapefunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14273 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/storage.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.075748 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/basisfunctiontest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/basisfunctiontest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/cube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/generic.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/mappertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/mappertest.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/onesimplex.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     6799 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/lagrange.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.079748 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7784 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15247 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/dgspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14609 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/interpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10730 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/localrestrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/quadratureinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/shapefunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14798 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/space.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.079748 dune-fem-2.9.dev20220529/dune/fem/space/mapper/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5181 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/code.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11629 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/codimensionmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5249 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/compile.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9342 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/dofmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11267 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/dynamicnonblockmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    34460 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/genericadaptivedofmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14790 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/ghost.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27918 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/indexsetdofmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/localkey.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10003 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/nonblockmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/parallel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/mapper/petsc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17960 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/p1bubble.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.079748 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/adaptmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4104 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/discontinuousgalerkin.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14743 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/generic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9028 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/lagrange.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5836 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/mapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/padaptivespace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5063 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/restrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.079748 dune-fem-2.9.dev20220529/dune/fem/space/rannacherturek/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/rannacherturek/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/rannacherturek/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5330 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/rannacherturek.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.079748 dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15832 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas/localinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8374 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.083748 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14152 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/caching.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/lagrange.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11522 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/legendre.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/legendrepolynomials.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/legendrepolynomials.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/localfunctions.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.083748 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_1d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8498 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_1d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_2d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)   248281 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_2d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_3d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)  3902513 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_3d.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9263 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/proxy.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/selectcaching.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/shapefunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5696 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/simple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13787 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/tensorproduct.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9749 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/tuple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21674 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/vectorial.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/wrapper.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.087748 dune-fem-2.9.dev20220529/dune/fem/space/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/1dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_8.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    13507 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_poly-0.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    13507 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_poly-1.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    13507 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_poly-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/3dgrid_8.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     4569 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11937 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/adapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/checklocalinterpolation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8729 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/combinedspacetest.cc
+-rwxr-xr-x   0 runner    (1001) docker     (121)      381 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/dgcomm-4.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      403 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/dgcomm-cached-4.sh
+-rw-r--r--   0 runner    (1001) docker     (121)    10093 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/dgcomm.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12417 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/functiontupleadapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/hierarchicspace.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11238 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/interpolation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    20840 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/l2projection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11302 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/lagrangeadapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/lagrangeglobalrefine.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11993 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/lagrangeinterpolation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/localadapter.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15788 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/padapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-auxiliarydofs.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9990 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-balladapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-fvadaptation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-globalrefine.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-localadaptation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8429 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-raviartthomasinterpolation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9828 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-spaceinterpolation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2774 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-tupledgspace.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/space/test/test-tuplespace.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fem/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11470 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/dynamicarray.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/eigenvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/envelope.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/objectstack.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10492 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/referencecounter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/referencevector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/rowreferencevector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/singleton.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/singleton.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6368 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/singletonlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/subvector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fem/storage/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/storage/test/dynamicarray.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fem/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/1dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/2dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/3dgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      394 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/adaptation-4.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/adaptation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/dfspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11998 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/dgl2projection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/exactsolution.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/fmatrixconverter.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/l2projection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5089 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/lagrangeinterpolation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/massoperator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/referencesolution.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4666 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/simpleoperators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/test-hierarchicall2projection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/test-intersectionindexset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/test-periodic.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6193 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/test-tupleoperator.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/testgrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/vtxprojection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/test/weightfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fem/version.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fempy/
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fempy/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/common/collectivecommunication.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fempy/function/
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18172 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/function/simplegridfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17902 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/function/virtualizedgridfunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fempy/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/geometry/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/geometry/edgelength.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.091748 dune-fem-2.9.dev20220529/dune/fempy/grid/
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/grid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5598 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/grid/adaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11522 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/grid/discretefunctionmanager.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11685 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/grid/globalmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6477 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/grid/virtualizedrestrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3622 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/parameter.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/py/
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/py/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/common/numpyvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22716 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/discretefunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/py/function/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/function/grid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/py/grid/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/grid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/grid/adaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17371 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/grid/function.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/grid/gridpart.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4443 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/grid/numpy.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/grid/restrictprolong.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/integrands.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/integrandsbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13519 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/operator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9939 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/scheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7015 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/space.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/spaceadapt.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/py/ufllocalfunction.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/pybind11/gridfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/pybind11/pybind11.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/pybind11/space.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/quadrature/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/quadrature/cachingpoint.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/quadrature/elementpoint.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9273 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/quadrature/fempyquadratures.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/space/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/space/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/space/adaptation.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/dune/fempy/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2068 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/backrest1.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      526 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/backrest2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/fempy-bcrsmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/fenics-elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/fenics-heat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3135 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/fenics-poisson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/filteredgridview.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/interpolate.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1099 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/levelspaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/localcontexttest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/mixed.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6401 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/scheme_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/test-quad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/test-tupledf.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3772 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/test_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/test_quad.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/testd2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/testnVector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2398 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/testoperator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/testufl2vtk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/testvecbackends.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune/fempy/test/vtktest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune-fem.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/dune.module
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.095748 dune-fem-2.9.dev20220529/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/lib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/pydemo/
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/pydemo/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5197 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/pydemo/advectiondiffusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6272 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/pydemo/testthreading.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4914 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6028 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6744 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/_fem.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/_spaceadaptation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/_discretefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/eigen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/istl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/function/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6137 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/function/_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/model/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/model/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/model/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/operator/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/operator/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13996 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9252 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/scheme/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/scheme/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16079 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/scheme/_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/scheme/dgmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/space/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/space/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14881 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30074 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/space/_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fem/utility/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/utility/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5440 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fem/view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/fenics/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fenics/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fenics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8402 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/fenics/_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.099748 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9522 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/formfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21942 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16503 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/ufl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/python/dune/models/integrands/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/formfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13812 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5945 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23066 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/integrands/ufl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14337 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/models/localfunction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/python/dune/source/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/python/dune/source/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/algorithm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/algorithm/extractincludes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/algorithm/extractvariables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13176 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4464 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18933 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/cplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7561 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/fem.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/python/dune/source/formatter/
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/formatter/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7236 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/formatter/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/source/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/python/dune/ufl/
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19283 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/applyrestrictions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40580 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/formfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/gatherderivatives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/latex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6751 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5032 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune/ufl/tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/python/dune_fem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune_fem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    38225 2022-05-29 21:03:41.000000 dune-fem-2.9.dev20220529/python/dune_fem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune_fem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune_fem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/python/dune_fem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      336 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/addauthors.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1067 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/check-headers.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3165 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/check-opts.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1260 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/check-tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.103748 dune-fem-2.9.dev20220529/scripts/ci-petsc/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/ci-petsc/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1234 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/fullcheck.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      119 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/getparameter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1302 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/mpiexec.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:41.107748 dune-fem-2.9.dev20220529/scripts/opts/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/ci-clang-5.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/ci-clang-6.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/ci-clang.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/ci-gcc.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/ci-gcc7.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/ci-headercheck.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_alberta.opts.unused
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_all.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_alu_cube.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_alu_simplex.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_none.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_spgrid.opts
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/opts/config_spgrid.opts.unused
+-rwxr-xr-x   0 runner    (1001) docker     (121)      245 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/replace.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1012 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/scripts/rundocker.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:41.107748 dune-fem-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:40.000000 dune-fem-2.9.dev20220529/setup.py
```

### Comparing `dune-fem-2.9.0rc1/.gitlab-ci.yml` & `dune-fem-2.9.dev20220529/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/AUTHORS` & `dune-fem-2.9.dev20220529/AUTHORS`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/CHANGELOG.md` & `dune-fem-2.9.dev20220529/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/CMakeLists.txt` & `dune-fem-2.9.dev20220529/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/COPYING` & `dune-fem-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/LICENSE.md` & `dune-fem-2.9.dev20220529/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/PKG-INFO` & `dune-fem-2.9.dev20220529/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-fem
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: A discretization module providing an implementation of mathematical abstractions to solve PDEs on parallel computers including local grid adaptivity, dynamic load balancing, and higher order discretization schemes
 Home-page: https://gitlab.dune-project.org/dune-fem/dune-fem
 Author: The Dune-Fem developer team
 Author-email: dune-fem@lists.dune-project.org
 License: UNKNOWN
 Description: DUNE-FEM
         ========
@@ -118,15 +118,15 @@
          [15]: http://faculty.cse.tamu.edu/davis/suitesparse.html
          [16]: http://www.fz-juelich.de/jsc/sionlib
          [17]: http://icl.cs.utk.edu/papi/software/index.html
          [18]: https://dune-project.org/sphinx/content/sphinx/dune-fem/
          [19]: https://gitlab.dune-project.org/dune-fem/dune-fem/-/pipelines/
         
         
-        git-74e87fef1ff200e0346b7d174471befd59a78917
+        git-05b6c5700eaebdd472d9fe71bdcb1e300a6f9293
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-fem-2.9.0rc1/README.md` & `dune-fem-2.9.dev20220529/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,8 +110,8 @@
  [15]: http://faculty.cse.tamu.edu/davis/suitesparse.html
  [16]: http://www.fz-juelich.de/jsc/sionlib
  [17]: http://icl.cs.utk.edu/papi/software/index.html
  [18]: https://dune-project.org/sphinx/content/sphinx/dune-fem/
  [19]: https://gitlab.dune-project.org/dune-fem/dune-fem/-/pipelines/
 
 
-git-74e87fef1ff200e0346b7d174471befd59a78917
+git-05b6c5700eaebdd472d9fe71bdcb1e300a6f9293
```

### Comparing `dune-fem-2.9.0rc1/cmake/modules/AddPAPIFlags.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/AddPAPIFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/AddSIONlibFlags.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/AddSIONlibFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/CommandLineHacks.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/CommandLineHacks.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/CorrectWindowsPaths.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/CorrectWindowsPaths.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/DuneFemMacros.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/DuneFemMacros.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,16 @@
 # if open mp should be used perform cmake check
 if(USE_OPENMP)
   find_package(OpenMP)
   if(OPENMP_FOUND)
     # add flags to compiler flags
     set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
 
-    # on MacOS we need to add the linker flags
+    # on MacOS we need to add the shared linker flags
     if(APPLE)
-      get_filename_component(OPENMP_LIB_PATH ${OpenMP_CXX_LIBRARIES} DIRECTORY)
-      set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -lomp -L${OPENMP_LIB_PATH}")
       set(CMAKE_SHARED_LINKER_FLAGS "${CMAKE_SHARED_LINKER_FLAGS} ${OpenMP_CXX_LIBRARIES}")
     endif()
   endif(OPENMP_FOUND)
 endif(USE_OPENMP)
 
 # check for phtreads
 include(FindPThreads)
```

### Comparing `dune-fem-2.9.0rc1/cmake/modules/DuneFempyMacros.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/DuneFempyMacros.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FemShort.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FemShort.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindAmgXSolver.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindAmgXSolver.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindPAPI.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindPAPI.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindPETSc.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindPETSc.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindPThreads.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindPThreads.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindPackageMultipass.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindPackageMultipass.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindSIONlib.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindSIONlib.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindViennaCL.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindViennaCL.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/FindXDR.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/FindXDR.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/ResolveCompilerPaths.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/ResolveCompilerPaths.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/cmake/modules/UseModelCompiler.cmake` & `dune-fem-2.9.dev20220529/cmake/modules/UseModelCompiler.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/config.h.cmake` & `dune-fem-2.9.dev20220529/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/doc/doxygen/Doxylocal` & `dune-fem-2.9.dev20220529/doc/doxygen/Doxylocal`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/doc/doxygen/pages/docrules.page` & `dune-fem-2.9.dev20220529/doc/doxygen/pages/docrules.page`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/doc/doxygen/pages/main.page` & `dune-fem-2.9.dev20220529/doc/doxygen/pages/main.page`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/doc/operator-concept.tex` & `dune-fem-2.9.dev20220529/doc/operator-concept.tex`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/bindguard.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/bindguard.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/explicitfieldvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/explicitfieldvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/fmatrixcol.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/fmatrixcol.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/forloop.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/forloop.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/geometrytypemap.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/geometrytypemap.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/hybrid.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/hybrid.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/intersectionside.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/metatwistutility.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-#ifndef DUNE_FEM_COMMON_INTERSECTIONSIDE_HH
-#define DUNE_FEM_COMMON_INTERSECTIONSIDE_HH
+#ifndef DUNE_FEM_METATWISTUTILITY_HH
+#define DUNE_FEM_METATWISTUTILITY_HH
 
-#include <dune/common/typelist.hh>
-#include <dune/common/typeutilities.hh>
+#include <cassert>
+
+#include <dune/fem/quadrature/caching/twistutility.hh>
 
 namespace Dune
 {
+
   namespace Fem
   {
-    enum class IntersectionSide : std::size_t { in = 0u, out = 1u };
-
-    template<class GF, class Intersection>
-    auto bindIntersection(GF& gf, const Intersection& intersection, IntersectionSide side, PriorityTag<2>)
-     -> decltype(gf.bind(intersection, side))
-    {
-      gf.bind(intersection, side);
-    }
 
-    template<class GF, class Intersection>
-    auto bindIntersection(GF& gf, const Intersection& intersection, IntersectionSide side, PriorityTag<1>)
-     -> decltype(gf.bind(intersection.impl().hostIntersection(), side))
+    /** \brief MetaTwistUtility forwards the twist calls to the TwistUtility of the
+     *         underlying HostTwistUtility.
+     *
+     *  \note The class Intersection implementation is assumed to have a method
+     *        hostIntersection().
+     */
+    template< class HostTwistUtility >
+    struct MetaTwistUtility
     {
-      gf.bind(intersection.impl().hostIntersection(), side);
-    }
+      typedef HostTwistUtility  HostTwistUtilityType;
+      typedef typename HostTwistUtilityType :: GridType  GridType;
 
-    template<class GF, class Intersection>
-    auto bindIntersection(GF& gf, const Intersection& intersection, IntersectionSide side, PriorityTag<0>)
-     -> decltype(gf.bind(intersection.inside()))
-    {
-      // store local copy to avoid problems with casting to temporary types
-      const auto entity = (side == IntersectionSide::in) ? intersection.inside() : intersection.outside();
-      gf.bind(entity);
-    }
+      //! \brief return 0 for inner face
+      template< class Intersection >
+      static int twistInSelf ( const GridType & grid, const Intersection & intersection )
+      {
+        return HostTwistUtilityType::twistInSelf( grid, intersection.impl().hostIntersection() );
+      }
+
+      //! \brief return 0 for outer face
+      template< class Intersection >
+      static int twistInNeighbor ( const GridType & grid , const Intersection & intersection )
+      {
+        return HostTwistUtilityType::twistInNeighbor( grid, intersection.impl().hostIntersection() );
+      }
+
+      /** \brief return geometry type of inside or outside entity */
+      template< class Intersection >
+      static GeometryType elementGeometry ( const Intersection &intersection, const bool inside )
+      {
+        return HostTwistUtilityType::elementGeometry( intersection.impl().hostIntersection(), inside );
+      }
+    };
 
+  } // namespace Fem
 
-    template<class GF, class Intersection>
-    void defaultIntersectionBind(GF &gf, const Intersection &intersection, IntersectionSide side)
-    {
-      bindIntersection(gf, intersection, side, PriorityTag<2>{});
-    }
-  }
-}
+} // namespace Dune
 
-#endif // DUNE_FEM_COMMON_INTERSECTIONSIDE_HH
+#endif // #ifndef DUNE_FEM_METATWISTUTILITY_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/localcontribution.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/localcontribution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/memory.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/memory.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/stackallocator.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/stackallocator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/test/test-hybrid.cc` & `dune-fem-2.9.dev20220529/dune/fem/common/test/test-hybrid.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/tupletypetraits.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/tupletypetraits.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/tupleutility.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/tupleutility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/typeindexedtuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/typeindexedtuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/common/utility.hh` & `dune-fem-2.9.dev20220529/dune/fem/common/utility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/adaptivefunction/adaptivefunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/adaptivefunction/adaptivefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/blockvectordiscretefunction/blockvectordiscretefunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/blockvectordiscretefunction/blockvectordiscretefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction/blockvectorfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction/blockvectorfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/blockvectorfunction/declaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/blockvectorfunction/declaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/blockvectors/defaultblockvectors.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/blockvectors/defaultblockvectors.hh`

 * *Files 2% similar despite different names*

```diff
@@ -326,20 +326,14 @@
 
     /** \brief Iterator pointing to before the first dof */
     IteratorType beforeBegin() { return array().beforeBegin(); }
 
     /** \brief Iterator pointing to before the first dof */
     ConstIteratorType beforeBegin() const { return array().beforeBegin(); }
 
-    /** \brief Iterator pointing to a given dof (non blocked numbering) */
-    IteratorType find( const SizeType dof ) { return array().find( dof ); }
-
-    /** \brief Iterator pointing to a given dof (non blocked numbering) */
-    ConstIteratorType find( const SizeType dof ) const { return array().find( dof ); }
-
     /** \brief Number of blocks */
     SizeType size () const { return array().size() / blockSize; }
 
     /** \brief Number of dofs in the block vector */
     SizeType numDofs() const { return array().size(); }
 
     FieldType* data() { return ContainerAccess< ArrayType >::data( array() ); }
@@ -551,32 +545,19 @@
     public:
       //! Default constructor
       Iterator( const EmbeddedIterator& it
 #ifndef NDEBUG
               , const EmbeddedIterator& end = EmbeddedIterator()
 #endif
               )
-        : Iterator( it, 0
-#ifndef NDEBUG
-                  , end
-#endif
-                  )
-      {}
-
-      //! Default constructor
-      Iterator( const EmbeddedIterator& it, const int index
-#ifndef NDEBUG
-              , const EmbeddedIterator& end = EmbeddedIterator()
-#endif
-              )
         : it_( it ),
 #ifndef NDEBUG
           end_( end ),
 #endif
-          index_( index )
+          index_(0)
       {}
 
       //! return dof
       FieldType& dereference () const
       {
         assert( it_ != end_ );
         assert( index_ < blockSize );
@@ -675,38 +656,14 @@
 
     ConstIteratorType beforeBegin() const
     {
       DUNE_THROW(NotImplemented,"ISTLBlockVector::beforeBegin not implemented yet");
       return array().end();
     }
 
-    /** \brief Iterator pointing to a given dof (non blocked numbering) */
-    IteratorType find( const SizeType dof )
-    {
-      const SizeType block = dof / blockSize;
-      const SizeType index = dof % blockSize;
-      return IteratorType( array().find( block ), index
-#ifndef NDEBUG
-                          , array().end()
-#endif
-                         );
-    }
-
-    /** \brief Iterator pointing to a given dof (non blocked numbering) */
-    ConstIteratorType find( const SizeType dof ) const
-    {
-      const SizeType block = dof / blockSize;
-      const SizeType index = dof % blockSize;
-      return ConstIteratorType( array().find( block ), index
-#ifndef NDEBUG
-                              , array().end()
-#endif
-                              );
-    }
-
     SizeType size() const { return array().size(); }
 
     /** \brief Number of dofs in the block vector */
     SizeType numDofs() const { return array().size() * DofBlock::dimension; }
 
     /** \brief Reserve memory.
      *
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/blockvectors/referenceblockvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/blockvectors/referenceblockvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/combinedfunction/combinedfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/combinedfunction/combinedfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/common.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/common.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/discretefunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/discretefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/discretefunction_inline.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/discretefunction_inline.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/dofblock.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/dofblock.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/dofiterator.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/dofiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/function.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/function.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/functionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/functionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/functor.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/functor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/gridfunctionadapter.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/gridfunctionadapter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/instationary.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/instationary.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/localcontribution.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/localcontribution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/localfunctionadapter.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/localfunctionadapter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/rangegenerators.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/rangegenerators.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/common/scalarproducts.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/common/scalarproducts.hh`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #include <map>
 #include <limits>
 #include <algorithm>
 
 #include <dune/common/exceptions.hh>
 #include <dune/common/genericiterator.hh>
 #include <dune/common/ftraits.hh>
+#include <dune/common/version.hh>
 
 #include <dune/grid/common/gridenums.hh>
 #include <dune/grid/common/datahandleif.hh>
 
 #if HAVE_DUNE_ISTL
 #include <dune/istl/scalarproducts.hh>
 #endif
@@ -45,17 +46,24 @@
       typedef Dune::BlockVector< Block > type;
     };
 
     template <class Block>
     struct ISTLScalarProductSelector< Dune::Fem::ISTLBlockVector< Block > >
       : public Dune::ScalarProduct< typename Dune::Fem::ISTLBlockVector< Block > :: DofContainerType >
     {
+#if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      //! define the category
+      enum { category=Dune::SolverCategory::sequential };
+#endif // #if !DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+
       typedef typename ISTLBlockVector< Block > :: DofContainerType type;
 
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
       Dune::SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
     };
 #endif
 
     //! Proxy class to evaluate ScalarProduct
     //! holding AuxiliaryDofs which is singleton per space and mapper
     template< class DiscreteFunction >
     class ParallelScalarProduct
@@ -114,19 +122,16 @@
       //! evaluate scalar product on dofVector and omit auxiliary nodes
       template < class DofVector, class OtherDofVector >
       RangeFieldType dotProduct ( const DofVector &x, const OtherDofVector &y ) const
       {
         typedef typename DiscreteFunctionSpaceType::LocalBlockIndices LocalBlockIndices;
 
         RangeFieldType scp = 0;
-        auto compScp = [&x, &y, &scp]( const size_t dof ){
-          Hybrid::forEach( LocalBlockIndices(), [ &x, &y, &scp, dof ] ( auto &&j ) { scp += x[ dof ][ j ] * y[ dof ][ j ]; } );
-        };
-        // compute scalar product for primary dofs
-        forEachPrimaryDof( space().auxiliaryDofs(), compScp );
+        for( const auto i : primaryDofs( space().auxiliaryDofs() ) )
+          Hybrid::forEach( LocalBlockIndices(), [ &x, &y, &scp, i ] ( auto &&j ) { scp += x[ i ][ j ] * y[ i ][ j ]; } );
         return space().gridPart().comm().sum( scp );
       }
 
 #if HAVE_DUNE_ISTL
     protected:
       typedef typename ISTLScalarProductSelector< typename DiscreteFunction :: DofVectorType > :: type BlockVectorType;
 
@@ -151,19 +156,20 @@
         // case of ALUGrid and DGSpace or FVSpace
         // BUG: We should not use the leafGridView to detect whether the grid has overlap!
         const bool deleteGhostEntries = (space().gridPart().grid().leafGridView().overlapSize( 0 ) == 0) && !space().continuous();
 
         // only delete ghost entries
         if( deleteGhostEntries )
         {
-          auto delEntry = [&x] (const size_t dof )
-          {
-            x[ dof ] = 0;
-          };
-          forEachAuxiliaryDof( space().auxiliaryDofs(), delEntry );
+          const auto &auxiliaryDofs = space().auxiliaryDofs();
+
+          // don't delete the last since this is the overall Size
+          const size_t auxiliarySize = auxiliaryDofs.size() - 1;
+          for(size_t auxiliary = 0; auxiliary<auxiliarySize; ++auxiliary)
+            x[ auxiliaryDofs[auxiliary] ] = 0;
         }
 #endif // #if HAVE_MPI
       }
 #endif // #if HAVE_DUNE_ISTL
       const DiscreteFunctionSpaceType &space_;
     };
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/hierarchical/dofvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/hierarchical/dofvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/hierarchical/function.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/hierarchical/function.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/average.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/average.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/bindable.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/bindable.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/const.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/const.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/converter.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/converter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/localfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/localfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/localfunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/localfunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/localfunctionsetadapter.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/localfunctionsetadapter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/mutable.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/mutable.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/localfunction/temporary.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/localfunction/temporary.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/petscdiscretefunction/petscdiscretefunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/petscdiscretefunction/petscdiscretefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/subfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/subfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/function/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/test-df.cc` & `dune-fem-2.9.dev20220529/dune/fem/function/test/test-df.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/test-filtered-df.cc` & `dune-fem-2.9.dev20220529/dune/fem/function/test/test-filtered-df.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/test-hierarchicalfunction-comm.cc` & `dune-fem-2.9.dev20220529/dune/fem/function/test/test-hierarchicalfunction-comm.cc`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
   v.clear();
 
   Dune::Fem::ConstLocalFunction< GridFunction > uLocal( u );
   Dune::Fem::TemporaryLocalFunction< typename DiscreteFunction::DiscreteFunctionSpaceType > vLocal( v.space() );
   Dune::Fem::LocalInterpolation< typename DiscreteFunction::DiscreteFunctionSpaceType > interpolation( v.space() );
 
   // iterate over selected partition
-  for( const auto& entity : elements( v.gridPart(), Dune::Partitions::all ) )
+  for( const auto entity : elements( v.gridPart(), Dune::Partitions::all ) )
   {
     // initialize u, v to entity
     auto uGuard = bindGuard( uLocal, entity );
     auto vGuard = bindGuard( vLocal, entity );
 
     // bind interpolation to entity
     auto iGuard = bindGuard( interpolation, entity );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/test-hierarchicalfunction.cc` & `dune-fem-2.9.dev20220529/dune/fem/function/test/test-hierarchicalfunction.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/test-lfa.cc` & `dune-fem-2.9.dev20220529/dune/fem/function/test/test-lfa.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/test/test-tuplediscretefunction.cc` & `dune-fem-2.9.dev20220529/dune/fem/function/test/test-tuplediscretefunction.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/discretefunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/discretefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/dofvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/dofvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/functor.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/functor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/tuplediscretefunction/scalarproducts.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/tuplediscretefunction/scalarproducts.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/vectorfunction/managedvectorfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction/managedvectorfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/function/vectorfunction/vectorfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/function/vectorfunction/vectorfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/adaptiveleafgridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/adaptiveleafgridpart.hh`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
       //! type of the grid part , i.e. this type
       typedef AdaptiveLeafGridPart< GridType, idxpitype, onlyCodimensionZero > GridPartType;
 
       /** \brief The type of the corresponding TwistUtility */
       typedef TwistUtility< GridType >  TwistUtilityType ;
 
-      typedef typename GridType::Communication CommunicationType;
+      typedef typename GridType::CollectiveCommunication CollectiveCommunicationType;
 
     protected:
       // choose the AdaptiveIndexSet (based on the HierarchicIndexSet)
       // to be revised
       template < int dummy, bool onlyCodimZero >
       struct AdaptiveLeafIndexSetChooser
       {
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/adaptiveleafindexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/adaptiveleafindexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/codimindexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/codimindexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/compositegeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/compositegeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/deaditerator.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/deaditerator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/defaultgridpartentity.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/defaultgridpartentity.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/entitysearch.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/entitysearch.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/extendedentity.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkseed.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,83 @@
-// -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
-// vi: set et ts=4 sw=2 sts=2:
-#ifndef DUNE_FEM_GRIDPART_COMMON_ENTITY_HH
-#define DUNE_FEM_GRIDPART_COMMON_ENTITY_HH
+#ifndef DUNE_FEM_GRIDPART_TEST_CHECKSEED_HH
+#define DUNE_FEM_GRIDPART_TEST_CHECKSEED_HH
+
+//- C++ includes
+#include <limits>
+#include <type_traits>
+
+//- dune-common includes
+#include <dune/fem/common/forloop.hh>
+#include <dune/common/exceptions.hh>
+
+//- dune-fem includes
+#include <dune/fem/gridpart/common/capabilities.hh>
 
-#include <dune/grid/common/entity.hh>
 
 namespace Dune
 {
 
-  /**
-   @brief Wrapper class for wrapped entities added a cast operator to the host
-   entity.
-
-   \tparam cd Codimension of the entity
-   \tparam dim Dimension of the grid
-   \tparam GridImp Type that is a model of Dune::Grid
-   \tparam EntityImp Class template that is a model of Dune::Entity
-
-  */
-  template<int cd, int dim, class GridImp, template<int,int,class> class EntityImp>
-  class ExtendedEntity : public Dune::Entity< cd, dim, GridImp, EntityImp >
+  namespace Fem
   {
-    typedef Dune::Entity< cd, dim, GridImp, EntityImp > BaseType;
-  public:
-    using BaseType::BaseType;
-
-  protected:
-    template<typename T>
-    struct ToVoid
-    {
-      typedef void type;
-    };
 
-    template <typename T, typename dummy = void>
-    struct checkHostEntity : std::false_type {};
+    /** \brief Iterate over all entities of all codimensions available in the grid part,
+     *         and perform a number of tests on each entity.
+     */
 
-    template <typename T>
-    struct checkHostEntity<T, typename ToVoid<typename T::HostEntityType>::type > : std::true_type{};
+    template< class GridPartType >
+    class CheckEntitySeed
+    {
+      template< class GridPart, bool >
+      struct If
+      {
+        template< int codim >
+        static void check ( const GridPart & )
+        { }
+      };
 
+      template< class GridPart >
+      struct If< GridPart, true >
+      {
+        template< const int codim >
+        static void check ( const GridPart &gridPart )
+        {
+          typedef typename GridPart::template Codim< codim >::EntityType EntityType;
+          typedef typename GridPart::template Codim< codim >::EntitySeedType EntitySeedType;
+          static_assert( std::is_same< EntitySeedType, typename EntityType::EntitySeed >::value, "Types of EntitySeed do not coincide" );
+
+          for( auto it = gridPart.template begin< codim >(); it != gridPart.template end< codim >(); ++it )
+          {
+            auto entity = *it;
+            auto seed = entity.seed();
+            if( gridPart.entity( seed ) != entity )
+              DUNE_THROW( Dune::Exception, "Could not recover entity from seed" );
+          }
+        }
+      };
 
-    template <class Impl, bool>
-    struct HE {
-      typedef Impl      HostEntity;
-      typedef BaseType  GridEntity;
-    };
+      template< int codim >
+      struct CheckCodim
+      {
+        template< class GridPart >
+        static void apply ( const GridPart &gridPart )
+        {
+          // check whether grid part has entity of given codimension
+          constexpr bool hasEntity = Dune::Fem::GridPartCapabilities::hasEntity< GridPart, codim >::v;
+          If< GridPart, hasEntity >::template check< codim >( gridPart );
+        }
+      };
 
-    template <class Impl>
-    struct HE< Impl, true >
-    {
-    private:
-      // type of grid entity
-      typedef typename Impl::HostGridPartType::GridType::template Codim<cd>::Entity __GEType;
     public:
-      typedef typename Impl::HostEntityType HostEntity;
-      typedef typename
-        std::conditional< std::is_same<HostEntity, __GEType>::value,
-                          BaseType, __GEType> :: type GridEntity;
-    };
-
-  public:
-    typedef typename BaseType::Implementation  ImplementationType;
-    static constexpr bool hasHostEntity = checkHostEntity< ImplementationType >::value;
-    typedef typename HE< ImplementationType, hasHostEntity >::HostEntity   HostEntityType;
-    typedef typename HE< ImplementationType, hasHostEntity >::GridEntity  GridEntityType;
-
-    /** \brief cast to HostEntityType if such type exists otherwise return implementation */
-    operator const HostEntityType& () const
-    {
-      if constexpr ( hasHostEntity )
-        return this->impl().hostEntity();
-      else
-        return this->impl();
-    }
+      static const int dimension = GridPartType::dimension;
 
-    /** \brief cast to HostEntityType if such type exists otherwise return implementation */
-    operator const GridEntityType& () const
-    {
-      if constexpr ( std::is_same< BaseType, GridEntityType > :: value )
-        return *this;
-      else
+      static void check ( const GridPartType &gridPart )
       {
-        return gridEntity(*this);
+        // generic for loop over all codimensions
+        Dune::Fem::ForLoop< CheckCodim, 0, dimension >::apply( gridPart );
       }
-    }
-  };
+    };
+
+  } // end namespace Fem
 
 } // end namespace Dune
-#endif
+
+#endif // #ifndef DUNE_FEM_GRIDPART_TEST_CHECKSEED_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridpart.hh`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,17 @@
 
       //! \brief Index set implementation
       typedef typename Traits::IndexSetType IndexSetType;
       //! \brief Index set implementation
       typedef IndexSetType IndexSet;
 
       //! \brief Collective communication
-      typedef typename Traits::CommunicationType CommunicationType;
+      typedef typename Traits::CollectiveCommunicationType CollectiveCommunicationType;
       //! \brief Collective communication
-      typedef CommunicationType Communication;
+      typedef CollectiveCommunicationType CollectiveCommunication;
 
       //! \brief Twist utility type
       typedef typename Traits::TwistUtilityType TwistUtilityType;
 
       //! \brief Maximum Partition type, the index set provides indices for
       static const PartitionIteratorType indexSetPartitionType
         = Traits::indexSetPartitionType;
@@ -274,15 +274,15 @@
       int boundaryId ( const IntersectionType &intersection ) const
       {
         CHECK_INTERFACE_IMPLEMENTATION( asImp().boundaryId( intersection ) );
         return asImp().boundaryId( intersection );
       }
 
       /** \brief obtain collective communication object */
-      const CommunicationType &comm () const
+      const CollectiveCommunicationType &comm () const
       {
         CHECK_INTERFACE_IMPLEMENTATION( asImp().comm() );
         return asImp().comm();
       }
 
       //! \brief corresponding communication method for grid part
       template< class DataHandleImp, class DataType >
@@ -376,15 +376,15 @@
       //! type of intersection iterator
       typedef typename Traits::IntersectionIteratorType IntersectionIteratorType;
 
       //! type of intersection
       typedef typename IntersectionIteratorType::Intersection IntersectionType;
 
       //! \brief Collective communication
-      typedef typename Traits::CommunicationType CommunicationType;
+      typedef typename Traits::CollectiveCommunicationType CollectiveCommunicationType;
 
       //! \brief type of DofManager
       typedef DofManager< GridType >  DofManagerType;
 
       //! type of boundary id provider specialized for each grid type
       typedef BoundaryIdProvider< GridType > BoundaryIdProviderType;
 
@@ -439,15 +439,15 @@
       template<class EntityType>
       bool contains (const EntityType& e) const
       {
         return BaseType::indexSet().contains(e);
       }
 
       /** \brief obtain collective communication object */
-      const CommunicationType &comm () const
+      const CollectiveCommunicationType &comm () const
       {
         return grid().comm();
       }
 
       /** \brief \copydoc GridPartInterface::entity
        *
        * \tparam  EntitySeed  entity seed from which to create entity
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridpart2gridview.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridpart2gridview.hh`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
       typedef typename GridPart::GridType Grid;
       typedef typename GridPart::IndexSetType IndexSet;
       typedef typename GridPart::IntersectionIteratorType IntersectionIterator;
 
       typedef typename IntersectionIterator::Intersection Intersection;
 
-      typedef typename GridPart::CommunicationType Communication;
+      typedef typename GridPart::CollectiveCommunicationType CollectiveCommunication;
 
       template< int codim >
       struct Codim
       : public Grid::Traits::template Codim< codim >
       {
         typedef typename GridPart::template Codim< codim >::EntityType Entity;
 
@@ -86,15 +86,15 @@
       /** \brief type of the intersection */
       typedef typename Traits::Intersection Intersection;
 
       /** \brief type of the intersection iterator */
       typedef typename Traits::IntersectionIterator IntersectionIterator;
 
       /** \brief type of the collective communication */
-      typedef typename Traits::Communication Communication;
+      typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
       /** \brief Codim Structure */
       template< int codim >
       struct Codim
       : public Traits::template Codim< codim >
       {};
 
@@ -178,15 +178,15 @@
       }
 
       IntersectionIterator iend ( const typename Codim< 0 >::Entity &entity ) const
       {
         return gridPart().iend( entity );
       }
 
-      const Communication &comm () const
+      const CollectiveCommunication &comm () const
       {
         return gridPart().comm();
       }
 
       int overlapSize ( int codim ) const
       {
         DUNE_THROW( NotImplemented, "Method ghostSize() not implemented yet" );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridpartadapter.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridpartadapter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/gridview2gridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/gridview2gridpart.hh`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     {
       typedef Implementation GridPartType;
 
       typedef GridView GridViewType;
       static const bool conforming = GridView::conforming;
 
       typedef typename GridViewType::Grid GridType;
-      typedef typename GridViewType::Communication CommunicationType;
+      typedef typename GridViewType::CollectiveCommunication CollectiveCommunicationType;
 
       typedef typename GridView::IndexSet IndexSetType;
 
       template< int codim >
       struct Codim
       {
         typedef typename GridViewType::template Codim< codim >::Entity EntityType;
@@ -97,16 +97,16 @@
 
       /** \copydoc Dune::Fem::GridPartInterface::IntersectionIteratorType */
       typedef typename BaseType::IntersectionIteratorType IntersectionIteratorType;
 
       /** \copydoc Dune::Fem::GridPartInterface::IndexSetType */
       typedef typename BaseType::IndexSetType IndexSetType;
 
-      /** \copydoc Dune::Fem::GridPartInterface::CommunicationType */
-      typedef typename BaseType::CommunicationType CommunicationType;
+      /** \copydoc Dune::Fem::GridPartInterface::CollectiveCommunicationType */
+      typedef typename BaseType::CollectiveCommunicationType CollectiveCommunicationType;
 
     private:
       typedef DofManager< GridType > DofManagerType;
 
       auto initGv( const GridView &gridView )
       {
         if constexpr ( storeCopy )
@@ -190,15 +190,15 @@
       /** \copydoc Dune::Fem::GridPartInterface::iend */
       IntersectionIteratorType iend ( const typename Codim< 0 >::EntityType &entity ) const
       {
         return gridView().iend( entity );
       }
 
       /** \copydoc Dune::Fem::GridPartInterface::comm */
-      const CommunicationType &comm () const { return gridView().comm(); }
+      const CollectiveCommunicationType &comm () const { return gridView().comm(); }
 
       /** \copydoc Dune::Fem::GridPartInterface::communicate */
       template< class DataHandle, class DataType >
       void communicate ( CommDataHandleIF< DataHandle, DataType > &dataHandle,
                          InterfaceType interface, CommunicationDirection direction ) const
       {
         gridView().communicate( dataHandle, interface, direction );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/indexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/indexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/localfunctiongeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/localfunctiongeometry.hh`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,15 @@
         return ret;
       }
 
       JacobianTransposed jacobianTransposed ( const LocalCoordinate &local ) const
       {
         const auto gradFT = localFunction().entity().geometry().jacobianTransposed( local );
 
-        typename LocalFunction::FunctionSpaceType::JacobianRangeType gradPhi;
-
+        FieldMatrix< ctype, coorddimension, coorddimension > gradPhi;
         localFunction().jacobian( local, gradPhi );
 
         JacobianTransposed jacTransposed( 0 );
         for( int i = 0; i < coorddimension; ++i )
         {
           FieldMatrixColumn< JacobianTransposed > col( jacTransposed, i );
           gradFT.mv( gradPhi[ i ], col );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/metatwistutility.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/intersectioniterator.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-#ifndef DUNE_FEM_METATWISTUTILITY_HH
-#define DUNE_FEM_METATWISTUTILITY_HH
+#ifndef DUNE_FEM_GRIDPART_GEOMETRYGRIDPART_INTERSECTIONITERATOR_HH
+#define DUNE_FEM_GRIDPART_GEOMETRYGRIDPART_INTERSECTIONITERATOR_HH
 
-#include <cassert>
+#include <type_traits>
 
-#include <dune/fem/quadrature/caching/twistutility.hh>
+#include <dune/grid/common/intersectioniterator.hh>
+
+#include <dune/fem/gridpart/geometrygridpart/intersection.hh>
 
 namespace Dune
 {
 
   namespace Fem
   {
 
-    /** \brief MetaTwistUtility forwards the twist calls to the TwistUtility of the
-     *         underlying HostTwistUtility.
-     *
-     *  \note The class Intersection implementation is assumed to have a method
-     *        hostIntersection().
-     */
-    template< class HostTwistUtility >
-    struct MetaTwistUtility
+    // GeometryGridPartIntersectionIterator
+    // ------------------------------------
+
+    template< class GridFamily >
+    class GeometryGridPartIntersectionIterator
     {
-      typedef HostTwistUtility  HostTwistUtilityType;
-      typedef typename HostTwistUtilityType :: GridType  GridType;
+      typedef GeometryGridPartIntersectionIterator< GridFamily > ThisType;
+
+      typedef typename std::remove_const_t< GridFamily >::Traits Traits;
+
+      typedef typename Traits::HostGridPartType::IntersectionIteratorType HostIntersectionIteratorType;
+
+      typedef typename Traits::template Codim< 0 >::Entity Entity;
+      typedef typename Traits::template Codim< 0 >::Geometry ElementGeometry;
+
+      typedef typename Traits::GridFunctionType GridFunctionType;
+
+      typedef GeometryGridPartIntersection< const GridFamily > IntersectionImplType;
+
+    public:
+      typedef Dune::Intersection< const GridFamily, IntersectionImplType > Intersection;
+
+      GeometryGridPartIntersectionIterator () = default;
+
+      GeometryGridPartIntersectionIterator ( const Entity &inside, const HostIntersectionIteratorType &hostIterator )
+        : hostIterator_( hostIterator ), gridFunction_( &inside.impl().gridFunction() ), insideGeo_( inside.geometry().impl() )
+      {}
+
+      bool equals ( const ThisType &other ) const { return (hostIterator_ == other.hostIterator_); }
+
+      void increment () { ++hostIterator_; }
+
+      Intersection dereference () const { return IntersectionImplType( *gridFunction_, insideGeo_, *hostIterator_ ); }
 
-      //! \brief return 0 for inner face
-      template< class Intersection >
-      static int twistInSelf ( const GridType & grid, const Intersection & intersection )
-      {
-        return HostTwistUtilityType::twistInSelf( grid, intersection.impl().hostIntersection() );
-      }
-
-      //! \brief return 0 for outer face
-      template< class Intersection >
-      static int twistInNeighbor ( const GridType & grid , const Intersection & intersection )
-      {
-        return HostTwistUtilityType::twistInNeighbor( grid, intersection.impl().hostIntersection() );
-      }
-
-      /** \brief return geometry type of inside or outside entity */
-      template< class Intersection >
-      static GeometryType elementGeometry ( const Intersection &intersection, const bool inside )
-      {
-        return HostTwistUtilityType::elementGeometry( intersection.impl().hostIntersection(), inside );
-      }
+    private:
+      HostIntersectionIteratorType hostIterator_;
+      const GridFunctionType *gridFunction_ = nullptr;
+      typename ElementGeometry::Implementation insideGeo_;
     };
 
   } // namespace Fem
 
 } // namespace Dune
 
-#endif // #ifndef DUNE_FEM_METATWISTUTILITY_HH
+#endif // #ifndef DUNE_FEM_GRIDPART_GEOMETRYGRIDPART_INTERSECTIONITERATOR_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/persistentindexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/persistentindexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/policies.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/policies.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/sharedgeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/sharedgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/simplegeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/simplegeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/common/unimplementedgeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/common/unimplementedgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/basicfilterwrapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/basicfilterwrapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/domainfilter.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/domainfilter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/filter.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/filter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/inversefilter.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/inversefilter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/radialfilter.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/radialfilter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/simple.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/simple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filter/voidfilter.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filter/voidfilter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/datahandle.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/datahandle.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/intersection.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/intersection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/intersectioniterator.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/intersectioniterator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart/iterator.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart/iterator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/filteredgridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/filteredgridpart.hh`

 * *Files 2% similar despite different names*

```diff
@@ -176,16 +176,16 @@
           typedef IteratorType Iterator;
         };
 
         typedef typename Partition< InteriorBorder_Partition >::IteratorType IteratorType;
         typedef IteratorType Iterator;
       };
 
-      typedef typename HostGridPartType::CommunicationType CommunicationType;
-      typedef CommunicationType Communication;
+      typedef typename HostGridPartType::CollectiveCommunicationType CollectiveCommunicationType;
+      typedef CollectiveCommunicationType CollectiveCommunication;
 
       //! \brief maximum partition type, the index set provides indices for
       static const PartitionIteratorType indexSetPartitionType = HostGridPartType::indexSetPartitionType;
 
       static const InterfaceType indexSetInterfaceType = HostGridPartType::indexSetInterfaceType;
 
       //! \brief is true if grid on this view only has conforming intersections
@@ -242,15 +242,15 @@
 
       //! \brief intersection iterator type
       typedef typename Traits:: IntersectionIteratorType IntersectionIteratorType;
 
       //! \brief intersection type
       typedef typename IntersectionIteratorType::Intersection IntersectionType;
 
-      typedef typename Traits::CommunicationType CommunicationType;
+      typedef typename Traits::CollectiveCommunicationType CollectiveCommunicationType;
 
       typedef ThisType GridViewType;
 
       //! \brief grid part typedefs, use those of traits
       template< int codim >
       struct Codim : public Traits :: template Codim< codim >
       {};
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/cornerstorage.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/cornerstorage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/datahandle.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/datahandle.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/entity.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/entity.hh`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,16 @@
       static const int dimensionworld = std::remove_const< GridFamily >::type::dimensionworld;
 
       typedef typename std::remove_const< GridFamily >::type::ctype ctype;
 
       typedef typename Traits::template Codim< codimension >::EntitySeed EntitySeed;
       typedef typename Traits::template Codim< codimension >::Geometry Geometry;
 
-      typedef typename Traits::HostGridPartType HostGridPartType;
-
     private:
+      typedef typename Traits::HostGridPartType HostGridPartType;
       typedef typename Traits::CoordFunctionType CoordFunctionType;
 
       typedef typename Geometry::Implementation GeometryImplType;
 
       typedef GeoCoordVector< mydimension, GridFamily > CoordVectorType;
 
     public:
@@ -125,17 +124,16 @@
       typedef typename Traits::template Codim< codimension >::Geometry Geometry;
       typedef typename Traits::template Codim< codimension >::LocalGeometry LocalGeometry;
 
       typedef typename Traits::HierarchicIterator HierarchicIterator;
       typedef typename Traits::LeafIntersectionIterator LeafIntersectionIterator;
       typedef typename Traits::LevelIntersectionIterator LevelIntersectionIterator;
 
-      typedef typename Traits::HostGridPartType HostGridPartType;
     private:
-
+      typedef typename Traits::HostGridPartType HostGridPartType;
       typedef typename Traits::CoordFunctionType CoordFunctionType;
 
       typedef typename Geometry::Implementation GeometryImplType;
 
       typedef GeoCoordVector< mydimension, GridFamily > CoordVectorType;
 
     public:
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/geometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/geometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/intersection.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/intersection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart/intersectioniterator.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart/intersectioniterator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geogridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geogridpart.hh`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         template< PartitionIteratorType pitype >
         struct Partition
         {
           typedef EntityIterator< codim, const GridPartFamily, IdIterator< codim, pitype, const GridPartFamily > > IteratorType;
         };
       };
 
-      typedef typename HostGridPartType::CommunicationType CommunicationType;
+      typedef typename HostGridPartType::CollectiveCommunicationType CollectiveCommunicationType;
 
       static const bool conforming = HostGridPartType::Traits::conforming;
     };
 
 
 
     // GeoGridPart
@@ -176,15 +176,15 @@
 
       typedef CoordFunction CoordFunctionType;
 
       typedef typename BaseType::GridType GridType;
       typedef typename BaseType::IndexSetType IndexSetType;
       typedef typename BaseType::IntersectionIteratorType IntersectionIteratorType;
       typedef typename BaseType::IntersectionType IntersectionType;
-      typedef typename BaseType::CommunicationType CommunicationType;
+      typedef typename BaseType::CollectiveCommunicationType CollectiveCommunicationType;
 
       template< int codim >
       struct Codim
       : public BaseType::template Codim< codim >
       {};
 
       explicit GeoGridPart ( const CoordFunctionType &coordFunction )
@@ -267,24 +267,21 @@
       }
 
       // convert a grid entity to a grid part entity ("Gurke!")
       template< class Entity >
       MakeableInterfaceObject< typename Codim< Entity::codimension >::EntityType >
       convert ( const Entity &entity ) const
       {
-        // make sure we have a grid entity
-        const auto& gridEntity = Fem::gridEntity( entity );
-
         // create a grid part entity from a given grid entity
         typedef typename Codim< Entity::codimension >::EntityType EntityType;
         typedef typename EntityType::Implementation Implementation;
         typedef MakeableInterfaceObject< EntityType > EntityObj;
 
         // here, grid part information can be passed, if necessary
-        return EntityObj( Implementation( coordFunction(), hostGridPart().convert( gridEntity ) ) );
+        return EntityObj( Implementation( coordFunction(), entity ) );
       }
 
       // return reference to the coordfunction
       const CoordFunctionType &coordFunction () const
       {
         assert( coordFunction_);
         return *coordFunction_;
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/datahandle.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/datahandle.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/entity.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/entity.hh`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,28 @@
     template< int codim, int dim, class GridFamily >
     class GeometryGridPartEntity
       : public DefaultGridPartEntity < codim, dim, GridFamily >
     {
       typedef typename std::remove_const< GridFamily >::type::Traits Traits;
       typedef typename Traits::GridFunctionType GridFunctionType;
 
-      //typedef typename GridFamily::GridType GridType;
-      //typedef typename GridType::template Codim<codim>::Entity GridEntityType;
-
     public:
       static const int codimension = codim;
       static const int dimension = std::remove_const< GridFamily >::type::dimension;
       static const int mydimension = dimension - codimension;
       static const int dimensionworld = std::remove_const< GridFamily >::type::dimensionworld;
 
       typedef typename std::remove_const< GridFamily >::type::ctype ctype;
 
       typedef typename Traits::template Codim< codimension >::EntitySeed EntitySeed;
       typedef typename Traits::template Codim< codimension >::Geometry Geometry;
 
-      typedef typename Traits::HostGridPartType HostGridPartType;
     private:
+      typedef typename Traits::HostGridPartType HostGridPartType;
+
       typedef typename Geometry::Implementation GeometryImplType;
 
     public:
       typedef typename HostGridPartType::template Codim< codimension >::EntityType HostEntityType;
 
       GeometryGridPartEntity () = default;
 
@@ -116,17 +114,16 @@
       typedef typename Traits::template Codim< codimension >::Geometry Geometry;
       typedef typename Traits::template Codim< codimension >::LocalGeometry LocalGeometry;
 
       typedef typename Traits::HierarchicIterator HierarchicIterator;
       typedef typename Traits::LeafIntersectionIterator LeafIntersectionIterator;
       typedef typename Traits::LevelIntersectionIterator LevelIntersectionIterator;
 
-      typedef typename Traits::HostGridPartType HostGridPartType;
     private:
-      typedef typename HostGridPartType::GridType GridType;
+      typedef typename Traits::HostGridPartType HostGridPartType;
 
     public:
       typedef typename HostGridPartType::template Codim< codimension >::EntityType HostEntityType;
 
       GeometryGridPartEntity () = default;
 
       GeometryGridPartEntity ( const GridFunctionType &gridFunction, HostEntityType hostEntity )
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/indexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/indexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/intersection.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart/intersection.hh`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 #include <type_traits>
 
 #include <dune/common/version.hh>
 
 #include <dune/geometry/referenceelements.hh>
 #include <dune/geometry/affinegeometry.hh>
-#include <dune/geometry/referenceelements.hh>
 #include <dune/fem/misc/boundaryidprovider.hh>
 
 namespace Dune
 {
 
   namespace Fem
   {
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart/intersectioniterator.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/intersectioniterator.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,68 @@
-#ifndef DUNE_FEM_GRIDPART_GEOMETRYGRIDPART_INTERSECTIONITERATOR_HH
-#define DUNE_FEM_GRIDPART_GEOMETRYGRIDPART_INTERSECTIONITERATOR_HH
+#ifndef DUNE_FEM_GRIDPART_IDGRIDPART_INTERSECTIONITERATOR_HH
+#define DUNE_FEM_GRIDPART_IDGRIDPART_INTERSECTIONITERATOR_HH
 
 #include <type_traits>
+#include <utility>
 
 #include <dune/grid/common/intersectioniterator.hh>
 
-#include <dune/fem/gridpart/geometrygridpart/intersection.hh>
+#include <dune/fem/gridpart/idgridpart/intersection.hh>
 
 namespace Dune
 {
 
   namespace Fem
   {
 
-    // GeometryGridPartIntersectionIterator
-    // ------------------------------------
+    // IdIntersectionIterator
+    // ----------------------
 
     template< class GridFamily >
-    class GeometryGridPartIntersectionIterator
+    class IdIntersectionIterator
     {
-      typedef GeometryGridPartIntersectionIterator< GridFamily > ThisType;
+      typedef IdIntersectionIterator< GridFamily > ThisType;
 
-      typedef typename std::remove_const_t< GridFamily >::Traits Traits;
+      typedef typename std::remove_const< GridFamily >::type::Traits Traits;
 
       typedef typename Traits::HostGridPartType::IntersectionIteratorType HostIntersectionIteratorType;
 
-      typedef typename Traits::template Codim< 0 >::Entity Entity;
-      typedef typename Traits::template Codim< 0 >::Geometry ElementGeometry;
-
-      typedef typename Traits::GridFunctionType GridFunctionType;
-
-      typedef GeometryGridPartIntersection< const GridFamily > IntersectionImplType;
+      typedef IdIntersection< const GridFamily > IntersectionImplType;
 
     public:
       typedef Dune::Intersection< const GridFamily, IntersectionImplType > Intersection;
+      typedef typename Traits::ExtraData  ExtraData;
 
-      GeometryGridPartIntersectionIterator () = default;
+      IdIntersectionIterator () = default;
 
-      GeometryGridPartIntersectionIterator ( const Entity &inside, const HostIntersectionIteratorType &hostIterator )
-        : hostIterator_( hostIterator ), gridFunction_( &inside.impl().gridFunction() ), insideGeo_( inside.geometry().impl() )
+      IdIntersectionIterator ( ExtraData data, HostIntersectionIteratorType hostIterator )
+      : data_( std::move( data ) ),
+        hostIterator_( std::move( hostIterator ) )
       {}
 
-      bool equals ( const ThisType &other ) const { return (hostIterator_ == other.hostIterator_); }
-
-      void increment () { ++hostIterator_; }
+      bool equals ( const ThisType &other ) const
+      {
+        return hostIterator_ == other.hostIterator_;
+      }
+
+      void increment ()
+      {
+        ++hostIterator_;
+      }
+
+      Intersection dereference () const
+      {
+        return IntersectionImplType( data(), *hostIterator_ );
+      }
 
-      Intersection dereference () const { return IntersectionImplType( *gridFunction_, insideGeo_, *hostIterator_ ); }
+      const ExtraData &data () const { return data_; }
 
-    private:
+    protected:
+      ExtraData data_;
       HostIntersectionIteratorType hostIterator_;
-      const GridFunctionType *gridFunction_ = nullptr;
-      typename ElementGeometry::Implementation insideGeo_;
     };
 
   } // namespace Fem
 
 } // namespace Dune
 
-#endif // #ifndef DUNE_FEM_GRIDPART_GEOMETRYGRIDPART_INTERSECTIONITERATOR_HH
+#endif // #ifndef DUNE_FEM_GRIDPART_IDGRIDPART_INTERSECTIONITERATOR_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/geometrygridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/geometrygridpart.hh`

 * *Files 5% similar despite different names*

```diff
@@ -164,16 +164,16 @@
         struct Partition
         {
           typedef EntityIterator< codim, const GridFamily, IdIterator< codim, pitype, const GridFamily > > IteratorType;
           typedef IteratorType Iterator;
         };
       };
 
-      typedef typename HostGridPartType::CommunicationType CommunicationType;
-      typedef CommunicationType Communication;
+      typedef typename HostGridPartType::CollectiveCommunicationType CollectiveCommunicationType;
+      typedef CollectiveCommunicationType CollectiveCommunication;
       static const bool conforming = HostGridPartType::Traits::conforming;
     };
 
 
 
     // GeometryGridPart
     // ----------------
@@ -205,17 +205,17 @@
       //! \brief type of intersection iterator
       typedef typename BaseType::IntersectionIterator     IntersectionIterator;
       //! \brief type of intersection
       typedef typename BaseType::IntersectionType IntersectionType;
       //! \brief type of intersection
       typedef typename BaseType::Intersection Intersection;
       //! \brief Collective communication
-      typedef typename BaseType::CommunicationType CommunicationType;
+      typedef typename BaseType::CollectiveCommunicationType CollectiveCommunicationType;
       //! \brief Collective communication
-      typedef typename BaseType::Communication     Communication;
+      typedef typename BaseType::CollectiveCommunication     CollectiveCommunication;
       typedef typename BaseType::GridViewType GridViewType;
 
       // the interface takes this from the grid
       static const int dimensionworld = GridFunction::FunctionSpaceType::dimRange;
 
       template< int codim >
       struct Codim
@@ -286,23 +286,20 @@
       }
 
       // convert a grid entity to a grid part entity ("Gurke!")
       template< class Entity >
       MakeableInterfaceObject< typename Codim< Entity::codimension >::EntityType >
       convert ( const Entity &entity ) const
       {
-        // make sure we have a grid entity
-        const auto& gridEntity = Fem::gridEntity( entity );
-
         // create a grid part entity from a given grid entity
         typedef typename Codim< Entity::codimension >::EntityType EntityType;
         typedef typename EntityType::Implementation Implementation;
         typedef MakeableInterfaceObject< EntityType > EntityObj;
         // here, grid part information can be passed, if necessary
-        return EntityObj( Implementation( gridFunction(), hostGridPart().convert( gridEntity ) ) );
+        return EntityObj( Implementation( gridFunction(), entity ) );
       }
       template < class EntitySeed >
       typename Codim< EntitySeed::codimension >::EntityType
       entity ( const EntitySeed &seed ) const
       {
         return convert( hostGridPart().entity(seed) );
       }
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/datahandle.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/datahandle.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/entity.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/entity.hh`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
       //! type of corresponding entity seed
       typedef typename GridFamily::template Codim< codimension >::EntitySeed EntitySeedType;
       //! type of corresponding geometry
       typedef typename Traits::template Codim< codimension >::Geometry Geometry;
 
       /** \} */
 
+    protected:
       // type of the host grid
       typedef typename Traits::HostGridPartType  HostGridPartType;
 
-    protected:
       // type of extra data, e.g. a pointer to grid (here empty)
       typedef typename Traits::ExtraData ExtraData;
 
     public:
       /** \name Host Types
        *  \{ */
 
@@ -154,30 +154,29 @@
     template< int codim, int dim, class GridFamily >
     class IdEntity : public IdEntityBasic< codim, dim, GridFamily >
     {
       typedef IdEntityBasic< codim, dim, GridFamily > BaseType ;
     protected:
       typedef typename std::remove_const< GridFamily >::type::Traits Traits;
 
-    public:
+    protected:
       // type of the host grid
       typedef typename Traits::HostGridPartType  HostGridPartType;
-    protected:
+
       // type of extra data, e.g. a pointer to grid (here empty)
       typedef typename Traits::ExtraData ExtraData;
 
     public:
       using BaseType :: codimension ;
 
       /** \name Host Types
        *  \{ */
 
       //! type of corresponding host entity
       typedef typename HostGridPartType::template Codim< codimension >::EntityType HostEntityType;
-
       /** \} */
 
       /** \brief construct a null entity */
       IdEntity () = default;
 
       IdEntity ( ExtraData data, HostEntityType hostEntity )
       : BaseType( data, hostEntity )
@@ -194,21 +193,20 @@
      */
     template< int dim, class GridFamily >
     class IdEntity< 0, dim, GridFamily > : public IdEntityBasic< 0, dim, GridFamily >
     {
       typedef IdEntityBasic< 0, dim, GridFamily > BaseType ;
     protected:
       typedef typename BaseType::Traits Traits;
+      typedef typename BaseType::HostGridPartType HostGridPartType;
 
       // type of extra data, e.g. a pointer to grid (here empty)
       typedef typename BaseType::ExtraData ExtraData;
 
     public:
-      typedef typename BaseType::HostGridPartType HostGridPartType;
-
       using BaseType::codimension ;
       using BaseType::data ;
       using BaseType::hostEntity ;
       /** \name Host Types
        *  \{ */
 
       //! type of corresponding host entity
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/geometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/geometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/indexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/indexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/intersection.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/intersection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart/intersectioniterator.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart/iterator.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-#ifndef DUNE_FEM_GRIDPART_IDGRIDPART_INTERSECTIONITERATOR_HH
-#define DUNE_FEM_GRIDPART_IDGRIDPART_INTERSECTIONITERATOR_HH
+#ifndef DUNE_FEM_GRIDPART_IDGRIDPART_ITERATOR_HH
+#define DUNE_FEM_GRIDPART_IDGRIDPART_ITERATOR_HH
 
 #include <type_traits>
 #include <utility>
 
-#include <dune/grid/common/intersectioniterator.hh>
-
-#include <dune/fem/gridpart/idgridpart/intersection.hh>
+#include <dune/common/version.hh>
+#include <dune/grid/common/gridenums.hh>
 
 namespace Dune
 {
 
   namespace Fem
   {
 
-    // IdIntersectionIterator
-    // ----------------------
+    // IdIterator
+    // ----------
 
-    template< class GridFamily >
-    class IdIntersectionIterator
+    template< int codim, PartitionIteratorType pitype, class GridFamily >
+    class IdIterator
     {
-      typedef IdIntersectionIterator< GridFamily > ThisType;
-
       typedef typename std::remove_const< GridFamily >::type::Traits Traits;
 
-      typedef typename Traits::HostGridPartType::IntersectionIteratorType HostIntersectionIteratorType;
-
-      typedef IdIntersection< const GridFamily > IntersectionImplType;
+      typedef typename Traits::HostGridPartType HostGridPartType;
 
     public:
-      typedef Dune::Intersection< const GridFamily, IntersectionImplType > Intersection;
-      typedef typename Traits::ExtraData  ExtraData;
+      typedef typename Traits::ExtraData ExtraData;
+      typedef typename HostGridPartType::template Codim< codim >::template Partition< pitype >::IteratorType HostIteratorType;
 
-      IdIntersectionIterator () = default;
+#if !DUNE_VERSION_NEWER(DUNE_GRID, 2, 6 )
+      static const int codimension = HostIteratorType::codimension;
+#endif
 
-      IdIntersectionIterator ( ExtraData data, HostIntersectionIteratorType hostIterator )
+      typedef typename Traits::template Codim< codim >::Entity Entity;
+
+      IdIterator () = default;
+
+      IdIterator ( ExtraData data, HostIteratorType hostIterator )
       : data_( std::move( data ) ),
         hostIterator_( std::move( hostIterator ) )
       {}
 
-      bool equals ( const ThisType &other ) const
+      void increment ()
       {
-        return hostIterator_ == other.hostIterator_;
+        ++hostIterator_;
       }
 
-      void increment ()
+      Entity dereference () const
       {
-        ++hostIterator_;
+        return typename Entity::Implementation( data_, *hostIterator_ );
       }
 
-      Intersection dereference () const
+      bool equals ( const IdIterator &rhs ) const
       {
-        return IntersectionImplType( data(), *hostIterator_ );
+        return hostIterator_ == rhs.hostIterator_;
       }
 
-      const ExtraData &data () const { return data_; }
+      int level () const
+      {
+        return hostIterator_.level();
+      }
 
-    protected:
+    private:
       ExtraData data_;
-      HostIntersectionIteratorType hostIterator_;
+      HostIteratorType hostIterator_;
     };
 
   } // namespace Fem
 
 } // namespace Dune
 
-#endif // #ifndef DUNE_FEM_GRIDPART_IDGRIDPART_INTERSECTIONITERATOR_HH
+#endif // #ifndef DUNE_FEM_GRIDPART_IDGRIDPART_ITERATOR_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/idgridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/idgridpart.hh`

 * *Files 5% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         template< PartitionIteratorType pitype >
         struct Partition
         {
           typedef EntityIterator< codim, const GridFamily, IdIterator< codim, pitype, const GridFamily > > IteratorType;
         };
       };
 
-      typedef typename HostGridPartType::CommunicationType CommunicationType;
+      typedef typename HostGridPartType::CollectiveCommunicationType CollectiveCommunicationType;
 
       static const bool conforming = HostGridPartType::Traits::conforming;
     };
 
 
 
     // IdGridPart
@@ -142,15 +142,15 @@
     public:
       typedef typename GridFamily::Traits::HostGridPartType HostGridPartType;
 
       typedef typename BaseType::GridType GridType;
       typedef typename BaseType::IndexSetType IndexSetType;
       typedef typename BaseType::IntersectionIteratorType IntersectionIteratorType;
       typedef typename BaseType::IntersectionType IntersectionType;
-      typedef typename BaseType::CommunicationType CommunicationType;
+      typedef typename BaseType::CollectiveCommunicationType CollectiveCommunicationType;
 
       template< int codim >
       struct Codim
       : public BaseType::template Codim< codim >
       {};
 
       explicit IdGridPart ( GridType &grid )
@@ -237,23 +237,20 @@
       }
 
       // convert a grid entity to a grid part entity ("Gurke!")
       template< class Entity >
       MakeableInterfaceObject< typename Codim< Entity::codimension >::EntityType >
       convert ( const Entity &entity ) const
       {
-        // make sure we have a grid entity
-        const auto& gridEntity = Fem::gridEntity( entity );
-
         // create a grid part entity from a given grid entity
         typedef typename Codim< Entity::codimension >::EntityType EntityType;
         typedef typename EntityType::Implementation Implementation;
         typedef MakeableInterfaceObject< EntityType > EntityObj;
         // here, grid part information can be passed, if necessary
-        return EntityObj( Implementation( data(), hostGridPart().convert( gridEntity ) ) );
+        return EntityObj( Implementation( entity ) );
       }
 
       const HostGridPartType &hostGridPart () const { return hostGridPart_; }
 
       HostGridPartType &hostGridPart () { return hostGridPart_; }
 
       typedef typename GridFamily::Traits::ExtraData ExtraData;
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/leafgridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/leafgridpart.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/levelgridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/levelgridpart.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkgeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkgridpart.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkgridpart.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkindexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkindexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/checkintersections.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/checkintersections.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/failure.hh` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/failure.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/test-gplagrangeinterpolation.cc` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/test-gplagrangeinterpolation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/gridpart/test/test-gridpart.cc` & `dune-fem-2.9.dev20220529/dune/fem/gridpart/test/test-gridpart.cc`

 * *Files 8% similar despite different names*

```diff
@@ -71,24 +71,14 @@
 
   // test assignment operator and destructor
   {
     GridPartType newGp( gp );
     newGp = gridPart;
   }
 
-  // conversion to and from grid's entity, which is needed for Adaptation
-  {
-    for( const auto& entity : Dune::elements( gp ) )
-    {
-      const auto& gridEntity = Dune::Fem::gridEntity( entity );
-      const auto& otherEntity = gp.convert( gridEntity );
-      otherEntity.type();
-    }
-  }
-
   // run tests
   std::cout << "Testing entities" << std::endl;
   testGridPart( gridPart );
   std::cout << std::endl;
 
   std::cout << "Testing subentities" << std::endl;
   testSubEntities< GridPartType::dimension >( gridPart );
@@ -101,15 +91,15 @@
   std::cout << "Testing entity seeds" << std::endl;
   Dune::Fem::CheckEntitySeed< GridPartType >::check( gridPart );
   std::cout << "Testing geometries" << std::endl;
   Dune::Fem::CheckGeometry< GridPartType, FailureHandlerType >::check( gridPart, failureHandler );
   std::cout << "Testing index set" << std::endl;
   Dune::Fem::CheckIndexSet< GridPartType, FailureHandlerType >::check( gridPart, failureHandler );
   std::cout << "Testing intersections" << std::endl;
-  ///Dune::Fem::CheckIntersections< GridPartType, FailureHandlerType >::check( gridPart, failureHandler );
+  Dune::Fem::CheckIntersections< GridPartType, FailureHandlerType >::check( gridPart, failureHandler );
 
   // check geometries of macro level and leaf level
   //Dune::GeometryChecker<typename GridPartType::GridType> checker;
   //checker.checkGeometry( gridPart );
   Dune::checkGeometryLifetime( gridPart );
 
   // check entity seeds
@@ -133,38 +123,14 @@
 void testFilteredGridPart( HostGridPartType& hostGridPart, FilterType& filter )
 {
   typedef Dune::Fem::FilteredGridPart< HostGridPartType, FilterType, UseConsecutiveIndexSet > GridPartType;
   GridPartType gridPart( hostGridPart, filter );
   testAll( gridPart );
 }
 
-template <class HostGridPartType, bool v>
-void geomGridPart(HostGridPartType& hostGridPart, std::integral_constant<bool, v> t)
-{
-  typedef Dune::Fem::FunctionSpace< typename HostGridPartType::ctype, typename HostGridPartType::ctype,
-                                    HostGridPartType::dimensionworld, HostGridPartType::dimensionworld > CoordFunctionSpaceType;
-  typedef Dune::Fem::LagrangeDiscreteFunctionSpace< CoordFunctionSpaceType, HostGridPartType, 1 > DiscreteCoordFunctionSpaceType;
-  DiscreteCoordFunctionSpaceType coordFunctionSpace( hostGridPart );
-  typedef Dune::Fem::AdaptiveDiscreteFunction< DiscreteCoordFunctionSpaceType > CoordFunctionType;
-  CoordFunctionType coordFunction( "coordinate function", coordFunctionSpace );
-  typedef Dune::Fem::Identity< CoordFunctionSpaceType > IdentityType;
-  IdentityType identity;
-  Dune::Fem::GridFunctionAdapter< IdentityType, HostGridPartType > identitydDF( "identity", identity, hostGridPart );
-  Dune::Fem::interpolate( identitydDF, coordFunction );
-  typedef Dune::Fem::GeometryGridPart< CoordFunctionType > GridPartType;
-  GridPartType gridPart( coordFunction );
-  testAll( gridPart );
-
-  if constexpr( v )
-  {
-    geomGridPart( gridPart, std::false_type() );
-  }
-}
-
-
 int main ( int argc, char ** argv )
 try
 {
   Dune::Fem::MPIManager::initialize( argc, argv );
 
   // create grid
   auto& grid = Dune::Fem::TestGrid::grid();
@@ -263,15 +229,27 @@
 
   // GeometryGridPart
   {
     std::cout << "************************************" << std::endl;
     std::cout << "***      GeometryGridPart        ***"<< std::endl;
     std::cout << "************************************" << std::endl;
 
-    geomGridPart( hostGridPart, std::true_type() );
+    typedef Dune::Fem::FunctionSpace< GridType::ctype, GridType::ctype, GridType::dimensionworld, GridType::dimensionworld > CoordFunctionSpaceType;
+    typedef Dune::Fem::LagrangeDiscreteFunctionSpace< CoordFunctionSpaceType, HostGridPartType, 1 > DiscreteCoordFunctionSpaceType;
+    DiscreteCoordFunctionSpaceType coordFunctionSpace( hostGridPart );
+    typedef Dune::Fem::AdaptiveDiscreteFunction< DiscreteCoordFunctionSpaceType > CoordFunctionType;
+    CoordFunctionType coordFunction( "coordinate function", coordFunctionSpace );
+    typedef Dune::Fem::Identity< CoordFunctionSpaceType > IdentityType;
+    IdentityType identity;
+    Dune::Fem::GridFunctionAdapter< IdentityType, HostGridPartType > identitydDF( "identity", identity, hostGridPart );
+    Dune::Fem::interpolate( identitydDF, coordFunction );
+    typedef Dune::Fem::GeometryGridPart< CoordFunctionType > GridPartType;
+    GridPartType gridPart( coordFunction );
+
+    testAll( gridPart );
   }
 
   // FilteredGridPart
   {
     std::cout << "******************************" << std::endl;
     std::cout << "***    FilteredGridPart    ***"<< std::endl;
     std::cout << "******************************" << std::endl;
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/asciiparser.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/asciiparser.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/dataoutput.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/dataoutput.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/datawriter.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/datawriter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/iointerface.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/iointerface.hh`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
                                    iTupel& lengthInterior )
         {
           // Yasp only can do origin = 0
           origin = 0;
 
           enum { tag = Grid::tag };
           YLoadBalance< dim > loadBalancer;
-          Torus< typename Grid::Communication, dim > torus( grid.comm(), tag, anz, &loadBalancer );
+          Torus< typename Grid::CollectiveCommunication, dim > torus( grid.comm(), tag, anz, &loadBalancer );
           torus.partition( torus.rank(), origin, anz, originInterior, lengthInterior );
         }
       };
 
 #if HAVE_DUNE_SPGRID
       template< class ct, int dim, template< int > class Strategy, class Comm >
       struct SaveParallelCartesianGrid< SPGrid< ct, dim, Strategy, Comm > >
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/iolock.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/iolock.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/iotuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/iotuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/latextablewriter.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/latextablewriter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/persistencemanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/persistencemanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/io/file/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/test/backuprestore.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/file/test/backuprestore.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/test/dataoutputtest.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/file/test/dataoutputtest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/test/persistencemanagertest.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/file/test/persistencemanagertest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/file/vtkio.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/file/vtkio.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/io.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/io.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/io.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/io.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/parameter/container.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/parameter/container.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/parameter/parametertree.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/parameter/parametertree.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/parameter/parser.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/parameter/parser.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/parameter/reader.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/parameter/reader.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/parameter.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/parameter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/asciistreams.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/asciistreams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/binarystreams.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/binarystreams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/sionlibstreams.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/sionlibstreams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/standardstreams.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/standardstreams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/streams.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/streams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/streams_inline.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/streams_inline.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/test/test-streams.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/test/test-streams.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/tuples.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/tuples.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/streams/virtualstreams.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/streams/virtualstreams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/io/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/test/parameterdicttest.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/test/parameterdicttest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/test/parametertest.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/test/parametertest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/test/testparameterfile` & `dune-fem-2.9.dev20220529/dune/fem/io/test/testparameterfile`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/converttemplate.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/converttemplate.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/dataconvert.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/dataconvert.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/datadisp.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/datadisp.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/errordisplay.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/errordisplay.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/grcommon.hh` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/grcommon.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/printhelp.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/printhelp.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/programtemplate.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/programtemplate.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/readioparams.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/readioparams.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/readiotupledata.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/readiotupledata.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/io/visual/grape/datadisp/readtupledata.cc` & `dune-fem-2.9.dev20220529/dune/fem/io/visual/grape/datadisp/readtupledata.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/marking/default.hh` & `dune-fem-2.9.dev20220529/dune/fem/marking/default.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/marking/doerfler.hh` & `dune-fem-2.9.dev20220529/dune/fem/marking/doerfler.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/marking/localerror.hh` & `dune-fem-2.9.dev20220529/dune/fem/marking/localerror.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/marking/maximum.hh` & `dune-fem-2.9.dev20220529/dune/fem/marking/maximum.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/misc/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,9 +9,7 @@
              linesegmentsampler.hh lpnorm.hh mapgeomtype.hh
              metaprogramming.hh mpimanager.hh
              nonconformitylevel.hh umfpack.hh domainintegral.hh)
 
 dune_add_subdirs(petsc threads)
 
 target_sources(dunefem PRIVATE femtimer.cc)
-
-exclude_from_headercheck( compatibility.hh )
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/alugridwriter.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/alugridwriter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/bartonnackmaninterface.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/bartonnackmaninterface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/boundaryidprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/boundaryidprovider.hh`

 * *Files 1% similar despite different names*

```diff
@@ -315,19 +315,12 @@
       template< class Intersection >
       static int boundaryId ( const Intersection &intersection )
       {
         return (intersection.boundary() ? (intersection.indexInInside()+1) : 0);
       }
     };
 
-    template< class GridPart, class Intersection>
-    inline static int boundaryId ( const Intersection &intersection )
-    {
-      return Dune::Fem::BoundaryIdProvider< typename GridPart::GridType > ::
-             boundaryId( intersection );
-    }
-
   } // namespace Fem
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_FEM_MISC_BOUNDARYIDPROVIDER_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/checkgeomaffinity.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/checkgeomaffinity.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/compatibility.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/compatibility.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef DUNE_FEM_MISC_COMPATIBILITY_HH
 #define DUNE_FEM_MISC_COMPATIBILITY_HH
 
-#error COMPATIBILITY HEADER SHOULD NOT BE USED ANYMORE: make_entity can be removed
+#warning DO NOT INCLUDE 'COMPATIBILITY': the function make_entity is not needed anymore
 
 #include <utility>
 
 #include <dune/grid/common/entity.hh>
 #include <dune/fem/version.hh>
 
 namespace Dune
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/debug.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/debug.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/debugbreak.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/debugbreak.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/domainintegral.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/domainintegral.hh`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
       void normLocal ( const EntityType &entity, unsigned int order, const LocalFunctionType &uLocal, ReturnType &sum ) const
       {
         CHECK_AND_CALL_INTERFACE_IMPLEMENTATION( asImp().normLocal( entity, order, uLocal, sum ) );
       }
 
       const GridPartType &gridPart () const { return gridPart_; }
 
-      const typename GridPartType::CommunicationType& comm () const
+      const typename GridPartType::CollectiveCommunicationType& comm () const
       {
         return gridPart().comm();
       }
 
       bool checkCommunicateFlag( bool communicate ) const
       {
 #ifndef NDEBUG
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/double.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/double.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/femeoc.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/femeoc.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/femeoctable.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/femeoctable.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/femtimer.cc` & `dune-fem-2.9.dev20220529/dune/fem/misc/femtimer.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/femtimer.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/femtimer.hh`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
       if( output_.is_open() )
       {
         output_ << "#  ******** TOTAL RUNTIME: " << totalTime
                 << "   ******** " << std::endl;
         output_.close();
       }
 
-      const MPIManager::Communication &comm = MPIManager::comm();
+      const MPIManager::CollectiveCommunication &comm = MPIManager::comm();
       if( comm.rank() == 0 )
       {
         double *totalTimes = new double[ comm.size() ];
         comm.gather( &totalTime, totalTimes, 1, 0 );
         double avgTime = 0.0;
         double minTime = std::numeric_limits< double >::max();
         double maxTime = std::numeric_limits< double >::min();
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/fieldmatrixhelper.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/fieldmatrixhelper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/flops.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/flops.hh`

 * *Files 8% similar despite different names*

```diff
@@ -133,16 +133,16 @@
         // compute mflops ourselfs
         values[ 4 ] = values[ 3 ] / values[ 0 ];
 
         result_t max( values );
         result_t min( values );
         result_t sum( values );
 
-        typedef MPIManager :: Communication Communication;
-        const Communication& comm = MPIManager :: comm();
+        typedef MPIManager :: CollectiveCommunication CollectiveCommunication;
+        const CollectiveCommunication& comm = MPIManager :: comm();
 
         const int size = max.size();
         // compute max, min, and sum of flop values
         comm.max( &max[ 0 ], size );
         comm.min( &min[ 0 ], size );
         comm.sum( &sum[ 0 ], size );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/fmatrixconverter.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/fmatrixconverter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/functor.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/functor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/griddeclaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/griddeclaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/gridfunctionview.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/gridfunctionview.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/gridname.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/gridname.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/gridobjectstreams.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/gridobjectstreams.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/gridsolution.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/gridsolution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/gridwidth.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/gridwidth.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/h1norm.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/h1norm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/l1norm.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/l1norm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/l2norm.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/l2norm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/linesegmentsampler.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/linesegmentsampler.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/lpnorm.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/lpnorm.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/mapgeomtype.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/mapgeomtype.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/metaprogramming.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/metaprogramming.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/mpimanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/mpimanager.hh`

 * *Files 2% similar despite different names*

```diff
@@ -336,16 +336,16 @@
       };
 
     } // end namespace detail
 
 
     struct MPIManager
     {
-      typedef Dune::Communication< MPIHelper::MPICommunicator >
-        Communication;
+      typedef Dune::CollectiveCommunication< MPIHelper::MPICommunicator >
+        CollectiveCommunication;
     private:
       static MPIManager &instance ()
       {
         return Singleton< MPIManager > :: instance();
       }
 
       static bool mpiFinalized ()
@@ -391,17 +391,17 @@
       static void finalize()
       {
         instance()._finalize();
       }
 
       static void initialize ( int &argc, char **&argv );
 
-      static const Communication &comm ()
+      static const CollectiveCommunication &comm ()
       {
-        const std::unique_ptr< Communication > &comm = instance().comm_;
+        const std::unique_ptr< CollectiveCommunication > &comm = instance().comm_;
         if( !comm )
           DUNE_THROW( InvalidStateException, "MPIManager has not been initialized." );
         return *comm;
       }
 
       static int rank ()
       {
@@ -442,15 +442,15 @@
 
       //! \brief run functor f with given arguments args in threaded mode
       template<typename F, typename... Args>
       static void run(F&& f, Args&&... args) { instance().pool_.run(f,args...); }
 
     private:
       MPIHelper *helper_ = nullptr;
-      std::unique_ptr< Communication > comm_;
+      std::unique_ptr< CollectiveCommunication > comm_;
       bool wasInitializedHere_ = false ;
 #if HAVE_PETSC
       bool petscWasInitializedHere_ = false ;
 #endif
       detail::ThreadPool pool_;
     };
 
@@ -468,15 +468,15 @@
   namespace Fem
   {
     class QuadratureStorageRegistry;
 
     inline void MPIManager::initialize ( int &argc, char **&argv )
     {
       MPIHelper *&helper = instance().helper_;
-      std::unique_ptr< Communication > &comm = instance().comm_;
+      std::unique_ptr< CollectiveCommunication > &comm = instance().comm_;
 
       // the following initialization overrides the MPI_Init in dune-common
       // to avoid a call to MPI_Finalize before all singletons have been deleted
 #if HAVE_MPI
       int wasInitialized = -1;
       MPI_Initialized( &wasInitialized );
       if(!wasInitialized)
@@ -521,15 +521,15 @@
       // if already initialized, do nothing further
       if( helper && comm )
         return ;
 
       // this will just initialize the static variables inside MPIHelper but
       // not call MPI_Init again
       helper = &MPIHelper::instance( argc, argv );
-      comm.reset( new Communication( helper->getCommunicator() ) );
+      comm.reset( new CollectiveCommunication( helper->getCommunicator() ) );
 
 #if HAVE_PETSC
       // initialize PETSc if present
       // returns true if PETSc was initialized during this call
       instance().petscWasInitializedHere_ =
         ::Dune::Petsc::initialize( rank() == 0, argc, argv );
 #endif
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/nonconformitylevel.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/nonconformitylevel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/petsc/petsccommon.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/petsc/petsccommon.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/petsc/petscdofblock.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/petsc/petscdofblock.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/petsc/petscvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/petsc/petscvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/threads/domainthreaditerator.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/threads/domainthreaditerator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/threads/threaditerator.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/threads/threaditerator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/threads/threaditeratorstorage.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/threads/threaditeratorstorage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/threads/threadpartitioner.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/threads/threadpartitioner.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/threads/threadsafevalue.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/threads/threadsafevalue.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/misc/umfpack.hh` & `dune-fem-2.9.dev20220529/dune/fem/misc/umfpack.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/1order/localmassmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/1order/localmassmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/automaticdifferenceoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/automaticdifferenceoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/differentiableoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/differentiableoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/localcontribution.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/localcontribution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/localmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/localmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/localmatrixcolumn.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/localmatrixcolumn.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/localmatrixwrapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/localmatrixwrapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/localoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/localoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/mapping.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/mapping.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/objpointer.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/objpointer.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/operator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/operator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/spaceoperatorif.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/spaceoperatorif.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/stencil.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/stencil.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/temporarylocalmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/temporarylocalmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/test/mappingtest.cc` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/test/mappingtest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/common/tuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/common/tuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/dghelmholtz.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/dghelmholtz.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/blockdiagonal.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/blockdiagonal.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/denserow.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/denserow.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/eigenoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/eigenoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/hierarchical.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/hierarchical.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/istladapter.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/istladapter.hh`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,18 @@
       typedef ISTLLinearOperatorAdapter< Operator > ThisType;
       typedef Dune::LinearOperator< typename Operator::DomainFunctionType::DofStorageType, typename Operator::RangeFunctionType::DofStorageType > BaseType;
 
       typedef typename Operator::DomainFunctionType DomainFunctionType;
       typedef typename Operator::RangeFunctionType  RangeFunctionType;
 
     public:
+#if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      enum {category=SolverCategory::sequential};
+#endif // #if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+
       typedef Operator OperatorType;
 
       typedef typename DomainFunctionType::DiscreteFunctionSpaceType DomainFunctionSpaceType;
       typedef typename RangeFunctionType::DiscreteFunctionSpaceType RangeFunctionSpaceType;
 
       typedef typename BaseType::domain_type domain_type;
       typedef typename BaseType::range_type range_type;
@@ -57,15 +61,17 @@
       {
         const DomainFunctionType fx( "ISTLLinearOperatorAdapter::applyscaleadd::x", domainSpace_, x );
         RangeFunctionType fy( "ISTLLinearOperatorAdapter::applyscaleadd::y", rangeSpace_ );
         op_( fx, fy );
         y.axpy( alpha, fy.blockVector() );
       }
 
-      SolverCategory::Category category () const { return SolverCategory::sequential; }
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       const OperatorType &op_;
       const DomainFunctionSpaceType &domainSpace_;
       const RangeFunctionSpaceType &rangeSpace_;
     };
 
@@ -75,14 +81,18 @@
       typedef ISTLMatrixFreeOperatorAdapter< Operator >   ThisType;
       typedef ISTLLinearOperatorAdapter< Operator >       BaseType;
 
       typedef typename Operator::DomainFunctionType       DomainFunctionType;
       typedef typename Operator::RangeFunctionType        RangeFunctionType;
 
     public:
+#if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      enum {category=SolverCategory::sequential};
+#endif // #if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+
       typedef Operator OperatorType;
 
       typedef typename DomainFunctionType::DiscreteFunctionSpaceType DomainFunctionSpaceType;
       typedef typename RangeFunctionType::DiscreteFunctionSpaceType  RangeFunctionSpaceType;
 
       template <class DF>
       struct IsISTLBlockVectorDiscreteFunction
@@ -137,15 +147,17 @@
         this->apply(x,tmp);
         tmp -= rhs;
 
         // return global sum of residuum
         return scp_.norm(tmp);
       }
 
-      SolverCategory::Category category () const { return SolverCategory::sequential; }
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
       //! return reference to preconditioner
       ParallelScalarProductType& scp() const { return scp_; }
 
       //! dummy function returning 0
       double averageCommTime () const { return 0; }
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/istloperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/istloperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/numpyoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/numpyoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/petscoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/petscoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/spoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/spoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/test/checklinearoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/checklinearoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/test/test-hierarchicallinearoperator.cc` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/test-hierarchicallinearoperator.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/linear/test/test-matrices.cc` & `dune-fem-2.9.dev20220529/dune/fem/operator/linear/test/test-matrices.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/blockmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/blockmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/colcompspmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/colcompspmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/columnobject.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/columnobject.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/densematrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/densematrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/eigenmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/eigenmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/functor.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/functor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/istlmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/istlmatrix.hh`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         //! type of row block vector
         typedef typename RowDiscreteFunctionType :: DofStorageType  RowBlockVectorType;
 
         //! type of column block vector
         typedef typename ColDiscreteFunctionType :: DofStorageType  ColBlockVectorType;
 
         //! type of communication object
-        typedef typename RangeSpaceType :: GridType :: Traits :: Communication   CommunicationType ;
+        typedef typename RangeSpaceType :: GridType :: Traits :: CollectiveCommunication   CollectiveCommunictionType ;
 
         typedef typename BaseType :: BuildMode BuildMode ;
 
       public:
         //! constructor used by ISTLMatrixObject to build matrix in implicit mode
         ImprovedBCRSMatrix(size_type rows, size_type cols, size_type nnz, double overflowFraction) :
           BaseType (rows, cols, nnz, overflowFraction, BaseType::implicit)
@@ -131,89 +131,14 @@
         {}
 
         //! copy constructor, needed by ISTL preconditioners
         ImprovedBCRSMatrix(const ImprovedBCRSMatrix& org) :
           BaseType(org)
         {}
 
-        ConstRowIterator slicedBegin( const size_type row ) const
-        {
-          return ConstRowIterator( this->r, row );
-        }
-
-        ConstRowIterator slicedEnd( const size_type row ) const
-        {
-          return ConstRowIterator( this->r, row );
-        }
-
-        std::pair< size_type, size_type > sliceBeginEnd( const size_type thread, const size_type numThreads ) const
-        {
-          const size_type sliceSize  = this->N() / numThreads ;
-          const size_type sliceBegin = thread * sliceSize ;
-          const size_type sliceEnd   = ( thread == numThreads-1 ) ? this->N() : (sliceBegin + sliceSize) ;
-          return std::make_pair( sliceBegin, sliceEnd );
-        }
-
-      protected:
-        template <class X, class Y, bool isMV>
-        void mvThreadedImpl( const field_type& alpha,
-                             const X& x, Y& y, std::integral_constant<bool, isMV> ) const
-        {
-          auto doMV = [this, &alpha, &x, &y] ()
-          {
-            const auto slice = sliceBeginEnd( MPIManager::thread(), MPIManager::numThreads() );
-            const ConstRowIterator endi = slicedEnd( slice.second );
-            for (ConstRowIterator i = slicedBegin(slice.first); i!=endi; ++i)
-            {
-              if constexpr ( isMV )
-                y[i.index()] = 0;
-
-              ConstColIterator endj = (*i).end();
-              for (ConstColIterator j=(*i).begin(); j!=endj; ++j)
-              {
-                auto&& xj = Dune::Impl::asVector(x[j.index()]);
-                auto&& yi = Dune::Impl::asVector(y[i.index()]);
-                if constexpr ( isMV )
-                  Dune::Impl::asMatrix(*j).umv(xj, yi);
-                else
-                  Dune::Impl::asMatrix(*j).usmv(alpha, xj, yi);
-              }
-            }
-          };
-
-          try {
-            // execute in parallel
-            MPIManager :: run ( doMV );
-          }
-          catch ( const SingleThreadModeError& e )
-          {
-            // serial version
-            if constexpr ( isMV )
-              this->mv( x, y );
-            else
-            {
-              DUNE_THROW(SingleThreadModeError,"ImprovedBCRSMatrix::usmvThreaded: Cannot recover from threading error. Disable threading!");
-              // this->usmv( alpha, x, y );
-            }
-          }
-        }
-
-      public:
-        template <class X, class Y>
-        void usmvThreaded( const field_type& alpha, const X& x, Y& y ) const
-        {
-          mvThreadedImpl(alpha, x, y, std::false_type() );
-        }
-
-        template <class X, class Y>
-        void mvThreaded( const X& x, Y& y ) const
-        {
-          mvThreadedImpl(1.0, x, y, std::true_type() );
-        }
-
         template < class SparsityPattern >
         void createEntries(const SparsityPattern& sparsityPattern)
         {
           const auto spEnd = sparsityPattern.end();
 
           // insert map of indices into matrix
           auto endcreate = this->createend();
@@ -786,18 +711,18 @@
       int sequence_;
 
       mutable std::unique_ptr< MatrixType > matrix_;
 
       mutable LocalMatrixStackType localMatrixStack_;
 
       mutable std::unique_ptr< MatrixAdapterType >     matrixAdap_;
+      mutable std::unique_ptr< ColumnBlockVectorType > Arg_;
+      mutable std::unique_ptr< RowBlockVectorType >    Dest_;
       // overflow fraction for implicit build mode
       const double overflowFraction_;
-      const bool threading_ ;
-
       ISTLSolverParameter param_;
     public:
       ISTLMatrixObject(const ISTLMatrixObject&) = delete;
 
       //! constructor
       //! \param rowSpace space defining row structure
       //! \param colSpace space defining column structure
@@ -806,30 +731,27 @@
         , rangeSpace_(rangeSpace)
         , rowMapper_( rangeSpace.blockMapper() )
         , colMapper_( domainSpace.blockMapper() )
         , size_(-1)
         , sequence_(-1)
         , localMatrixStack_( *this )
         , overflowFraction_( param.overflowFraction() )
-        , threading_( param.threading() )
         , param_( param )
       {}
 
     protected:
       //! return reference to system matrix (may not be finalized)
       //! For finalized matrix use exportMatrix
       MatrixType& matrix() const
       {
         assert( matrix_ );
         return *matrix_;
       }
 
     public:
-      bool threading() const { return threading_; }
-
       void printTexInfo(std::ostream& out) const
       {
         out << "ISTL MatrixObj: ";
         out  << "\\\\ \n";
       }
 
       //! return matrix adapter object
@@ -1031,23 +953,14 @@
 
       //! apply with discrete functions
       void apply(const ColumnDiscreteFunctionType& arg, RowDiscreteFunctionType& dest) const
       {
         matrixAdapter().apply( arg.blockVector(), dest.blockVector() );
       }
 
-      //! apply with arbitrary discrete functions
-      template <class CDF, class RDF>
-      void apply(const CDF& arg, RDF& dest) const
-      {
-        // this can happen when different storages are used for discrete
-        // function and matrix/solver objects
-        DUNE_THROW(NotImplemented,"ISTLMatrixObj::apply called for DiscreteFunctions not specified in the template list");
-      }
-
       //! resort row numbering in matrix to have ascending numbering
       void resort()
       {}
 
       //! create precondition matrix does nothing because preconditioner is
       //! created only when requested
       void createPreconditionMatrix()
@@ -1233,16 +1146,28 @@
       void preConErrorMsg(int preCon) const
       {
         exit(1);
       }
 
       void removeObj ()
       {
+        Dest_.reset( nullptr );
+        Arg_.reset( nullptr );
         matrixAdap_.reset( nullptr );
       }
+
+      void createBlockVectors () const
+      {
+        if( !Arg_  )
+          Arg_.reset( new RowBlockVectorType( rowMapper_.size() ) );
+        if( !Dest_ )
+          Dest_.reset( new ColumnBlockVectorType( colMapper_.size() ) );
+
+        createMatrixAdapter ();
+      }
     };
 
   } // namespace Fem
 
 } // namespace Dune
 
 #endif // #if HAVE_DUNE_ISTL
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/istlmatrixadapter.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/istlmatrixadapter.hh`

 * *Files 8% similar despite different names*

```diff
@@ -61,32 +61,29 @@
       //! copy constructor
       ISTLParallelMatrixAdapterInterface ( const ISTLParallelMatrixAdapterInterface &org )
       : matrix_( org.matrix_ ),
         rowSpace_( org.rowSpace_ ),
         colSpace_( org.colSpace_ ),
         scp_( colSpace_ ),
         preconditioner_( org.preconditioner_ ),
-        averageCommTime_( org.averageCommTime_ ),
-        threading_( org.threading_ )
+        averageCommTime_( org.averageCommTime_ )
       {}
 
       //! constructor: just store a reference to a matrix
       //! and the spaces as well as preconditioning method
       ISTLParallelMatrixAdapterInterface ( MatrixType &matrix,
                                            const RowSpaceType &rowSpace,
                                            const ColSpaceType &colSpace,
-                                           const PreconditionAdapterType& precon,
-                                           const bool threading = true )
+                                           const PreconditionAdapterType& precon )
       : matrix_( matrix ),
         rowSpace_( rowSpace ),
         colSpace_( colSpace ),
         scp_( colSpace_ ),
         preconditioner_( precon ),
-        averageCommTime_( 0 ),
-        threading_( threading )
+        averageCommTime_( 0 )
       {}
 
       //! return communication time
       virtual double averageCommTime() const { return averageCommTime_ ; }
 
       //! return reference to preconditioner
       virtual PreconditionAdapterType &preconditionAdapter() { return preconditioner_; }
@@ -115,16 +112,17 @@
         DUNE_THROW(NotImplemented,"interface method residuum not overloaded!");
         return 0.0;
       }
 
       //! get matrix
       const MatrixType& getmat () const override { return matrix_; }
 
-      //! return true if matvec and preconditioning should use threading (depends on implementation of preconditioning)
-      bool threading () const { return threading_; }
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       void communicate( Y &y ) const
       {
         if( rowSpace_.grid().comm().size() <= 1 )
           return;
 
@@ -136,15 +134,14 @@
 
       MatrixType &matrix_;
       const RowSpaceType &rowSpace_;
       const ColSpaceType &colSpace_;
       mutable ParallelScalarProductType scp_;
       PreconditionAdapterType preconditioner_;
       mutable double averageCommTime_;
-      const bool threading_;
     };
 
     template <class MatrixImp>
     class LagrangeParallelMatrixAdapter
       : public ISTLParallelMatrixAdapterInterface< MatrixImp >
     {
       typedef LagrangeParallelMatrixAdapter< MatrixImp > ThisType;
@@ -166,15 +163,18 @@
 
       //! export types
       typedef MatrixType  matrix_type;
       typedef X domain_type;
       typedef Y range_type;
       typedef typename X::field_type field_type;
 
-      using BaseType :: threading;
+#if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      //! define the category
+      enum { category=SolverCategory::sequential };
+#endif // #if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       using BaseType :: matrix_;
       using BaseType :: scp_ ;
       using BaseType :: colSpace_ ;
       using BaseType :: rowSpace_ ;
       using BaseType :: averageCommTime_;
@@ -186,40 +186,31 @@
       {}
 
       //! constructor: just store a reference to a matrix
       //! and the spaces as well as preconditioning method
       LagrangeParallelMatrixAdapter ( MatrixType &matrix,
                                       const RowSpaceType &rowSpace,
                                       const ColSpaceType &colSpace,
-                                      const PreconditionAdapterType& precon,
-                                      const bool threading = true )
-      : BaseType( matrix, rowSpace, colSpace, precon, threading )
+                                      const PreconditionAdapterType& precon )
+      : BaseType( matrix, rowSpace, colSpace, precon )
       {}
 
       //! apply operator to x:  \f$ y = A(x) \f$
       void apply ( const X &x, Y &y ) const override
       {
-        if( threading() )
-          matrix_.mvThreaded(x, y );
-        else
-          matrix_.mv( x, y );
-
+        matrix_.mv( x, y );
         communicate( y );
       }
 
       //! apply operator to x, scale and add:  \f$ y = y + \alpha A(x) \f$
       void applyscaleadd ( field_type alpha, const X &x, Y &y) const override
       {
         if( rowSpace_.grid().comm().size() <= 1 )
         {
-          if( threading() )
-            matrix_.usmvThreaded(alpha, x, y );
-          else
-            matrix_.usmv(alpha,x,y);
-
+          matrix_.usmv(alpha,x,y);
           communicate( y );
         }
         else
         {
           Y tmp( y.size() );
           apply( x, tmp );
           y.axpy( alpha, tmp );
@@ -233,15 +224,17 @@
         this->apply(x,tmp);
         tmp -= rhs;
 
         // return global sum of residuum
         return scp_.norm(tmp);
       }
 
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
       SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       void communicate( Y &y ) const
       {
         if( rowSpace_.grid().comm().size() <= 1 )
           return;
 
@@ -275,15 +268,18 @@
 
       //! export types
       typedef MatrixType  matrix_type;
       typedef X domain_type;
       typedef Y range_type;
       typedef typename X::field_type field_type;
 
-      using BaseType :: threading;
+#if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      //! define the category
+      enum { category=SolverCategory::sequential };
+#endif // #if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       using BaseType :: matrix_;
       using BaseType :: scp_;
       using BaseType :: rowSpace_;
       using BaseType :: colSpace_;
       using BaseType :: averageCommTime_;
@@ -294,46 +290,39 @@
         : BaseType( org )
       {}
 
       //! constructor: just store a reference to a matrix
       DGParallelMatrixAdapter (MatrixType& A,
                                const RowSpaceType& rowSpace,
                                const ColSpaceType& colSpace,
-                               const PreconditionAdapterType& precon,
-                               const bool threading = true)
-        : BaseType( A, rowSpace, colSpace, precon, threading )
+                               const PreconditionAdapterType& precon )
+        : BaseType( A, rowSpace, colSpace, precon )
       {}
 
       //! apply operator to x:  \f$ y = A(x) \f$
       void apply (const X& x, Y& y) const override
       {
         // exchange data first
         communicate( x );
 
         // apply vector to matrix
-        if( threading() )
-          matrix_.mvThreaded( x, y );
-        else
-          matrix_.mv(x,y);
+        matrix_.mv(x,y);
 
         // delete non-interior
         scp_.deleteNonInterior( y );
       }
 
       //! apply operator to x, scale and add:  \f$ y = y + \alpha A(x) \f$
       void applyscaleadd (field_type alpha, const X& x, Y& y) const override
       {
         // exchange data first
         communicate( x );
 
         // apply matrix
-        if( threading() )
-          matrix_.usmvThreaded(alpha, x, y );
-        else
-          matrix_.usmv(alpha,x,y);
+        matrix_.usmv(alpha,x,y);
 
         // delete non-interior
         scp_.deleteNonInterior( y );
       }
 
       double residuum(const Y& rhs, X& x) const override
       {
@@ -378,15 +367,17 @@
         }
 
         res = rowSpace_.grid().comm().sum( res );
         // return global sum of residuum
         return std::sqrt( res );
       }
 
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
       SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       void communicate(const X& x) const
       {
         if( rowSpace_.grid().comm().size() <= 1 ) return ;
 
         Dune::Timer commTime;
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/istlpreconditioner.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/istlpreconditioner.hh`

 * *Files 1% similar despite different names*

```diff
@@ -204,41 +204,16 @@
       }
 
       // Implementation of SOR and Jacobi's method
       // Note: for SOR we have xnew == xold
       void forwardIterate (const M& A, X& xnew, const X& xold, const Y& b, const field_type& w,
                            const DiagonalType& diagInv ) const
       {
-        bool runParallel = threading_ && (&xnew != &xold); // Jacobi only
-
-        if( runParallel )
-        {
-          auto doIterate = [this, &A, &xnew, &xold, &b, &w, &diagInv] ()
-          {
-            const auto slice = A.sliceBeginEnd( MPIManager::thread(), MPIManager::numThreads() );
-            // standard forwards iteration
-            iterate( A, xnew, xold, b, w, diagInv,
-                     A.slicedBegin( slice.first ), A.slicedEnd( slice.second ), std::true_type() );
-          };
-
-          try {
-            // execute in parallel
-            MPIManager :: run ( doIterate );
-          }
-          catch ( const SingleThreadModeError& e )
-          {
-            runParallel = false;
-          }
-        }
-
-        if( ! runParallel )
-        {
-          // serial version
-          iterate( A, xnew, xold, b, w, diagInv, A.begin(), A.end(), std::true_type() );
-        }
+        // standard forwards iteration
+        iterate( A, xnew, xold, b, w, diagInv, A.begin(), A.end(), std::true_type() );
       }
 
       // Implementation of SOR and Jacobi's method
       // Note: for SOR we have xnew == xold
       void backwardIterate (const M& A, X& xnew, const X& xold, const Y& b, const field_type& w,
                             const DiagonalType& diagInv ) const
       {
@@ -250,22 +225,19 @@
       const MatrixObject& mObj_;
       const MatrixType& _A_;
       const int _n;
       const double _w;
 
       DiagonalType diagonalInv_;
 
-      const bool threading_;
-
     public:
       ParallelIterative( const MatrixObject& mObj, int n=1, double relax=1.0  )
         : mObj_( mObj ),
           _A_( mObj.exportMatrix() ),
-          _n( n ), _w(relax),
-          threading_( mObj.threading()  )
+          _n( n ), _w(relax)
       {
         Dune::CheckIfDiagonalPresent<MatrixType,l>::check(_A_);
 
         const auto& space = mObj_.domainSpace();
         if( space.continuous() )
         {
           // only communicate diagonal if matrix blocks are small
@@ -436,21 +408,21 @@
       typedef MatrixImp MatrixType;
       typedef typename MatrixType :: RowBlockVectorType X;
       typedef typename MatrixType :: ColBlockVectorType Y;
 
       // use BCRSMatrix type because of specializations in dune-istl
       typedef typename MatrixType :: BaseType ISTLMatrixType ;
 
-      typedef typename MatrixType :: CommunicationType
-        CommunicationType;
+      typedef typename MatrixType :: CollectiveCommunictionType
+        CollectiveCommunictionType;
 
       // matrix adapter for AMG
   //#if HAVE_MPI
   //    typedef Dune::OverlappingSchwarzOperator<
-  //     ISTLMatrixType, X, Y, CommunicationType> OperatorType ;
+  //     ISTLMatrixType, X, Y, CollectiveCommunictionType> OperatorType ;
   //#else
       typedef MatrixAdapter< ISTLMatrixType, X, Y > OperatorType;
   //#endif
       mutable std::shared_ptr< OperatorType > op_;
 
       // auto pointer to preconditioning object
       typedef Preconditioner<X,Y> PreconditionerInterfaceType;
@@ -542,15 +514,15 @@
       //! create preconditioner of given type
       template <class PreconditionerType>
       PreconditionerWrapper(MatrixType & matrix,
                             int iter,
                             field_type relax,
                             bool verbose,
                             const PreconditionerType* p ,
-                            const CommunicationType& comm)
+                            const CollectiveCommunictionType& comm)
   //#if HAVE_MPI
   //      : op_( new OperatorType( matrix, comm ) )
   //#else
         : op_( new OperatorType( matrix ) )
   //#endif
         , preconder_( createAMGPreconditioner(comm, iter, relax, p) )
         , preEx_( 2 )
@@ -601,15 +573,15 @@
       {
         return (preconder_ ? preconder_->category() : SolverCategory::sequential);
       }
 
     protected:
       template <class Smoother>
       PreconditionerInterfaceType*
-      createAMGPreconditioner(const CommunicationType& comm,
+      createAMGPreconditioner(const CollectiveCommunictionType& comm,
                 int iter, field_type relax, const Smoother* )
       {
         typedef typename Dune::FieldTraits< field_type>::real_type real_type;
         typedef typename std::conditional< std::is_convertible<field_type,real_type>::value,
                          Dune::Amg::FirstDiagonal, Dune::Amg::RowSum >::type Norm;
         typedef Dune::Amg::CoarsenCriterion<
                 Dune::Amg::UnSymmetricCriterion<ISTLMatrixType, Norm > > Criterion;
@@ -694,16 +666,15 @@
       static MatrixAdapterType*
       matrixAdapterObject( const MatrixObjectType& matrixObj,
                            const MatrixAdapterType*,
                            const ISTLSolverParameter& param )
       {
         typedef typename MatrixAdapterType :: PreconditionAdapterType PreConType;
         return new MatrixAdapterType( matrixObj.exportMatrix(),
-                                      matrixObj.domainSpace(), matrixObj.rangeSpace(), PreConType(param.verbose()),
-                                      matrixObj.threading() );
+                                      matrixObj.domainSpace(), matrixObj.rangeSpace(), PreConType(param.verbose()) );
       }
 
     };
 
 #ifndef DISABLE_ISTL_PRECONDITIONING
     //! Specialization for domain space == range space
     template < class Space, class DomainBlock, class RangeBlock,
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/matrix/spmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/matrix/spmatrix.hh`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,22 @@
       static const size_type defaultCol = std::numeric_limits<size_type>::max();
       static const size_type zeroCol    = std::numeric_limits<size_type>::max()-1;
       static const int firstCol = 0;
 
       SparseRowMatrix(const ThisType& ) = delete;
 
       //! construct matrix of zero size
-      explicit SparseRowMatrix( const bool threading = true ) :
-        values_(0), columns_(0), rows_(0), dim_({{0,0}}), maxNzPerRow_(0), compressed_( false ), threading_( threading )
+      explicit SparseRowMatrix() :
+        values_(0), columns_(0), rows_(0), dim_({{0,0}}), maxNzPerRow_(0), compressed_( false )
       {}
 
       //! construct matrix with 'rows' rows and 'cols' columns,
       //! maximum 'nz' non zero values in each row
-      SparseRowMatrix(const size_type rows, const size_type cols, const size_type nz, const bool threading = true ) :
-        values_(0), columns_(0), rows_(0), dim_({{0,0}}), maxNzPerRow_(0), compressed_( false ), threading_( threading )
+      SparseRowMatrix(const size_type rows, const size_type cols, const size_type nz) :
+        values_(0), columns_(0), rows_(0), dim_({{0,0}}), maxNzPerRow_(0), compressed_( false )
       {
         reserve(rows,cols,nz);
       }
 
       //! reserve memory for given rows, columns and number of non zeros
       void reserve(const size_type rows, const size_type cols, const size_type nz)
       {
@@ -143,63 +143,34 @@
         columns_[ column ] = col;
       }
 
       //! ret = A*f
       template<class ArgDFType, class DestDFType>
       void apply(const ArgDFType& f, DestDFType& ret ) const
       {
-        bool runParallel = threading_;
+        constexpr auto blockSize = ArgDFType::DiscreteFunctionSpaceType::localBlockSize;
+        auto ret_it = ret.dbegin();
 
-        auto doApply = [this, &f, &ret]()
+        for(size_type row = 0; row<dim_[0]; ++row)
         {
-          constexpr auto blockSize = ArgDFType::DiscreteFunctionSpaceType::localBlockSize;
-
-          // compute slice of rows to be worked on
-          const auto slice = sliceBeginEnd( MPIManager::thread(), MPIManager::numThreads(), std::true_type() );
-
-          // same as begin just with a row not necessarily zero
-          auto ret_it = ret.dofVector().find( slice.first );
-
-          const auto& fDofVec = f.dofVector();
-          for(size_type row = slice.first; row<slice.second; ++row)
+          const size_type endrow = endRow( row );
+          (*ret_it) = 0.0;
+          for(size_type col = startRow( row ); col<endrow; ++col)
           {
-            const size_type endrow = endRow( row );
-            (*ret_it) = 0.0;
-            for(size_type col = startRow( row ); col<endrow; ++col)
-            {
-              const auto realCol = columns_[ col ];
-
-              if( ! compressed_ && ((realCol == defaultCol) || (realCol == zeroCol)) )
-                continue;
-
-              const auto blockNr = realCol / blockSize ;
-              const auto dofNr   = realCol % blockSize ;
-              (*ret_it) += values_[ col ] * fDofVec[ blockNr ][ dofNr ];
-            }
+            const auto realCol = columns_[ col ];
 
-            ++ret_it;
-          }
-        };
+            if( ! compressed_ && ((realCol == defaultCol) || (realCol == zeroCol)) )
+              continue;
 
-        if( runParallel )
-        {
-          try {
-            // execute in parallel
-            MPIManager :: run ( doApply );
-          }
-          catch ( const SingleThreadModeError& e )
-          {
-            runParallel = false;
+            const auto blockNr = realCol / blockSize ;
+            const auto dofNr   = realCol % blockSize ;
+            (*ret_it) += values_[ col ] * f.dofVector()[ blockNr ][ dofNr ];
           }
-        }
 
-        // run serial if threading disabled or something else went wrong
-        if( ! runParallel )
-        {
-          doApply();
+          ++ret_it;
         }
       }
 
       //! return value of entry (row,col)
       field_type get(const size_type row, const size_type col) const
       {
         assert((col>=0) && (col < dim_[1]));
@@ -369,88 +340,46 @@
         return std::tie(values_,columns_,rows_);
       }
 
       //! Apply Jacobi/SOR method
       template<class DiagType, class ArgDFType, class DestDFType, class WType>
       void forwardIterative(const DiagType& diagInv, const ArgDFType& b, const DestDFType& xold, DestDFType& xnew, const WType& w ) const
       {
-        parallelIterative(diagInv, b, xold, xnew, w, std::true_type() );
+        parallelIterative( diagInv.dofVector().begin(),
+                           b.dofVector().begin(),
+                           xold,
+                           xnew.dofVector().begin(),
+                           w,
+                           0,         // row begin
+                           dim_[ 0 ], // row end
+                           std::true_type() );
       }
 
       //! Apply Jacobi/SOR method
       template<class DiagType, class ArgDFType, class DestDFType, class WType>
       void backwardIterative(const DiagType& diagInv, const ArgDFType& b, const DestDFType& xold, DestDFType& xnew, const WType& w ) const
       {
-        parallelIterative(diagInv, b, xold, xnew, w, std::false_type() );
+        parallelIterative( diagInv.dofVector().beforeEnd(),
+                           b.dofVector().beforeEnd(),
+                           xold,
+                           xnew.dofVector().beforeEnd(),
+                           w,
+                           dim_[ 0 ] - 1, // row beforeEnd
+                           size_type(-1), // row beforeBegin
+                           std::false_type() );
       }
 
     protected:
-      // return slice of rows for given thread in forward direction
-      std::pair< size_type, size_type > sliceBeginEnd(const size_type thread,  const size_type numThreads, std::true_type ) const
-      {
-        const size_type sliceSize  = this->rows() / numThreads;
-        const size_type sliceBegin = (thread * sliceSize) ;
-        const size_type sliceEnd   = (thread == numThreads-1 ) ? this->rows(): (sliceBegin + sliceSize);
-        return std::make_pair( sliceBegin, sliceEnd );
-      }
-
-      // return slice of rows for given thread in backward direction
-      std::pair< size_type, size_type > sliceBeginEnd(const size_type thread, const size_type numThreads, std::false_type ) const
-      {
-        std::pair< size_type, size_type > beginEnd = sliceBeginEnd( thread, numThreads, std::true_type() );
-        return std::make_pair( beginEnd.second-1, beginEnd.first-1 );
-      }
-
-      template<class DiagType, class ArgDFType, class DestDFType, class WType, bool forward >
-      void parallelIterative(const DiagType& diagInv, const ArgDFType& b, const DestDFType& xold, DestDFType& xnew,
-                             const WType& w, std::integral_constant<bool, forward> direction ) const
-      {
-        bool runParallel = threading_ && (&xold != &xnew) ; // only for Jacobi
-
-        auto doIterate = [this, &diagInv, &b, &xold, &xnew, &w, &direction] ()
-        {
-          // compute slice to be worked on depending on direction
-          const auto slice = sliceBeginEnd( MPIManager::thread(), MPIManager::numThreads(), direction );
-
-          doParallelIterative( diagInv.dofVector().find( slice.first ), // still O(1) operation just like for begin()
-                               b.dofVector().find( slice.first ),
-                               xold,
-                               xnew.dofVector().find( slice.first ),
-                               w,
-                               slice.first, // row begin
-                               slice.second,   // row end
-                               direction );
-        };
-
-        if( runParallel )
-        {
-          try {
-            // execute in parallel
-            MPIManager :: run ( doIterate );
-          }
-          catch ( const SingleThreadModeError& e )
-          {
-            runParallel = false;
-          }
-        }
-
-        // run serial if threading disabled or something else went wrong
-        if( ! runParallel )
-        {
-          doIterate();
-        }
-      }
-
       //! Apply Jacobi/SOR method
       template<class DiagIt, class ArgDFIt, class DestDFType, class DestDFIt,
                class WType, bool forward>
-      void doParallelIterative(DiagIt diag, ArgDFIt bit, const DestDFType& xold, DestDFIt xit,
-                               const WType& w,
-                               size_type row, const size_type end,
-                               std::integral_constant<bool, forward> ) const
+      void parallelIterative(DiagIt diag, ArgDFIt bit, const DestDFType& xold, DestDFIt xit,
+                             const WType& w,
+                             size_type row, const size_type end,
+                             std::integral_constant<bool, forward> ) const
       {
         constexpr auto blockSize = DestDFType::DiscreteFunctionSpaceType::localBlockSize;
 
         const auto nextRow = [&diag, &xit, &bit](size_type &row)
         {
           if constexpr ( forward )
           {
@@ -458,15 +387,14 @@
           }
           else
           {
             --diag; --xit; --bit; --row;
           }
         };
 
-        const auto& xOldVec = xold.dofVector();
         for(; row != end; nextRow(row))
         {
           auto rhs = (*bit);
 
           const size_type endrow = endRow( row );
           for(size_type col = startRow( row ); col<endrow; ++col)
           {
@@ -474,15 +402,15 @@
 
             if( (realCol == row ) || (! compressed_ && ((realCol == defaultCol) || (realCol == zeroCol))) )
               continue;
 
             const auto blockNr = realCol / blockSize ;
             const auto dofNr   = realCol % blockSize ;
 
-            rhs -= values_[ col ] * xOldVec[ blockNr ][ dofNr ] ;
+            rhs -= values_[ col ] * xold.dofVector()[ blockNr ][ dofNr ] ;
           }
 
           (*xit) = w * (rhs * (*diag));
         }
       }
       //! resize matrix
       void resize(size_type rows, size_type cols, size_type nz)
@@ -563,15 +491,14 @@
       ValuesVector  values_;
       IndicesVector columns_;
       IndicesVector rows_;
 
       std::array<size_type,2> dim_;
       size_type maxNzPerRow_;
       bool compressed_;
-      const bool threading_;
     };
 
 
 
     //! SparseRowMatrixObject
     template< class DomainSpace, class RangeSpace,
               class Matrix = SparseRowMatrix< typename DomainSpace::RangeFieldType > >
@@ -621,15 +548,15 @@
                              const RangeSpaceType &rangeSpace,
                              const SolverParameter& param = SolverParameter() )
       : domainSpace_( domainSpace ),
         rangeSpace_( rangeSpace ),
         domainMapper_( domainSpace_.blockMapper() ),
         rangeMapper_( rangeSpace_.blockMapper() ),
         sequence_( -1 ),
-        matrix_( param.threading() ),
+        matrix_(),
         localMatrixStack_( *this )
       {}
 
       //! get domain space (i.e. space that builds the rows)
       const DomainSpaceType& domainSpace() const
       {
         return domainSpace_;
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/dgl2projection.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/dgl2projection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/hdivprojection.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/hdivprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/local/l2projection.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/l2projection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/dense.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/dense.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/localrieszprojection.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/localrieszprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/local/riesz/orthonormal.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/local/riesz/orthonormal.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/projection/vtxprojection.hh` & `dune-fem-2.9.dev20220529/dune/fem/operator/projection/vtxprojection.hh`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         typedef typename DiscreteFunction::GridPartType GridPartType;
 
         typedef typename GridPartType::IntersectionType IntersectionType;
         typedef typename GridPartType::template Codim< 0 >::EntityType EntityType;
         typedef typename DiscreteFunction::DiscreteFunctionSpaceType
           DiscreteFunctionSpaceType;
 
-        if( u.space().gridPart().isConforming() || !Fem::GridPartCapabilities::hasGrid< GridPartType >::v )
+        if( GridPartType::Traits::conforming || !Fem::GridPartCapabilities::hasGrid< GridPartType >::v )
           return;
 
         const auto &blockMapper = u.space().blockMapper();
 
         std::vector< typename DiscreteFunction::DofType > ldu, ldw;
         const std::size_t localBlockSize = DiscreteFunctionSpaceType::localBlockSize;
         const std::size_t maxNumBlocks = blockMapper.maxNumDofs();
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/operator/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/operator/test/unitrows.cc` & `dune-fem-2.9.dev20220529/dune/fem/operator/test/unitrows.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/agglomerationquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/agglomerationquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/cacheprovider.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/cacheprovider.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/cacheprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/cacheprovider.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/pointmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/pointmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/pointprovider.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/pointprovider.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/pointprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/pointprovider.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/registry.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/registry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/cache_test.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/cache_test.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/point_test.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/point_test.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/test/twist_test.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/test/twist_test.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/topology.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/topology.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/topology.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/topology.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistprovider.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistprovider.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistprovider.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistutility.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistutility.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/caching/twistutility.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/caching/twistutility.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/cachingpointlist.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/cachingpointlist.hh`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,15 @@
        */
       CachingPointList ( const GridPartType &gridPart,
                          const IntersectionType &intersection,
                          const QuadratureKeyType& quadKey, const typename Base :: Side side )
         : Base( getPointList( intersection, quadKey, side ) ),
           twist_( getTwist( gridPart, intersection, side ) ),
           mapper_( CacheProviderType::getMapper( quadImp(), elementGeometry(), localFaceIndex(), twist_) ),
-          points_( PointProviderType::getPoints( quadImp().ipList().id(), elementGeometry() ) ),
-          intersection_(intersection)
+          points_( PointProviderType::getPoints( quadImp().ipList().id(), elementGeometry() ) )
       {
       }
 
       const QuadraturePointWrapperType operator[] ( const size_t i ) const
       {
         return QuadraturePointWrapperType( *this, i );
       }
@@ -284,19 +283,14 @@
       /** \copydoc Dune::Fem::IntegrationPointList::point
        */
       const CoordinateType &point ( const size_t i ) const
       {
         return points_[ cachingPoint( i ) ];
       }
 
-      const IntersectionType &intersection() const
-      {
-        return intersection_;
-      }
-
       /** \copydoc Dune::Fem::CachingInterface::twisted */
       static constexpr bool twisted() { return true; }
 
       /** \copydoc Dune::Fem::CachingInterface::twistId */
       inline int twistId () const { return twist_ + 4; }
 
       /** \copydoc Dune::Fem::CachingInterface::cachingPoint */
@@ -375,15 +369,14 @@
         }
       }
 
     private:
       const int twist_;
       const MapperPairType &mapper_;
       const PointVectorType &points_;
-      const IntersectionType &intersection_;
     };
 
   } //namespace Fem
 
 } //namespace Dune
 
 #endif // #ifndef DUNE_FEM_CACHINGPOINTLIST_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/cachingquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/cachingquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/cornerpointset.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/cornerpointset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/defaultquadratures.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/defaultquadratures.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/dunequadratures.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/dunequadratures.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/elementpointlist.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/elementpointlist.hh`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,15 @@
        *        a cube (otherwise elementGeometry() returns a wrong geometry).
        */
       ElementIntegrationPointList ( const GridPartType &gridPart,
                                     const IntersectionType &intersection,
                                     const QuadratureKeyType& quadKey,
                                     const typename Base :: Side side )
       : Base( getPointList( intersection, quadKey, side ) ),
-        referenceGeometry_( side == Base::INSIDE ?  intersection.geometryInInside() : intersection.geometryInOutside()),
-        intersection_(intersection)
+        referenceGeometry_( side == Base::INSIDE ? intersection.geometryInInside() : intersection.geometryInOutside() )
       {}
 
       const QuadraturePointWrapperType operator[] ( size_t i ) const
       {
         return QuadraturePointWrapperType( *this, i );
       }
 
@@ -182,18 +181,14 @@
       {
         dummy_ = referenceGeometry_.global( localPoint( i ) );
         return dummy_;
       }
 
       using Base::localFaceIndex;
 
-      const IntersectionType &intersection() const
-      {
-        return intersection_;
-      }
     protected:
       Base getPointList ( const IntersectionType &intersection, const int order,
                           const typename Base :: Side side )
       {
         switch( side )
         {
           case Base :: INSIDE:
@@ -209,15 +204,14 @@
         }
       }
 
     private:
       typedef typename IntersectionIteratorType::Intersection::LocalGeometry ReferenceGeometry;
 
       ReferenceGeometry referenceGeometry_;
-      const IntersectionType &intersection_;
       mutable CoordinateType dummy_;
     };
 
   } // namespace Fem
 
 } // namespace Dune
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/elementpointlistbase.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/elementpointlistbase.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/elementquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/elementquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/femquadratures.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/femquadratures.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/femquadratures_inline.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/femquadratures_inline.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/gausspoints.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/gausspoints.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/gausspoints_implementation.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/gausspoints_implementation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/gausslegendre.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/gausslegendre.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/geometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/geometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/geometric/quadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/geometric/quadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/idprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/idprovider.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/integrator.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/integrator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/interpolationquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/interpolationquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/intersectionquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/intersectionquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/lumpingquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/lumpingquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature0d.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature0d.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature1d.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature1d.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature2d.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature2d.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/pardgsimplexquadrature3d.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/pardgsimplexquadrature3d.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/pyramidpoints.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/pyramidpoints.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/quadprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/quadprovider.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/quadrature.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/quadrature.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/quadratureimp.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/quadratureimp.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/quadratureimp_inline.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/quadratureimp_inline.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/3dcubesimp.dgf` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/3dcubesimp.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/agglomerationquadrature.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/agglomerationquadrature.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/cachingquadrature.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/cachingquadrature.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/checkleafcodim1.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/checkleafcodim1.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/elementquadrature.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/elementquadrature.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/quad_test.cc` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/quad_test.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/quadrature/test/quad_test.hh` & `dune-fem-2.9.dev20220529/dune/fem/quadrature/test/quad_test.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/conservationlawmodel.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/conservationlawmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/dgelliptic.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/dgelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/dgfemscheme.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/dgfemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/diffusionmodel.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/diffusionmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/dirichletconstraints.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/dirichletconstraints.hh`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,14 @@
       if( intersection.boundary() )
       {
         // get dirichlet information from model
         DirichletBlock block;
         block.fill(0);
         std::array<int,dimRange> dblock;
 
-        model.init(intersection);
         const bool isDirichletIntersection = model.isDirichletIntersection( intersection, dblock );
         if (isDirichletIntersection)
         {
           for ( unsigned int i=0;i<localBlockSize;++i)
             block[i] = dblock[i];
           // get face number of boundary intersection
           const int face = intersection.indexInInside();
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/dirichletwrapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/dirichletwrapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/elliptic.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/femscheme.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/galerkin.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/galerkin.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/integrands.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/integrands.hh`

 * *Files 0% similar despite different names*

```diff
@@ -388,18 +388,18 @@
       using RRangeType = typename detail::GetDimRange<std::tuple_element_t<0,RangeValueType>>::type;
       typedef std::array<int,RRangeType::dimension> DirichletComponentType;
       typedef typename EntityType::Geometry::LocalCoordinate DomainType;
 
     private:
       typedef typename EntityType::Geometry::LocalCoordinate LocalCoordinateType;
 
-      typedef FemPy::CachingPoint< GridPart, LocalCoordinateType, 0 > InteriorCachingPointType;
-      typedef FemPy::ElementPoint< GridPart, LocalCoordinateType, 0 > InteriorElementPointType;
-      typedef FemPy::CachingPoint< GridPart, LocalCoordinateType, 1 > SurfaceCachingPointType;
-      typedef FemPy::ElementPoint< GridPart, LocalCoordinateType, 1 > SurfaceElementPointType;
+      typedef FemPy::CachingPoint< LocalCoordinateType, 0 > InteriorCachingPointType;
+      typedef FemPy::ElementPoint< LocalCoordinateType, 0 > InteriorElementPointType;
+      typedef FemPy::CachingPoint< LocalCoordinateType, 1 > SurfaceCachingPointType;
+      typedef FemPy::ElementPoint< LocalCoordinateType, 1 > SurfaceElementPointType;
 
       template< class QP >
       static Fem::QuadraturePointWrapper< QP > asQP ( const QP &qp )
       {
         return static_cast< Fem::QuadraturePointWrapper< QP > >( qp );
       }
 
@@ -438,15 +438,15 @@
 
         virtual bool hasDirichletBoundary () const = 0;
         virtual bool isDirichletIntersection( const IntersectionType& inter, DirichletComponentType &dirichletComponent ) const = 0;
         virtual void dirichlet( int bndId, const DomainType &x,RRangeType &value) const = 0;
       };
 
       template< class Impl >
-      struct DUNE_PRIVATE Implementation final
+      struct Implementation final
         : public Interface
       {
         Implementation ( Impl impl ) : impl_( std::move( impl ) )
         {
         }
         virtual Interface *clone () const override { return new Implementation( *this ); }
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/linearized.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/linearized.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/schemes/molgalerkin.hh` & `dune-fem-2.9.dev20220529/dune/fem/schemes/molgalerkin.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/solver/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/amgistl.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/amgistl.hh`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         typedef int GlobalLookupIndexSet;
 
         explicit FemCommunication ( const DiscreteFunctionSpaceType &dfSpace,  Dune::SolverCategory::Category solverCategory = Dune::SolverCategory::sequential )
           : dfSpace_( dfSpace ), solverCategory_( solverCategory )
         {}
 
-        const typename DiscreteFunctionSpace::GridPartType::CommunicationType &communicator () const { return dfSpace_.gridPart().comm(); }
+        const typename DiscreteFunctionSpace::GridPartType::CollectiveCommunicationType &communicator () const { return dfSpace_.gridPart().comm(); }
 
         template< class T >
         void copyOwnerToAll ( const T &x, T &y ) const
         {
           y = x;
           typedef Dune::Fem::HierarchicalDiscreteFunction< DiscreteFunctionSpaceType > DiscreteFunctionType;
           DiscreteFunctionType z( "", dfSpace_, reinterpret_cast< typename DiscreteFunctionType::DofVectorType & >( y ) );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/amgxsolver.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/amgxsolver.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/cginverseoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/cginverseoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/communication/fem.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/communication/fem.hh`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
       public:
         typedef DiscreteFunctionSpace DiscreteFunctionSpaceType;
 
         explicit FemCommunication ( const DiscreteFunctionSpaceType &dfSpace,  Dune::SolverCategory::Category solverCategory = Dune::SolverCategory::sequential )
           : dfSpace_( dfSpace ), solverCategory_( solverCategory )
         {}
 
-        const typename DiscreteFunctionSpace::GridPartType::CommunicationType &communicator () const { return dfSpace_.gridPart().comm(); }
+        const typename DiscreteFunctionSpace::GridPartType::CollectiveCommunicationType &communicator () const { return dfSpace_.gridPart().comm(); }
 
         template< class T >
         void copyOwnerToAll ( const T &x, T &y ) const
         {
           y = x;
           project( y );
           FemCommunicationVector< DiscreteFunctionSpaceType, T > z( dfSpace_, y );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/communication/hierarchical.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/communication/hierarchical.hh`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
       public:
         typedef DiscreteFunctionSpace DiscreteFunctionSpaceType;
 
         explicit HierarchicalCommunication ( const DiscreteFunctionSpaceType &dfSpace,  Dune::SolverCategory::Category solverCategory = Dune::SolverCategory::sequential )
           : dfSpace_( dfSpace ), solverCategory_( solverCategory )
         {}
 
-        const typename DiscreteFunctionSpace::GridPartType::CommunicationType &communicator () const { return dfSpace_.gridPart().comm(); }
+        const typename DiscreteFunctionSpace::GridPartType::CollectiveCommunicationType &communicator () const { return dfSpace_.gridPart().comm(); }
 
         template< class T >
         void copyOwnerToAll ( const T &x, T &y ) const
         {
           y = x;
           project( y );
           HierarchicalCommunicationVector< DiscreteFunctionSpaceType, T > z( dfSpace_, y );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/communication/owneroverlapcopy.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/communication/owneroverlapcopy.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/diagonalpreconditioner.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/diagonalpreconditioner.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/eigen.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/eigen.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/fempreconditioning.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/fempreconditioning.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/inverseoperatorinterface.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/inverseoperatorinterface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/istl.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/istl.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/istlinverseoperators.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/istlinverseoperators.hh`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
       typedef ISTLPreconditionAdapter< Preconditioner > ThisType;
       typedef Dune::Preconditioner< typename Preconditioner::RangeFunctionType::DofStorageType, typename Preconditioner::DomainFunctionType::DofStorageType > BaseType;
 
       typedef typename Preconditioner::DomainFunctionType DomainFunctionType;
       typedef typename Preconditioner::RangeFunctionType  RangeFunctionType;
 
     public:
+#if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      enum {category=SolverCategory::sequential};
+#endif // #if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+
       typedef typename BaseType::domain_type domain_type;
       typedef typename BaseType::range_type  range_type;
       typedef typename BaseType::field_type  field_type;
 
       typedef typename DomainFunctionType::DiscreteFunctionSpaceType DomainFunctionSpaceType;
       typedef typename RangeFunctionType::DiscreteFunctionSpaceType  RangeFunctionSpaceType;
 
@@ -69,15 +73,17 @@
           RangeFunctionType px( "ISTLPreconditionAdapter::apply::x", rangeSpace_, x );
           DomainFunctionType py( "ISTLPreconditionAdapter::apply::y", domainSpace_, y );
 
           (*precon_)( px, py );
         }
       }
 
-      SolverCategory::Category category () const { return SolverCategory::sequential; }
+#if DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
+      SolverCategory::Category category () const override { return SolverCategory::sequential; }
+#endif // #if ! DUNE_VERSION_NEWER(DUNE_ISTL, 2, 6)
 
     protected:
       const Preconditioner *precon_;
       const DomainFunctionSpaceType &domainSpace_;
       const RangeFunctionSpaceType &rangeSpace_;
     };
 
@@ -249,16 +255,16 @@
     template< class DiscreteFunction, int method, class Preconditioner >
     struct ISTLInverseOperatorTraits
     {
       typedef DiscreteFunction  DiscreteFunctionType;
       typedef Operator< DiscreteFunction, DiscreteFunction > OperatorType;
       typedef Preconditioner PreconditionerType;
 
-      typedef ISTLBlockVectorDiscreteFunction< typename DiscreteFunction::DiscreteFunctionSpaceType > SolverDiscreteFunctionType ;
       typedef Dune::Fem::ISTLLinearOperator< DiscreteFunction, DiscreteFunction > AssembledOperatorType;
+      typedef ISTLBlockVectorDiscreteFunction< typename DiscreteFunction::DiscreteFunctionSpaceType > SolverDiscreteFunctionType ;
 
       typedef ISTLInverseOperator< DiscreteFunction, method, Preconditioner >  InverseOperatorType;
       typedef ISTLSolverParameter SolverParameterType;
     };
 
     template< class DiscreteFunction, int method, class Preconditioner >
     class ISTLInverseOperator : public InverseOperatorInterface<
@@ -278,22 +284,22 @@
 
       using BaseType :: bind;
       using BaseType :: unbind;
       using BaseType :: setMaxIterations;
       using BaseType :: setMaxLinearIterations;
 
     protected:
-      typedef typename Traits::SolverDiscreteFunctionType       SolverDiscreteFunctionType;
-
       typedef typename DomainFunctionType :: DiscreteFunctionSpaceType
         DiscreteFunctionSpaceType;
 
+      typedef ISTLLinearOperatorAdapter< OperatorType >         ISTLOperatorType;
+      typedef ISTLPreconditionAdapter< PreconditionerType >     ISTLPreconditionerAdapterType;
 
-      typedef typename SolverDiscreteFunctionType::ScalarProductType   ParallelScalarProductType;
-      typedef typename SolverDiscreteFunctionType::DofStorageType      BlockVectorType;
+      typedef typename RangeFunctionType :: ScalarProductType   ParallelScalarProductType;
+      typedef typename RangeFunctionType::DofStorageType        BlockVectorType;
 
       typedef ISTLSolverAdapter< method, BlockVectorType > SolverAdapterType;
       typedef typename SolverAdapterType::ReductionType ReductionType;
     public:
 
       //non-deprecated constructors
       ISTLInverseOperator ( const ISTLSolverParameter & parameter = ISTLSolverParameter() )
@@ -313,61 +319,50 @@
       {
         bind( op, preconditioner );
       }
 
     protected:
       // apply for arbitrary domain function type and matching range function type
       template <class DomainFunction>
-      int apply( const DomainFunction& u, SolverDiscreteFunctionType& w ) const
+      int apply( const DomainFunction& u, RangeFunctionType& w ) const
       {
         auto& scp = w.scalarProduct();
         // u may not be a discrete function, therefore use w.space()
         const DiscreteFunctionSpaceType& space = w.space();
-
-        typedef Dune::Preconditioner< BlockVectorType, BlockVectorType > ISTLPreconditionerType;
-        std::shared_ptr< ISTLPreconditionerType > istlPre;
-        if constexpr (std::is_same< SolverDiscreteFunctionType, RangeFunctionType >::value )
-        {
-          typedef ISTLPreconditionAdapter< PreconditionerType > ISTLPreconditionerAdapterType;
-          istlPre.reset( new ISTLPreconditionerAdapterType( preconditioner_, space, space ) );
-        }
+        ISTLPreconditionerAdapterType istlPreconditioner( preconditioner_, space, space );
 
         if( assembledOperator_ )
         {
           auto& matrix = assembledOperator_->matrixAdapter( *(solverAdapter_.parameter()) );
           // if preconditioner_ was set use that one, otherwise the one from the matrix object
-          ISTLPreconditionerType& matrixPre = matrix.preconditionAdapter();
-          ISTLPreconditionerType& precon    = ( preconditioner_ ) ? (*istlPre) : matrixPre;
+          typedef Dune::Preconditioner< BlockVectorType, BlockVectorType > PreconditionerType;
+          PreconditionerType& matrixPre = matrix.preconditionAdapter();
+          PreconditionerType& istlPre   = istlPreconditioner;
+          PreconditionerType& precon    = ( preconditioner_ ) ? istlPre : matrixPre;
           return solve( matrix, scp, precon, u, w );
         }
-
-        if constexpr (std::is_same< SolverDiscreteFunctionType, RangeFunctionType >::value )
+        else
         {
           assert( operator_ );
-          assert( istlPre );
-          typedef ISTLLinearOperatorAdapter< OperatorType >  ISTLOperatorType;
           ISTLOperatorType istlOperator( *operator_, space, space );
-          return solve( istlOperator, scp, *istlPre, u, w );
+          return solve( istlOperator, scp, istlPreconditioner, u, w );
         }
-
-        DUNE_THROW(InvalidStateException,"ISTLInverseOperator::apply: No valid operator found!");
-        return -1;
       }
 
       //! final solve execution only copying the right hand side
       template< class OperatorAdapter, class ISTLPreconditioner, class DomainFunction >
       int solve ( OperatorAdapter &istlOperator, ParallelScalarProductType &scp,
                   ISTLPreconditioner &preconditioner,
                   const DomainFunction& u,
-                  SolverDiscreteFunctionType& w ) const
+                  RangeFunctionType& w ) const
       {
         if( ! rhs_ )
         {
           // u may not be a discrete function, therefore use w.space()
-          rhs_.reset( new SolverDiscreteFunctionType( "ISTLInvOp::rhs", w.space() ) );
+          rhs_.reset( new DomainFunctionType( "ISTLInvOp::rhs", w.space() ) );
           rightHandSideCopied_ = false;
         }
 
         if( ! rightHandSideCopied_ )
         {
           // copy right hand side since ISTL solvers seem to modify it
           rhs_->assign( u );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/krylovinverseoperators.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/krylovinverseoperators.hh`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
       KrylovInverseOperator ( const SolverParameter &parameter = SolverParameter(Parameter::container()) )
       : BaseType( parameter ),
         precondObj_(),
         verbose_( parameter.verbose() ),
         method_( method < 0 ? parameter.solverMethod( supportedSolverMethods() ) : method ),
         precondMethod_( parameter.preconditionMethod( supportedPreconditionMethods() ) )
       {
-        // assert( parameter_->errorMeasure() == 0 );
+        assert( parameter_->errorMeasure() == 0 );
       }
 
       template <class Operator>
       void bind ( const Operator &op )
       {
         if( precondMethod_ && std::is_base_of< AssembledOperator< DomainFunctionType, DomainFunctionType >, Operator > :: value )
         {
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/ldlsolver.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/ldlsolver.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/linear/bicgstab.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/linear/bicgstab.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/linear/cg.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/linear/cg.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/linear/gmres.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/linear/gmres.hh`

 * *Files 5% similar despite different names*

```diff
@@ -73,23 +73,26 @@
       {
         y[ l ] = 0;
       }
 
       const auto& auxiliaryDofs = vjp.space().auxiliaryDofs();
       const auto& vj = vjp.dofVector();
 
-      auto scp = [&m, &y, &vj, &v] (const size_t dof)
+      const size_t numAuxiliarys = auxiliaryDofs.size();
+      for( size_t auxiliary = 0, i = 0 ; auxiliary < numAuxiliarys; ++auxiliary, ++i  )
       {
-        for(int l=0; l<m; ++l)
+        const size_t nextAuxiliary = auxiliaryDofs[ auxiliary ];
+        for(; i < nextAuxiliary; ++i )
         {
-          y[ l ] += (vj[ dof ] * v[ l ].dofVector()[ dof ]);
+          for(int l=0; l<m; ++l)
+          {
+            y[ l ] += (vj[ i ] * v[ l ].dofVector()[ i ]);
+          }
         }
-      };
-      // see dune/fem/space/common/auiliarydofs.hh
-      forEachPrimaryDof( auxiliaryDofs, scp );
+      }
 
       // communicate sum
       comm.sum( y, m );
   }
 
   //! dblas_rotate with inc = 1
   template<class FieldType>
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/multistep.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/multistep.hh`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   /** \brief \newimplementation Base class for explicit multistep method. */
   template<class Operator>
   class ExplMultiStepBase
   {
   public:
     typedef typename Operator::DestinationType DestinationType;
     typedef typename DestinationType :: DiscreteFunctionSpaceType SpaceType;
-    // typedef typename SpaceType :: GridType :: Traits :: Communication DuneCommunicatorType;
+    // typedef typename SpaceType :: GridType :: Traits :: CollectiveCommunication DuneCommunicatorType;
   protected:
     std::vector< std::vector<double> > a;
     std::vector<double> b;
     std::vector<double> c;
     size_t steps_;
     double gamma_;
     std::vector<DestinationType*> Uj;
@@ -369,15 +369,15 @@
   class ExplMultiStep : public TimeProvider ,
                         public ExplMultiStepBase<Operator>
   {
     typedef ExplMultiStepBase<Operator> BaseType;
   public:
     typedef typename Operator :: DestinationType DestinationType;
     typedef typename DestinationType :: DiscreteFunctionSpaceType SpaceType;
-    typedef typename SpaceType :: GridType :: Traits :: Communication DuneCommunicatorType;
+    typedef typename SpaceType :: GridType :: Traits :: CollectiveCommunication DuneCommunicatorType;
 
   public:
     /** \brief constructor
       \param[in] op Operator \f$L\f$
       \param[in] pord polynomial order
       \param[in] cfl cfl number
       \param[in] verbose verbosity
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/newtoninverseoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/newtoninverseoperator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
      *       Source: "Globally Convergent Inexact Newton Methods", Stanley C. Eisenstat and Homer F. Walker, https://doi.org/10.1137/0804022.
     */
     class EisenstatWalkerStrategy
     {
     protected:
       const double etaMax_ = 0.99;
       const double gamma_ = 0.1;
+      const double newtonTolerance_;
       mutable double previousEta_ = -1.0;
-      mutable double previousResidual_ = -1.0;
-      mutable double newtonTolerance_;
+      mutable double previousResidual_ = -1;
 
     public:
       /** constructor
        *  \param[in]  newtonTolerance      the absolute tolerance of the Newton method
       */
       EisenstatWalkerStrategy(const double newtonTolerance) : newtonTolerance_(newtonTolerance) {}
       double nextLinearTolerance(const double currentResidual) const
@@ -53,15 +53,14 @@
           const double etaC = indicator < 0.1 ? std::min(etaA, etaMax_) : std::min(etaMax_, std::max(etaA, indicator));
           eta = std::min(etaMax_, std::max(etaC, 0.5 * newtonTolerance_ / currentResidual));
         }
         previousResidual_ = currentResidual;
         previousEta_ = eta;
         return eta;
       }
-      void setTolerance(const double newtonTolerance) { newtonTolerance_ = newtonTolerance; }
     };
 
     // NewtonParameter
     // ---------------
 
     template <class SolverParam = SolverParameter>
     struct NewtonParameter
@@ -393,16 +392,14 @@
        *
        *  \note The tolerance is read from the paramter
        *        <b>fem.solver.newton.tolerance</b>
        */
 
       void setErrorMeasure ( ErrorMeasureType finished ) { finished_ = std::move( finished ); }
 
-      EisenstatWalkerStrategy& eisenstatWalker () { return eisenstatWalker_; }
-
       void bind ( const OperatorType &op ) { op_ = &op; }
 
       void bind ( const OperatorType &op, const PreconditionerType& preconditioner )
       {
         bind( op );
         if( preconditioningAvailable )
           preconditioner_ = &preconditioner;
@@ -421,15 +418,14 @@
       void updateLinearTolerance () const {
         if (linearToleranceStrategy_ == ParameterType::LinearToleranceStrategy::eisenstatwalker) {
           double newTol = eisenstatWalker_.nextLinearTolerance( delta_ );
           jInv_.parameter().setTolerance( newTol );
         }
       }
       bool verbose() const { return verbose_ && Parameter::verbose( Parameter::solverStatistics ); }
-      double residual () const { return delta_; }
 
       NewtonFailure failed () const
       {
         // check for finite |residual| - this also works for -ffinite-math-only (gcc)
         // nan test not working with optimization flags...
         if( !(delta_ < std::numeric_limits< DomainFieldType >::max()) || std::isnan( delta_ ) )
           return NewtonFailure::InvalidResidual;
@@ -528,15 +524,15 @@
       mutable LinearInverseOperatorType jInv_;
       mutable std::unique_ptr< JacobianOperatorType > jOp_;
       ParameterType parameter_;
       mutable int stepCompleted_;
       typename ParameterType::LineSearchMethod lsMethod_;
       ErrorMeasureType finished_;
       typename ParameterType::LinearToleranceStrategy linearToleranceStrategy_;
-      EisenstatWalkerStrategy eisenstatWalker_;
+      const EisenstatWalkerStrategy eisenstatWalker_;
     };
 
 
     // Implementation of NewtonInverseOperator
     // ---------------------------------------
 
     template< class JacobianOperator, class LInvOp >
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/odesolver.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/odesolver.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/odesolverinterface.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/odesolverinterface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/parameter.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/parameter.hh`

 * *Files 1% similar despite different names*

```diff
@@ -220,19 +220,14 @@
       }
 
       virtual int preconditionerLevel () const
       {
         return parameter_.getValue< int >( keyPrefix_ + "preconditioning.level", 0 );
       }
 
-      virtual bool threading () const
-      {
-        return parameter_.getValue< bool >( keyPrefix_ + "threading", true );
-      }
-
      private:
       virtual double absoluteTol__ ( )  const
       {
         if( absoluteTol_ < 0 )
         {
           if(parameter_.exists(keyPrefix_ + "linabstol"))
           {
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/parameterdoc.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/parameterdoc.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/petscinverseoperators.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/petscinverseoperators.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/preconditionedinverseoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/preconditionedinverseoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/preconditionfunctionwrapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/preconditionfunctionwrapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/basicimplicit.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/basicimplicit.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/basicrow.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/basicrow.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/butchertable.cc` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/butchertable.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/butchertable.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/butchertable.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/explicit.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/explicit.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/implicit.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/implicit.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/row.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/row.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/semiimplicit.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/semiimplicit.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/rungekutta/timestepcontrol.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/rungekutta/timestepcontrol.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/spqrsolver.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/spqrsolver.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/test/inverseoperatortest.cc` & `dune-fem-2.9.dev20220529/dune/fem/solver/test/inverseoperatortest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/test/newtontest.cc` & `dune-fem-2.9.dev20220529/dune/fem/solver/test/newtontest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/test/odetest.cc` & `dune-fem-2.9.dev20220529/dune/fem/solver/test/odetest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 // than a simple, tuned up double.
 template <int N>
 class myDest : public Dune::FieldVector<double, N> {
   typedef myDest< N > ThisType;
 private:
   struct GridPartDummy
   {
-    typedef Dune::Communication< Dune::No_Comm > CommunicationType;
+    typedef Dune::CollectiveCommunication< Dune::No_Comm > CollectiveCommunicationType;
 
-    const CommunicationType &comm () const { return comm_; }
+    const CollectiveCommunicationType &comm () const { return comm_; }
 
-    CommunicationType comm_;
+    CollectiveCommunicationType comm_;
   };
 
   struct SpaceDummy {
     typedef GridPartDummy GridPartType;
     typedef std::array<int, 1 > AuxiliaryDofsType;
 
     SpaceDummy () : auxiliaryDofs_() { auxiliaryDofs_[ 0 ] = N; }
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/test/parameter` & `dune-fem-2.9.dev20220529/dune/fem/solver/test/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/test/test-timeprovider.cc` & `dune-fem-2.9.dev20220529/dune/fem/solver/test/test-timeprovider.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/timeprovider.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/timeprovider.hh`

 * *Files 5% similar despite different names*

```diff
@@ -208,32 +208,32 @@
      *  for( ; tp.time() < endTime; tp.next() )
      *  {
      *    // do stuff
      *  }
      *  \endcode
      *
      */
-    template< class Communication = typename MPIManager::Communication >
+    template< class CollectiveCommunication = typename MPIManager::CollectiveCommunication >
     class FixedStepTimeProvider
     : public TimeProviderBase
     {
-      typedef FixedStepTimeProvider< Communication > ThisType;
+      typedef FixedStepTimeProvider< CollectiveCommunication > ThisType;
       typedef TimeProviderBase BaseType;
 
     public:
-      typedef Communication CommunicationType;
+      typedef CollectiveCommunication CollectiveCommunicationType;
 
       /** \brief constructor
        *
        *  \param[in]  startTime     initial time
        *  \param[in]  timeStepSize  time step size
        *  \param[in]  comm          collective communication (default Dune::Fem::MPIManager::comm())
        */
       explicit FixedStepTimeProvider ( const double startTime, const double timeStepSize,
-                                       const CommunicationType &comm,
+                                       const CollectiveCommunicationType &comm,
                                        const ParameterReader &parameter = Parameter::container() )
         : BaseType( startTime, parameter ), comm_( comm )
       {
         dt_ = timeStepSize;
         initTimeStep();
       }
 
@@ -255,15 +255,15 @@
       explicit FixedStepTimeProvider ( const ParameterReader &parameter = Parameter::container() )
         : BaseType( parameter.getValue< double>( "fem.timeprovider.starttime", 0.0 ), parameter ), comm_( MPIManager::comm() )
       {
         dt_ = parameter.getValidValue< double >("fem.timeprovider.fixedtimestep", [] ( double v ) { return v > 0.0;} );
         initTimeStep();
       }
 
-      explicit FixedStepTimeProvider ( const CommunicationType &comm,
+      explicit FixedStepTimeProvider ( const CollectiveCommunicationType &comm,
                                        const ParameterReader &parameter = Parameter::container() )
         : BaseType( parameter.getValue< double>( "fem.timeprovider.starttime", 0.0 ), parameter ), comm_( comm )
       {
         dt_ = parameter.getValidValue< double >("fem.timeprovider.fixedtimestep", [] ( double v ) { return v > 0.0;} );
         initTimeStep();
       }
       virtual ~FixedStepTimeProvider () {}
@@ -291,15 +291,15 @@
 
       inline void initTimeStep ()
       {
         valid_ = true;
         initTimeStepEstimate();
       }
 
-      const CommunicationType &comm_;
+      const CollectiveCommunicationType &comm_;
     };
 
 
     /**
        \ingroup ODESolver
        \brief   manager for global simulation time of time-dependent solutions
 
@@ -371,16 +371,16 @@
        either during the construction of the Dune::TimeProvider or
        by using the parameter \c fem.timeprovider.factor.
        A further parameter read by the Dune::TimeProvider is
        fem.timeprovider.starttime defining the starting time of
        the simulation (default is zero).
 
        The most general implementation is given in the class
-       Dune::Fem::TimeProvider< Communication< C > >  which
-       takes a Dune::Communication instance in the
+       Dune::Fem::TimeProvider< CollectiveCommunication< C > >  which
+       takes a Dune::CollectiveCommunication instance in the
        constructor which is used in parallel computations is
        syncronize the time step. It defaults to
        Dune::Fem::MPIManager::comm() and also works for serial runs.
 
        If the communication manager from a given grid is to be used
        the class Dune::Fem::GridTimeProvider using the GridType as
        template argument can be used instead, with the same
@@ -395,23 +395,23 @@
        \parametername \c fem.timeprovider.updatestep \n
                       only do the update of the time step size
                       every 'updatestep' to avoid the
                       expensive communication to achieve this
                       (for testing only);
                       defaults to 1
      */
-    template< class Communication = typename MPIManager::Communication >
+    template< class CollectiveCommunication = typename MPIManager::CollectiveCommunication >
     class TimeProvider
     : public TimeProviderBase
     {
-      typedef TimeProvider< Communication > ThisType;
+      typedef TimeProvider< CollectiveCommunication > ThisType;
       typedef TimeProviderBase BaseType;
 
     public:
-      typedef Communication CommunicationType;
+      typedef CollectiveCommunication CollectiveCommunicationType;
 
     protected:
 
       using BaseType::parameter_;
 
       inline double getCflFactor() const
       {
@@ -434,29 +434,29 @@
       : BaseType( parameter ),
         comm_( MPIManager::comm() ),
         cfl_( getCflFactor() ),
         updateStep_( getUpdateStep() ),
         counter_( updateStep_ )
       {}
 
-      explicit TimeProvider ( const CommunicationType &comm, const ParameterReader &parameter = Parameter::container() )
+      explicit TimeProvider ( const CollectiveCommunicationType &comm, const ParameterReader &parameter = Parameter::container() )
       : BaseType( parameter ),
         comm_( comm ),
         cfl_( getCflFactor() ),
         updateStep_( getUpdateStep() ),
         counter_( updateStep_ )
       {}
 
       /** \brief constructor taking start time
        *
        *  \param[in]  startTime  initial time
        *  \param[in]  comm       collective communication (default Dune::Fem::MPIManager::comm())
        */
       explicit TimeProvider ( const double startTime,
-                              const CommunicationType &comm = MPIManager::comm() )
+                              const CollectiveCommunicationType &comm = MPIManager::comm() )
       : BaseType( startTime ),
         comm_( comm ),
         cfl_( getCflFactor() ),
         updateStep_( getUpdateStep() ),
         counter_( updateStep_ )
       {}
 
@@ -464,15 +464,15 @@
        *
        *  \param[in]  startTime  initial time
        *  \param[in]  cfl        CFL constant
        *  \param[in]  comm       collective communication (default Dune::Fem::MPIManager::comm())
        */
       TimeProvider ( const double startTime,
                      const double cfl,
-                     const CommunicationType &comm = MPIManager::comm() )
+                     const CollectiveCommunicationType &comm = MPIManager::comm() )
       : BaseType( startTime ),
         comm_( comm ),
         cfl_( cfl ),
         updateStep_( 1 ),
         counter_( updateStep_ )
       {}
 
@@ -584,41 +584,41 @@
       using BaseType::dt_;
       using BaseType::invdt_;
       using BaseType::dtEstimate_;
       using BaseType::dtUpperBound_;
       using BaseType::valid_;
       using BaseType::timeStep_;
 
-      const CommunicationType& comm_;
+      const CollectiveCommunicationType& comm_;
       const double cfl_;
       const int updateStep_;
       int counter_;
     };
 
 
 
     /** \class   GridTimeProvider
      *  \ingroup ODESolver
      *  \brief   the same functionality as the Dune::TimeProvider.
      *
-     *  This implementation of a timeprovider takes the Communication
+     *  This implementation of a timeprovider takes the CollectiveCommunicate
      *  from a Dune::Grid instance.
      */
     template< class Grid >
     class GridTimeProvider
-    : public TimeProvider< typename Grid::Traits::Communication >
+    : public TimeProvider< typename Grid::Traits::CollectiveCommunication >
     {
       typedef GridTimeProvider< Grid > ThisType;
-      typedef TimeProvider< typename Grid::Traits::Communication > BaseType;
+      typedef TimeProvider< typename Grid::Traits::CollectiveCommunication > BaseType;
 
       // type of DofManager for sequence number
       typedef DofManager < Grid > DofManagerType ;
 
     public:
-      typedef typename Grid::Traits::Communication CommunicationType;
+      typedef typename Grid::Traits::CollectiveCommunication CollectiveCommunicationType;
 
       explicit GridTimeProvider ( const Grid &grid )
       : BaseType( grid.comm() ),
         dm_( DofManagerType ::instance( grid ) ),
         sequence_( -1 )
       {}
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/umfpacksolver.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/umfpacksolver.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/solver/viennacl.hh` & `dune-fem-2.9.dev20220529/dune/fem/solver/viennacl.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/space/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/basisfunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/basisfunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/codegen.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/codegen.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/default.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/default.hh`

 * *Files 2% similar despite different names*

```diff
@@ -476,48 +476,14 @@
           for( unsigned int qp = 0; qp < nop; ++qp )
           {
             axpy( quad[ qp ], jacobianFactors[ qp ], dofs );
           }
         }
       }
 
-      //! \brief evaluate all basis function and multiply with given values and add to dofs
-      template< class QuadratureType, class HessianArray, class DofVector >
-      void axpyImpl ( const QuadratureType &quad, const HessianArray &hessianFactors, DofVector &dofs, const HessianRangeType& ) const
-      {
-        assert( hessianFactors.size() >= quad.nop() );
-        /* TODO add code generation for hessians
-        // if shape function set supports codegen and quadrature supports caching
-        if constexpr ( codegenShapeFunctionSet && std::is_base_of< CachingInterface, QuadratureType > :: value)
-        {
-          typedef Codegen :: EvaluateCallerInterfaceTraits< QuadratureType, HessianArray, DofVector, Geometry >  Traits;
-          typedef Codegen :: EvaluateCallerInterface< Traits > BaseEvaluationType;
-
-          // get base function evaluate caller (calls axpyRanges)
-          const auto& baseEval = BaseEvaluationType::storage( *this, hessianCache( quad ), quad );
-
-          // true if implementation exists
-          if( baseEval )
-          {
-            // call appropriate axpyRanges method
-            const Geometry &geo = geometry();
-            baseEval->axpyHessian( quad, geo, hessianFactors, dofs );
-            return ;
-          }
-        }
-        */
-        {
-          const unsigned int nop = quad.nop();
-          for( unsigned int qp = 0; qp < nop; ++qp )
-          {
-            axpy( quad[ qp ], hessianFactors[ qp ], dofs );
-          }
-        }
-      }
-
       template <class QuadratureType>
       const auto& rangeCache( const QuadratureType& quad ) const
       {
         return shapeFunctionSet().scalarShapeFunctionSet().impl().rangeCache( quad );
       }
 
       template <class QuadratureType>
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/evaluatecaller.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/evaluatecaller.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/evaluatecallerdeclaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/evaluatecallerdeclaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/evaluatecallerdefaultimpl.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/evaluatecallerdefaultimpl.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/functor.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/functor.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/anisotropic.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/anisotropic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/basisfunctionsets.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/basisfunctionsets.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/legendre.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/legendre.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/orthogonal.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/orthogonal.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/typeindexset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/typeindexset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/typemap.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/typemap.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/hpdg/vectorial.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/hpdg/vectorial.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/piolatransformation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/piolatransformation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/simple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/simple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/checkbasisfunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/checkbasisfunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-cachingbasisfunctionset.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-cachingbasisfunctionset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-defaultbasisfunctionset.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-defaultbasisfunctionset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-generate.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-generate.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-simplebasisfunctionset.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-simplebasisfunctionset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-tuplebasisfunctionset.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-tuplebasisfunctionset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/test/test-vectorialbasisfunctionset.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/test/test-vectorialbasisfunctionset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/transformation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/transformation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/transformed.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/transformed.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/tuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/tuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/basisfunctionset/vectorial.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/basisfunctionset/vectorial.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/brezzidouglasmarini.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/brezzidouglasmarini.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/combineddofstorage.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/combineddofstorage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/combinedspace.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/combinedspace.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/generic.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/generic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/interpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/interpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/lagrangepointsetexporter.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/lagrangepointsetexporter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/powerlocalrestrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/powerlocalrestrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/powermapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/powermapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/powerspace.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/powerspace.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/subobjects.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/subobjects.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/tuplelocalrestrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/tuplelocalrestrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/tuplemapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/tuplemapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/combinedspace/tuplespace.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/combinedspace/tuplespace.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/space/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/adaptationmanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/adaptationmanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/adaptcallbackhandle.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/adaptcallbackhandle.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/allgeomtypes.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/allgeomtypes.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/auxiliarydofs.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/auxiliarydofs.hh`

 * *Files 13% similar despite different names*

```diff
@@ -126,23 +126,14 @@
 
       //! return number of auxiliary dofs
       IndexType size () const
       {
         return auxiliarys_.size();
       }
 
-      //! return number of primaryDofs
-      IndexType primarySize () const
-      {
-        const IndexType last = auxiliarys_.size() - 1;
-        // last entry is the overall size, thus substract size - 1 from the
-        // overall number to obtain the number of primary dofs
-        return auxiliarys_[ last ] - last ;
-      }
-
       ConstIterator begin () const { return ConstIterator( auxiliarys_, 0 ); }
       ConstIterator end () const { assert( size() > 0 ); return ConstIterator( auxiliarys_, size()-1 ); }
 
       //! return true if index is contained, meaning it is a auxiliary dof
       bool contains ( IndexType index ) const { return std::binary_search( begin(), end(), index ); }
 
       [[deprecated("Use contains instead")]]
@@ -264,60 +255,21 @@
       template <class Entity>
       bool sendRank(const Entity& entity) const
       {
         const PartitionType ptype = entity.partitionType();
         return (ptype == InteriorEntity) || (ptype == BorderEntity);
       }
 
-    protected:
+    private:
       int myRank_, mySize_;
       std::set< IndexType > &auxiliarySet_;
       const MapperType &mapper_;
     };
 
 
-    /** \brief @ingroup Communication
-     *
-     *  Apply action encoded in Functor f to all auxiliary dofs.
-     *  \param[in]  auxiliaryDofs  AuxiliaryDofs instance (from space)
-     *  \param[in]  f  a Functor or lambda offering operator()( const size_t dof )
-     */
-    template <class AuxiliaryDofs, class F>
-    static void forEachAuxiliaryDof( const AuxiliaryDofs& auxiliaryDofs, F&& f )
-    {
-      // don't delete the last since this is the overall Size
-      const size_t auxiliarySize = auxiliaryDofs.size() - 1;
-      for(size_t auxiliary = 0; auxiliary<auxiliarySize; ++auxiliary)
-      {
-        // apply action to auxiliary dof
-        f( auxiliaryDofs[auxiliary] );
-      }
-    }
-
-    /** \brief @ingroup Communication
-     *
-     *  Apply action encoded in Functor f to all primary dofs.
-     *  \param[in]  auxiliaryDofs  AuxiliaryDofs instance (from space)
-     *  \param[in]  f  a Functor or lambda offering operator()( const size_t dof )
-     */
-    template <class AuxiliaryDofs, class F>
-    static void forEachPrimaryDof( const AuxiliaryDofs& auxiliaryDofs, F&& f )
-    {
-      const size_t numAuxiliarys = auxiliaryDofs.size();
-      for( size_t auxiliary = 0, dof = 0 ; auxiliary < numAuxiliarys; ++auxiliary, ++dof  )
-      {
-        const size_t nextAuxiliary = auxiliaryDofs[ auxiliary ];
-        for(; dof < nextAuxiliary; ++dof )
-        {
-          // apply action to primary dof
-          f( dof );
-        }
-      }
-    }
-
 
     // PrimaryDofs
     // -----------
 
     /** \brief @ingroup Communication
      *
      *  In parallel computations the dofs of a discrete function are made up by
@@ -375,15 +327,14 @@
             continue;
         }
 
         const AuxiliaryDofsType *auxiliaryDofs_ = nullptr;
         IndexType index_ = 0, auxiliary_ = 0;
       };
 
-      [[deprecated("Use forEachPrimaryDof instead!")]]
       explicit PrimaryDofs ( const AuxiliaryDofsType &auxiliaryDofs )
         : auxiliaryDofs_( auxiliaryDofs )
       {}
 
       ConstIterator begin () const { return ConstIterator( auxiliaryDofs_, 0, 0 ); }
       ConstIterator end () const { return ConstIterator( auxiliaryDofs_[ auxiliaryDofs_.size()-1 ], auxiliaryDofs_.size() ); }
 
@@ -395,15 +346,14 @@
 
 
 
     // primaryDofs
     // -----------
 
     template< class AuxiliaryDofs >
-    [[deprecated("Use forEachPrimaryDof instead!" )]]
     inline static PrimaryDofs< AuxiliaryDofs > primaryDofs ( const AuxiliaryDofs &auxiliaryDofs )
     {
       return PrimaryDofs< AuxiliaryDofs >( auxiliaryDofs );
     }
 
     template< class AuxiliaryDofs >
     [[deprecated("Use primaryDofs instead!" )]]
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/basesetlocalkeystorage.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/basesetlocalkeystorage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/cachedcommmanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/cachedcommmanager.hh`

 * *Files 0% similar despite different names*

```diff
@@ -866,15 +866,15 @@
 
 
 
     template< class BlockMapper >
     template< class Space >
     inline void DependencyCache< BlockMapper > :: buildMaps( const Space& space )
     {
-      typedef typename Space::GridPartType::CommunicationType CommunicationType;
+      typedef typename Space::GridPartType::CollectiveCommunicationType CommunicationType;
       if( interface_ == InteriorBorder_All_Interface )
       {
         LinkBuilder< CommunicationType, LinkStorageType, IndexMapVectorType,
                      InteriorBorder_All_Interface >
           handle( space.gridPart().comm(),
                   space.blockMapper(),
                   linkStorage_, sendIndexMap_, recvIndexMap_ );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/commindexmap.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/commindexmap.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/commoperations.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/commoperations.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/communicationmanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/communicationmanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/datacollector.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/datacollector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/dataprojection.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/dataprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/default.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/default.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/dataprojection/tuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/dataprojection/tuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/defaultcommhandler.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/defaultcommhandler.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/discretefunctionspace.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/discretefunctionspace.hh`

 * *Files 2% similar despite different names*

```diff
@@ -424,34 +424,14 @@
        */
       inline int size () const
       {
         CHECK_INTERFACE_IMPLEMENTATION( asImp().size() );
         return asImp().size();
       }
 
-      /** \brief get number of primary DoFs for this space
-
-          \returns number of primary DoFs (degrees of freedom that are owned by this process )
-       */
-      inline int primarySize () const
-      {
-        CHECK_INTERFACE_IMPLEMENTATION( asImp().primarySize() );
-        return asImp().primarySize();
-      }
-
-      /** \brief get number of auxiliary DoFs for this space
-
-          \returns number of auxiliary DoFs (degrees of freedom that are NOT owned by this process)
-       */
-      inline int auxiliarySize () const
-      {
-        CHECK_INTERFACE_IMPLEMENTATION( asImp().auxiliarySize() );
-        return asImp().auxiliarySize();
-      }
-
       /** \brief get iterator pointing to the first entity of the associated grid
                  partition
 
           \returns iterator pointing to first entity
        */
       inline IteratorType begin () const
       {
@@ -776,27 +756,14 @@
 
       /** \copydoc Dune::Fem::DiscreteFunctionSpaceInterface::size */
       inline int size () const
       {
         return blockMapper().size() * localBlockSize ;
       }
 
-      /** \copydoc Dune::Fem::DiscreteFunctionSpaceInterface::primarySize */
-      inline int primarySize () const
-      {
-        return auxiliaryDofs().primarySize() * localBlockSize;
-      }
-
-      /** \copydoc Dune::Fem::DiscreteFunctionSpaceInterface::auxiliarySize */
-      inline int auxiliarySize () const
-      {
-        // total size minus primary dofs
-        return size() - primarySize();
-      }
-
       //! \brief return the maximal number of dofs on entities
       inline int maxNumDofs () const
       {
         return blockMapper().maxNumDofs() * localBlockSize;
       }
 
       /** \copydoc Dune::Fem::DiscreteFunctionSpaceInterface::begin() const
@@ -1006,15 +973,15 @@
 
     private:
       typedef DiscreteFunctionSpaceAdapter< FunctionSpaceType, GridPartType >
         ThisType;
       typedef FunctionSpaceType BaseType;
 
     public:
-      enum { polynomialOrder = 6 }; // default polynomial order basically for determination of quadrature orders
+      enum { polynomialOrder = 111 };
 
       //! type of the grid
       typedef typename GridPartType :: GridType GridType;
       //! type of the index set
       typedef typename GridPartType :: IndexSetType IndexSetType;
       //! type of the grid iterator
       typedef typename GridPartType :: template Codim< 0 > :: IteratorType
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/dofmanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/dofmanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/dofstorage.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/dofstorage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/functionspace.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/functionspace.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/functionspaceinterface.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/functionspaceinterface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/interpolate.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/interpolate.hh`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     {
       ConstLocalFunction< GridFunction > uLocal( u );
       LocalContribution< DiscreteFunction, Assembly::Set > vLocal( v );
       LocalInterpolation< typename DiscreteFunction::DiscreteFunctionSpaceType >
         interpolation( v.space() );
 
       // iterate over selected partition
-      for( const auto& entity : elements( v.gridPart(), ps ) )
+      for( const auto entity : elements( v.gridPart(), ps ) )
       {
         // initialize u to entity
         auto uGuard = bindGuard( uLocal, entity );
 
         // bind v to entity
         auto vGuard = bindGuard( vLocal, entity );
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/loadbalancer.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/loadbalancer.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/localinterpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/localinterpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/localrestrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/localrestrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/restrictprolongfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/restrictprolongfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/restrictprolonginterface.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/restrictprolonginterface.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/restrictprolongtuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/restrictprolongtuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/common/uniquefacetorientation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/common/uniquefacetorientation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/basisfunctionsets.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/basisfunctionsets.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/declaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/declaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/generic.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/generic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/hierarchiclegendre.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/hierarchiclegendre.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/interpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/interpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/lagrange.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/lagrange.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/legendre.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/legendre.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/localdgmassmatrix.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/localdgmassmatrix.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/localinterpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/localinterpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/localrestrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/localrestrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/shapefunctionsets.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/shapefunctionsets.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/discontinuousgalerkin/tuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/discontinuousgalerkin/tuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/finitevolume/basisfunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/basisfunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/finitevolume/basisfunctionsets.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/basisfunctionsets.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/finitevolume/interpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/interpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/finitevolume/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/finitevolume/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/fourier/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/fourier/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/fourier/declaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/fourier/declaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/fourier/dofmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/fourier/dofmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/fourier/functionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/fourier/functionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/fourier/interpolate.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/fourier/interpolate.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/fourier/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/fourier/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/anisotropic.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/anisotropic.hh`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,14 @@
       template< class FunctionSpace, class GridPart, int order, class Storage >
       class AnisotropicDiscontinuousGalerkinSpace
       : public hpDG::DiscontinuousGalerkinSpace< AnisotropicDiscontinuousGalerkinSpaceTraits< FunctionSpace, GridPart, order, Storage > >
       {
         using BaseType = hpDG::DiscontinuousGalerkinSpace< AnisotropicDiscontinuousGalerkinSpaceTraits< FunctionSpace, GridPart, order, Storage > >;
 
       public:
-        static const int polynomialOrder = order;
-
         using GridPartType = typename BaseType::GridPartType;
         using EntityType   = typename BaseType::EntityType;
         using BasisFunctionSetsType = typename BaseType::BasisFunctionSetsType;
         typedef typename BaseType::KeyType  KeyType;
 
         explicit AnisotropicDiscontinuousGalerkinSpace ( GridPartType &gridPart,
                                                          const Dune::InterfaceType interface = Dune::InteriorBorder_All_Interface,
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/blockmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/blockmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/datahandle.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/datahandle.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/default.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/default.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/legendre.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/legendre.hh`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,14 @@
       template< class FunctionSpace, class GridPart, int order, class Storage >
       class LegendreDiscontinuousGalerkinSpace
       : public hpDG::DiscontinuousGalerkinSpace< LegendreDiscontinuousGalerkinSpaceTraits< FunctionSpace, GridPart, order, false, Storage > >
       {
         using BaseType = hpDG::DiscontinuousGalerkinSpace< LegendreDiscontinuousGalerkinSpaceTraits< FunctionSpace, GridPart, order, false, Storage > >;
 
       public:
-        static const int polynomialOrder = order;
-
         using GridPartType = typename BaseType::GridPartType;
         using BasisFunctionSetsType = typename BaseType::BasisFunctionSetsType;
 
         explicit LegendreDiscontinuousGalerkinSpace ( GridPartType &gridPart,
                                                       const Dune::InterfaceType interface = Dune::InteriorBorder_All_Interface,
                                                       const Dune::CommunicationDirection direction = Dune::ForwardCommunication )
           : BaseType( gridPart, BasisFunctionSetsType{}, order, interface, direction )
@@ -127,16 +125,14 @@
       template< class FunctionSpace, class GridPart, int order, class Storage >
       class HierarchicLegendreDiscontinuousGalerkinSpace
       : public hpDG::DiscontinuousGalerkinSpace< LegendreDiscontinuousGalerkinSpaceTraits< FunctionSpace, GridPart, order, true, Storage > >
       {
         using BaseType = hpDG::DiscontinuousGalerkinSpace< LegendreDiscontinuousGalerkinSpaceTraits< FunctionSpace, GridPart, order, true, Storage > >;
 
       public:
-        static const int polynomialOrder = order;
-
         using GridPartType = typename BaseType::GridPartType;
         using EntityType   = typename BaseType::EntityType;
         using BasisFunctionSetsType = typename BaseType::BasisFunctionSetsType;
 
         explicit HierarchicLegendreDiscontinuousGalerkinSpace ( GridPartType &gridPart,
                                                                 const Dune::InterfaceType interface = Dune::InteriorBorder_All_Interface,
                                                                 const Dune::CommunicationDirection direction = Dune::ForwardCommunication )
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/localdofstorage.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/localdofstorage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/orthogonal.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/orthogonal.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/hpdg/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/hpdg/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/adaptmanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/adaptmanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/declaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/declaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/dofmappercode.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/dofmappercode.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/genericbasefunctions.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/genericbasefunctions.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/genericgeometry.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/genericgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/genericlagrangepoints.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/genericlagrangepoints.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/interpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/interpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/lagrangepoints.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/lagrangepoints.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/restrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/restrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/shapefunctionset.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/shapefunctionset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/shapefunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/shapefunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/storage.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/storage.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/basisfunctiontest.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/basisfunctiontest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/basisfunctiontest.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/basisfunctiontest.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/cube.dgf` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/cube.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/generic.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/generic.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/main.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/main.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/mappertest.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/mappertest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange/test/mappertest.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange/test/mappertest.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/lagrange.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/lagrange.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/capabilities.hh`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,22 @@
       };
 
 
       template< class LFEMap, class FunctionSpace, class Storage >
       struct hasStaticPolynomialOrder< LocalFiniteElementSpace< LFEMap, FunctionSpace, Storage > >
       {
         static const bool v = false;
-        static const int order = 6; // default polynomial order if not specified otherwise
+        static const int order = 111;
       };
 
       template< class LFEMap, class FunctionSpace, class Storage >
       struct hasStaticPolynomialOrder< DiscontinuousLocalFiniteElementSpace< LFEMap, FunctionSpace, Storage > >
       {
         static const bool v = false;
-        static const int order = 6; // default polynomial order if not specified otherwise
+        static const int order = 111;
       };
 
 
       template< class LFEMap, class FunctionSpace, class Storage >
       struct isContinuous< LocalFiniteElementSpace< LFEMap, FunctionSpace, Storage > >
       {
         static const bool v = false;
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/dgspace.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/dgspace.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/interpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/interpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/localrestrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/localrestrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/quadratureinterpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/quadratureinterpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/shapefunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/shapefunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/localfiniteelement/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/localfiniteelement/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/code.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/code.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/codimensionmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/codimensionmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/compile.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/compile.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/dofmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/dofmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/dynamicnonblockmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/dynamicnonblockmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/genericadaptivedofmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/genericadaptivedofmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/ghost.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/ghost.hh`

 * *Files 6% similar despite different names*

```diff
@@ -347,17 +347,14 @@
 
       //! return dof number of salve with index
       GlobalKeyType operator [] ( int index ) const { return mapper().interiorSize() + index; }
 
       //! return number of auxiliary dofs
       SizeType size () const { return mapper().ghostSize()+1; }
 
-      //! return number of primary dofs
-      SizeType primarySize () const { return mapper().interiorSize(); }
-
       ConstIteratorType begin () const { return ConstIteratorType( mapper().interiorSize() ); }
       ConstIteratorType end () const { return ConstIteratorType( mapper().interiorSize() + mapper().ghostSize() ); }
 
       //! return true if index is contained, meaning it is an auxiliary dof
       bool contains ( GlobalKeyType index ) const { return (static_cast< SizeType >( index ) >= mapper().interiorSize()); }
 
       void rebuild () {}
@@ -366,35 +363,14 @@
       const GridPartType &gridPart () const { return mapper().gridPart(); }
 
     private:
       const MapperType &mapper_;
     };
 
 
-    /** \brief @ingroup Communication
-     *
-     *  Apply action encoded in Functor f to all primary dofs.
-     *  \param[in]  auxiliaryDofs  AuxiliaryDofs instance (from space)
-     *  \param[in]  f  a Functor or lambda offering operator()( const size_t dof )
-     *
-     *  \note: This is a specialization for the Petsc  GhostMapper based AuxiliaryDofs.
-     */
-    template <class GridPart, class BaseMapper, class GlobalKey, class F>
-    static void forEachPrimaryDof( const AuxiliaryDofs< GridPart, GhostDofMapper< GridPart, BaseMapper, GlobalKey > >& auxiliaryDofs, F&& f )
-    {
-      const size_t size = auxiliaryDofs.mapper().interiorSize();
-      for( size_t dof = 0 ; dof<size; ++dof )
-      {
-        // apply action to primary dof
-        f( dof );
-      }
-    }
-
-
-
 
     // PrimaryDofs for AuxiliaryDofs< GhostDofMapper >
     // ------------------------------------------
 
     template< class GridPart, class BaseMapper, class GlobalKey >
     struct PrimaryDofs< AuxiliaryDofs< GridPart, GhostDofMapper< GridPart, BaseMapper, GlobalKey > > >
     {
@@ -403,15 +379,14 @@
       typedef typename AuxiliaryDofsType::GlobalKeyType GlobalKeyType;
       typedef typename AuxiliaryDofsType::GridPartType GridPartType;
       typedef typename AuxiliaryDofsType::MapperType MapperType;
       typedef typename AuxiliaryDofsType::SizeType SizeType;
 
       typedef __GhostDofMapper::ConstIterator< GlobalKeyType > ConstIteratorType;
 
-      [[deprecated("Use forEachPrimaryDof instead!")]]
       explicit PrimaryDofs ( const AuxiliaryDofsType &auxiliaryDofs )
         : mapper_( auxiliaryDofs.mapper() )
       {}
 
       ConstIteratorType begin () const { return ConstIteratorType( 0 ); }
       ConstIteratorType end () const { return ConstIteratorType( size() ); }
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/indexsetdofmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/indexsetdofmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/localkey.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/localkey.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/nonblockmapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/nonblockmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/parallel.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/parallel.hh`

 * *Files 6% similar despite different names*

```diff
@@ -170,51 +170,46 @@
 
       // update
 
       void update ()
       {
         AuxiliaryDofs< GridPartType, BaseMapperType > auxiliaryDofs( gridPart(), baseMapper() );
         auxiliaryDofs.rebuild();
-        //auto primaryDofs = Dune::Fem::primaryDofs( auxiliaryDofs );
+        auto primaryDofs = Dune::Fem::primaryDofs( auxiliaryDofs );
 
-        const auto primarySize = auxiliaryDofs.primarySize(); // primaryDofs.size();
-        size_ = primarySize;  // primaryDofs.size();
+        size_ = primaryDofs.size();
         offset_ = exScan( gridPart().comm(), size_ );
         size_ = gridPart().comm().sum( size_ );
 
         std::size_t baseSize = baseMapper().size();
         mapping_.resize( baseSize );
         GlobalKeyType next = static_cast< GlobalKeyType >( offset_ );
-        std::vector< GlobalKeyType >& mapping = mapping_;
-        auto mapNext = [&mapping, &next] (const auto i) { mapping[ i ] = next++; };
-        // for all primary dofs build mapping
-        forEachPrimaryDof( auxiliaryDofs, mapNext );
-        //for( const auto i : primaryDofs )
-        //  mapping_[ i ] = next++;
-        assert( next == static_cast< GlobalKeyType >( offset_ + primarySize ) );
+        for( const auto i : primaryDofs )
+          mapping_[ i ] = next++;
+        assert( next == static_cast< GlobalKeyType >( offset_ + primaryDofs.size() ) );
 
         __ParallelDofMapper::BuildDataHandle< GridPartType, BaseMapperType, GlobalKeyType > dataHandle( baseMapper(), auxiliaryDofs, mapping_ );
         gridPart().communicate( dataHandle, InteriorBorder_All_Interface, ForwardCommunication );
       }
 
       const GridPartType &gridPart () const { return gridPart_; }
       const BaseMapperType &baseMapper () const { return baseMapper_; }
 
       const std::vector< GlobalKeyType > &mapping () const { return mapping_; }
 
     private:
       template< class Comm, class T >
-      static T exScan ( const Communication< Comm > &comm, T in )
+      static T exScan ( const CollectiveCommunication< Comm > &comm, T in )
       {
         return T( 0 );
       }
 
 #if HAVE_MPI
       template< class T >
-      static T exScan ( const Communication< MPI_Comm > &comm, T in )
+      static T exScan ( const CollectiveCommunication< MPI_Comm > &comm, T in )
       {
         T out( 0 );
         MPI_Exscan( &in, &out, 1, MPITraits< T >::getType(), MPI_SUM, static_cast< MPI_Comm >( comm ) );
         return out;
       }
 #endif // #if HAVE_MPI
```

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/mapper/petsc.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/mapper/petsc.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/p1bubble.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/p1bubble.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/adaptmanager.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/adaptmanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/capabilities.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/declaration.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/declaration.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/discontinuousgalerkin.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/discontinuousgalerkin.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/generic.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/generic.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/lagrange.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/lagrange.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/mapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/mapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/padaptivespace/restrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/padaptivespace/restrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/rannacherturek.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/rannacherturek.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/raviartthomas/localinterpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas/localinterpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/raviartthomas/space.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/raviartthomas/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/caching.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/caching.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/legendre.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/legendre.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/legendrepolynomials.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/legendrepolynomials.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/legendrepolynomials.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/legendrepolynomials.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/localfunctions.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/localfunctions.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_1d.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_1d.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_2d.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_2d.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_3d.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal/orthonormalbase_3d.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/orthonormal.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/orthonormal.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/proxy.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/proxy.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/selectcaching.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/selectcaching.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/shapefunctionset.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/shapefunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/simple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/simple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/tensorproduct.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/tensorproduct.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/tuple.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/tuple.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/vectorial.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/vectorial.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/shapefunctionset/wrapper.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/shapefunctionset/wrapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_poly-0.dgf` & `dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_poly-0.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_poly-1.dgf` & `dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_poly-1.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/2dgrid_poly-2.dgf` & `dune-fem-2.9.dev20220529/dune/fem/space/test/2dgrid_poly-2.dgf`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/space/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/adapt.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/adapt.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/checklocalinterpolation.hh` & `dune-fem-2.9.dev20220529/dune/fem/space/test/checklocalinterpolation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/combinedspacetest.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/combinedspacetest.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/dgcomm.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/dgcomm.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/functiontupleadapt.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/functiontupleadapt.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/hierarchicspace.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/hierarchicspace.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/interpolation.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/interpolation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/l2projection.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/l2projection.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/lagrangeadapt.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/lagrangeadapt.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/lagrangeglobalrefine.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/lagrangeglobalrefine.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/lagrangeinterpolation.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/lagrangeinterpolation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/localadapter.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/localadapter.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/padapt.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/padapt.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-auxiliarydofs.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-auxiliarydofs.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-balladapt.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-balladapt.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-fvadaptation.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-fvadaptation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-globalrefine.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-globalrefine.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-localadaptation.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-localadaptation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-raviartthomasinterpolation.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-raviartthomasinterpolation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-spaceinterpolation.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-spaceinterpolation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-tupledgspace.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-tupledgspace.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/space/test/test-tuplespace.cc` & `dune-fem-2.9.dev20220529/dune/fem/space/test/test-tuplespace.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/dynamicarray.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/dynamicarray.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/eigenvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/eigenvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/envelope.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/envelope.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/objectstack.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/objectstack.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/referencecounter.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/referencecounter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/referencevector.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/referencevector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/rowreferencevector.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/rowreferencevector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/singleton.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/singleton.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/singletonlist.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/singletonlist.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/subvector.hh` & `dune-fem-2.9.dev20220529/dune/fem/storage/subvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/storage/test/dynamicarray.cc` & `dune-fem-2.9.dev20220529/dune/fem/storage/test/dynamicarray.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fem/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/adaptation.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/adaptation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/dfspace.hh` & `dune-fem-2.9.dev20220529/dune/fem/test/dfspace.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/dgl2projection.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/dgl2projection.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/exactsolution.hh` & `dune-fem-2.9.dev20220529/dune/fem/test/exactsolution.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/fmatrixconverter.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/fmatrixconverter.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/l2projection.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/l2projection.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/lagrangeinterpolation.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/lagrangeinterpolation.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/massoperator.hh` & `dune-fem-2.9.dev20220529/dune/fem/test/massoperator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/parameter` & `dune-fem-2.9.dev20220529/dune/fem/test/parameter`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/referencesolution.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/referencesolution.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/simpleoperators.hh` & `dune-fem-2.9.dev20220529/dune/fem/test/simpleoperators.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/test-hierarchicall2projection.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/test-hierarchicall2projection.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/test-intersectionindexset.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/test-intersectionindexset.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/test-periodic.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/test-periodic.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/test-tupleoperator.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/test-tupleoperator.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/testgrid.hh` & `dune-fem-2.9.dev20220529/dune/fem/test/testgrid.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/vtxprojection.cc` & `dune-fem-2.9.dev20220529/dune/fem/test/vtxprojection.cc`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/test/weightfunction.hh` & `dune-fem-2.9.dev20220529/dune/fem/test/weightfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fem/version.hh` & `dune-fem-2.9.dev20220529/dune/fem/version.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/common/collectivecommunication.hh` & `dune-fem-2.9.dev20220529/dune/fempy/common/collectivecommunication.hh`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,43 @@
 namespace Dune
 {
 
   namespace FemPy
   {
 
     template< class BinaryFunction, class C, class T >
-    inline static int scan ( const Dune::Communication< C > &comm, T *inout, std::size_t size )
+    inline static int scan ( const Dune::CollectiveCommunication< C > &comm, T *inout, std::size_t size )
     {
       return 0;
     }
 
 #if HAVE_MPI
     template< class BinaryFunction, class T >
-    inline static int scan ( const Dune::Communication< MPI_Comm > &comm, T *inout, std::size_t size )
+    inline static int scan ( const Dune::CollectiveCommunication< MPI_Comm > &comm, T *inout, std::size_t size )
     {
       return MPI_Scan( MPI_IN_PLACE, inout, size, MPITraits< T >::getType(), (Generic_MPI_Op< T, BinaryFunction >::get()), static_cast< MPI_Comm >( comm ) );
     }
 #endif // #if HAVE_MPI
 
     template< class BinaryFunction, class C, class T >
-    inline static T scan ( const Dune::Communication< C > &comm, const T &in )
+    inline static T scan ( const Dune::CollectiveCommunication< C > &comm, const T &in )
     {
       T out( in );
       scan< BinaryFunction >( &out, 1u );
       return out;
     }
 
     template< class BinaryFunction, class C, class T, std::size_t size >
-    inline static int scan ( const Dune::Communication< C > &comm, std::array< T, size > &inout )
+    inline static int scan ( const Dune::CollectiveCommunication< C > &comm, std::array< T, size > &inout )
     {
       return scan( comm, inout.data(), size );
     }
 
     template< class BinaryFunction, class C, class T, class A >
-    inline static int scan ( const Dune::Communication< C > &comm, std::vector< T, A > &inout )
+    inline static int scan ( const Dune::CollectiveCommunication< C > &comm, std::vector< T, A > &inout )
     {
       return scan( comm, inout.data(), inout.size() );
     }
 
   } // namespace FemPy
 
 } // namespace Dune
```

### Comparing `dune-fem-2.9.0rc1/dune/fempy/function/simplegridfunction.hh` & `dune-fem-2.9.dev20220529/dune/fempy/function/simplegridfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/function/virtualizedgridfunction.hh` & `dune-fem-2.9.dev20220529/dune/fempy/function/virtualizedgridfunction.hh`

 * *Files 4% similar despite different names*

```diff
@@ -51,18 +51,16 @@
 
       typedef typename FunctionSpaceType::DomainType DomainType;
       typedef typename FunctionSpaceType::RangeType RangeType;
       typedef typename FunctionSpaceType::JacobianRangeType JacobianRangeType;
       typedef typename FunctionSpaceType::HessianRangeType HessianRangeType;
 
     private:
-      template <int codim>
-      using CachingPoint = FemPy::CachingPoint< GridPart, LocalCoordinateType, codim >;
-      template <int codim>
-      using ElementPoint = FemPy::ElementPoint< GridPart, LocalCoordinateType, codim >;
+      typedef FemPy::CachingPoint< LocalCoordinateType > CachingPoint;
+      typedef FemPy::ElementPoint< LocalCoordinateType > ElementPoint;
 
       // typically used quadratures for efficient evaluation of basis functions
       typedef Dune::Fem::CachingQuadrature< GridPart, 0 > ElementQuadratureType ;
       typedef Dune::Fem::CachingQuadrature< GridPart, 1 > FaceQuadratureType ;
       typedef Dune::Fem::CachingQuadrature< GridPart, 0, Dune::FemPy::FempyQuadratureTraits > ElementFemQuadratureType;
       typedef Dune::Fem::CachingQuadrature< GridPart, 1, Dune::FemPy::FempyQuadratureTraits > FaceFemQuadratureType;
 
@@ -78,28 +76,22 @@
 
       struct Interface
       {
         virtual ~Interface () = default;
         virtual Interface *clone () const = 0;
 
         virtual void evaluate ( const LocalCoordinateType &x, RangeType &value ) const = 0;
-        virtual void evaluate ( const CachingPoint<0> &x, RangeType &value ) const = 0;
-        virtual void evaluate ( const CachingPoint<1> &x, RangeType &value ) const = 0;
-        virtual void evaluate ( const ElementPoint<0> &x, RangeType &value ) const = 0;
-        virtual void evaluate ( const ElementPoint<1> &x, RangeType &value ) const = 0;
+        virtual void evaluate ( const CachingPoint &x, RangeType &value ) const = 0;
+        virtual void evaluate ( const ElementPoint &x, RangeType &value ) const = 0;
         virtual void jacobian ( const LocalCoordinateType &x, JacobianRangeType &jacobian ) const = 0;
-        virtual void jacobian ( const CachingPoint<0> &x, JacobianRangeType &jacobian ) const = 0;
-        virtual void jacobian ( const CachingPoint<1> &x, JacobianRangeType &jacobian ) const = 0;
-        virtual void jacobian ( const ElementPoint<0> &x, JacobianRangeType &jacobian ) const = 0;
-        virtual void jacobian ( const ElementPoint<1> &x, JacobianRangeType &jacobian ) const = 0;
+        virtual void jacobian ( const CachingPoint &x, JacobianRangeType &jacobian ) const = 0;
+        virtual void jacobian ( const ElementPoint &x, JacobianRangeType &jacobian ) const = 0;
         virtual void hessian ( const LocalCoordinateType &x, HessianRangeType &hessian ) const = 0;
-        virtual void hessian ( const CachingPoint<0> &x, HessianRangeType &hessian ) const = 0;
-        virtual void hessian ( const CachingPoint<1> &x, HessianRangeType &hessian ) const = 0;
-        virtual void hessian ( const ElementPoint<0> &x, HessianRangeType &hessian ) const = 0;
-        virtual void hessian ( const ElementPoint<1> &x, HessianRangeType &hessian ) const = 0;
+        virtual void hessian ( const CachingPoint &x, HessianRangeType &hessian ) const = 0;
+        virtual void hessian ( const ElementPoint &x, HessianRangeType &hessian ) const = 0;
 
         virtual void evaluateQuadrature( const ElementQuadratureType& quad, RangeValueVectorType& values ) const = 0 ;
         virtual void evaluateQuadrature( const FaceQuadratureType& quad, RangeValueVectorType& values ) const = 0 ;
         virtual void evaluateQuadrature( const ElementFemQuadratureType& quad, RangeValueVectorType& values ) const = 0 ;
         virtual void evaluateQuadrature( const FaceFemQuadratureType& quad, RangeValueVectorType& values ) const = 0 ;
         virtual void jacobianQuadrature( const ElementQuadratureType& quad, JacobianRangeValueVectorType& values ) const = 0 ;
         virtual void jacobianQuadrature( const FaceQuadratureType& quad, JacobianRangeValueVectorType& values ) const = 0 ;
@@ -125,28 +117,22 @@
           impl_( gf )
         {
         }
 
         virtual Interface *clone () const override { return new Implementation( *this ); }
 
         virtual void evaluate ( const LocalCoordinateType &x, RangeType &value ) const override { impl().evaluate( x, value ); }
-        virtual void evaluate ( const CachingPoint<0> &x, RangeType &value ) const override { impl().evaluate( asQP( x ), value ); }
-        virtual void evaluate ( const CachingPoint<1> &x, RangeType &value ) const override { impl().evaluate( asQP( x ), value ); }
-        virtual void evaluate ( const ElementPoint<0> &x, RangeType &value ) const override { impl().evaluate( asQP( x ), value ); }
-        virtual void evaluate ( const ElementPoint<1> &x, RangeType &value ) const override { impl().evaluate( asQP( x ), value ); }
+        virtual void evaluate ( const CachingPoint &x, RangeType &value ) const override { impl().evaluate( asQP( x ), value ); }
+        virtual void evaluate ( const ElementPoint &x, RangeType &value ) const override { impl().evaluate( asQP( x ), value ); }
         virtual void jacobian ( const LocalCoordinateType &x, JacobianRangeType &jacobian ) const override { impl().jacobian( x, jacobian ); }
-        virtual void jacobian ( const CachingPoint<0> &x, JacobianRangeType &jacobian ) const override { impl().jacobian( asQP( x ), jacobian ); }
-        virtual void jacobian ( const CachingPoint<1> &x, JacobianRangeType &jacobian ) const override { impl().jacobian( asQP( x ), jacobian ); }
-        virtual void jacobian ( const ElementPoint<0> &x, JacobianRangeType &jacobian ) const override { impl().jacobian( asQP( x ), jacobian ); }
-        virtual void jacobian ( const ElementPoint<1> &x, JacobianRangeType &jacobian ) const override { impl().jacobian( asQP( x ), jacobian ); }
+        virtual void jacobian ( const CachingPoint &x, JacobianRangeType &jacobian ) const override { impl().jacobian( asQP( x ), jacobian ); }
+        virtual void jacobian ( const ElementPoint &x, JacobianRangeType &jacobian ) const override { impl().jacobian( asQP( x ), jacobian ); }
         virtual void hessian ( const LocalCoordinateType &x, HessianRangeType &hessian ) const override { impl().hessian( x, hessian ); }
-        virtual void hessian ( const CachingPoint<0> &x, HessianRangeType &hessian ) const override { impl().hessian( asQP( x ), hessian ); }
-        virtual void hessian ( const CachingPoint<1> &x, HessianRangeType &hessian ) const override { impl().hessian( asQP( x ), hessian ); }
-        virtual void hessian ( const ElementPoint<0> &x, HessianRangeType &hessian ) const override { impl().hessian( asQP( x ), hessian ); }
-        virtual void hessian ( const ElementPoint<1> &x, HessianRangeType &hessian ) const override { impl().hessian( asQP( x ), hessian ); }
+        virtual void hessian ( const CachingPoint &x, HessianRangeType &hessian ) const override { impl().hessian( asQP( x ), hessian ); }
+        virtual void hessian ( const ElementPoint &x, HessianRangeType &hessian ) const override { impl().hessian( asQP( x ), hessian ); }
         virtual void evaluateQuadrature( const ElementQuadratureType& quad, RangeValueVectorType& values ) const override { impl().evaluateQuadrature( quad, values ); }
         virtual void evaluateQuadrature( const FaceQuadratureType& quad, RangeValueVectorType& values ) const override { impl().evaluateQuadrature( quad, values ); }
         virtual void evaluateQuadrature( const ElementFemQuadratureType& quad, RangeValueVectorType& values ) const override { impl().evaluateQuadrature( quad, values ); }
         virtual void evaluateQuadrature( const FaceFemQuadratureType& quad, RangeValueVectorType& values ) const override { impl().evaluateQuadrature( quad, values ); }
         virtual void jacobianQuadrature( const ElementQuadratureType& quad, JacobianRangeValueVectorType& values ) const override { impl().jacobianQuadrature( quad, values ); }
         virtual void jacobianQuadrature( const FaceQuadratureType& quad, JacobianRangeValueVectorType& values ) const override { impl().jacobianQuadrature( quad, values ); }
         virtual void jacobianQuadrature( const ElementFemQuadratureType& quad, JacobianRangeValueVectorType& values ) const override { impl().jacobianQuadrature( quad, values ); }
@@ -208,59 +194,59 @@
         using Fem::coordinate;
         impl_->evaluate( coordinate( x ), value );
       }
       template< class Quadrature >
       std::enable_if_t< std::is_convertible< Quadrature, Fem::CachingInterface >::value >
       evaluate ( const Fem::QuadraturePointWrapper< Quadrature > &x, RangeType &value ) const
       {
-        impl_->evaluate( CachingPoint<Quadrature::codimension>( x ), value );
+        impl_->evaluate( CachingPoint( x ), value );
       }
       template< class Quadrature >
       std::enable_if_t< !std::is_convertible< Quadrature, Fem::CachingInterface >::value >
       evaluate ( const Fem::QuadraturePointWrapper< Quadrature > &x, RangeType &value ) const
       {
-        impl_->evaluate( ElementPoint<Quadrature::codimension>( x ), value );
+        impl_->evaluate( ElementPoint( x ), value );
       }
 
       template< class Point >
       void jacobian ( const Point &x, JacobianRangeType &jacobian ) const
       {
         using Fem::coordinate;
         impl_->jacobian( coordinate( x ), jacobian );
       }
       template< class Quadrature >
       std::enable_if_t< std::is_convertible< Quadrature, Fem::CachingInterface >::value >
       jacobian ( const Fem::QuadraturePointWrapper< Quadrature > &x, JacobianRangeType &jacobian ) const
       {
-        impl_->jacobian( CachingPoint<Quadrature::codimension>( x ), jacobian );
+        impl_->jacobian( CachingPoint( x ), jacobian );
       }
       template< class Quadrature >
       std::enable_if_t< !std::is_convertible< Quadrature, Fem::CachingInterface >::value >
       jacobian ( const Fem::QuadraturePointWrapper< Quadrature > &x, JacobianRangeType &jacobian ) const
       {
-        impl_->jacobian( ElementPoint<Quadrature::codimension>( x ), jacobian );
+        impl_->jacobian( ElementPoint( x ), jacobian );
       }
 
       template< class Point >
       void hessian ( const Point &x, HessianRangeType &hessian ) const
       {
         using Fem::coordinate;
         impl_->hessian( coordinate( x ), hessian );
       }
       template< class Quadrature >
       std::enable_if_t< std::is_convertible< Quadrature, Fem::CachingInterface >::value >
       hessian ( const Fem::QuadraturePointWrapper< Quadrature > &x, HessianRangeType &hessian ) const
       {
-        impl_->hessian( CachingPoint<Quadrature::codimension>( x ), hessian );
+        impl_->hessian( CachingPoint( x ), hessian );
       }
       template< class Quadrature >
       std::enable_if_t< !std::is_convertible< Quadrature, Fem::CachingInterface >::value >
       hessian ( const Fem::QuadraturePointWrapper< Quadrature > &x, HessianRangeType &hessian ) const
       {
-        impl_->hessian( ElementPoint<Quadrature::codimension>( x ), hessian );
+        impl_->hessian( ElementPoint( x ), hessian );
       }
 
       template< class Quadrature, class ... Vectors >
       void evaluateQuadrature ( const Quadrature &quad, Vectors & ... values ) const
       {
         static_assert( sizeof...( Vectors ) > 0, "evaluateQuadrature needs to be called with at least one vector." );
         std::ignore = std::make_tuple( ( evaluateSingleQuadrature( quad, values ), 1 ) ... );
```

### Comparing `dune-fem-2.9.0rc1/dune/fempy/geometry/edgelength.hh` & `dune-fem-2.9.dev20220529/dune/fempy/geometry/edgelength.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/grid/adaptation.hh` & `dune-fem-2.9.dev20220529/dune/fempy/grid/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/grid/discretefunctionmanager.hh` & `dune-fem-2.9.dev20220529/dune/fempy/grid/discretefunctionmanager.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/grid/globalmapper.hh` & `dune-fem-2.9.dev20220529/dune/fempy/grid/globalmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/grid/virtualizedrestrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fempy/grid/virtualizedrestrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/parameter.hh` & `dune-fem-2.9.dev20220529/dune/fempy/parameter.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/common/numpyvector.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/common/numpyvector.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/discretefunction.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/discretefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/function/grid.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/function/grid.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/grid/adaptation.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/grid/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/grid/function.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/grid/function.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/grid/gridpart.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/grid/gridpart.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/grid/numpy.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/grid/numpy.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/grid/restrictprolong.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/grid/restrictprolong.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/gridview.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/gridview.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/integrands.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/integrands.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/integrandsbase.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/integrandsbase.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/operator.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/operator.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/scheme.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/scheme.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/space.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/space.hh`

 * *Files 3% similar despite different names*

```diff
@@ -116,16 +116,14 @@
       }
 
       template< class Space, class... options >
       void registerSpace ( pybind11::handle module, pybind11::class_< Space, options... > cls )
       {
         registerFunctionSpace(module,cls);
         cls.def_property_readonly( "size", [] ( Space &self ) -> int { return self.size(); } );
-        cls.def_property_readonly( "primarySize", [] ( Space &self ) -> int { return self.primarySize(); } );
-        cls.def_property_readonly( "auxiliarySize", [] ( Space &self ) -> int { return self.auxiliarySize(); } );
         cls.def_property_readonly( "_sizeOfField", [] ( Space &self ) -> unsigned int { return sizeof(typename Space::RangeFieldType); } );
         cls.def_property_readonly( "localBlockSize", [] ( Space &spc ) -> unsigned int { return spc.localBlockSize; } );
         cls.def("localOrder", [] ( Space &self, typename Space::EntityType &e) -> int { return self.order(e); } );
         cls.def("map", [] ( Space &spc, typename Space::EntityType &e) -> std::vector<unsigned int>
             { std::vector<unsigned int> idx(spc.blockMapper().numDofs(e));
               spc.blockMapper().mapEach(e, Fem::AssignFunctor< std::vector< unsigned int > >( idx ) );
               return idx;
```

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/spaceadapt.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/spaceadapt.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/py/ufllocalfunction.hh` & `dune-fem-2.9.dev20220529/dune/fempy/py/ufllocalfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/pybind11/gridfunction.hh` & `dune-fem-2.9.dev20220529/dune/fempy/pybind11/gridfunction.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/pybind11/space.hh` & `dune-fem-2.9.dev20220529/dune/fempy/pybind11/space.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/quadrature/cachingpoint.hh` & `dune-fem-2.9.dev20220529/dune/fempy/quadrature/cachingpoint.hh`

 * *Files 18% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
   namespace FemPy
   {
 
     // CachingPoint
     // ------------
 
-    template< class GridPart, class Coordinate, int codim > // = 0 >
+    template< class Coordinate, int codim = 0 >
     struct CachingPoint;
 
-    template< class GridPart, class Coordinate >
-    struct CachingPoint< GridPart, Coordinate, 0 >
+    template< class Coordinate >
+    struct CachingPoint< Coordinate, 0 >
       : public Fem::CachingInterface
     {
-      typedef CachingPoint< GridPart, Coordinate, 0 > This;
+      typedef CachingPoint< Coordinate, 0 > This;
 
     public:
       static const int codimension = 0 ;
 
       typedef Coordinate CoordinateType;
       typedef typename FieldTraits< Coordinate >::real_type RealType;
       typedef Coordinate LocalCoordinateType;
@@ -57,63 +57,55 @@
       std::size_t cachingPoint ( std::size_t qp ) const { assert( qp == 0u ); return idx_; }
 
     private:
       std::size_t id_, idx_;
       const CoordinateType &position_;
     };
 
-    template< class GridPart, class Coordinate >
-    struct CachingPoint< GridPart, Coordinate, 1 >
+    template< class Coordinate >
+    struct CachingPoint< Coordinate, 1 >
       : public Fem::CachingInterface
     {
-      typedef CachingPoint< GridPart, Coordinate, 1 > This;
+      typedef CachingPoint< Coordinate, 1 > This;
 
     public:
       static const int codimension = 1 ;
 
       typedef Coordinate CoordinateType;
       typedef typename FieldTraits< Coordinate >::real_type RealType;
       typedef FieldVector< typename FieldTraits< Coordinate >::field_type, Coordinate::dimension-1 > LocalCoordinateType;
-      typedef typename GridPart::IntersectionType IntersectionType;
 
       template< class Quadrature, std::enable_if_t< std::is_convertible< Quadrature, Fem::CachingInterface >::value, int > = 0 >
       CachingPoint ( const Quadrature &quadrature, std::size_t idx )
         : id_( quadrature.id() ),
           idx_( quadrature.cachingPoint( idx ) ),
           position_( quadrature.point( idx ) ),
-          localPosition_( quadrature.localPoint( idx ) ),
-          intersection_( quadrature.intersection() )
+          localPosition_( quadrature.localPoint( idx ) )
       {}
 
       template< class Quadrature, std::enable_if_t< std::is_convertible< Quadrature, Fem::CachingInterface >::value, int > = 0 >
       explicit CachingPoint ( const Fem::QuadraturePointWrapper< Quadrature > &x )
         : CachingPoint( x.quadrature(), x.index() )
       {}
 
       explicit operator Fem::QuadraturePointWrapper< This > () const noexcept { return Fem::QuadraturePointWrapper< This >( *this, 0u ); }
 
-      const IntersectionType &intersection() const
-      {
-        return intersection_;
-      }
-
       std::size_t id () const { return id_; }
 
       int nop() const { return 1; }
 
       const CoordinateType &point ( std::size_t qp ) const { return position_; }
       const LocalCoordinateType &localPoint ( std::size_t qp ) const { return localPosition_; }
 
       std::size_t cachingPoint ( std::size_t qp ) const { assert( qp == 0u ); return idx_; }
 
     private:
       std::size_t id_, idx_;
       const CoordinateType &position_;
       const LocalCoordinateType &localPosition_;
-      const IntersectionType &intersection_;
     };
 
   } // namespace FemPy
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_FEMPY_QUADRATURE_CACHINGPOINT_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fempy/quadrature/elementpoint.hh` & `dune-fem-2.9.dev20220529/dune/fempy/quadrature/elementpoint.hh`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 
   namespace FemPy
   {
 
     // ElementPoint
     // ------------
 
-    template< class GridPart, class Coordinate, int codim >
+    template< class Coordinate, int codim = 0 >
     struct ElementPoint;
 
-    template< class GridPart, class Coordinate >
-    struct ElementPoint< GridPart, Coordinate, 0 >
+    template< class Coordinate >
+    struct ElementPoint< Coordinate, 0 >
     {
-      typedef ElementPoint< GridPart, Coordinate, 0 > This;
+      typedef ElementPoint< Coordinate, 0 > This;
 
     public:
-      static const int codimension = 0 ;
       typedef Coordinate CoordinateType;
       typedef typename FieldTraits< Coordinate >::real_type RealType;
       typedef Coordinate LocalCoordinateType;
 
       template< class Quadrature >
       ElementPoint ( const Quadrature &quadrature, std::size_t idx )
         : position_( quadrature.point( idx ) )
@@ -46,52 +45,43 @@
       const CoordinateType &point ( std::size_t qp ) const { return position_; }
       const LocalCoordinateType &localPoint ( std::size_t qp ) const { return position_; }
 
     private:
       const CoordinateType &position_;
     };
 
-    template< class GridPart, class Coordinate >
-    struct ElementPoint< GridPart, Coordinate, 1 >
+    template< class Coordinate >
+    struct ElementPoint< Coordinate, 1 >
     {
-      typedef ElementPoint< GridPart, Coordinate, 1 > This;
+      typedef ElementPoint< Coordinate, 1 > This;
 
     public:
-      static const int codimension = 1 ;
       typedef Coordinate CoordinateType;
       typedef typename FieldTraits< Coordinate >::real_type RealType;
       typedef FieldVector< typename FieldTraits< Coordinate >::field_type, Coordinate::dimension-1 > LocalCoordinateType;
-      typedef typename GridPart::IntersectionType IntersectionType;
 
       template< class Quadrature >
       ElementPoint ( const Quadrature &quadrature, std::size_t idx )
         : position_( quadrature.point( idx ) ),
-          localPosition_( quadrature.localPoint( idx ) ),
-          intersection_( quadrature.intersection() )
+          localPosition_( quadrature.localPoint( idx ) )
       {}
 
       template< class Quadrature >
       explicit ElementPoint ( const Fem::QuadraturePointWrapper< Quadrature > &x )
         : ElementPoint( x.quadrature(), x.index() )
       {}
 
       explicit operator Fem::QuadraturePointWrapper< This > () const noexcept { return Fem::QuadraturePointWrapper< This >( *this, 0u ); }
 
       const CoordinateType &point ( std::size_t qp ) const { return position_; }
       const LocalCoordinateType &localPoint ( std::size_t qp ) const { return localPosition_; }
 
-      const IntersectionType &intersection() const
-      {
-        return intersection_;
-      }
-
     private:
       CoordinateType position_;
       const LocalCoordinateType &localPosition_;
-      const IntersectionType &intersection_;
     };
 
   } // namespace FemPy
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_FEMPY_QUADRATURE_ELEMENTPOINT_HH
```

### Comparing `dune-fem-2.9.0rc1/dune/fempy/quadrature/fempyquadratures.hh` & `dune-fem-2.9.dev20220529/dune/fempy/quadrature/fempyquadratures.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/space/adaptation.hh` & `dune-fem-2.9.dev20220529/dune/fempy/space/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/CMakeLists.txt` & `dune-fem-2.9.dev20220529/dune/fempy/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/backrest1.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/backrest1.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/backrest2.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/backrest2.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/codegen.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/codegen.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/fempy-bcrsmatrix.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/fempy-bcrsmatrix.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/fenics-elasticity.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/fenics-elasticity.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/fenics-heat.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/fenics-heat.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/fenics-poisson.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/fenics-poisson.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/filteredgridview.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/filteredgridview.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/interpolate.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/interpolate.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/levelspaces.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/levelspaces.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/localcontexttest.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/localcontexttest.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/mixed.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/mixed.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/scheme_assemble.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/scheme_assemble.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/test-quad.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/test-quad.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/test-tupledf.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/test-tupledf.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/test_assembly.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/test_assembly.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/test_quad.hpp` & `dune-fem-2.9.dev20220529/dune/fempy/test/test_quad.hpp`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/testd2.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/testd2.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/testnVector.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/testnVector.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/testoperator.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/testoperator.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/testvecbackends.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/testvecbackends.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune/fempy/test/vtktest.py` & `dune-fem-2.9.dev20220529/dune/fempy/test/vtktest.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/dune.module` & `dune-fem-2.9.dev20220529/dune.module`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Module: dune-fem
-Version: 2.9
+Version: 2.9-git
 Author: The Dune-Fem developer team
 Maintainer: dune-fem@lists.dune-project.org
 Description: A discretization module providing an implementation of mathematical abstractions to solve PDEs on parallel computers including local grid adaptivity, dynamic load balancing, and higher order discretization schemes
 URL: https://gitlab.dune-project.org/dune-fem/dune-fem
 Python-Requires: matplotlib scipy fenics-ufl==2019.1.0 dune-alugrid dune-istl dune-localfunctions
 Depends: dune-grid (>= 2.9) dune-alugrid (>= 2.9) dune-istl (>= 2.9) dune-localfunctions (>= 2.9)
 Suggests: dune-spgrid (>= 2.9) dune-polygongrid
```

### Comparing `dune-fem-2.9.0rc1/pydemo/advectiondiffusion.py` & `dune-fem-2.9.dev20220529/pydemo/advectiondiffusion.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/pydemo/testthreading.py` & `dune-fem-2.9.dev20220529/pydemo/testthreading.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/__init__.py` & `dune-fem-2.9.dev20220529/python/dune/fem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from . import view as view
 from . import space as space
 from . import discretefunction as discretefunction
 from . import operator as operator
 from . import scheme as scheme
 from . import function as function
 from . import model as model
-from . import plotting
 
 # finalization of fem module (i.e. calling PETSc finalize etc)
 atexit.register( _fem.__finalizeFemModule__ )
 
 registry = {}
 
 registry["view"] = {
```

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/__main__.py` & `dune-fem-2.9.dev20220529/python/dune/fem/__main__.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/_adaptation.py` & `dune-fem-2.9.dev20220529/python/dune/fem/_adaptation.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/_fem.cc` & `dune-fem-2.9.dev20220529/python/dune/fem/_fem.cc`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
       Dune::Fem::detail::SingletonStorage::getStorage();
       module.attr( "_singleton" ) = pybind11::cast( Dune::Fem::detail::SingletonStorage::storage_ );
     }
     int argc = 0;
     char **argv = nullptr;
     Dune::Fem::MPIManager::initialize( argc, argv );
 
-    if( !pybind11::already_registered< Dune::Fem::MPIManager::Communication >() )
-      DUNE_THROW( Dune::Exception, "Communication not registered, yet" );
+    if( !pybind11::already_registered< Dune::Fem::MPIManager::CollectiveCommunication >() )
+      DUNE_THROW( Dune::Exception, "CollectiveCommunication not registered, yet" );
 
     module.attr( "comm" ) = pybind11::cast( Dune::Fem::MPIManager::comm() );
   }
   catch ( const std::exception &e )
   {
     std::cout << e.what() << std::endl;
   }
```

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/_spaceadaptation.py` & `dune-fem-2.9.dev20220529/python/dune/fem/_spaceadaptation.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/discretefunction/_discretefunctions.py` & `dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/_discretefunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,15 @@
         headers = ["dune/fem/function/adaptivefunction.hh"]
     elif dfStorage == "istl":
         dfType  = lambda space: "Dune::Fem::ISTLBlockVectorDiscreteFunction< " + space.cppTypeName + " >"
         headers = ["dune/fem/function/blockvectorfunction.hh"]
     elif dfStorage == "petsc":
         dfType  = lambda space: "Dune::Fem::PetscDiscreteFunction< " + space.cppTypeName + " >"
         headers = ["dune/fem/function/petscdiscretefunction.hh"]
-    else:
-        raise ValueError(f"_storage: wrong discrete function storage {dfStorage}. Valid are 'numpy','petsc','istl'")
+
 
     rdfType = lambda space,rspace: dfType(space if rspace is None else rspace)
 
     # as_numpy, as_istl, as_petsc
     asStorage = "as_" + dfStorage
 
     if solverStorage == "numpy":
@@ -82,16 +81,14 @@
             dfStorage,\
             headers + ["dune/fem/operator/linear/petscoperator.hh"] + petscheader + space.cppIncludes,\
             dfType(space),\
             equalSpaces(space,rspace),\
             solvers.petscsolver,\
             asStorage
         ]
-    else:
-        raise ValueError(f"_storage: wrong discrete function storage {dfStorage}. Valid are 'numpy','petsc','istl'")
 
 def numpy():
     return _storage(dfStorage="numpy")
 
 def istl():
     return _storage(dfStorage="istl")
```

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/discretefunction/_solvers.py` & `dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/_solvers.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/discretefunction/adaptive.py` & `dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/adaptive.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/discretefunction/eigen.py` & `dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/eigen.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/discretefunction/istl.py` & `dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/istl.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/discretefunction/numpy.py` & `dune-fem-2.9.dev20220529/python/dune/fem/discretefunction/numpy.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/function/_functions.py` & `dune-fem-2.9.dev20220529/python/dune/fem/function/_functions.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/model/_models.py` & `dune-fem-2.9.dev20220529/python/dune/fem/model/_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,22 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import sys
 import logging
 logger = logging.getLogger(__name__)
 
 import dune.common.checkconfiguration as checkconfiguration
-from dune.ufl import DirichletBC
-
-def warnNewCartesianIds(view,*args):
-    try:
-        needsChecking = view.hierarchicalGrid._cartesianConstructionWithIds
-    except AttributeError:
-        needsChecking = False
-
-    if needsChecking:
-        dirichletBCs = [arg for arg in args
-                        if isinstance(arg, DirichletBC)]
-        if ( len(dirichletBCs) == 1
-                 and isinstance(dirichletBCs[0].subDomain,int)
-                 and dirichletBCs[0].subDomain==1 ):
-            print(
-"""
-Warning: note that the boundary ids of the Cartesian domain have changed
-for some unstructured grids (alu and mmesh). They are now set according to
-the convention for structured grids based on the dune reference element, i.e.,
-in 2d left=1, right=2, bottom=3, top=4. How to get rid of this warning:
-
-- You can switch to the old ids by passing 'boundary=False' to the
-  'cartesianDomain' function. But this option will be removed soon.
-- If you want to set boundary conditions on the whole boundary you can remove the
-  final parameter ('subDomain') from the 'DirichletBC' class.
-- If you are already using the new boundary ids and want only Dirichlet
-  conditions on the left side (so the warning is wrongly provided) then
-  please add a second 'DirichletBC' instance to the scheme constructor with
-  a boundary id above 2^dim - sorry about this...
-""")
 
 def conservationlaw(view, equation, *args, **kwargs):
     import ufl
     import dune.ufl
     import dune.models.conservationlaw as conservationlaw
 
     coefficients = kwargs.pop('coefficients', dict())
 
-    warnNewCartesianIds(view,*args)
     Model = conservationlaw.load(view, equation, *args, **kwargs).Model
     # the following needs to be done for the linearized problem:
     # if isinstance(equation, ufl.equation.Equation):
     #     lhs = ufl.algorithms.expand_indices(ufl.algorithms.expand_derivatives(ufl.algorithms.expand_compounds(equation.lhs)))
     #     if lhs == ufl.adjoint(lhs):
     #         setattr(Model, 'symmetric', 'true')
     #    else:
@@ -65,13 +34,12 @@
     import dune.models.integrands as integrands
 
     tempVars   = kwargs.pop('tempVars', True)
     virtualize = kwargs.pop('virtualize',True)
     modelPatch = kwargs.pop('modelPatch',None)
     includes   = kwargs.pop('includes',None)
 
-    warnNewCartesianIds(view,*args)
     Integrands = integrands.load(view, form, *args,
                      tempVars=tempVars,virtualize=virtualize,
                      modelPatch=modelPatch,includes=includes)
 
     return Integrands(*args, **kwargs)
```

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/operator/__init__.py` & `dune-fem-2.9.dev20220529/python/dune/fem/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/plotting.py` & `dune-fem-2.9.dev20220529/python/dune/fem/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from dune.plotting import block, disable
 from ufl import as_vector
 globalBlock = block
 
 def triangulationOfNetwork(grid, level=0, linewidth=0.01):
     from matplotlib.tri import Triangulation
-    x, t = grid.tessellate(level)
+    x, t = grid.tesselate(level)
     n, m = len(x), len(t)
     t = append(t.T, [zeros(m, dtype=int32)], axis=0).T
     t = append(t, zeros((m,3), dtype=int32), axis=0)
     x = append(x, zeros((2*m,2)), axis=0)
     for i in range(m):
         i0 = n+2*i
         t[i][2] = i0
@@ -47,15 +47,15 @@
         data = solution.pointData(level)
 
         if grid.dimGrid == 1 and grid.dimWorld == 1:
             if solution.dimRange > 1:
                 data = linalg.norm(solution.pointData(level),axis=1)
             else:
                 data = solution.pointData(level)[:,0]
-            pyplot.plot(grid.tessellate(level)[0], data, '-p')
+            pyplot.plot(grid.tesselate(level)[0], data, '-p')
             if xlim:
                 fig.gca().set_xlim(xlim)
             fig.tight_layout()
             return
 
         if grid.dimGrid == 1:
             triangulation = triangulationOfNetwork(grid, level, linewidth)
@@ -89,18 +89,14 @@
             if logscale:
                 data = abs(data)
                 logNorm = {"norm":LogNorm()}
             else:
                 logNorm = {}
             minData = amin(data)
             maxData = amax(data)
-            r = maxData-minData
-            # avoid some weird 'white' patches when value hits min/max
-            minData -= r*0.01
-            maxData += r*0.01
             if clim == None:
                 clim = [minData, maxData]
             # having extend not 'both' does not seem to work (needs fixing)...
             if clim[0] > minData and clim[1] < maxData:
                 extend = 'both'
             elif clim[0] > minData:
                 extend = 'min'
```

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/scheme/__init__.py` & `dune-fem-2.9.dev20220529/python/dune/fem/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/scheme/_schemes.py` & `dune-fem-2.9.dev20220529/python/dune/fem/scheme/_schemes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     """
     Return storage that fits chosen solver (default: space.storage)
     """
     from dune.fem.discretefunction import _storage
     storage = space.storage
 
     # this feature only works for numpy storage of the space
-    if storage[0] == 'numpy' and isinstance(solver, tuple) and len(solver) > 1:
-        try:
+    if storage[0] == 'numpy' and solver is not None:
+        if isString(solver[0]):
             # changing the storage only works for petsc and istl, but is not needed for suitesparse
-            return _storage(dfStorage=storage[0], solverStorage=solver[0])(space), solver[1]
-        except ValueError:
-            pass
+            if solver[0] == 'petsc' or solver[0] == 'istl':
+                # return storage and solver name
+                return _storage(dfStorage="numpy", solverStorage=solver[0])(space), solver[1]
 
     # otherwise simply return arguments that were passed
     return storage, solver
 
 def getSolver(solver, storage, default):
     if not solver:
         return default(storage)
```

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/scheme/dgmodel.py` & `dune-fem-2.9.dev20220529/python/dune/fem/scheme/dgmodel.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/space/__init__.py` & `dune-fem-2.9.dev20220529/python/dune/fem/space/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/space/_spaces.py` & `dune-fem-2.9.dev20220529/python/dune/fem/space/_spaces.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fem/view.py` & `dune-fem-2.9.dev20220529/python/dune/fem/view.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/fenics/_compatibility.py` & `dune-fem-2.9.dev20220529/python/dune/fenics/_compatibility.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/conservationlaw/__init__.py` & `dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/conservationlaw/compiler.py` & `dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/compiler.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/conservationlaw/formfiles.py` & `dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/formfiles.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/conservationlaw/model.py` & `dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/conservationlaw/ufl.py` & `dune-fem-2.9.dev20220529/python/dune/models/conservationlaw/ufl.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/integrands/compiler.py` & `dune-fem-2.9.dev20220529/python/dune/models/integrands/compiler.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/integrands/formfiles.py` & `dune-fem-2.9.dev20220529/python/dune/models/integrands/formfiles.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/integrands/load.py` & `dune-fem-2.9.dev20220529/python/dune/models/integrands/load.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/integrands/model.py` & `dune-fem-2.9.dev20220529/python/dune/models/integrands/model.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/models/integrands/ufl.py` & `dune-fem-2.9.dev20220529/python/dune/models/integrands/ufl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 from ufl.equation import Equation
 from ufl import UFLException
 from dune.ufl.tensors import ExprTensor
 from dune.source.cplusplus import UnformattedExpression, SwitchStatement, Declaration, UnformattedBlock, assign, Block, ConstructExpression
 
 from dune.source.builtin import make_pair
 from dune.source.cplusplus import InitializerList, Variable
-from dune.source.cplusplus import construct, lambda_, makeExpression,\
-                                  maxEdgeLength, minEdgeLength, return_,\
-                                  boundaryIdFct
+from dune.source.cplusplus import construct, lambda_, makeExpression, maxEdgeLength, minEdgeLength, return_
 from dune.source.cplusplus import SourceWriter
 from dune.source.algorithm.extractvariables import extractVariablesFromExpressions, extractVariablesFromStatements
 
 from dune.common.hashit import hashIt
 
-from dune.ufl import codegen, DirichletBC, Constant, BoundaryId
+from dune.ufl import codegen, DirichletBC
 from dune.ufl.gatherderivatives import gatherDerivatives
 from dune.ufl.linear import splitForm
 import dune.ufl.tensors as tensors
 
 from .model import Integrands
 
 def generateCode(predefined, testFunctions, tensorMap, tempVars=True):
@@ -222,25 +220,23 @@
 
     derivatives = gatherDerivatives(form, [phi, u])
 
     derivatives_phi = derivatives[0]
     derivatives_u = derivatives[1]
     derivatives_ubar = map_expr_dags(Replacer({u: ubar}), derivatives_u)
 
-    boundaryId = BoundaryId( form.ufl_cell() )
-
     try:
         integrands.field = u.ufl_function_space().field
     except AttributeError:
         pass
 
-    integrals = splitForm(form, [phi], boundaryId)
+    integrals = splitForm(form, [phi])
 
     dform = apply_derivatives(derivative(action(form, ubar), ubar, u))
-    linearizedIntegrals = splitForm(dform, [phi, u], boundaryId)
+    linearizedIntegrals = splitForm(dform, [phi, u])
 
     if not set(integrals.keys()) <= {'cell', 'exterior_facet', 'interior_facet'}:
         raise Exception('unknown integral encountered in ' + str(set(integrals.keys())) + '.')
 
     if 'cell' in integrals.keys():
         arg = Variable(integrands.domainValueTuple, 'u')
 
@@ -260,28 +256,26 @@
         integrands.predefineCoefficients(predefined, False)
         integrands.linearizedInterior = generateUnaryLinearizedCode(predefined, derivatives_phi, derivatives_u, linearizedIntegrals.get('cell'), tempVars=tempVars)
 
     if 'exterior_facet' in integrals.keys():
         arg = Variable(integrands.domainValueTuple, 'u')
 
         predefined = {derivatives_u[i]: arg[i] for i in range(len(derivatives_u))}
-        predefined[boundaryId] = boundaryIdFct(integrands.intersection())
         predefined[x] = integrands.spatialCoordinate('x')
         predefined[n] = integrands.facetNormal('x')
         predefined[cellVolume] = integrands.cellVolume()
         predefined[maxCellEdgeLength] = maxEdgeLength(integrands.cellGeometry())
         predefined[minCellEdgeLength] = minEdgeLength(integrands.cellGeometry())
         predefined[facetArea] = integrands.facetArea()
         predefined[maxFacetEdgeLength] = maxEdgeLength(integrands.facetGeometry())
         predefined[minFacetEdgeLength] = minEdgeLength(integrands.facetGeometry())
         integrands.predefineCoefficients(predefined, False)
         integrands.boundary = generateUnaryCode(predefined, derivatives_phi, integrals['exterior_facet'], tempVars=tempVars);
 
         predefined = {derivatives_ubar[i]: arg[i] for i in range(len(derivatives_u))}
-        predefined[boundaryId] = boundaryIdFct(integrands.intersection())
         predefined[x] = integrands.spatialCoordinate('x')
         predefined[n] = integrands.facetNormal('x')
         predefined[cellVolume] = integrands.cellVolume()
         predefined[maxCellEdgeLength] = maxEdgeLength(integrands.cellGeometry())
         predefined[minCellEdgeLength] = minEdgeLength(integrands.cellGeometry())
         predefined[facetArea] = integrands.facetArea()
         predefined[maxFacetEdgeLength] = maxEdgeLength(integrands.facetGeometry())
@@ -325,15 +319,14 @@
 
     if dirichletBCs:
         integrands.hasDirichletBoundary = True
 
         predefined = {}
         # predefined[x] = UnformattedExpression('auto', 'entity().geometry().global( Dune::Fem::coordinate( ' + integrands.arg_x.name + ' ) )')
         predefined[x] = UnformattedExpression('auto', 'intersection.geometry().center( )')
-        predefined[boundaryId] = boundaryIdFct(integrands.intersection())
         integrands.predefineCoefficients(predefined, False)
 
         maxId = 0
         codeDomains = []
         bySubDomain = dict()
         neuman = []
         wholeDomain = None
```

### Comparing `dune-fem-2.9.0rc1/python/dune/models/localfunction.py` & `dune-fem-2.9.dev20220529/python/dune/models/localfunction.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/algorithm/extractincludes.py` & `dune-fem-2.9.dev20220529/python/dune/source/algorithm/extractincludes.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/algorithm/extractvariables.py` & `dune-fem-2.9.dev20220529/python/dune/source/algorithm/extractvariables.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/basemodel.py` & `dune-fem-2.9.dev20220529/python/dune/source/basemodel.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/builtin.py` & `dune-fem-2.9.dev20220529/python/dune/source/builtin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,32 @@
 from __future__ import division, print_function, unicode_literals
 
 from ..common.utility import isString
 
 from .expression import Variable
 
 class BuiltInFunction:
-    def __init__(self, header, cppType, name, namespace='std', targs=None, args=None, extra=None):
+    def __init__(self, header, cppType, name, namespace='std', targs=None, args=None):
         self.header = header
         self.cppType = cppType
-        self.fctName = name
+        self.name = name
         self.namespace = namespace
-        self.targs = None if targs is None else [a.strip() for a in targs]
+        self.tarts = None if targs is None else [a.strip() for a in targs]
         self.args = [] if args is None else [a.strip() if isString(a) else a for a in args]
-        if extra is None:
-            self.name = self.fctName
-        else:
-            self.name = self.fctName + extra.strip()
 
         if len(self.args) > 0:
             arg = self.args[len(self.args)-1]
             self.variadic = (isinstance(arg, Variable) and arg.cppType.endswith('...'))
         else:
             self.variadic = False
 
     def __call__(self, *args):
         if (len(args) != len(self.args)) and not self.variadic:
             raise Exception('Wrong number of Arguments: ' + str(len(args)) + ' (should be ' + str(len(self.args)) + ').')
         from .expression import Application, makeExpression
-        """
-        if self.extra is not None:
-            name = self.name + self.extra
-        else:
-            name = self.name
-        copy = BuiltInFunction(self.header, self.cppType, name,
-               self.namespace, self.targs, self.args, extra=None)
-        """
         return Application(self, args=[makeExpression(arg) for arg in args])
 
     def __eq__(self, other):
         if not isinstance(other, BuiltInFunction):
             return False
         if (other.namespace == self.namespace) and (other.name == self.name):
             assert (other.header == self.header)
@@ -47,44 +35,32 @@
             return False
 
     def __hash__(self):
         return hash(("BuildInFunction", self.namespace, self.cppType, self.name))
 
     def __str__(self):
         if self.namespace is None:
-            return self.fctName
+            return self.name
         else:
-            return self.namespace + '::' + self.fctName
+            return self.namespace + '::' + self.name
 
     def __repr__(self):
         return "built-in(" + str(self) + ")"
 
-not_ = BuiltInFunction('functional', 'X', 'logical_not',
-               targs=['class X'], args=['const X &x'],
-               extra="()")
-or_  = BuiltInFunction('functional', 'X', 'logical_or',
-               targs=['class X'], args=['const X &x', 'const X &y'],
-               extra="()")
-and_ = BuiltInFunction('functional', 'X', 'logical_and',
-               targs=['class X'], args=['const X &x', 'const X &y'],
-               extra="()")
-max_ = BuiltInFunction('algorithm',  'X', 'max', targs=['class X'], args=['const X &x', 'const X &y'])
-min_ = BuiltInFunction('algorithm',  'X', 'min', targs=['class X'], args=['const X &x', 'const X &y'])
+
+and_ = BuiltInFunction('algorithm', 'X', 'std::logical_and', targs=['class X'], args=['const X &x', 'const X &y'])
+max_ = BuiltInFunction('algorithm', 'X', 'max', targs=['class X'], args=['const X &x', 'const X &y'])
+min_ = BuiltInFunction('algorithm', 'X', 'min', targs=['class X'], args=['const X &x', 'const X &y'])
 
 abs_ = BuiltInFunction('cmath', 'X', 'abs', targs=['class X'], args=['const X &x'])
 atan = BuiltInFunction('cmath', 'X', 'atan', targs=['class X'], args=['const X &x'])
 atan2 = BuiltInFunction('cmath', 'X', 'atan2', targs=['class X'], args=['const X &x', 'const X &y'])
 exp = BuiltInFunction('cmath', 'X', 'exp', targs=['class X'], args=['const X &x'])
 cos = BuiltInFunction('cmath', 'X', 'cos', targs=['class X'], args=['const X &x'])
 cosh = BuiltInFunction('cmath', 'X', 'cosh', targs=['class X'], args=['const X &x'])
-
-boundaryIdFct = BuiltInFunction('dune/fem/misc/boundaryidprovider.hh', 'int',
-  'boundaryId<GridPartType>', namespace='Dune::Fem', targs=['class GridPartType','class Intersection'],
-  args=['const Intersection &intersection'])
-
 log = BuiltInFunction('cmath', 'X', 'log', targs=['class X'], args=['const X &x'])
 pow_ = BuiltInFunction('cmath', 'X', 'pow', targs=['class X'], args=['const X &x', 'const X &y'])
 sin = BuiltInFunction('cmath', 'X', 'sin', targs=['class X'], args=['const X &x'])
 sinh = BuiltInFunction('cmath', 'X', 'sinh', targs=['class X'], args=['const X &x'])
 sqrt = BuiltInFunction('cmath', 'X', 'sqrt', targs=['class X'], args=['const X &x'])
 tan = BuiltInFunction('cmath', 'X', 'tan', targs=['class X'], args=['const X &x'])
 tanh = BuiltInFunction('cmath', 'X', 'tanh', targs=['class X'], args=['const X &x'])
```

### Comparing `dune-fem-2.9.0rc1/python/dune/source/common.py` & `dune-fem-2.9.dev20220529/python/dune/source/common.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/cplusplus.py` & `dune-fem-2.9.dev20220529/python/dune/source/cplusplus.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/expression.py` & `dune-fem-2.9.dev20220529/python/dune/source/expression.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/fem.py` & `dune-fem-2.9.dev20220529/python/dune/source/fem.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/formatter/expression.py` & `dune-fem-2.9.dev20220529/python/dune/source/formatter/expression.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/function.py` & `dune-fem-2.9.dev20220529/python/dune/source/function.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/source/operator.py` & `dune-fem-2.9.dev20220529/python/dune/source/operator.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/__init__.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -537,17 +537,7 @@
     markdown.for_type(ufl.equation.Equation, lambda e: "\\begin{equation*}" + equation2latex(e) + "\\end{equation*}")
 
     # disable warning for calling repr to UFL forms and equations
     plain.for_type(ufl.Form, lambda f, p, c: None)
     plain.for_type(ufl.equation.Equation, lambda e, p, c: None)
 except Exception as e:
     pass
-
-import ufl.geometry
-from ufl.core.ufl_type import ufl_type
-from ufl.classes import all_ufl_classes, terminal_classes, ufl_classes
-@ufl_type()
-class BoundaryId(ufl.geometry.GeometricFacetQuantity):
-    """UFL boundary id: can be used in a conditional to fix the desired boundary id."""
-    __slots__ = ()
-    name = "facetid"
-all_ufl_classes.add(BoundaryId)
```

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/applyrestrictions.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/applyrestrictions.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/codegen.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,23 +65,17 @@
         except KeyError:
             raise Exception('%s not available for this expression.' % expr._ufl_class_.__name__)
 
     def abs(self, expr, x):
         self.using.add(Using(cplusplus.abs_))
         return self._makeTmp(cplusplus.abs_(x))
 
-    def not_condition(self, o, x):
-        self.using.add(Using(cplusplus.not_))
-        return self._makeTmp(cplusplus.not_(x))
-    def and_condition(self, expr, left, right):
+    def AndCondition(self, expr, left, right):
         self.using.add(Using(cplusplus.and_))
         return self._makeTmp(cplusplus.and_(left, right))
-    def or_condition(self, expr, left, right):
-        self.using.add(Using(cplusplus.or_))
-        return self._makeTmp(cplusplus.or_(left, right))
 
     def argument(self, expr):
         try:
             return self._makeTmp(self.predefined[expr], True)
         except KeyError:
             raise Exception('Unknown argument: ' + str(expr.number()))
 
@@ -89,16 +83,14 @@
         self.using.add(Using(cplusplus.atan))
         return self._makeTmp(cplusplus.atan(x))
 
     def atan_2(self, expr, x, y):
         self.using.add(Using(cplusplus.atan2))
         return self._makeTmp(cplusplus.atan2(x, y))
 
-    boundary_id = _require_predefined
-
     cell_volume = _require_predefined
 
     def coefficient(self, expr):
         try:
             return self._makeTmp(self.predefined[expr], True)
         except KeyError:
             pass
@@ -556,17 +548,14 @@
     def facetNormal(self, x):
         return UnformattedExpression('GlobalCoordinateType', 'intersection_.unitOuterNormal( ' + x + '.localPosition() )')
 
     def cellVolume(self, side=None):
         entity = 'entity()' if side is None else 'entity_[ static_cast< std::size_t >( ' + side + ' ) ]'
         return UnformattedExpression('auto', entity + '.geometry().volume()')
 
-    def intersection(self):
-        return UnformattedExpression('auto', 'intersection_')
-
     def cellGeometry(self, side=None):
         entity = 'entity()' if side is None else 'entity_[ static_cast< std::size_t >( ' + side + ' ) ]'
         return UnformattedExpression('auto', entity + '.geometry()')
 
     def facetArea(self):
         return UnformattedExpression('auto', 'intersection_.geometry().volume()')
```

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/gatherderivatives.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/gatherderivatives.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/latex.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/latex.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/linear.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/linear.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from ufl.differentiation import Grad
 from ufl.restriction import Restricted
 
 from .applyrestrictions import applyRestrictions
 
 from .tensors import conditionalExprTensor, ExprTensor, keys
 
-from ufl import conditional, eq
-
 def sumTensorMaps(left, right):
     result = {key: l.copy() for key, l in left.items()}
     for key, r in right.items():
         l = left.get(key)
         result[key] = r.copy() if l is None else l + r
     return result
 
@@ -175,37 +173,26 @@
 
 
 def splitMultiLinearExpr(expr, arguments=None):
     if arguments is None:
         arguments = extract_arguments(expr)
     return MultiLinearExprSplitter(arguments).visit(expr)
 
-def splitForm(form, arguments, idFct=None):
+
+
+def splitForm(form, arguments=None):
     if arguments is None:
         arguments = form.arguments()
 
     form = applyRestrictions(form)
     form = expand_indices(apply_derivatives(apply_algebra_lowering(form)))
     form = applyRestrictions(form)
 
     integrals = {}
     for integral in form.integrals():
-        domain_id = integral.subdomain_id()
-        if type( domain_id ) is int:
-            domain_id = [domain_id]
-        if type( domain_id ) in [list,tuple]:
-            assert integral.integral_type() == 'exterior_facet',\
-                   "integral id is at the moment only available for boundary (ds)"
-            for id in domain_id:
-                assert type(id) is int and id > 0
-                a = integral.integrand() *\
-                             conditional( eq(idFct,id), 1.,0. )
-        else:
-            assert domain_id == 'everywhere'
-            a = integral.integrand()
-        right = splitMultiLinearExpr(a, arguments)
+        right = splitMultiLinearExpr(integral.integrand(), arguments)
         left = integrals.get(integral.integral_type())
         if left is not None:
             right = sumTensorMaps(left, right)
         integrals[integral.integral_type()] = right
 
     return integrals
```

### Comparing `dune-fem-2.9.0rc1/python/dune/ufl/tensors.py` & `dune-fem-2.9.dev20220529/python/dune/ufl/tensors.py`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/python/dune_fem.egg-info/PKG-INFO` & `dune-fem-2.9.dev20220529/python/dune_fem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-fem
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: A discretization module providing an implementation of mathematical abstractions to solve PDEs on parallel computers including local grid adaptivity, dynamic load balancing, and higher order discretization schemes
 Home-page: https://gitlab.dune-project.org/dune-fem/dune-fem
 Author: The Dune-Fem developer team
 Author-email: dune-fem@lists.dune-project.org
 License: UNKNOWN
 Description: DUNE-FEM
         ========
@@ -118,15 +118,15 @@
          [15]: http://faculty.cse.tamu.edu/davis/suitesparse.html
          [16]: http://www.fz-juelich.de/jsc/sionlib
          [17]: http://icl.cs.utk.edu/papi/software/index.html
          [18]: https://dune-project.org/sphinx/content/sphinx/dune-fem/
          [19]: https://gitlab.dune-project.org/dune-fem/dune-fem/-/pipelines/
         
         
-        git-74e87fef1ff200e0346b7d174471befd59a78917
+        git-05b6c5700eaebdd472d9fe71bdcb1e300a6f9293
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-fem-2.9.0rc1/python/dune_fem.egg-info/SOURCES.txt` & `dune-fem-2.9.dev20220529/python/dune_fem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/check-headers.sh` & `dune-fem-2.9.dev20220529/scripts/check-headers.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/check-opts.sh` & `dune-fem-2.9.dev20220529/scripts/check-opts.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/check-tests.sh` & `dune-fem-2.9.dev20220529/scripts/check-tests.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/fullcheck.sh` & `dune-fem-2.9.dev20220529/scripts/fullcheck.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/mpiexec.sh` & `dune-fem-2.9.dev20220529/scripts/mpiexec.sh`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_alberta.opts.unused` & `dune-fem-2.9.dev20220529/scripts/opts/config_alberta.opts.unused`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_all.opts` & `dune-fem-2.9.dev20220529/scripts/opts/config_all.opts`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_alu_cube.opts` & `dune-fem-2.9.dev20220529/scripts/opts/config_alu_cube.opts`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_alu_simplex.opts` & `dune-fem-2.9.dev20220529/scripts/opts/config_alu_simplex.opts`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_none.opts` & `dune-fem-2.9.dev20220529/scripts/opts/config_none.opts`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_spgrid.opts` & `dune-fem-2.9.dev20220529/scripts/opts/config_spgrid.opts`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/opts/config_spgrid.opts.unused` & `dune-fem-2.9.dev20220529/scripts/opts/config_spgrid.opts.unused`

 * *Files identical despite different names*

### Comparing `dune-fem-2.9.0rc1/scripts/rundocker.sh` & `dune-fem-2.9.dev20220529/scripts/rundocker.sh`

 * *Files identical despite different names*

