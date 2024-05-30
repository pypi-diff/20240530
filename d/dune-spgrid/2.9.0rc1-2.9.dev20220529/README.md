# Comparing `tmp/dune-spgrid-2.9.0rc1.tar.gz` & `tmp/dune-spgrid-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-spgrid-2.9.0rc1.tar", last modified: Fri Oct 21 08:17:12 2022, max compression
+gzip compressed data, was "dune-spgrid-2.9.dev20220529.tar", last modified: Sun May 29 21:03:49 2022, max compression
```

## Comparing `dune-spgrid-2.9.0rc1.tar` & `dune-spgrid-2.9.dev20220529.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15456 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.611901 dune-spgrid-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.611901 dune-spgrid-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/cmake/modules/DuneSpgridMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.611901 dune-spgrid-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.611901 dune-spgrid-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/doc/doxygen/main.page
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/doc/doxygen/structure.page
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.615901 dune-spgrid-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.615901 dune-spgrid-2.9.0rc1/dune/common/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/common/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/common/iostream.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.615901 dune-spgrid-2.9.0rc1/dune/grid/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.615901 dune-spgrid-2.9.0rc1/dune/grid/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/extensions/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/extensions/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/extensions/superentityiterator.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.615901 dune-spgrid-2.9.0rc1/dune/grid/spgrid/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6869 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/backuprestore.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5886 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/boundarysegmentiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/cachedpartitionlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7087 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9165 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/communication.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/cube.hh
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/decomposition.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8975 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/dgfparser.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5544 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/direction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/domain.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/entityinfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/entityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/fileio.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/geometricgridlevel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18965 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/geometrycache.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26898 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/grid.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12336 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/gridlevel.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10931 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/hierarchiciterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7534 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/hierarchicsearch.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/hindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/idset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9901 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/linkage.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/mesh.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7600 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/messagebuffer.hh
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/misc.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8183 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/multiindex.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6561 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/normal.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/partition.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/partitionlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/partitionpool.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/persistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/referencecube.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15504 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/refinement.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6659 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/superentityiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/topology.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid/tree.hh
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/spgrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/dune/grid/test/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/1dcube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/2dcube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/2dtorus.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/3dcube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/4dcube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/5dcube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/6dcube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/bndsegcheck.cc
--rwxr-xr-x   0 runner    (1001) docker     (121)      286 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/bndsegcheck.sh
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/checkbndsegiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/checkidcommunication.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/checkseiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/checktree.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8018 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/decomposition.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/test-jacobians.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6872 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/test-spgrid.cc
--rwxr-xr-x   0 runner    (1001) docker     (121)      460 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune/grid/test/test-spgrid.sh
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune-spgrid.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/dune.module
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/python/dune/spgrid/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune/spgrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune/spgrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:17:12.619902 dune-spgrid-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:12.000000 dune-spgrid-2.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.523810 dune-spgrid-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15456 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-05-29 21:03:49.523810 dune-spgrid-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.511810 dune-spgrid-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/cmake/modules/DuneSpgridMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/doc/doxygen/main.page
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/doc/doxygen/structure.page
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/dune/common/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/common/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/common/iostream.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/dune/grid/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.515810 dune-spgrid-2.9.dev20220529/dune/grid/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/extensions/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/extensions/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/extensions/superentityiterator.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.519810 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/backuprestore.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5886 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/boundarysegmentiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3657 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/cachedpartitionlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7087 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9285 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/communication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/cube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/decomposition.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9015 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/dgfparser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5544 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/direction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/domain.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/entityinfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3528 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/entityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/fileio.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/geometricgridlevel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18953 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/geometrycache.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26954 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/grid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12336 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/gridlevel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10879 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/hierarchiciterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7534 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/hierarchicsearch.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/hindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/idset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9901 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/linkage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/mesh.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/messagebuffer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/misc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8183 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/multiindex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6561 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/normal.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/partition.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/partitionlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/partitionpool.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/persistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/referencecube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15504 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/refinement.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6659 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/superentityiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/topology.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7663 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid/tree.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/spgrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.519810 dune-spgrid-2.9.dev20220529/dune/grid/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/1dcube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/2dcube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/2dtorus.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/3dcube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/4dcube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/5dcube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/6dcube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/bndsegcheck.cc
+-rwxr-xr-x   0 runner    (1001) docker     (121)      286 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/bndsegcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     4814 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/checkbndsegiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/checkidcommunication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/checkseiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/checktree.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8018 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/decomposition.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/test-jacobians.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6872 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/test-spgrid.cc
+-rwxr-xr-x   0 runner    (1001) docker     (121)      460 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune/grid/test/test-spgrid.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune-spgrid.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/dune.module
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.519810 dune-spgrid-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.519810 dune-spgrid-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.519810 dune-spgrid-2.9.dev20220529/python/dune/spgrid/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/python/dune/spgrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-05-29 21:03:48.000000 dune-spgrid-2.9.dev20220529/python/dune/spgrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:49.523810 dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:49.523810 dune-spgrid-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:49.000000 dune-spgrid-2.9.dev20220529/setup.py
```

### Comparing `dune-spgrid-2.9.0rc1/.gitlab-ci.yml` & `dune-spgrid-2.9.dev20220529/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/AUTHORS` & `dune-spgrid-2.9.dev20220529/AUTHORS`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/CHANGELOG.md` & `dune-spgrid-2.9.dev20220529/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/LICENSE` & `dune-spgrid-2.9.dev20220529/LICENSE`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/PKG-INFO` & `dune-spgrid-2.9.dev20220529/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-spgrid
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: module providing a structured grid
 Home-page: https://gitlab.dune-project.org/extensions/dune-spgrid
 Author: Martin Nolte
 Author-email: nolte.mrtn@gmail.com
 License: UNKNOWN
 Description: Dune-SPGrid
         ===========
