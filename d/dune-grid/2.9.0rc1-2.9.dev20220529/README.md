# Comparing `tmp/dune-grid-2.9.0rc1.tar.gz` & `tmp/dune-grid-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-grid-2.9.0rc1.tar", last modified: Fri Oct 21 08:16:55 2022, max compression
+gzip compressed data, was "dune-grid-2.9.dev20220529.tar", last modified: Sun May 29 21:03:33 2022, max compression
```

## Comparing `dune-grid-2.9.0rc1.tar` & `dune-grid-2.9.dev20220529.tar`

### file list

```diff
@@ -1,716 +1,639 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)    14504 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20951 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)    20951 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.220006 dune-grid-2.9.0rc1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    19036 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.216006 dune-grid-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.220006 dune-grid-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/cmake/modules/AddAlbertaFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/cmake/modules/DuneGridMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3165 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/cmake/modules/FindAlberta.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/cmake/modules/GridType.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/cmake/modules/UseUG.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.220006 dune-grid-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.220006 dune-grid-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     3145 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/doxygen/Doxydep
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/doxygen/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/doxygen/modules.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.220006 dune-grid-2.9.0rc1/doc/grids/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.220006 dune-grid-2.9.0rc1/doc/grids/amc/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-1-1.amc
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-1-2.amc
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-1-3.amc
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-2-2.amc
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-2-3.amc
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-2-4.amc
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/grid-3-3.amc
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/macro.amc
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/amc/periodic-torus.amc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.224006 dune-grid-2.9.0rc1/doc/grids/dgf/
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/basicunitcube-2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/cube-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/cube-testgrid-2-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/cube-testgrid-2-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/cube_grid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/distorted-cube-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/example-projection.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid10.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid10a.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid10b.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid11.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid12.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid1c.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid1gen.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid1s.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid2a.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid2b.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid2c.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid2e.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid5.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid6.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid7.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid9.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/grid2Y.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/grid3A.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/grid3Y.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/helix-deprecated.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/helix.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/octahedron.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-1-1.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-1-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-1-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-2-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    29483 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-2-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   733321 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-3-3-large.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     7800 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-3-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/test1d-vertex.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/test1d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/test2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/test2d_offset.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/test2ug.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/test3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/torus-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/torus-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/dgf/unstr_cube.dgf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.228006 dune-grid-2.9.0rc1/doc/grids/gmsh/
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/circle.geo
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/circle1storder.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/circle1storder.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/circle2ndorder.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/circle2ndorder.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/curved2d.geo
--rw-r--r--   0 runner    (1001) docker     (121)    22999 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/curved2d.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/curved2d.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/hybrid-testgrid-2d.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/hybrid-testgrid-2d.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)     3850 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/hybrid-testgrid-3d.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/hybrid-testgrid-3d.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/oned-testgrid.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/oned-testgrid.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid.geo
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)     9328 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid1storder.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid1storder.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)    27015 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid2ndorder.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid2ndorder.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid4.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid4.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)    36268 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/sphere.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/sphere.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope.geo
--rw-r--r--   0 runner    (1001) docker     (121)    11575 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)    11575 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope1storder.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope1storder.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)    34814 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope2ndorder.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/telescope2ndorder.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/twotets.geo
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/twotets.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/twotets.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/unitcube.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/unitcube.msh.license
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/unitsquare_quads_2x2.msh
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gmsh/unitsquare_quads_2x2.msh.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.228006 dune-grid-2.9.0rc1/doc/grids/gridfactory/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gridfactory/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13286 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gridfactory/hybridtestgrids.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9467 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/gridfactory/testgrids.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.232006 dune-grid-2.9.0rc1/doc/grids/starcd/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/star.cel
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/star.cel.license
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/star.vrt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/star.vrt.license
--rw-r--r--   0 runner    (1001) docker     (121)    95230 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/tets.cel
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/tets.cel.license
--rw-r--r--   0 runner    (1001) docker     (121)    11840 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/tets.vrt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/tets.vrt.license
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withprism.cel
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withprism.cel.license
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withprism.vrt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withprism.vrt.license
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withpyramid.cel
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withpyramid.cel.license
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withpyramid.vrt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/grids/starcd/withpyramid.vrt.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.232006 dune-grid-2.9.0rc1/doc/recipes/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/recipes/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/recipes/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5265 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/recipes/recipe-integration.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3509 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/doc/recipes/recipe-iterate-over-grid.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.232006 dune-grid-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.232006 dune-grid-2.9.0rc1/dune/grid/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.236006 dune-grid-2.9.0rc1/dune/grid/albertagrid/
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    22700 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/agrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18669 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/albertagrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/albertaheader.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/albertareader.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4607 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/algebra.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/backuprestore.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/coordcache.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/dgfparser.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5542 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/dgfparser.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.236006 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/
--rw-r--r--   0 runner    (1001) docker     (121)    10520 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_tetrahedron.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_tetrahedron.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)    10672 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_triangle.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_triangle.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)     7871 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/dofadmin.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9825 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/dofvector.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13460 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/elementinfo.cc
--rw-r--r--   0 runner    (1001) docker     (121)    24107 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/elementinfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9795 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/entity.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11993 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/entityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/geometry.cc
--rw-r--r--   0 runner    (1001) docker     (121)    17310 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/geometrycache.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5576 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/geometryreference.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19287 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/gridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/gridfamily.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14681 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4727 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/hierarchiciterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/indexsets.cc
--rw-r--r--   0 runner    (1001) docker     (121)    18544 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/indexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/indexstack.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13052 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/intersection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5453 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/leafiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5518 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/level.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/leveliterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/macrodata.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12989 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/macrodata.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/macroelement.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/meshpointer.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13157 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/meshpointer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15785 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/misc.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/persistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7077 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/projection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9305 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/refinement.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/structuredgridfactory.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.236006 dune-grid-2.9.0rc1/dune/grid/albertagrid/test/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7086 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/test/test-alberta3d-refine.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/transformation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16449 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/treeiterator.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2528 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/undefAllMacros.pl
--rw-r--r--   0 runner    (1001) docker     (121)     7803 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/undefine-2.0.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16218 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid/undefine-3.0.hh
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/albertagrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.240006 dune-grid-2.9.0rc1/dune/grid/common/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/adaptcallback.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3927 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/backuprestore.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8214 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/boundaryprojection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/boundarysegment.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7581 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17583 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/cube-to-tet-6.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/cube-to-tet-6.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    41310 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/cube-to-tet-6.svg
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/cube-to-tet-6.svg.license
--rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/datahandleif.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12541 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/defaultgridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23607 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4914 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/entityiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/entityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21139 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    41885 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/grid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/gridenums.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14965 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/gridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7158 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/gridinfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12673 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/idlocalref.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/idlocalref.eps.license
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/idlocalref.fig
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/idlocalref.fig.license
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/idlocalref.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/idlocalref.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    19752 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/indexidset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19467 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8969 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10005 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/islocalref.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/islocalref.eps.license
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/islocalref.fig
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/islocalref.fig.license
--rw-r--r--   0 runner    (1001) docker     (121)     7634 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/islocalref.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/islocalref.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     7814 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/mapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15650 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/mcmgmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11182 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/partitionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    39197 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/rangegenerators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8245 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/scsgmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11636 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/sizecache.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.240006 dune-grid-2.9.0rc1/dune/grid/common/test/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12303 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/test/mcmgmappertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/common/test/scsgmappertest.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.240006 dune-grid-2.9.0rc1/dune/grid/geometrygrid/
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/backuprestore.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5824 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/cachedcoordfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4261 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10246 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/coordfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/coordfunctioncaller.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6621 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/cornerstorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28006 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/entityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7138 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21393 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/grid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/gridfamily.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8104 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13400 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/helix.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/helix.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/hostcorners.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/identity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/idset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3263 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/indexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/intersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid/persistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5990 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/geometrygrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.244006 dune-grid-2.9.0rc1/dune/grid/identitygrid/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12483 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridentity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridentityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridhierarchiciterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8986 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridindexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3900 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridintersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11200 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridintersections.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridleafiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridleveliterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15370 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/identitygrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.244006 dune-grid-2.9.0rc1/dune/grid/io/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.244006 dune-grid-2.9.0rc1/dune/grid/io/file/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.244006 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.248006 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/basic.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/basic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4535 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundarydom.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7515 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundarydom.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundaryseg.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundaryseg.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/cube.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/cube.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/dim.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/dim.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/general.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/general.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/gridparameter.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/gridparameter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5795 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/interval.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4166 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/interval.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/periodicfacetrans.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/periodicfacetrans.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/polygon.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/polyhedron.hh
--rw-r--r--   0 runner    (1001) docker     (121)    28407 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/projection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7555 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/projection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplex.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplex.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplexgeneration.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplexgeneration.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/vertex.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/vertex.hh
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfexception.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7010 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfgeogrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5317 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfgridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3004 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfidentitygrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6064 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfoned.hh
--rw-r--r--   0 runner    (1001) docker     (121)    33451 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfparser.cc
--rw-r--r--   0 runner    (1001) docker     (121)    32944 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfparser.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfug.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6728 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfug.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15882 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15215 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfyasp.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/entitykey.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5249 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/entitykey_inline.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26926 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/gridptr.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/macrogrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/parser.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.252006 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/
--rw-r--r--   0 runner    (1001) docker     (121)   202441 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    79520 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/Orb_cut.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/Orb_cut.png.license
--rw-r--r--   0 runner    (1001) docker     (121)   288273 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/checkdgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/example-projection.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/example-projection.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    63735 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10a.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10a.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    32218 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10b.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10b.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    14008 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10c.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10c.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    25735 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10s.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10s.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    30035 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid11a.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid11a.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    42853 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid11b.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid11b.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    26806 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid12_1.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid12_1.png.license
--rw-r--r--   0 runner    (1001) docker     (121)   186095 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid12_2.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid12_2.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1c.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1c.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1cs.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1cs.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1gen.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1gen.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1genangle.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1genangle.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1s.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1s.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     5575 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2a.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2a.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     9665 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2b.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2b.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    20049 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2c.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2c.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    20088 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2d.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2d.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    90055 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2e.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2e.png.license
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid5c.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid5c.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     3801 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid5s.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid5s.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    44861 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid6c.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid6c.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    50075 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid6s.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid6s.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    76909 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7.png.license
--rw-r--r--   0 runner    (1001) docker     (121)   144373 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7angle.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7angle.png.license
--rw-r--r--   0 runner    (1001) docker     (121)   289461 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7area.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7area.png.license
--rw-r--r--   0 runner    (1001) docker     (121)   122356 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/pmdc.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/pmdc.png.license
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/test-dgf-alberta.cc
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/test-dgf-oned.cc
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/test-dgf-ug.cc
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/test-dgf-yasp.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.252006 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/dgf2dgf.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/gmsh2dgf.cc
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser.hh
--rw-r--r--   0 runner    (1001) docker     (121)    45033 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/gmshreader.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10155 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/gmshwriter.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.252006 dune-grid-2.9.0rc1/dune/grid/io/file/gnuplot/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/gnuplot/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/gnuplot/gnuplot.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/gnuplot.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7861 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/printgrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6959 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/starcdreader.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.256006 dune-grid-2.9.0rc1/dune/grid/io/file/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/checkvtkfile.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/conformvolumevtktest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10254 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/gmshtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/gnuplottest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/nonconformboundaryvtktest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/printgridtest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/starcdreadertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6959 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/subsamplingvtktest.cc
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/test-linking.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/vtksequencetest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/test/vtktest.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.256006 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/b64enc.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17394 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/basicwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/boundaryiterators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/boundarywriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10446 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/common.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/corner.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/corneriterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    21298 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/dataarraywriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10029 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/function.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12708 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/functionwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/pointiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/pvtuwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4694 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/skeletonfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/streams.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13506 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/subsamplingvtkwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/volumeiterators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/volumewriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtksequencewriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6129 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtksequencewriterbase.hh
--rw-r--r--   0 runner    (1001) docker     (121)    55573 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtkwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13161 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtuwriter.hh
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/io/file/vtk.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/modules.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.256006 dune-grid-2.9.0rc1/dune/grid/onedgrid/
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/nulliteratorfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/nulliteratorfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17440 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)    16518 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridentity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridentityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6042 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2809 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridhieriterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10016 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridindexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridintersectioniterators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16195 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridintersections.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridleafiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridleveliterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridlist.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12975 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridviews.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13422 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/onedgrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.260006 dune-grid-2.9.0rc1/dune/grid/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4195 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/basicunitcube.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/check-albertareader.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkadaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12243 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkcomcorrectness.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19064 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkcommunicate.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkentitylifetime.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkentityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12267 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkgeometryinfather.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkgridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkidset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19895 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26565 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkintersectionit.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkintersectionlifetime.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkiterators.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkjacobians.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15840 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checkpartition.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/checktwists.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/functions.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/geometrygrid-coordfunction-copyconstructor.cc
--rw-r--r--   0 runner    (1001) docker     (121)    36913 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/gridcheck.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/issue-53-uggrid-intersections.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15368 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/staticcheck.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6639 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-alberta.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8818 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-geogrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-gridinfo.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-hierarchicsearch.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-identitygrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5950 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-loadbalancing.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-mcmg-geogrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6645 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-oned.cc
--rw-r--r--   0 runner    (1001) docker     (121)    32340 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-parallel-ug.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14818 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/test-ug.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/testiteratorranges.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.260006 dune-grid-2.9.0rc1/dune/grid/test/yasp/
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistant.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistantoffset.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-backuprestore-tensor.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-constructor.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6536 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-entityshifttable.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-partitioner.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-tensorgridfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-yaspfactory-1d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-yaspfactory-2d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-yaspfactory-3d.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7628 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.264006 dune-grid-2.9.0rc1/dune/grid/uggrid/
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6279 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/boundaryextractor.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/boundaryextractor.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22654 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/ug_undefs.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23946 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14280 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridentity.cc
--rw-r--r--   0 runner    (1001) docker     (121)    18882 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridentity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridentityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24336 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10129 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6289 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridgeometry.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7225 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridhieriterator.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridhieriterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14296 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridindexsets.cc
--rw-r--r--   0 runner    (1001) docker     (121)    25683 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridindexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridintersectioniterators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    27353 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridintersections.cc
--rw-r--r--   0 runner    (1001) docker     (121)    16192 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridintersections.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6630 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridleafiterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4114 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridleveliterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridlocalgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10604 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridrenumberer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14166 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uggridviews.hh
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/ugincludes.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4945 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/uglbgatherscatter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/ugmessagebuffer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    39652 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/ugwrapper.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2085 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid/undefAllMacros.pl
--rw-r--r--   0 runner    (1001) docker     (121)    28313 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/uggrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.264006 dune-grid-2.9.0rc1/dune/grid/utility/
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/entitycommhelper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19729 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/globalindexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6626 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/gridinfo-gmsh-main.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10076 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/gridinfo.hh
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/gridtype.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6034 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/hierarchicsearch.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/hostgridaccess.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/multiindex.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9577 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/parmetisgridpartitioner.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7515 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainerinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8790 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainermap.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainervector.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainerwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9607 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/structuredgridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13823 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/tensorgridfactory.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.264006 dune-grid-2.9.0rc1/dune/grid/utility/test/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/test/globalindexsettest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/test/persistentcontainertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9745 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/test/structuredgridfactorytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/test/tensorgridfactorytest.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12892 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/test/vertexordertest.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/utility/vertexorderfactory.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/dune/grid/yaspgrid/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11451 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/backuprestore.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12221 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/coordinates.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16417 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.eps.license
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.fig
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.fig.license
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     7489 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/partitioning.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5332 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/structuredyaspgridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16927 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.eps
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.eps.license
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.fig
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.fig.license
--rw-r--r--   0 runner    (1001) docker     (121)     5414 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.png
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    15187 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/torus.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29220 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridentity.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridentityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridgeometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridhierarchiciterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgrididset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridindexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11096 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridintersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridintersectioniterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridleveliterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridpersistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29339 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid/ygrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)    81831 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/grid/yaspgrid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/dune/python/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/dune/python/grid/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/commops.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10011 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/enums.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11932 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/factory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15899 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/function.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13027 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20090 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)    18479 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/hierarchical.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8497 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/idset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14058 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3853 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/intersection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/localview.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19613 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/mapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15504 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/numpy.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6554 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/numpycommdatahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/object.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/persistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/pygridfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17507 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/range.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6050 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/simplegridfunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4682 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/grid/vtk.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/dune/python/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/backrest1.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/backrest2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3818 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/test-ug.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/test_gf1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/test_gf2.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/test_indexset.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune/python/test/ugfromfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune-grid.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/dune.module
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/lib/dunegridam2cmake.lib
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.268006 dune-grid-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/python/dune/grid/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3217 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/_grid.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15324 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/_grids.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/datahandle.py
--rw-r--r--   0 runner    (1001) docker     (121)    15474 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/grid_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/python/dune/grid/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/tutorial/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/tutorial/circle1storder.msh
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/tutorial/example.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/python/dune/grid/tutorial/test2d_offset.dgf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/python/dune_grid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-21 08:16:55.000000 dune-grid-2.9.0rc1/python/dune_grid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25294 2022-10-21 08:16:55.000000 dune-grid-2.9.0rc1/python/dune_grid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:16:55.000000 dune-grid-2.9.0rc1/python/dune_grid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-21 08:16:55.000000 dune-grid-2.9.0rc1/python/dune_grid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:16:55.000000 dune-grid-2.9.0rc1/python/dune_grid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/src/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:16:55.272006 dune-grid-2.9.0rc1/src/gridinfo-gmsh/
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/src/gridinfo-gmsh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/src/gridinfo-gmsh/gridinfo-gmsh-alberta-2d.cc
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/src/gridinfo-gmsh/gridinfo-gmsh-alberta-3d.cc
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/src/gridinfo-gmsh/gridinfo-gmsh-ug-2d.cc
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-10-21 08:16:54.000000 dune-grid-2.9.0rc1/src/gridinfo-gmsh/gridinfo-gmsh-ug-3d.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    13630 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20951 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)    20951 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.855694 dune-grid-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.859694 dune-grid-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/cmake/modules/AddAlbertaFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/cmake/modules/DuneGridMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/cmake/modules/FindAlberta.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/cmake/modules/GridType.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/cmake/modules/UseUG.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.859694 dune-grid-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.859694 dune-grid-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2972 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/doxygen/Doxydep
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/doxygen/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/doxygen/modules.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.859694 dune-grid-2.9.dev20220529/doc/grids/
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.859694 dune-grid-2.9.dev20220529/doc/grids/amc/
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-1-1.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-1-2.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-1-3.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-2-2.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-2-3.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-2-4.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/grid-3-3.amc
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/macro.amc
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/amc/periodic-torus.amc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.863694 dune-grid-2.9.dev20220529/doc/grids/dgf/
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/basicunitcube-2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/cube-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/cube-testgrid-2-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/cube-testgrid-2-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/cube_grid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/distorted-cube-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/example-projection.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid10.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid10a.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid10b.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid11.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid12.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid1c.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid1gen.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid1s.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid2a.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid2b.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid2c.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid2e.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid5.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid6.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid7.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid9.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/grid2Y.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/grid3A.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/grid3Y.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/helix-deprecated.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/helix.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/octahedron.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-1-1.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-1-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-1-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     2796 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-2-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    29310 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-2-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   733148 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-3-3-large.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     7627 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-3-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/test1d-vertex.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/test1d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/test2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/test2d_offset.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/test2ug.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/test3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/torus-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/torus-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/dgf/unstr_cube.dgf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.867694 dune-grid-2.9.dev20220529/doc/grids/gmsh/
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/circle.geo
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/circle1storder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/circle2ndorder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/curved2d.geo
+-rw-r--r--   0 runner    (1001) docker     (121)    22999 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/curved2d.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/hybrid-testgrid-2d.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     3850 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/hybrid-testgrid-3d.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/oned-testgrid.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid.geo
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     9328 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid1storder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    27015 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid2ndorder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    36268 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/sphere.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope.geo
+-rw-r--r--   0 runner    (1001) docker     (121)    11575 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    11575 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope1storder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    34814 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope2ndorder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/twotets.geo
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/twotets.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/unitcube.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gmsh/unitsquare_quads_2x2.msh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.867694 dune-grid-2.9.dev20220529/doc/grids/gridfactory/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gridfactory/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13111 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gridfactory/hybridtestgrids.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9292 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/gridfactory/testgrids.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.867694 dune-grid-2.9.dev20220529/doc/grids/starcd/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/star.cel
+-rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/star.vrt
+-rw-r--r--   0 runner    (1001) docker     (121)    95230 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/tets.cel
+-rw-r--r--   0 runner    (1001) docker     (121)    11840 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/tets.vrt
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/withprism.cel
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/withprism.vrt
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/withpyramid.cel
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/grids/starcd/withpyramid.vrt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.867694 dune-grid-2.9.dev20220529/doc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/recipes/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/recipes/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5093 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/recipes/recipe-integration.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/doc/recipes/recipe-iterate-over-grid.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.867694 dune-grid-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.867694 dune-grid-2.9.dev20220529/dune/grid/
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.871694 dune-grid-2.9.dev20220529/dune/grid/albertagrid/
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    22403 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/agrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18494 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/albertagrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/albertaheader.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/albertareader.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/algebra.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/backuprestore.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/coordcache.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/dgfparser.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5367 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/dgfparser.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.871694 dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    10520 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/alberta_tetrahedron.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    10672 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/alberta_triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/dofadmin.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9650 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/dofvector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13285 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/elementinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    23932 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/elementinfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9620 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/entity.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11818 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/entityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6873 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    16067 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometrycache.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3290 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometryreference.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19112 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/gridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/gridfamily.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13940 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4552 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/hierarchiciterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/indexsets.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    18369 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/indexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5830 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/indexstack.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12877 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/leafiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5343 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/level.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/leveliterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11053 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/macrodata.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12814 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/macrodata.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/macroelement.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/meshpointer.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12982 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/meshpointer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15610 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/misc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/persistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6902 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/projection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9130 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/refinement.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7983 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/structuredgridfactory.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.871694 dune-grid-2.9.dev20220529/dune/grid/albertagrid/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6911 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/test/test-alberta3d-refine.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/transformation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16274 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/treeiterator.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2354 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/undefAllMacros.pl
+-rw-r--r--   0 runner    (1001) docker     (121)     7628 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/undefine-2.0.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16043 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid/undefine-3.0.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/albertagrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.875694 dune-grid-2.9.dev20220529/dune/grid/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3650 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/adaptcallback.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3752 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/backuprestore.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8039 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/boundaryprojection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3953 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/boundarysegment.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7406 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17583 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/cube-to-tet-6.png
+-rw-r--r--   0 runner    (1001) docker     (121)    41310 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/cube-to-tet-6.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     8007 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/datahandleif.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11784 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/defaultgridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23432 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4739 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/entityiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/entityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15553 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    40913 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/grid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4877 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/gridenums.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14790 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/gridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6983 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/gridinfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11730 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/idlocalref.eps
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/idlocalref.fig
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/idlocalref.png
+-rw-r--r--   0 runner    (1001) docker     (121)    19577 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/indexidset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19292 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10005 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/islocalref.eps
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/islocalref.fig
+-rw-r--r--   0 runner    (1001) docker     (121)     7634 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/islocalref.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7639 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/mapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15475 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/mcmgmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11007 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/partitionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    39022 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/rangegenerators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8070 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/scsgmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11461 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/sizecache.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.875694 dune-grid-2.9.dev20220529/dune/grid/common/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12128 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/test/mcmgmappertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/common/test/scsgmappertest.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.879694 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/backuprestore.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/cachedcoordfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10071 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/coordfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/coordfunctioncaller.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6446 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/cornerstorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27831 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/entityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21684 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/grid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4849 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/gridfamily.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7567 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13400 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/helix.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/hostcorners.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/identity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/idset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/indexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6015 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/intersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13767 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid/persistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5815 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/geometrygrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.879694 dune-grid-2.9.dev20220529/dune/grid/identitygrid/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12308 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridentity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridentityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3643 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridhierarchiciterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8811 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridindexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridintersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11025 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridintersections.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridleafiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridleveliterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15206 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/identitygrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.879694 dune-grid-2.9.dev20220529/dune/grid/io/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.879694 dune-grid-2.9.dev20220529/dune/grid/io/file/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.879694 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.883694 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3002 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/basic.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/basic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundarydom.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundarydom.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4558 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundaryseg.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundaryseg.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/cube.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/cube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/dim.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/dim.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/general.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/general.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/gridparameter.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/gridparameter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5620 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/interval.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/interval.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/periodicfacetrans.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/periodicfacetrans.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/polygon.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/polyhedron.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    28232 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/projection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7380 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/projection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7653 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplex.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplexgeneration.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplexgeneration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/vertex.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/vertex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfexception.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6835 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfgeogrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfgridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2829 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfidentitygrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5889 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfoned.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    33276 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfparser.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    32769 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfparser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3428 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfug.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6553 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfug.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15707 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15040 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfyasp.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/entitykey.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5074 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/entitykey_inline.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26751 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/gridptr.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/macrogrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/parser.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.887694 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/
+-rw-r--r--   0 runner    (1001) docker     (121)   202441 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    79520 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/Orb_cut.png
+-rw-r--r--   0 runner    (1001) docker     (121)   288273 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/checkdgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5670 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/example-projection.png
+-rw-r--r--   0 runner    (1001) docker     (121)    63735 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10.png
+-rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10a.png
+-rw-r--r--   0 runner    (1001) docker     (121)    32218 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10b.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14008 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10c.png
+-rw-r--r--   0 runner    (1001) docker     (121)    25735 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10s.png
+-rw-r--r--   0 runner    (1001) docker     (121)    30035 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid11a.png
+-rw-r--r--   0 runner    (1001) docker     (121)    42853 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid11b.png
+-rw-r--r--   0 runner    (1001) docker     (121)    26806 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid12_1.png
+-rw-r--r--   0 runner    (1001) docker     (121)   186095 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid12_2.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1c.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1cs.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1gen.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1genangle.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1s.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5575 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2a.png
+-rw-r--r--   0 runner    (1001) docker     (121)     9665 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2b.png
+-rw-r--r--   0 runner    (1001) docker     (121)    20049 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2c.png
+-rw-r--r--   0 runner    (1001) docker     (121)    20088 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2d.png
+-rw-r--r--   0 runner    (1001) docker     (121)    90055 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2e.png
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid5c.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3801 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid5s.png
+-rw-r--r--   0 runner    (1001) docker     (121)    44861 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid6c.png
+-rw-r--r--   0 runner    (1001) docker     (121)    50075 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid6s.png
+-rw-r--r--   0 runner    (1001) docker     (121)    76909 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid7.png
+-rw-r--r--   0 runner    (1001) docker     (121)   144373 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid7angle.png
+-rw-r--r--   0 runner    (1001) docker     (121)   289461 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid7area.png
+-rw-r--r--   0 runner    (1001) docker     (121)   122356 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/pmdc.png
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/test-dgf-alberta.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/test-dgf-oned.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/test-dgf-ug.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/test-dgf-yasp.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.887694 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/dgf2dgf.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/gmsh2dgf.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    44858 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/gmshreader.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9980 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/gmshwriter.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.887694 dune-grid-2.9.dev20220529/dune/grid/io/file/gnuplot/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/gnuplot/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/gnuplot/gnuplot.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/gnuplot.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7686 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/printgrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6784 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/starcdreader.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.887694 dune-grid-2.9.dev20220529/dune/grid/io/file/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/checkvtkfile.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/conformvolumevtktest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10079 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/gmshtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/gnuplottest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/nonconformboundaryvtktest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/printgridtest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/starcdreadertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6784 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/subsamplingvtktest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/test-linking.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/vtksequencetest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/test/vtktest.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.891694 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/b64enc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17219 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/basicwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6298 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/boundaryiterators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/boundarywriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/common.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/corner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/corneriterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    21123 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/dataarraywriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9854 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/function.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12533 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/functionwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4306 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/pointiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7303 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/pvtuwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/skeletonfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/streams.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13331 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/subsamplingvtkwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/volumeiterators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/volumewriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtksequencewriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5954 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtksequencewriterbase.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    55398 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtkwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12986 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtuwriter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/io/file/vtk.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/modules.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.891694 dune-grid-2.9.dev20220529/dune/grid/onedgrid/
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/nulliteratorfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/nulliteratorfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17265 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    16343 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridentity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridentityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5867 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridhieriterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9841 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridindexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3193 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridintersectioniterators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16020 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridintersections.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridleafiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridleveliterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3736 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridlist.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12234 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridviews.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13267 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/onedgrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.895694 dune-grid-2.9.dev20220529/dune/grid/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/basicunitcube.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/check-albertareader.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9289 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkadaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12068 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkcomcorrectness.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18889 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkcommunicate.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4531 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkentitylifetime.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5681 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkentityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12092 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkgeometryinfather.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkgridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkidset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19720 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26390 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkintersectionit.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkintersectionlifetime.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3563 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkiterators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkjacobians.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15665 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checkpartition.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/checktwists.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/functions.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/geometrygrid-coordfunction-copyconstructor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    36738 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/gridcheck.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/issue-53-uggrid-intersections.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15160 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/staticcheck.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6464 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-alberta.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8643 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-geogrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-gridinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-hierarchicsearch.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-identitygrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5775 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-loadbalancing.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-mcmg-geogrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-oned.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    32128 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-parallel-ug.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11217 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/test-ug.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/testiteratorranges.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.895694 dune-grid-2.9.dev20220529/dune/grid/test/yasp/
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistant.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistantoffset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-backuprestore-tensor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-constructor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6361 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-entityshifttable.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-tensorgridfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-yaspfactory-1d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-yaspfactory-2d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-yaspfactory-3d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7453 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.899695 dune-grid-2.9.dev20220529/dune/grid/uggrid/
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6104 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/boundaryextractor.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/boundaryextractor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22479 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/ug_undefs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23781 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14105 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridentity.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    17029 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridentity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridentityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24161 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9964 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6114 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridgeometry.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7050 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridhieriterator.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridhieriterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14121 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridindexsets.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    25508 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridindexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4000 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridintersectioniterators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27178 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridintersections.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    16017 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridintersections.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridleafiterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridleveliterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridlocalgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10429 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridrenumberer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13317 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridviews.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/ugincludes.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/uglbgatherscatter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/ugmessagebuffer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    39371 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/ugwrapper.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1911 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid/undefAllMacros.pl
+-rw-r--r--   0 runner    (1001) docker     (121)    28220 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/uggrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.899695 dune-grid-2.9.dev20220529/dune/grid/utility/
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/entitycommhelper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19585 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/globalindexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6451 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/gridinfo-gmsh-main.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9901 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/gridinfo.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/gridtype.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/hierarchicsearch.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5213 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/hostgridaccess.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/multiindex.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/parmetisgridpartitioner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainerinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8610 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainermap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4543 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainervector.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainerwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9432 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/structuredgridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13678 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/tensorgridfactory.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.899695 dune-grid-2.9.dev20220529/dune/grid/utility/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4949 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/test/globalindexsettest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/test/persistentcontainertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/test/structuredgridfactorytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/test/tensorgridfactorytest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12717 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/test/vertexordertest.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/utility/vertexorderfactory.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11252 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/backuprestore.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12046 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/coordinates.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16417 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/grid.eps
+-rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/grid.fig
+-rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/grid.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3857 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/partitioning.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5157 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/structuredyaspgridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16927 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/subgrid.eps
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/subgrid.fig
+-rw-r--r--   0 runner    (1001) docker     (121)     5414 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/subgrid.png
+-rw-r--r--   0 runner    (1001) docker     (121)    15028 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/torus.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    29015 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridentity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridentityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridgeometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridhierarchiciterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgrididset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridindexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10921 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridintersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridintersectioniterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridleveliterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3798 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridpersistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    29164 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid/ygrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    81370 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/grid/yaspgrid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/dune/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/dune/python/grid/
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/commops.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9836 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/enums.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11757 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/factory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15724 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/function.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12843 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19911 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18304 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/hierarchical.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8322 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/idset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13883 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/intersection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/localview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19438 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/mapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13933 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/numpy.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6379 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/numpycommdatahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/object.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/persistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/pygridfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17332 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/range.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5875 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/simplegridfunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/grid/vtk.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/dune/python/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/backrest1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/backrest2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/test-ug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/test_gf1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/test_gf2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/test_indexset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune/python/test/ugfromfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune-grid.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/dune.module
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/lib/dunegridam2cmake.lib
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.903694 dune-grid-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/python/dune/grid/
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/_grid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14223 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/_grids.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/datahandle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14989 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/grid_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/python/dune/grid/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/tutorial/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/tutorial/circle1storder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/tutorial/example.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune/grid/tutorial/test2d_offset.dgf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/python/dune_grid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune_grid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    21580 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune_grid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/python/dune_grid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/src/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:33.907694 dune-grid-2.9.dev20220529/src/gridinfo-gmsh/
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/src/gridinfo-gmsh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/src/gridinfo-gmsh/gridinfo-gmsh-alberta-2d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/src/gridinfo-gmsh/gridinfo-gmsh-alberta-3d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/src/gridinfo-gmsh/gridinfo-gmsh-ug-2d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-29 21:03:33.000000 dune-grid-2.9.dev20220529/src/gridinfo-gmsh/gridinfo-gmsh-ug-3d.cc
```

### Comparing `dune-grid-2.9.0rc1/.gitlab-ci.yml` & `dune-grid-2.9.dev20220529/.gitlab-ci.yml`

 * *Files 17% similar despite different names*

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
   - . /duneci/bin/duneci-init-job
   - duneci-install-module https://gitlab.dune-project.org/core/dune-common.git
   - duneci-install-module https://gitlab.dune-project.org/core/dune-geometry.git
   - duneci-install-module https://gitlab.dune-project.org/staging/dune-uggrid.git
 
@@ -51,17 +48,7 @@
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

### Comparing `dune-grid-2.9.0rc1/CHANGELOG.md` & `dune-grid-2.9.dev20220529/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,9 @@
-<!--
-SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
--->
-
 # Master (will become release 2.9)
 
