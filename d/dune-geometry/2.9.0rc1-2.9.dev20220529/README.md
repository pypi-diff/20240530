# Comparing `tmp/dune-geometry-2.9.0rc1.tar.gz` & `tmp/dune-geometry-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-geometry-2.9.0rc1.tar", last modified: Fri Oct 21 08:16:43 2022, max compression
+gzip compressed data, was "dune-geometry-2.9.dev20220529.tar", last modified: Sun May 29 21:03:22 2022, max compression
```

## Comparing `dune-geometry-2.9.0rc1.tar` & `dune-geometry-2.9.dev20220529.tar`

### file list

```diff
@@ -1,178 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.140045 dune-geometry-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8343 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19939 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)    19939 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.124045 dune-geometry-2.9.0rc1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    19036 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-10-21 08:16:43.140045 dune-geometry-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.124045 dune-geometry-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.124045 dune-geometry-2.9.0rc1/doc/appl/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.128045 dune-geometry-2.9.0rc1/doc/appl/refelements/
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/SVG.readme
--rw-r--r--   0 runner    (1001) docker     (121)    32279 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    18672 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    24644 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron_edges.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron_edges.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    22601 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron_edges.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron_edges.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_line.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_line.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_line.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_line.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    33552 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    16136 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    22684 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism_edges.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism_edges.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    17156 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism_edges.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism_edges.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    46806 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    14481 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    29035 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid_edges.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid_edges.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    14901 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid_edges.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid_edges.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_quadrilateral.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_quadrilateral.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     8363 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_quadrilateral.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_quadrilateral.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    29836 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    12036 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    22586 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron_edges.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron_edges.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    12263 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron_edges.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron_edges.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)     6480 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_triangle.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_triangle.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_triangle.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/gg_triangle.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    12281 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/appl/refelements/referenceelementspage.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.132045 dune-geometry-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/doxygen/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/doxygen/modules.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.132045 dune-geometry-2.9.0rc1/doc/refinement/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/kuhntriangulation.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/kuhntriangulation.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    30988 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/referencetokuhn0.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/referencetokuhn0.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    27309 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/refinement.tex
--rw-r--r--   0 runner    (1001) docker     (121)    17926 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/simplexvertexindex.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/doc/refinement/simplexvertexindex.svg.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.132045 dune-geometry-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.132045 dune-geometry-2.9.0rc1/dune/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    22182 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/affinegeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12753 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/axisalignedcubegeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5509 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/deprecated_topology.hh
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/dimension.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7056 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/generalvertexorder.hh
--rw-r--r--   0 runner    (1001) docker     (121)    35204 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/multilineargeometry.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/compositequadraturerule.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussjacobi.mac
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gausslobatto.mac
--rw-r--r--   0 runner    (1001) docker     (121)    79582 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gausslobattoquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)   260229 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussradau.mac
--rw-r--r--   0 runner    (1001) docker     (121)    75178 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussradauleftquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)    73591 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussradaurightquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)   263989 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/jacobi1quadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)   263991 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/jacobi2quadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/jacobiNquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/pointquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/prismquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/quadraturerules.cc
--rw-r--r--   0 runner    (1001) docker     (121)    41680 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/simplexquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7297 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/tensorproductquadrature.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8388 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/writequad.mac
--rw-r--r--   0 runner    (1001) docker     (121)    17553 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/quadraturerules.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11178 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/referenceelement.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6740 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/referenceelementimplementation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    28586 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/referenceelementimplementation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16332 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/referenceelements.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/geometry/refinement/
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7642 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/base.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14413 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/hcube.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13723 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/hcubetriangulation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13835 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/prismtriangulation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13712 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/pyramidtriangulation.cc
--rw-r--r--   0 runner    (1001) docker     (121)    27558 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement/simplex.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10238 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/refinement.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/geometry/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3435 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11160 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/checkgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8051 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-affinegeometry.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-axisalignedcubegeometry.cc
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-constexpr-geometrytype.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-cornerstoragerefwrap.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-fromvertexcount.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-geometrytype-id.cc
--rw-r--r--   0 runner    (1001) docker     (121)    17479 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-multilineargeometry.cc
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-nonetype.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9647 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-quadrature.cc
--rw-r--r--   0 runner    (1001) docker     (121)    19329 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-referenceelements.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10124 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/test/test-refinement.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5316 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/topologyfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20007 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/type.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/typeindex.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/geometry/utility/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/utility/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/utility/typefromvertexcount.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22964 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/virtualrefinement.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14761 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/geometry/virtualrefinement.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/python/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/python/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/geometry/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/geometry/multilineargeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5325 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/geometry/quadraturerules.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10416 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/geometry/referenceelements.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9270 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/geometry/type.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/dune/python/test/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/test/geometrytype.py
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/test/refelement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune/python/test/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune-geometry.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/dune.module
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/python/dune/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/dune/geometry/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/dune/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/dune/geometry/_geometry.cc
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/dune/geometry/_referenceelements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/python/dune/geometry/quadpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:43.136045 dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-10-21 08:16:43.000000 dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5951 2022-10-21 08:16:43.000000 dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:16:43.000000 dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-21 08:16:43.000000 dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:16:43.000000 dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:16:43.140045 dune-geometry-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:16:42.000000 dune-geometry-2.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     7809 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19939 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)    19939 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.811612 dune-geometry-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.811612 dune-geometry-2.9.dev20220529/doc/appl/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.815612 dune-geometry-2.9.dev20220529/doc/appl/refelements/
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/SVG.readme
+-rw-r--r--   0 runner    (1001) docker     (121)    32279 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18672 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    24644 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron_edges.png
+-rw-r--r--   0 runner    (1001) docker     (121)    22601 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron_edges.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_line.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_line.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    33552 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism.png
+-rw-r--r--   0 runner    (1001) docker     (121)    16136 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    22684 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism_edges.png
+-rw-r--r--   0 runner    (1001) docker     (121)    17156 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism_edges.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    46806 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14481 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    29035 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid_edges.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14901 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid_edges.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_quadrilateral.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8363 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_quadrilateral.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    29836 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12036 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    22586 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron_edges.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12263 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron_edges.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     6480 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_triangle.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    12106 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/appl/refelements/referenceelementspage.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.815612 dune-geometry-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/doxygen/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/doxygen/modules.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.815612 dune-geometry-2.9.dev20220529/doc/refinement/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/refinement/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/refinement/kuhntriangulation.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    30988 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/refinement/referencetokuhn0.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    27134 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/refinement/refinement.tex
+-rw-r--r--   0 runner    (1001) docker     (121)    17926 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/doc/refinement/simplexvertexindex.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.815612 dune-geometry-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.815612 dune-geometry-2.9.dev20220529/dune/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21039 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/affinegeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11287 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/axisalignedcubegeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5334 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/deprecated_topology.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/dimension.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6881 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/generalvertexorder.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    33285 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/multilineargeometry.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.819612 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/compositequadraturerule.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussjacobi.mac
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gausslobatto.mac
+-rw-r--r--   0 runner    (1001) docker     (121)    79407 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gausslobattoquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)   260054 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussradau.mac
+-rw-r--r--   0 runner    (1001) docker     (121)    75003 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussradauleftquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    73416 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussradaurightquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)   263814 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/jacobi1quadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)   263816 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/jacobi2quadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/jacobiNquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/pointquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/prismquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/quadraturerules.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    41505 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/simplexquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7122 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/tensorproductquadrature.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8031 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/writequad.mac
+-rw-r--r--   0 runner    (1001) docker     (121)    18038 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11003 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/referenceelement.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/referenceelementimplementation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    28411 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/referenceelementimplementation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16155 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/referenceelements.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.819612 dune-geometry-2.9.dev20220529/dune/geometry/refinement/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7467 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/base.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14238 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/hcube.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13548 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/hcubetriangulation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13660 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/prismtriangulation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13537 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/pyramidtriangulation.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    27382 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement/simplex.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/refinement.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.819612 dune-geometry-2.9.dev20220529/dune/geometry/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9083 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/checkgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7876 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-affinegeometry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-axisalignedcubegeometry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-constexpr-geometrytype.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-cornerstoragerefwrap.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-fromvertexcount.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-geometrytype-id.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    17304 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-multilineargeometry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-nonetype.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9472 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-quadrature.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    19154 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-referenceelements.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/test/test-refinement.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/topologyfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19832 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/type.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5483 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/typeindex.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.819612 dune-geometry-2.9.dev20220529/dune/geometry/utility/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/utility/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/utility/typefromvertexcount.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22789 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/virtualrefinement.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14587 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/geometry/virtualrefinement.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.819612 dune-geometry-2.9.dev20220529/dune/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.819612 dune-geometry-2.9.dev20220529/dune/python/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/geometry/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/geometry/multilineargeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5150 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/geometry/quadraturerules.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10241 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/geometry/referenceelements.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9095 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/geometry/type.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/dune/python/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/test/geometrytype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/test/refelement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune/python/test/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune-geometry.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/dune.module
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/python/dune/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune/geometry/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune/geometry/_geometry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune/geometry/_referenceelements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4346 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune/geometry/quadpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:22.823613 dune-geometry-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:22.000000 dune-geometry-2.9.dev20220529/setup.py
```

### Comparing `dune-geometry-2.9.0rc1/CHANGELOG.md` & `dune-geometry-2.9.dev20220529/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-<!--
-SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 # Master (will become release 2.9)
 