@@ -64,15 +64,15 @@
         | `SPGRID_ANISOTROPIC`        | Anisotropic                    |
         | `SPGRID_ANISOTROPIC_SERIAL` | Anisotropic (no MPI)           |
         | `SPGRID_BISECTION`          | Bisection                      |
         | `SPGRID_BISECTION_SERIAL`   | Bisection (no MPI)             |
         | `SPGRID_COUNT_FLOPS`        | use Dune::Fem::Double as ctype |
         
         
-        git-4dd44056484d599767e7e33d685958cc5cb3a0e1
+        git-9627b15ad28ffa4447ba6b7fc83e5950bc6034f7
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-spgrid-2.9.0rc1/README.md` & `dune-spgrid-2.9.dev20220529/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 | `SPGRID_ANISOTROPIC`        | Anisotropic                    |
 | `SPGRID_ANISOTROPIC_SERIAL` | Anisotropic (no MPI)           |
 | `SPGRID_BISECTION`          | Bisection                      |
 | `SPGRID_BISECTION_SERIAL`   | Bisection (no MPI)             |
 | `SPGRID_COUNT_FLOPS`        | use Dune::Fem::Double as ctype |
 
 
-git-4dd44056484d599767e7e33d685958cc5cb3a0e1
+git-9627b15ad28ffa4447ba6b7fc83e5950bc6034f7
```

### Comparing `dune-spgrid-2.9.0rc1/cmake/modules/DuneSpgridMacros.cmake` & `dune-spgrid-2.9.dev20220529/cmake/modules/DuneSpgridMacros.cmake`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/doc/doxygen/main.page` & `dune-spgrid-2.9.dev20220529/doc/doxygen/main.page`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/common/iostream.hh` & `dune-spgrid-2.9.dev20220529/dune/common/iostream.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/extensions/superentityiterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/extensions/superentityiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/CMakeLists.txt` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/backuprestore.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/backuprestore.hh`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
    *  \tparam  Grid  type of grid
    */
   template< class ct, int dim, template< int > class Ref, class Comm >
   struct BackupRestoreFacility< SPGrid< ct, dim, Ref, Comm > >
   {
     typedef SPGrid< ct, dim, Ref, Comm > Grid;
 
-    typedef typename Grid::Communication Communication;
+    typedef typename Grid::CollectiveCommunication CollectiveCommunication;
 
     /** \brief write a hierarchic grid to disk
      *
      *  \param[in]  grid        grid to write
      *  \param[in]  path        path to write the file to
      *  \param[in]  fileprefix  prefix of the file name
      */
@@ -96,28 +96,28 @@
      *  \param[in]  path        path to write the file to
      *  \param[in]  fileprefix  prefix of the file name
      *  \param[in]  comm        collective communication (optional)
      *
      *  \returns a pointer to the grid (allocated by new)
      */
     static Grid *restore ( const std::string &path, const std::string &fileprefix,
-                           const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() )
+                           const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() )
     {
       return restore( path + "/" + fileprefix + ".spgrid" );
     }
 
     /** \brief read a hierarchic grid from disk
      *
      *  \param[in]  filename    name of the file to read
      *  \param[in]  comm        collective communication (optional)
      *
      *  \returns a pointer to the grid (allocated by new)
      */
     static Grid *restore ( const std::string &filename,
-                           const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() )
+                           const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() )
     {
       std::ifstream stream( filename.c_str() );
       if( !stream )
         DUNE_THROW( IOError, "Unable to open file: " + filename );
 
       Grid *grid = 0;
       SPGridIOData< ct, dim, Ref > ioData;
@@ -134,15 +134,15 @@
 
     /** \brief read a hierarchic grid from a stream
      *
      *  \param[in]  stream      std::stream to read the grid from
      *  \param[in]  comm        collective communication (optional)
      */
     static Grid *restore ( std::istream &stream,
-                           const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() )
+                           const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() )
     {
       Grid *grid = 0;
       SPGridIOData< ct, dim, Ref > ioData;
       if( ioData.read( stream ) )
         grid = restore( ioData, comm );
 
       if( !parallelAnd( comm, grid ) )
@@ -165,15 +165,15 @@
       ioData.maxLevel = grid.maxLevel();
       ioData.refinements.resize( ioData.maxLevel );
       for( int level = 0; level < ioData.maxLevel; ++level )
         ioData.refinements[ level ] = grid.gridLevel( level+1 ).refinement().policy();
     }
 
     static Grid *restore ( const SPGridIOData< ct, dim, Ref > &ioData,
-                           const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() )
+                           const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() )
     {
       if( ioData.partitions != comm.size() )
       {
         std::cerr << "Warning: Reading grid with different number of partitions,"
                   << " index sets will not coincide." << std::endl;
       }
 
@@ -186,15 +186,15 @@
           grid->globalRefine( 1, ioData.refinements[ level ] );
         else
           grid->globalRefine( 1 );
       }
       return grid;
     }
 