-- The `Geometry` interface was extended by methods `jacobian(local)` and `jacobianInverse(local)`
-  and corresponding typedefs `Jacobian` and `JacobianInverse`. All grid implementations need to
-  provide the new interface. For transition, the methods and typedefs are default-implemented
-  in the `Dune::Geometry` interface class which is used for all grid geometries.
-
 - The `Geometry::integrationElement` now needs to return the type `Volume`
   instead of `ctype`. Note that this may be different from `ctype` if the grid
   supports typed dimensions. In such a case, `ctype` is a length, and not
   appropriate for a volume quantity.
 
 - The `FindAlberta.cmake` module only searches for world dimension libraries up to dim 3. This
   can be increased by setting the CMake variable `ALBERTA_MAX_WORLD_DIM`
@@ -27,28 +17,21 @@
 
 ## Deprecations and removals
 
 - Support for PSurface has been removed.
 
 - Support for AmiraMesh has been removed.
 
-- Following the deprecation of `CollectiveCommunication` in dune-common, grids define
-  the type `Communication`. The type `CollectiveCommunication` is deprecated and
-  will be removed after Dune 2.9.
-
 - The CMake function `add_dune_ug_flags` is deprecated. It should not be used since
   all flags are already set automatically. Also the package flags for the UG grid are
   not registered any more.
 
 - The `dune-uggrid` module does not set the preprocessor flag `HAVE_UG` anymore.
   Use `HAVE_DUNE_UGGRID` instead.
 
-- The `YLoadBalance` interface is deprecated, as well the
-  implementations. Users should switch to `Yasp::Partitioning`.
-
 # Release 2.8
 
 - Specialization of `StructuredGridFactory` for `AlbertaGrid` is added to address the special
   numbering requirements of that grid.
 
 - Return type of `GridFactory::createGrid()` changed to `std::unique_ptr`. While still the
   replacement type `ToUniquePtr` from dune-common works, it is marked deprecated and the std
```

### Comparing `dune-grid-2.9.0rc1/CMakeLists.txt` & `dune-grid-2.9.dev20220529/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 cmake_minimum_required(VERSION 3.13)
 project("dune-grid" C CXX)
 
 if(NOT (dune-common_DIR OR dune-common_ROOT OR
         "${CMAKE_PREFIX_PATH}" MATCHES ".*dune-common.*"))
     string(REPLACE  ${PROJECT_NAME} dune-common dune-common_DIR
       ${PROJECT_BINARY_DIR})
```

### Comparing `dune-grid-2.9.0rc1/COPYING` & `dune-grid-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/INSTALL` & `dune-grid-2.9.dev20220529/INSTALL`

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

### Comparing `dune-grid-2.9.0rc1/LICENSE.md` & `dune-grid-2.9.dev20220529/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/PKG-INFO` & `dune-grid-2.9.dev20220529/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-grid
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: module providing main interfaces for setting and traversing grids
 Home-page: https://gitlab.dune-project.org/core/dune-grid
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
         
         
-        git-d29ed3fdccc0087bfba94d907cca3abd85b55cf3
+        git-ce5efe9e428f6c22bc9e8484e45c8365114ee95e
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-grid-2.9.0rc1/README.md` & `dune-grid-2.9.dev20220529/README.md`

 * *Files 12% similar despite different names*

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
 
 
-git-d29ed3fdccc0087bfba94d907cca3abd85b55cf3
+git-ce5efe9e428f6c22bc9e8484e45c8365114ee95e
```

### Comparing `dune-grid-2.9.0rc1/cmake/modules/AddAlbertaFlags.cmake` & `dune-grid-2.9.dev20220529/cmake/modules/AddAlbertaFlags.cmake`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Module providing convenience methods for compile binaries with Alberta support.
 #
 # .. cmake_function:: add_dune_alberta_flags
 #
 #    .. cmake_param:: targets
 #       :single:
 #       :required:
```

### Comparing `dune-grid-2.9.0rc1/cmake/modules/DuneGridMacros.cmake` & `dune-grid-2.9.dev20220529/cmake/modules/DuneGridMacros.cmake`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # .. cmake_module::
 #
 #    This modules content is executed whenever a module required or suggests dune-grid!
 #
 
 include(CheckFunctionExists)
 check_function_exists(mkstemp HAVE_MKSTEMP)
```