-- The `Geometry` interface was extended by methods `jacobian(local)` and `jacobianInverse(local)`
-  and corresponding typedefs `Jacobian` and `JacobianInverse`. This is implemented by all geometry
-  implementations provided by dune-geometry. But external implementations need to be adjusted
-  to pass the interface check provided by `checkgeometry.hh`.
-
 - The `Geometry::integrationElement` now needs to return the type `Volume`
   instead of `ctype`. Note that this may be different from `ctype` if the
   geometry supports typed dimensions. In such case, `ctype` is a length, and not
   appropriate for a volume quantity.
 
 # Release 2.8
 
@@ -73,15 +63,15 @@
   the methods `size()` and `contains()`.
 - The methods `GeometryType(int)` and `GeometryType(unsigned int)` have been deprecated
   and will be removed after the release of dune-geometry 2.7.  Instead, please now use
   `GeometryTypes::cube(dim)` to construct one- or two-dimensional `GeometryType` objects.
 - Geometry implementations now export a type `Volume` that is used for the return
   value of the `volume` methods.  So does the generic `ReferenceElement` implementation.
 -   More efficient quadrature rules for simplices are available that
-    need less quadrature points to achieve the same order.  For now these
+    need less quadrature points to achive the same order.  For now these
     have to be explicitly requested:
     ```c++
     auto&& rule = Dune::QuadratureRules<...>::rule(..., Dune::QuadratureType::GaussJacobi_n_0);
     ```
     See [!127].
 
     [!127]: https://gitlab.dune-project.org/core/dune-geometry/merge_requests/127
```

### Comparing `dune-geometry-2.9.0rc1/CMakeLists.txt` & `dune-geometry-2.9.dev20220529/CMakeLists.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 cmake_minimum_required(VERSION 3.13)
 project("dune-geometry" C CXX)
 
 if(NOT (dune-common_DIR OR dune-common_ROOT OR
         "${CMAKE_PREFIX_PATH}" MATCHES ".*dune-common.*"))
     string(REPLACE  ${PROJECT_NAME} dune-common dune-common_DIR
       ${PROJECT_BINARY_DIR})
```

### Comparing `dune-geometry-2.9.0rc1/COPYING` & `dune-geometry-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/INSTALL` & `dune-geometry-2.9.dev20220529/INSTALL`

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

### Comparing `dune-geometry-2.9.0rc1/LICENSE.md` & `dune-geometry-2.9.dev20220529/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/PKG-INFO` & `dune-geometry-2.9.dev20220529/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-geometry
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Geometry Transformations, Reference Elements and Quadrature Rules
 Home-page: https://gitlab.dune-project.org/core/dune-geometry
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
         
         
-        git-273db91ded0a5807cb45ab6d21e7cbdd6970dc11
+        git-96a9468acdc641888f54374fc7b16682667867fd
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-geometry-2.9.0rc1/README.md` & `dune-geometry-2.9.dev20220529/README.md`

 * *Files 13% similar despite different names*

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
 
 
-git-273db91ded0a5807cb45ab6d21e7cbdd6970dc11
+git-96a9468acdc641888f54374fc7b16682667867fd
```

### Comparing `dune-geometry-2.9.0rc1/config.h.cmake` & `dune-geometry-2.9.dev20220529/config.h.cmake`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /* begin dune-geometry
    put the definitions for config.h specific to
    your project here. Everything above will be
    overwritten
 */
 /* begin private */
 /* Name of package */
```

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron_edges.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron_edges.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_hexahedron_edges.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_hexahedron_edges.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_line.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_line.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_line.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_line.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism_edges.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism_edges.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_prism_edges.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_prism_edges.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid_edges.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid_edges.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_pyramid_edges.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_pyramid_edges.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_quadrilateral.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_quadrilateral.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_quadrilateral.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_quadrilateral.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron_edges.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron_edges.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_tetrahedron_edges.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_tetrahedron_edges.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_triangle.png` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_triangle.png`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/gg_triangle.svg` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/gg_triangle.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/appl/refelements/referenceelementspage.txt` & `dune-geometry-2.9.dev20220529/doc/appl/refelements/referenceelementspage.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /**
 \page GeometryGenericGeometry Generic Geometries
 @ingroup GeometryReferenceElements
 
 \section GeometryGeometryIntroduction Introduction
 
 In the following we will give a definition of reference
@@ -191,15 +189,15 @@
 \f$T_1 = \mathbf{p}^{\vert\vert\vert\circ\circ}\f$ and
 \f$T_2 = \mathbf{p}^{\circ\circ\circ\circ\vert}\f$.
 For these topologies we have \f$s_d( T_1 ) = s_d( T_2 ) = 10\f$.
 
 
 \section GeometryGeometryElement Reference Domains
 
-For each reference topology \f$T\f$ we associate the set of corners
+For each reference topology \f$T\f$ we assosiate the set of corners
 \f$\mathcal{C}(T):=(p_i(T))_{1=1}^{s_d(T)}\subset\mathbf{R}^d(T)\f$ 
 defined through 
 - \f$T=\mathbf{p}\f$: \f$p_0(T)=0\in\mathbf{R}^0\f$
 - \f$T=t^\vert\f$: \f$p_k(T)=(p_k(t),0),p_{d'+k}(T)=(p_k(t),1)\f$
   for \f$k=1,\dots,d'\f$, with \f$d'=s_d(t)\f$.
 - \f$T=t^\circ\f$: \f$p_k(T)=(p_k(t),0)\f$ 
   for \f$k=1,\dots,d-1\f$ and \f$p_d(T)=e_d\f$ with
```

### Comparing `dune-geometry-2.9.0rc1/doc/doxygen/Doxylocal` & `dune-geometry-2.9.dev20220529/doc/doxygen/Doxylocal`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # This file contains local changes to the doxygen configuration
 # please us '+=' to add file/directories to the lists
 
 # The INPUT tag can be used to specify the files and/or directories that contain
 # documented source files. You may enter file names like "myfile.cpp" or
 # directories like "/usr/src/myproject". Separate the files or directories
 # with spaces.
```

### Comparing `dune-geometry-2.9.0rc1/doc/refinement/kuhntriangulation.svg` & `dune-geometry-2.9.dev20220529/doc/refinement/kuhntriangulation.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/refinement/referencetokuhn0.svg` & `dune-geometry-2.9.dev20220529/doc/refinement/referencetokuhn0.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/doc/refinement/refinement.tex` & `dune-geometry-2.9.dev20220529/doc/refinement/refinement.tex`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-% SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 \documentclass[english,a4paper]{article}
 \usepackage[latin1]{inputenc}
 \usepackage{babel}
 \usepackage{listings}
 \usepackage{float}
 \usepackage{type1cm}
 \usepackage{paralist}
@@ -96,15 +93,15 @@
 \item[Element:] An element is an {\em entity} of the same dimension as
   the grid it belongs to.
 \item[Vertex:] A vertex is an {\em entity} of dimension 0 (a point).
 \item[Codimension:] Let $d_G$ be the dimension of a grid and $d_e$ the
   dimension of one of its {\em entities}.  The codimension $c_e$ of that
   entity is defined as $c_e:=d_G-d_e$.  That means that the
   codimension of a {\em vertex} equals the dimension of its grid,
-  while the codimension of an {\em element} is always 0.
+  while the codimension of an {\em element} is alway 0.
 \item[Subentity:] When we refine an {\em entity}, we can view it as a
   grid consisting of smaller entities of the same or lower dimension.
   To distinguish these smaller entities from those who belong to a
   full-fledged grid, we call then subentities.  Subentities also have
   a codimension: let $d_e$ be the dimension of the refined entity and
   $d_s$ be the dimension of one of its subentities, than $c_s:=d_e-d_s$
   is the codimension of the subentity.
```

### Comparing `dune-geometry-2.9.0rc1/doc/refinement/simplexvertexindex.svg` & `dune-geometry-2.9.dev20220529/doc/refinement/simplexvertexindex.svg`

 * *Files identical despite different names*

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/affinegeometry.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/affinegeometry.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_AFFINEGEOMETRY_HH
 #define DUNE_GEOMETRY_AFFINEGEOMETRY_HH
 
 /** \file
  *  \brief An implementation of the Geometry interface for affine geometries
  *  \author Martin Nolte
  */