-    static bool parallelAnd ( const Communication &comm, bool condition )
+    static bool parallelAnd ( const CollectiveCommunication &comm, bool condition )
     {
       int result( condition );
       result = comm.sum( result );
       return (result == comm.size());
     }
   };
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/boundarysegmentiterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/boundarysegmentiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/cachedpartitionlist.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/cachedpartitionlist.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/capabilities.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/capabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/communication.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/communication.hh`

 * *Files 4% similar despite different names*

```diff
@@ -18,40 +18,40 @@
 
   // SPCommunicationTraits
   // ---------------------
 
   template< class Comm >
   struct SPCommunicationTraits
   {
-    typedef Dune::Communication< Comm > Communication;
+    typedef Dune::CollectiveCommunication< Comm > CollectiveCommunication;
 
     template< class C >
-    static Communication comm ( const C & )
+    static CollectiveCommunication comm ( const C & )
     {
       return defaultComm();
     }
 
-    static Communication defaultComm ()
+    static CollectiveCommunication defaultComm ()
     {
-      return Communication();
+      return CollectiveCommunication();
     }
   };
 
 #if HAVE_MPI
   template<>
   struct SPCommunicationTraits< MPI_Comm >
   {
-    typedef Dune::Communication< MPI_Comm > Communication;
+    typedef Dune::CollectiveCommunication< MPI_Comm > CollectiveCommunication;
 
-    static Communication comm ( const MPI_Comm &mpiComm )
+    static CollectiveCommunication comm ( const MPI_Comm &mpiComm )
     {
-      return Communication( mpiComm );
+      return CollectiveCommunication( mpiComm );
     }
 
-    static Communication defaultComm ()
+    static CollectiveCommunication defaultComm ()
     {
       return comm( MPI_COMM_WORLD );
     }
   };
 #endif // #if HAVE_MPI
 
 
@@ -81,16 +81,16 @@
     typedef SPPartitionList< dimension > PartitionList;
 
     typedef typename DataHandle::DataType DataType;
 
     typedef typename GridLevel::CommInterface Interface;
 
   private:
-    typedef SPPackedMessageWriteBuffer< typename Grid::Communication > WriteBuffer;
-    typedef SPPackedMessageReadBuffer< typename Grid::Communication > ReadBuffer;
+    typedef SPPackedMessageWriteBuffer< typename Grid::CollectiveCommunication > WriteBuffer;
+    typedef SPPackedMessageReadBuffer< typename Grid::CollectiveCommunication > ReadBuffer;
 
   public:
     SPCommunication ( const GridLevel &gridLevel, DataHandle &dataHandle,
                       InterfaceType iftype, CommunicationDirection dir );
 
     SPCommunication ( const SPCommunication & ) = delete;
     SPCommunication ( SPCommunication &&other );
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/cube.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/cube.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/decomposition.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/decomposition.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/dgfparser.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/dgfparser.hh`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
   template< class ct, int dim, template< int > class Ref, class Comm >
   class DGFGridFactory< SPGrid< ct, dim, Ref, Comm > >
   {
   public:
     typedef SPGrid< ct, dim, Ref, Comm > Grid;
 
     typedef MPIHelper::MPICommunicator MPICommunicatorType;
-    typedef typename Grid::Communication Communication;
+    typedef typename Grid::CollectiveCommunication CollectiveCommunication;
 
     static const int dimension = Grid::dimension;
     typedef typename Grid::template Codim< 0 >::Entity Element;
     typedef typename Grid::template Codim< dimension >::Entity Vertex;
 
   private:
     typedef FieldVector< double, dimension > Point;
@@ -155,15 +155,15 @@
     std::vector< double > &parameter ( const Entity &entity )
     {
       DUNE_THROW( InvalidStateException,
                   "Calling DGFGridFactory::parameter is only allowed if there are parameters." );
     }
 
   private:
-    void generate ( std::istream &input, const Communication &comm );
+    void generate ( std::istream &input, const CollectiveCommunication &comm );
 
     template< class Geometry >
     static void getCorners ( const Geometry &geometry, std::vector< Point > &corners )
     {
       corners.resize( geometry.corners() );
       for( int i = 0; i < geometry.corners(); ++i )
       {
@@ -201,15 +201,15 @@
     input.close();
   }
 
 
   template< class ct, int dim, template< int > class Ref, class Comm >
   inline void
   DGFGridFactory< SPGrid< ct, dim, Ref, Comm > >
-    ::generate ( std::istream &input, const Communication &comm )
+    ::generate ( std::istream &input, const CollectiveCommunication &comm )
   {
     dgf::IntervalBlock intervalBlock( input );
 
     if( !intervalBlock.isactive() )
       DUNE_THROW( DGFException, "DGF stream must contain an interval block to be used with SPGrid< ct, " << dim << " >." );
     if( intervalBlock.numIntervals() != 1 )
       DUNE_THROW( DGFException, "SPGrid< ct, " << dim << " > can only handle 1 interval block." );
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/direction.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/direction.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/domain.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/domain.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/entity.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/entity.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/entityinfo.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/entityinfo.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/entityseed.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/entityseed.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/fileio.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/fileio.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/geometricgridlevel.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/geometricgridlevel.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/geometry.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/geometry.hh`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #define DUNE_SPGRID_GEOMETRY_HH
 
 #include <type_traits>
 
 #include <dune/geometry/type.hh>
 
 #include <dune/common/typetraits.hh>