### Comparing `dune-grid-2.9.0rc1/cmake/modules/FindAlberta.cmake` & `dune-grid-2.9.dev20220529/cmake/modules/FindAlberta.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 #[=======================================================================[.rst:
 FindAlberta
 -----------
 
 Find Alberta, an Adaptive multiLevel finite element toolbox using Bisectioning
 refinement and Error control by Residual Techniques for scientific Applications.
 (see https://gitlab.mathematik.uni-stuttgart.de/ians-nmh/alberta/alberta3)
```

### Comparing `dune-grid-2.9.0rc1/cmake/modules/GridType.cmake` & `dune-grid-2.9.dev20220529/cmake/modules/GridType.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Implement the GRIDTYPE preprocessor magic
 #
 # .. cmake_function:: dune_define_gridtype
 #
 #    .. cmake_param:: output
 #       :single:
 #       :required:
```

### Comparing `dune-grid-2.9.0rc1/cmake/modules/UseUG.cmake` & `dune-grid-2.9.dev20220529/cmake/modules/UseUG.cmake`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # If dune-uggrid was found this module adds the dgf magic to config.h
 # and makes add_dune_ug_flags available.
 #
 
 # Add dgf magic to config.h and register flags
 if(dune-uggrid_FOUND)
   dune_define_gridtype(GRID_CONFIG_H_BOTTOM GRIDTYPE UGGRID
```

### Comparing `dune-grid-2.9.0rc1/config.h.cmake` & `dune-grid-2.9.dev20220529/config.h.cmake`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /* begin dune-grid
    put the definitions for config.h specific to
    your project here. Everything above will be
    overwritten
 */
 /* begin private */
 /* Name of package */
```

### Comparing `dune-grid-2.9.0rc1/doc/doxygen/Doxydep` & `dune-grid-2.9.dev20220529/doc/doxygen/Doxydep`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/perl -w
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 use strict;
 use English;
 use IO::Handle;
 
 # OPTIONS
 my $defaulttarget = "doxygen-tag";
```

### Comparing `dune-grid-2.9.0rc1/doc/doxygen/Doxylocal` & `dune-grid-2.9.dev20220529/doc/doxygen/Doxylocal`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 INPUT                 += @srcdir@/mainpage.txt \
                          @srcdir@/modules.txt \
                          @top_srcdir@/doc/recipes \
                          @top_srcdir@/doc/recipes/mainpage.txt \
                          @top_srcdir@/dune/grid/modules.txt \
                          @top_srcdir@/dune/grid/albertagrid \
                          @top_srcdir@/dune/grid/albertagrid.hh \
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/amc/grid-3-3.amc` & `dune-grid-2.9.dev20220529/doc/grids/amc/grid-3-3.amc`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 DIM:          3 
 DIM_OF_WORLD: 3
 
 number of vertices: 8
 number of elements: 6
 
 vertex coordinates:
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/amc/periodic-torus.amc` & `dune-grid-2.9.dev20220529/doc/grids/amc/periodic-torus.amc`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # Example macro triangulation for a mesh with periodic boundaries: a
 # topological torus.
 
 DIM: 2
 DIM_OF_WORLD: 2
 
 number of elements: 8
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/CMakeLists.txt` & `dune-grid-2.9.dev20220529/doc/grids/dgf/CMakeLists.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 set(GRIDS
   basicunitcube-2d.dgf
   cube-2.dgf
   cube_grid.dgf
   cube-testgrid-2-2.dgf
   cube-testgrid-2-3.dgf
   distorted-cube-3.dgf
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/cube_grid.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/cube_grid.dgf`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 vertex
 0 0 0  % vertex 0
 38 0 0  % vertex 1
 0 51.75 0  % vertex 2
 38 51.75 0  % vertex 3
 69 138 0  % vertex 4
 69 100 0  % vertex 5
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid10.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid10b.dgf`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 vertex 
+parameters 1
 firstindex 1
- 0   0  5   # 1
- 0   0  0   # 2
- 0 -10  0   # 3 
- 0 -10 10   # 4 
- 0  10 10   # 5 
- 0  10  5   # 6 
-
-30  10  0   # 7 
-30 -10  0   # 8 
-30 -10 10   # 9 
-30  10 10   # 10 
-
-25  10  0   # 11 
-25   0  0   # 12 
-25   0  5   # 13 
-25  10  5   # 14 
-
-0    0 10   # 15 
-
-30   0  0   # 16
-30   0  5   # 17
-30   0 10   # 18
-30  10  5   # 19
-30 -10  5   # 20
-
-25  10 10   # 21
-25   0 10   # 22
-25 -10 10   # 23
-25 -10  5   # 24 
-25 -10  0   # 25
+ 0   0  5   5   # 1
+ 0   0  0   0   # 2
+ 0 -10  0 -10   # 3 
+ 0 -10 10   0   # 4 
+ 0  10 10  20   # 5 
+ 0  10  5  15   # 6 
+
+30  10  0   40 # 7 
+30 -10  0   20 # 8 
+30 -10 10   30 # 9 
+30  10 10   50 # 10 
+
+25  10  0   35 # 11 
+25   0  0   25 # 12 
+25   0  5   30 # 13 
+25  10  5   40 # 14 
+
+0    0 10   10 # 15 
+
+30   0  0   30 # 16
+30   0  5   35 # 17
+30   0 10   40 # 18
+30  10  5   45 # 19
+30 -10  5   25 # 20
+
+25  10 10   45 # 21
+25   0 10   35 # 22
+25 -10 10   25 # 23
+25 -10  5   20 # 24 
+25 -10  0   15 # 25
 
-0  -10  5   # 26
+0  -10  5   -5 # 26
 #
 Cube
 map 0 1 3 2  4 5 7 6
 21 14 13 22  5  6  1 15 
 23 22 13 24  4 15  1 26 
 25 24 13 12  3 26  1  2 
 17 19 7 16  13 14 11 12 
@@ -64,9 +63,9 @@
 4   4 15 22 23
 4   23 9 18 22
 4   22 18 10 21
 # 
 boundarydomain
 default 3 
 #
-# examplegrid10.dgf
+# examplegrid10b.dgf
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid10a.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid10a.dgf`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 vertex 
 firstindex 1
  0   0  5   # 1
  0   0  0   # 2
  0 -10  0   # 3 
  0 -10 10   # 4 
  0  10 10   # 5
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid10b.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid10.dgf`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 vertex 
-parameters 1
 firstindex 1
- 0   0  5   5   # 1
- 0   0  0   0   # 2
- 0 -10  0 -10   # 3 
- 0 -10 10   0   # 4 
- 0  10 10  20   # 5 
- 0  10  5  15   # 6 
-
-30  10  0   40 # 7 
-30 -10  0   20 # 8 
-30 -10 10   30 # 9 
-30  10 10   50 # 10 
-
-25  10  0   35 # 11 
-25   0  0   25 # 12 
-25   0  5   30 # 13 
-25  10  5   40 # 14 
-
-0    0 10   10 # 15 
-
-30   0  0   30 # 16
-30   0  5   35 # 17
-30   0 10   40 # 18
-30  10  5   45 # 19
-30 -10  5   25 # 20
-
-25  10 10   45 # 21
-25   0 10   35 # 22
-25 -10 10   25 # 23
-25 -10  5   20 # 24 
-25 -10  0   15 # 25
+ 0   0  5   # 1
+ 0   0  0   # 2
+ 0 -10  0   # 3 
+ 0 -10 10   # 4 
+ 0  10 10   # 5 
+ 0  10  5   # 6 
+
+30  10  0   # 7 
+30 -10  0   # 8 
+30 -10 10   # 9 
+30  10 10   # 10 
+
+25  10  0   # 11 
+25   0  0   # 12 
+25   0  5   # 13 
+25  10  5   # 14 
+
+0    0 10   # 15 
+
+30   0  0   # 16
+30   0  5   # 17
+30   0 10   # 18
+30  10  5   # 19
+30 -10  5   # 20
+
+25  10 10   # 21
+25   0 10   # 22
+25 -10 10   # 23
+25 -10  5   # 24 
+25 -10  0   # 25
 
-0  -10  5   -5 # 26
+0  -10  5   # 26
 #
 Cube
 map 0 1 3 2  4 5 7 6
 21 14 13 22  5  6  1 15 
 23 22 13 24  4 15  1 26 
 25 24 13 12  3 26  1  2 
 17 19 7 16  13 14 11 12 
@@ -65,9 +62,9 @@
 4   4 15 22 23
 4   23 9 18 22
 4   22 18 10 21
 # 
 boundarydomain
 default 3 
 #
-# examplegrid10b.dgf
+# examplegrid10.dgf
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid1s.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid1s.dgf`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 Vertex        % the vertices of the grid
 -1   -1       % vertex 0
 -0.2 -1       % vertex 1
  1   -1       % vertex 2
  1    -0.6    % vertex 3
  1    1       % vertex 4
 -1    1       % vertex 5
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid2c.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid2b.dgf`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 Interval
 -1  -1       % first corner 
  1  1        % second corner
  4  4        % 4 cells in x and 4 in y direction
 #
 Vertex       % some additional points
  0.75 0.75   % inside the interval
  0.9 0.9     % also inside the interval
  1.25 1.25   % and one outside of the interval
 #
-Simplexgenerator
-min-angle 30    % quality enhancment
-max-area 0.01   % area restriction
-display 0       % show result using Triangle viewer
+Simplexgenerator  
+min-angle 30      % quality enhancment
+display 0         % show result using Triangle viewer
+% area restriction
 
 % to use Triangle from a certain path, uncomment this path line
-%path $HOME/bin      % path to Triangle
+%path $HOME/bin   % path to Triangle
 
 #
 BOUNDARYDOMAIN
-1  -1 -1    1 -1       % lower boundary has id 1
-2  -10 -10    10  10   % all others have id 2 (could use default keyword...)
+1   1 -1    1.25  1.25  % right boundary has id 1
+2  -1  1    1.25  1.25  % upper boundary has id 2
+3  -1 -1   -1  1        % left boundary has id 3
+4  -1 -1    1 -1        % lower boundary has id 4
 #BOUNDARYDOMAIN
-# examplegrid2c.dgf
+# examplegrid2b.dgf
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/examplegrid7.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/examplegrid7.dgf`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 Simplexgenerator
 %min-angle 1.1        % quality enhancment 
 %max-area 0.1         % maximum element area restriction
 display 0              % show result using the Tetgen viewer
 
 % to use TetGen from a certain path, uncomment this path line
 %path $HOME/bin         % path to Tetgen
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-2-2.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-2-2.dgf`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 VERTEX
 0.0000000000000000e+00 0.0000000000000000e+00
 1.0000000000000000e+00 0.0000000000000000e+00
 1.0000000000000000e+00 1.0000000000000000e+00
 0.0000000000000000e+00 1.0000000000000000e+00
 3.4999999999999998e-01 7.5000000000000000e-01
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-2-3.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-2-3.dgf`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 VERTEX
 1.0000000000000000e+00 0.0000000000000000e+00 0.0000000000000000e+00
 0.0000000000000000e+00 1.0000000000000000e+00 0.0000000000000000e+00
 -1.0000000000000000e+00 0.0000000000000000e+00 0.0000000000000000e+00
 0.0000000000000000e+00 -1.0000000000000000e+00 0.0000000000000000e+00
 0.0000000000000000e+00 0.0000000000000000e+00 -1.0000000000000000e+00
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-3-3-large.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-3-3-large.dgf`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 Vertex
 7.17174e-05 66.8155 79.7895 
 7.17174e-05 61.9093 85.9635 
 7.17174e-05 61.9093 76.9564 
 13.8908 65.3557 79.7895 
 12.8712 60.5549 85.9635 
 12.8712 60.5549 76.9564
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/simplex-testgrid-3-3.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/simplex-testgrid-3-3.dgf`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 
 VERTEX
 2.0000000000000001e-01 -9.9999999999999989e-01 1.0000000000000000e+01
 1.2000000000000000e+00 -9.9999999999999944e-01 1.0000000000000000e+01
 -8.5725275940314732e-17 -8.0000000000000004e-01 8.7500000000000000e+00
 -5.1435165564188829e-16 1.9999999999999996e-01 8.7500000000000000e+00
 -2.0000000000000001e-01 -1.0000000000000000e+00 7.5000000000000000e+00
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/dgf/unstr_cube.dgf` & `dune-grid-2.9.dev20220529/doc/grids/dgf/unstr_cube.dgf`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 DGF
-% SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-% SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 VERTEX
 firstindex 1
 0 0
 0.0909 0
 0.1818 0
 0.2727 0
 0.3636 0
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/circle1storder.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/circle1storder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/circle2ndorder.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/circle2ndorder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/curved2d.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/curved2d.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/hybrid-testgrid-2d.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/hybrid-testgrid-2d.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/hybrid-testgrid-3d.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/hybrid-testgrid-3d.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid.geo` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid.geo`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // mesh width associated with points
 lc = 1;
 
 // vertices of the pyramid
 Point(1) = {0, 0, 0, lc};
 Point(2) = {1, 0, 0, lc};
 Point(3) = {1, 1, 0, lc};
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid1storder.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid1storder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/pyramid2ndorder.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/pyramid2ndorder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/sphere.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/sphere.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/telescope.geo` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope.geo`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // mesh width associated with points
 lc = 0.5;
 
 // circle
 r  = 1.0;
 cx = 0.0;
 cy = 0.0;
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/telescope.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/telescope1storder.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope1storder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/telescope2ndorder.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/telescope2ndorder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gmsh/twotets.msh` & `dune-grid-2.9.dev20220529/doc/grids/gmsh/twotets.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/gridfactory/hybridtestgrids.hh` & `dune-grid-2.9.dev20220529/doc/grids/gridfactory/hybridtestgrids.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_HYBRID_TESTGRIDS_HH
 #define DUNE_HYBRID_TESTGRIDS_HH
 
 /** \file
     \author Oliver Sander
     \brief Provides C++ code that creates hybrid grids suitable for unit tests,
         using the GridFactory.
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/gridfactory/testgrids.hh` & `dune-grid-2.9.dev20220529/doc/grids/gridfactory/testgrids.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DOC_GRIDS_GRIDFACTORY_TESTGRIDS_HH
 #define DOC_GRIDS_GRIDFACTORY_TESTGRIDS_HH
 
 #include <utility>
 #include <vector>
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-grid-2.9.0rc1/doc/grids/starcd/star.cel` & `dune-grid-2.9.dev20220529/doc/grids/starcd/star.cel`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/starcd/star.vrt` & `dune-grid-2.9.dev20220529/doc/grids/starcd/star.vrt`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/starcd/tets.cel` & `dune-grid-2.9.dev20220529/doc/grids/starcd/tets.cel`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/grids/starcd/tets.vrt` & `dune-grid-2.9.dev20220529/doc/grids/starcd/tets.vrt`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/doc/recipes/recipe-integration.cc` & `dune-grid-2.9.dev20220529/doc/recipes/recipe-integration.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file COPYING in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /**
  * \page recipe-integration Integrate a function on a grid
  *
  * A fundamental task in any PDE solver is integration of a function over a domain given by a grid:
  * \f[
  *  I = \int_\Omega u(x)\,dx = \sum_{e\in E^0} \int_e u(x)\,dx
  * \f]
```

### Comparing `dune-grid-2.9.0rc1/doc/recipes/recipe-iterate-over-grid.cc` & `dune-grid-2.9.dev20220529/doc/recipes/recipe-iterate-over-grid.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file COPYING in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /**
  * \page recipe-iterate-over-grid Iterating over a grid
  *
  * A fundamental task in many finite element-type discretizations is iterating
  * over the elements of a grid, for example in order to numerically compute integrals
  * on it. All DUNE grids provide a unified interface for this and related operations.
  *
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_subdirectory(test)
 
 if(Alberta_FOUND)
   foreach(_dim ${ALBERTA_WORLD_DIMS})
     target_sources(dunealbertagrid${_dim}d PRIVATE
       dgfparser.cc
       elementinfo.cc
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/agrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/agrid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRID_IMP_HH
 #define DUNE_ALBERTAGRID_IMP_HH
 
 /** \file
  *  \author Robert Kloefkorn and Martin Nolte
@@ -157,22 +155,16 @@
     typedef typename Traits::HierarchicIndexSet HierarchicIndexSet;
 
     //! type of global id set
     typedef typename Traits::GlobalIdSet GlobalIdSet;
     //! type of local id set
     typedef typename Traits::LocalIdSet LocalIdSet;
 
-    //! type of communication
-    typedef typename Traits::Communication Communication;
-
-    /**
-     * \deprecated Use Communication instead! Will be removed after Dune 2.9.
-     */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    //! type of collective communication
+    typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
   private:
     //! type of LeafIterator
     typedef typename Traits::template Codim<0>::LeafIterator LeafIterator;
 
     //! id set impl
     typedef AlbertaGridIdSet<dim,dimworld> IdSetImp;
@@ -402,17 +394,17 @@
 
     //! returns true, if a least one element is marked for coarsening
     bool preAdapt ();
 
     //! clean up some markers
     void postAdapt();
 
-    /** \brief return reference to communication, if MPI found
+    /** \brief return reference to collective communication, if MPI found
      * this is specialisation for MPI */
-    const Communication &comm () const
+    const CollectiveCommunication &comm () const
     {
       return comm_;
     }
 
     static std::string typeName ()
     {
       std::ostringstream s;
@@ -553,16 +545,16 @@
     const Alberta::GlobalVector &
     getCoord ( const ElementInfo &elementInfo, int vertex ) const;
 
   private:
     // pointer to an Albert Mesh, which contains the data
     MeshPointer mesh_;
 
-    // communication
-    Communication comm_;
+    // collective communication
+    CollectiveCommunication comm_;
 
     // maximum level of the mesh
     int maxlevel_;
 
     // number of boundary segments within the macro grid
     size_t numBoundarySegments_;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/albertagrid.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/albertagrid.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRID_CC
 #define DUNE_ALBERTAGRID_CC
 
 //************************************************************************
 //
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/albertaheader.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/albertaheader.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAHEADER_HH
 #define DUNE_ALBERTAHEADER_HH
 
 #if HAVE_ALBERTA
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/albertareader.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/albertareader.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_ALBERTAREADER_HH
 #define DUNE_ALBERTA_ALBERTAREADER_HH
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/algebra.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/algebra.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_ALGEBRA_HH
 #define DUNE_ALBERTA_ALGEBRA_HH
 
 #include <dune/common/fvector.hh>
 #include <dune/common/fmatrix.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/backuprestore.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/backuprestore.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_ALBERTAGRID_BACKUPRESTORE_HH
 #define DUNE_GRID_ALBERTAGRID_BACKUPRESTORE_HH
 
 #include <dune/grid/common/backuprestore.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/capabilities.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/capabilities.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_CAPABILITIES_HH
 #define DUNE_ALBERTA_CAPABILITIES_HH
 
 #include <dune/geometry/type.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/coordcache.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/coordcache.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_COORDCACHE_HH
 #define DUNE_ALBERTA_COORDCACHE_HH
 
 #include <dune/grid/albertagrid/meshpointer.hh>
 #include <dune/grid/albertagrid/dofadmin.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/datahandle.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/datahandle.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRIDDATAHANDLE_HH
 #define DUNE_ALBERTAGRIDDATAHANDLE_HH
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/dgfparser.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/dgfparser.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 // compile surface grid support into the lib even for ALBERTA 2.0
 #define DUNE_ALBERTA_SURFACE_GRID 1
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/dgfparser.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/dgfparser.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_DGFPARSER_HH
 #define DUNE_ALBERTA_DGFPARSER_HH
 
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_tetrahedron.svg` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/alberta_tetrahedron.svg`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/doc/alberta_triangle.svg` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/doc/alberta_triangle.svg`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/dofadmin.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/dofadmin.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_DOFADMIN_HH
 #define DUNE_ALBERTA_DOFADMIN_HH
 
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/dofvector.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/dofvector.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_DOFVECTOR_HH
 #define DUNE_ALBERTA_DOFVECTOR_HH
 
 #include <cstdlib>
 #include <limits>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/elementinfo.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/elementinfo.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 /** \file
  *  \author Martin Nolte
  *  \brief  provides a wrapper for ALBERTA's el_info structure
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/elementinfo.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/elementinfo.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_ELEMENTINFO_HH
 #define DUNE_ALBERTA_ELEMENTINFO_HH
 
 /** \file
  *  \author Martin Nolte
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/entity.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/entity.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_ENTITY_CC
 #define DUNE_ALBERTA_ENTITY_CC
 
 namespace Dune
 {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/entity.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/entity.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_ENTITY_HH
 #define DUNE_ALBERTA_ENTITY_HH
 
 #include <dune/grid/common/entity.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/entityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/entityseed.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_ENTITYSEED_HH
 #define DUNE_ALBERTA_ENTITYSEED_HH
 
 #include <dune/grid/albertagrid/elementinfo.hh>
 #include <dune/grid/albertagrid/meshpointer.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/geometry.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometry.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_GEOMETRY_CC
 #define DUNE_ALBERTA_GEOMETRY_CC
 
 #include <dune/grid/albertagrid/algebra.hh>
 #include <dune/grid/albertagrid/geometry.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/geometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometry.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_GEOMETRY_HH
 #define DUNE_ALBERTA_GEOMETRY_HH
 
 #include <dune/grid/common/geometry.hh>
 #include <dune/grid/albertagrid/misc.hh>
@@ -125,17 +123,14 @@
 
     typedef FieldVector< ctype, mydimension > LocalCoordinate;
     typedef FieldVector< ctype, coorddimension > GlobalCoordinate;
 
     typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianTransposed;
     typedef FieldMatrix< ctype, coorddimension, mydimension > JacobianInverseTransposed;
 
-    typedef FieldMatrix< ctype, coorddimension, mydimension > Jacobian;
-    typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianInverse;
-
   private:
     static constexpr int numCorners = mydimension + 1;
 
     typedef FieldMatrix< ctype, numCorners, coorddimension > CoordMatrix;
 
   public:
     AlbertaGridGeometry ()
@@ -230,26 +225,14 @@
     /** \brief transposed inverse of the geometry mapping's Jacobian */
     const JacobianInverseTransposed &
     jacobianInverseTransposed ( [[maybe_unused]] const LocalCoordinate &local ) const
     {
       return jacobianInverseTransposed();
     }
 
-    /** \brief geometry mapping's Jacobian */
-    Jacobian jacobian ( const LocalCoordinate &local ) const
-    {
-      return jacobianTransposed(local).transposed();
-    }
-
-    /** \brief inverse of the geometry mapping's Jacobian */
-    JacobianInverse jacobianInverse ( const LocalCoordinate &local ) const
-    {
-      return jacobianInverseTransposed(local).transposed();
-    }
-
     //***********************************************************************
     //  Methods that not belong to the Interface, but have to be public
     //***********************************************************************
 
     /** \brief invalidate the geometry */
     void invalidate ()
     {
@@ -341,17 +324,14 @@
 
     typedef FieldVector< ctype, mydimension > LocalCoordinate;
     typedef FieldVector< ctype, coorddimension > GlobalCoordinate;
 
     typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianTransposed;
     typedef FieldMatrix< ctype, coorddimension, mydimension > JacobianInverseTransposed;
 
-    typedef FieldMatrix< ctype, coorddimension, mydimension > Jacobian;
-    typedef FieldMatrix< ctype, mydimension, coorddimension > JacobianInverse;
-
   private:
     static constexpr int numCorners = mydimension + 1;
 
     typedef FieldMatrix< ctype, numCorners, coorddimension > CoordMatrix;
 
   public:
     AlbertaGridGlobalGeometry ()
@@ -456,26 +436,14 @@
     /** \brief transposed inverse of the geometry mapping's Jacobian */
     const JacobianInverseTransposed &
     jacobianInverseTransposed ( const LocalCoordinate &local ) const
     {
       return jacobianInverseTransposed();
     }
 
-    /** \brief geometry mapping's Jacobian */
-    Jacobian jacobian ( const LocalCoordinate &local ) const
-    {
-      return jacobianTransposed(local).transposed();
-    }
-
-    /** \brief inverse of the geometry mapping's Jacobian */
-    JacobianInverse jacobianInverse ( const LocalCoordinate &local ) const
-    {
-      return jacobianInverseTransposed(local).transposed();
-    }
-
     //***********************************************************************
     //  Methods that not belong to the Interface, but have to be public
     //***********************************************************************
 
     /** \brief invalidate the geometry */
     void invalidate ()
     {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/geometrycache.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/geometrycache.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_GEOMETRYCACHE_HH
 #define DUNE_ALBERTA_GEOMETRYCACHE_HH
 
 #include <dune/grid/albertagrid/misc.hh>
 #include <dune/grid/albertagrid/algebra.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/gridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/gridfactory.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ALBERTA_GRIDFACTORY_HH
 #define DUNE_ALBERTA_GRIDFACTORY_HH
 
 /** \file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/gridfamily.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/gridfamily.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRID_GRIDFAMILTY_HH
 #define DUNE_ALBERTAGRID_GRIDFAMILTY_HH
 
 /** \file
  *  \author Martin Nolte
@@ -141,21 +139,15 @@
 
       typedef IndexSet< GridImp, LevelIndexSetImp, int, std::array< GeometryType, 1 > > LevelIndexSet;
       typedef IndexSet< GridImp, LeafIndexSetImp, int, std::array< GeometryType, 1 > > LeafIndexSet;
       typedef AlbertaGridHierarchicIndexSet< dim, dimworld > HierarchicIndexSet;
       typedef IdSet<GridImp,IdSetImp,IdType> GlobalIdSet;
       typedef IdSet<GridImp,IdSetImp,IdType> LocalIdSet;
 
-      typedef Dune::Communication< No_Comm > Communication;
-
-      /**
-       * \deprecated Use Communication instead! Will be removed after Dune 2.9.
-       */
-      [[deprecated("Use Communication instead!")]]
-      typedef Communication CollectiveCommunication;
+      typedef Dune::Communication< No_Comm > CollectiveCommunication;
     };
   };
 
 }
 
 #endif // #if HAVE_ALBERTA
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/gridview.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/gridview.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRID_GRIDVIEW_HH
 #define DUNE_ALBERTAGRID_GRIDVIEW_HH
 
 #if HAVE_ALBERTA
 
@@ -39,20 +37,16 @@
     /** \brief type of the intersection */
     typedef typename Grid::Traits::LevelIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid::Traits::LevelIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid::Traits::Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid::Traits::CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid::Traits::template Codim< cd >::template Partition< All_Partition >::LevelIterator Iterator;
 
       typedef typename Grid::Traits::template Codim< cd >::Entity Entity;
@@ -91,20 +85,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits::Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits::IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits::Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits::template Codim<cd> {};
 
     constexpr static bool conforming = Traits::conforming;
 
@@ -213,16 +203,16 @@
     IntersectionIterator
     iend ( const typename Codim< 0 >::Entity &entity ) const
     {
       typename IntersectionIteratorImpl::End end;
       return IntersectionIteratorImpl( entity.impl(), end );
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize ( [[maybe_unused]] int codim ) const { return 0; }
 
@@ -257,20 +247,16 @@
     /** \brief type of the intersection */
     typedef typename Grid::Traits::LeafIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid::Traits::LeafIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid::Traits::Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid::Traits::CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid::Traits::template Codim< cd >::template Partition< All_Partition >::LeafIterator
       Iterator;
 
@@ -310,20 +296,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits::Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits::IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits::Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits::template Codim<cd> {};
 
     constexpr static bool conforming = Traits::conforming;
 
@@ -432,16 +414,16 @@
     iend ( const typename Codim< 0 >::Entity &entity ) const
     {
       assert( !!entity.impl().elementInfo() );
       typename IntersectionIteratorImpl::End end;
       return IntersectionIteratorImpl( entity.impl(), end );
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize ( [[maybe_unused]] int codim ) const { return 0; }
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/hierarchiciterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/hierarchiciterator.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_HIERARCHICITERATOR_HH
 #define DUNE_ALBERTA_HIERARCHICITERATOR_HH
 
 #include <dune/grid/albertagrid/elementinfo.hh>
 #include <dune/grid/common/entityiterator.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/indexsets.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/indexsets.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #if HAVE_ALBERTA
 
 #include <dune/grid/albertagrid/indexsets.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/indexsets.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/indexsets.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRIDINDEXSETS_HH
 #define DUNE_ALBERTAGRIDINDEXSETS_HH
 
 #include <array>
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/indexstack.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/indexstack.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTAGRID_INDEXSTACK_HH
 #define DUNE_ALBERTAGRID_INDEXSTACK_HH
 
 #include <assert.h>
 #include <stack>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/intersection.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/intersection.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_INTERSECTION_CC
 #define DUNE_ALBERTA_INTERSECTION_CC
 
 #include <dune/grid/albertagrid/intersection.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/intersection.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/intersection.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_INTERSECTION_HH
 #define DUNE_ALBERTA_INTERSECTION_HH
 
 #include <dune/grid/common/intersection.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/intersectioniterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/intersectioniterator.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_INTERSECTIONITERATOR_HH
 #define DUNE_ALBERTA_INTERSECTIONITERATOR_HH
 
 #include <dune/grid/common/intersectioniterator.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/leafiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/leafiterator.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_LEAFITERATOR_HH
 #define DUNE_ALBERTA_LEAFITERATOR_HH
 
 #include <dune/grid/common/entityiterator.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/level.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/level.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_LEVEL_HH
 #define DUNE_ALBERTA_LEVEL_HH
 
 #include <cassert>
 #include <cstdlib>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/leveliterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/leveliterator.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_LEVELITERATOR_HH
 #define DUNE_ALBERTA_LEVELITERATOR_HH
 
 #include <dune/grid/common/entityiterator.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/macrodata.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/macrodata.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <vector>
 #include <array>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/macrodata.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/macrodata.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_MACRODATA_HH
 #define DUNE_ALBERTA_MACRODATA_HH
 
 /** \file
  *  \author Martin Nolte
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/macroelement.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/macroelement.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_MACROELEMENT_HH
 #define DUNE_ALBERTA_MACROELEMENT_HH
 
 #include <dune/grid/albertagrid/misc.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/meshpointer.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/meshpointer.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #if HAVE_ALBERTA
 
 #include <dune/grid/albertagrid/meshpointer.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/meshpointer.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/meshpointer.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_MESHPOINTER_HH
 #define DUNE_ALBERTA_MESHPOINTER_HH
 
 /** \file
  *  \author Martin Nolte
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/misc.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/misc.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_MISC_HH
 #define DUNE_ALBERTA_MISC_HH
 
 #include <cassert>
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/projection.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/projection.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_NODEPROJECTION_HH
 #define DUNE_ALBERTA_NODEPROJECTION_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/refinement.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/refinement.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_REFINEMENT_HH
 #define DUNE_ALBERTA_REFINEMENT_HH
 
 /** \file
  *  \author Martin Nolte
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/structuredgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/structuredgridfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ALBERTA_STRUCTUREDGRIDFACTORY_HH
 #define DUNE_ALBERTA_STRUCTUREDGRIDFACTORY_HH
 
 /** \file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/test/test-alberta3d-refine.cc` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/test/test-alberta3d-refine.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
 
 #include <cmath>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/transformation.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/transformation.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ALBERTA_TRANSFORMATION_HH
 #define DUNE_ALBERTA_TRANSFORMATION_HH
 
 #include <dune/common/fvector.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/treeiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/treeiterator.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ALBERTA_TREEITERATOR_HH
 #define DUNE_ALBERTA_TREEITERATOR_HH
 
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/undefAllMacros.pl` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/undefAllMacros.pl`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 #!/usr/bin/perl -w
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 
 use strict;
 
 # configuration
 my $packagename = 'alberta';
 my $outfilename = $packagename."_undefs.hh";
 my $cppflagname = 'ALBERTA_CPPFLAGS';
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/undefine-2.0.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/undefine-2.0.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
  * \brief Contains <tt>\#undef</tt>s for all preprocessor macros
  * defined by alberta.
  *
  * This file is created automatically by the perl script <tt>undefAllMacros.pl</tt>.
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/albertagrid/undefine-3.0.hh` & `dune-grid-2.9.dev20220529/dune/grid/albertagrid/undefine-3.0.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
  * \brief Contains <tt>\#undef</tt>s for all preprocessor macros
  * defined by alberta.
  *
  * This file is created automatically by the perl script <tt>undefAllMacros.pl</tt>.
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/common/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 set(HEADERS
   adaptcallback.hh
   backuprestore.hh
   boundaryprojection.hh
   boundarysegment.hh
   capabilities.hh
   datahandleif.hh
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/adaptcallback.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/adaptcallback.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_ADAPTCALLBACK_HH
 #define DUNE_GRID_COMMON_ADAPTCALLBACK_HH
 
 /** \file
  *  \author Martin Nolte
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/backuprestore.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/backuprestore.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_BACKUPRESTORE_HH
 #define DUNE_GRID_COMMON_BACKUPRESTORE_HH
 
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/boundaryprojection.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/boundaryprojection.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_BOUNDARYPROJECTION_HH
 #define DUNE_GRID_COMMON_BOUNDARYPROJECTION_HH
 
 //- system includes
 #include <cmath>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/boundarysegment.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/boundarysegment.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_BOUNDARY_SEGMENT_HH
 #define DUNE_GRID_COMMON_BOUNDARY_SEGMENT_HH
 
 #include <map>
 #include <sstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/capabilities.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/capabilities.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_CAPABILITIES_HH
 #define DUNE_GRID_COMMON_CAPABILITIES_HH
 
 /** \file
     \brief A set of traits classes to store static information about grid implementation
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/cube-to-tet-6.png` & `dune-grid-2.9.dev20220529/dune/grid/common/cube-to-tet-6.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/cube-to-tet-6.svg` & `dune-grid-2.9.dev20220529/dune/grid/common/cube-to-tet-6.svg`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/datahandleif.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/datahandleif.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_DATAHANDLEIF_HH
 #define DUNE_GRID_COMMON_DATAHANDLEIF_HH
 
 /** @file
    @author Robert Kloefkorn
@@ -22,15 +20,15 @@
      buffer. As message buffers might be deeply implemented in various
      packages the message buffers implementations cannot be derived from
      this interface class. Therefore we just apply the engine concept to
      wrap the message buffer call and make sure that the interface is
      fulfilled.
 
      \tparam MessageBufferImp Implementation of message buffer used by the grids' communication method
-     \ingroup GICommunication
+     \ingroup GICollectiveCommunication
    */
   template <class MessageBufferImp>
   class MessageBufferIF
   {
     MessageBufferImp & buff_;
   public:
     //! stores reference to original buffer \c buff
@@ -67,15 +65,15 @@
      communication in parallel runs using the Grid::communicate methods.
      Here the Barton-Nackman trick is used to interprete data handle objects
      as its interface. Therefore usable data handle classes need to be
      derived from this class.
 
      \tparam DataHandleImp implementation of the users data handle
      \tparam DataTypeImp type of data that are going to be communicated which is exported as \c DataType (for example double)
-     \ingroup GICommunication
+     \ingroup GICollectiveCommunication
    */
   template <class DataHandleImp, class DataTypeImp>
   class CommDataHandleIF
   {
     template <class M>
     class CheckFixedSizeMethod
     {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/defaultgridview.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/defaultgridview.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_DEFAULTGRIDVIEW_HH
 #define DUNE_GRID_COMMON_DEFAULTGRIDVIEW_HH
 
 #include <dune/common/typetraits.hh>
 #include <dune/common/exceptions.hh>
@@ -35,20 +33,16 @@
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LevelIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LevelIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid :: Traits
       :: template Codim< cd > :: template Partition< All_Partition > :: LevelIterator
       Iterator;
@@ -90,20 +84,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     constexpr static bool conforming = Traits :: conforming;
 
@@ -178,16 +168,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return entity.impl().ilevelend();
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize(int codim) const
     {
@@ -228,20 +218,16 @@
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LeafIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LeafIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid :: Traits
       :: template Codim< cd > :: template Partition< All_Partition > :: LeafIterator
       Iterator;
@@ -283,20 +269,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     constexpr static bool conforming = Traits :: conforming;
 
@@ -371,16 +353,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return entity.impl().ileafend();
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize(int codim) const
     {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/entity.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/entity.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_ENTITY_HH
 #define DUNE_GRID_COMMON_ENTITY_HH
 
 #include <type_traits>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/entityiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/entityiterator.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_ENTITYITERATOR_HH
 #define DUNE_GRID_COMMON_ENTITYITERATOR_HH
 
 #include <cstddef>
 #include <iterator>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/entityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/entityseed.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_ENTITY_SEED_HH
 #define DUNE_GRID_COMMON_ENTITY_SEED_HH
 
 #include <dune/grid/common/grid.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/geometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/geometry.hh`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_GEOMETRY_HH
 #define DUNE_GRID_COMMON_GEOMETRY_HH
 
 /** \file
     \brief Wrapper and interface classes for element geometries
  */
 
 #include <cassert>
 
 #include <dune/common/fmatrix.hh>
 #include <dune/common/typetraits.hh>
-#include <dune/common/transpose.hh>
-#include <dune/common/std/type_traits.hh>
 
 #include <dune/geometry/referenceelements.hh>
 
 namespace Dune
 {
 
   // External Forward Declarations
@@ -126,72 +122,14 @@
      * However, it is guaranteed to have the following properties:
      * - It satisfies the ConstMatrix interface.
      * - It is copy constructible and copy assignable.
      * .
      */
     typedef typename Implementation::JacobianTransposed JacobianTransposed;
 
-  private:
-
-    template<class Implementation_T>
-    using JacobianInverseOfImplementation = decltype(typename Implementation_T::JacobianInverse{std::declval<Implementation_T>().jacobianInverse(std::declval<LocalCoordinate>())});
-
-    using JacobianInverseDefault = decltype(transpose(std::declval<JacobianInverseTransposed>()));
-
-    template<class Implementation_T>
-    using JacobianOfImplementation = decltype(typename Implementation_T::Jacobian{std::declval<Implementation_T>().jacobian(std::declval<LocalCoordinate>())});
-
-    using JacobianDefault = decltype(transpose(std::declval<JacobianTransposed>()));
-
-    auto jacobianImpl ( const LocalCoordinate &local, std::true_type /*implDetected*/ ) const
-    {
-      return impl().jacobian(local);
-    }
-
-    [[deprecated("Geometry implementatons are required to provide a jacobian(local) method. The default implementation is deprecated and will be removed after release 2.9")]]
-    auto jacobianImpl ( const LocalCoordinate &local, std::false_type /*implNotDetected*/ ) const
-    {
-      return transpose(jacobianTransposed(local));
-    }
-
-    auto jacobianInverseImpl ( const LocalCoordinate &local, std::true_type /*implDetected*/ ) const
-    {
-      return impl().jacobianInverse(local);
-    }
-
-    [[deprecated("Geometry implementatons are required to provide a jacobianInverse(local) method. The default implementation is deprecated and will be removed after release 2.9")]]
-    auto jacobianInverseImpl ( const LocalCoordinate &local, std::false_type /*implNotDetected*/ ) const
-    {
-      return transpose(jacobianInverseTransposed(local));
-    }
-
-  public:
-
-    /**
-     * \brief type of jacobian inverse
-     *
-     * The exact type is implementation-dependent.
-     * However, it is guaranteed to have the following properties:
-     * - You can multilply it from the right to a suitable FieldMatrix
-     * - It is copy constructible and copy assignable.
-     * .
-     */
-    using JacobianInverse = Std::detected_or_t<JacobianInverseDefault, JacobianInverseOfImplementation, Implementation>;
-
-    /**
-     * \brief type of jacobian
-     *
-     * The exact type is implementation-dependent.
-     * However, it is guaranteed to have the following properties:
-     * - You can multilply it from the right to a suitable FieldMatrix
-     * - It is copy constructible and copy assignable.
-     * .
-     */
-    using Jacobian = Std::detected_or_t<JacobianDefault, JacobianOfImplementation, Implementation>;
-
     /** \brief Return the type of the reference element. The type can
        be used to access the Dune::ReferenceElement.
      */
     GeometryType type () const { return impl().type(); }
 
     /** \brief Return true if the geometry mapping is affine and false otherwise */
     bool affine() const { return impl().affine(); }
@@ -325,59 +263,14 @@
      *
      *  \note The exact return type is implementation defined.
      */
     JacobianInverseTransposed jacobianInverseTransposed ( const LocalCoordinate &local ) const
     {
       return impl().jacobianInverseTransposed(local);
     }
-
-    /** \brief Return the Jacobian
-     *
-     *  The Jacobian is defined in the documentation of
-     *  \ref Dune::Geometry::integrationElement "integrationElement".
-     *
-     *  \param[in]  local  position \f$x\in D\f$
-     *
-     *  \return \f$J_g(x)\f$
-     *
-     *  \note The exact return type is implementation defined.
-     */
-    Jacobian jacobian ( const LocalCoordinate& local ) const
-    {
-      auto implDetected = Std::is_detected<JacobianOfImplementation, Implementation>{};
-      return jacobianImpl(local, implDetected);
-    }
-
-    /** \brief Return inverse of Jacobian
-     *
-     *  The Jacobian is defined in the documentation of
-     *  \ref Dune::Geometry::integrationElement "integrationElement".
-     *
-     *  \param[in]  local  position \f$x\in D\f$
-     *  \return \f$J_g^{-1}(x)\f$
-     *
-     *  The use of this function is to compute the jacobians of some function
-     *  \f$f : W \to \textbf{R}\f$ at some position \f$y=g(x)\f$, where
-     *  \f$x\in D\f$ and \f$g\f$ the transformation of the Geometry.
-     *  When we set \f$\hat{f}(x) = f(g(x))\f$ and apply the chain rule we obtain
-     *  \f[\nabla f(g(x)) = J_{\hat{f}}(x) J_g^{-1}(x).\f]
-     *
-     *  \note In the non-quadratic case \f$\textrm{cdim} \neq \textrm{mydim}\f$, the
-     *        pseudoinverse of \f$J_g(x)\f$ is returned.
-     *        This means that its transposed is inverse for all tangential vectors in
-     *        \f$g(x)\f$ while mapping all normal vectors to zero.
-     *
-     *  \note The exact return type is implementation defined.
-     */
-    JacobianInverse jacobianInverse ( const LocalCoordinate &local ) const
-    {
-      auto implDetected = Std::is_detected<JacobianInverseOfImplementation, Implementation>{};
-      return jacobianInverseImpl(local, implDetected);
-    }
-
     //===========================================================
     /** @name Interface for grid implementers
      */
     //@{
     //===========================================================
 
     //! copy constructor from implementation
@@ -419,20 +312,14 @@
 
     //! type of jacobian inverse transposed
     typedef FieldMatrix< ctype, cdim, mydim > JacobianInverseTransposed;
 
     //! type of jacobian transposed
     typedef FieldMatrix< ctype, mydim, cdim > JacobianTransposed;
 
-    //! type of jacobian inverse
-    typedef FieldMatrix< ctype, mydim, cdim > JacobianInverse;
-
-    //! type of jacobian
-    typedef FieldMatrix< ctype, cdim, mydim > Jacobian;
-
     //! return volume of the geometry
     Volume volume () const
     {
       GeometryType type = asImp().type();
 
       // get corresponding reference element
       auto refElement = referenceElement< ctype , mydim >(type);
@@ -456,26 +343,14 @@
       auto refElement = referenceElement< ctype , mydim >(type);
 
       // center is (for now) the centroid of the reference element mapped to
       // this geometry.
       return asImp().global(refElement.position(0,0));
     }
 
-    //! Return the Jacobian
-    Jacobian jacobian ( const LocalCoordinate& local ) const
-    {
-      return asImp().jacobianTransposed(local).transposed();
-    }
-
-    //! Return inverse of Jacobian
-    JacobianInverse jacobianInverse ( const LocalCoordinate &local ) const
-    {
-      return asImp().jacobianInverseTransposed(local).transposed();
-    }
-
   private:
     //!  Barton-Nackman trick
     GeometryImp<mydim,cdim,GridImp>& asImp () {return static_cast<GeometryImp<mydim,cdim,GridImp>&>(*this);}
     const GeometryImp<mydim,cdim,GridImp>& asImp () const {return static_cast<const GeometryImp<mydim,cdim,GridImp>&>(*this);}
   }; // end GeometryDefault
 
   template<int cdim, class GridImp, template<int,int,class> class GeometryImp>
@@ -497,20 +372,14 @@
 
     //! type of jacobian inverse transposed
     typedef FieldMatrix< ctype, cdim, mydim > JacobianInverseTransposed;
 
     //! type of jacobian transposed
     typedef FieldMatrix< ctype, mydim, cdim > JacobianTransposed;
 
-    //! type of jacobian inverse
-    typedef FieldMatrix< ctype, mydim, cdim > JacobianInverse;
-
-    //! type of jacobian
-    typedef FieldMatrix< ctype, cdim, mydim > Jacobian;
-
     //! return the only coordinate
     FieldVector<ctype, cdim> global (const FieldVector<ctype, mydim>& local) const
     {
       return asImp().corner(0);
     }
 
     //! return empty vector
@@ -527,26 +396,14 @@
 
     //! return center of the geometry
     FieldVector<ctype, cdim> center () const
     {
       return asImp().corner(0);
     }
 
-    //! Return the Jacobian
-    Jacobian jacobian ( const LocalCoordinate& local ) const
-    {
-      return asImp().jacobianTransposed(local).transposed();
-    }
-
-    //! Return inverse of Jacobian
-    JacobianInverse jacobianInverse ( const LocalCoordinate &local ) const
-    {
-      return asImp().jacobianInverseTransposed(local).transposed();
-    }
-
   private:
     // Barton-Nackman trick
     GeometryImp<mydim,cdim,GridImp>& asImp () {return static_cast<GeometryImp<mydim,cdim,GridImp>&>(*this);}
     const GeometryImp<mydim,cdim,GridImp>& asImp () const {return static_cast<const GeometryImp<mydim,cdim,GridImp>&>(*this);}
   }; // end GeometryDefault
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/grid.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/grid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_GRID_HH
 #define DUNE_GRID_COMMON_GRID_HH
 
 /** \file
     \brief Different resources needed by all grid implementations
@@ -12,15 +10,14 @@
 #include <iostream>
 #include <string>
 #include <vector>
 
 // dune-common includes
 #include <dune/common/fvector.hh>
 #include <dune/common/typetraits.hh>
-#include <dune/common/typeutilities.hh>
 
 // dune-geometry includes
 #include <dune/geometry/type.hh>
 
 // local includes
 #include <dune/grid/common/gridenums.hh>
 #include <dune/grid/common/exceptions.hh>
@@ -182,15 +179,15 @@
 
          - Dune::ReferenceElement describes the topology and geometry of standard entities.
          Any given entity of the grid can be completely specified by a reference element
          and a map from this reference element to world coordinate space.
 
          - Dune::GeometryType defines names for the reference elements.
 
-         - Dune::Communication defines an interface to global communication
+         - Dune::CollectiveCommunication defines an interface to global communication
          operations in a portable and transparent way. In particular also for sequential grids.
 
 
 
          @section Grid2 Types making up a grid implementation
 
      Each implementation of the Dune grid interface consist of a number of related types which
@@ -504,33 +501,19 @@
     /*! \brief A type that is a model of Dune::IdSet
        which provides a unique and persistent numbering for
        all entities in the grid. The numbering is only unique in a single process
        and it is not necessarily consecutive.
      */
     typedef typename GridFamily::Traits::LocalIdSet LocalIdSet;
 
-  protected:
-    template <class T>
-    using Communication_t = typename T::Communication;
-    template <class T>
-    using DeprecatedCollectiveCommunication_t = typename T::CollectiveCommunication;
-
-  public:
-    /*! \brief A type that is a model of Dune::Communication.
-       It provides a portable way for communication on the set
+    /*! \brief A type that is a model of Dune::CollectiveCommunication.
+       It provides a portable way for collective communication on the set
        of processes used by the grid.
      */
-    // if this line produces a warning then the Communication typedef is missing
-    // in the GridFamily::Traits
-    using Communication = detected_or_fallback_t< DeprecatedCollectiveCommunication_t,
-                                                  Communication_t, typename GridFamily::Traits>;
-
-    /** \deprecated Use Communication instead! Will be removed at some point in the future.
-     */
-    using CollectiveCommunication [[deprecated("CollectiveCommunication is deprecated, use Communication instead!")]] = Communication;
+    typedef typename GridFamily::Traits::CollectiveCommunication CollectiveCommunication;
 
     //! Define type used for coordinates in grid module
     typedef ct ctype;
     //@}
 
 
     //===========================================================
@@ -728,16 +711,16 @@
 
     //===========================================================
     /** @name Parallel data distribution and communication
      */
     //@{
     //===========================================================
 
-    //! return const reference to a communication object. The return type is a model of Dune::Communication.
-    const Communication &comm () const
+    //! return const reference to a collective communication object. The return type is a model of Dune::CollectiveCommunication.
+    const CollectiveCommunication &comm () const
     {
       CHECK_INTERFACE_IMPLEMENTATION(asImp().comm());
       return asImp().comm();
     }
     //@}
 
     /*! \brief Re-balances the load each process has to handle for a parallel grid,
@@ -968,15 +951,15 @@
      \brief A traits struct that collects all associated types of one grid model
      @ingroup GIMiscellaneous
 
      \tparam dim Grid dimension
      \tparam dimw Dimension of the world that the grid is embedded in
      \tparam GIDType Type used for global ids
      \tparam LIDType Type used for local ids
-     \tparam CCType Communication implementation class
+     \tparam CCType CollectiveCommunication implementation class
    */
   template <int dim, int dimw, class GridImp,
       template<int,int,class> class GeometryImp,
       template<int,int,class> class EntityImp,
       template<int,PartitionIteratorType,class> class LevelIteratorImp,
       template<class> class LeafIntersectionImp,
       template<class> class LevelIntersectionImp,
@@ -1063,20 +1046,16 @@
     /** \brief The type of the leaf index set. */
     typedef IndexSet<const GridImp,LeafIndexSetImp> LeafIndexSet;
     /** \brief The type of the global id set. */
     typedef IdSet<const GridImp,GlobalIdSetImp,GIDType> GlobalIdSet;
     /** \brief The type of the local id set. */
     typedef IdSet<const GridImp,LocalIdSetImp,LIDType> LocalIdSet;
 
-    /** \brief The type of the communication. */
-    typedef CCType Communication;
-
-    /** \deprecated Use Communication instead! Will be removed at some point in the future. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief The type of the collective communication. */
+    typedef CCType CollectiveCommunication;
   };
 
   // Definition of capabilities for the interface class
   namespace Capabilities
   {
 
     // capabilities for the interface class depend on the implementation
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/gridenums.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/gridenums.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_GRIDENUMS_HH
 #define DUNE_GRID_COMMON_GRIDENUMS_HH
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/gridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/gridfactory.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_GRIDFACTORY_HH
 #define DUNE_GRID_COMMON_GRIDFACTORY_HH
 
 /** \file
     \brief Provide a generic factory class for unstructured grids.
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/gridinfo.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/gridinfo.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_COMMON_GRIDINFO_HH
 #define DUNE_GRID_COMMON_GRIDINFO_HH
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/gridview.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/gridview.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_GRIDVIEW_HH
 #define DUNE_GRID_COMMON_GRIDVIEW_HH
 
 #include <typeinfo>
 
-#include <dune/common/std/type_traits.hh>
 #include <dune/common/iteratorrange.hh>
 #include <dune/common/parallel/future.hh>
 
 #include <dune/geometry/type.hh>
 
 #include <dune/grid/common/datahandleif.hh>
 #include <dune/grid/common/rangegenerators.hh>
@@ -87,33 +84,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-  protected:
-    template <class T>
-    using Communication_t = typename T :: Communication;
-    template <class T>
-    using DeprecatedCollectiveCommunication_t = typename T :: CollectiveCommunication;
-
-  public:
-    /*! \brief A type that is a model of Dune::Communication.
-       It provides a portable way for communication on the set
-       of processes used by the grid.
-     */
-    // if this line produces a warning then the Communication typedef is missing
-    // in the Traits
-    using Communication = detected_or_fallback_t<DeprecatedCollectiveCommunication_t,
-                                                 Communication_t, Traits>;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9.
-     */
-    using CollectiveCommunication [[deprecated("CollectiveCommunication is deprecated, use Communication instead!")]] = Communication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief A struct that collects all associated types of one implementation
                from the Traits class.
      */
     template< int cd >
     struct Codim {
       /** \brief type of iterator returned by the grid view */
@@ -134,15 +114,15 @@
       {
         /** \brief iterator over a given codim and partition type */
         typedef typename Traits :: template Codim< cd >
         :: template Partition< pit > :: Iterator Iterator;
       };
     }; //: public Traits :: template Codim<cd> {};
 
-    /** \brief Export if this grid view is guaranteed conforming */
+    /** \brief Export if this grid view is conforming */
     constexpr static bool conforming = Traits :: conforming;
 
     /** \brief type used for coordinates in grid */
     typedef typename Grid::ctype ctype;
 
     //! \brief The dimension of the grid
     constexpr static int dimension = Grid :: dimension;
@@ -272,16 +252,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return impl().iend(entity);
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return impl().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize(int codim) const
     {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/idlocalref.eps` & `dune-grid-2.9.dev20220529/dune/grid/common/idlocalref.eps`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/idlocalref.fig` & `dune-grid-2.9.dev20220529/dune/grid/common/idlocalref.fig`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/idlocalref.png` & `dune-grid-2.9.dev20220529/dune/grid/common/idlocalref.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/indexidset.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/indexidset.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_COMMON_INDEXIDSET_HH
 #define DUNE_GRID_COMMON_INDEXIDSET_HH
 
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/intersection.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/intersection.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_COMMON_INTERSECTION_HH
 #define DUNE_GRID_COMMON_INTERSECTION_HH
 
 #include <dune/grid/common/grid.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/intersectioniterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/intersectioniterator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_INTERSECTIONITERATOR_HH
 #define DUNE_GRID_COMMON_INTERSECTIONITERATOR_HH
 
 #include <dune/common/iteratorfacades.hh>
 #include <dune/common/proxymemberaccess.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/islocalref.eps` & `dune-grid-2.9.dev20220529/dune/grid/common/islocalref.eps`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/islocalref.fig` & `dune-grid-2.9.dev20220529/dune/grid/common/islocalref.fig`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/islocalref.png` & `dune-grid-2.9.dev20220529/dune/grid/common/islocalref.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/mapper.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/mapper.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_MAPPER_HH
 #define DUNE_GRID_COMMON_MAPPER_HH
 
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/mcmgmapper.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/mcmgmapper.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_COMMON_MCMGMAPPER_HH
 #define DUNE_GRID_COMMON_MCMGMAPPER_HH
 
 #include <functional>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/partitionset.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/partitionset.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_PARTITIONSET_HH
 #define DUNE_GRID_COMMON_PARTITIONSET_HH
 
 #include <dune/common/keywords.hh>
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/rangegenerators.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/rangegenerators.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_RANGEGENERATORS_HH
 #define DUNE_GRID_COMMON_RANGEGENERATORS_HH
 
 #include <dune/common/iteratorrange.hh>
 #include <dune/common/rangeutilities.hh>
@@ -115,15 +113,15 @@
    * \code
      std::size_t count = 0;
      for (const auto& e : elements(gv))
      {
        do_stuff();
        for (const auto& i : intersections(gv,e))
        {
-         if (i.boundary())
+         if (e.boundary())
            ++count;
        }
      }
      \endcode
    *
    * <h2>Sub-entities</h2>
    *
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/scsgmapper.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/scsgmapper.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_SCSGMAPPER_HH
 #define DUNE_GRID_COMMON_SCSGMAPPER_HH
 
 #include <iostream>
 #include "mapper.hh"
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/sizecache.hh` & `dune-grid-2.9.dev20220529/dune/grid/common/sizecache.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_COMMON_SIZECACHE_HH
 #define DUNE_GRID_COMMON_SIZECACHE_HH
 
 #include <cassert>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/test/mcmgmappertest.cc` & `dune-grid-2.9.dev20220529/dune/grid/common/test/mcmgmappertest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 /** \file
     \brief A unit test for the MultipleCodimMultipleGeometryMapper
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/common/test/scsgmappertest.cc` & `dune-grid-2.9.dev20220529/dune/grid/common/test/scsgmappertest.cc`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 /** \file
     \brief A unit test for the SingleCodimSingleGeomTypeMapper
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/backuprestore.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/backuprestore.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_BACKUPRESTORE_HH
 #define DUNE_GEOGRID_BACKUPRESTORE_HH
 
 #include <type_traits>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/cachedcoordfunction.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/cachedcoordfunction.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_CACHEDCOORDFUNCTION_HH
 #define DUNE_GEOGRID_CACHEDCOORDFUNCTION_HH
 
 #include <cassert>
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/capabilities.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/capabilities.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_CAPABILITIES_HH
 #define DUNE_GEOGRID_CAPABILITIES_HH
 
 #include <cassert>
 #include <type_traits>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/coordfunction.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/coordfunction.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_COORDFUNCTION_HH
 #define DUNE_GEOGRID_COORDFUNCTION_HH
 
 #include <cassert>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/coordfunctioncaller.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/coordfunctioncaller.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_COORDFUNCTIONCALLER_HH
 #define DUNE_GEOGRID_COORDFUNCTIONCALLER_HH
 
 #include <dune/grid/geometrygrid/hostcorners.hh>
 #include <dune/grid/geometrygrid/coordfunction.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/cornerstorage.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/cornerstorage.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_CORNERSTORAGE_HH
 #define DUNE_GEOGRID_CORNERSTORAGE_HH
 
 #include <array>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/datahandle.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/datahandle.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_DATAHANDLE_HH
 #define DUNE_GEOGRID_DATAHANDLE_HH
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/entity.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/entity.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_ENTITY_HH
 #define DUNE_GEOGRID_ENTITY_HH
 
 #include <dune/geometry/referenceelements.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/entityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/entityseed.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_ENTITYSEED_HH
 #define DUNE_GEOGRID_ENTITYSEED_HH
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/geometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/geometry.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_GEOMETRY_HH
 #define DUNE_GEOGRID_GEOMETRY_HH
 
 #include <utility>
 
@@ -122,17 +120,14 @@
 
     public:
       typedef typename Mapping::LocalCoordinate LocalCoordinate;
       typedef typename Mapping::GlobalCoordinate GlobalCoordinate;
 
       typedef typename Mapping::JacobianTransposed JacobianTransposed;
       typedef typename Mapping::JacobianInverseTransposed JacobianInverseTransposed;
-      typedef typename Mapping::Jacobian Jacobian;
-      typedef typename Mapping::JacobianInverse JacobianInverse;
-
 
       Geometry () : grid_( nullptr ), mapping_( nullptr ) {}
 
       explicit Geometry ( const Grid &grid ) : grid_( &grid ), mapping_( nullptr ) {}
 
       template< class CoordVector >
       Geometry ( const Grid &grid, const GeometryType &type, const CoordVector &coords )
@@ -199,17 +194,14 @@
 
       ctype integrationElement ( const LocalCoordinate &local ) const { return mapping_->integrationElement( local ); }
       ctype volume () const { return mapping_->volume(); }
 
       JacobianTransposed jacobianTransposed ( const LocalCoordinate &local ) const { return mapping_->jacobianTransposed( local ); }
       JacobianInverseTransposed jacobianInverseTransposed ( const LocalCoordinate &local ) const { return mapping_->jacobianInverseTransposed( local ); }
 
-      Jacobian jacobian ( const LocalCoordinate &local ) const { return mapping_->jacobian( local ); }
-      JacobianInverse jacobianInverse ( const LocalCoordinate &local ) const { return mapping_->jacobianInverse( local ); }
-
       const Grid &grid () const { assert( grid_ ); return *grid_; }
 
     private:
       void destroyMapping ()
       {
         mapping_->~Mapping();
         grid().deallocateStorage( mapping_, sizeof( Mapping ) );
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/grid.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/grid.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_GRID_HH
 #define DUNE_GEOGRID_GRID_HH
 
 #include <memory>
 
@@ -206,20 +204,15 @@
     /** \name Miscellaneous Types
      * \{ */
 
     //! type of vector coordinates (e.g., double)
     typedef typename Traits::ctype ctype;
 
     //! communicator with all other processes having some part of the grid
-    typedef typename Traits::Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9.
-     */
-    [[deprecated("Use Communication instead!!")]]
-    typedef Communication CollectiveCommunication;
+    typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
     /** \} */
 
     /** \name Construction and Destruction
      *  \{ */
 
     /** \brief constructor
@@ -230,15 +223,15 @@
      *  \param[in]  hostGrid       reference to the grid to wrap
      *  \param[in]  coordFunction  reference to the coordinate function
      *  \param[in]  allocator      storage allocator
      */
     GeometryGrid ( HostGrid &hostGrid, CoordFunction &coordFunction, const Allocator &allocator = Allocator() )
       : hostGrid_( Dune::stackobject_to_shared_ptr(hostGrid) ),
         coordFunction_( Dune::stackobject_to_shared_ptr(coordFunction) ),
-        levelIndexSets_( hostGrid_->maxLevel()+1 ),
+        levelIndexSets_( hostGrid_->maxLevel()+1, nullptr, allocator ),
         storageAllocator_( allocator )
     {}
 
     /** \brief constructor
      *
      *  The grid takes ownership of the pointers to host grid and coordinate
      *  function. They will be deleted when the grid is destroyed.
@@ -246,15 +239,15 @@
      *  \param[in]  hostGrid       shared pointer to the grid to wrap
      *  \param[in]  coordFunction  shared pointer to the coordinate function
      *  \param[in]  allocator      storage allocator
      */
     GeometryGrid ( std::shared_ptr<HostGrid> hostGrid, std::shared_ptr<CoordFunction> coordFunction, const Allocator &allocator = Allocator() )
       : hostGrid_( hostGrid ),
         coordFunction_( coordFunction ),
-        levelIndexSets_( hostGrid_->maxLevel()+1 ),
+        levelIndexSets_( hostGrid_->maxLevel()+1, nullptr, allocator ),
         storageAllocator_( allocator )
     {}
 
     /** \brief constructor
      *
      *  The grid takes ownership of the pointer to host grid and it will
      *  be deleted when the grid is destroyed. The coordinate function
@@ -262,19 +255,29 @@
      *
      *  \param[in]  hostGrid       shared pointer to the grid to wrap
      *  \param[in]  allocator      storage allocator
      */
     GeometryGrid ( std::shared_ptr<HostGrid> hostGrid, const Allocator &allocator = Allocator() )
       : hostGrid_( hostGrid ),
         coordFunction_( std::make_shared<CoordFunction>( this->hostGrid() ) ),
-        levelIndexSets_( hostGrid_->maxLevel()+1 ),
+        levelIndexSets_( hostGrid_->maxLevel()+1, nullptr, allocator ),
         storageAllocator_( allocator )
     {}
 
 
+    /** \brief destructor
+     */
+    ~GeometryGrid ()
+    {
+      for( unsigned int i = 0; i < levelIndexSets_.size(); ++i )
+      {
+        if( levelIndexSets_[ i ] )
+          delete( levelIndexSets_[ i ] );
+      }
+    }
 
     /** \} */
 
     /** \name Size Methods
      *  \{ */
 
     /** \brief obtain maximal grid level
@@ -366,19 +369,19 @@
       assert( levelIndexSets_.size() == (size_t)(maxLevel()+1) );
       if( (level < 0) || (level > maxLevel()) )
       {
         DUNE_THROW( GridError, "LevelIndexSet for nonexisting level " << level
                                                                       << " requested." );
       }
 
-      auto& levelIndexSetPtr = levelIndexSets_[ level ];
-      if( !levelIndexSetPtr )
-        levelIndexSetPtr = std::make_unique<LevelIndexSet>( hostGrid().levelIndexSet( level ) );
-      assert( levelIndexSetPtr );
-      return *levelIndexSetPtr;
+      LevelIndexSet *&levelIndexSet = levelIndexSets_[ level ];
+      if( !levelIndexSet )
+        levelIndexSet = new LevelIndexSet( hostGrid().levelIndexSet( level ) );
+      assert( levelIndexSet );
+      return *levelIndexSet;
     }
 
     const LeafIndexSet &leafIndexSet () const
     {
       if( !leafIndexSet_ )
         leafIndexSet_.reset( hostGrid().leafIndexSet() );
       assert( leafIndexSet_ );
@@ -417,23 +420,23 @@
     {
       hostGrid().postAdapt();
     }
 
     /** \name Parallel Data Distribution and Communication Methods
      *  \{ */
 
-    /** \brief obtain Communication object
+    /** \brief obtain CollectiveCommunication object
      *
-     *  The Communication object should be used to globally
+     *  The CollectiveCommunication object should be used to globally
      *  communicate information between all processes sharing this grid.
      *
-     *  \note The Communication object returned is identical to the
+     *  \note The CollectiveCommunication object returned is identical to the
      *        one returned by the host grid.
      */
-    const Communication &comm () const
+    const CollectiveCommunication &comm () const
     {
       return hostGrid().comm();
     }
 
 #if 0
     // data handle interface different between geo and interface
 
@@ -555,15 +558,23 @@
      *        called.
      */
     void update ()
     {
       // adapt the coordinate function
       GeoGrid::AdaptCoordFunction< typename CoordFunction::Interface >::adapt( coordFunction() );
 
-      levelIndexSets_.resize( maxLevel()+1 );
+      const int newNumLevels = maxLevel()+1;
+      const int oldNumLevels = levelIndexSets_.size();
+
+      for( int i = newNumLevels; i < oldNumLevels; ++i )
+      {
+        if( levelIndexSets_[ i ] )
+          delete levelIndexSets_[ i ];
+      }
+      levelIndexSets_.resize( newNumLevels, nullptr );
     }
 
 
     /** \brief obtain constant reference to the coordinate function */
     const CoordFunction &coordFunction () const { return *coordFunction_; }
 
     /** \brief obtain mutable reference to the coordinate function. */
@@ -588,15 +599,15 @@
     {
       storageAllocator_.deallocate( (char *)p, size );
     }
 
   private:
     std::shared_ptr<HostGrid> const hostGrid_;
     std::shared_ptr<CoordFunction> coordFunction_;
-    mutable std::vector<std::unique_ptr<LevelIndexSet>> levelIndexSets_;
+    mutable std::vector< LevelIndexSet *, typename std::allocator_traits<Allocator>::template rebind_alloc< LevelIndexSet * > > levelIndexSets_;
     mutable LeafIndexSet leafIndexSet_;
     mutable GlobalIdSet globalIdSet_;
     mutable LocalIdSet localIdSet_;
     mutable typename std::allocator_traits<Allocator>::template rebind_alloc< char > storageAllocator_;
   };
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/gridfamily.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/gridfamily.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_GRIDFAMILY_HH
 #define DUNE_GEOGRID_GRIDFAMILY_HH
 
 #include <dune/grid/common/grid.hh>
 #include <dune/grid/geometrygrid/capabilities.hh>
@@ -104,21 +102,15 @@
         typedef GeoGrid::IndexSet< const Grid, typename HostGrid::Traits::LevelIndexSet > LevelIndexSet;
 
         typedef GeoGrid::IdSet< const Grid, typename HostGrid::Traits::GlobalIdSet >
         GlobalIdSet;
         typedef GeoGrid::IdSet< const Grid, typename HostGrid::Traits::LocalIdSet >
         LocalIdSet;
 
-        typedef typename HostGrid::Traits::Communication Communication;
-
-        /**
-         * \deprecated Use Communication instead! Will be removed after Dune 2.9.
-         */
-        [[deprecated("Use Communication instead!")]]
-        typedef Communication CollectiveCommunication;
+        typedef typename HostGrid::Traits::CollectiveCommunication CollectiveCommunication;
 
         typedef Dune::GridView< GeoGrid::GridViewTraits< typename HostGrid::LeafGridView, CoordFunction, Allocator > > LeafGridView;
         typedef Dune::GridView< GeoGrid::GridViewTraits< typename HostGrid::LevelGridView, CoordFunction, Allocator > > LevelGridView;
       };
     };
 
   } // namespace GeoGrid
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/gridview.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/gridview.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_GRIDVIEW_HH
 #define DUNE_GEOGRID_GRIDVIEW_HH
 
 #include <dune/common/typetraits.hh>
 #include <dune/common/exceptions.hh>
@@ -53,21 +51,15 @@
 
       typedef Dune::Intersection< const Grid, GeoGrid::Intersection< const Grid, HostIntersection > > Intersection;
 
       typedef Dune::IntersectionIterator
       < const Grid, GeoGrid::IntersectionIterator< const Grid, HostIntersectionIterator >, GeoGrid::Intersection< const Grid, HostIntersection > >
       IntersectionIterator;
 
-      typedef typename HostGridView::Communication Communication;
-
-      /**
-       * \deprecated Use Communication instead! Will be removed after Dune 2.9.
-       */
-      [[deprecated("Use Communication instead!!")]]
-      typedef Communication CollectiveCommunication;
+      typedef typename HostGridView::CollectiveCommunication CollectiveCommunication;
 
       template< int codim >
       struct Codim
       {
         typedef GeoGrid::Iterator< HostGridView, codim, All_Partition, const Grid > IteratorImp;
         typedef Dune::EntityIterator< codim, const Grid, IteratorImp > Iterator;
 
@@ -106,21 +98,15 @@
 
       typedef typename Traits::IndexSet IndexSet;
 
       typedef typename Traits::Intersection Intersection;
 
       typedef typename Traits::IntersectionIterator IntersectionIterator;
 
-      typedef typename Traits::Communication Communication;
-
-      /**
-       * \deprecated Use Communication instead! Will be removed after Dune 2.9.
-       */
-      [[deprecated("Use Communication instead!!")]]
-      typedef Communication CollectiveCommunication;
+      typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
       template< int codim >
       struct Codim
         : public Traits::template Codim< codim >
       {};
 
       static const bool conforming = Traits::conforming;
@@ -211,15 +197,15 @@
 
       IntersectionIterator iend ( const typename Codim< 0 >::Entity &entity ) const
       {
         typedef GeoGrid::IntersectionIterator< const Grid, typename HostGridView::IntersectionIterator > IntersectionIteratorImpl;
         return IntersectionIteratorImpl( entity, hostGridView().iend( entity.impl().hostEntity() ) );
       }
 
-      const Communication &comm () const
+      const CollectiveCommunication &comm () const
       {
         return hostGridView().comm();
       }
 
       int overlapSize ( int codim ) const
       {
         return hostGridView().overlapSize( codim );
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/helix.png` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/helix.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/identity.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/identity.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_IDENTITY_HH
 #define DUNE_GEOGRID_IDENTITY_HH
 
 #include <dune/grid/geometrygrid/coordfunction.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/idset.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/idset.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_IDSET_HH
 #define DUNE_GEOGRID_IDSET_HH
 
 #include <dune/grid/common/indexidset.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/indexsets.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/indexsets.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_INDEXSETS_HH
 #define DUNE_GEOGRID_INDEXSETS_HH
 
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/intersection.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/intersection.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_INTERSECTION_HH
 #define DUNE_GEOGRID_INTERSECTION_HH
 
 #include <dune/grid/geometrygrid/declaration.hh>
 #include <dune/grid/geometrygrid/cornerstorage.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/intersectioniterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/intersectioniterator.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_INTERSECTIONITERATOR_HH
 #define DUNE_GEOGRID_INTERSECTIONITERATOR_HH
 
 #include <dune/grid/geometrygrid/intersection.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/iterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/iterator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_ITERATOR_HH
 #define DUNE_GEOGRID_ITERATOR_HH
 
 #include <cassert>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid/persistentcontainer.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid/persistentcontainer.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_PERSISTENTCONTAINER_HH
 #define DUNE_GEOGRID_PERSISTENTCONTAINER_HH
 
 #include <dune/grid/geometrygrid/declaration.hh>
 #include <dune/grid/utility/persistentcontainer.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/geometrygrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/geometrygrid.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <dune/grid/geometrygrid/grid.hh>
 #include <dune/grid/geometrygrid/persistentcontainer.hh>
 
 /** \addtogroup GeoGrid
  *
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridentity.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridentity.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRIDENTITY_HH
 #define DUNE_IDENTITYGRIDENTITY_HH
 
 /** \file
  * \brief The IdentityGridEntity class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridentityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridentityseed.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITY_GRID_ENTITY_SEED_HH
 #define DUNE_IDENTITY_GRID_ENTITY_SEED_HH
 
 /**
  * \file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridgeometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridgeometry.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRIDGEOMETRY_HH
 #define DUNE_IDENTITYGRIDGEOMETRY_HH
 
 /** \file
  * \brief The IdentityGridGeometry class and its specializations
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridhierarchiciterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridhierarchiciterator.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRIDHIERITERATOR_HH
 #define DUNE_IDENTITYGRIDHIERITERATOR_HH
 
 /** \file
  * \brief The IdentityGridHierarchicIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridindexsets.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridindexsets.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRID_INDEXSETS_HH
 #define DUNE_IDENTITYGRID_INDEXSETS_HH
 
 /** \file
  * \brief The index and id sets for the IdentityGrid class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridintersectioniterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridintersectioniterator.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRID_INTERSECTIONITERATOR_HH
 #define DUNE_IDENTITYGRID_INTERSECTIONITERATOR_HH
 
 #include "identitygridintersections.hh"
 #include "identitygridentity.hh"
@@ -67,16 +65,16 @@
     }
 
   private:
     //**********************************************************
     //  private data
     //**********************************************************
 
-    const GridImp* identityGrid_ = nullptr;
-    HostLeafIntersectionIterator hostIterator_ = {};
+    const GridImp* identityGrid_;
+    HostLeafIntersectionIterator hostIterator_;
   };
 
 
 
 
   //! \todo Please doc me !
   template<class GridImp>
@@ -119,16 +117,16 @@
     Intersection dereference() const {
       return IdentityGridLevelIntersection<GridImp>(identityGrid_,*hostIterator_);
     }
 
   private:
 
 
-    const GridImp* identityGrid_ = nullptr;
-    HostLevelIntersectionIterator hostIterator_ = {};
+    const GridImp* identityGrid_;
+    HostLevelIntersectionIterator hostIterator_;
 
   };
 
 
 }  // namespace Dune
 
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridintersections.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridintersections.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRID_INTERSECTIONS_HH
 #define DUNE_IDENTITYGRID_INTERSECTIONS_HH
 
 #include "identitygridleafiterator.hh"
 #include <dune/grid/identitygrid/identitygridentity.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridleafiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridleafiterator.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRIDLEAFITERATOR_HH
 #define DUNE_IDENTITYGRIDLEAFITERATOR_HH
 
 #include <dune/grid/common/gridenums.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid/identitygridleveliterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid/identitygridleveliterator.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IDENTITYGRIDLEVELITERATOR_HH
 #define DUNE_IDENTITYGRIDLEVELITERATOR_HH
 
 #include <dune/grid/common/gridenums.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/identitygrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/identitygrid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_IDENTITYGRID_HH
 #define DUNE_GRID_IDENTITYGRID_HH
 
 /** \file
  * \brief The IdentityGrid class
@@ -375,15 +373,15 @@
      */
     void loadBalance(int strategy, int minlevel, int depth, int maxlevel, int minelement){
       DUNE_THROW(NotImplemented, "IdentityGrid::loadBalance()");
     }
 #endif
 
 
-    /** \brief dummy communication */
+    /** \brief dummy collective communication */
     const Communication<No_Comm>& comm () const
     {
       return ccobj;
     }
 
 
     // **********************************************************
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/CMakeLists.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 target_sources(dunegrid PRIVATE
     basic.cc  boundarydom.cc  boundaryseg.cc
     cube.cc  dim.cc  general.cc  gridparameter.cc
     interval.cc  periodicfacetrans.cc projection.cc simplex.cc  simplexgeneration.cc  vertex.cc)
 #add_dune_mpi_flags(dgfparserblocks)
 
 set(HEADERS
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/basic.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/basic.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/basic.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/basic.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/basic.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_BASICBLOCK_HH
 #define DUNE_DGF_BASICBLOCK_HH
 
 #include <cassert>
 #include <cctype>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundarydom.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundarydom.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/boundarydom.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundarydom.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundarydom.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_BOUNDARYDOMBLOCK_HH
 #define DUNE_DGF_BOUNDARYDOMBLOCK_HH
 
 #include <iostream>
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundaryseg.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundaryseg.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/boundaryseg.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/boundaryseg.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/boundaryseg.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_BOUNDARYSEGBLOCK_HH
 #define DUNE_DGF_BOUNDARYSEGBLOCK_HH
 
 #include <cassert>
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/cube.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/cube.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/cube.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/cube.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/cube.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_CUBEBLOCK_HH
 #define DUNE_DGF_CUBEBLOCK_HH
 
 #include <cassert>
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/dim.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/dim.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_DIMBLOCK_HH
 #define DUNE_DGF_DIMBLOCK_HH
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/general.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/general.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/general.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/general.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/general.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_IO_FILE_DGFPARSER_BLOCKS_GENERAL_HH
 #define DUNE_GRID_IO_FILE_DGFPARSER_BLOCKS_GENERAL_HH
 
 #include <iostream>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/gridparameter.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/gridparameter.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/gridparameter.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/gridparameter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/gridparameter.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_GRIDPARAMETERBLOCK_HH
 #define DUNE_DGF_GRIDPARAMETERBLOCK_HH
 
 #include <iostream>
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/interval.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/interval.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/interval.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/interval.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/interval.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_INTERVALBLOCK_HH
 #define DUNE_DGF_INTERVALBLOCK_HH
 
 #include <iostream>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/periodicfacetrans.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/periodicfacetrans.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_PERIODICFACETRANSBLOCK_HH
 #define DUNE_DGF_PERIODICFACETRANSBLOCK_HH
 
 #include <iostream>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/polygon.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/polygon.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- mode: C++; tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=2 sw=2 sts=2:
 #ifndef DUNE_POLYGON_HH
 #define DUNE_POLYGON_HH
 
 #include <iostream>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/polyhedron.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/polyhedron.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- mode: C++; tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=2 sw=2 sts=2:
 #ifndef DUNE_POLYHEDRON_HH
 #define DUNE_POLYHEDRON_HH
 
 #include <algorithm>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/projection.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/projection.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/common/math.hh>
 
 #include <dune/grid/io/file/dgfparser/blocks/projection.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/projection.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/projection.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_PROJECTIONBLOCK_HH
 #define DUNE_DGF_PROJECTIONBLOCK_HH
 
 #include <map>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplex.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplex.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/simplex.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplex.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/vertex.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,57 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-#ifndef DUNE_DGF_SIMPLEXBLOCK_HH
-#define DUNE_DGF_SIMPLEXBLOCK_HH
+#ifndef DUNE_DGF_VERTEXBLOCK_HH
+#define DUNE_DGF_VERTEXBLOCK_HH
 
 #include <iostream>
 #include <vector>
 
 #include <dune/grid/io/file/dgfparser/blocks/basic.hh>
 
 namespace Dune
 {
 
   namespace dgf
   {
-    // SimplexBlock
-    // ------------
 
-    class SimplexBlock
+    class VertexBlock
       : public BasicBlock
     {
-      unsigned int nofvtx;
+      int dimvertex;         // the dimension of the vertices (determined from DGF file)
+      int dimworld;          // the dimension of the world (either dimvertex or given by user)
+      bool goodline;         // active line describes a vertex
       int vtxoffset;
-      int dimgrid;
-      bool goodline;                 // active line describes a vertex
-      int nofparams;                 // nof parameters
+      int nofParam;
 
     public:
-      SimplexBlock ( std :: istream &in, int pnofvtx, int pvtxoffset, int &pdimgrid );
+      // initialize vertex block
+      VertexBlock ( std :: istream &in, int &pdimworld );
 
-      int get ( std :: vector< std :: vector< unsigned int > > &simplex,
-                std :: vector< std :: vector< double > > &params,
+      int get ( std :: vector< std :: vector< double > > &vtx,
+                std :: vector< std :: vector< double > > &param,
                 int &nofp );
 
-      // cubes -> simplex
-      static int
-      cube2simplex ( std :: vector< std :: vector< double > > &vtx,
-                     std :: vector< std :: vector< unsigned int > > &elements,
-                     std :: vector< std :: vector< double > > &params );
-
       // some information
-      bool ok ()
+      bool ok () const
       {
         return goodline;
       }
 
-      int nofsimplex ()
+      int offset () const
       {
-        return noflines();
+        return vtxoffset;
       }
 
     private:
-      // get the dimension of the grid
-      int getDimGrid ();
-      // get next simplex
-      bool next ( std :: vector< unsigned int > &simplex,
-                  std :: vector< double > &param );
+      // get dimworld
+      int getDimWorld ();
+
+      // get next vertex
+      bool next ( std :: vector< double > &point, std :: vector< double > &param );
     };
 
   } // end namespace dgf
 
 } // end namespace Dune
 
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplexgeneration.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplexgeneration.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/simplexgeneration.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/simplexgeneration.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/simplexgeneration.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_SIMPLEXGENERATIONBLOCK_HH
 #define DUNE_DGF_SIMPLEXGENERATIONBLOCK_HH
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/blocks/vertex.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/blocks/vertex.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/io/file/dgfparser/blocks/vertex.hh>
 
 namespace Dune
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfgeogrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfgeogrid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGFGEOGRID_HH
 #define DUNE_DGFGEOGRID_HH
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfgridfactory.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_GRIDFACTORY_HH
 #define DUNE_DGF_GRIDFACTORY_HH
 
 #include <iostream>
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfidentitygrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfidentitygrid.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGFPARSER_DGFIDENTITYGRID_HH
 #define DUNE_DGFPARSER_DGFIDENTITYGRID_HH
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfoned.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfoned.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_FILE_IO_DGFPARSER_DGFONED_HH
 #define DUNE_GRID_FILE_IO_DGFPARSER_DGFONED_HH
 
 //- C++ includes
 #include <algorithm>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfparser.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfparser.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <cstdio>
 #if HAVE_MKSTEMP
 #include <unistd.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfparser.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfparser.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_MACROGRIDPARSER_HH
 #define DUNE_MACROGRIDPARSER_HH
 
 #include <iostream>
 #include <fstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfug.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfug.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/geometry/utility/typefromvertexcount.hh>
 
 #include <dune/grid/io/file/dgfparser/dgfug.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfug.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfug.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_IO_FILE_DGFPARSER_DGFUG_HH
 #define DUNE_GRID_IO_FILE_DGFPARSER_DGFUG_HH
 
 //- C++ includes
 #include <fstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfwriter.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_IO_FILE_DGFPARSER_DGFWRITER_HH
 #define DUNE_GRID_IO_FILE_DGFPARSER_DGFWRITER_HH
 
 /** \file
  *  \brief write a GridView to a DGF file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/dgfyasp.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/dgfyasp.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGFPARSERYASP_HH
 #define DUNE_DGFPARSERYASP_HH
 
 #include <dune/grid/common/intersection.hh>
 #include <dune/grid/yaspgrid.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/entitykey.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/entitykey.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGFEnTITYKEY_HH
 #define DUNE_DGFEnTITYKEY_HH
 
 #include <iostream>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/entitykey_inline.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/entitykey_inline.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ENTITYKEY_INLINE_HH
 #define DUNE_ENTITYKEY_INLINE_HH
 
 #include <algorithm>
 #include <dune/geometry/referenceelements.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/gridptr.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/gridptr.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_GRIDPTR_HH
 #define DUNE_DGF_GRIDPTR_HH
 
 #include <cassert>
 #include <cctype>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/macrogrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/macrogrid.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_MACROGRID_HH
 #define DUNE_DGF_MACROGRID_HH
 
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/parser.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/parser.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_DGF_DUNEGRIDFORMATPARSER_HH
 #define DUNE_DGF_DUNEGRIDFORMATPARSER_HH
 
 #include <iostream>
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 dune_add_test(NAME test-dgf-yasp
               SOURCES test-dgf-yasp.cc
               LINK_LIBRARIES dunegrid
               COMPILE_DEFINITIONS DUNE_GRID_EXAMPLE_GRIDS_PATH=\"${PROJECT_SOURCE_DIR}/doc/grids/\"
              )
 
 dune_add_test(NAME test-dgf-yasp-offset
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/Orb_cut.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/Orb_cut.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/checkdgf.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/checkdgf.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_TEST_CHECKDGF_HH
 #define DUNE_GRID_TEST_CHECKDGF_HH
 
 #define CHECK 1
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/example-projection.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/example-projection.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10a.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10a.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10b.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10b.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10c.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10c.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid10s.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid10s.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid11a.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid11a.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid11b.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid11b.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid12_1.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid12_1.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid12_2.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid12_2.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1c.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1c.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1cs.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1cs.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1gen.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1gen.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1genangle.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1genangle.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid1s.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid1s.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2a.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2a.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2b.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2b.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2c.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2c.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2d.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2d.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid2e.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid2e.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid5c.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid5c.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid5s.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid5s.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid6c.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid6c.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid6s.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid6s.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid7.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7angle.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid7angle.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/examplegrid7area.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/examplegrid7area.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/pmdc.png` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/pmdc.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/test/test-dgf-alberta.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/test/test-dgf-yasp.cc`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
-#include <dune/grid/albertagrid.hh>
+#include <dune/grid/yaspgrid.hh>
 #include <dune/grid/io/file/dgfparser.hh>
+#include "../dgfyasp.hh"
 #include "checkdgf.hh"
 
 using namespace Dune;
 
 int main(int argc, char ** argv)
 try {
-  runDGFTest<AlbertaGrid<2>>(argc,argv);
+#ifdef TESTCOORDINATES
+  using Grid=YaspGrid<2,EquidistantOffsetCoordinates<double,2>>;
+#else
+  using Grid=YaspGrid<3>;
+#endif
+  runDGFTest<Grid>(argc,argv);
   return 0;
 }
 catch( const Dune::Exception &e )
 {
   std::cerr << e << std::endl;
   return 1;
 }
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/CMakeLists.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 set(GRIDTYPE ONEDGRID)
 set(GRIDDIM 1)
 
 set(EXTRA_PROGRAMS dgf2dgf gmsh2dgf)
 
 foreach(exe ${EXTRA_PROGRAMS})
   add_dgf_executable(${exe}  EXCLUDE_FROM_ALL ${exe}.cc)
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/dgf2dgf.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/dgf2dgf.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
  *  \author Matrin Nolte
  *  \brief a small program converting a DGF file into a DGF file
  *
  *  dgf2dgf is a small example program for the DGFWriter. It reads a DGF file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/dgfparser/utils/gmsh2dgf.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/dgfparser/utils/gmsh2dgf.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
  *  \author Matrin Nolte
  *  \brief a small program converting a gmsh file into a DGF file
  *
  *  gmsh2dgf is a small example program for the DGFWriter. It reads a gmsh file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/gmshreader.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/gmshreader.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GMSHREADER_HH
 #define DUNE_GMSHREADER_HH
 
 #include <cstdarg>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/gmshwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/gmshwriter.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_IO_FILE_GMSHWRITER_HH
 #define DUNE_GRID_IO_FILE_GMSHWRITER_HH
 
 #include <fstream>
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/gnuplot/gnuplot.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/gnuplot/gnuplot.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** @file
     @author Christian Engwer
     @brief Implementation of gnuplot output for 1D and 2D grids
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/gnuplot.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/gnuplot.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_IO_GNUPLOT_HH
 #define DUNE_IO_GNUPLOT_HH
 
 /** @file
     @author Christian Engwer
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/printgrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/printgrid.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PRINTGRID_HH
 #define DUNE_PRINTGRID_HH
 
 #include <fstream>
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/starcdreader.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/starcdreader.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_STARCD_READER_HH
 #define DUNE_STARCD_READER_HH
 
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 # TODO when porting this file to dune_add_test, the GMSH test needed to be adapted.
 # It previously relied on the flags added to the executable to switch different grid types.
 # I have adapted it quickly by adding a preprocesor variable. This could be and should
 # be done more nicely.
 #
 
 dune_add_test(SOURCES conformvolumevtktest.cc)
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/checkvtkfile.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/checkvtkfile.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_IO_FILE_TEST_CHECKVTKFILE_HH
 #define DUNE_GRID_IO_FILE_TEST_CHECKVTKFILE_HH
 
 #include <cstddef>
 #include <cstdlib>
 #include <iostream>
 #include <iomanip>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/conformvolumevtktest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/conformvolumevtktest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #if HAVE_CONFIG_H
 #include <config.h>
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/gmshtest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/gmshtest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include "config.h"
 
 #include <iostream>
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/gnuplottest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/gnuplottest.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 #include <iostream>
 #include <ostream>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/grid/io/file/gnuplot.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/nonconformboundaryvtktest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/nonconformboundaryvtktest.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #if HAVE_CONFIG_H
 #include "config.h"
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/printgridtest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/printgridtest.cc`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil -*-
 
 // Based on: Boilerplate tutorial poisson_uniform.cc
 
 #ifdef HAVE_CONFIG_H
 #include "config.h"
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/starcdreadertest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/starcdreadertest.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/subsamplingvtktest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/subsamplingvtktest.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #if HAVE_CONFIG_H
 #include "config.h" // autoconf defines, needed by the dune headers
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/vtksequencetest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/vtksequencetest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include "config.h"
 
 #include <memory>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/test/vtktest.cc` & `dune-grid-2.9.dev20220529/dune/grid/io/file/test/vtktest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #if HAVE_CONFIG_H
 #include "config.h" // autoconf defines, needed by the dune headers
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/b64enc.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/b64enc.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_B64ENC_HH
 #define DUNE_GRID_IO_FILE_VTK_B64ENC_HH
 
 #include <assert.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/basicwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/basicwriter.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_BASICWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_BASICWRITER_HH
 
 #include <fstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/boundaryiterators.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/boundaryiterators.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_BOUNDARYITERATORS_HH
 #define DUNE_GRID_IO_FILE_VTK_BOUNDARYITERATORS_HH
 
 #include <iterator>
@@ -168,15 +166,15 @@
       typedef VTK::Corner<Cell> Corner;
       typedef VTK::CornerIterator<CellIterator> CornerIterator;
 
       typedef Corner Point;
       typedef CornerIterator PointIterator;
 
       typedef NonConformingConnectivityWriter<Cell> ConnectivityWriter;
-      typedef typename GV::Communication Communication;
+      typedef typename GV::CollectiveCommunication CollectiveCommunication;
 
       explicit NonConformingBoundaryIteratorFactory(const GV& gv_)
         : gv(gv_)
       { }
 
       CellIterator beginCells() const {
         return CellIterator(gv);
@@ -194,15 +192,15 @@
 
       PointIterator beginPoints() const { return beginCorners(); }
       PointIterator endPoints() const { return endCorners(); }
 
       ConnectivityWriter makeConnectivity() const {
         return ConnectivityWriter();
       }
-      const Communication& comm() const {
+      const CollectiveCommunication& comm() const {
         return gv.comm();
       }
     };
 
   } // namespace VTK
 
   //! \} group VTK
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/boundarywriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/boundarywriter.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_BOUNDARYWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_BOUNDARYWRITER_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/common.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/common.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_COMMON_HH
 #define DUNE_GRID_IO_FILE_VTK_COMMON_HH
 
 #include <limits>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/corner.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/corner.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_CORNER_HH
 #define DUNE_GRID_IO_FILE_VTK_CORNER_HH
 
 #include <dune/grid/io/file/vtk/common.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/corneriterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/corneriterator.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_CORNERITERATOR_HH
 #define DUNE_GRID_IO_FILE_VTK_CORNERITERATOR_HH
 
 #include <iterator>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/dataarraywriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/dataarraywriter.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_DATAARRAYWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_DATAARRAYWRITER_HH
 
 #include <cstdint>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/function.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/function.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_FUNCTION_HH
 #define DUNE_GRID_IO_FILE_VTK_FUNCTION_HH
 
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/functionwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/functionwriter.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_FUNCTIONWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_FUNCTIONWRITER_HH
 
 #include <cstddef>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/pointiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/pointiterator.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_POINTITERATOR_HH
 #define DUNE_GRID_IO_FILE_VTK_POINTITERATOR_HH
 
 #include <iterator>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/pvtuwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/pvtuwriter.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_PVTUWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_PVTUWRITER_HH
 
 #include <ostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/skeletonfunction.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/skeletonfunction.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_SKELETONFUNCTION_HH
 #define DUNE_GRID_IO_FILE_VTK_SKELETONFUNCTION_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/streams.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/streams.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_STREAMS_HH
 #define DUNE_GRID_IO_FILE_VTK_STREAMS_HH
 
 #include <ostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/subsamplingvtkwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/subsamplingvtkwriter.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_SUBSAMPLINGVTKWRITER_HH
 #define DUNE_SUBSAMPLINGVTKWRITER_HH
 
 #include <ostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/volumeiterators.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/volumeiterators.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_VOLUMEITERATORS_HH
 #define DUNE_GRID_IO_FILE_VTK_VOLUMEITERATORS_HH
 
 #include <dune/grid/common/gridenums.hh>
@@ -40,15 +38,15 @@
 
       typedef VTK::Corner<Cell> Point;
       typedef VTK::PointIterator<CellIterator,
           typename GV::IndexSet> PointIterator;
 
       typedef ConformingConnectivityWriter<ConformingVolumeIteratorFactory<GV>
           > ConnectivityWriter;
-      typedef typename GV::Communication Communication;
+      typedef typename GV::CollectiveCommunication CollectiveCommunication;
 
       explicit ConformingVolumeIteratorFactory(const GV& gv_)
         : gv(gv_)
       { }
 
       CellIterator beginCells() const {
         return gv.template begin<0, InteriorBorder_Partition>();
@@ -70,15 +68,15 @@
       PointIterator endPoints() const {
         return PointIterator(endCells());
       }
 
       ConnectivityWriter makeConnectivity() const {
         return ConnectivityWriter(*this);
       }
-      const Communication& comm() const {
+      const CollectiveCommunication& comm() const {
         return gv.comm();
       }
     };
 
     template<typename GV>
     class NonConformingVolumeIteratorFactory {
       const GV& gv;
@@ -93,15 +91,15 @@
       typedef VTK::Corner<Cell> Corner;
       typedef VTK::CornerIterator<CellIterator> CornerIterator;
 
       typedef Corner Point;
       typedef CornerIterator PointIterator;
 
       typedef NonConformingConnectivityWriter<Cell> ConnectivityWriter;
-      typedef typename GV::Communication Communication;
+      typedef typename GV::CollectiveCommunication CollectiveCommunication;
 
       explicit NonConformingVolumeIteratorFactory(const GV& gv_)
         : gv(gv_)
       { }
 
       CellIterator beginCells() const {
         return gv.template begin<0, InteriorBorder_Partition>();
@@ -119,15 +117,15 @@
 
       PointIterator beginPoints() const { return beginCorners(); }
       PointIterator endPoints() const { return endCorners(); }
 
       ConnectivityWriter makeConnectivity() const {
         return ConnectivityWriter();
       }
-      const Communication& comm() const {
+      const CollectiveCommunication& comm() const {
         return gv.comm();
       }
     };
 
   } // namespace VTK
 
   //! \} group VTK
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/volumewriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/volumewriter.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_VOLUMEWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_VOLUMEWRITER_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtksequencewriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtksequencewriter.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_VTKSEQUENCE_HH
 #define DUNE_VTKSEQUENCE_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtksequencewriterbase.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtksequencewriterbase.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_VTKSEQUENCEWRITERBASE_HH
 #define DUNE_GRID_IO_FILE_VTK_VTKSEQUENCEWRITERBASE_HH
 
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtkwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtkwriter.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_VTKWRITER_HH
 #define DUNE_VTKWRITER_HH
 
 #include <cstring>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/io/file/vtk/vtuwriter.hh` & `dune-grid-2.9.dev20220529/dune/grid/io/file/vtk/vtuwriter.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_IO_FILE_VTK_VTUWRITER_HH
 #define DUNE_GRID_IO_FILE_VTK_VTUWRITER_HH
 
 #include <ostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/modules.txt` & `dune-grid-2.9.dev20220529/dune/grid/modules.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 // -*- tab-width: 4; indent-tabs-mode: nil -*-
-// SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /* This file determines the order how things appear in the doxygen
    documentation within the Grid group. It works like this:
 
    @defgroup commands appear only in this file here which is
-   parsed before the other files (because it is mentioned first
+   parsed before the other files (because it is mentioned first 
    in the Doxyfile).
 
    Only @addtogroup is used in the code documentation.
 */
 
   /**
 	 @defgroup GridInterface The Grid Interface
@@ -18,27 +16,27 @@
   */
   /** @defgroup GIRelatedTypes Related types and enumerations
       @ingroup GridInterface */
   /** @defgroup GIGrid Grid Abstract Base Class
       @ingroup GridInterface */
   /** @defgroup GIGridView GridView
       @ingroup GridInterface */
-  /** @defgroup GIEntity Entity
+  /** @defgroup GIEntity Entity 
       @ingroup GridInterface */
   /** @defgroup GIGeometry Geometry
       @ingroup GridInterface */
   /** @defgroup GIEntityPointer EntityIterators
       @ingroup GridInterface */
   /** @defgroup GIIntersectionIterator Intersections
       @ingroup GridInterface */
   /** @defgroup GIIteration Iterating over grid entities and intersections
       @ingroup GridInterface */
   /** @defgroup IndexIdSets IndexSet and IdSet
 	  @ingroup GridInterface */
-  /** @defgroup GICommunication Communication
+  /** @defgroup GICollectiveCommunication CollectiveCommunication
       @ingroup GridInterface */
   /** @defgroup GIMiscellaneous Miscellaneous
 	  @ingroup GridInterface */
   /** @defgroup GICapabilities Capabilities
 	  @ingroup GridInterface */
 
   /**
@@ -54,18 +52,18 @@
 
   /** \defgroup GeoGrid GeometryGrid
     \ingroup GridImplementations */
 
   /** \defgroup IdentityGrid IdentityGrid
     \ingroup GridImplementations */
 
-	/** @defgroup OneDGrid OneDGrid
+	/** @defgroup OneDGrid OneDGrid 
 		@ingroup GridImplementations */
 
-	/** @defgroup UGGrid UGGrid
+	/** @defgroup UGGrid UGGrid 
 		@ingroup GridImplementations */
 
 	/** @defgroup YaspGrid YaspGrid
 		@ingroup GridImplementations */
 
 	/** @defgroup AlbertaGrid AlbertaGrid
 		@ingroup GridImplementations */
@@ -78,34 +76,34 @@
 	        @ingroup IO
                 @brief An interface for the creation of macro grids, for use by grid file readers etc.
           */
 
         /** @defgroup DuneGridFormatParser The Dune Grid Format (DGF)
             @ingroup IO */
 
-        /** @defgroup DGFGridParameter DGF grid parameter for different grids
+        /** @defgroup DGFGridParameter DGF grid parameter for different grids 
             @ingroup DuneGridFormatParser */
 
         /** @defgroup VTK Visualization ToolKit (VTK)
             @ingroup IO */
-
+        
         /** @defgroup Gnuplot Gnuplot
             @ingroup IO */
 
         /** @defgroup Gmsh Gmsh grid format
             @ingroup IO */
 
         /** @defgroup StarCD StarCD
             @ingroup IO */
 
   /*
      @defgroup GridPart Grid Parts
      @ingroup Grid
   */
-
+  
   /**
 	 @defgroup GridDevel Grid Developer API
 	 @ingroup Grid
         @brief Interfaces needed to implement a new \ref Grid "Dune::Grid"
 
         For help implementing the geometries of your grid, have a look at \ref
         GenericGeometry from \ref dune-geometry.
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/nulliteratorfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/nulliteratorfactory.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONEDGRID_NULL_ITERATORS_HH
 #define DUNE_ONEDGRID_NULL_ITERATORS_HH
 
 #include "onedgridlist.hh"
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgrid.cc` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgrid.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include "../onedgrid.hh"
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridentity.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridentity.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_ENTITY_HH
 #define DUNE_ONE_D_GRID_ENTITY_HH
 
 #include <array>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridentityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridentityseed.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
-#ifndef DUNE_ONE_D_GRID_ENTITY_SEED_HH
-#define DUNE_ONE_D_GRID_ENTITY_SEED_HH
-
-#include "onedgridentity.hh"
+#ifndef DUNE_UGGRID_ENTITY_SEED_HH
+#define DUNE_UGGRID_ENTITY_SEED_HH
 
 /** \file
- *  \brief Implementation of EntitySeed for the OneDGrid grid manager
+ *  \brief Implementation of EntitySeed for the UGGrid grid manager
  */
 
 namespace Dune {
 
-  /** \brief Store a reference to an entity with a minimal memory footprint
+  /** \brief Store a reference to an entity with a minimal memory footprint (one pointer)
    */
   template<int codim, class GridImp>
-  class OneDGridEntitySeed
+  class UGGridEntitySeed
   {
     // grid dimension
     constexpr static int dim = GridImp::dimension;
   public:
 
+    //! codimension of underlying entity
     constexpr static int codimension = codim;
 
     //! default construct an invalid entity seed
-    OneDGridEntitySeed ()
+    UGGridEntitySeed ()
       : target_(nullptr)
     {}
 
     //! construct entity seed from entity
-    OneDGridEntitySeed (const OneDGridEntity<codim,dim,GridImp>& entity)
-      : target_(entity.target_)
+    UGGridEntitySeed (const UGGridEntity<codim,dim,GridImp>& entity)
+      : target_(entity.getTarget())
     {}
 
     //! check whether the EntitySeed refers to a valid Entity
     bool isValid() const
     {
       return target_ != nullptr;
     }
 
-    /** \brief Access to the underlying OneDGrid data structure */
-    OneDEntityImp<dim-codim>* target() const
+    /** \brief Access to the underlying UG data structure */
+    typename UG_NS<dim>::template Entity<codim>::T* target() const
     {
       return target_;
     }
 
   private:
-    /** \brief Plain old pointer to the corresponding OneDGrid data structure */
-    OneDEntityImp<dim-codim>* target_;
+    /** \brief Plain old pointer to the corresponding UG data structure */
+    typename UG_NS<dim>::template Entity<codim>::T* target_;
   };
 
 } // end namespace Dune
 
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridfactory.cc` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridfactory.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <dune/grid/onedgrid/onedgridfactory.hh>
 #include <dune/grid/onedgrid/onedgridindexsets.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridfactory.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_ONEDGRID_FACTORY_HH
 #define DUNE_ONEDGRID_FACTORY_HH
 
 /** \file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridhieriterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridhieriterator.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_HIERITERATOR_HH
 #define DUNE_ONE_D_GRID_HIERITERATOR_HH
 
 /** \file
  * \brief The OneDGridHierarchicIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridindexsets.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridindexsets.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONEDGRID_INDEXSETS_HH
 #define DUNE_ONEDGRID_INDEXSETS_HH
 
 /** \file
     \brief The index and id sets for the OneDGrid class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridintersectioniterators.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridintersectioniterators.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_INTERSECTION_ITERATORS_HH
 #define DUNE_ONE_D_GRID_INTERSECTION_ITERATORS_HH
 
 /** \file
  * \brief The OneDGridLevelIntersectionIterator and OneDGridLeafIntersectionIterator classes
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridintersections.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridintersections.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_INTERSECTIONS_HH
 #define DUNE_ONE_D_GRID_INTERSECTIONS_HH
 
 /** \file
  * \brief The OneDGridLevelIntersection and OneDGridLeafIntersection classes
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridleafiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridleafiterator.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_LEAFITERATOR_HH
 #define DUNE_ONE_D_GRID_LEAFITERATOR_HH
 
 /** \file
  * \brief The OneDGridLeafIterator class
@@ -34,15 +32,15 @@
       this->virtualEntity_.impl().setToTarget((OneDEntityImp<1-codim>*) std::get<1-codim>(grid_->entityImps_[fullRefineLevel]).begin());
 
       if (!this->virtualEntity_.impl().target_->isLeaf())
         increment();
     }
 
     //! Constructor
-    OneDGridLeafIterator() : grid_(nullptr)
+    OneDGridLeafIterator()
     {
       this->virtualEntity_.impl().setToTarget(OneDGridNullIteratorFactory<1-codim>::null());
     }
 
     //! prefix increment
     void increment() {
       // Increment until you find a leaf entity
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridleveliterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridleveliterator.hh`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_LEVELITERATOR_HH
 #define DUNE_ONE_D_GRID_LEVELITERATOR_HH
 
 /** \file
  * \brief The OneDGridLevelIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridlist.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridlist.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONEDGRID_LIST_HH
 #define DUNE_ONEDGRID_LIST_HH
 
 #include <dune/common/iteratorfacades.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid/onedgridviews.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid/onedgridviews.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_ONEDGRID_ONEDGRIDVIEWS_HH
 #define DUNE_GRID_ONEDGRID_ONEDGRIDVIEWS_HH
 
 #include <type_traits>
 #include <tuple>
@@ -43,20 +41,16 @@
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LevelIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LevelIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid :: Traits
       :: template Codim< cd > :: template Partition< All_Partition > :: LevelIterator
       Iterator;
@@ -96,20 +90,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     constexpr static bool conforming = Traits :: conforming;
 
@@ -184,16 +174,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return entity.impl().ilevelend();
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize([[maybe_unused]] int codim) const
     {
@@ -233,20 +223,16 @@
 
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LeafIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LeafIntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid :: Traits
       :: template Codim< cd > :: template Partition< All_Partition > :: LeafIterator
       Iterator;
@@ -285,20 +271,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits :: Communication Communication;
-
-    /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     constexpr static bool conforming = Traits :: conforming;
 
@@ -373,16 +355,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return entity.impl().ileafend();
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize([[maybe_unused]] int codim) const
     {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/onedgrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/onedgrid.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ONE_D_GRID_HH
 #define DUNE_ONE_D_GRID_HH
 
 #include <tuple>
 #include <vector>
@@ -293,15 +291,15 @@
      * \param refCount I don't know what this is good for.  It doesn't
      *        actually do anything.
      */
     void globalRefine(int refCount);
 
     // dummy parallel functions
 
-    const Communication &comm () const
+    const CollectiveCommunication &comm () const
     {
       return ccobj;
     }
 
 
   private:
 
@@ -321,15 +319,15 @@
     }
 
     /** \brief Get element lists directly -- makes the code more readable */
     const OneDGridList<OneDEntityImp<1> >& elements(int level) const {
       return std::get<1>(entityImps_[level]);
     }
 
-    Communication ccobj;
+    CollectiveCommunication ccobj;
 
     /** \brief Update all indices and ids */
     void setIndices();
 
     /** \brief Produce an entity id that has not been used in this grid before.
      */
     unsigned int getNextFreeId()
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/test/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 add_subdirectory(yasp)
 
 dune_add_test(SOURCES geometrygrid-coordfunction-copyconstructor.cc)
 
 dune_add_test(NAME test-geogrid-yaspgrid
               SOURCES test-geogrid.cc
               LINK_LIBRARIES dunegrid
@@ -33,20 +30,19 @@
 
 dune_add_test(SOURCES testiteratorranges.cc)
 
 dune_add_test(SOURCES test-hierarchicsearch.cc)
 
 dune_add_test(SOURCES test-ug.cc
               LINK_LIBRARIES dunegrid
-              COMPILE_DEFINITIONS DUNE_GRID_EXAMPLE_GRIDS_PATH=\"${PROJECT_SOURCE_DIR}/doc/grids/\"
               CMAKE_GUARD dune-uggrid_FOUND)
 
 dune_add_test(SOURCES test-parallel-ug.cc
               LINK_LIBRARIES dunegrid
-              CMAKE_GUARD dune-uggrid_FOUND
+              CMAKE_GUARD "dune-uggrid_FOUND AND MPI_FOUND"
               MPI_RANKS 1 2 3 4 8
               TIMEOUT 300)
 
 dune_add_test(SOURCES test-loadbalancing.cc
               LINK_LIBRARIES dunegrid
               CMAKE_GUARD dune-uggrid_FOUND)
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/basicunitcube.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/basicunitcube.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef  BASICUNITCUBE_HH
 #define  BASICUNITCUBE_HH
 
 // StructuredGridFactory cannot replace BasicUnitCube when creating a projected unit cube in test-alberta.cc
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/check-albertareader.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/check-albertareader.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECK_ALBERTAREADER_HH
 #define DUNE_GRID_TEST_CHECK_ALBERTAREADER_HH
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkadaptation.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkadaptation.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKADAPTATION_HH
 #define DUNE_GRID_TEST_CHECKADAPTATION_HH
 
 #include <dune/common/typetraits.hh>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkcomcorrectness.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkcomcorrectness.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKCOMMCORRECTNESS_HH
 #define DUNE_GRID_TEST_CHECKCOMMCORRECTNESS_HH
 
 #include <config.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkcommunicate.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkcommunicate.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKCOMMUNICATE_HH
 #define DUNE_GRID_TEST_CHECKCOMMUNICATE_HH
 
 #include <iostream>
 #include <fstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkentitylifetime.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkentitylifetime.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKENTITYLIFETIME_HH
 #define DUNE_GRID_TEST_CHECKENTITYLIFETIME_HH
 
 /** \file
     \brief Tests that make sure range-based entity iteration works correctly
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkentityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkentityseed.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_CHECK_ENTITYSEED_HH
 #define DUNE_GRID_CHECK_ENTITYSEED_HH
 
 //- C++ includes
 #include <cassert>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkgeometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkgeometry.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_TEST_CHECKGEOMETRY_HH
 #define DUNE_GRID_TEST_CHECKGEOMETRY_HH
 
 #include <limits>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkgeometryinfather.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkgeometryinfather.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKGEOMETRYINFATHER_HH
 #define DUNE_GRID_TEST_CHECKGEOMETRYINFATHER_HH
 
 #include <dune/common/typetraits.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkgridfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_TEST_CHECKGRIDFACTORY_HH
 #define DUNE_GRID_TEST_CHECKGRIDFACTORY_HH
 
 #include <algorithm>
 #include <memory>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkidset.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkidset.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKIDSET_HH
 #define DUNE_GRID_TEST_CHECKIDSET_HH
 
 #include <iostream>
 #include <map>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkindexset.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkindexset.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKINDEXSET_HH
 #define DUNE_GRID_TEST_CHECKINDEXSET_HH
 
 #include <algorithm>
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkintersectionit.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkintersectionit.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKINTERSECTIONIT_HH
 #define DUNE_GRID_TEST_CHECKINTERSECTIONIT_HH
 
 #include <cmath>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkintersectionlifetime.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkintersectionlifetime.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKINTERSECTIONLIFETIME_HH
 #define DUNE_GRID_TEST_CHECKINTERSECTIONLIFETIME_HH
 
 /** \file
     \brief Tests that make sure range-based intersection iteration works correctly
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkiterators.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkiterators.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKITERATORS_HH
 #define DUNE_GRID_TEST_CHECKITERATORS_HH
 
 #include <iostream>
 #include <map>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkjacobians.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkjacobians.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKJACOBIANS_HH
 #define DUNE_GRID_TEST_CHECKJACOBIANS_HH
 
 #include <dune/common/dynvector.hh>
 #include <dune/common/exceptions.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checkpartition.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checkpartition.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_TEST_CHECKPARTITION_HH
 #define DUNE_GRID_TEST_CHECKPARTITION_HH
 
 #include <cstddef>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/checktwists.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/checktwists.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_CHECKTWISTS_HH
 #define DUNE_GRID_TEST_CHECKTWISTS_HH
 
 #include <dune/geometry/referenceelements.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/functions.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/functions.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GEOGRID_TEST_FUNCTIONS_HH
 #define DUNE_GEOGRID_TEST_FUNCTIONS_HH
 
 #include <dune/grid/geometrygrid/coordfunction.hh>
 #include <dune/grid/geometrygrid/identity.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/geometrygrid-coordfunction-copyconstructor.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/geometrygrid-coordfunction-copyconstructor.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 /*
  * Test that an implicit copy generator is available for classes derived from
  * - Dune::AnalyticalCoordFunction
  * - Dune::DiscreteCoordFunction
  *
  * See https://gitlab.dune-project.org/flyspray/FS/issues/1463
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/gridcheck.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/gridcheck.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_GRIDCHECK_HH
 #define DUNE_GRID_TEST_GRIDCHECK_HH
 
 /** \file
     \brief Implements a generic grid check
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/issue-53-uggrid-intersections.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/issue-53-uggrid-intersections.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 /*
  * Check leaf intersection geometry on UGGrid.
  *
  * Reference: https://gitlab.dune-project.org/core/dune-grid/issues/53
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/staticcheck.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/staticcheck.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_STATICCHECK_HH
 #define DUNE_GRID_TEST_STATICCHECK_HH
 
 /** \file
     \brief Implements static grid checks
@@ -39,16 +37,14 @@
     typename Geometry::LocalCoordinate v(0.0);
     geo.global(v);
     typename Geometry::GlobalCoordinate g(0.0);
     geo.local(g);
     geo.integrationElement(v);
     geo.jacobianTransposed( v );
     geo.jacobianInverseTransposed( v );
-    geo.jacobian( v );
-    geo.jacobianInverse( v );
   }
 
   GeometryInterface ()
   {
     c = check;
   }
 
@@ -452,15 +448,15 @@
     }
 
     IntersectionIteratorInterface< Grid, IntersectionIterator >();
 
     // parallel interface
     using GhostIterator [[maybe_unused]] = typename GridView::template Codim< 0 >::template
       Partition< Dune::Ghost_Partition >::Iterator;
-    using Communication [[maybe_unused]] = typename GridView::Communication;
+    using CollectiveCommunication [[maybe_unused]] = typename GridView::CollectiveCommunication;
 
     gv.template begin< 0, Dune::Ghost_Partition >();
     gv.template end< 0, Dune::Ghost_Partition >();
 
     gv.overlapSize( 0 );
     gv.ghostSize( 0 );
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-alberta.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-alberta.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <iostream>
 #include <sstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-geogrid.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-geogrid.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifdef HAVE_CONFIG_H
 #include <config.h>
 #endif
 
 #ifdef COORDFUNCTION
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-hierarchicsearch.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-hierarchicsearch.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include <config.h>
 
 #include <cstdlib>
 
 #include <array>
 #include <iostream>
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-identitygrid.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-identitygrid.cc`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifdef HAVE_CONFIG_H
 #include <config.h>
 #endif
 
 #include <dune/grid/yaspgrid.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-loadbalancing.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-loadbalancing.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifdef HAVE_CONFIG_H
 # include "config.h"
 #endif
 #include <iostream>
 
 #include <dune/grid/io/file/vtk/vtkwriter.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-mcmg-geogrid.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-mcmg-geogrid.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/common/fvector.hh>
 #include <dune/common/parallel/mpihelper.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-oned.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-oned.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <vector>
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-parallel-ug.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-parallel-ug.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 // Test parallel interface if a parallel UG is used
 
 #include <config.h>
 
 #include <unistd.h>
@@ -11,15 +9,14 @@
 #include <iomanip>
 #include <memory>
 #include <vector>
 #include <bitset>
 
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/float_cmp.hh>
-#include <dune/common/stdstreams.hh>
 #include <dune/geometry/referenceelements.hh>
 #include <dune/grid/common/gridenums.hh>
 #include <dune/grid/common/mcmgmapper.hh>
 #include <dune/grid/uggrid.hh>
 #include <dune/grid/utility/structuredgridfactory.hh>
 
 using namespace Dune;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/test-ug.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/test-ug.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <memory>
 
 #include <dune/common/parallel/mpihelper.hh>
 
 /*
    Instantiate UG-Grid and feed it to the generic gridcheck()
  */
 #include <dune/grid/uggrid.hh>
-#include <dune/grid/io/file/gmshreader.hh>
 #include <doc/grids/gridfactory/hybridtestgrids.hh>
 
 #include "gridcheck.hh"
 #include "checkcommunicate.hh"
 #include "checkgeometryinfather.hh"
 #include "checkintersectionit.hh"
 #include "checkpartition.hh"
@@ -109,58 +106,14 @@
   // the GridFactory can reuse an existing UGGrid object, and I would like to keep
   // that for the time being.
   factory.createGrid().release();
 
 }
 
 
-// compute boundary length of a given mesh
-double integrateBoundary(const Dune::UGGrid<2>& grid)
-{
-  double len = 0.0;
-  auto && gv = grid.leafGridView();
-  for (const auto& e : elements(gv))
-  {
-    for (const auto& i : intersections(gv,e))
-    {
-      if (i.boundary())
-        len += i.geometry().volume();
-    }
-  }
-  return len;
-}
-
-
-// test approximation to a curved boundary: refine, compare with the
-// exact length and check the expected 2nd order convergence rate
-void testGeometryApproximation(Dune::UGGrid<2>& grid, double exact, bool verbose = false)
-{
-    double len = integrateBoundary(grid);
-    if (verbose)
-      std::cout << "boundary length: " << len << "\t" << exact << std::endl;
-    double eoc = 0.0;
-    for (unsigned int l = 0; l < 5; l++)
-    {
-      grid.globalRefine(1);
-      double len_refined = integrateBoundary(grid);
-      double err0 = std::abs(len-exact);
-      double err  = std::abs(len_refined-exact);
-      eoc  = std::log2(err0/err); // h0/h = 2
-      if (verbose)
-        std::cout << "boundary length: " << len_refined
-                  << "\t" << exact
-                  << "\terr=" << err
-                  << "\teoc=" << eoc << std::endl;
-      len = len_refined;
-    }
-    // we expect 2nd order convergence
-    if (Dune::FloatCmp::ne(eoc,2.0,0.02))
-      DUNE_THROW(Dune::GridError, "Geometry approximation does not show expected 2nd order convergence");
-}
-
 template <class GridType >
 void markOne ( GridType & grid , int num , int ref )
 {
   int count = 0;
 
   for(const auto& element : elements(grid.leafGridView()))
   {
@@ -330,57 +283,14 @@
         DUNE_THROW(Dune::GridError, "output of geometryInFather() depends on boundary parametrization!");
 
     }
 
   }
 
   // ////////////////////////////////////////////////////////////////////////
-  //   Check refinement to boundary (exact circle geometry).
-  //   Upon refinement new vertices should be moved towards the exact geomtry,
-  //   so that the boundary is better resolved
-  // ////////////////////////////////////////////////////////////////////////
-  {
-    // geometry is a half circle with radius 15, so the exact length
-    // of the boundary is $`R \cdot \pi + 2 R`$
-    double exact = (M_PI + 2.0) * 15.0;
-    testGeometryApproximation(gridWithParametrization, exact);
-  }
-
-  // ////////////////////////////////////////////////////////////////////////
-  //   Check refinement to boundary (quadratic gmsh boundary)
-  //   upon refinement new vertices should be moved towards the exact geomtry,
-  //   so that the boundary is better resolved
-  // ////////////////////////////////////////////////////////////////////////
-  {
-    Dune::GridFactory<Dune::UGGrid<2>> gridFactory;
-    const std::string path(DUNE_GRID_EXAMPLE_GRIDS_PATH);
-    const std::string inputName(path+"gmsh/circle2ndorder.msh");
-    std::cout << "Reading mesh file " << inputName << std::endl;
-    auto reader = Dune::GmshReader<Dune::UGGrid<2>>(inputName, gridFactory);
-    auto gmshgrid = gridFactory.createGrid();
-    // 1/6 of a circle as 2nd order polynomial:
-    /* the following python code can be used to compute the exact solution below:
-         import sympy
-         from sympy import *
-         tau = sympy.symbols('τ')
-         N = 6 # segments
-         t = [0, pi/N, 2*pi/N]
-         x = list(map(sin, t))
-         y = list(map(cos, t))
-         px  = interpolate(list(zip(t,x)),tau)
-         py  = interpolate(list(zip(t,y)),tau)
-         V = simplify(sqrt(diff(px,tau)**2+diff(py,tau)**2)) # det(J)
-         len = N * integrate(V, (tau,0,t[-1]))
-         print(simplify(len), " = ", len.evalf())
-     */
-    double exact = 6.27593206157460;
-    testGeometryApproximation(*gmshgrid, exact);
-  }
-
-  // ////////////////////////////////////////////////////////////////////////
   //   Check whether copies of elements have the same global ID
   // ////////////////////////////////////////////////////////////////////////
 
   {
     std::cout << "Testing if copies of elements have the same id." << std::endl;
     Dune::UGGrid<2> locallyRefinedGrid;
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/testiteratorranges.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/testiteratorranges.cc`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistant.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistantoffset.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
@@ -18,23 +16,23 @@
 
 int main (int argc , char **argv) {
   try {
     // Initialize MPI, if present
     const auto & mpiHelper = Dune::MPIHelper::instance(argc, argv);
 
     std::string testID =
-      "backuprestore-equidistant-np" + std::to_string(mpiHelper.size());
+      "backuprestore-equidistantoffset-np" + std::to_string(mpiHelper.size());
 
     // check the backup restore facility
     check_backuprestore(testID,
-                        YaspFactory<2,Dune::EquidistantCoordinates<double,2> >::buildGrid());
+                        YaspFactory<2,Dune::EquidistantOffsetCoordinates<double,2> >::buildGrid());
 
     // Test again with refinement
     check_backuprestore(testID + "-ref",
-                        YaspFactory<2,Dune::EquidistantCoordinates<double,2> >::buildGrid(true, 1));
+                        YaspFactory<2,Dune::EquidistantOffsetCoordinates<double,2> >::buildGrid(true, 1));
 
   } catch (Dune::Exception &e) {
     std::cerr << e << std::endl;
     return 1;
   } catch (...) {
     std::cerr << "Generic exception!" << std::endl;
     return 2;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistantoffset.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-backuprestore-tensor.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
@@ -18,23 +16,23 @@
 
 int main (int argc , char **argv) {
   try {
     // Initialize MPI, if present
     const auto & mpiHelper = Dune::MPIHelper::instance(argc, argv);
 
     std::string testID =
-      "backuprestore-equidistantoffset-np" + std::to_string(mpiHelper.size());
+      "backuprestore-tensor-np" + std::to_string(mpiHelper.size());
 
     // check the backup restore facility
     check_backuprestore(testID,
-                        YaspFactory<2,Dune::EquidistantOffsetCoordinates<double,2> >::buildGrid());
+                        YaspFactory<2,Dune::TensorProductCoordinates<double,2> >::buildGrid());
 
     // Test again with refinement
     check_backuprestore(testID + "-ref",
-                        YaspFactory<2,Dune::EquidistantOffsetCoordinates<double,2> >::buildGrid(true, 1));
+                        YaspFactory<2,Dune::TensorProductCoordinates<double,2> >::buildGrid(true, 1));
 
   } catch (Dune::Exception &e) {
     std::cerr << e << std::endl;
     return 1;
   } catch (...) {
     std::cerr << "Generic exception!" << std::endl;
     return 2;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-backuprestore-tensor.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistant.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
@@ -18,23 +16,23 @@
 
 int main (int argc , char **argv) {
   try {
     // Initialize MPI, if present
     const auto & mpiHelper = Dune::MPIHelper::instance(argc, argv);
 
     std::string testID =
-      "backuprestore-tensor-np" + std::to_string(mpiHelper.size());
+      "backuprestore-equidistant-np" + std::to_string(mpiHelper.size());
 
     // check the backup restore facility
     check_backuprestore(testID,
-                        YaspFactory<2,Dune::TensorProductCoordinates<double,2> >::buildGrid());
+                        YaspFactory<2,Dune::EquidistantCoordinates<double,2> >::buildGrid());
 
     // Test again with refinement
     check_backuprestore(testID + "-ref",
-                        YaspFactory<2,Dune::TensorProductCoordinates<double,2> >::buildGrid(true, 1));
+                        YaspFactory<2,Dune::EquidistantCoordinates<double,2> >::buildGrid(true, 1));
 
   } catch (Dune::Exception &e) {
     std::cerr << e << std::endl;
     return 1;
   } catch (...) {
     std::cerr << "Generic exception!" << std::endl;
     return 2;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-constructor.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-constructor.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <dune/common/parallel/mpihelper.hh>
 #include <dune/common/fvector.hh>
 #include <dune/grid/yaspgrid.hh>
 
 #include <array>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-entityshifttable.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-entityshifttable.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #include "config.h"
 
 #include <iostream>
 
 #include <dune/common/deprecated.hh>
 #include <dune/common/test/testsuite.hh>
 #include <dune/grid/yaspgrid.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-tensorgridfactory.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-tensorgridfactory.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-yaspfactory-1d.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-yaspfactory-3d.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
@@ -18,29 +16,30 @@
 
 int main (int argc , char **argv) {
   try {
     // Initialize MPI, if present
     const auto & mpiHelper = Dune::MPIHelper::instance(argc, argv);
 
     std::string testID =
-      "yaspfactory-1d-np" + std::to_string(mpiHelper.size());
+      "yaspfactory-3d-np" + std::to_string(mpiHelper.size());
 
     check_yasp(testID + "equidistant",
-               YaspFactory<1,Dune::EquidistantCoordinates<double,1> >::buildGrid());
+               YaspFactory<3,Dune::EquidistantCoordinates<double,3> >::buildGrid());
     check_yasp(testID + "equidistantoffset",
-               YaspFactory<1,Dune::EquidistantOffsetCoordinates<double,1> >::buildGrid());
+               YaspFactory<3,Dune::EquidistantOffsetCoordinates<double,3> >::buildGrid());
     check_yasp(testID + "tensor",
-               YaspFactory<1,Dune::TensorProductCoordinates<double,1> >::buildGrid());
+               YaspFactory<3,Dune::TensorProductCoordinates<double,3> >::buildGrid());
 
+    // Test the generic constructor
     check_yasp(testID + "equidistant-generic-constructor",
-               YaspFactory<1,Dune::EquidistantCoordinates<double,1> >::buildGrid(true,0,false,true));
+               YaspFactory<3,Dune::EquidistantCoordinates<double,3> >::buildGrid(true,0,false,true));
     check_yasp(testID + "equidistantoffset-generic-constructor",
-               YaspFactory<1,Dune::EquidistantOffsetCoordinates<double,1> >::buildGrid(true,0,false,true));
+               YaspFactory<3,Dune::EquidistantOffsetCoordinates<double,3> >::buildGrid(true,0,false,true));
     check_yasp(testID + "tensor-generic-constructor",
-               YaspFactory<1,Dune::TensorProductCoordinates<double,1> >::buildGrid(true,0,false,true));
+               YaspFactory<3,Dune::TensorProductCoordinates<double,3> >::buildGrid(true,0,false,true));
 
   } catch (Dune::Exception &e) {
     std::cerr << e << std::endl;
     return 1;
   } catch (...) {
     std::cerr << "Generic exception!" << std::endl;
     return 2;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-yaspfactory-2d.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-yaspfactory-2d.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid-yaspfactory-3d.cc` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid-yaspfactory-1d.cc`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <iostream>
 #include <fstream>
@@ -18,30 +16,29 @@
 
 int main (int argc , char **argv) {
   try {
     // Initialize MPI, if present
     const auto & mpiHelper = Dune::MPIHelper::instance(argc, argv);
 
     std::string testID =
-      "yaspfactory-3d-np" + std::to_string(mpiHelper.size());
+      "yaspfactory-1d-np" + std::to_string(mpiHelper.size());
 
     check_yasp(testID + "equidistant",
-               YaspFactory<3,Dune::EquidistantCoordinates<double,3> >::buildGrid());
+               YaspFactory<1,Dune::EquidistantCoordinates<double,1> >::buildGrid());
     check_yasp(testID + "equidistantoffset",
-               YaspFactory<3,Dune::EquidistantOffsetCoordinates<double,3> >::buildGrid());
+               YaspFactory<1,Dune::EquidistantOffsetCoordinates<double,1> >::buildGrid());
     check_yasp(testID + "tensor",
-               YaspFactory<3,Dune::TensorProductCoordinates<double,3> >::buildGrid());
+               YaspFactory<1,Dune::TensorProductCoordinates<double,1> >::buildGrid());
 
-    // Test the generic constructor
     check_yasp(testID + "equidistant-generic-constructor",
-               YaspFactory<3,Dune::EquidistantCoordinates<double,3> >::buildGrid(true,0,false,true));
+               YaspFactory<1,Dune::EquidistantCoordinates<double,1> >::buildGrid(true,0,false,true));
     check_yasp(testID + "equidistantoffset-generic-constructor",
-               YaspFactory<3,Dune::EquidistantOffsetCoordinates<double,3> >::buildGrid(true,0,false,true));
+               YaspFactory<1,Dune::EquidistantOffsetCoordinates<double,1> >::buildGrid(true,0,false,true));
     check_yasp(testID + "tensor-generic-constructor",
-               YaspFactory<3,Dune::TensorProductCoordinates<double,3> >::buildGrid(true,0,false,true));
+               YaspFactory<1,Dune::TensorProductCoordinates<double,1> >::buildGrid(true,0,false,true));
 
   } catch (Dune::Exception &e) {
     std::cerr << e << std::endl;
     return 1;
   } catch (...) {
     std::cerr << "Generic exception!" << std::endl;
     return 2;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/test/yasp/test-yaspgrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/test/yasp/test-yaspgrid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_TEST_TEST_YASPGRID_HH
 #define DUNE_GRID_TEST_TEST_YASPGRID_HH
 
 #include <string>
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 if(dune-uggrid_FOUND)
   target_sources(dunegrid PRIVATE
     uggridintersections.cc
     uggrid.cc
     uggridentity.cc
     boundaryextractor.cc
     boundaryextractor.hh
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/boundaryextractor.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/boundaryextractor.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/common/grid.hh>  // for the exceptions
 
 #include "boundaryextractor.hh"
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/boundaryextractor.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/boundaryextractor.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_BOUNDARY_EXTRACTOR_HH
 #define DUNE_BOUNDARY_EXTRACTOR_HH
 
 /** \file
     \brief Contains helper classes for the creation of UGGrid objects
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/ug_undefs.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/ug_undefs.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
  * \brief Contains <tt>#undef</tt>s for all preprocessor macros
  * defined by UG.
  *
  * This file is created automatically by the perl script <tt>undefAllMacros.pl</tt>.
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggrid.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggrid.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <set>
 #include <map>
@@ -31,15 +29,15 @@
 //***********************************************************************
 
 template<> int UGGrid<2>::numOfUGGrids = 0;
 template<> int UGGrid<3>::numOfUGGrids = 0;
 
 
 template <int dim>
-UGGrid < dim >::UGGrid(UGCommunication comm)
+UGGrid < dim >::UGGrid(UGCollectiveCommunication comm)
   : multigrid_(nullptr),
     ccobj_(comm),
     leafIndexSet_(*this),
     idSet_(*this),
     refinementType_(LOCAL),
     closureType_(GREEN),
     someElementHasBeenMarkedForRefinement_(false),
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridentity.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridentity.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/uggrid.hh>
 #include <dune/grid/uggrid/uggridentity.hh>
 #include <dune/grid/uggrid/uggridrenumberer.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridentity.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridentity.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRIDENTITY_HH
 #define DUNE_UGGRIDENTITY_HH
 
 /** \file
  * \brief The UGGridEntity class and its specializations
@@ -139,36 +137,14 @@
      */
     std::vector<std::pair<int,PartitionType> > partitionTypes () const
     {
       std::vector<std::pair<int,PartitionType> > result;
 
 #ifndef ModelP
       result.push_back(std::make_pair(0, InteriorEntity));
-#elif DUNE_UGGRID_DDD_InfoProcListRange
-      const auto range = UG_NS<dim>::DDD_InfoProcListRange(gridImp_->multigrid_->dddContext(), UG_NS<dim>::ParHdr(target_));
-      for (auto&& [rank, priority] : range)
-      {
-        if (priority == UG_NS<dim>::PrioHGhost || priority == UG_NS<dim>::PrioVGhost || priority == UG_NS<dim>::PrioVHGhost)
-          result.push_back(std::make_pair(rank, GhostEntity));
-        else
-        {
-          // The entity is not ghost.  If it is (UG)PrioBorder somewhere, it is (Dune)Border.
-          // Otherwise it is (Dune)Interior.
-          bool hasBorderCopy = false;
-          for (auto&& [rank2, priority2] : range) {
-            if (priority2 == UG_NS<dim>::PrioBorder)
-            {
-              hasBorderCopy = true;
-              break;
-            }
-          }
-
-          result.push_back(std::make_pair(rank, (hasBorderCopy) ? BorderEntity : InteriorEntity));
-        }
-      }
 #else
       int *plist = UG_NS<dim>::DDD_InfoProcList(gridImp_->multigrid_->dddContext(),
                                                 UG_NS<dim>::ParHdr(target_));
 
       for (int i = 0; plist[i] >= 0; i += 2)
       {
         int rank = plist[i];
@@ -196,29 +172,20 @@
     }
 
   protected:
 #ifdef ModelP
     // \todo Unify with the following method
     bool hasBorderCopy() const
     {
-#if DUNE_UGGRID_DDD_InfoProcListRange
-      for (auto&& [rank, priority] : UG_NS<dim>::DDD_InfoProcListRange(
-             gridImp_->multigrid_->dddContext(),
-             UG_NS<dim>::ParHdr(target_))) {
-        if (priority == UG_NS<dim>::PrioBorder)
-          return true;
-      }
-#else
       int  *plist = UG_NS<dim>::DDD_InfoProcList(
         gridImp_->multigrid_->dddContext(),
         UG_NS<dim>::ParHdr(target_));
       for (int i = 0; plist[i] >= 0; i += 2)
         if (plist[i + 1] == UG_NS<dim>::PrioBorder)
           return true;
-#endif
 
       return false;
     }
 #endif
 
 
   public:
@@ -390,22 +357,14 @@
      */
     std::vector<std::pair<int,PartitionType> > partitionTypes () const
     {
       std::vector<std::pair<int,PartitionType> > result;
 
 #ifndef ModelP
       result.push_back(std::make_pair(0, InteriorEntity));
-#elif DUNE_UGGRID_DDD_InfoProcListRange
-      for (auto&& [rank, priority] : UG_NS<dim>::DDD_InfoProcListRange(
-             gridImp_->multigrid_->dddContext(), &target_->ge.ddd)) {
-        if (priority == UG_NS<dim>::PrioHGhost || priority == UG_NS<dim>::PrioVGhost || priority == UG_NS<dim>::PrioVHGhost)
-          result.push_back(std::make_pair(rank, GhostEntity));
-        else
-          result.push_back(std::make_pair(rank, InteriorEntity));
-      }
 #else
       int *plist = UG_NS<dim>::DDD_InfoProcList(gridImp_->multigrid_->dddContext(),
                                                 &target_->ge.ddd);
 
       for (int i = 0; plist[i] >= 0; i += 2)
       {
         int rank = plist[i];
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridfactory.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridfactory.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <config.h>
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridfactory.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_UGGRID_FACTORY_HH
 #define DUNE_UGGRID_FACTORY_HH
 
 /** \file
@@ -260,15 +258,15 @@
     /** \brief Return true if the intersection has been explictily insterted into the factory */
     virtual bool
     wasInserted ( const typename UGGrid<dimworld>::LeafIntersection &intersection ) const
     {
       return (insertionIndex( intersection ) < boundarySegmentVertices_.size());
     }
 
-    using Communication = typename UGGrid<dimworld>::Communication;
+    using Communication = typename UGGrid<dimworld>::CollectiveCommunication;
 
     /** \brief Return the Communication used by the grid factory
      *
      * Use the Communication available from the grid.
      */
     Communication comm() const
     {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridgeometry.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridgeometry.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <algorithm>
 
 #include <dune/grid/uggrid.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridgeometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridgeometry.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRIDGEOMETRY_HH
 #define DUNE_UGGRIDGEOMETRY_HH
 
 /** \file
  * \brief The UGGridGeometry class and its specializations
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridhieriterator.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridhieriterator.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <dune/grid/uggrid.hh>
 #include <dune/grid/uggrid/uggridhieriterator.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridhieriterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridhieriterator.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGHIERITERATOR_HH
 #define DUNE_UGHIERITERATOR_HH
 
 /** \file
  * \brief The UGGridHierarchicIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridindexsets.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridindexsets.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/uggrid.hh>
 #include <dune/grid/uggrid/uggridindexsets.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridindexsets.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridindexsets.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRID_INDEXSETS_HH
 #define DUNE_UGGRID_INDEXSETS_HH
 
 /** \file
     \brief The index and id sets for the UGGrid class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridintersectioniterators.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridintersectioniterators.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGINTERSECTIONIT_HH
 #define DUNE_UGINTERSECTIONIT_HH
 
 /** \file
  * \brief The UGGridIntersectionIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridintersections.cc` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridintersections.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include <config.h>
 
 #include <dune/grid/uggrid.hh>
 #include <dune/grid/uggrid/uggridintersections.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridintersections.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridintersections.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRID_INTERSECTIONS_HH
 #define DUNE_UGGRID_INTERSECTIONS_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridleafiterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridleafiterator.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRIDLEAFITERATOR_HH
 #define DUNE_UGGRIDLEAFITERATOR_HH
 
 /** \file
  * \brief The UGGridLeafIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridleveliterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridleveliterator.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRIDLEVELITERATOR_HH
 #define DUNE_UGGRIDLEVELITERATOR_HH
 
 /** \file
  * \brief The UGGridLevelIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridlocalgeometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridlocalgeometry.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGGRID_LOCALGEOMETRY_HH
 #define DUNE_UGGRID_LOCALGEOMETRY_HH
 
 /** \file
  * \brief The UGGridLocalGeometry class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridrenumberer.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridrenumberer.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_UGGRID_RENUMBERER_HH
 #define DUNE_UGGRID_RENUMBERER_HH
 
 /** \file
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uggridviews.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uggridviews.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_UGGRID_UGGRIDVIEWS_HH
 #define DUNE_GRID_UGGRID_UGGRIDVIEWS_HH
 
 #include <dune/geometry/type.hh>
 
@@ -35,20 +33,16 @@
       /** \brief type of the intersection */
       typedef typename Grid :: Traits :: LevelIntersection Intersection;
 
       /** \brief type of the intersection iterator */
       typedef typename Grid :: Traits :: LevelIntersectionIterator
       IntersectionIterator;
 
-      /** \brief type of the communication */
-      typedef typename Grid :: Traits :: Communication Communication;
-
-      /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-      [[deprecated("Use Communication instead!")]]
-      typedef Communication CollectiveCommunication;
+      /** \brief type of the collective communication */
+      typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
       template< int cd >
       struct Codim
       {
         typedef typename Grid :: Traits
         :: template Codim< cd > :: template Partition< All_Partition > :: LevelIterator
         Iterator;
@@ -91,20 +85,16 @@
 
       /** \brief type of the intersection */
       typedef typename Traits :: Intersection Intersection;
 
       /** \brief type of the intersection iterator */
       typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-      /** \brief type of the communication */
-      typedef typename Traits :: Communication Communication;
-
-      /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-      [[deprecated("Use Communication instead!")]]
-      typedef Communication CollectiveCommunication;
+      /** \brief type of the collective communication */
+      typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
       /** \brief Codim Structure */
       template< int cd >
       struct Codim : public Traits :: template Codim<cd> {};
 
       constexpr static bool conforming = Traits :: conforming;
 
@@ -195,16 +185,16 @@
       /** \brief obtain end intersection iterator with respect to this view */
       IntersectionIterator
       iend ( const typename Codim< 0 > :: Entity &entity ) const
       {
         return entity.impl().ilevelend();
       }
 
-      /** \brief obtain communication object */
-      const Communication &comm () const
+      /** \brief obtain collective communication object */
+      const CollectiveCommunication &comm () const
       {
         return grid().comm();
       }
 
       /** \brief Return size of the overlap region for a given codim on the grid view.  */
       int overlapSize(int codim) const
       {
@@ -250,20 +240,16 @@
       /** \brief type of the intersection */
       typedef typename Grid :: Traits :: LeafIntersection Intersection;
 
       /** \brief type of the intersection iterator */
       typedef typename Grid :: Traits :: LeafIntersectionIterator
       IntersectionIterator;
 
-      /** \brief type of the communication */
-      typedef typename Grid :: Traits :: Communication Communication;
-
-      /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-      [[deprecated("Use Communication instead!")]]
-      typedef Communication CollectiveCommunication;
+      /** \brief type of the collective communication */
+      typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
       template< int cd >
       struct Codim
       {
         typedef typename Grid :: Traits
         :: template Codim< cd > :: template Partition< All_Partition > :: LeafIterator
         Iterator;
@@ -306,20 +292,16 @@
 
       /** \brief type of the intersection */
       typedef typename Traits :: Intersection Intersection;
 
       /** \brief type of the intersection iterator */
       typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-      /** \brief type of the communication */
-      typedef typename Traits :: Communication Communication;
-
-      /** \deprecated Use Communication instead! Will be removed after Dune 2.9. */
-      [[deprecated("Use Communication instead!")]]
-      typedef Communication CollectiveCommunication;
+      /** \brief type of the collective communication */
+      typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
       /** \brief Codim Structure */
       template< int cd >
       struct Codim : public Traits :: template Codim<cd> {};
 
       constexpr static bool conforming = Traits :: conforming;
 
@@ -351,19 +333,14 @@
 
       /** \brief obtain number of entities with a given geometry type */
       int size ( const GeometryType &type ) const
       {
         return grid().size( type );
       }
 
-      bool isConforming() const
-      {
-        return Traits::conforming;
-      }
-
       /** \brief obtain begin iterator for this view */
       template< int cd >
       typename Codim< cd > :: Iterator begin () const
       {
         return UGGridLeafIterator<cd, All_Partition, const Grid>(grid());
       }
 
@@ -398,16 +375,16 @@
       /** \brief obtain end intersection iterator with respect to this view */
       IntersectionIterator
       iend ( const typename Codim< 0 > :: Entity &entity ) const
       {
         return entity.impl().ileafend();
       }
 
-      /** \brief obtain communication object */
-      const Communication &comm () const
+      /** \brief obtain collective communication object */
+      const CollectiveCommunication &comm () const
       {
         return grid().comm();
       }
 
       /** \brief Return size of the overlap region for a given codim on the grid view.  */
       int overlapSize(int codim) const
       {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/ugincludes.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/ugincludes.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGINCLUDES_HH
 #define DUNE_UGINCLUDES_HH
 
 /** \file
  * \brief All includes of UG headers in one single spot
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/uglbgatherscatter.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/uglbgatherscatter.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_UGLBGATHERSCATTER_HH
 #define DUNE_UGLBGATHERSCATTER_HH
 
 namespace Dune {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/ugmessagebuffer.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/ugmessagebuffer.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef UG_MESSAGE_BUFFER_HH
 #define UG_MESSAGE_BUFFER_HH
 
 #include <algorithm>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/ugwrapper.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/ugwrapper.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
  * \brief Encapsulates some UG macros and functions
  */
 
 /** \todo Here only to provide the constant DBL_EPSILON.  There's maybe a better way? */
@@ -121,34 +119,27 @@
       UG_NAMESPACE::DDD_IFOneway(
 #if DUNE_UGGRID_HAVE_DDDCONTEXT
         context,
 #endif
         dddIf, dddIfDir, s, gather, scatter);
     }
 
-#if DUNE_UGGRID_DDD_InfoProcListRange
-    static auto DDD_InfoProcListRange(DDD::DDDContext& context, DDD_HEADER* hdr) noexcept
-    {
-      return UG_NAMESPACE::DDD_InfoProcListRange(context, hdr);
-    }
-#else
     static int *DDD_InfoProcList(
 #if DUNE_UGGRID_HAVE_DDDCONTEXT
                              DDD::DDDContext& context,
 #endif
       DDD_HEADER *hdr)
     {
 #if DUNE_UGGRID_HAVE_DDDCONTEXT
       //return DDD::DDD_InfoProcList(context, hdr);
       return UG_NAMESPACE::DDD_InfoProcList(context, hdr);
 #else
       return UG_NAMESPACE::DDD_InfoProcList(hdr);
 #endif
     }
-#endif
 
     static DDD_IF_DIR IF_FORWARD()
     {
       return UG_NAMESPACE::IF_FORWARD;
     }
 
     static DDD_IF_DIR IF_BACKWARD()
@@ -1156,14 +1147,15 @@
                                        const double *alpha, const double *beta,
                                        UG_NAMESPACE ::BndSegFuncPtr boundarySegmentFunction,
                                        void *userData) {
       return UG_NAMESPACE ::CreateBoundarySegment(name,            // internal name of the boundary segment
                                                   left,             //  id of left subdomain
                                                   right,             //  id of right subdomain
                                                   index,         // Index of the segment
+                                                  UG_NAMESPACE ::NON_PERIODIC, // I don't know what this means
                                                   point,
                                                   alpha,
                                                   beta,
                                                   boundarySegmentFunction,
                                                   userData);
     }
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid/undefAllMacros.pl` & `dune-grid-2.9.dev20220529/dune/grid/uggrid/undefAllMacros.pl`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 #!/usr/bin/perl -w
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 
 # TODO: Detect location of UG from the DUNE build system
 $UGROOT = "/home/sander/uginst";
 
 # Counts the total number of #undefs emitted
 $counter = 0;
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/uggrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/uggrid.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_UGGRID_HH
 #define DUNE_UGGRID_HH
 
 /** \file
@@ -128,17 +126,17 @@
 template <class DataHandle, int GridDim, int codim>
 int Dune::UGMessageBuffer<DataHandle,GridDim,codim>::level = -1;
 #endif // ModelP
 
 namespace Dune {
 
 #ifdef ModelP
-    using UGCommunication = Communication<MPI_Comm>;
+    using UGCollectiveCommunication = Communication<MPI_Comm>;
 #else
-    using UGCommunication = Communication<No_Comm>;
+    using UGCollectiveCommunication = Communication<No_Comm>;
 #endif
 
   template<int dim>
   struct UGGridFamily
   {
     typedef GridTraits<dim,dim,Dune::UGGrid<dim>,
         UGGridGeometry,
@@ -152,15 +150,15 @@
         UGGridLeafIterator,
         UGGridLevelIndexSet< const UGGrid<dim> >,
         UGGridLeafIndexSet< const UGGrid<dim> >,
         UGGridIdSet< const UGGrid<dim> >,
         typename UG_NS<dim>::UG_ID_TYPE,
         UGGridIdSet< const UGGrid<dim> >,
         typename UG_NS<dim>::UG_ID_TYPE,
-        UGCommunication,
+        UGCollectiveCommunication,
         UGGridLevelGridViewTraits,
         UGGridLeafGridViewTraits,
         UGGridEntitySeed,
         UGGridLocalGeometry>
     Traits;
   };
 
@@ -263,15 +261,15 @@
     typedef UG::DOUBLE ctype;
 
     //! The type used for process ranks
     typedef unsigned int Rank;
 
     /** \brief Default constructor
      */
-    UGGrid(UGCommunication comm = {});
+    UGGrid(UGCollectiveCommunication comm = {});
 
     //! Destructor
     ~UGGrid()  noexcept(false);
 
     //! Return maximum level defined in this grid. Levels are numbered
     //! 0 ... maxlevel with 0 the coarsest level.
     int maxLevel() const;
@@ -542,16 +540,16 @@
       if (dataHandle.contains(dim,dim))
         UGLBGatherScatter::template scatter<dim>(this->leafGridView(), dataHandle);
 #endif
 
       return true;
     }
 
-    /** the communication */
-    const UGCommunication& comm () const
+    /** the collective communication */
+    const UGCollectiveCommunication& comm () const
     {
       return ccobj_;
     }
 
   protected:
 #ifdef ModelP
     template <int codim, class GridView, class DataHandle>
@@ -659,16 +657,16 @@
      */
     void loadState(const std::string& filename);
 
   private:
     /** \brief UG multigrid, which contains the actual grid hierarchy structure */
     typename UG_NS<dim>::MultiGrid* multigrid_;
 
-    /** \brief The communication object. */
-    UGCommunication ccobj_;
+    /** \brief The collective communication object. */
+    UGCollectiveCommunication ccobj_;
 
     /** \brief Recomputes entity indices after the grid was changed
         \param setLevelZero If this is false, level indices of the level 0 are not touched
         \param nodePermutation Permutation array for the vertex level 0 indices.  If this is NULL,
         the identity is used.
      */
     void setIndices(bool setLevelZero,
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/entitycommhelper.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/entitycommhelper.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_ENTITYCOMMHELPER_HH
 #define DUNE_ENTITYCOMMHELPER_HH
 
 #include <dune/grid/common/gridenums.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/globalindexset.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/globalindexset.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 /** \file
  *
  *  \brief Provides a globally unique index for all entities of a distributed Dune grid
  *
@@ -97,15 +95,15 @@
     /** define data types */
     typedef typename GridView::Grid Grid;
 
     typedef typename GridView::Grid::GlobalIdSet GlobalIdSet;
     typedef typename GridView::Grid::GlobalIdSet::IdType IdType;
     typedef typename GridView::Traits::template Codim<0>::Iterator Iterator;
 
-    typedef typename Grid::Communication Communication;
+    typedef typename Grid::CollectiveCommunication CollectiveCommunication;
 
     typedef std::map<IdType,Index> MapId2Index;
     typedef std::map<Index,Index>    IndexMap;
 
     /*********************************************************************************************/
     /* calculate unique partitioning for all entities of a given codim in a given GridView,      */
     /* assuming they all have the same geometry, i.e. codim, type                                */
@@ -341,15 +339,15 @@
                     : uniqueEntityPartition->numOwners(rank);
 
       // Compute the global, non-redundant number of entities, i.e. the number of entities in the set
       // without double, aka. redundant entities, on the interprocessor boundary via global reduce. */
       nGlobalEntity_ = gridview.comm().template sum<int>(nLocalEntity);
 
       /* communicate the number of locally owned entities to all other processes so that the respective offset
-       * can be calculated on the respective processor; we use the Dune mpi communication facility
+       * can be calculated on the respective processor; we use the Dune mpi collective communication facility
        * for this; first, we gather the number of locally owned entities on the root process and, second, we
        * broadcast the array to all processes where the respective offset can be calculated. */
 
       std::vector<int> offset(size);
       std::fill(offset.begin(), offset.end(), 0);
 
       /** Share number of locally owned entities */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/gridinfo-gmsh-main.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/gridinfo-gmsh-main.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_UTILITY_GRIDINFO_GMSH_MAIN_HH
 #define DUNE_GRID_UTILITY_GRIDINFO_GMSH_MAIN_HH
 
 #include <cstddef>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/gridinfo.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/gridinfo.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_UTILITY_GRIDINFO_HH
 #define DUNE_GRID_UTILITY_GRIDINFO_HH
 
 #include <algorithm>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/hierarchicsearch.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/hierarchicsearch.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_HIERARCHICSEARCH_HH
 #define DUNE_GRID_HIERARCHICSEARCH_HH
 
 /**
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/hostgridaccess.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/hostgridaccess.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_HOSTGRIDACCESS_HH
 #define DUNE_GRID_HOSTGRIDACCESS_HH
 
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/multiindex.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/multiindex.hh`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_UTILITY_MULTIINDEX_HH
 #define DUNE_GRID_UTILITY_MULTIINDEX_HH
 
 /** \file
  *  \brief Implements a multiindex with arbitrary dimension and fixed index ranges
  *  This is used by various factory classes.
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/parmetisgridpartitioner.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/parmetisgridpartitioner.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_UTILITY_PARMETISGRIDPARTITIONER_HH
 #define DUNE_GRID_UTILITY_PARMETISGRIDPARTITIONER_HH
 
 /** \file
  *  \brief Compute a repartitioning of a Dune grid using ParMetis
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainer.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainer.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PERSISTENTCONTAINER_HH
 #define DUNE_PERSISTENTCONTAINER_HH
 
 #include <map>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainerinterface.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainerinterface.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PERSISTENTCONTAINERINTERFACE_HH
 #define DUNE_PERSISTENTCONTAINERINTERFACE_HH
 
 #ifndef HEADERCHECK
 #error "This header exists for documentation purposes only and should never be included directly."
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainermap.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainermap.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PERSISTENTCONTAINERMAP_HH
 #define DUNE_PERSISTENTCONTAINERMAP_HH
 
 #include <algorithm>
 #include <cassert>
@@ -83,15 +81,15 @@
     }
 
     Size size () const { return data_.size(); }
 
     void resize ( const Value &value = Value() )
     {
       Hybrid::forEach( std::make_index_sequence< Grid::dimension+1 >{},
-        [ & ]( auto i ){ if( int(i) == this->codimension() ) this->template resize< i >( value ); } );
+        [ & ]( auto i ){ if( i == this->codimension() ) this->template resize< i >( value ); } );
     }
 
     void shrinkToFit () {}
 
     void fill ( const Value &value ) { std::fill( begin(), end(), value ); }
 
     void swap ( This &other )
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainervector.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainervector.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PERSISTENTCONTAINERVECTOR_HH
 #define DUNE_PERSISTENTCONTAINERVECTOR_HH
 
 #include <algorithm>
 #include <cassert>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/persistentcontainerwrapper.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/persistentcontainerwrapper.hh`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PERSISTENTCONTAINERWRAPPER_HH
 #define DUNE_PERSISTENTCONTAINERWRAPPER_HH
 
 #include <dune/grid/utility/hostgridaccess.hh>
 #include <dune/grid/utility/persistentcontainer.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/structuredgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/structuredgridfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_STRUCTURED_GRID_FACTORY_HH
 #define DUNE_STRUCTURED_GRID_FACTORY_HH
 
 /** \file
     \brief A class to construct structured cube and simplex grids using the grid factory
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/tensorgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/tensorgridfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_UTILITY_TENSORGRIDFACTORY_HH
 #define DUNE_GRID_UTILITY_TENSORGRIDFACTORY_HH
 
 /** \file
  *  \brief This file provides a factory class for tensorproduct
  *  grids. This is a collection of methods to generate monotonous
  *  sequences as needed for a tensorproduct grid. Apart
@@ -37,15 +35,15 @@
    *
    * \tparam Grid the grid type
    */
   template<typename Grid>
   class TensorGridFactory
   {
   public:
-    typedef typename Grid::Traits::Communication Comm;
+    typedef typename Grid::Traits::CollectiveCommunication Comm;
     typedef typename Grid::ctype ctype;
     static const int dim = Grid::dimension;
 
     std::unique_ptr<Grid> createGrid(Comm comm = Comm())
     {
       TensorGridFactoryCreator<Grid> creator(*this);
       return creator.createGrid(comm);
@@ -301,15 +299,15 @@
 
   // class that implements the actual grid creation process. The default is implementing
   // standard creation for unstructured grids. Provide a specialization for other grids.
   template<typename Grid>
   class TensorGridFactoryCreator
   {
   public:
-    typedef typename Grid::Traits::Communication Comm;
+    typedef typename Grid::Traits::CollectiveCommunication Comm;
     typedef typename Grid::ctype ctype;
     static const int dim = Grid::dimension;
 
     TensorGridFactoryCreator(const TensorGridFactory<Grid>& factory) : _factory(factory) {}
 
     std::unique_ptr<Grid> createGrid(Comm comm)
     {
@@ -385,15 +383,15 @@
   };
 
   template<typename ctype, int dim>
   class TensorGridFactoryCreator<YaspGrid<dim, TensorProductCoordinates<ctype, dim> > >
   {
   public:
     typedef YaspGrid<dim, TensorProductCoordinates<ctype, dim> > Grid;
-    typedef typename Grid::Communication Comm;
+    typedef typename Grid::CollectiveCommunication Comm;
 
     TensorGridFactoryCreator(const TensorGridFactory<Grid>& factory) : _factory(factory) {}
 
     std::unique_ptr<Grid> createGrid(Comm comm)
     {
       return std::make_unique<Grid>(_factory.coords(), std::bitset<dim>(0ULL), 1, comm);
     }
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/test/globalindexsettest.cc` & `dune-grid-2.9.dev20220529/dune/grid/utility/test/globalindexsettest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #include "config.h"
 
 #include <iostream>
 #include <numeric>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/test/persistentcontainertest.cc` & `dune-grid-2.9.dev20220529/dune/grid/utility/test/persistentcontainertest.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
     \brief A unit test for the PersistentContainer
  */
 
 #include <config.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/test/structuredgridfactorytest.cc` & `dune-grid-2.9.dev20220529/dune/grid/utility/test/structuredgridfactorytest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
     \brief A unit test for the StructuredGridFactory
  */
 
 #include <config.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/test/tensorgridfactorytest.cc` & `dune-grid-2.9.dev20220529/dune/grid/utility/test/tensorgridfactorytest.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 /** \file
     \brief A unit test for the TensorGridFactory
  */
 
 #include <config.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/test/vertexordertest.cc` & `dune-grid-2.9.dev20220529/dune/grid/utility/test/vertexordertest.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 /** \file
     \brief A unit test for the VertexOrder classes
  */
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/utility/vertexorderfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/utility/vertexorderfactory.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_GRID_UTILITY_VERTEXORDERFACTORY_HH
 #define DUNE_GRID_UTILITY_VERTEXORDERFACTORY_HH
 
 #include <algorithm>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/CMakeLists.txt` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 set(HEADERS
   backuprestore.hh
   coordinates.hh
   partitioning.hh
   structuredyaspgridfactory.hh
   torus.hh
   yaspgridentity.hh
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/backuprestore.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/backuprestore.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRID_BACKUPRESTORE_HH
 #define DUNE_GRID_YASPGRID_BACKUPRESTORE_HH
 
 //- system headers
 #include <fstream>
-#include <iterator>
 
 //- Dune headers
 #include <dune/common/exceptions.hh>
 #include <dune/common/fvector.hh>
 #include <dune/grid/common/backuprestore.hh>
 #include <dune/grid/yaspgrid.hh>
 
@@ -79,15 +76,15 @@
   /** \copydoc Dune::BackupRestoreFacility */
   template<int dim, class Coordinates>
   struct BackupRestoreFacility<Dune::YaspGrid<dim, Coordinates> >
   {
     // type of grid
     typedef typename Dune::YaspGrid<dim, Coordinates> Grid;
     typedef typename Grid::ctype ctype;
-    typedef typename Grid::Traits::Communication Comm;
+    typedef typename Grid::Traits::CollectiveCommunication Comm;
 
     /** \copydoc Dune::BackupRestoreFacility::backup(grid,filename)  */
     static void backup ( const Grid &grid, const std::string &filename )
     {
       if (grid.comm().rank() == 0)
       {
         std::ofstream file(filename);
@@ -110,15 +107,15 @@
         stream << grid.torus().dims(i) << " ";
       stream << std::endl << "Refinement level: " << grid.maxLevel() << std::endl;
       stream << "Periodicity: ";
       for (int i=0; i<dim; i++)
         stream << (grid.isPeriodic(i) ? "1 " : "0 ");
       stream << std::endl << "Overlap: " << grid.overlapSize(0,0) << std::endl;
       stream << "KeepPhysicalOverlap: ";
-      for (typename Grid::YGridLevelIterator i=std::next(grid.begin()); i != grid.end(); ++i)
+      for (typename Grid::YGridLevelIterator i=++grid.begin(); i != grid.end(); ++i)
         stream << (i->keepOverlap ? "1" : "0") << " ";
       stream << std::endl;
       stream << "Coarse Size: ";
       for (int i=0; i<dim; i++)
         stream << grid.levelSize(0,i) << " ";
       stream << std::endl;
       stream << "Meshsize: " ;
@@ -197,15 +194,15 @@
       MaybeHaveOrigin<Coordinates>::readOrigin(stream, origin);
 
       // the constructor takes the upper right corner...
       Dune::FieldVector<ctype,dim> length(h);
       for (int i=0; i<dim; i++)
         length[i] *= coarseSize[i];
 
-      Yasp::FixedSizePartitioning<dim> lb(torus_dims);
+      YaspFixedSizePartitioner<dim> lb(torus_dims);
 
       Grid* grid = MaybeHaveOrigin<Coordinates>::createGrid(origin, length, coarseSize, periodic, overlap, comm, &lb);
 
       for (int i=0; i<refinement; ++i)
       {
         grid->refineOptions(physicalOverlapSize[i]);
         grid->globalRefine(1);
@@ -217,15 +214,15 @@
 
   /** \copydoc Dune::BackupRestoreFacility */
   template<int dim, class ctype>
   struct BackupRestoreFacility<YaspGrid<dim,TensorProductCoordinates<ctype,dim> > >
   {
     // type of grid
     typedef YaspGrid<dim,TensorProductCoordinates<ctype,dim> > Grid;
-    typedef typename Grid::Traits::Communication Comm;
+    typedef typename Grid::Traits::CollectiveCommunication Comm;
 
     /** \copydoc Dune::BackupRestoreFacility::backup(grid,filename)  */
     static void backup ( const Grid &grid, const std::string &filename )
     {
       std::ostringstream filename_str;
       filename_str << filename << grid.comm().rank();
       std::ofstream file( filename_str.str() );
@@ -247,15 +244,15 @@
         stream << grid.torus().dims(i) << " ";
       stream << std::endl << "Refinement level: " << grid.maxLevel() << std::endl;
       stream << "Periodicity: ";
       for (int i=0; i<dim; i++)
         stream << (grid.isPeriodic(i) ? "1 " : "0 ");
       stream << std::endl << "Overlap: " << grid.overlapSize(0,0) << std::endl;
       stream << "KeepPhysicalOverlap: ";
-      for (typename Grid::YGridLevelIterator i=std::next(grid.begin()); i != grid.end(); ++i)
+      for (typename Grid::YGridLevelIterator i=++grid.begin(); i != grid.end(); ++i)
         stream << (i->keepOverlap ? "1" : "0") << " ";
       stream << std::endl;
       stream << "Coarse Size: ";
       for (int i=0; i<dim; i++)
         stream << grid.levelSize(0,i) << " ";
       stream << std::endl;
 
@@ -339,15 +336,15 @@
         for (int i=0; i<size; i++)
         {
           stream >> tmp;
           coords[d][i] = tmp;
         }
       }
 
-      Yasp::FixedSizePartitioning<dim> lb(torus_dims);
+      YaspFixedSizePartitioner<dim> lb(torus_dims);
       Grid* grid = new Grid(coords, periodic, overlap, comm, coarseSize, &lb);
 
       for (int i=0; i<refinement; ++i)
       {
         grid->refineOptions(physicalOverlapSize[i]);
         grid->globalRefine(1);
       }
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/coordinates.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/coordinates.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRID_COORDINATES_HH
 #define DUNE_GRID_YASPGRID_COORDINATES_HH
 
 #include <array>
 #include <bitset>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.eps` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/grid.eps`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.fig` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/grid.fig`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/grid.png` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/grid.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/structuredyaspgridfactory.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/structuredyaspgridfactory.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRID_STRUCTUREDYASPGRIDFACTORY_HH
 #define DUNE_GRID_YASPGRID_STRUCTUREDYASPGRIDFACTORY_HH
 
 #include <memory>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.eps` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/subgrid.eps`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.fig` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/subgrid.fig`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/subgrid.png` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/subgrid.png`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/torus.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/torus.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRID_TORUS_HH
 #define DUNE_GRID_YASPGRID_TORUS_HH
 
 #include <array>
 #include <bitset>
@@ -38,15 +36,15 @@
      using asynchronous communication with MPI. The periodic case is handled where one process
      might have to exchange several messages with the same process. (Logically, a process has always
      \f$3^d-1\f$ neighbors, but several of these logical neighbors might be identical)
 
      - Provide means to partition a grid to the torus.
 
    */
-  template<class Communication, int d>
+  template<class CollectiveCommunication, int d>
   class Torus {
   public:
     //! type used to pass tupels in and out
     typedef std::array<int, d> iTupel;
 
 
   private:
@@ -64,19 +62,19 @@
 
   public:
     //! constructor making uninitialized object
     Torus ()
     {}
 
     //! make partitioner from communicator and coarse mesh size
-    Torus (Communication comm, int tag, iTupel size, int overlap, const Yasp::Partitioning<d>* partitioner)
+    Torus (CollectiveCommunication comm, int tag, iTupel size, const YLoadBalance<d>* lb)
       : _comm(comm), _tag(tag)
     {
       // determine dimensions
-      partitioner->partition(size, _comm.size(), _dims, overlap);
+      lb->loadbalance(size, _comm.size(), _dims);
 
       // compute increments for lexicographic ordering
       int inc = 1;
       for (int i=0; i<d; i++)
       {
         _increment[i] = inc;
         inc *= _dims[i];
@@ -117,15 +115,15 @@
     //! return dimensions of torus in direction i
     int dims (int i) const
     {
       return _dims[i];
     }
 
     //! return communicator
-    Communication comm () const
+    CollectiveCommunication comm () const
     {
       return _comm;
     }
 
     //! return tag used by torus
     int tag () const
     {
@@ -517,15 +515,15 @@
           {
             delta[i] = -1;
           }
       }
 
     }
 
-    Communication _comm;
+    CollectiveCommunication _comm;
 
     iTupel _dims;
     iTupel _increment;
     int _tag;
     std::deque<CommPartner> _sendlist;
     std::deque<CommPartner> _recvlist;
 
@@ -533,16 +531,16 @@
     mutable std::vector<CommTask> _recvrequests;
     mutable std::vector<CommTask> _localsendrequests;
     mutable std::vector<CommTask> _localrecvrequests;
 
   };
 
   //! Output operator for Torus
-  template <class Communication, int d>
-  inline std::ostream& operator<< (std::ostream& s, const Torus<Communication, d> & t)
+  template <class CollectiveCommunication, int d>
+  inline std::ostream& operator<< (std::ostream& s, const Torus<CollectiveCommunication, d> & t)
   {
     t.print(s);
     return s;
   }
 }
 
 #endif
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridentity.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridentity.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDENTITY_HH
 #define DUNE_GRID_YASPGRIDENTITY_HH
 
 #include <dune/common/math.hh>
 #include <dune/geometry/type.hh>
@@ -418,16 +416,16 @@
     public:
     const I& transformingsubiterator() const { return _it; }
     const YGLI& gridlevel() const { return _g; }
     I& transformingsubiterator() { return _it; }
     YGLI& gridlevel() { return _g; }
     const GridImp * yaspgrid() const { return _g->mg; }
     protected:
-    I _it = {};               // position in the grid level
-    YGLI _g = {};               // access to grid level
+    I _it;               // position in the grid level
+    YGLI _g;               // access to grid level
   };
 
 
   // specialization for codim=0
   template<int dim, class GridImp>
   class YaspEntity<0,dim,GridImp>
     : public EntityDefaultImplementation <0,dim,GridImp,YaspEntity>
@@ -797,16 +795,16 @@
       for (int j=0; j<dim; j++)
         coord[j] += move[j];
 
       int which = _g->overlapfront[cc].shiftmapping(shift);
       return _g->overlapfront[cc].superindex(coord,which);
     }
 
-    I _it = {};         // position in the grid level
-    YGLI _g = {};         // access to grid level
+    I _it;         // position in the grid level
+    YGLI _g;         // access to grid level
   };
 
 
   // specialization for codim=dim (vertex)
   template<int dim, class GridImp>
   class YaspEntity<dim,dim,GridImp>
     : public EntityDefaultImplementation <dim,dim,GridImp,YaspEntity>
@@ -964,14 +962,14 @@
     const I& transformingsubiterator() const { return _it; }
     const YGLI& gridlevel() const { return _g; }
     I& transformingsubiterator() { return _it; }
     YGLI& gridlevel() { return _g; }
 
     const GridImp * yaspgrid() const { return _g->mg; }
   protected:
-    I _it = {};               // position in the grid level
-    YGLI _g = {};               // access to grid level
+    I _it;               // position in the grid level
+    YGLI _g;               // access to grid level
   };
 
 }   // namespace Dune
 
 #endif  // DUNE_GRID_YASPGRIDENTITY_HH
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridentityseed.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridentityseed.hh`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDENTITYSEED_HH
 #define DUNE_GRID_YASPGRIDENTITYSEED_HH
 
 /** \file
  * \brief The YaspEntitySeed class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridgeometry.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridgeometry.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDGEOMETRY_HH
 #define DUNE_GRID_YASPGRIDGEOMETRY_HH
 
 /** \file
  * \brief The YaspGeometry class and its specializations
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridhierarchiciterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridhierarchiciterator.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDHIERARCHICITERATOR_HH
 #define DUNE_GRID_YASPGRIDHIERARCHICITERATOR_HH
 
 /** \file
  * The YaspHierarchicIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgrididset.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgrididset.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDIDSET_HH
 #define DUNE_GRID_YASPGRIDIDSET_HH
 
 
 namespace Dune {
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridindexsets.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridindexsets.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDINDEXSET_HH
 #define DUNE_GRID_YASPGRIDINDEXSET_HH
 
 /** \file
  *
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridintersection.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridintersection.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDINTERSECTION_HH
 #define DUNE_GRID_YASPGRIDINTERSECTION_HH
 
 /** \file
  * \brief The YaspIntersection class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridintersectioniterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridintersectioniterator.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDINTERSECTIONITERATOR_HH
 #define DUNE_GRID_YASPGRIDINTERSECTIONITERATOR_HH
 
 /** \file
  * \brief The YaspIntersectionIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridleveliterator.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridleveliterator.hh`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDLEVELITERATOR_HH
 #define DUNE_GRID_YASPGRIDLEVELITERATOR_HH
 
 /** \file
  * \brief The YaspLevelIterator class
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/yaspgridpersistentcontainer.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/yaspgridpersistentcontainer.hh`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRIDPERSISTENTCONTAINER_HH
 #define DUNE_GRID_YASPGRIDPERSISTENTCONTAINER_HH
 
 /** \file
  * \brief Specialization of the PersistentContainer for YaspGrid
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid/ygrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid/ygrid.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRID_YGRID_HH
 #define DUNE_GRID_YASPGRID_YGRID_HH
 
 #include <array>
 #include <vector>
```

### Comparing `dune-grid-2.9.0rc1/dune/grid/yaspgrid.hh` & `dune-grid-2.9.dev20220529/dune/grid/yaspgrid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_GRID_YASPGRID_HH
 #define DUNE_GRID_YASPGRID_HH
 
 #include <cstdint>
 #include <iostream>
-#include <iterator>
 #include <vector>
 #include <algorithm>
 #include <stack>
 #include <type_traits>
 
 #include <dune/grid/common/backuprestore.hh>
 #include <dune/grid/common/grid.hh>     // the grid base classes
@@ -78,23 +75,23 @@
 #include <dune/grid/yaspgrid/yaspgridindexsets.hh>
 #include <dune/grid/yaspgrid/yaspgrididset.hh>
 #include <dune/grid/yaspgrid/yaspgridpersistentcontainer.hh>
 
 namespace Dune {
 
 #if HAVE_MPI
-  using YaspCommunication = Communication<MPI_Comm>;
+  using YaspCollectiveCommunication = Communication<MPI_Comm>;
 #else
-  using YaspCommunication = Communication<No_Comm>;
+  using YaspCollectiveCommunication = Communication<No_Comm>;
 #endif
 
   template<int dim, class Coordinates>
   struct YaspGridFamily
   {
-    typedef YaspCommunication CCType;
+    typedef YaspCollectiveCommunication CCType;
 
     typedef GridTraits<dim,                                     // dimension of the grid
         dim,                                                    // dimension of the world space
         Dune::YaspGrid<dim, Coordinates>,
         YaspGeometry,YaspEntity,
         YaspLevelIterator,                                      // type used for the level iterator
         YaspIntersection,              // leaf  intersection
@@ -164,23 +161,20 @@
 
     template<int, PartitionIteratorType, typename>
     friend class YaspLevelIterator;
 
     template<typename>
     friend class YaspHierarchicIterator;
 
-    using Base = GridDefaultImplementation<dim,dim,typename Coordinates::ctype,YaspGridFamily<dim, Coordinates> >;
   protected:
 
   public:
     //! Type used for coordinates
     typedef typename Coordinates::ctype ctype;
-
-    using Communication = typename Base::Communication;
-    using CollectiveCommunicationType [[deprecated("Use Communication. Will be removed after release 2.9")]] = typename Base::Communication;
+    typedef YaspCollectiveCommunication CollectiveCommunicationType;
 
 #ifndef DOXYGEN
     typedef typename Dune::YGrid<Coordinates> YGrid;
     typedef typename Dune::YGridList<Coordinates>::Intersection Intersection;
 
     /** \brief A single grid level within a YaspGrid
      */
@@ -237,15 +231,15 @@
     typedef FieldVector<ctype, dim> fTupel;
 
     // communication tag used by multigrid
     enum { tag = 17 };
 #endif
 
     //! return reference to torus
-    const Torus<Communication, dim>& torus () const
+    const Torus<CollectiveCommunicationType, dim>& torus () const
     {
       return _torus;
     }
 
     //! return number of cells on finest level in given direction on all processors
     int globalSize(int i) const
     {
@@ -286,46 +280,38 @@
 
     //! Iterator over the grid levels
     typedef typename ReservedVector<YGridLevel,32>::const_iterator YGridLevelIterator;
 
     //! return iterator pointing to coarsest level
     YGridLevelIterator begin () const
     {
-      return _levels.begin();
+      return YGridLevelIterator(_levels,0);
     }
 
     //! return iterator pointing to given level
     YGridLevelIterator begin (int i) const
     {
       if (i<0 || i>maxLevel())
         DUNE_THROW(GridError, "level not existing");
-      return std::next(_levels.begin(), i);
+      return YGridLevelIterator(_levels,i);
     }
 
     //! return iterator pointing to one past the finest level
     YGridLevelIterator end () const
     {
-      return _levels.end();
+      return YGridLevelIterator(_levels,maxLevel()+1);
     }
 
     // static method to create the default load balance strategy
-    [[deprecated("use defaultPartitioner")]]
     static const YLoadBalanceDefault<dim>* defaultLoadbalancer()
     {
       static YLoadBalanceDefault<dim> lb;
       return & lb;
     }
 
-    // static method to create the default partitioning strategy
-    static const Yasp::Partitioning<dim>* defaultPartitioner()
-    {
-      static Yasp::DefaultPartitioning<dim> lb;
-      return & lb;
-    }
-
   protected:
     /** \brief Make a new YGridLevel structure
      *
      * \param coords      the coordinate container
      * \param periodic    indicate periodicity for each direction
      * \param o_interior  origin of interior (non-overlapping) cell decomposition
      * \param overlap     to be used on this grid level
@@ -580,15 +566,15 @@
       std::vector<mpifriendly_ygrid> mpifriendly_send_recvgrid(_torus.neighbors());
       std::vector<mpifriendly_ygrid> mpifriendly_recv_recvgrid(_torus.neighbors());
       std::vector<mpifriendly_ygrid> mpifriendly_send_sendgrid(_torus.neighbors());
       std::vector<mpifriendly_ygrid> mpifriendly_recv_sendgrid(_torus.neighbors());
 
       // fill send buffers; iterate over all neighboring processes
       // non-periodic case is handled automatically because intersection will be zero
-      for (typename Torus<Communication,dim>::ProcListIterator i=_torus.sendbegin(); i!=_torus.sendend(); ++i)
+      for (typename Torus<CollectiveCommunicationType,dim>::ProcListIterator i=_torus.sendbegin(); i!=_torus.sendend(); ++i)
       {
         // determine if we communicate with this neighbor (and what)
         bool skip = false;
         iTupel coord = _torus.coord();   // my coordinates
         iTupel delta = i.delta();        // delta to neighbor
         iTupel nb = coord;               // the neighbor
         for (int k=0; k<dim; k++) nb[k] += delta[k];
@@ -624,43 +610,43 @@
         {
           send_sendgrid[i.index()] = YGridComponent<Coordinates>();
           send_recvgrid[i.index()] = YGridComponent<Coordinates>();
         }
       }
 
       // issue send requests for sendgrid being sent to all neighbors
-      for (typename Torus<Communication,dim>::ProcListIterator i=_torus.sendbegin(); i!=_torus.sendend(); ++i)
+      for (typename Torus<CollectiveCommunicationType,dim>::ProcListIterator i=_torus.sendbegin(); i!=_torus.sendend(); ++i)
       {
         mpifriendly_send_sendgrid[i.index()] = mpifriendly_ygrid(send_sendgrid[i.index()]);
         _torus.send(i.rank(), &mpifriendly_send_sendgrid[i.index()], sizeof(mpifriendly_ygrid));
       }
 
       // issue recv requests for sendgrids of neighbors
-      for (typename Torus<Communication,dim>::ProcListIterator i=_torus.recvbegin(); i!=_torus.recvend(); ++i)
+      for (typename Torus<CollectiveCommunicationType,dim>::ProcListIterator i=_torus.recvbegin(); i!=_torus.recvend(); ++i)
         _torus.recv(i.rank(), &mpifriendly_recv_sendgrid[i.index()], sizeof(mpifriendly_ygrid));
 
       // exchange the sendgrids
       _torus.exchange();
 
       // issue send requests for recvgrid being sent to all neighbors
-      for (typename Torus<Communication,dim>::ProcListIterator i=_torus.sendbegin(); i!=_torus.sendend(); ++i)
+      for (typename Torus<CollectiveCommunicationType,dim>::ProcListIterator i=_torus.sendbegin(); i!=_torus.sendend(); ++i)
       {
         mpifriendly_send_recvgrid[i.index()] = mpifriendly_ygrid(send_recvgrid[i.index()]);
         _torus.send(i.rank(), &mpifriendly_send_recvgrid[i.index()], sizeof(mpifriendly_ygrid));
       }
 
       // issue recv requests for recvgrid of neighbors
-      for (typename Torus<Communication,dim>::ProcListIterator i=_torus.recvbegin(); i!=_torus.recvend(); ++i)
+      for (typename Torus<CollectiveCommunicationType,dim>::ProcListIterator i=_torus.recvbegin(); i!=_torus.recvend(); ++i)
         _torus.recv(i.rank(), &mpifriendly_recv_recvgrid[i.index()], sizeof(mpifriendly_ygrid));
 
       // exchange the recvgrid
       _torus.exchange();
 
       // process receive buffers and compute intersections
-      for (typename Torus<Communication,dim>::ProcListIterator i=_torus.recvbegin(); i!=_torus.recvend(); ++i)
+      for (typename Torus<CollectiveCommunicationType,dim>::ProcListIterator i=_torus.recvbegin(); i!=_torus.recvend(); ++i)
       {
         // what must be sent to this neighbor
         Intersection send_intersection;
         mpifriendly_ygrid yg = mpifriendly_recv_recvgrid[i.index()];
         recv_recvgrid[i.index()] = YGridComponent<Coordinates>(yg.origin,yg.size);
         send_intersection.grid = sendgrid.intersection(recv_recvgrid[i.index()]);
         send_intersection.rank = i.rank();
@@ -728,22 +714,22 @@
     typedef YaspIndexSet<YaspGrid<dim, Coordinates>, true > LeafIndexSetType;
     typedef YaspGlobalIdSet<YaspGrid<dim, Coordinates> > GlobalIdSetType;
 
     /** Standard constructor for a YaspGrid with a given Coordinates object
      *  @param coordinates Object that stores or computes the vertex coordinates
      *  @param periodic tells if direction is periodic or not
      *  @param overlap size of overlap on coarsest grid (same in all directions)
-     *  @param comm the communication object for this grid. An MPI communicator can be given here.
-     *  @param partitioner pointer to an overloaded Yasp::Partitioning instance
+     *  @param comm the collective communication object for this grid. An MPI communicator can be given here.
+     *  @param lb pointer to an overloaded YLoadBalance instance
      */
     YaspGrid (const Coordinates& coordinates,
               std::bitset<dim> periodic = std::bitset<dim>(0ULL),
               int overlap = 1,
-              Communication comm = Communication(),
-              const Yasp::Partitioning<dim>* partitioner = defaultPartitioner())
+              CollectiveCommunicationType comm = CollectiveCommunicationType(),
+              const YLoadBalance<dim>* lb = defaultLoadbalancer())
       : ccobj(comm)
       , leafIndexSet_(*this)
       , _periodic(periodic)
       , _overlap(overlap)
       , keep_ovlp(true)
       , adaptRefCount(0)
       , adaptActive(false)
@@ -751,15 +737,15 @@
       _levels.resize(1);
 
       // Number of elements per coordinate direction on the coarsest level
       for (std::size_t i=0; i<dim; i++)
         _coarseSize[i] = coordinates.size(i);
 
       // Construct the communication torus
-      _torus = decltype(_torus)(comm,tag,_coarseSize,overlap,partitioner);
+      _torus = decltype(_torus)(comm,tag,_coarseSize,lb);
 
       iTupel o;
       std::fill(o.begin(), o.end(), 0);
       iTupel o_interior(o);
       iTupel s_interior(_coarseSize);
 
       _torus.partition(_torus.rank(),o,_coarseSize,o_interior,s_interior);
@@ -899,26 +885,26 @@
     }
 
     /** Standard constructor for an equidistant YaspGrid
      *  @param L extension of the domain
      *  @param s number of cells on coarse mesh in each direction
      *  @param periodic tells if direction is periodic or not
      *  @param overlap size of overlap on coarsest grid (same in all directions)
-     *  @param comm the communication object for this grid. An MPI communicator can be given here.
-     *  @param partitioner pointer to an overloaded Yasp::Partitioning instance
+     *  @param comm the collective communication object for this grid. An MPI communicator can be given here.
+     *  @param lb pointer to an overloaded YLoadBalance instance
      */
     template<class C = Coordinates,
              typename std::enable_if_t< std::is_same_v<C, EquidistantCoordinates<ctype,dim> >, int> = 0>
     YaspGrid (Dune::FieldVector<ctype, dim> L,
               std::array<int, std::size_t{dim}> s,
               std::bitset<std::size_t{dim}> periodic = std::bitset<std::size_t{dim}>{0ULL},
               int overlap = 1,
-              Communication comm = Communication(),
-              const Yasp::Partitioning<dim>* partitioner = defaultPartitioner())
-      : ccobj(comm), _torus(comm,tag,s,overlap,partitioner), leafIndexSet_(*this),
+              CollectiveCommunicationType comm = CollectiveCommunicationType(),
+              const YLoadBalance<dim>* lb = defaultLoadbalancer())
+      : ccobj(comm), _torus(comm,tag,s,lb), leafIndexSet_(*this),
         _L(L), _periodic(periodic), _coarseSize(s), _overlap(overlap),
         keep_ovlp(true), adaptRefCount(0), adaptActive(false)
     {
       _levels.resize(1);
 
       iTupel o;
       std::fill(o.begin(), o.end(), 0);
@@ -928,15 +914,15 @@
       _torus.partition(_torus.rank(),o,s,o_interior,s_interior);
 
 #if HAVE_MPI
       // check whether the grid is large enough to be overlapping
       for (int i=0; i<dim; i++)
       {
         // find out whether the grid is too small to
-        int toosmall = (s_interior[i] < 2*overlap) &&    // interior is very small
+        int toosmall = (s_interior[i] / 2 <= overlap) &&    // interior is very small
             (periodic[i] || (s_interior[i] != s[i]));    // there is an overlap in that direction
         // communicate the result to all those processes to have all processors error out if one process failed.
         int global = 0;
         MPI_Allreduce(&toosmall, &global, 1, MPI_INT, MPI_LOR, comm);
         if (global)
           DUNE_THROW(Dune::GridError,"YaspGrid does not support degrees of freedom shared by more than immediately neighboring subdomains."
                                      " Note that this also holds for DOFs on subdomain boundaries."
@@ -969,27 +955,27 @@
 
     /** Constructor for an equidistant YaspGrid with non-trivial origin
      *  @param lowerleft Lower left corner of the domain
      *  @param upperright Upper right corner of the domain
      *  @param s number of cells on coarse mesh in each direction
      *  @param periodic tells if direction is periodic or not
      *  @param overlap size of overlap on coarsest grid (same in all directions)
-     *  @param comm the communication object for this grid. An MPI communicator can be given here.
-     *  @param partitioner pointer to an overloaded Yasp::Partitioning instance
+     *  @param comm the collective communication object for this grid. An MPI communicator can be given here.
+     *  @param lb pointer to an overloaded YLoadBalance instance
      */
     template<class C = Coordinates,
              typename std::enable_if_t< std::is_same_v<C, EquidistantOffsetCoordinates<ctype,dim> >, int> = 0>
     YaspGrid (Dune::FieldVector<ctype, dim> lowerleft,
               Dune::FieldVector<ctype, dim> upperright,
               std::array<int, std::size_t{dim}> s,
               std::bitset<std::size_t{dim}> periodic = std::bitset<std::size_t{dim}>(0ULL),
               int overlap = 1,
-              Communication comm = Communication(),
-              const Yasp::Partitioning<dim>* partitioner = defaultPartitioner())
-      : ccobj(comm), _torus(comm,tag,s,overlap,partitioner), leafIndexSet_(*this),
+              CollectiveCommunicationType comm = CollectiveCommunicationType(),
+              const YLoadBalance<dim>* lb = defaultLoadbalancer())
+      : ccobj(comm), _torus(comm,tag,s,lb), leafIndexSet_(*this),
         _L(upperright - lowerleft),
         _periodic(periodic), _coarseSize(s), _overlap(overlap),
         keep_ovlp(true), adaptRefCount(0), adaptActive(false)
     {
       _levels.resize(1);
 
       iTupel o;
@@ -1000,15 +986,15 @@
       _torus.partition(_torus.rank(),o,s,o_interior,s_interior);
 
 #if HAVE_MPI
       // check whether the grid is large enough to be overlapping
       for (int i=0; i<dim; i++)
       {
         // find out whether the grid is too small to
-        int toosmall = (s_interior[i] < 2*overlap) &&    // interior is very small
+        int toosmall = (s_interior[i] / 2 <= overlap) &&    // interior is very small
             (periodic[i] || (s_interior[i] != s[i]));    // there is an overlap in that direction
         // communicate the result to all those processes to have all processors error out if one process failed.
         int global = 0;
         MPI_Allreduce(&toosmall, &global, 1, MPI_INT, MPI_LOR, comm);
         if (global)
           DUNE_THROW(Dune::GridError,"YaspGrid does not support degrees of freedom shared by more than immediately neighboring subdomains."
                                      " Note that this also holds for DOFs on subdomain boundaries."
@@ -1038,25 +1024,25 @@
       init();
     }
 
     /** @brief Standard constructor for a tensorproduct YaspGrid
      *  @param coords coordinate vectors to be used for coarse grid
      *  @param periodic tells if direction is periodic or not
      *  @param overlap size of overlap on coarsest grid (same in all directions)
-     *  @param comm the communication object for this grid. An MPI communicator can be given here.
-     *  @param partitioner pointer to an overloaded Yasp::Partitioning instance
+     *  @param comm the collective communication object for this grid. An MPI communicator can be given here.
+     *  @param lb pointer to an overloaded YLoadBalance instance
      */
     template<class C = Coordinates,
              typename std::enable_if_t< std::is_same_v<C, TensorProductCoordinates<ctype,dim> >, int> = 0>
     YaspGrid (std::array<std::vector<ctype>, std::size_t{dim}> coords,
               std::bitset<std::size_t{dim}> periodic = std::bitset<std::size_t{dim}>(0ULL),
               int overlap = 1,
-              Communication comm = Communication(),
-              const Yasp::Partitioning<dim>* partitioner = defaultPartitioner())
-      : ccobj(comm), _torus(comm,tag,Dune::Yasp::sizeArray<dim>(coords),overlap,partitioner),
+              CollectiveCommunicationType comm = CollectiveCommunicationType(),
+              const YLoadBalance<dim>* lb = defaultLoadbalancer())
+      : ccobj(comm), _torus(comm,tag,Dune::Yasp::sizeArray<dim>(coords),lb),
         leafIndexSet_(*this), _periodic(periodic), _overlap(overlap),
         keep_ovlp(true), adaptRefCount(0), adaptActive(false)
     {
       if (!Dune::Yasp::checkIfMonotonous(coords))
         DUNE_THROW(Dune::GridError,"Setup of a tensorproduct grid requires monotonous sequences of coordinates.");
 
       _levels.resize(1);
@@ -1075,15 +1061,15 @@
       _torus.partition(_torus.rank(),o,_coarseSize,o_interior,s_interior);
 
 #if HAVE_MPI
       // check whether the grid is large enough to be overlapping
       for (int i=0; i<dim; i++)
       {
         // find out whether the grid is too small to
-        int toosmall = (s_interior[i] < 2*overlap) &&               // interior is very small
+        int toosmall = (s_interior[i] / 2 <= overlap) &&               // interior is very small
              (periodic[i] || (s_interior[i] != _coarseSize[i]));    // there is an overlap in that direction
         // communicate the result to all those processes to have all processors error out if one process failed.
         int global = 0;
         MPI_Allreduce(&toosmall, &global, 1, MPI_INT, MPI_LOR, comm);
         if (global)
           DUNE_THROW(Dune::GridError,"YaspGrid does not support degrees of freedom shared by more than immediately neighboring subdomains."
                                      " Note that this also holds for DOFs on subdomain boundaries."
@@ -1149,28 +1135,28 @@
     /** @brief Constructor for a tensorproduct YaspGrid with only coordinate
      *         information on this processor
      *  @param comm MPI communicator where this mesh is distributed to
      *  @param coords coordinate vectors to be used for coarse grid
      *  @param periodic tells if direction is periodic or not
      *  @param overlap size of overlap on coarsest grid (same in all directions)
      *  @param coarseSize the coarse size of the global grid
-     *  @param partitioner pointer to an overloaded Yasp::Partitioning instance
+     *  @param lb pointer to an overloaded YLoadBalance instance
      *
      *  @warning The construction of overlapping coordinate ranges is
      *           an error-prone procedure. For this reason, it is kept private.
      *           You can safely use it through BackupRestoreFacility. All other
      *           use is not supported for the moment.
      */
     YaspGrid (std::array<std::vector<ctype>, std::size_t{dim}> coords,
               std::bitset<std::size_t{dim}> periodic,
               int overlap,
-              Communication comm,
+              CollectiveCommunicationType comm,
               std::array<int,dim> coarseSize,
-              const Yasp::Partitioning<dim>* partitioner = defaultPartitioner())
-      : ccobj(comm), _torus(comm,tag,coarseSize,overlap,partitioner), leafIndexSet_(*this),
+              const YLoadBalance<dim>* lb = defaultLoadbalancer())
+      : ccobj(comm), _torus(comm,tag,coarseSize,lb), leafIndexSet_(*this),
         _periodic(periodic), _coarseSize(coarseSize), _overlap(overlap),
         keep_ovlp(true), adaptRefCount(0), adaptActive(false)
     {
       // check whether YaspGrid has been given the correct template parameter
       static_assert(std::is_same<Coordinates,TensorProductCoordinates<ctype,dim> >::value,
                   "YaspGrid coordinate container template parameter and given constructor values do not match!");
 
@@ -1755,17 +1741,17 @@
     }
 
     const typename Traits::LeafIndexSet& leafIndexSet() const
     {
       return leafIndexSet_;
     }
 
-    /*! @brief return a communication object
+    /*! @brief return a collective communication object
      */
-    const Communication& comm () const
+    const CollectiveCommunicationType& comm () const
     {
       return ccobj;
     }
 
   private:
 
     // number of boundary segments of the level 0 grid
@@ -1853,17 +1839,17 @@
         return YaspLevelIterator<cd,pitype,GridImp>(g,g->overlap[cd].end());
       if (pitype<=All_Partition || pitype == Ghost_Partition)
         return YaspLevelIterator<cd,pitype,GridImp>(g,g->overlapfront[cd].end());
 
       DUNE_THROW(GridError, "YaspLevelIterator with this codim or partition type not implemented");
     }
 
-    Communication ccobj;
+    CollectiveCommunicationType ccobj;
 
-    Torus<Communication,dim> _torus;
+    Torus<CollectiveCommunicationType,dim> _torus;
 
     std::vector< std::shared_ptr< YaspIndexSet<const YaspGrid<dim,Coordinates>, false > > > indexsets;
     YaspIndexSet<const YaspGrid<dim,Coordinates>, true> leafIndexSet_;
     YaspGlobalIdSet<const YaspGrid<dim,Coordinates> > theglobalidset;
 
     Dune::FieldVector<ctype, dim> _L;
     iTupel _s;
@@ -1879,33 +1865,33 @@
 #if __cpp_deduction_guides >= 201611
   // Class template deduction guides
   template<typename ctype, int dim>
   YaspGrid(FieldVector<ctype, dim>,
            std::array<int, std::size_t{dim}>,
            std::bitset<std::size_t{dim}> = std::bitset<std::size_t{dim}>{0ULL},
            int = 1,
-           YaspCommunication = YaspCommunication(),
+           YaspCollectiveCommunication = YaspCollectiveCommunication(),
            const YLoadBalance<dim>* = YaspGrid< dim, EquidistantCoordinates<ctype, dim> >::defaultLoadbalancer())
     -> YaspGrid< dim, EquidistantCoordinates<ctype, dim> >;
 
   template<typename ctype, int dim>
   YaspGrid(FieldVector<ctype, dim>,
            FieldVector<ctype, dim>,
            std::array<int, std::size_t{dim}>,
            std::bitset<std::size_t{dim}> = std::bitset<std::size_t{dim}>{0ULL},
            int = 1,
-           YaspCommunication = YaspCommunication(),
+           YaspCollectiveCommunication = YaspCollectiveCommunication(),
            const YLoadBalance<dim>* = YaspGrid< dim, EquidistantOffsetCoordinates<ctype, dim> >::defaultLoadbalancer())
     -> YaspGrid< dim, EquidistantOffsetCoordinates<ctype, dim> >;
 
   template<typename ctype, std::size_t dim>
   YaspGrid(std::array<std::vector<ctype>, dim>,
            std::bitset<dim> = std::bitset<dim>{0ULL},
            int = 1,
-           YaspCommunication = YaspCommunication(),
+           YaspCollectiveCommunication = YaspCollectiveCommunication(),
            const YLoadBalance<int{dim}>* = YaspGrid< int{dim}, TensorProductCoordinates<ctype, int{dim}> >::defaultLoadbalancer())
     -> YaspGrid< int{dim}, TensorProductCoordinates<ctype, int{dim}> >;
 #endif
 
   //! Output operator for multigrids
   template <int d, class CC>
   std::ostream& operator<< (std::ostream& s, const YaspGrid<d,CC>& grid)
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/capabilities.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/capabilities.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_CAPABILITIES_HH
 #define DUNE_PYTHON_GRID_CAPABILITIES_HH
 
 #include <type_traits>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/entity.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/entity.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_ENTITY_HH
 #define DUNE_PYTHON_GRID_ENTITY_HH
 
 #include <string>
 #include <tuple>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/factory.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/factory.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_FACTORY_HH
 #define DUNE_PYTHON_GRID_FACTORY_HH
 
 #include <cstddef>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/function.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/function.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_FUNCTION_HH
 #define DUNE_PYTHON_GRID_FUNCTION_HH
 
 #include <functional>
 #include <string>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/geometry.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/geometry.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_PYTHON_GRID_GEOMETRY_HH
 #define DUNE_PYTHON_GRID_GEOMETRY_HH
 
 #include <cstddef>
@@ -50,15 +48,15 @@
         // g = (dimRange,localCoord,nofQuad)
         auto g = gVec.unchecked();
         // ret = (dimRange,globalCoord,nofQuad)
         pybind11::array_t< double > ret( std::array< ssize_t, 3 >{{ g.shape( 0 ), static_cast< ssize_t >( Geometry::GlobalCoordinate::size() ), g.shape( 2 ) }} );
         auto y = ret.template mutable_unchecked< 3 >();
         if( x.shape( 1 ) != g.shape( 2 ) )
           std::cout << x.shape( 1 ) << " " << g.shape( 2 ) << std::endl;
-        if( x.shape( 0 ) != ssize_t(LocalCoordinate::size()) )
+        if( x.shape( 0 ) != LocalCoordinate::size() )
           std::cout << x.shape( 0 ) << " " << Geometry::LocalCoordinate::size() << std::endl;
 
         for( ssize_t p = 0; p < g.shape( 2 ); ++p )
         {
           LocalCoordinate xLocal;
           for( std::size_t l = 0; l < LocalCoordinate::size(); ++l )
             xLocal[ l ] = x( l, p );
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/gridview.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/gridview.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_GRIDPART_HH
 #define DUNE_PYTHON_GRID_GRIDPART_HH
 
 #include <array>
 #include <stdexcept>
@@ -378,20 +376,20 @@
 
       cls.def( "coordinates", [] ( const GridView &self ) { return coordinates( self ); },
         R"doc(
           Returns: `numpy` array with the coordinates of all vertices in the grid in
                    the format `[ [x_1,y_1], [x_2,y_2], ..., [x_N,y_N] ]` for example
                    in 2d.
         )doc" );
-      cls.def( "tessellate", [] ( const GridView &self, int level ) { return tessellate( self, level ); }, "level"_a = 0,
+      cls.def( "tesselate", [] ( const GridView &self, int level ) { return tesselate( self, level ); }, "level"_a = 0,
         R"doc(
-          Generated a possibly refined tessellation using only simplices.
+          Generated a possibly refined tesselation using only simplices.
 
           Args:
-              level: virtual refinement level to use to generate the tessellation
+              level: virtual refinement level to use to generate the tesselation
 
           Returns: (coordinates,simplices) where coordinates is a `numpy` array
                    of the vertex coodinates
                    (e.g. in 2d `[ [x_1,y_1], [x_2,y_2], ..., [x_N,y_N] ]` )
                    and simplices is a `numpy` array of the vertices of the simplices
                    (e.g. in 2d `[s_11,s_12,s_13], [s_21,s_22,s_23], ..., [s_N1,s_N2,s_N3] ]` )
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/hierarchical.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/hierarchical.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_HIERARCHICAL_HH
 #define DUNE_PYTHON_GRID_HIERARCHICAL_HH
 
 #include <array>
 #include <functional>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/idset.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/idset.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_IDSET_HH
 #define DUNE_PYTHON_GRID_IDSET_HH
 
 #include <functional>
 #include <tuple>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/indexset.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/indexset.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_INDEXSET_HH
 #define DUNE_PYTHON_GRID_INDEXSET_HH
 
 #include <string>
 #include <tuple>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/intersection.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/intersection.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_INTERSECTION_HH
 #define DUNE_PYTHON_GRID_INTERSECTION_HH
 
 #include <dune/common/visibility.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/localview.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/localview.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_GRID_LOCALVIEW_HH
 #define DUNE_PYTHON_GRID_LOCALVIEW_HH
 
 #include <map>
 
 #include <dune/common/visibility.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/mapper.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/mapper.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_MAPPER_HH
 #define DUNE_PYTHON_GRID_MAPPER_HH
 
 #include <functional>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/numpy.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/numpy.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_GRID_NUMPY_HH
 #define DUNE_PYTHON_GRID_NUMPY_HH
 
 #include <cassert>
 #include <cstddef>
 
 #include <algorithm>
@@ -119,17 +117,18 @@
       return result;
     }
 
 
 
     // tessellate
     // ----------
+
     template< class GridView, unsigned int partitions >
     inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tessellate ( const GridView &gridView, RefinementIntervals intervals, PartitionSet< partitions > ps )
+    tesselate ( const GridView &gridView, RefinementIntervals intervals, PartitionSet< partitions > ps )
     {
       typedef typename GridView::ctype ctype;
 
       const std::size_t dimGrid = GridView::dimension;
       const std::size_t dimWorld = GridView::dimensionworld;
 
       std::vector< FieldVector< ctype, dimWorld > > coords;
@@ -157,17 +156,17 @@
       }
 
       return std::make_pair( makeNumPyArray< ctype >( coords, { coords.size(), dimWorld } ), makeNumPyArray< int >( simplices, { simplices.size(), dimGrid+1 } ) );
     }
 
     template< class GridView, unsigned int partitions >
     inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tessellate ( const GridView &gridView, int level, PartitionSet< partitions > ps )
+    tesselate ( const GridView &gridView, int level, PartitionSet< partitions > ps )
     {
-      return tessellate( gridView, refinementLevels( level ), ps );
+      return tesselate( gridView, refinementLevels( level ), ps );
     }
 
     template< class GridView, unsigned int partitions >
     inline static std::vector< pybind11::array_t< typename GridView::ctype > >
     polygons ( const GridView &gridView, PartitionSet< partitions > ps )
     {
       typedef typename GridView::ctype ctype;
@@ -251,24 +250,24 @@
         values.push_back( Python::makeNumPyArray< typename FieldTraits< Range >::field_type >( entry.second.second, { entry.second.second.size(), GetDimension<Range>::value } ) );
       }
       return std::make_pair(ret, values);
     }
 
     template< class GridView, unsigned int partitions >
     inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tessellate ( const GridView &gridView, PartitionSet< partitions > ps )
+    tesselate ( const GridView &gridView, PartitionSet< partitions > ps )
     {
-      return tessellate( gridView, 0, ps );
+      return tesselate( gridView, 0, ps );
     }
 
     template< class GridView >
     inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tessellate ( const GridView &gridView, int level = 0 )
+    tesselate ( const GridView &gridView, int level = 0 )
     {
-      return tessellate( gridView, level, Partitions::all );
+      return tesselate( gridView, level, Partitions::all );
     }
 
     template< class GridView >
     inline static std::vector< pybind11::array_t< typename GridView::ctype > >
     polygons ( const GridView &gridView )
     {
       return polygons( gridView, Partitions::all );
@@ -365,35 +364,12 @@
 
     template< class GridFunction >
     inline static auto cellData ( const GridFunction &gridFunction, int level = 0 )
     {
       return cellData( gridFunction, level, Partitions::all );
     }
 
-
-    // deprecated tesselate (note spelling) functions
-    template< class GridView, unsigned int partitions >
-    [[deprecated("use 'tessellate' (note spelling)")]]
-    inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tesselate ( const GridView &gridView, RefinementIntervals intervals, PartitionSet< partitions > ps )
-    { return tessellate( gridView, intervals, ps); }
-    template< class GridView, unsigned int partitions >
-    [[deprecated("use 'tessellate' (note spelling)")]]
-    inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tesselate ( const GridView &gridView, int level, PartitionSet< partitions > ps )
-    { return tessellate( gridView, level, ps); }
-    template< class GridView, unsigned int partitions >
-    [[deprecated("use 'tessellate' (note spelling)")]]
-    inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tesselate ( const GridView &gridView, PartitionSet< partitions > ps )
-    { return tessellate( gridView, ps); }
-    template< class GridView >
-    [[deprecated("use 'tessellate' (note spelling)")]]
-    inline static std::pair< pybind11::array_t< typename GridView::ctype >, pybind11::array_t< int > >
-    tesselate ( const GridView &gridView, int level = 0 )
-    { tessellate(gridView, level); }
-
   } // namespace FemPy
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_PYTHON_GRID_NUMPY_HH
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/numpycommdatahandle.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/numpycommdatahandle.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_UTILITY_VECTORCOMMDATAHANDLE_HH
 #define DUNE_PYTHON_UTILITY_VECTORCOMMDATAHANDLE_HH
 
 #include <cassert>
 #include <cstddef>
 
 #include <algorithm>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/object.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/object.hh`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_GRID_OBJECT_HH
 #define DUNE_PYTHON_GRID_OBJECT_HH
 
 #include <type_traits>
 #include <utility>
 
 #include <dune/common/typeutilities.hh>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/persistentcontainer.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/persistentcontainer.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_PERSISTENTCONTAINER_HH
 #define DUNE_PYTHON_GRID_PERSISTENTCONTAINER_HH
 
 #include <array>
 #include <stdexcept>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/pygridfunction.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/pygridfunction.hh`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_GRID_PY_PYFUNCTION_HH
 #define DUNE_GRID_PY_PYFUNCTION_HH
 
 #include <string>
 #include <utility>
 
 #include <dune/python/pybind11/pybind11.h>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/range.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/range.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 #ifndef DUNE_PYTHON_GRID_RANGE_HH
 #define DUNE_PYTHON_GRID_RANGE_HH
 
 #include <string>
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/simplegridfunction.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/simplegridfunction.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 #ifndef DUNE_PYTHON_FUNCTION_SIMPLEGRIDFUNCTION_HH
 #define DUNE_PYTHON_FUNCTION_SIMPLEGRIDFUNCTION_HH
 
 #include <cassert>
 
 #include <type_traits>
 #include <utility>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/grid/vtk.hh` & `dune-grid-2.9.dev20220529/dune/python/grid/vtk.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 2; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #ifndef DUNE_PYTHON_GRID_VTK_HH
 #define DUNE_PYTHON_GRID_VTK_HH
 
 #include <type_traits>
```

### Comparing `dune-grid-2.9.0rc1/dune/python/test/backrest1.py` & `dune-grid-2.9.dev20220529/dune/python/test/backrest1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import pickle, numpy
 import dune.generator
 
 def backup():
     from dune.grid import structuredGrid
     grid = structuredGrid([0,0],[1,1],[2,2])
     grid.hierarchicalGrid.globalRefine(2)
```

### Comparing `dune-grid-2.9.0rc1/dune/python/test/interpolate.py` & `dune-grid-2.9.dev20220529/dune/python/test/interpolate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import time, math, numpy, io
 import dune
 from dune.generator import algorithm
 import dune.geometry
 from dune.grid import cartesianDomain
 from dune.grid import yaspGrid as gridView
```

### Comparing `dune-grid-2.9.0rc1/dune/python/test/test-ug.py` & `dune-grid-2.9.dev20220529/dune/python/test/test-ug.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import math
 import dune.common
 import dune.grid
 import sys
 
 # initialize MPI *if present*
 try:
```

### Comparing `dune-grid-2.9.0rc1/dune/python/test/test_gf2.py` & `dune-grid-2.9.dev20220529/dune/python/test/test_gf2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from io import StringIO
 import math
 from dune.common import FieldVector
 from dune.grid import gridFunction, structuredGrid
 
 codeFunc = """
 #include <cmath>
```

### Comparing `dune-grid-2.9.0rc1/lib/dunegridam2cmake.lib` & `dune-grid-2.9.dev20220529/lib/dunegridam2cmake.lib`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*-sh-*-
-# SPDX-FileCopyrightInfo: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 
 ##########################################
 ###
 ### Function for converting configure options
 ### to CMake options for dune-grid
 ###
 ##########################################
```

### Comparing `dune-grid-2.9.0rc1/pyproject.toml` & `dune-grid-2.9.dev20220529/pyproject.toml`

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

### Comparing `dune-grid-2.9.0rc1/python/dune/grid/__init__.py` & `dune-grid-2.9.dev20220529/python/dune/grid/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from ._grid import *
 from .core import *
 
 from ._grids import *
 
 from dune.common import FieldVector
 from dune.common.utility import getNumberOfParameters
```

### Comparing `dune-grid-2.9.0rc1/python/dune/grid/_grid.cc` & `dune-grid-2.9.dev20220529/python/dune/grid/_grid.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-// SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-// SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
 // -*- tab-width: 4; indent-tabs-mode: nil; c-basic-offset: 2 -*-
 // vi: set et ts=4 sw=2 sts=2:
 
 #include <dune/grid/common/gridenums.hh>
 #include <dune/grid/io/file/vtk/vtkwriter.hh>
 
 #include <dune/python/grid/commops.hh>
```

### Comparing `dune-grid-2.9.0rc1/python/dune/grid/_grids.py` & `dune-grid-2.9.dev20220529/python/dune/grid/_grids.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,19 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 from dune.common.checkconfiguration import assertCMakeHave, ConfigurationError
 from dune.typeregistry import generateTypeName
 
 class CartesianDomain(tuple):
-    @staticmethod
-    def bndDomain(lower, upper):
-        bnd = ""
-        lower = list(lower)
-        upper = list(upper)
-        dim = len(lower)
-        for i in range(dim):
-            l = lower.copy()
-            u = upper.copy()
-            l[i] -= 1e-5
-            u[i] = lower[i]
-
-            bnd += str(2*i+1) + " " + " ".join(str(x) for x in l) +\
-                                " " + " ".join(str(x) for x in u) + "\n"
-            l = lower.copy()
-            u = upper.copy()
-            l[i] = upper[i]
-            u[i] = upper[i] + 1e-5
-            bnd += str(2*i+2) + " " + " ".join(str(x) for x in l) +\
-                                " " + " ".join(str(x) for x in u) + "\n"
-        return bnd
-
-    def __new__ (cls, lower,upper,division,boundary=True,**parameters):
+    def __new__ (cls, lower,upper,division,**parameters):
         from ._grid import reader
-
         dgf = "DGF\n"
         dgf += "INTERVAL\n"
         dgf += " ".join([str(x) for x in lower]) + "\n"
         dgf += " ".join([str(x) for x in upper]) + "\n"
         dgf += " ".join([str(x) for x in division]) + "\n"
         dgf += "#\n"
-
-        if boundary:
-            dgf += "BOUNDARYDOMAIN\n"
-            dgf += CartesianDomain.bndDomain(lower,upper)
-            dgf += "#\n"
-
         dgf += "GRIDPARAMETER\n"
         foundRefEdge = False
         for key in parameters:
             if key.lower() == 'refinementedge':
                 foundRefEdge = True
             dgf += key + " " + str(parameters[key]) + "\n"
         # set default value for refinementedge if not provided to avoid warning
@@ -71,21 +39,20 @@
                             else "0" for j in range(dim)])
                         dgf += "\n"
                 dgf += "#\n"
         except KeyError:
             pass
         return super(CartesianDomain, cls).__new__(cls,
                        tuple( (reader.dgfString, dgf) ) )
-    def __init__(self,lower,upper,division,boundary=True,**parameters):
+    def __init__(self,lower,upper,division,**parameters):
         self.dimgrid = len(lower)
         self.lower = lower
         self.upper = upper
         self.division = division
         self.param = parameters
-        self.boundaryWasSet = boundary
     def dimgrid(self):
         return self.dimgrid
 
 def onedGrid(constructor):
     from .grid_generator import module, getDimgrid
 
     typeName = "Dune::OneDGrid"
```

### Comparing `dune-grid-2.9.0rc1/python/dune/grid/grid_generator.py` & `dune-grid-2.9.dev20220529/python/dune/grid/grid_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import os, inspect
 from ..generator.generator import SimpleGenerator
 from dune.common.hashit import hashIt
 from dune.common import FieldVector
 from dune.common.utility import isString
 from dune.deprecate import deprecated
 from dune.grid import gridFunction, DataType
 from dune.grid import OutputType
 from dune.generator.algorithm import cppType
 from dune.generator import builder
-from dune.deprecate import deprecated
 
 def getDimgrid(constructor):
     dimgrid = None
     if not dimgrid:
         try:
             dimgrid = constructor.dimgrid
         except AttributeError:
@@ -29,15 +25,15 @@
         raise ValueError("Couldn't extract dimension of grid from constructor arguments, added dimgrid parameter")
     return dimgrid
 
 def triangulation(grid, level=0):
     if grid.dimGrid != 2:
         raise Exception("Grid must be 2-dimensional for use as matplotlib triangulation.")
     from matplotlib.tri import Triangulation
-    x, triangles = grid.tessellate(level)
+    x, triangles = grid.tesselate(level)
     return Triangulation(x[:,0], x[:,1], triangles)
 
 _writeVTKDispatcher = []
 def _writeVTK(vtk,grid,f,name,dataTag):
     done = False
     try:
         f.addToVTKWriter(name, vtk, dataTag)
@@ -289,19 +285,14 @@
     return gf
 
 def addAttr(module, cls):
     setattr(cls, "_module", module)
     setattr(cls, "writeVTK", writeVTK)
     setattr(cls, "sequencedVTK", sequencedVTK)
     setattr(cls, "_functions", {})
-    @deprecated(name="dune.grid.GridView.tesselate", msg="Use 'tessellate' (note spelling)")
-    def tesselate(gv, *args,**kwargs):
-        return gv.tessellate(*args,**kwargs)
-    setattr(cls,"tesselate", tesselate)
-    [[deprecated("use 'tessellate' (note spelling)")]]
 
     if cls.dimension == 2:
         setattr(cls, "plot", plot)
         setattr(cls, "triangulation", triangulation)
     else:
         def throwFunc(msg):
             def throw(*args, **kwargs):
```

### Comparing `dune-grid-2.9.0rc1/python/dune/grid/tutorial/circle1storder.msh` & `dune-grid-2.9.dev20220529/python/dune/grid/tutorial/circle1storder.msh`

 * *Files identical despite different names*

### Comparing `dune-grid-2.9.0rc1/python/dune/grid/tutorial/example.py` & `dune-grid-2.9.dev20220529/python/dune/grid/tutorial/example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 import math
 import sys, os
 
 # find grid files relative to example.py script
 griddir = os.path.dirname(sys.argv[0])
 
 # example of how to perform operations on a given grid
```

### Comparing `dune-grid-2.9.0rc1/python/dune_grid.egg-info/PKG-INFO` & `dune-grid-2.9.dev20220529/python/dune_grid.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: dune-grid
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: module providing main interfaces for setting and traversing grids
 Home-page: https://gitlab.dune-project.org/core/dune-grid
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
         
         
-        git-d29ed3fdccc0087bfba94d907cca3abd85b55cf3
+        git-ce5efe9e428f6c22bc9e8484e45c8365114ee95e
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-grid-2.9.0rc1/python/dune_grid.egg-info/SOURCES.txt` & `dune-grid-2.9.dev20220529/python/dune_grid.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 LICENSE.md
 README.md
 config.h.cmake
 dune-grid.pc.in
 dune.module
 pyproject.toml
 setup.py
-LICENSES/LicenseRef-GPL-2.0-only-with-DUNE-exception.txt
 cmake/modules/AddAlbertaFlags.cmake
 cmake/modules/CMakeLists.txt
 cmake/modules/DuneGridMacros.cmake
 cmake/modules/FindAlberta.cmake
 cmake/modules/GridType.cmake
 cmake/modules/UseUG.cmake
 doc/CMakeLists.txt
@@ -81,71 +80,46 @@
 doc/grids/dgf/test3d.dgf
 doc/grids/dgf/torus-2.dgf
 doc/grids/dgf/torus-3.dgf
 doc/grids/dgf/unstr_cube.dgf
 doc/grids/gmsh/CMakeLists.txt
 doc/grids/gmsh/circle.geo
 doc/grids/gmsh/circle1storder.msh
-doc/grids/gmsh/circle1storder.msh.license
 doc/grids/gmsh/circle2ndorder.msh
-doc/grids/gmsh/circle2ndorder.msh.license
 doc/grids/gmsh/curved2d.geo
 doc/grids/gmsh/curved2d.msh
-doc/grids/gmsh/curved2d.msh.license
 doc/grids/gmsh/hybrid-testgrid-2d.msh
-doc/grids/gmsh/hybrid-testgrid-2d.msh.license
 doc/grids/gmsh/hybrid-testgrid-3d.msh
-doc/grids/gmsh/hybrid-testgrid-3d.msh.license
 doc/grids/gmsh/oned-testgrid.msh
-doc/grids/gmsh/oned-testgrid.msh.license
 doc/grids/gmsh/pyramid.geo
 doc/grids/gmsh/pyramid.msh
-doc/grids/gmsh/pyramid.msh.license
 doc/grids/gmsh/pyramid1storder.msh
-doc/grids/gmsh/pyramid1storder.msh.license
 doc/grids/gmsh/pyramid2ndorder.msh
-doc/grids/gmsh/pyramid2ndorder.msh.license
 doc/grids/gmsh/pyramid4.msh
-doc/grids/gmsh/pyramid4.msh.license
 doc/grids/gmsh/sphere.msh
-doc/grids/gmsh/sphere.msh.license
 doc/grids/gmsh/telescope.geo
 doc/grids/gmsh/telescope.msh
-doc/grids/gmsh/telescope.msh.license
 doc/grids/gmsh/telescope1storder.msh
-doc/grids/gmsh/telescope1storder.msh.license
 doc/grids/gmsh/telescope2ndorder.msh
-doc/grids/gmsh/telescope2ndorder.msh.license
 doc/grids/gmsh/twotets.geo
 doc/grids/gmsh/twotets.msh
-doc/grids/gmsh/twotets.msh.license
 doc/grids/gmsh/unitcube.msh
-doc/grids/gmsh/unitcube.msh.license
 doc/grids/gmsh/unitsquare_quads_2x2.msh
-doc/grids/gmsh/unitsquare_quads_2x2.msh.license
 doc/grids/gridfactory/CMakeLists.txt
 doc/grids/gridfactory/hybridtestgrids.hh
 doc/grids/gridfactory/testgrids.hh
 doc/grids/starcd/CMakeLists.txt
 doc/grids/starcd/star.cel
-doc/grids/starcd/star.cel.license
 doc/grids/starcd/star.vrt
-doc/grids/starcd/star.vrt.license
 doc/grids/starcd/tets.cel
-doc/grids/starcd/tets.cel.license
 doc/grids/starcd/tets.vrt
-doc/grids/starcd/tets.vrt.license
 doc/grids/starcd/withprism.cel
-doc/grids/starcd/withprism.cel.license
 doc/grids/starcd/withprism.vrt
-doc/grids/starcd/withprism.vrt.license
 doc/grids/starcd/withpyramid.cel
-doc/grids/starcd/withpyramid.cel.license
 doc/grids/starcd/withpyramid.vrt
-doc/grids/starcd/withpyramid.vrt.license
 doc/recipes/CMakeLists.txt
 doc/recipes/mainpage.txt
 doc/recipes/recipe-integration.cc
 doc/recipes/recipe-iterate-over-grid.cc
 dune/CMakeLists.txt
 dune/grid/CMakeLists.txt
 dune/grid/albertagrid.hh
@@ -203,58 +177,47 @@
 dune/grid/albertagrid/structuredgridfactory.hh
 dune/grid/albertagrid/transformation.hh
 dune/grid/albertagrid/treeiterator.hh
 dune/grid/albertagrid/undefAllMacros.pl
 dune/grid/albertagrid/undefine-2.0.hh
 dune/grid/albertagrid/undefine-3.0.hh
 dune/grid/albertagrid/doc/alberta_tetrahedron.svg
-dune/grid/albertagrid/doc/alberta_tetrahedron.svg.license
 dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg
-dune/grid/albertagrid/doc/alberta_tetrahedron_edges.svg.license
 dune/grid/albertagrid/doc/alberta_triangle.svg
-dune/grid/albertagrid/doc/alberta_triangle.svg.license
 dune/grid/albertagrid/test/CMakeLists.txt
 dune/grid/albertagrid/test/test-alberta3d-refine.cc
 dune/grid/common/CMakeLists.txt
 dune/grid/common/adaptcallback.hh
 dune/grid/common/backuprestore.hh
 dune/grid/common/boundaryprojection.hh
 dune/grid/common/boundarysegment.hh
 dune/grid/common/capabilities.hh
 dune/grid/common/cube-to-tet-6.png
-dune/grid/common/cube-to-tet-6.png.license
 dune/grid/common/cube-to-tet-6.svg
-dune/grid/common/cube-to-tet-6.svg.license
 dune/grid/common/datahandleif.hh
 dune/grid/common/defaultgridview.hh
 dune/grid/common/entity.hh
 dune/grid/common/entityiterator.hh
 dune/grid/common/entityseed.hh
 dune/grid/common/exceptions.hh
 dune/grid/common/geometry.hh
 dune/grid/common/grid.hh
 dune/grid/common/gridenums.hh
 dune/grid/common/gridfactory.hh
 dune/grid/common/gridinfo.hh
 dune/grid/common/gridview.hh
 dune/grid/common/idlocalref.eps
-dune/grid/common/idlocalref.eps.license
 dune/grid/common/idlocalref.fig
-dune/grid/common/idlocalref.fig.license
 dune/grid/common/idlocalref.png
-dune/grid/common/idlocalref.png.license
 dune/grid/common/indexidset.hh
 dune/grid/common/intersection.hh
 dune/grid/common/intersectioniterator.hh
 dune/grid/common/islocalref.eps
-dune/grid/common/islocalref.eps.license
 dune/grid/common/islocalref.fig
-dune/grid/common/islocalref.fig.license
 dune/grid/common/islocalref.png
-dune/grid/common/islocalref.png.license
 dune/grid/common/mapper.hh
 dune/grid/common/mcmgmapper.hh
 dune/grid/common/partitionset.hh
 dune/grid/common/rangegenerators.hh
 dune/grid/common/scsgmapper.hh
 dune/grid/common/sizecache.hh
 dune/grid/common/test/CMakeLists.txt
@@ -272,15 +235,14 @@
 dune/grid/geometrygrid/entity.hh
 dune/grid/geometrygrid/entityseed.hh
 dune/grid/geometrygrid/geometry.hh
 dune/grid/geometrygrid/grid.hh
 dune/grid/geometrygrid/gridfamily.hh
 dune/grid/geometrygrid/gridview.hh
 dune/grid/geometrygrid/helix.png
-dune/grid/geometrygrid/helix.png.license
 dune/grid/geometrygrid/hostcorners.hh
 dune/grid/geometrygrid/identity.hh
 dune/grid/geometrygrid/idset.hh
 dune/grid/geometrygrid/indexsets.hh
 dune/grid/geometrygrid/intersection.hh
 dune/grid/geometrygrid/intersectioniterator.hh
 dune/grid/geometrygrid/iterator.hh
@@ -347,77 +309,46 @@
 dune/grid/io/file/dgfparser/blocks/simplex.cc
 dune/grid/io/file/dgfparser/blocks/simplex.hh
 dune/grid/io/file/dgfparser/blocks/simplexgeneration.cc
 dune/grid/io/file/dgfparser/blocks/simplexgeneration.hh
 dune/grid/io/file/dgfparser/blocks/vertex.cc
 dune/grid/io/file/dgfparser/blocks/vertex.hh
 dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png
-dune/grid/io/file/dgfparser/test/BBEETH1M.d_cut.png.license
 dune/grid/io/file/dgfparser/test/CMakeLists.txt
 dune/grid/io/file/dgfparser/test/Orb_cut.png
-dune/grid/io/file/dgfparser/test/Orb_cut.png.license
 dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png
-dune/grid/io/file/dgfparser/test/bunny.p65.param_skin.png.license
 dune/grid/io/file/dgfparser/test/checkdgf.hh
 dune/grid/io/file/dgfparser/test/example-projection.png
-dune/grid/io/file/dgfparser/test/example-projection.png.license
 dune/grid/io/file/dgfparser/test/examplegrid10.png
-dune/grid/io/file/dgfparser/test/examplegrid10.png.license
 dune/grid/io/file/dgfparser/test/examplegrid10a.png
-dune/grid/io/file/dgfparser/test/examplegrid10a.png.license
 dune/grid/io/file/dgfparser/test/examplegrid10b.png
-dune/grid/io/file/dgfparser/test/examplegrid10b.png.license
 dune/grid/io/file/dgfparser/test/examplegrid10c.png
-dune/grid/io/file/dgfparser/test/examplegrid10c.png.license
 dune/grid/io/file/dgfparser/test/examplegrid10s.png
-dune/grid/io/file/dgfparser/test/examplegrid10s.png.license
 dune/grid/io/file/dgfparser/test/examplegrid11a.png
-dune/grid/io/file/dgfparser/test/examplegrid11a.png.license
 dune/grid/io/file/dgfparser/test/examplegrid11b.png
-dune/grid/io/file/dgfparser/test/examplegrid11b.png.license
 dune/grid/io/file/dgfparser/test/examplegrid12_1.png
-dune/grid/io/file/dgfparser/test/examplegrid12_1.png.license
 dune/grid/io/file/dgfparser/test/examplegrid12_2.png
-dune/grid/io/file/dgfparser/test/examplegrid12_2.png.license
 dune/grid/io/file/dgfparser/test/examplegrid1c.png
-dune/grid/io/file/dgfparser/test/examplegrid1c.png.license
 dune/grid/io/file/dgfparser/test/examplegrid1cs.png
-dune/grid/io/file/dgfparser/test/examplegrid1cs.png.license
 dune/grid/io/file/dgfparser/test/examplegrid1gen.png
-dune/grid/io/file/dgfparser/test/examplegrid1gen.png.license
 dune/grid/io/file/dgfparser/test/examplegrid1genangle.png
-dune/grid/io/file/dgfparser/test/examplegrid1genangle.png.license
 dune/grid/io/file/dgfparser/test/examplegrid1s.png
-dune/grid/io/file/dgfparser/test/examplegrid1s.png.license
 dune/grid/io/file/dgfparser/test/examplegrid2a.png
-dune/grid/io/file/dgfparser/test/examplegrid2a.png.license
 dune/grid/io/file/dgfparser/test/examplegrid2b.png
-dune/grid/io/file/dgfparser/test/examplegrid2b.png.license
 dune/grid/io/file/dgfparser/test/examplegrid2c.png
-dune/grid/io/file/dgfparser/test/examplegrid2c.png.license
 dune/grid/io/file/dgfparser/test/examplegrid2d.png
-dune/grid/io/file/dgfparser/test/examplegrid2d.png.license
 dune/grid/io/file/dgfparser/test/examplegrid2e.png
-dune/grid/io/file/dgfparser/test/examplegrid2e.png.license
 dune/grid/io/file/dgfparser/test/examplegrid5c.png
-dune/grid/io/file/dgfparser/test/examplegrid5c.png.license
 dune/grid/io/file/dgfparser/test/examplegrid5s.png
-dune/grid/io/file/dgfparser/test/examplegrid5s.png.license
 dune/grid/io/file/dgfparser/test/examplegrid6c.png
-dune/grid/io/file/dgfparser/test/examplegrid6c.png.license
 dune/grid/io/file/dgfparser/test/examplegrid6s.png
-dune/grid/io/file/dgfparser/test/examplegrid6s.png.license
 dune/grid/io/file/dgfparser/test/examplegrid7.png
-dune/grid/io/file/dgfparser/test/examplegrid7.png.license
 dune/grid/io/file/dgfparser/test/examplegrid7angle.png
-dune/grid/io/file/dgfparser/test/examplegrid7angle.png.license
 dune/grid/io/file/dgfparser/test/examplegrid7area.png
-dune/grid/io/file/dgfparser/test/examplegrid7area.png.license
 dune/grid/io/file/dgfparser/test/pmdc.png
-dune/grid/io/file/dgfparser/test/pmdc.png.license
 dune/grid/io/file/dgfparser/test/test-dgf-alberta.cc
 dune/grid/io/file/dgfparser/test/test-dgf-oned.cc
 dune/grid/io/file/dgfparser/test/test-dgf-ug.cc
 dune/grid/io/file/dgfparser/test/test-dgf-yasp.cc
 dune/grid/io/file/dgfparser/utils/CMakeLists.txt
 dune/grid/io/file/dgfparser/utils/dgf2dgf.cc
 dune/grid/io/file/dgfparser/utils/gmsh2dgf.cc
@@ -510,15 +441,14 @@
 dune/grid/test/testiteratorranges.cc
 dune/grid/test/yasp/CMakeLists.txt
 dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistant.cc
 dune/grid/test/yasp/test-yaspgrid-backuprestore-equidistantoffset.cc
 dune/grid/test/yasp/test-yaspgrid-backuprestore-tensor.cc
 dune/grid/test/yasp/test-yaspgrid-constructor.cc
 dune/grid/test/yasp/test-yaspgrid-entityshifttable.cc
-dune/grid/test/yasp/test-yaspgrid-partitioner.cc
 dune/grid/test/yasp/test-yaspgrid-tensorgridfactory.cc
 dune/grid/test/yasp/test-yaspgrid-yaspfactory-1d.cc
 dune/grid/test/yasp/test-yaspgrid-yaspfactory-2d.cc
 dune/grid/test/yasp/test-yaspgrid-yaspfactory-3d.cc
 dune/grid/test/yasp/test-yaspgrid.hh
 dune/grid/uggrid/CMakeLists.txt
 dune/grid/uggrid/boundaryextractor.cc
@@ -573,27 +503,21 @@
 dune/grid/utility/test/structuredgridfactorytest.cc
 dune/grid/utility/test/tensorgridfactorytest.cc
 dune/grid/utility/test/vertexordertest.cc
 dune/grid/yaspgrid/CMakeLists.txt
 dune/grid/yaspgrid/backuprestore.hh
 dune/grid/yaspgrid/coordinates.hh
 dune/grid/yaspgrid/grid.eps
-dune/grid/yaspgrid/grid.eps.license
 dune/grid/yaspgrid/grid.fig
-dune/grid/yaspgrid/grid.fig.license
 dune/grid/yaspgrid/grid.png
-dune/grid/yaspgrid/grid.png.license
 dune/grid/yaspgrid/partitioning.hh
 dune/grid/yaspgrid/structuredyaspgridfactory.hh
 dune/grid/yaspgrid/subgrid.eps
-dune/grid/yaspgrid/subgrid.eps.license
 dune/grid/yaspgrid/subgrid.fig
-dune/grid/yaspgrid/subgrid.fig.license
 dune/grid/yaspgrid/subgrid.png
-dune/grid/yaspgrid/subgrid.png.license
 dune/grid/yaspgrid/torus.hh
 dune/grid/yaspgrid/yaspgridentity.hh
 dune/grid/yaspgrid/yaspgridentityseed.hh
 dune/grid/yaspgrid/yaspgridgeometry.hh
 dune/grid/yaspgrid/yaspgridhierarchiciterator.hh
 dune/grid/yaspgrid/yaspgrididset.hh
 dune/grid/yaspgrid/yaspgridindexsets.hh
```

### Comparing `dune-grid-2.9.0rc1/src/gridinfo-gmsh/CMakeLists.txt` & `dune-grid-2.9.dev20220529/src/gridinfo-gmsh/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# SPDX-FileCopyrightText: Copyright (C) DUNE Project contributors, see file LICENSE.md in module root
-# SPDX-License-Identifier: LicenseRef-GPL-2.0-only-with-DUNE-exception
-
 if(ALBERTA_2D_LIB_FOUND AND ENABLE_GRID_EXTRA_UTILS)
   add_executable(dune-gridinfo-gmsh-alberta-2d gridinfo-gmsh-alberta-2d.cc)
   target_link_libraries(dune-gridinfo-gmsh-alberta-2d PRIVATE dunegrid)
   add_dune_alberta_flags(dune-gridinfo-gmsh-alberta-2d GRIDDIM 2)
   set(PROGRAMS ${PROGRAMS} dune-gridinfo-gmsh-alberta-2d)
 endif(ALBERTA_2D_LIB_FOUND AND ENABLE_GRID_EXTRA_UTILS)
```