@@ -504,20 +502,14 @@
 
     /** \brief Type for the transposed Jacobian matrix */
     typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianTransposed;
 
     /** \brief Type for the transposed inverse Jacobian matrix */
     typedef FieldMatrix< ctype, coorddimension, mydimension > JacobianInverseTransposed;
 
-    /** \brief Type for the Jacobian matrix */
-    typedef FieldMatrix< ctype, coorddimension, mydimension > Jacobian;
-
-    /** \brief Type for the inverse Jacobian matrix */
-    typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianInverse;
-
   private:
     //! type of reference element
     typedef Geo::ReferenceElement< Geo::ReferenceElementImplementation< ctype, mydimension > > ReferenceElement;
 
     typedef Geo::ReferenceElements< ctype, mydimension > ReferenceElements;
 
     // Helper class to compute a matrix pseudo inverse
@@ -644,36 +636,14 @@
      *  \f[J^{-1}(x) J(x) = I.\f]
      */
     const JacobianInverseTransposed &jacobianInverseTransposed ([[maybe_unused]] const LocalCoordinate &local) const
     {
       return jacobianInverseTransposed_;
     }
 
-    /** \brief Obtain the Jacobian
-     *
-     *  \param[in]  local  local coordinate to evaluate Jacobian in
-     *
-     *  \returns a copy of the transposed of the Jacobian
-     */
-    Jacobian jacobian ([[maybe_unused]] const LocalCoordinate &local) const
-    {
-      return jacobianTransposed_.transposed();
-    }
-
-    /** \brief Obtain the Jacobian's inverse
-     *
-     *  The Jacobian's inverse is defined as a pseudo-inverse. If we denote
-     *  the Jacobian by \f$J(x)\f$, the following condition holds:
-     *  \f[J^{-1}(x) J(x) = I.\f]
-     */
-    JacobianInverse jacobianInverse ([[maybe_unused]] const LocalCoordinate &local) const
-    {
-      return jacobianInverseTransposed_.transposed();
-    }
-
     friend ReferenceElement referenceElement ( const AffineGeometry &geometry )
     {
       return geometry.refElement_;
     }
 
   private:
     ReferenceElement refElement_;
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/axisalignedcubegeometry.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/axisalignedcubegeometry.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_GEOMETRY_AXISALIGNED_CUBE_GEOMETRY_HH
 #define DUNE_GEOMETRY_AXISALIGNED_CUBE_GEOMETRY_HH
 
 /** \file
     \brief A geometry implementation for axis-aligned hypercubes
  */
@@ -86,32 +84,14 @@
         The FieldMatrix will never contain more than one entry per column,
         hence it could be replaced by something more efficient.
      */
     typedef typename std::conditional<dim==coorddim,
         DiagonalMatrix<ctype,dim>,
         FieldMatrix<ctype,coorddim,dim> >::type JacobianInverseTransposed;
 
-    /**
-     * \brief Return type of jacobian
-     *
-     * This is a fast DiagonalMatrix if dim==coorddim, and a FieldMatrix otherwise.
-     * The FieldMatrix will never contain more than one entry per row,
-     * hence it could be replaced by something more efficient.
-     */
-    using Jacobian = std::conditional_t<dim==coorddim, DiagonalMatrix<ctype,dim>, FieldMatrix<ctype,coorddim,dim> >;
-
-    /**
-     * \brief Return type of jacobianInverse
-     *
-     * This is a fast DiagonalMatrix if dim==coorddim, and a FieldMatrix otherwise.
-     * The FieldMatrix will never contain more than one entry per row,
-     * hence it could be replaced by something more efficient.
-     */
-    using JacobianInverse = std::conditional_t<dim==coorddim, DiagonalMatrix<ctype,dim>, FieldMatrix<ctype,dim,coorddim> >;
-
     /** \brief Constructor from a lower left and an upper right corner
 
         \note Only for dim==coorddim
      */
     AxisAlignedCubeGeometry(const Dune::FieldVector<ctype,coorddim> lower,
                             const Dune::FieldVector<ctype,coorddim> upper)
       : lower_(lower),
@@ -200,38 +180,26 @@
       // Actually compute the result.  Uses different methods depending
       // on what kind of matrix JacobianTransposed is.
       jacobianTransposed(result);
 
       return result;
     }
 
-    /** \brief Inverse Jacobian transposed of the transformation from local to global coordinates */
+    /** \brief Jacobian transposed of the transformation from local to global coordinates */
     JacobianInverseTransposed jacobianInverseTransposed([[maybe_unused]] const LocalCoordinate& local) const
     {
       JacobianInverseTransposed result;
 
       // Actually compute the result.  Uses different methods depending
       // on what kind of matrix JacobianTransposed is.
       jacobianInverseTransposed(result);
 
       return result;
     }
 
-    /** \brief Jacobian of the transformation from local to global coordinates */
-    Jacobian jacobian([[maybe_unused]] const LocalCoordinate& local) const
-    {
-      return jacobianTransposed(local).transposed();
-    }
-
-    /** \brief Inverse Jacobian of the transformation from local to global coordinates */
-    JacobianInverse jacobianInverse([[maybe_unused]] const LocalCoordinate& local) const
-    {
-      return jacobianInverseTransposed(local).transposed();
-    }
-
     /** \brief Return the integration element, i.e., the determinant term in the integral
                transformation formula
      */
     Volume integrationElement([[maybe_unused]] const LocalCoordinate& local) const
     {
       return volume();
     }
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/deprecated_topology.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/deprecated_topology.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_DEPRECATED_TOPOLOGY_HH
 #define DUNE_DEPRECATED_TOPOLOGY_HH
 
   namespace Impl
   {
 
     // Basic Topology Types
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/dimension.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/dimension.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_DIMENSION_HH
 #define DUNE_GEOMETRY_DIMENSION_HH
 
 #include <type_traits>
 
 namespace Dune {
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/generalvertexorder.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/generalvertexorder.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_GEOMETRY_GENERALVERTEXORDER_HH
 #define DUNE_GEOMETRY_GENERALVERTEXORDER_HH
 
 #include <algorithm>
 #include <cassert>
 #include <cstddef>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/multilineargeometry.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/multilineargeometry.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_MULTILINEARGEOMETRY_HH
 #define DUNE_GEOMETRY_MULTILINEARGEOMETRY_HH
 
 #include <cassert>
 #include <functional>
 #include <iterator>
 #include <limits>
@@ -199,20 +197,14 @@
 
     //! type of jacobian transposed
     typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianTransposed;
 
     //! type of jacobian inverse transposed
     class JacobianInverseTransposed;
 
-    /** \brief Type for the Jacobian matrix */
-    typedef FieldMatrix< ctype, coorddimension, mydimension > Jacobian;
-
-    /** \brief Type for the inverse Jacobian matrix */
-    typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianInverse;
-
   protected:
 
     typedef Dune::ReferenceElements< ctype, mydimension > ReferenceElements;
 
   public:
 
     //! type of reference element
@@ -393,37 +385,14 @@
     JacobianInverseTransposed jacobianInverseTransposed ( const LocalCoordinate &local ) const;
 
     friend ReferenceElement referenceElement ( const MultiLinearGeometry &geometry )
     {
       return geometry.refElement();
     }
 
-
-    /** \brief Obtain the Jacobian
-     *
-     *  \param[in]  local  local coordinate to evaluate Jacobian in
-     *
-     *  \returns a copy of the transposed of the Jacobian
-     */
-    Jacobian jacobian (const LocalCoordinate &local) const
-    {
-      return jacobianTransposed(local).transposed();
-    }
-
-    /** \brief Obtain the Jacobian's inverse
-     *
-     *  The Jacobian's inverse is defined as a pseudo-inverse. If we denote
-     *  the Jacobian by \f$J(x)\f$, the following condition holds:
-     *  \f[J^{-1}(x) J(x) = I.\f]
-     */
-    JacobianInverse jacobianInverse (const LocalCoordinate &local) const
-    {
-      return jacobianInverseTransposed(local).transposed();
-    }
-
   protected:
 
     ReferenceElement refElement () const
     {
       return refElement_;
     }
 
@@ -540,16 +509,14 @@
 
     typedef typename Base::LocalCoordinate LocalCoordinate;
     typedef typename Base::GlobalCoordinate GlobalCoordinate;
     typedef typename Base::Volume Volume;
 
     typedef typename Base::JacobianTransposed JacobianTransposed;
     typedef typename Base::JacobianInverseTransposed JacobianInverseTransposed;
-    typedef typename Base::Jacobian Jacobian;
-    typedef typename Base::JacobianInverse JacobianInverse;
 
     template< class CornerStorage >
     CachedMultiLinearGeometry ( const ReferenceElement &referenceElement, const CornerStorage &cornerStorage )
       : Base( referenceElement, cornerStorage ),
         affine_( Base::affine( jacobianTransposed_ ) ),
         jacobianInverseTransposedComputed_( false ),
         integrationElementComputed_( false )
@@ -689,36 +656,14 @@
         }
         return jacobianInverseTransposed_;
       }
       else
         return Base::jacobianInverseTransposed( local );
     }
 