-#include <dune/common/transpose.hh>
 
 #include <dune/geometry/type.hh>
 #include <dune/geometry/referenceelements.hh>
 
 #include <dune/grid/spgrid/referencecube.hh>
 #include <dune/grid/spgrid/entityinfo.hh>
 
@@ -47,17 +46,14 @@
     // just to make the Dune interface happy
     typedef GlobalVector GlobalCoordinate;
     typedef LocalVector LocalCoordinate;
 
     typedef typename GeometryCache::JacobianTransposed JacobianTransposed;
     typedef typename GeometryCache::JacobianInverseTransposed JacobianInverseTransposed;
 
-    using Jacobian = std::decay_t<decltype(transposedView(std::declval<const JacobianTransposed&>()))>;
-    using JacobianInverse = std::decay_t<decltype(transposedView(std::declval<const JacobianInverseTransposed&>()))>;
-
   protected:
     SPBasicGeometry ()
     {}
 
   public:
     GeometryType type () const { return GeometryTypes::cube( mydimension ); }
 
@@ -72,17 +68,14 @@
 
     ctype volume () const { return asImpl().geometryCache().volume(); }
     ctype integrationElement ( const LocalVector &local ) const { return volume(); }
 
     const JacobianTransposed &jacobianTransposed ( const LocalVector &local ) const;
     const JacobianInverseTransposed &jacobianInverseTransposed ( const LocalVector &local ) const;
 
-    auto jacobian ( const LocalVector &local ) const;
-    auto jacobianInverse ( const LocalVector &local ) const;
-
   protected:
     const Impl &asImpl () const { return static_cast< const Impl & >( *this ); }
   };
 
 
 
   // SPGeometry
@@ -131,17 +124,14 @@
     : entityInfo_( gridLevel, id ),
       origin_( computeOrigin() )
     {}
 
     using Base::jacobianTransposed;
     using Base::jacobianInverseTransposed;
 
-    using Base::jacobian;
-    using Base::jacobianInverse;
-
     GlobalVector origin () const { return origin_; }
     const GeometryCache &geometryCache () const { return entityInfo().geometryCache(); }
 
     const GridLevel &gridLevel () const { return entityInfo().gridLevel(); }
 
     const EntityInfo &entityInfo () const { return entityInfo_; }
     EntityInfo &entityInfo () { return entityInfo_; }
@@ -194,17 +184,14 @@
     : geometryCache_( geometryCache ),
       origin_( origin )
     {}
 
     using Base::jacobianTransposed;
     using Base::jacobianInverseTransposed;
 
-    using Base::jacobian;
-    using Base::jacobianInverse;
-
     GlobalVector origin () const { return origin_; }
     const GeometryCache &geometryCache () const { return geometryCache_; }
 
   private:
     GeometryCache geometryCache_;
     GlobalVector origin_;
   };
@@ -246,27 +233,10 @@
   template< int mydim, int cdim, class Grid, class Impl >
   inline const typename SPBasicGeometry< mydim, cdim, Grid, Impl >::JacobianInverseTransposed &
   SPBasicGeometry< mydim, cdim, Grid, Impl >::jacobianInverseTransposed ( const LocalVector &local ) const
   {
     return asImpl().geometryCache().jacobianInverseTransposed();
   }
 
-  template< int mydim, int cdim, class Grid, class Impl >
-  inline auto SPBasicGeometry< mydim, cdim, Grid, Impl >::jacobian ( const LocalVector &local ) const
-  {
-    // Handing out a transposedView is OK, because jacobianTransposed
-    // returns a reference to a cached value.
-    return transposedView(jacobianTransposed(local));
-  }
-
-
-  template< int mydim, int cdim, class Grid, class Impl >
-  inline auto SPBasicGeometry< mydim, cdim, Grid, Impl >::jacobianInverse ( const LocalVector &local ) const
-  {
-    // Handing out a transposedView is OK, because jacobianInverseTransposed
-    // returns a reference to a cached value.
-    return transposedView(jacobianInverseTransposed(local));
-  }
-
 } // namespace Dune
 
 #endif // #ifndef DUNE_SPGRID_GEOMETRY_HH
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/geometrycache.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/geometrycache.hh`

 * *Files 1% similar despite different names*

```diff
@@ -34,39 +34,39 @@
 
   template< int dim >
   struct SPGeometryPattern< dim, 0 >
   {
     typedef SPDirection< dim > Direction;
 
     SPGeometryPattern () = default;
-    explicit SPGeometryPattern ( Direction /*dir*/ ) {}
+    explicit SPGeometryPattern ( Direction dir ) {}
 
     int nonzero ( const int k ) const;
     int zero ( const int k ) const;
   };
 
   template< int dim >
   struct SPGeometryPattern< dim, dim >
   {
     typedef SPDirection< dim > Direction;
 
     SPGeometryPattern () = default;
-    explicit SPGeometryPattern ( Direction /*dir*/ ) {}
+    explicit SPGeometryPattern ( Direction dir ) {}
 
     int nonzero ( const int k ) const;
     int zero ( const int k ) const;
   };
 
   template<>
   struct SPGeometryPattern< 0, 0 >
   {
     typedef SPDirection< 0 > Direction;
 
     SPGeometryPattern () = default;
-    explicit SPGeometryPattern ( Direction /*dir*/ ) {}
+    explicit SPGeometryPattern ( Direction dir ) {}
 
     int nonzero ( const int k ) const;
     int zero ( const int k ) const;
   };
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/grid.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/grid.hh`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,15 @@
       typedef SPReferenceCubeContainer< ct, dim > ReferenceCubeContainer;
       typedef typename ReferenceCubeContainer::ReferenceCube ReferenceCube;
       typedef SPDomain< ct, dim > Domain;
       typedef SPMesh< dim > Mesh;
       typedef Ref< dim > Refinement;
       typedef typename Refinement::Policy RefinementPolicy;
 
-      typedef typename SPCommunicationTraits< Comm >::Communication Communication;
-      typedef Communication CollectiveCommunication;
+      typedef typename SPCommunicationTraits< Comm >::CollectiveCommunication CollectiveCommunication;
 
       typedef Dune::Intersection< const Grid, SPIntersection< const Grid > > LevelIntersection;
       typedef LevelIntersection LeafIntersection;
 
       typedef Dune::IntersectionIterator< const Grid, SPIntersectionIterator< const Grid >, SPIntersection< const Grid > > LevelIntersectionIterator;
       typedef LevelIntersectionIterator LeafIntersectionIterator;
 
@@ -162,16 +161,15 @@
     static const int dimensionworld = ReferenceCube::dimension;
 
     typedef typename ReferenceCube::GlobalVector GlobalVector;
 
     typedef typename Traits::GlobalIdSet GlobalIdSet;
     typedef typename Traits::LocalIdSet LocalIdSet;
 
-    typedef typename Traits::Communication Communication;
-    typedef Communication CollectiveCommunication;
+    typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
     template< int codim >
     struct Codim
     : Base::template Codim< codim >
     {
       typedef typename Traits::template Codim< codim >::ReferenceCube ReferenceCube;
 
@@ -195,25 +193,25 @@
     typedef typename GridLevel::PartitionList PartitionList;
 
     typedef typename LevelGridView::Traits::GridViewImp LevelGridViewImpl;
     typedef typename LeafGridView::Traits::GridViewImp LeafGridViewImpl;
 
   public:
     SPGrid ( const Domain &domain, const MultiIndex &cells,
-             const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() );
+             const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() );
 
     SPGrid ( const Domain &domain, const MultiIndex &cells, const MultiIndex &overlap,
-             const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() );
+             const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() );
 
     SPGrid ( const GlobalVector &a, const GlobalVector &b, const MultiIndex &cells,
-             const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() );
+             const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() );
 
     SPGrid ( const GlobalVector &a, const GlobalVector &b, const MultiIndex &cells,
              const MultiIndex &overlap,
-             const Communication &comm = SPCommunicationTraits< Comm >::defaultComm() );
+             const CollectiveCommunication &comm = SPCommunicationTraits< Comm >::defaultComm() );
 
     SPGrid ( const This & ) = delete;
     SPGrid ( This &&other );
 
     const ReferenceCube &referenceCube () const
     {
       return refCubes_.get();
@@ -406,15 +404,15 @@
     communicate ( CommDataHandleIF< DataHandle, Data > &data,
                   InterfaceType interface, CommunicationDirection dir ) const
     {
       LeafGridView view = leafGridView();
       return view.impl().communicate( data, interface, dir );
     }
 
-    const Communication &comm () const;
+    const CollectiveCommunication &comm () const;
 
     template< class Seed >
     typename Traits::template Codim< Seed::codimension >::Entity entity ( const Seed &seed ) const
     {
       typedef typename Traits::template Codim< Seed::codimension >::Entity Entity;
       typedef SPEntity< Seed::codimension, dimension, const This > EntityImpl;
       typename EntityImpl::EntityInfo entityInfo( gridLevel( seed.impl().level() ), seed.impl().id(), seed.impl().partitionNumber() );
@@ -471,41 +469,41 @@
       return typename Codim< 1 >::LocalGeometry( *localFaceGeometry_[ face ] );
     }
 
     void createLocalGeometries ();
     void setupMacroGrid ();
     void setupBoundaryIndices ();
 
-    static Communication defaultCommunication ();
+    static CollectiveCommunication defaultCommunication ();
 
     Domain domain_;
     Mesh globalMesh_;
     MultiIndex overlap_;
     ReferenceCubeContainer refCubes_;
     std::vector< std::unique_ptr< GridLevel > > gridLevels_;
     std::vector< LevelGridView > levelGridViews_;
     LeafGridView leafGridView_;
     HierarchicIndexSet hierarchicIndexSet_;
     GlobalIdSet globalIdSet_;
     LocalIdSet localIdSet_;
-    Communication comm_;
+    CollectiveCommunication comm_;
     std::size_t boundarySize_;
     std::vector< std::array< std::size_t, 2*dimension > > boundaryOffset_;
     std::array< std::unique_ptr< const typename Codim< 1 >::LocalGeometryImpl >, ReferenceCube::numFaces > localFaceGeometry_;
   };
 
 
 
   // Implementation of SPGrid
   // ------------------------
 
   template< class ct, int dim, template< int > class Ref, class Comm >
   inline SPGrid< ct, dim, Ref, Comm >
     ::SPGrid ( const Domain &domain, const MultiIndex &cells,
-               const Communication &comm )
+               const CollectiveCommunication &comm )
   : domain_( domain ),
     globalMesh_( cells ),
     overlap_( MultiIndex::zero() ),
     leafGridView_( LeafGridViewImpl() ),
     hierarchicIndexSet_( *this ),
     comm_( comm )
   {
@@ -513,15 +511,15 @@
     setupMacroGrid();
   }
 
 
   template< class ct, int dim, template< int > class Ref, class Comm >
   inline SPGrid< ct, dim, Ref, Comm >
     ::SPGrid ( const Domain &domain, const MultiIndex &cells, const MultiIndex &overlap,
-               const Communication &comm )
+               const CollectiveCommunication &comm )
   : domain_( domain ),
     globalMesh_( cells ),
     overlap_( overlap ),
     leafGridView_( LeafGridViewImpl() ),
     hierarchicIndexSet_( *this ),
     comm_( comm )
   {
@@ -529,15 +527,15 @@
     setupMacroGrid();
   }
 
 
   template< class ct, int dim, template< int > class Ref, class Comm >
   inline SPGrid< ct, dim, Ref, Comm >
     ::SPGrid ( const GlobalVector &a, const GlobalVector &b, const MultiIndex &cells,
-               const Communication &comm )
+               const CollectiveCommunication &comm )
   : domain_( a, b ),
     globalMesh_( cells ),
     overlap_( MultiIndex::zero() ),
     leafGridView_( LeafGridViewImpl() ),
     hierarchicIndexSet_( *this ),
     comm_( comm )
   {
@@ -545,15 +543,15 @@
     setupMacroGrid();
   }
 
 
   template< class ct, int dim, template< int > class Ref, class Comm >
   inline SPGrid< ct, dim, Ref, Comm >
     ::SPGrid ( const GlobalVector &a, const GlobalVector &b, const MultiIndex &cells,
-               const MultiIndex &overlap, const Communication &comm )
+               const MultiIndex &overlap, const CollectiveCommunication &comm )
   : domain_( a, b ),
     globalMesh_( cells ),
     overlap_( overlap ),
     leafGridView_( LeafGridViewImpl() ),
     hierarchicIndexSet_( *this ),
     comm_( comm )
   {
@@ -658,15 +656,15 @@
         handle.postRefinement( *it );
       handle.postAdapt();
     }
   }
 
 
   template< class ct, int dim, template< int > class Ref, class Comm >
-  inline const typename SPGrid< ct, dim, Ref, Comm >::Communication &
+  inline const typename SPGrid< ct, dim, Ref, Comm >::CollectiveCommunication &
   SPGrid< ct, dim, Ref, Comm >::comm () const
   {
     return comm_;
   }
 
 
   template< class ct, int dim, template< int > class Ref, class Comm >
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/gridlevel.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/gridlevel.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/gridview.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/gridview.hh`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     typedef SPIndexSet< const Grid > IndexSet;
     typedef Dune::Intersection< const Grid, SPIntersection< const Grid > > Intersection;
     typedef Dune::IntersectionIterator< const Grid, SPIntersectionIterator< const Grid >, SPIntersection< const Grid > > IntersectionIterator;
 
     static const bool hasBoundarySegmentIterator = true;
     typedef Dune::IntersectionIterator< const Grid, SPBoundarySegmentIterator< const Grid >, SPIntersection< const Grid > > BoundarySegmentIterator;
 