-    /** \brief Obtain the Jacobian
-     *
-     *  \param[in]  local  local coordinate to evaluate Jacobian in
-     *
-     *  \returns a copy of the transposed of the Jacobian
-     */
-    Jacobian jacobian (const LocalCoordinate &local) const
-    {
-      return jacobianTransposed(local).transposed();
-    }
-
-    /** \brief Obtain the Jacobian's inverse
-     *
-     *  The Jacobian's inverse is defined as a pseudo-inverse. If we denote
-     *  the Jacobian by \f$J(x)\f$, the following condition holds:
-     *  \f[J^{-1}(x) J(x) = I.\f]
-     */
-    JacobianInverse jacobianInverse (const LocalCoordinate &local) const
-    {
-      return jacobianInverseTransposed(local).transposed();
-    }
-
   protected:
     using Base::refElement;
 
   private:
     mutable JacobianTransposed jacobianTransposed_;
     mutable JacobianInverseTransposed jacobianInverseTransposed_;
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/compositequadraturerule.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/compositequadraturerule.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_COMPOSITE_QUADRATURE_RULE_HH
 #define DUNE_GEOMETRY_COMPOSITE_QUADRATURE_RULE_HH
 
 /** \file
  * \brief Construct composite quadrature rules from other quadrature rules
  */
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussjacobi.mac` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussjacobi.mac`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 /*
- * SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
- * SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
- */
-/*
  * Run `maxima --batch gaussjacobi.mac'.
  */
 
 /* adjust search path */
 file_search_maxima: append(["$$$.{mac,max}"],file_search_maxima);
 
 load(orthopoly)$
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gausslobatto.mac` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gausslobatto.mac`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 /*
- * SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
- * SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
- */
-/*
  * Run `maxima --batch gausslobatto.mac'.
  */
 
 /* adjust search path */
 file_search_maxima: append(["$$$.{mac,max}"],file_search_maxima);
 
 load(orthopoly)$
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gausslobattoquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gausslobattoquadrature.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by gausslobatto.mac! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_GaussLobatto_HH
 #define DUNE_GEOMETRY_QUADRATURE_GaussLobatto_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussquadrature.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by jacobian.mac! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_Gauss_HH
 #define DUNE_GEOMETRY_QUADRATURE_Gauss_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussradau.mac` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussradau.mac`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 /*
- * SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
- * SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
- */
-/*
  * Run `maxima --batch gaussradau.mac'.
  */
 
 /* adjust search path */
 file_search_maxima: append(["$$$.{mac,max}"],file_search_maxima);
 
 load(orthopoly)$
@@ -24,15 +20,15 @@
   see https://mathworld.wolfram.com/RadauQuadrature.htm
 
   Left Gauss-Radau rule:
     inner points are given as the roots of (legendre_{n-1} + legendre_{n})/(x + 1),
     the outer point -1 is obtained by multiplication with (x + 1)
 
   Right Gauss-Radau rule:
-    substitute x by -x
+    substitue x by -x
 */
 points_left(n) := legendre_p(n-1,x) + legendre_p(n, x)$
 weights_left(n,xx) := at(ratsimp((1 - x)/(n*n*legendre_p(n-1,x)^2)), x=xx)$
 
 points_right(n) := legendre_p(n-1,-x) + legendre_p(n, -x)$
 weights_right(n,xx) := at(ratsimp((1 + x)/(n*n*legendre_p(n-1,-x)^2)), x=xx)$
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussradauleftquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussradauleftquadrature.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by gaussradau.mac! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_GaussRadauLeft_HH
 #define DUNE_GEOMETRY_QUADRATURE_GaussRadauLeft_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/gaussradaurightquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/gaussradaurightquadrature.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by gaussradau.mac! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_GaussRadauRight_HH
 #define DUNE_GEOMETRY_QUADRATURE_GaussRadauRight_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/jacobi1quadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/jacobi1quadrature.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by jacobian.mac! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_Jacobi1_HH
 #define DUNE_GEOMETRY_QUADRATURE_Jacobi1_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/jacobi2quadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/jacobi2quadrature.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by jacobian.mac! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_Jacobi2_HH
 #define DUNE_GEOMETRY_QUADRATURE_Jacobi2_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/jacobiNquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/jacobiNquadrature.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_QUADRATURERULES_JACOBI_N_0_H
 #define DUNE_GEOMETRY_QUADRATURERULES_JACOBI_N_0_H
 
 #include <vector>
 #include <type_traits>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/pointquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/pointquadrature.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_QUADRATURE_POINT_HH
 #define DUNE_GEOMETRY_QUADRATURE_POINT_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
 #error This is a private header that should not be included directly.
 #error Use #include <dune/geometry/quadraturerules.hh> instead.
 #endif
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/prismquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/prismquadrature.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_QUADRATURE_PRISM_HH
 #define DUNE_GEOMETRY_QUADRATURE_PRISM_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
 #error This is a private header that should not be included directly.
 #error Use #include <dune/geometry/quadraturerules.hh> instead.
 #endif
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/simplexquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/simplexquadrature.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_QUADRATURE_SIMPLEX_HH
 #define DUNE_GEOMETRY_QUADRATURE_SIMPLEX_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
 #error This is a private header that should not be included directly.
 #error Use #include <dune/geometry/quadraturerules.hh> instead.
 #endif
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/tensorproductquadrature.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/tensorproductquadrature.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_QUADRATURERULES_TENSORPRODUCTQUADRATURE_HH
 #define DUNE_GEOMETRY_QUADRATURERULES_TENSORPRODUCTQUADRATURE_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
 #error This is a private header that should not be included directly.
 #error Use #include <dune/geometry/quadraturerules.hh> instead.
 #endif
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules/writequad.mac` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules/writequad.mac`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-/*
- * SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
- * SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
- */
 load(to_poly_solve)$
 
 epsilon: 1e-110$
 
 
 /*
   write_quad computes the points and weights for quadrature rules.
@@ -31,16 +27,14 @@
 write_quad(file, name, scriptname, points_generator, weights_generator, max_order, num_endpoints) :=
 block([delivered_order,twice_free_points,free_points,num_points,points,weights,S,i,p,w,fd],
 
 fd: openw(file),
 
 printf(fd, "// -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 //
 // WARNING
 // This file is automatically generated by ~a! Don't edit by hand!
 #ifndef DUNE_GEOMETRY_QUADRATURE_~a_HH
 #define DUNE_GEOMETRY_QUADRATURE_~a_HH
 
 #ifndef DUNE_INCLUDING_IMPLEMENTATION
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/quadraturerules.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/quadraturerules.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_GEOMETRY_QUADRATURERULES_HH
 #define DUNE_GEOMETRY_QUADRATURERULES_HH
 
 #include <algorithm>
 #include <iostream>
 #include <limits>
@@ -83,15 +81,15 @@
       /** \brief Gauss-Legendre rules (default)
       *
       *  -1D: Gauss-Jacobi rule with parameters \f$\alpha = \beta =0 \f$, i.e. for integrals with a constant weight function.
       *       The quadrature points do not include interval endpoints.
       *       Polynomials of order 2n - 1 can be integrated exactly.
       *  -higher dimension: For the 2D/3D case efficient rules for certain geometries may be used if available.
       *                     Higher dimensional quadrature rules are constructed via \p TensorProductQuadratureRule.
-      *                     In this case the 1D rules eventually need higher order to compensate occurring weight functions(i.e. simplices).
+      *                     In this case the 1D rules eventually need higher order to compensate occuring weight functions(i.e. simplices).
       */
       GaussLegendre = 0,
 
       /** \brief Gauss-Jacobi rules with \f$\alpha =1\f$
       *
       *  -1D Gauss-Jacobi rule with parameters \f$\alpha =1,\ \beta =0 \f$
       *  -Is used to construct efficient simplex quadrature rules of higher order
@@ -106,15 +104,15 @@
       GaussJacobi_2_0 = 2,
 
       /** \brief Gauss-Legendre rules with \f$\alpha =n\f$
       *
       *  -1D: Gauss-Jacobi rule with parameters \f$\alpha = n,\ \beta =0 \f$
       *  -higher dimension: For the 2D/3D case efficient rules for certain geometries may be used if available.
       *                     Higher dimensional quadrature rules are constructed via \p TensorProductQuadratureRule.
-      *                     In this case the 1D rules respect eventually occurring weight functions(i.e. simplices).
+      *                     In this case the 1D rules respect eventually occuring weight functions(i.e. simplices).
       *  -The rules for high dimension or order are computed at run time and only floating point number types are supported.(LAPACK is needed for this case)
       *  -Most efficient quadrature type for simplices.
       *
       *   \note For details please use the book "Approximate Calculation of Multiple Integrals" by A.H. Stroud published in 1971.
       */
       GaussJacobi_n_0 = 3,
 