-    typedef typename Grid::Communication Communication;
-    typedef Communication CollectiveCommunication;
+    typedef typename Grid::CollectiveCommunication CollectiveCommunication;
 
     static const bool conforming = true;
 
     template< int codim >
     struct Codim
     {
       typedef typename Grid::Traits::template Codim< codim >::Entity Entity;
@@ -87,16 +86,15 @@
     template< class > friend class SPGridView;
 
   public:
     typedef typename ViewTraits::Grid Grid;
     typedef typename ViewTraits::IndexSet IndexSet;
     typedef typename ViewTraits::IntersectionIterator IntersectionIterator;
     typedef typename ViewTraits::BoundarySegmentIterator BoundarySegmentIterator;
-    typedef typename ViewTraits::Communication Communication;
-    typedef Communication CollectiveCommunication;
+    typedef typename ViewTraits::CollectiveCommunication CollectiveCommunication;
 
     typedef SPGridLevel< Grid > GridLevel;
 
     template< int codim >
     struct Codim
       : public ViewTraits::template Codim< codim >
     {};
@@ -149,15 +147,15 @@
     template< class Entity >
     typename Codim< Entity::codimension >::SuperEntityIterator
     superEntityEnd ( const Entity &entity ) const;
 
     BoundarySegmentIterator boundarySegmentBegin ( int face = 0 ) const;
     BoundarySegmentIterator boundarySegmentEnd ( int face = GridLevel::numFaces-1 ) const;
 
-    const Communication &comm () const { return grid().comm(); }
+    const CollectiveCommunication &comm () const { return grid().comm(); }
 
     template< class DataHandle, class Data >
     SPCommunication< Grid, CommDataHandleIF< DataHandle, Data > >
     communicate ( CommDataHandleIF< DataHandle, Data > &data, InterfaceType iftype, CommunicationDirection dir ) const
     {
       return SPCommunication< Grid, CommDataHandleIF< DataHandle, Data > >( gridLevel(), data, iftype, dir );
     }
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/hierarchiciterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/hierarchiciterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/hierarchicsearch.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/hierarchicsearch.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/hindexset.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/hindexset.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/idset.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/idset.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/indexset.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/indexset.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/intersection.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/intersection.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/intersectioniterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/intersectioniterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/iterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/iterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/linkage.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/linkage.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/mesh.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/mesh.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/messagebuffer.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/messagebuffer.hh`

 * *Files 10% similar despite different names*

```diff
@@ -83,41 +83,41 @@
   };
 
 
 
   // SPPackedMessageWriteBuffer
   // --------------------------
 
-  template< class Communication >
+  template< class CollectiveCommunication >
   class SPPackedMessageWriteBuffer;
 
   template< class C >
-  class SPPackedMessageWriteBuffer< Communication< C > >
+  class SPPackedMessageWriteBuffer< CollectiveCommunication< C > >
     : public SPBasicPackedMessageWriteBuffer
   {
-    typedef SPPackedMessageWriteBuffer< Communication< C > > This;
+    typedef SPPackedMessageWriteBuffer< CollectiveCommunication< C > > This;
     typedef SPBasicPackedMessageWriteBuffer Base;
 
   public:
-    explicit SPPackedMessageWriteBuffer ( const Communication< C > &comm ) {}
+    explicit SPPackedMessageWriteBuffer ( const CollectiveCommunication< C > &comm ) {}
 
     void send ( int rank, int tag ) {}
     void wait () {}
   };
 
 #if HAVE_MPI
   template<>
-  class SPPackedMessageWriteBuffer< Communication< MPI_Comm > >
+  class SPPackedMessageWriteBuffer< CollectiveCommunication< MPI_Comm > >
     : public SPBasicPackedMessageWriteBuffer
   {
-    typedef SPPackedMessageWriteBuffer< Communication< MPI_Comm > > This;
+    typedef SPPackedMessageWriteBuffer< CollectiveCommunication< MPI_Comm > > This;
     typedef SPBasicPackedMessageWriteBuffer Base;
 
   public:
-    explicit SPPackedMessageWriteBuffer ( const Communication< MPI_Comm > &comm ) : comm_( comm ) {}
+    explicit SPPackedMessageWriteBuffer ( const CollectiveCommunication< MPI_Comm > &comm ) : comm_( comm ) {}
 
     void send ( int rank, int tag )
     {
       MPI_Isend( buffer_, position_, MPI_PACKED, rank, tag, comm_, &request_ );
     }
 
     void wait () { MPI_Wait( &request_, MPI_STATUS_IGNORE ); }
@@ -196,26 +196,26 @@
   };
 
 
 
   // SPPackedMessageReadBuffer
   // -------------------------
 
-  template< class Communication >
+  template< class CollectiveCommunication >
   class SPPackedMessageReadBuffer;
 
   template< class C >