@@ -196,67 +194,83 @@
   /** \brief A container for all quadrature rules of dimension <tt>dim</tt>
       \ingroup Quadrature
    */
   template<typename ctype, int dim>
   class QuadratureRules {
 
     /** \brief Internal short-hand notation for the type of quadrature rules this container contains */
-    using QuadratureRule = Dune::QuadratureRule<ctype, dim>;
-
-    // indexed by quadrature order
-    using QuadratureOrderVector = std::vector<std::pair<std::once_flag, QuadratureRule> >;
+    typedef Dune::QuadratureRule<ctype, dim> QuadratureRule;
+    //! \brief a quadrature rule (for each quadrature order, geometry type,
+    //!        and quadrature type)
+    static void initQuadratureRule(QuadratureRule *qr, QuadratureType::Enum qt,
+                                   const GeometryType &t, int p)
+    {
+      *qr = QuadratureRuleFactory<ctype,dim>::rule(t,p,qt);
+    }
 
-    // indexed by geometry type
-    using GeometryTypeVector = std::vector<std::pair<std::once_flag, QuadratureOrderVector> >;
+    typedef std::vector<std::pair<std::once_flag, QuadratureRule> >
+      QuadratureOrderVector; // indexed by quadrature order
+    //! \brief initialize the vector indexed by the quadrature order (for each
+    //!        geometry type and quadrature type)
+    static void initQuadratureOrderVector(QuadratureOrderVector *qov,
+                                          QuadratureType::Enum qt,
+                                          const GeometryType &t)
+    {
+      if(dim == 0)
+        // we only need one quadrature rule for points, not maxint
+        *qov = QuadratureOrderVector(1);
+      else
+        *qov = QuadratureOrderVector(QuadratureRuleFactory<ctype,dim>::maxOrder(t,qt)+1);
+    }
 
-    // indexed by quadrature type enum
-    using QuadratureCacheVector = std::vector<std::pair<std::once_flag, GeometryTypeVector> >;
+    typedef std::vector<std::pair<std::once_flag, QuadratureOrderVector> >
+      GeometryTypeVector; // indexed by geometry type
+    //! \brief initialize the vector indexed by the geometry type (for each
+    //!        quadrature type)
+    static void initGeometryTypeVector(GeometryTypeVector *gtv)
+    {
+      *gtv = GeometryTypeVector(LocalGeometryTypeIndex::size(dim));
+    }
 
     //! real rule creator
-    DUNE_EXPORT const QuadratureRule& _rule(const GeometryType& t, int p, QuadratureType::Enum qt=QuadratureType::GaussLegendre) const
+    DUNE_EXPORT const QuadratureRule& _rule(const GeometryType& t, int p, QuadratureType::Enum qt=QuadratureType::GaussLegendre)
     {
       assert(t.dim()==dim);
 
       DUNE_ASSERT_CALL_ONCE();
 
-      static QuadratureCacheVector quadratureCache(QuadratureType::size);
-
-      auto& [ onceFlagQuadratureType, geometryTypes ] = quadratureCache[qt];
-      // initialize geometry types for this quadrature type once
-      std::call_once(onceFlagQuadratureType, [&types = geometryTypes]{
-        types = GeometryTypeVector(LocalGeometryTypeIndex::size(dim));
-      });
-
-      auto& [ onceFlagGeometryType, quadratureOrders ] = geometryTypes[LocalGeometryTypeIndex::index(t)];
-      // initialize quadrature orders for this geometry type and quadrature type once
-      std::call_once(onceFlagGeometryType, [&, &orders = quadratureOrders]{
-        // we only need one quadrature rule for points, not maxint
-        const auto numRules = dim == 0 ? 1 : QuadratureRuleFactory<ctype,dim>::maxOrder(t, qt)+1;
-        orders = QuadratureOrderVector(numRules);
-      });
+      static std::vector<std::pair< // indexed by quadrature type
+        std::once_flag,
+        GeometryTypeVector
+        > > quadratureCache(QuadratureType::size);
+
+      auto & quadratureTypeLevel = quadratureCache[qt];
+      std::call_once(quadratureTypeLevel.first, initGeometryTypeVector,
+                     &quadratureTypeLevel.second);
+
+      auto & geometryTypeLevel =
+        quadratureTypeLevel.second[LocalGeometryTypeIndex::index(t)];
+      std::call_once(geometryTypeLevel.first, initQuadratureOrderVector,
+                     &geometryTypeLevel.second, qt, t);
 
       // we only have one quadrature rule for points
-      auto& [ onceFlagQuadratureOrder, quadratureRule ] = quadratureOrders[dim == 0 ? 0 : p];
-      // initialize quadrature rule once
-      std::call_once(onceFlagQuadratureOrder, [&, &rule = quadratureRule]{
-        rule = QuadratureRuleFactory<ctype,dim>::rule(t, p, qt);
-      });
+      auto & quadratureOrderLevel = geometryTypeLevel.second[dim == 0 ? 0 : p];
+      std::call_once(quadratureOrderLevel.first, initQuadratureRule,
+                     &quadratureOrderLevel.second, qt, t, p);
 
-      return quadratureRule;
+      return quadratureOrderLevel.second;
     }
-
     //! singleton provider
     DUNE_EXPORT static QuadratureRules& instance()
     {
       static QuadratureRules instance;
       return instance;
     }
-
     //! private constructor
-    QuadratureRules () = default;
+    QuadratureRules () {}
   public:
     //! maximum quadrature order for given geometry type and quadrature type
     static unsigned
     maxOrder(const GeometryType& t,
              QuadratureType::Enum qt=QuadratureType::GaussLegendre)
     {
       return QuadratureRuleFactory<ctype,dim>::maxOrder(t,qt);
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/referenceelement.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/referenceelement.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFERENCEELEMENT_HH
 #define DUNE_GEOMETRY_REFERENCEELEMENT_HH
 
 #include <dune/geometry/type.hh>
 
 namespace Dune {
   namespace Geo {
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/referenceelementimplementation.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/referenceelementimplementation.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <dune/geometry/referenceelementimplementation.hh>
 
 namespace Dune
 {
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/referenceelementimplementation.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/referenceelementimplementation.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFERENCEELEMENTIMPLEMENTATION_HH
 #define DUNE_GEOMETRY_REFERENCEELEMENTIMPLEMENTATION_HH
 
 #include <cassert>
 
 #include <algorithm>
 #include <limits>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/referenceelements.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/referenceelements.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFERENCEELEMENTS_HH
 #define DUNE_GEOMETRY_REFERENCEELEMENTS_HH
 
 #include <cassert>
 
 #include <algorithm>
 #include <limits>
@@ -360,15 +358,15 @@
     using DefaultReferenceElement = typename DefaultReferenceElementExtractor<T...>::type;
 
   }
 
   // looks up the type of a reference element by trying to instantiate the correct overload
   // of referenceElement() for the given arguments. This will fail if there is no valid
   // overload and should be used with detected_or or some other utility that places the
-  // instantiation in SFINAE context.
+  // instantation in SFINAE context.
   //
   // this is placed directly in namespace Dune to avoid any weird surprises
 
   template<typename... T>
   using LookupReferenceElement = decltype(referenceElement(std::declval<T>()...));
 
 #endif // DOXYGEN
@@ -420,15 +418,15 @@
 
   }
 
 #ifndef DOXYGEN
 
   namespace Impl {
 
-    // helpers for triggering a deprecation warning for occurrences of the old
+    // helpers for triggering a deprecation warning for occurences of the old
     // ReferenceElement syntax (Dune::ReferenceElement<T,int>)
 
     // this looks a little weird, encoding the type in the return type of a nested function,
     // but it was the only reliable way to trigger the warning iff the compiler encounters
     // an invalid use. Other solutions either miss some (or all) uses or trigger false alarms.
 
     template<typename T>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement/base.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement/base.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFINEMENT_BASE_CC
 #define DUNE_GEOMETRY_REFINEMENT_BASE_CC
 
 /*!
  * \file
  *
  * \brief This file contains the parts independent of a particular
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement/hcube.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement/hcube.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFINEMENT_HCUBE_CC
 #define DUNE_GEOMETRY_REFINEMENT_HCUBE_CC
 
 /*!
  * \file
  * \brief This file contains the \ref Refinement implementation for
  *        hypercubes (quadrilaterals, hexahedrons, etc.).
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement/hcubetriangulation.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement/hcubetriangulation.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFINEMENT_HCUBETRIANGULATION_CC
 #define DUNE_GEOMETRY_REFINEMENT_HCUBETRIANGULATION_CC
 
 /*!
  * \file
  * \brief This file contains the \ref Refinement implementation for
  *        triangulating hypercubes (quadrilateral -> triangle,
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement/prismtriangulation.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement/prismtriangulation.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFINEMENT_PRISMTRIANGULATION_CC
 #define DUNE_GEOMETRY_REFINEMENT_PRISMTRIANGULATION_CC
 
 #include <dune/common/fvector.hh>
 #include <dune/common/typetraits.hh>
 
 #include <dune/geometry/referenceelements.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement/pyramidtriangulation.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement/pyramidtriangulation.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFINEMENT_PYRAMIDTRIANGULATION_CC
 #define DUNE_GEOMETRY_REFINEMENT_PYRAMIDTRIANGULATION_CC
 
 #include <dune/common/fvector.hh>
 #include <dune/common/typetraits.hh>
 
 #include <dune/geometry/referenceelements.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement/simplex.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement/simplex.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_COMMON_REFINEMENT_SIMPLEX_CC
 #define DUNE_GRID_COMMON_REFINEMENT_SIMPLEX_CC
 
 // This file is part of DUNE, a Distributed and Unified Numerics Environment
 // This file is copyright (C) 2005 Jorrit Fahlke <jorrit@jorrit.de>
 // This file is licensed under version 2 of the GNU General Public License,
 // with a special "runtime exception."  See COPYING at the top of the source
@@ -102,15 +100,15 @@
 
    @image html simplexvertexindex.png "The image shows the Kuhn0 tetrahedron of width 2 (wireframe).  It is partitioned into a tetrahedron (green), a triangle (red), a line (blue), and a vertex (black), each of width 1 and each a Kuhn0 simplex."
 
    Let us calculate the index of vertex 9, which has the coordinates
    \f$(x_0,x_1,x_2)=(2,2,2)\f$.
    - First we count the number of vertices in the green tetrahedron of
     width \f$x_0-1=1\f$ (4).  Then we take the green tetrahedron away.
-    What's left is a triangle, which extends into the (1,2)-plane.
+    Whats left is a triangle, which extends into the (1,2)-plane.
    - Now we count the number of vertices in the red triangle of width
     \f$x_1-1=1\f$ (3).  Again we take the counted points away and are
     left with a line which extends into direction 2.
    - We take the blue line of width \f$x_2-1=1\f$, count the number of
     vertices (2), and throw away the counted stuff.  The only thing
     remaining is a point, so we're done.
    - We add the counted stuff together and get indeed 9.
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/refinement.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/refinement.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_REFINEMENT_HH
 #define DUNE_GEOMETRY_REFINEMENT_HH
 
 /*!
  * \file
  * \brief This file simply includes all \ref Refinement implementations
  *        so you don't have to do them separately.
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/CMakeLists.txt` & `dune-geometry-2.9.dev20220529/dune/geometry/test/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 dune_add_test(SOURCES test-affinegeometry.cc
               LINK_LIBRARIES dunegeometry)
 
 dune_add_test(SOURCES test-axisalignedcubegeometry.cc
               LINK_LIBRARIES dunegeometry)
 
 # whether the compiler is affected by
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/checkgeometry.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/test/checkgeometry.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_CHECK_GEOMETRY_HH
 #define DUNE_CHECK_GEOMETRY_HH
 
 #include <limits>
 
 #include <dune/common/typetraits.hh>
@@ -15,47 +13,14 @@
 #include <dune/geometry/referenceelements.hh>
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/geometry/referenceelements.hh>
 
 namespace Dune
 {
 
-  namespace Impl
-  {
-
-    // Helper function to convert a matrix to a FieldMatrix
-    // using only the mv method.
-    template<class ctype, int rows, int cols, class M>
-    Dune::FieldMatrix<ctype, rows, cols> toFieldMatrix(const M& m){
-      Dune::FieldMatrix<ctype, rows, cols> result;
-      for (int j=0; j<cols; j++) {
-        FieldVector<ctype,cols> idColumn(0);
-        idColumn[j] = 1;
-        FieldVector<ctype,rows> column;
-        m.mv(idColumn,column);
-        for (int k=0; k<rows; k++)
-          result[k][j] = column[k];
-      }
-      return result;
-    }
-
-    // Helper function to check if FieldMatrix is an identity matrix
-    template<class ctype, int rows, int cols>
-    bool isIdentity(const Dune::FieldMatrix<ctype, rows, cols>& m, double tolerance){
-      if (rows != cols)
-        return false;
-      for(int i=0; i<rows; ++i)
-        for(int j=0; j<rows; ++j)
-          if (std::abs(m[i][j] - (i == j ? 1 : 0)) >= tolerance)
-            return false;
-      return true;
-    }
-
-  }
-
   /**
    * \brief Static and dynamic checks for all features of a Geometry
    *
    * This excludes anything related to being part of a grid.
    *
    * \tparam TestGeometry The type of the geometry to be tested
    *
@@ -91,20 +56,14 @@
 
     // Matrix-like type for the return value of the jacobianTransposed method
     typedef typename TestGeometry::JacobianTransposed JacobianTransposed;
 
     // Matrix-like type for the return value of the jacobianInverseTransposed method
     typedef typename TestGeometry::JacobianInverseTransposed JacobianInverseTransposed;
 
-    // Matrix-like type for the return value of the jacobian method
-    typedef typename TestGeometry::Jacobian Jacobian;
-
-    // Matrix-like type for the return value of the jacobianInverse method
-    typedef typename TestGeometry::JacobianInverse JacobianInverse;
-
     const ctype tolerance = std::sqrt( std::numeric_limits< ctype >::epsilon() );
 
     ////////////////////////////////////////////////////////////////////////
 
     const int corners = geometry.corners();
     if( corners == 0 )
       DUNE_THROW( Exception, "A geometry must have at least one corner." );
@@ -198,85 +157,80 @@
 
       // Test whether the methods 'local' and 'global' are inverse to each other
       if ( (x - geometry.local( geometry.global( x ) )).two_norm() > tolerance ) {
         std::cerr << "Error: global and local are not inverse to each other." << std::endl;
         pass = false;
       }
 
-      const JacobianTransposed &Jt = geometry.jacobianTransposed( x );
-      const JacobianInverseTransposed &Jit = geometry.jacobianInverseTransposed( x );
-      const Jacobian &J = geometry.jacobian( x );
-      const JacobianInverse &Ji = geometry.jacobianInverse( x );
-
-      // Transform to FieldMatrix, so we can have coefficient access and other goodies
-      auto JtAsFieldMatrix = Impl::toFieldMatrix< ctype, mydim, coorddim >(Jt);
-      auto JitAsFieldMatrix = Impl::toFieldMatrix< ctype, coorddim, mydim >(Jit);
-      auto JAsFieldMatrix = Impl::toFieldMatrix< ctype, coorddim, mydim >(J);
-      auto JiAsFieldMatrix = Impl::toFieldMatrix< ctype, mydim, coorddim >(Ji);
-
-
       // Test whether the methods 'jacobianTransposed' and 'jacobianInverseTransposed'
       // return matrices that are inverse to each other.
-      {
-        FieldMatrix< ctype, mydim, mydim > id = JtAsFieldMatrix * JitAsFieldMatrix;
-        if(not Impl::isIdentity(id, tolerance))
-        {
-          std::cerr << "Error: jacobianTransposed and jacobianInverseTransposed are not inverse to each other." << std::endl;
-          std::cout << "       id != [ ";
-          for( int j = 0; j < mydim; ++j )
-            std::cout << (j > 0 ? " | " : "") << id[ j ];
-          std::cout << " ]" << std::endl;
-          pass = false;
-        }
-      }
+      const JacobianTransposed &jt = geometry.jacobianTransposed( x );
+      const JacobianInverseTransposed &jit = geometry.jacobianInverseTransposed( x );
+
+      // Transform to FieldMatrix, so we can have coefficent access and other goodies
+      // We need some black magic for the transformation, because there is no
+      // official easy way yet.
+      // The following code does the transformation by multiplying jt and jit from
+      // the right by identity matrices.  That way, only the mv method is used.
+      FieldMatrix< ctype, mydim, coorddim > jtAsFieldMatrix;
+      for (int j=0; j<coorddim; j++) {
+
+        FieldVector<ctype,coorddim> idColumn(0);
+        idColumn[j] = 1;
+
+        FieldVector<ctype,mydim> column;
+        jt.mv(idColumn,column);
+
+        for (int k=0; k<mydim; k++)
+          jtAsFieldMatrix[k][j] = column[k];
 
-      // Test whether the methods 'jacobian' and 'jacobianInverse'
-      // return matrices that are inverse to each other.
-      {
-        FieldMatrix< ctype, mydim, mydim > id = JiAsFieldMatrix * JAsFieldMatrix;
-        if(not Impl::isIdentity(id, tolerance))
-        {
-          std::cerr << "Error: jacobian and jacobianInverse are not inverse to each other." << std::endl;
-          std::cout << "       id != [ ";
-          for( int j = 0; j < mydim; ++j )
-            std::cout << (j > 0 ? " | " : "") << id[ j ];
-          std::cout << " ]" << std::endl;
-          pass = false;
-        }
       }
 
-      // Test whether the methods 'jacobianTransposed' and 'jacobianInverseTransposed'
-      // are the transposed of 'jacobian' and 'jacobianInverse', respectively.
-      {
-        if( (JtAsFieldMatrix - JAsFieldMatrix.transposed()).infinity_norm() != 0 )
-        {
-          std::cerr << "Error: jacobian and jacobianTransposed are not transposed to each other." << std::endl;
-          pass = false;
-        }
+      FieldMatrix< ctype, coorddim, mydim > jitAsFieldMatrix;
+      for (int j=0; j<mydim; j++) {
+
+        FieldVector<ctype,mydim> idColumn(0);
+        idColumn[j] = 1;
+
+        FieldVector<ctype,coorddim> column;
+        jit.mv(idColumn,column);
+
+        for (int k=0; k<coorddim; k++)
+          jitAsFieldMatrix[k][j] = column[k];
+
       }
+
+
+      FieldMatrix< ctype, mydim, mydim > id;
+      FMatrixHelp::multMatrix( jtAsFieldMatrix, jitAsFieldMatrix, id );
+      bool isId = true;
+      for( int j = 0; j < mydim; ++j )
+        for( int k = 0; k < mydim; ++k )
+          isId &= (std::abs( id[ j ][ k ] - (j == k ? 1 : 0) ) < tolerance);
+      if( !isId)
       {
-        if( (JitAsFieldMatrix - JiAsFieldMatrix.transposed()).infinity_norm() != 0 )
-        {
-          std::cerr << "Error: jacobianInverse and jacobianInverseTransposed are not transposed to each other." << std::endl;
-          pass = false;
-        }
+        std::cerr << "Error: jacobianTransposed and jacobianInverseTransposed are not inverse to each other." << std::endl;
+        std::cout << "       id != [ ";
+        for( int j = 0; j < mydim; ++j )
+          std::cout << (j > 0 ? " | " : "") << id[ j ];
+        std::cout << " ]" << std::endl;
+        pass = false;
       }
 
-
       // Test whether integrationElement returns something nonnegative
       if( geometry.integrationElement( x ) < 0 ) {
         std::cerr << "Error: Negative integrationElement found." << std::endl;
         pass = false;
       }
 
       FieldMatrix< ctype, mydim, mydim > jtj( 0 );
       for( int i = 0; i < mydim; ++i )
         for( int j = 0; j < mydim; ++j )
           for( int k = 0; k < coorddim; ++k )
-            jtj[ i ][ j ] += JtAsFieldMatrix[ i ][ k ] * JtAsFieldMatrix[ j ][ k ];
+            jtj[ i ][ j ] += jtAsFieldMatrix[ i ][ k ] * jtAsFieldMatrix[ j ][ k ];
 
       if( abs( sqrt( jtj.determinant() ) - geometry.integrationElement( x ) ) > tolerance ) {
         std::cerr << "Error: integrationElement is not consistent with jacobianTransposed." << std::endl;
         pass = false;
       }
       if (geometry.affine())
         if( abs( geometry.volume() - refElement.volume()*geometry.integrationElement( x ) ) > tolerance ) {
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-affinegeometry.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-affinegeometry.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <vector>
 
 #include <dune/geometry/affinegeometry.hh>
 #include <dune/geometry/referenceelements.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-axisalignedcubegeometry.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-axisalignedcubegeometry.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /** \file
     \brief A unit test for the AxisAlignedCubeGeometry class
  */
 
 #if HAVE_CONFIG_H
 #include <config.h>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-cornerstoragerefwrap.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-cornerstoragerefwrap.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /** @file
  *
  * \brief Test std::reference_wrapper<SomeContainer> as the CornerStorage in
  *        MultiLinearGeometry.
  */
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-fromvertexcount.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-fromvertexcount.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <string>
 #include <iostream>
 #include <vector>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-multilineargeometry.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-multilineargeometry.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <functional>
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-quadrature.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-quadrature.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <algorithm>
 #include <limits>
 #include <iostream>
 #include <type_traits>
 
 #include <config.h>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-referenceelements.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-referenceelements.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /** \file
     \brief A unit test for the ReferenceElements
     \todo For several element types the subEntities() method is not tested yet!
  */
 
 #include <config.h>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/test/test-refinement.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/test/test-refinement.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 /*!
  * \file
  * \brief Unit tests for the virtual refinement code
  */
 
 #include "config.h"
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/topologyfactory.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/topologyfactory.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_TOPOLOGYFACTORY_HH
 #define DUNE_GEOMETRY_TOPOLOGYFACTORY_HH
 
 #include <cassert>
 
 #include <array>
 #include <map>
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/type.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/type.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_TYPE_HH
 #define DUNE_GEOMETRY_TYPE_HH
 
 /** \file
  *  \brief A unique label for each type of element that can occur in a grid
  */
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/typeindex.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/typeindex.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_TYPEINDEX_HH
 #define DUNE_GEOMETRY_TYPEINDEX_HH
 
 /**
  * \file
  * \brief Helper classes to provide indices for geometrytypes for use in a
  *        vector
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/utility/typefromvertexcount.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/utility/typefromvertexcount.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_TYPE_FROM_VERTEX_COUNT_HH
 #define DUNE_GEOMETRY_TYPE_FROM_VERTEX_COUNT_HH
 
 #include <dune/geometry/type.hh>
 
 namespace Dune {
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/virtualrefinement.cc` & `dune-geometry-2.9.dev20220529/dune/geometry/virtualrefinement.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_GEOMETRY_VIRTUALREFINEMENT_CC
 #define DUNE_GEOMETRY_VIRTUALREFINEMENT_CC
 
 /*!
  * \file
  * \brief This file contains the virtual wrapper around refinement.
```

### Comparing `dune-geometry-2.9.0rc1/dune/geometry/virtualrefinement.hh` & `dune-geometry-2.9.dev20220529/dune/geometry/virtualrefinement.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GEOMETRY_VIRTUALREFINEMENT_HH
 #define DUNE_GEOMETRY_VIRTUALREFINEMENT_HH
 
 /*!
  * \file
  *
  * \brief This file contains the virtual wrapper around refinement.
@@ -30,15 +28,15 @@
  * geometryTypes, this can be quiet annoying.
  *
  * VirtualRefinement does all of this switch() statements for you.  It
  * defines a common virtual base class per dimension, and derives one
  * class for each geometryType and coerceTo from that class.  The
  * derived classes simply wrap the non-virtual classes from \link
  * Refinement Refinement\endlink.  This makes it possible to treat each
- * geometryType (of a given dimension) the same, and thus eliminates
+ * geometryType (of a given dimension) the same, and thus eleminates
  * the many repetitions of lots of code.
  *
  * But the case statements are not totally gone yet.  VirtualRefinement
  * does these statements once and for all by wrapping them into the
  * buildRefinement() function.
  *
  * \section Virtual_User_interface The user Interface
@@ -229,15 +227,15 @@
  * \subsection Virtual_Iterators The iterators
  * <!-------------------------------->
  *
  * We can't do the same thing with the iterators as we do with class
  * VirtualRefinement.  Since they are polymorph we cannot simply pass
  * them into user code.  They are not singletons, so we also cannot
  * pass references to them.  Passing pointers to iterators would work,
- * but then the programmer has to remember to explicitly delete them.
+ * but then the programmer has to remember to explecitely delete them.
  * Also, it is uncommon for iterators to be handled by their pointers.
  *
  * What we do instead is having a wrapper class which conforms to the
  * iterator interface and is the same for all
  * VirtualRefinementIterators of a given dimension.  This class
  * contains a pointer to a polymorph backend object implementing the
  * iterator.  The various VirtualRefinementImps then derive from the
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/geometry/multilineargeometry.hh` & `dune-geometry-2.9.dev20220529/dune/python/geometry/multilineargeometry.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #ifndef DUNE_PYTHON_GEOMETRY_MULTILINEARGEOMETRY_HH
 #define DUNE_PYTHON_GEOMETRY_MULTILINEARGEOMETRY_HH
 
 #include <type_traits>
 
 #include <dune/common/visibility.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/geometry/quadraturerules.hh` & `dune-geometry-2.9.dev20220529/dune/python/geometry/quadraturerules.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_GEOMETRY_QUADRATURERULES_HH
 #define DUNE_PYTHON_GEOMETRY_QUADRATURERULES_HH
 
 #include <array>
 #include <tuple>
 
 #include <dune/common/visibility.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/geometry/referenceelements.hh` & `dune-geometry-2.9.dev20220529/dune/python/geometry/referenceelements.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_GEOMETRY_REFERENCEELEMENTS_HH
 #define DUNE_PYTHON_GEOMETRY_REFERENCEELEMENTS_HH
 
 #include <array>
 #include <functional>
 #include <string>
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/geometry/type.hh` & `dune-geometry-2.9.dev20220529/dune/python/geometry/type.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_GEOMETRY_TYPE_HH
 #define DUNE_PYTHON_GEOMETRY_TYPE_HH
 
 #include <cassert>
 
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/test/CMakeLists.txt` & `dune-geometry-2.9.dev20220529/dune/python/test/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 dune_python_add_test(NAME pyrefelement
                      SCRIPT refelement.py
                      WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
                      LABELS quick)
 dune_python_add_test(NAME pygeometrytype
                      SCRIPT geometrytype.py
                      WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/test/geometrytype.py` & `dune-geometry-2.9.dev20220529/dune/python/test/geometrytype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from dune.geometry import *
 
 # make sure t can be reconstructed from str(t)
 for t in (vertex, line, triangle, quadrilateral, tetrahedron, pyramid, prism, hexahedron):
     assert GeometryType(str(t)) == t
 
 for d in range(10):
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/test/refelement.py` & `dune-geometry-2.9.dev20220529/dune/python/test/refelement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from dune.geometry import referenceElement
 from dune.geometry import vertex, line, triangle, quadrilateral, tetrahedron, pyramid, prism, hexahedron, none
 
 def test(r):
     for codim in range(r.dimension+1):
         types = r.types(codim)
         if len(types) != r.size(codim):
```

### Comparing `dune-geometry-2.9.0rc1/dune/python/test/test_quad.py` & `dune-geometry-2.9.dev20220529/dune/python/test/test_quad.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import time, math, numpy
 import dune.geometry as geo
 
 def monomial(p):
     def function(point):
         return sum( x**p for x in point)
     return function
```

### Comparing `dune-geometry-2.9.0rc1/pyproject.toml` & `dune-geometry-2.9.dev20220529/pyproject.toml`

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

### Comparing `dune-geometry-2.9.0rc1/python/dune/geometry/_geometry.cc` & `dune-geometry-2.9.dev20220529/python/dune/geometry/_geometry.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 #include <dune/python/geometry/type.hh>
 #include <dune/python/pybind11/pybind11.h>
 
 PYBIND11_MODULE( _geometry, module )
 {
   Dune::Python::registerGeometryType( module );
```

### Comparing `dune-geometry-2.9.0rc1/python/dune/geometry/_referenceelements.py` & `dune-geometry-2.9.dev20220529/python/dune/geometry/_referenceelements.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from dune.generator.generator import SimpleGenerator
 from dune.common.hashit import hashIt
 def module(dim):
     typeName = "Dune::Geo::ReferenceElement<Dune::Geo::ReferenceElementImplementation<double," + str(dim) + "> >"
     includes = ["dune/python/geometry/referenceelements.hh"]
     typeHash = "referenceelements_" + hashIt(typeName)
     generator = SimpleGenerator("ReferenceElements", "Dune::Python")
```

### Comparing `dune-geometry-2.9.0rc1/python/dune/geometry/quadpy.py` & `dune-geometry-2.9.dev20220529/python/dune/geometry/quadpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import logging
 
 logger = logging.getLogger(__name__)
 
 try:
     import quadpy as qp
     import numpy
```

### Comparing `dune-geometry-2.9.0rc1/python/dune_geometry.egg-info/PKG-INFO` & `dune-geometry-2.9.dev20220529/python/dune_geometry.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-geometry
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Geometry Transformations, Reference Elements and Quadrature Rules
 Home-page: https://gitlab.dune-project.org/core/dune-geometry
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
         
         
-        git-273db91ded0a5807cb45ab6d21e7cbdd6970dc11
+        git-96a9468acdc641888f54374fc7b16682667867fd
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