-  class SPPackedMessageReadBuffer< Communication< C > >
+  class SPPackedMessageReadBuffer< CollectiveCommunication< C > >
     : public SPBasicPackedMessageReadBuffer
   {
-    typedef SPPackedMessageReadBuffer< Communication< C > > This;
+    typedef SPPackedMessageReadBuffer< CollectiveCommunication< C > > This;
     typedef SPBasicPackedMessageReadBuffer Base;
 
   public:
-    explicit SPPackedMessageReadBuffer ( const Communication< C > &comm ) {}
+    explicit SPPackedMessageReadBuffer ( const CollectiveCommunication< C > &comm ) {}
 
     void receive ( int rank, int rag, std::size_t size )
     {
       DUNE_THROW( IOError, "Nothing to receive in a serial communication." );
     }
 
     void receive ( int rank, int tag ) { receive( rank, tag, 0 ); }
@@ -229,22 +229,22 @@
     {
       return readBuffers.end();
     }
   };
 
 #if HAVE_MPI
   template<>
-  class SPPackedMessageReadBuffer< Communication< MPI_Comm > >
+  class SPPackedMessageReadBuffer< CollectiveCommunication< MPI_Comm > >
     : public SPBasicPackedMessageReadBuffer
   {
-    typedef SPPackedMessageReadBuffer< Communication< MPI_Comm > > This;
+    typedef SPPackedMessageReadBuffer< CollectiveCommunication< MPI_Comm > > This;
     typedef SPBasicPackedMessageReadBuffer Base;
 
   public:
-    SPPackedMessageReadBuffer ( const Communication< MPI_Comm > &comm ) : comm_( comm ) {}
+    SPPackedMessageReadBuffer ( const CollectiveCommunication< MPI_Comm > &comm ) : comm_( comm ) {}
 
     void receive ( int rank, int tag, std::size_t size )
     {
       rank_ = rank;
       reset( size );
       MPI_Irecv( buffer_, size_, MPI_BYTE, rank, tag, comm_, &request_ );
     }
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/misc.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/misc.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/multiindex.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/multiindex.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/normal.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/normal.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/partition.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/partition.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/partitionlist.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/partitionlist.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/partitionpool.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/partitionpool.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/persistentcontainer.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/persistentcontainer.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/referencecube.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/referencecube.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/refinement.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/refinement.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/superentityiterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/superentityiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/topology.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/topology.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid/tree.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid/tree.hh`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     private:
       const GridLevel &leafLevel () const { return gridLevel().grid().leafLevel(); }
 
       bool isDone () const { return (&gridLevel() == rootLevel_); }
 
       EntityInfo entityInfo_;
-      const GridLevel *rootLevel_ = nullptr;
+      const GridLevel *rootLevel_;
       IsLeaf isLeaf_;
     };
 
 
 
     // TreeIterator for Intersection
     // -----------------------------
```

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/spgrid.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/spgrid.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/CMakeLists.txt` & `dune-spgrid-2.9.dev20220529/dune/grid/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/bndsegcheck.cc` & `dune-spgrid-2.9.dev20220529/dune/grid/test/bndsegcheck.cc`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/checkbndsegiterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/test/checkbndsegiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/checkidcommunication.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/test/checkidcommunication.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/checkseiterator.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/test/checkseiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/checktree.hh` & `dune-spgrid-2.9.dev20220529/dune/grid/test/checktree.hh`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/decomposition.cc` & `dune-spgrid-2.9.dev20220529/dune/grid/test/decomposition.cc`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/test-jacobians.cc` & `dune-spgrid-2.9.dev20220529/dune/grid/test/test-jacobians.cc`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/dune/grid/test/test-spgrid.cc` & `dune-spgrid-2.9.dev20220529/dune/grid/test/test-spgrid.cc`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/pyproject.toml` & `dune-spgrid-2.9.dev20220529/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # This is uses the `Python-Requires` field in the `dune.modules` file to
 # populate the `requires` entry. Additional packages needed for the package
 # build should be added in the `dune.modules`. These packages will then also be
 # included in the package install from source.
 #
 [build-system]
-requires = ['cmake>=3.13', 'dune-grid<=v2.9.0rc1', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
+requires = ['cmake>=3.13', 'dune-grid<=2.9.dev20220529', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
```

### Comparing `dune-spgrid-2.9.0rc1/python/dune/spgrid/__init__.py` & `dune-spgrid-2.9.dev20220529/python/dune/spgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/PKG-INFO` & `dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-spgrid
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: module providing a structured grid
 Home-page: https://gitlab.dune-project.org/extensions/dune-spgrid
 Author: Martin Nolte
 Author-email: nolte.mrtn@gmail.com
 License: UNKNOWN
 Description: Dune-SPGrid
         ===========
@@ -64,15 +64,15 @@
         | `SPGRID_ANISOTROPIC`        | Anisotropic                    |
         | `SPGRID_ANISOTROPIC_SERIAL` | Anisotropic (no MPI)           |
         | `SPGRID_BISECTION`          | Bisection                      |
         | `SPGRID_BISECTION_SERIAL`   | Bisection (no MPI)             |
         | `SPGRID_COUNT_FLOPS`        | use Dune::Fem::Double as ctype |
         
         
-        git-4dd44056484d599767e7e33d685958cc5cb3a0e1
+        git-9627b15ad28ffa4447ba6b7fc83e5950bc6034f7
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-spgrid-2.9.0rc1/python/dune_spgrid.egg-info/SOURCES.txt` & `dune-spgrid-2.9.dev20220529/python/dune_spgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

