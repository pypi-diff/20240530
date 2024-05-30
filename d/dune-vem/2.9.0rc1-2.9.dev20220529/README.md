# Comparing `tmp/dune-vem-2.9.0rc1.tar.gz` & `tmp/dune-vem-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-vem-2.9.0rc1.tar", last modified: Fri Oct 21 08:17:07 2022, max compression
+gzip compressed data, was "dune-vem-2.9.dev20220529.tar", last modified: Sun May 29 21:03:44 2022, max compression
```

## Comparing `dune-vem-2.9.0rc1.tar` & `dune-vem-2.9.dev20220529.tar`

### file list

```diff
@@ -1,390 +1,356 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.035936 dune-vem-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.003936 dune-vem-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.007936 dune-vem-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/cmake/modules/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/cmake/modules/DuneVemMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.007936 dune-vem-2.9.0rc1/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.007936 dune-vem-2.9.0rc1/data/PolyMesher/
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/GenPolyMesh.m
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/HornDomain.m
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/MbbDomain.m
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/MichellDomain.m
--rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/PolyMesher.m
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/SuspensionDomain.m
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/UnitSqDomain.m
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/WrenchDomain.m
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/barycentreOfPolygon.m
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/dCircle.m
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/dDiff.m
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/dIntersect.m
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/dLine.m
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/dRectangle.m
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/dUnion.m
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.007936 dune-vem-2.9.0rc1/data/PolyMesher/meshes/
--rw-r--r--   0 runner    (1001) docker     (121)   802530 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/polymesher-mesh.msh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/
--rw-r--r--   0 runner    (1001) docker     (121)   391183 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-1024-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)    44931 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-128-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)     5173 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-16-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)   801474 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-2048-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)    91606 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-256-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)    10509 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-32-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-4-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)   190237 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-512-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)    21923 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-64-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-8-polygons.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/genPerturbedMesh.m
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/genmesh.m
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/data/gmsh/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/mymesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/unit_sq_4x4_npart=4.msh
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/unit_sq_8x8_npart=16.msh
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/unit_sq_8x8_npart=2.msh
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/unit_sq_8x8_npart=4.msh
--rw-r--r--   0 runner    (1001) docker     (121)    64077 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/gmsh/unitsq-tria-unstr_npart=16.msh
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/meshdata.mat
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/partitioned-mesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/rd.m
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/shpfun.m
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/test.msh
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/testmesh2.msh
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/unitcube-2d-unstr.geo
--rw-r--r--   0 runner    (1001) docker     (121)    15946 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/unitcube-2d-unstr.msh
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/data/unitcube-2d.dgf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/agglomeration/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/agglomeration.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19820 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/basisfunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6657 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/boundingbox.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/dgmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11262 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/dgspace.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10626 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/dofmapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/functor.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19038 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/agglomeration/shapefunctionset.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/function/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/function/simple.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/io/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/io/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13730 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/io/gmsh.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5844 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/io/gmsh.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/compatibility.hh
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/grid.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/leastSquares.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/matrixWrappers.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/pseudoinverse.hh
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/misc/vector.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/operator/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.011936 dune-vem-2.9.0rc1/dune/vem/operator/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/constraints/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16403 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/constraints/dirichlet.hh
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/constraints/noconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    31932 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/diffusionmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/mass.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12065 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/vemdirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19692 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/operator/vemelliptic.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.015936 dune-vem-2.9.0rc1/dune/vem/py/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/py/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/py/integrands.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.015936 dune-vem-2.9.0rc1/dune/vem/space/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20590 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/basisfunctionset.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23782 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/curlfree.hh
--rw-r--r--   0 runner    (1001) docker     (121)    42219 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/default.hh
--rw-r--r--   0 runner    (1001) docker     (121)    32441 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/divfree.hh
--rw-r--r--   0 runner    (1001) docker     (121)    29841 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/hk.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/indexset.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/interpolate.hh
--rw-r--r--   0 runner    (1001) docker     (121)    39333 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/interpolation.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/space/test.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.015936 dune-vem-2.9.0rc1/dune/vem/test/
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/biharmonic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/curlfree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/divfree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/elliptic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3826 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/hk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/hk_laplace.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/perturbation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/threadedgenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10457 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/uzawa.py
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/varyingcoeff.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/voronoiseeds368.pickle
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune/vem/test/voronoiseeds92.pickle
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune-vem.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/dune.module
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.015936 dune-vem-2.9.0rc1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/lib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.015936 dune-vem-2.9.0rc1/notMaintained/
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    45661 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/dune-vem.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.015936 dune-vem-2.9.0rc1/notMaintained/gmsh/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/mymesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_4x4_npart=4.msh
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_8x8_npart=16.msh
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_8x8_npart=2.msh
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_8x8_npart=4.msh
--rw-r--r--   0 runner    (1001) docker     (121)    64077 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/gmsh/unitsq-tria-unstr_npart=16.msh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.019936 dune-vem-2.9.0rc1/notMaintained/heat-test/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6541 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/agglo-heat.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.019936 dune-vem-2.9.0rc1/notMaintained/heat-test/data/
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/circle.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/parameter
--rw-r--r--   0 runner    (1001) docker     (121)    30075 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/sphere.dgf
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/spiral-2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/unitcube-1d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/data/unitcube-2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    15591 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6076 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/heat.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/heatmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/heatscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/l2model.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8743 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/model.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/modelinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/temporalprobleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17368 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/vemelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6609 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/heat-test/vemscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.019936 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.019936 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/fem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/partitioned-mesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/vem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/dataoutputparameters.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17754 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16632 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/fem-helmholtz.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6076 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8826 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/model.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/modelinterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13973 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/poisson.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3444 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vem-helmholtz.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15707 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vemdirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17491 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vemelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6331 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vemscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.019936 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.019936 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/fem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/unit-square-one-partition.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/vem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)    15089 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/fem-nonlinear.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/nonlinearmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5601 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vem-nonlinear.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15601 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vemdirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17375 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vemelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6057 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vemscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.023936 dune-vem-2.9.0rc1/notMaintained/poisson-test/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.023936 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/agglo-dg.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.023936 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/data/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/data/agglomeration-parameter
--rw-r--r--   0 runner    (1001) docker     (121)   748198 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/data/partitioned-mesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/dataoutputparameters.hh
--rw-r--r--   0 runner    (1001) docker     (121)    27778 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/dgelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/dgrhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7092 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6820 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/model.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.023936 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/anisotropic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproduct.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproductmixedbc.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/curvedridges.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/interface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/reentrantcorner.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/sinusproduct.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/sphereproblem.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8733 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/vemscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.023936 dune-vem-2.9.0rc1/notMaintained/poisson-test/data/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/data/mymesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/data/parameter
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/data/trivial.param
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/data/unitcube-2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    27730 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/dgelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7992 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/dgrhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/dune-poisson-agglo-DG.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7887 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/femscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.023936 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.027936 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/data/
--rw-r--r--   0 runner    (1001) docker     (121)   225340 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/data/mesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/data/parameter
--rw-r--r--   0 runner    (1001) docker     (121)    25754 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/dgelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6198 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/dgrhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/dune-dgpoisson.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/model.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/poisson.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/model.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/poisson.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/readme.info
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/travel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5897 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/trivial-agglomeration.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.027936 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.027936 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/data/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)   263718 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/data/mymesh.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/data/vem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)    19362 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/model.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11299 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/poisson.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3437 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vem-poisson-pmesh.cc
--rw-r--r--   0 runner    (1001) docker     (121)    17323 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vemdirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20970 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vemelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6559 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vemscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.027936 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.027936 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/fem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)    36823 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-quads.msh
--rw-r--r--   0 runner    (1001) docker     (121)    63840 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-trias.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-4x4-quads.msh
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-agg-trias-4x4.msh
--rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/unit-square-one-partition.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/vem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)    15089 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/fem-quasilinear-fp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12766 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/quasilinearmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6349 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vem-quasilinear-fp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    16404 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemdirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16287 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemdirichletconstraintsfromnewton.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25489 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemelliptic-fp.hh
--rw-r--r--   0 runner    (1001) docker     (121)    23280 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6420 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.027936 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/fem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)    36823 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-16x16-quads.msh
--rw-r--r--   0 runner    (1001) docker     (121)    63840 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-16x16-trias.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-4x4-quads.msh
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-agg-trias-4x4.msh
--rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/unit-square-one-partition.msh
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/vem-parameter
--rw-r--r--   0 runner    (1001) docker     (121)    15089 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/dirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/elliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/fem-quasilinear.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/femscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/probleminterface.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13227 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/quasilinearmodel.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/rhs.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6312 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vem-quasilinear.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15601 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vemdirichletconstraints.hh
--rw-r--r--   0 runner    (1001) docker     (121)    25186 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vemelliptic.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6415 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vemscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)    55575 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-Pk.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-dgspace.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10295 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-dmatrix.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-gmsh.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3676 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-indexset.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11134 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-leastsquares.cc
--rw-r--r--   0 runner    (1001) docker     (121)    41137 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-reactiondiffusion.cc
--rw-r--r--   0 runner    (1001) docker     (121)    44089 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/notMaintained/test-reactiondiffusion2.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/pydemo/
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/Hdivspace
--rw-r--r--   0 runner    (1001) docker     (121)     7784 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/biharmonic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/conditioning.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/conditioning.sh
--rw-r--r--   0 runner    (1001) docker     (121)     6898 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/cylinderSplit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/cylinderUzawa.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/divfree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/divfree2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/hktest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7333 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7726 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/pydemo/oldScript/
--rw-r--r--   0 runner    (1001) docker     (121)     7572 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/oldScript/demoA.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/oldScript/elasticity.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/oldScript/elliptic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/parameter
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/plotInterpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4783 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     6574 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/testelliptic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3843 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/testingscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     9130 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/uzawa.py
--rw-r--r--   0 runner    (1001) docker     (121)    13952 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/vemdemo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pydemo/wilmore.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/python/dune/vem/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/bbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/min_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/qhull_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/python/dune/vem/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/cylinderUzawa.py
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/laplace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/mixedSolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/uzawa.py
--rw-r--r--   0 runner    (1001) docker     (121)     8565 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/vemdemo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/tutorial/willmore.py
--rw-r--r--   0 runner    (1001) docker     (121)    38024 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/vem.py
--rw-r--r--   0 runner    (1001) docker     (121)     7533 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune/vem/voronoi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:07.031936 dune-vem-2.9.0rc1/python/dune_vem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune_vem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13450 2022-10-21 08:17:07.000000 dune-vem-2.9.0rc1/python/dune_vem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune_vem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune_vem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/python/dune_vem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:17:07.035936 dune-vem-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-21 08:17:06.000000 dune-vem-2.9.0rc1/stamp-vc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.615774 dune-vem-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.615774 dune-vem-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/cmake/modules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/cmake/modules/DuneVemMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.615774 dune-vem-2.9.dev20220529/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.619774 dune-vem-2.9.dev20220529/data/PolyMesher/
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/GenPolyMesh.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/HornDomain.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/MbbDomain.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/MichellDomain.m
+-rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/PolyMesher.m
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/SuspensionDomain.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/UnitSqDomain.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/WrenchDomain.m
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/barycentreOfPolygon.m
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/dCircle.m
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/dDiff.m
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/dIntersect.m
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/dLine.m
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/dRectangle.m
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/dUnion.m
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.619774 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/
+-rw-r--r--   0 runner    (1001) docker     (121)   802530 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/polymesher-mesh.msh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/
+-rw-r--r--   0 runner    (1001) docker     (121)   391183 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-1024-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    44931 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-128-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     5173 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-16-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)   801474 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-2048-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    91606 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-256-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    10509 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-32-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-4-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)   190237 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-512-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    21923 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-64-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-8-polygons.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/genPerturbedMesh.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/genmesh.m
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/data/gmsh/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/mymesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/unit_sq_4x4_npart=4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/unit_sq_8x8_npart=16.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/unit_sq_8x8_npart=2.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/unit_sq_8x8_npart=4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    64077 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/gmsh/unitsq-tria-unstr_npart=16.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/meshdata.mat
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/partitioned-mesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/rd.m
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/shpfun.m
+-rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/test.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/testmesh2.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/unitcube-2d-unstr.geo
+-rw-r--r--   0 runner    (1001) docker     (121)    15946 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/unitcube-2d-unstr.msh
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/data/unitcube-2d.dgf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/agglomeration/
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/agglomeration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19744 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/basisfunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6657 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/boundingbox.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/dgmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11262 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/dgspace.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11542 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/dofmapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/functor.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17761 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/agglomeration/shapefunctionset.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/function/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/function/simple.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/io/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13730 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/io/gmsh.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5844 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/io/gmsh.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/compatibility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/grid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/leastSquares.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/matrixWrappers.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/pseudoinverse.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/misc/vector.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/operator/
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/operator/constraints/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/constraints/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16403 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/constraints/dirichlet.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/constraints/noconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    31892 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/diffusionmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4485 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/mass.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11023 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/vemdirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19680 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/operator/vemelliptic.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.623774 dune-vem-2.9.dev20220529/dune/vem/py/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/py/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/py/integrands.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.627774 dune-vem-2.9.dev20220529/dune/vem/space/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14968 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/basisfunctionset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    33657 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/default.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    41915 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/hk.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/indexset.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/interpolate.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune/vem/space/test.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune-vem.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/dune.module
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.627774 dune-vem-2.9.dev20220529/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/lib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.627774 dune-vem-2.9.dev20220529/notMaintained/
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    45661 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/dune-vem.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.627774 dune-vem-2.9.dev20220529/notMaintained/gmsh/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/mymesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_4x4_npart=4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_8x8_npart=16.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_8x8_npart=2.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_8x8_npart=4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    64077 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/gmsh/unitsq-tria-unstr_npart=16.msh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.627774 dune-vem-2.9.dev20220529/notMaintained/heat-test/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6541 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/agglo-heat.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.627774 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/circle.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    30075 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/sphere.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/spiral-2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/unitcube-1d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/data/unitcube-2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    15591 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6076 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/heat.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/heatmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/heatscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/l2model.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8743 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/model.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/modelinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/temporalprobleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17368 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/vemelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6609 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/heat-test/vemscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.631774 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.631774 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/fem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/partitioned-mesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/vem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/dataoutputparameters.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17754 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16632 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/fem-helmholtz.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     6076 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8826 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/model.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/modelinterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13973 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/poisson.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3444 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vem-helmholtz.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15707 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vemdirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17491 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vemelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6331 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vemscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.631774 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.631774 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/fem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/unit-square-one-partition.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/vem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    15089 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/fem-nonlinear.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/nonlinearmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5601 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vem-nonlinear.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15601 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vemdirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17375 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vemelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6057 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vemscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.631774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/agglo-dg.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/data/agglomeration-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)   748198 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/data/partitioned-mesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/dataoutputparameters.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    27778 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/dgelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/dgrhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7092 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6820 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/model.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/anisotropic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproduct.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproductmixedbc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/curvedridges.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/interface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/reentrantcorner.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/sinusproduct.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/sphereproblem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8733 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/vemscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/mymesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/trivial.param
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/unitcube-2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    27730 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/dgelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7992 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/dgrhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/dune-poisson-agglo-DG.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7887 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/femscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   225340 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/data/mesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/data/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    25754 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/dgelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6198 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/dgrhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/dune-dgpoisson.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/model.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/poisson.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4431 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7299 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/model.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/poisson.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4431 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/readme.info
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/travel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5897 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/trivial-agglomeration.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.635774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.639774 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   263718 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/data/mymesh.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/data/vem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    19362 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/model.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11299 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/poisson.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3437 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vem-poisson-pmesh.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    17323 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vemdirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20970 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vemelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6559 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vemscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.639774 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.639774 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/fem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    36823 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-quads.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    63840 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-trias.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-4x4-quads.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-agg-trias-4x4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/unit-square-one-partition.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/vem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    15089 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/fem-quasilinear-fp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12766 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/quasilinearmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6349 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vem-quasilinear-fp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    16404 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemdirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16287 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemdirichletconstraintsfromnewton.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25489 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemelliptic-fp.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    23280 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6420 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.639774 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.639774 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/fem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    36823 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-16x16-quads.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    63840 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-16x16-trias.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-4x4-quads.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-agg-trias-4x4.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/unit-square-one-partition.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/vem-parameter
+-rw-r--r--   0 runner    (1001) docker     (121)    15089 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/dirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/elliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/fem-quasilinear.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5465 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/femscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/probleminterface.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13227 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/quasilinearmodel.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/rhs.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6312 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vem-quasilinear.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15601 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vemdirichletconstraints.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    25186 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vemelliptic.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6415 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vemscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    55575 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-Pk.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-dgspace.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10295 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-dmatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-gmsh.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3676 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-indexset.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    11134 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-leastsquares.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    41137 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-reactiondiffusion.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    44089 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/notMaintained/test-reactiondiffusion2.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/pydemo/
+-rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/biharmonic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/conditioning.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     7333 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/pydemo/oldScript/
+-rw-r--r--   0 runner    (1001) docker     (121)     7572 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/oldScript/demoA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/oldScript/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/oldScript/elliptic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/parameter
+-rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/plotInterpolation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6574 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/testelliptic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/uzawa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8565 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/vemdemo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12978 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/vemtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pydemo/wilmore.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/python/dune/vem/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/min_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/qhull_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/python/dune/vem/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8565 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/tutorial/vemdemo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28684 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/vem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6591 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune/vem/voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/python/dune_vem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune_vem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12537 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune_vem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune_vem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune_vem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/python/dune_vem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:44.643774 dune-vem-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-29 21:03:44.000000 dune-vem-2.9.dev20220529/stamp-vc
```

### Comparing `dune-vem-2.9.0rc1/CMakeLists.txt` & `dune-vem-2.9.dev20220529/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 dune_project()
 dune_enable_all_packages()
 
 include(AddMPIFlags)
 
 add_subdirectory("dune")
 add_subdirectory("cmake/modules")
+# add_subdirectory("lib")
 add_subdirectory(python)
 
 # finalize the dune project, e.g. generating config.h etc.
 finalize_dune_project(GENERATE_CONFIG_H_CMAKE)
```

### Comparing `dune-vem-2.9.0rc1/PKG-INFO` & `dune-vem-2.9.dev20220529/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-vem
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Implementation of a number of virtual element spaces and bilinear forms
 Home-page: https://gitlab.dune-project.org/dune-fem/dune-vem
 Author: Andreas Dedner
 Author-email: a.s.dedner@warwick.ac.uk
 License: UNKNOWN
 Description: Preparing the Sources
         =========================
@@ -59,15 +59,15 @@
         
         for further options.
         
         
         The full build-system is described in the dune-common/doc/buildsystem (Git version) or under share/doc/dune-common/buildsystem if you installed DUNE!
         
         
-        git-ebed1814cbfb128fa8b3fd6ae1061263d3eb653e
+        git-b8e7da0a28e5a215676202b5b80fda0bd32a9191
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-vem-2.9.0rc1/README.md` & `dune-vem-2.9.dev20220529/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 
 for further options.
 
 
 The full build-system is described in the dune-common/doc/buildsystem (Git version) or under share/doc/dune-common/buildsystem if you installed DUNE!
 
 
-git-ebed1814cbfb128fa8b3fd6ae1061263d3eb653e
+git-b8e7da0a28e5a215676202b5b80fda0bd32a9191
```

### Comparing `dune-vem-2.9.0rc1/config.h.cmake` & `dune-vem-2.9.dev20220529/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/GenPolyMesh.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/GenPolyMesh.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/HornDomain.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/HornDomain.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/MbbDomain.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/MbbDomain.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/MichellDomain.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/MichellDomain.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/PolyMesher.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/PolyMesher.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/SuspensionDomain.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/SuspensionDomain.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/UnitSqDomain.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/UnitSqDomain.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/WrenchDomain.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/WrenchDomain.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/barycentreOfPolygon.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/barycentreOfPolygon.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/dCircle.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/dCircle.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/dDiff.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/dDiff.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/dIntersect.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/dIntersect.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/dLine.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/dLine.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/dRectangle.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/dRectangle.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/dUnion.m` & `dune-vem-2.9.dev20220529/data/PolyMesher/dUnion.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/polymesher-mesh.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/polymesher-mesh.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-1024-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-1024-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-128-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-128-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-16-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-16-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-2048-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-2048-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-256-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-256-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-32-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-32-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-4-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-4-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-512-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-512-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-64-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-64-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/PolyMesher/meshes/test-meshes/mesh-8-polygons.msh` & `dune-vem-2.9.dev20220529/data/PolyMesher/meshes/test-meshes/mesh-8-polygons.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/genPerturbedMesh.m` & `dune-vem-2.9.dev20220529/data/genPerturbedMesh.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/genmesh.m` & `dune-vem-2.9.dev20220529/data/genmesh.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/gmsh/unit_sq_4x4_npart=4.msh` & `dune-vem-2.9.dev20220529/data/gmsh/unit_sq_4x4_npart=4.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/gmsh/unit_sq_8x8_npart=16.msh` & `dune-vem-2.9.dev20220529/data/gmsh/unit_sq_8x8_npart=16.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/gmsh/unit_sq_8x8_npart=2.msh` & `dune-vem-2.9.dev20220529/data/gmsh/unit_sq_8x8_npart=2.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/gmsh/unit_sq_8x8_npart=4.msh` & `dune-vem-2.9.dev20220529/data/gmsh/unit_sq_8x8_npart=4.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/gmsh/unitsq-tria-unstr_npart=16.msh` & `dune-vem-2.9.dev20220529/data/gmsh/unitsq-tria-unstr_npart=16.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/rd.m` & `dune-vem-2.9.dev20220529/data/rd.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/shpfun.m` & `dune-vem-2.9.dev20220529/data/shpfun.m`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/test.msh` & `dune-vem-2.9.dev20220529/data/test.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/testmesh2.msh` & `dune-vem-2.9.dev20220529/data/testmesh2.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/data/unitcube-2d-unstr.msh` & `dune-vem-2.9.dev20220529/data/unitcube-2d-unstr.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/agglomeration.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/agglomeration.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/basisfunctionset.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/basisfunctionset.hh`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
       typedef typename FunctionSpaceType::DomainType DomainType;
       typedef typename FunctionSpaceType::RangeType RangeType;
       typedef typename FunctionSpaceType::JacobianRangeType JacobianRangeType;
       typedef typename FunctionSpaceType::HessianRangeType HessianRangeType;
 
       static constexpr int dimDomain = DomainType::dimension;
-      static_assert(RangeType::dimension==1);
 
       typedef typename ReferenceElements< typename DomainType::field_type, dimDomain >::ReferenceElement ReferenceElementType;
 
     private:
       struct Transformation
       {
         Transformation() {}
@@ -312,20 +311,20 @@
       void hessianEach ( const Point &x, Functor functor ) const
       {
         sfEvaluateAll(x,hess_);
         for (std::size_t beta=0;beta<size();++beta)
           functor(beta,transformation_( hess_[beta] ));
       }
 
+    private:
       template< class Point >
       DomainType position ( const Point &x ) const
       {
         return bbox().transform( entity().geometry().global( Fem::coordinate( x ) ) );
       }
-    private:
       // make basis orthogonal
       // k = 0
       // for i < N
       //   for j < i; ++k
       //     b_i -= r_k b_j {Remove the projection of b_i onto b_j
       //   b_i /= r_k
       template <class Vector>
@@ -367,15 +366,14 @@
       {
         assert(values.size()==size());
         Fem::AssignFunctor< decltype(values) > f( values );
         auto y = position(x);
         for (std::size_t beta=0;beta<size();++beta)
           shapeFunctionSet_.hessianEach( y, f);
         // onb( values ); // Note: failing axpy on FV<FM> due to missing // double*FM
-        if (!useOnb_) return;
         std::size_t k = 0;
         for (std::size_t i=0;i<values.size();++i,++k)
         {
           for (std::size_t j=0;j<i;++j,++k)
             for (std::size_t r=0;r<values[i].size();++r)
               values[i][r].axpy(-bbox().r(k), values[j][r]);
           values[i] /= bbox().r(k);
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/boundingbox.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/boundingbox.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/dgmapper.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/dgmapper.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/dgspace.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/dgspace.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/dofmapper.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/dofmapper.hh`

 * *Files 5% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 
     protected:
       const IndexSetType &indexSet_;
       unsigned int maxNumDofs_ = 0;
       SizeType size_;
       std::vector< SubEntityInfo > subEntityInfo_;
       std::array< int, dimension+1 > codimIndex_;
+      std::vector< bool > edgeTwist_;
     };
 
 
 
     // Implementation of AgglomerationDofMapper
     // ----------------------------------------
 
@@ -224,16 +225,15 @@
       {
         const std::size_t numSubAgglomerates = indexSet().subAgglomerates( element, info.codim );
         for( std::size_t subAgglomerate = 0; subAgglomerate < numSubAgglomerates; ++subAgglomerate )
         {
           const SizeType subIndex = indexSet().subIndex( element, subAgglomerate, info.codim );
           SizeType index = info.offset + SizeType( info.numDofs ) * subIndex;
 
-          if( false )
-          // if ( (info.codim == 1) && (indexSet().twist(subIndex) == 1) )
+          if( (info.codim == 1) && (edgeTwist_[ subIndex ] == 1) )
           {
             const SizeType begin = index;
             for( index += info.numDofs; index > begin; )
               f( local++, --index );
           }
           else
           {
@@ -255,16 +255,15 @@
         return;
 
       const auto result = indexSet().globalIndex( entity );
       if( !result.second )
         return;
 
       SizeType index = info.offset + SizeType( info.numDofs ) * result.first;
-      if( false )
-      // if ( (Entity::codimension == 1) && (indexSet().twist(result.first)) )
+      if( (Entity::codimension == 1) && (edgeTwist_[ result.first ]) )
       {
         for( unsigned int i = info.numDofs; i > 0; )
           f( --i, index++ );
       }
       else
       {
         for( unsigned int i = 0; i < info.numDofs; )
@@ -281,14 +280,32 @@
       for( SubEntityInfo &info : subEntityInfo_ )
       {
         info.offset = size_;
         size_ += SizeType( info.numDofs ) * SizeType( indexSet().size( info.codim ) );
         maxNumDofs_ += SizeType( info.numDofs ) * SizeType( indexSet().maxSubAgglomerates( info.codim ) );
       }
 
+      if( dimension > 1 )
+      {
+        const auto &idSet = agglomeration().gridPart().grid().globalIdSet();
+
+        edgeTwist_.resize( indexSet().size( dimension-1 ) );
+        for( const auto element : elements( agglomeration().gridPart(), Partitions::interiorBorder ) )
+        {
+          const auto &refElement = ReferenceElements< typename GridPart::ctype, dimension >::general( element.type() );
+
+          const int numEdges = refElement.size( dimension-1 );
+          for( int i = 0; i < numEdges; ++i )
+          {
+            const auto left = idSet.subId( Dune::Fem::gridEntity(element), refElement.subEntity( i, dimension-1, 0, dimension ), dimension );
+            const auto right = idSet.subId( Dune::Fem::gridEntity(element), refElement.subEntity( i, dimension-1, 1, dimension ), dimension );
+            edgeTwist_[ indexSet().subIndex( element, i, dimension-1 ) ] = (right < left);
+          }
+        }
+      }
     }
 
   } // namespace Fem
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_VEM_AGGLOMERATION_DOFMAPPER_HH
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/functor.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/functor.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/indexset.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/indexset.hh`

 * *Files 3% similar despite different names*

```diff
@@ -156,15 +156,15 @@
       double elementDiameter( const ElementType &element ) const
       {
         return elementDiameter( index( element ) );
       }
       double vertexDiameter( std::size_t index ) const { return vertexDiameters_[index]; }
       double vertexDiameter( const ElementType &element, std::size_t index ) const
       {
-        return vertexDiameter( globalIndex(element,index,dimension).first );
+        return vertexDiameter( localIndex(element,index,dimension) );
       }
       std::pair<double,double> diameters() const { return {minDiameter_,maxDiameter_}; }
       const BoundingBox<GridPart>& boundingBox( std::size_t index ) const
       {
         return agglomeration().boundingBox(index);
       }
       const BoundingBox<GridPart>& boundingBox( const ElementType &element ) const
@@ -175,23 +175,14 @@
       {
         return agglomeration().boundingBoxes();
       }
       Std::vector< BoundingBox< GridPart > >& boundingBoxes()
       {
         return const_cast<AgglomerationType&>(agglomeration()).boundingBoxes();
       }
-      bool twist( std::size_t i ) const
-      {
-        return edgeTwist_[ i ];
-      }
-      bool twist( const typename GridPart::IntersectionType &intersection ) const
-      {
-        return edgeTwist_[ subIndex( intersection.inside(), intersection.indexInInside(), dimension-1 ) ];
-      }
-
 
       void update();
     private:
       const Agglomerate &agglomerate ( std::size_t agglomerateIndex ) const { return agglomerates_[ agglomerateIndex ]; }
       const Agglomerate &agglomerate ( const ElementType &element ) const { return agglomerate( index( element ) ); }
 
       AgglomerationType &agglomeration_;
@@ -199,15 +190,14 @@
       Std::vector< Agglomerate > agglomerates_;
       std::array< std::size_t, dimension+1 > size_;
       std::array< std::size_t, dimension+1 > maxSubAgglomerates_;
       std::vector< std::vector< int > > globalIndex_;
       Std::vector< double > vertexDiameters_;
       double minDiameter_, maxDiameter_;
       std::size_t counter_;
-      std::vector< bool > edgeTwist_;
     };
 
 
 
     // AgglomerationIndexSet::Agglomerate
     // ----------------------------------
 
@@ -452,33 +442,13 @@
         }
       }
       for ( std::size_t k = 0; k < vertexCount.size(); ++k)
         vertexDiameters_[k] /= double(vertexCount[k]);
 
       maxDiameter_ = *std::max_element(vertexDiameters_.begin(),vertexDiameters_.end());
       minDiameter_ = *std::min_element(vertexDiameters_.begin(),vertexDiameters_.end());
-
-      // store edge twists
-      if( dimension > 1 )
-      {
-        const auto &idSet = agglomeration_.gridPart().grid().globalIdSet();
-
-        edgeTwist_.resize( size( dimension-1 ) );
-        for( const auto element : elements( agglomeration_.gridPart(), Partitions::interiorBorder ) )
-        {
-          const auto &refElement = ReferenceElements< typename GridPart::ctype, dimension >::general( element.type() );
-
-          const int numEdges = refElement.size( dimension-1 );
-          for( int i = 0; i < numEdges; ++i )
-          {
-            const auto left = idSet.subId( Dune::Fem::gridEntity(element), refElement.subEntity( i, dimension-1, 0, dimension ), dimension );
-            const auto right = idSet.subId( Dune::Fem::gridEntity(element), refElement.subEntity( i, dimension-1, 1, dimension ), dimension );
-            edgeTwist_[ subIndex( element, i, dimension-1 ) ] = (right < left);
-          }
-        }
-      }
     }
   } // namespace Vem
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_VEM_AGGLOMERATION_INDEXSET_HH
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/agglomeration/shapefunctionset.hh` & `dune-vem-2.9.dev20220529/dune/vem/agglomeration/shapefunctionset.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/function/simple.hh` & `dune-vem-2.9.dev20220529/dune/vem/function/simple.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/io/gmsh.cc` & `dune-vem-2.9.dev20220529/dune/vem/io/gmsh.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/io/gmsh.hh` & `dune-vem-2.9.dev20220529/dune/vem/io/gmsh.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/misc/leastSquares.hh` & `dune-vem-2.9.dev20220529/dune/vem/misc/leastSquares.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/misc/matrixWrappers.hh` & `dune-vem-2.9.dev20220529/dune/vem/misc/matrixWrappers.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/misc/pseudoinverse.hh` & `dune-vem-2.9.dev20220529/dune/vem/misc/pseudoinverse.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/misc/vector.hh` & `dune-vem-2.9.dev20220529/dune/vem/misc/vector.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/operator/constraints/dirichlet.hh` & `dune-vem-2.9.dev20220529/dune/vem/operator/constraints/dirichlet.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/operator/constraints/noconstraints.hh` & `dune-vem-2.9.dev20220529/dune/vem/operator/constraints/noconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/operator/diffusionmodel.hh` & `dune-vem-2.9.dev20220529/dune/vem/operator/diffusionmodel.hh`

 * *Files 0% similar despite different names*

```diff
@@ -351,18 +351,18 @@
       using DRangeType = typename detail::GetDimRange<std::tuple_element_t<0,DomainValueType>>::type;
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
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/operator/mass.hh` & `dune-vem-2.9.dev20220529/dune/vem/operator/mass.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/operator/vemdirichletconstraints.hh` & `dune-vem-2.9.dev20220529/dune/vem/operator/vemdirichletconstraints.hh`

 * *Files 6% similar despite different names*

```diff
@@ -73,60 +73,32 @@
         case 1: return (maskValue == 1);
         case 2: return (maskValue == 2);
         case 3: return (maskValue >= 1);
       }
       return false; // can't be reached
     }
 
+#if 0
     template < class DiscreteFunctionType >
     void operator ()( const DiscreteFunctionType& u, DiscreteFunctionType& w ) const
     {
       BaseType::operator()(u,w);
     }
-#if 0
     template < class DiscreteFunctionType >
     void operator ()( const typename DiscreteFunctionType::RangeType& value, DiscreteFunctionType& w ) const
     {
       BaseType::operator()(value,w);
     }
 #endif
 
     template < class DiscreteFunctionType >
     void operator ()( const typename DiscreteFunctionType::RangeType& value, DiscreteFunctionType& w ) const
     {
-
-      BaseType::updateDirichletDofs();
-      if( BaseType::hasDirichletDofs_ )
-        for( const EntityType &entity : space_ )
-        {
-          auto wLocal = w.localFunction( entity );
-          // get number of Lagrange Points
-          const int localBlocks = space_.blockMapper().numDofs( entity );
-
-          // map local to global BlockDofs
-          std::vector< std::size_t > globalBlockDofs( localBlocks );
-          space_.blockMapper().map( entity, globalBlockDofs );
-          std::vector< double > valuesModel( localBlocks*localBlockSize );
-          Vem::Std::vector< char > mask( localBlocks );
-          space_.interpolation()( entity, mask );
-
-          int localDof = 0;
-          for( int localBlock = 0; localBlock < localBlocks; ++localBlock )
-          {
-            // store result to dof vector
-            int global = globalBlockDofs[ localBlock ];
-            for( int l = 0; l < localBlockSize; ++l, ++localDof )
-            {
-              if( dirichletBlocks_[ global ][ l ] && applyConstraint(mask[ localBlock ]))
-                wLocal[ localDof ] = 0;
-            }
-          }
-        }
+      this->operator()(w);
     }
-
     template < class DiscreteFunctionType >
     void operator ()( DiscreteFunctionType& w ) const
     {
       BaseType::updateDirichletDofs();
       if( BaseType::hasDirichletDofs_ )
       {
         Dune::Fem::MutableLocalFunction< DiscreteFunctionType > wLocal( w );
@@ -137,14 +109,17 @@
         }
       }
     }
     template < class DiscreteFunctionType >
     void operator ()( const DiscreteFunctionType &u,
                       DiscreteFunctionType& w, Operation op) const
     {
+      // if (op == Operation::set)
+      //   this->operator()(u,w);
+
       BaseType::updateDirichletDofs();
       if( BaseType::hasDirichletDofs_ )
       {
         Dune::Fem::ConstLocalFunction< DiscreteFunctionType > uLocal( u );
         Dune::Fem::MutableLocalFunction< DiscreteFunctionType > wLocal( w );
         for( const auto &entity : space_ )
         {
@@ -191,14 +166,15 @@
 
       // map local to global dofs
       std::vector<std::size_t> globalBlockDofs(localBlocks);
       // obtain all DofBlocks for this element
       space_.blockMapper().map( entity, globalBlockDofs );
       Vem::Std::vector< char > mask( localBlocks );
       space_.interpolation()( entity, mask );
+
       // counter for all local dofs (i.e. localBlockDof * localBlockSize + ... )
       int localDof = 0;
       // iterate over face dofs and set unit row
       for( int localBlockDof = 0 ; localBlockDof < localBlocks; ++ localBlockDof )
       {
         int global = globalBlockDofs[localBlockDof];
         for( int l = 0; l < localBlockSize; ++ l, ++ localDof )
@@ -231,30 +207,30 @@
       std::vector< std::size_t > globalBlockDofs( localBlocks );
       space_.blockMapper().map( entity, globalBlockDofs );
       std::vector< double > valuesModel( localBlocks*localBlockSize );
       Vem::Std::vector< char > mask( localBlocks );
       space_.interpolation()( entity, mask );
 
       int localDof = 0;
+
       for( int localBlock = 0; localBlock < localBlocks; ++localBlock )
       {
         // store result to dof vector
         int global = globalBlockDofs[ localBlock ];
         for( int l = 0; l < localBlockSize; ++l, ++localDof )
-        {
           if( dirichletBlocks_[ global ][ l ] &&
               applyConstraint(mask[ localBlock ]))
           {
             std::fill(valuesModel.begin(),valuesModel.end(),0);
-            space_.interpolation()( entity, BoundaryWrapper(model_,dirichletBlocks_[global][l]),  valuesModel );
+            space_.interpolation()( entity, BoundaryWrapper(model_,dirichletBlocks_[global][l]),
+                valuesModel );
             // store result
             assert( (unsigned int)localDof < wLocal.size() );
             wLocal[ localDof ] = valuesModel[ localDof ];
           }
-        }
       }
     }
     template< class LocalFunctionType, class LocalContributionType >
     void dirichletDofTreatment( const LocalFunctionType &uLocal,
                                 LocalContributionType &wLocal, Operation op ) const
     {
       // get entity
@@ -269,15 +245,14 @@
       std::vector< std::size_t > globalBlockDofs( localBlocks );
       space_.blockMapper().map( entity, globalBlockDofs );
 
       std::vector<double> values( localBlocks*localBlockSize );
       std::vector<double> valuesModel( localBlocks*localBlockSize );
       Vem::Std::vector< char > mask( localBlocks );
       assert( uLocal.size() == values.size() );
-      assert( wLocal.size() == values.size() );
       for (unsigned int i=0;i<uLocal.size();++i)
         values[i] = uLocal[i];
       space_.interpolation()( entity, mask );
 
       int localDof = 0;
 
       for( int localBlock = 0; localBlock < localBlocks; ++localBlock )
@@ -288,15 +263,17 @@
         {
           if( dirichletBlocks_[ global ][l] &&
               applyConstraint(mask[ localBlock ]) )
           {
             if (op == Operation::sub)
             {
               std::fill(valuesModel.begin(),valuesModel.end(),0);
-              space_.interpolation() ( entity, BoundaryWrapper(model_,dirichletBlocks_[global][l]), valuesModel );
+              space_.interpolation()
+                 ( entity, BoundaryWrapper(model_,dirichletBlocks_[global][l]),
+                     valuesModel );
               values[ localDof ] -= valuesModel[ localDof ];
             }
             assert( (unsigned int)localDof < wLocal.size() );
             wLocal[ localDof ] = values[ localDof ];
           }
         }
       }
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/operator/vemelliptic.hh` & `dune-vem-2.9.dev20220529/dune/vem/operator/vemelliptic.hh`

 * *Files 0% similar despite different names*

```diff
@@ -225,16 +225,16 @@
         // local vertex number in the triangle/quad, this is not the local vertex number of the polygon!
         const int j = refElement.subEntity(faceIndex, 1, i, GridPartType::dimension);
         // global coordinate of the vertex
         DomainType globalPoint = geometry.corner(j);
         // local coordinate of the vertex
         DomainType localPoint = geometry.local(globalPoint);
 
-        DomainRangeType vu(0);
-        // uLocal.evaluate(localPoint, vu);
+        DomainRangeType vu;
+        uLocal.evaluate(localPoint, vu);
 
         double bbH2 = pow(bbox.volume()/bbox.diameter(),2);
         // std::cout << "vemelliptic:" << pow(bbox.diameter(),2) << " " << bbox.volume() << std::endl;
         RangeRangeType Dcoeff = model().gradStabilization(localPoint,vu);
         Dcoeff.axpy(bbH2, model().massStabilization(localPoint,vu) );
         Dcoeff.axpy(1./bbH2, model().hessStabilization(localPoint,vu) );
 
@@ -344,16 +344,16 @@
       for (int i = 0; i < numEdgeVertices; ++i)
       {
         const int j = refElement.subEntity(faceIndex, 1, i, GridPartType::dimension);
         // global coordinate of the vertex
         DomainType globalPoint = geometry.corner(j);
         // local coordinate of the vertex
         DomainType localPoint = geometry.local(globalPoint);
-        DomainRangeType vu(0);
-        // uLocal.evaluate(localPoint, vu);
+        DomainRangeType vu;
+        uLocal.evaluate(localPoint, vu);
 
         double bbH2 = pow(bbox.volume()/bbox.diameter(),2);
         // std::cout << "vemelliptic:" << pow(bbox.diameter(),2) << " " << bbox.volume() << std::endl;
         RangeRangeType Dcoeff = model().gradStabilization(localPoint,vu);
         Dcoeff.axpy(bbH2, model().massStabilization(localPoint,vu) );
         Dcoeff.axpy(1./bbH2, model().hessStabilization(localPoint,vu) );
         RangeRangeType LinDcoeff = model().linGradStabilization(localPoint,vu);
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/py/integrands.hh` & `dune-vem-2.9.dev20220529/dune/vem/py/integrands.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/space/basisfunctionset.hh` & `dune-vem-2.9.dev20220529/dune/vem/space/basisfunctionset.hh`

 * *Files 22% similar despite different names*

```diff
@@ -24,18 +24,18 @@
   namespace Vem
   {
 
     // VEMBasisFunctionSet
     // -------------------
 
     // TODO: add template arguments for ValueProjection and JacobianProjection
-    template< class Entity, class ShapeFunctionSet, class InterpolationType >
+    template< class Entity, class ShapeFunctionSet >
     class VEMBasisFunctionSet
     {
-      typedef VEMBasisFunctionSet< Entity, ShapeFunctionSet, InterpolationType > ThisType;
+      typedef VEMBasisFunctionSet< Entity, ShapeFunctionSet > ThisType;
 
     public:
       typedef Entity EntityType;
 
       typedef typename ShapeFunctionSet::FunctionSpaceType FunctionSpaceType;
 
       typedef typename FunctionSpaceType::DomainFieldType DomainFieldType;
@@ -54,34 +54,31 @@
 
       typedef FieldMatrix < DomainFieldType, dimDomain, dimDomain > HessianMatrixType;
 
       const auto& valueProjection() const { return (*valueProjections_)[agglomerate_]; }
       const auto& jacobianProjection() const { return (*jacobianProjections_)[agglomerate_]; }
       const auto& hessianProjection() const { return (*hessianProjections_)[agglomerate_]; }
       typedef Std::vector< Std::vector< DomainFieldType > > ValueProjection;
-      typedef Std::vector< Std::vector< DomainFieldType > > JacobianProjection;
-      typedef Std::vector< Std::vector< DomainFieldType > > HessianProjection;
+      typedef Std::vector< Std::vector< DomainType > > JacobianProjection;
+      typedef Std::vector< Std::vector< HessianMatrixType > > HessianProjection;
       template <class T>
       using Vector = Std::vector<T>;
 
       VEMBasisFunctionSet () = default;
 
       VEMBasisFunctionSet ( const EntityType &entity,
                             int agglomerate,
                             std::shared_ptr<Vector<ValueProjection>> valueProjections,
                             std::shared_ptr<Vector<JacobianProjection>> jacobianProjections,
                             std::shared_ptr<Vector<HessianProjection>> hessianProjections,
-                            ShapeFunctionSet shapeFunctionSet,
-                            std::shared_ptr<InterpolationType> interpolation
-                          )
+                            ShapeFunctionSet shapeFunctionSet = ShapeFunctionSet() )
         : entity_( &entity ), //polygon
           agglomerate_(agglomerate),
           shapeFunctionSet_( std::move( shapeFunctionSet ) ),
-          interpolation_(interpolation),
-          valueProjections_( valueProjections ),
+          valueProjections_( valueProjections),
           jacobianProjections_( jacobianProjections ),
           hessianProjections_( hessianProjections ),
           size_( valueProjection()[0].size() )
       {}
 
       int order () const { return shapeFunctionSet_.order(); }
 
@@ -96,290 +93,124 @@
       void evaluateAll ( const Quadrature &quadrature, const DofVector &dofs, Values &values ) const
       {
         const std::size_t nop = quadrature.nop();
         for( std::size_t qp = 0; qp < nop; ++qp )
           evaluateAll( quadrature[ qp ], dofs, values[ qp ] );
       }
 
-      template< class F, int d, class DofVector >
-      void evaluateAll ( const Dune::FieldVector<F,d> &x, const DofVector &dofs, RangeType &value ) const
+      template< class Point, class DofVector >
+      void evaluateAll ( const Point &x, const DofVector &dofs, RangeType &value ) const
       {
-        // needed for plotting for example: assert(0);
         value = RangeType( 0 );
-        shapeFunctionSet_.evaluateEach( x, [ this, &dofs, &value ] ( std::size_t alpha, RangeType phi_alpha ) {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &dofs, &value ] ( std::size_t alpha, RangeType phi_alpha ) {
             for( std::size_t j = 0; j < size(); ++j )
               value.axpy( valueProjection()[ alpha ][ j ]*dofs[ j ], phi_alpha );
           } );
       }
-      template< class Point, class DofVector >
-      void evaluateAll ( const Point &x, const DofVector &dofs, RangeType &value ) const
-      {
-        value = RangeType( 0 );
-        if constexpr ( Point::QuadratureType::codimension == 1)
-        {
-          Std::vector < Dune::DynamicMatrix<double> > localDofVectorMatrix(2);
-          Std::vector<Std::vector<unsigned int>> mask(2,Std::vector<unsigned int>(0));
-          auto locx = x.localPosition();
-          auto normal = x.quadrature().intersection().unitOuterNormal(locx);
-          auto edgeSF = (*interpolation_)(x.quadrature().intersection(), localDofVectorMatrix, mask);
-          edgeSF.evaluateEach(locx, [&](std::size_t beta, RangeType psi)
-          {
-            if (beta < localDofVectorMatrix[0].size())
-              for (std::size_t s=0; s<mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-              {
-                std::size_t j = mask[0][s];
-                value.axpy( localDofVectorMatrix[0][beta][s] * dofs[ j ], psi );
-              }
-          });
-        }
-        else
-        {
-          shapeFunctionSet_.evaluateEach( x, [ this, &dofs, &value ] ( std::size_t alpha, RangeType phi_alpha ) {
-              for( std::size_t j = 0; j < size(); ++j )
-                value.axpy( valueProjection()[ alpha ][ j ]*dofs[ j ], phi_alpha );
-            } );
-        }
-      }
 
-      template< class F, int d, class Values >
-      void evaluateAll ( const Dune::FieldVector<F,d> &x, Values &values ) const
+      template< class Point, class Values > const
+      void evaluateAll ( const Point &x, Values &values ) const
       {
-        // needed for plotting for example: assert(0);
         assert( values.size() >= size() );
         std::fill( values.begin(), values.end(), RangeType( 0 ) );
-        shapeFunctionSet_.evaluateEach( x, [ this, &values ] ( std::size_t alpha, RangeType phi_alpha ) {
+        shapeFunctionSet_.evaluateEach( position(x), [ this, &values ] ( std::size_t alpha, RangeType phi_alpha ) {
             for( std::size_t j = 0; j < size(); ++j )
               values[ j ].axpy( valueProjection()[ alpha ][ j ], phi_alpha );
           } );
       }
-      template< class Point, class Values >
-      void evaluateAll ( const Point &x, Values &values ) const
-      {
-        assert( values.size() >= size() );
-        std::fill( values.begin(), values.end(), RangeType( 0 ) );
-        if constexpr ( Point::QuadratureType::codimension == 1)
-        {
-          Std::vector < Dune::DynamicMatrix<double> > localDofVectorMatrix(2);
-          Std::vector<Std::vector<unsigned int>> mask(2,Std::vector<unsigned int>(0));
-          auto locx = x.localPosition();
-          auto normal = x.quadrature().intersection().unitOuterNormal(locx);
-          auto edgeSF = (*interpolation_)(x.quadrature().intersection(), localDofVectorMatrix, mask);
-          edgeSF.evaluateEach(locx, [&](std::size_t beta, RangeType psi)
-          {
-            if (beta < localDofVectorMatrix[0].size())
-              for (std::size_t s=0; s<mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-              {
-                std::size_t alpha = mask[0][s];
-                values[alpha].axpy( localDofVectorMatrix[0][beta][s], psi );
-              }
-          });
-        }
-        else
-        {
-          // std::cout << "B: using value projection\n";
-          shapeFunctionSet_.evaluateEach( x, [ this, &values ] ( std::size_t alpha, RangeType phi_alpha ) {
-              for( std::size_t j = 0; j < size(); ++j )
-                values[ j ].axpy( valueProjection()[ alpha ][ j ], phi_alpha );
-            } );
-        }
-      }
 
+      // TODO: use lower order shape function set for Jacobian?
+      static void axpyJac(const DomainFieldType lam, const DomainType &dom, const RangeType &ran,
+                          JacobianRangeType &ret)
+      {
+        for (int r=0;r<RangeType::dimension;++r)
+          for (int d=0;d<DomainType::dimension;++d)
+            ret[r][d] += lam*dom[d]*ran[r];
+      }
       template< class Quadrature, class DofVector, class Jacobians >
       void jacobianAll ( const Quadrature &quadrature, const DofVector &dofs, Jacobians &jacobians ) const
       {
         const std::size_t nop = quadrature.nop();
         for( std::size_t qp = 0; qp < nop; ++qp )
           jacobianAll( quadrature[ qp ], dofs, jacobians[ qp ] );
       }
-      template< class F, int d, class DofVector >
-      void jacobianAll ( const Dune::FieldVector<F,d> &x, const DofVector &dofs, JacobianRangeType &jacobian ) const
-      {
-        jacobian = JacobianRangeType( 0 );
-        shapeFunctionSet_.jacobianEach( x, [ this, &dofs, &jacobian ] ( std::size_t alpha, JacobianRangeType dphi_alpha ) {
-            for( std::size_t j = 0; j < size(); ++j )
-              jacobian.axpy( jacobianProjection()[ alpha ][ j ]*dofs[ j ], dphi_alpha );
-          } );
-      }
       template< class Point, class DofVector >
       void jacobianAll ( const Point &x, const DofVector &dofs, JacobianRangeType &jacobian ) const
       {
         jacobian = JacobianRangeType( 0 );
-        if constexpr ( Point::QuadratureType::codimension == 1)
-        {
-          Std::vector< Dune::DynamicMatrix<double> > localDofVectorMatrix(2);
-          Std::vector< Std::vector<unsigned int> > mask(2,Std::vector<unsigned int>(0));
-          auto locx = x.localPosition();
-          DomainType normal = x.quadrature().intersection().unitOuterNormal(locx);
-          const auto &jit = x.quadrature().intersection().geometry().jacobianInverseTransposed(locx);
-
-          auto edgeSF = (*interpolation_)(x.quadrature().intersection(), localDofVectorMatrix, mask);
-
-          // first step: take normal derivative if available
-          if (localDofVectorMatrix[1].size() > 0)
-            edgeSF.evaluateEach(locx, [&](std::size_t beta, RangeType psi)
-            {
-              if (beta < localDofVectorMatrix[1].size())
-              {
-                JacobianRangeType dpsi(0);
-                for (std::size_t r=0;r<dimRange;++r)
-                  dpsi[r].axpy(psi[r],normal);
-                for (std::size_t s=0; s<mask[1].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-                {
-                  std::size_t j = mask[1][s];
-                  jacobian.axpy( localDofVectorMatrix[1][beta][s]*dofs[j], dpsi );
-                }
-              }
-            });
-          else
-            shapeFunctionSet_.jacobianEach( x, [ & ] ( std::size_t alpha, JacobianRangeType dphi_alpha ) {
-                JacobianRangeType dpsi(0);
-                for (std::size_t r=0;r<dimRange;++r)
-                  dpsi[r].axpy(dphi_alpha[r]*normal,normal);
-                for( std::size_t j = 0; j < size(); ++j )
-                  jacobian.axpy( jacobianProjection()[ alpha ][ j ]*dofs[ j ], dpsi );
-              } );
-          // second step: tangential derivatives
-          edgeSF.jacobianEach(locx, [&](std::size_t beta, auto dhatpsi)
-          {
-            if (beta < localDofVectorMatrix[0].size())
-            {
-              // note: edge sfs in reference coordinate so apply scaling 1/|S|
-              JacobianRangeType dpsi;
-              for (std::size_t r=0;r<dimRange;++r)
-              {
-                jit.mv(dhatpsi[r], dpsi[r]);
-                assert( std::abs(dpsi[r]*normal) < 1e-10 );
-              }
-              for (std::size_t s=0; s<mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-              {
-                std::size_t j = mask[0][s];
-                jacobian.axpy( localDofVectorMatrix[0][beta][s]*dofs[ j ], dpsi );
-              }
-            }
-          });
-        }
-        else
-        {
-          shapeFunctionSet_.jacobianEach( x, [ this, &dofs, &jacobian ] ( std::size_t alpha, JacobianRangeType dphi_alpha ) {
-              for( std::size_t j = 0; j < size(); ++j )
-                jacobian.axpy( jacobianProjection()[ alpha ][ j ]*dofs[ j ], dphi_alpha );
-            } );
-        }
-      }
-      template< class F, int d, class Jacobians >
-      void jacobianAll ( const Dune::FieldVector<F,d> &x, Jacobians &jacobians ) const
-      {
-        assert( jacobians.size() >= size() );
-        std::fill( jacobians.begin(), jacobians.end(), JacobianRangeType( 0 ) );
-        shapeFunctionSet_.jacobianEach( x, [ this, &jacobians ] ( std::size_t alpha, JacobianRangeType dphi_alpha ) {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &dofs, &jacobian ] ( std::size_t alpha, RangeType phi_alpha ) {
+            const auto &jacobianProjectionAlpha = jacobianProjection()[alpha];
             for( std::size_t j = 0; j < size(); ++j )
-              jacobians[ j ].axpy( jacobianProjection()[ alpha ][ j ], dphi_alpha );
+              axpyJac( dofs[j], jacobianProjectionAlpha[j], phi_alpha, jacobian );
           } );
       }
-      template< class Point, class Jacobians >
+      template< class Point, class Jacobians > const
       void jacobianAll ( const Point &x, Jacobians &jacobians ) const
       {
         assert( jacobians.size() >= size() );
         std::fill( jacobians.begin(), jacobians.end(), JacobianRangeType( 0 ) );
-        if constexpr ( Point::QuadratureType::codimension == 1)
-        {
-          Std::vector< Dune::DynamicMatrix<double> > localDofVectorMatrix(2);
-          Std::vector< Std::vector<unsigned int> > mask(2,Std::vector<unsigned int>(0));
-          auto locx = x.localPosition();
-          DomainType normal = x.quadrature().intersection().unitOuterNormal(locx);
-          const auto &jit = x.quadrature().intersection().geometry().jacobianInverseTransposed(locx);
-
-          auto edgeSF = (*interpolation_)(x.quadrature().intersection(), localDofVectorMatrix, mask);
-
-          // first step: take normal derivative if available
-          if (localDofVectorMatrix[1].size() > 0)
-            edgeSF.evaluateEach(locx, [&](std::size_t beta, RangeType psi)
-            {
-              if (beta < localDofVectorMatrix[1].size())
-              {
-                JacobianRangeType dpsi(0);
-                for (std::size_t r=0;r<dimRange;++r)
-                  dpsi[r].axpy(psi[r],normal);
-                for (std::size_t s=0; s<mask[1].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-                {
-                  std::size_t alpha = mask[1][s];
-                  jacobians[alpha].axpy( localDofVectorMatrix[1][beta][s], dpsi );
-                }
-              }
-            });
-          else
-            shapeFunctionSet_.jacobianEach( x, [ & ] ( std::size_t alpha, JacobianRangeType dphi_alpha ) {
-                JacobianRangeType dpsi(0);
-                for (std::size_t r=0;r<dimRange;++r)
-                  dpsi[r].axpy(dphi_alpha[r]*normal,normal);
-                for( std::size_t j = 0; j < size(); ++j )
-                  jacobians[ j ].axpy( jacobianProjection()[ alpha ][ j ], dpsi );
-              } );
-          // second step: tangential derivatives
-          edgeSF.jacobianEach(locx, [&](std::size_t beta, auto dhatpsi)
-          {
-            if (beta < localDofVectorMatrix[0].size())
-            {
-              // note: edge sfs in reference coordinate so apply jit - also
-              // transforms to tangential derivative
-              JacobianRangeType dpsi;
-              for (std::size_t r=0;r<dimRange;++r)
-              {
-                jit.mv(dhatpsi[r], dpsi[r]);
-                assert( std::abs(dpsi[r]*normal) < 1e-10 );
-              }
-              for (std::size_t s=0; s<mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-              {
-                std::size_t alpha = mask[0][s];
-                jacobians[alpha].axpy( localDofVectorMatrix[0][beta][s], dpsi );
-              }
-            }
-          });
-        }
-        else
-        {
-          shapeFunctionSet_.jacobianEach( x, [ this, &jacobians ] ( std::size_t alpha, JacobianRangeType dphi_alpha ) {
-              for( std::size_t j = 0; j < size(); ++j )
-                jacobians[ j ].axpy( jacobianProjection()[ alpha ][ j ], dphi_alpha );
-            } );
-        }
+        shapeFunctionSet_.evaluateEach( position(x), [ this, &jacobians ] ( std::size_t alpha, RangeType phi_alpha ) {
+            const auto &jacobianProjectionAlpha = jacobianProjection()[alpha];
+            for( std::size_t j = 0; j < size(); ++j )
+              axpyJac( 1, jacobianProjectionAlpha[j], phi_alpha, jacobians[j] );
+        } );
       }
 
+      static void axpyHes(const DomainFieldType lam, const HessianMatrixType &dom, const RangeType &ran,
+                          HessianRangeType &ret)
+      {
+        for (int r=0;r<RangeType::dimension;++r)
+          for (int dx=0;dx<DomainType::dimension;++dx)
+            for (int dy=0;dy<DomainType::dimension;++dy)
+              ret[r][dx][dy] += lam*dom[dx][dy]*ran[r];
+      }
       template< class Quadrature, class DofVector, class Hessians >
       void hessianAll ( const Quadrature &quadrature, const DofVector &dofs, Hessians &hessians ) const
       {
         const std::size_t nop = quadrature.nop();
         for(std::size_t qp = 0; qp <nop; ++qp )
           hessianAll( quadrature[ qp ], dofs, hessians[ qp ] );
       }
 
       template< class Point, class DofVector >
       void hessianAll ( const Point &x, const DofVector &dofs, HessianRangeType &hessian ) const
       {
         hessian = HessianRangeType( 0 );
-        shapeFunctionSet_.hessianEach( x, [this, &dofs, &hessian ] ( std::size_t alpha, HessianRangeType d2phi_alpha ) {
+        shapeFunctionSet_.evaluateEach( position(x), [this, &dofs, &hessian ] ( std::size_t alpha, RangeType phi_alpha ) {
             const auto &hessianProjectionAlpha = hessianProjection()[alpha];
             for( std::size_t j = 0; j < size(); ++j )
-              hessian.axpy( hessianProjectionAlpha[ j ]*dofs[ j ], d2phi_alpha );
+              axpyHes( dofs[j], hessianProjectionAlpha[j], phi_alpha, hessian );
         } );
       }
-      template< class Point, class Hessians >
+
+      template< class Point, class Hessians > const
       void hessianAll ( const Point &x, Hessians &hessians ) const
       {
         assert( hessians.size() >= size() );
         std::fill( hessians.begin(), hessians.end(), HessianRangeType( 0 ) );
-        shapeFunctionSet_.hessianEach( x, [ this, &hessians ] ( std::size_t alpha, HessianRangeType d2phi_alpha ) {
+        shapeFunctionSet_.evaluateEach( position(x), [ this, &hessians ] ( std::size_t alpha, RangeType phi_alpha ) {
             const auto &hessianProjectionAlpha = hessianProjection()[alpha];
             for( std::size_t j = 0; j < size(); ++j )
-              hessians[ j ].axpy( hessianProjectionAlpha[ j ], d2phi_alpha );
+              axpyHes( 1, hessianProjectionAlpha[j], phi_alpha, hessians[j] );
         } );
       }
 
       const EntityType &entity () const { assert( entity_ ); return *entity_; }
 
+#if 0
+      template< class Point, class Factor >
+      void axpy ( const Point &x, const Factor &factor, DynamicVector<DomainType> &dofs ) const
+      {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &factor, &dofs ] ( std::size_t alpha, RangeType phi_alpha ) {
+            for( std::size_t j = 0; j < size(); ++j )
+              dofs[ j ].axpy( valueProjection()[ alpha ][ j ], factor*phi_alpha );
+          } );
+      }
+#endif
+
       /********************************************/
 
       template< class Quadrature, class Vector, class DofVector >
       void_t<typename Quadrature::QuadratureKeyType> axpy ( const Quadrature &quad, const Vector &values, DofVector &dofs ) const
       {
         const unsigned int nop = quad.nop();
         for( unsigned int qp = 0; qp < nop; ++qp )
@@ -433,25 +264,81 @@
         hessianAll(x, hessians);
         for (std::size_t i=0; i<size; ++i)
           for (std::size_t r=0; r<RangeType::dimension; ++r)
             for (std::size_t d=0; d<DomainType::dimension; ++d)
               dofs[i] += hessians[i][r][d]*hessianFactor[r][d];
       }
 
+      /********************************************/
+
+      template< class Point >
+      void axpy ( const Point &x, const JacobianRangeType &factor, DynamicVector<DomainType> &dofs ) const
+      {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &factor, &dofs ] ( std::size_t alpha, RangeType phi_alpha ) {
+            for( std::size_t j = 0; j < size(); ++j )
+            {
+              DomainType f;
+              factor.mtv(phi_alpha,f);
+              dofs[ j ].axpy( valueProjection()[ alpha ][ j ], f );
+            }
+          } );
+      }
+      template< class Point >
+      void axpy ( const Point &x, const RangeType &f1, const DomainType &f2, DynamicVector<DomainType> &dofs ) const
+      {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &f1, &f2, &dofs ] ( std::size_t alpha, RangeType phi_alpha ) {
+            for( std::size_t j = 0; j < size(); ++j )
+              dofs[ j ].axpy( valueProjection()[ alpha ][ j ], f2*(phi_alpha*f1) );
+          } );
+      }
+
+      template< class Point >
+      void axpy ( const Point &x, const JacobianRangeType &factor, DynamicVector<HessianMatrixType> &dofs ) const
+      {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &factor, &dofs ] ( std::size_t alpha, RangeType phi_alpha ) {
+            for( std::size_t j = 0; j < size(); ++j )
+              for ( std::size_t l = 0; l < dimDomain; ++l )
+                for ( std::size_t k = 0; k < dimDomain; ++k )
+                {
+                  DomainType f;
+                  factor.mtv(phi_alpha,f);
+                  dofs[ j ][l][k] +=
+                      0.5*( jacobianProjection()[ alpha ][ j ][ k ]*f[l] +
+                            jacobianProjection()[ alpha ][ j ][ l ]*f[k] );
+                }
+          } );
+      }
+      template< class Point >
+      void axpy ( const Point &x, const RangeType &factor, const DomainType &normal, DynamicVector<HessianMatrixType> &dofs ) const
+      {
+        shapeFunctionSet_.evaluateEach( position( x ), [ this, &factor, &dofs, &normal ] ( std::size_t alpha, RangeType phi_alpha ) {
+            for( std::size_t j = 0; j < size(); ++j )
+            {
+              DomainFieldType Gn = 0;
+              for ( std::size_t n = 0; n < dimDomain; ++n )
+                Gn += jacobianProjection()[ alpha ][ j ][ n ]*normal[n];
+              Gn *= phi_alpha*factor;
+              for ( std::size_t l = 0; l < dimDomain; ++l )
+                for ( std::size_t k = 0; k < dimDomain; ++k )
+                    dofs[ j ][l][k] += Gn * 0.5*(normal[k]*normal[l] + normal[l]*normal[k] );
+            }
+          } );
+      }
+
+
     private:
       template< class Point >
       DomainType position ( const Point &x ) const
       {
         return Fem::coordinate(x);
       }
 
       const EntityType *entity_ = nullptr;
       std::size_t agglomerate_;
       ShapeFunctionSet shapeFunctionSet_;
-      std::shared_ptr<InterpolationType> interpolation_;
       std::shared_ptr<Vector<ValueProjection>> valueProjections_;
       std::shared_ptr<Vector<JacobianProjection>> jacobianProjections_;
       std::shared_ptr<Vector<HessianProjection>> hessianProjections_;
       size_t size_;
     };
 
   } // namespace Vem
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/space/default.hh` & `dune-vem-2.9.dev20220529/dune/vem/space/default.hh`

 * *Files 21% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 #include <dune/fem/space/basisfunctionset/vectorial.hh>
 #include <dune/fem/space/shapefunctionset/orthonormal.hh>
 #include <dune/fem/space/shapefunctionset/proxy.hh>
 #include <dune/fem/space/shapefunctionset/vectorial.hh>
 #include <dune/fem/space/common/capabilities.hh>
 
 #include <dune/vem/space/indexset.hh>
+#include <dune/vem/agglomeration/dofmapper.hh>
 #include <dune/vem/misc/compatibility.hh>
 #include <dune/vem/misc/pseudoinverse.hh>
 #include <dune/vem/misc/leastSquares.hh>
 #include <dune/vem/misc/matrixWrappers.hh>
+#include <dune/vem/space/basisfunctionset.hh>
 #include <dune/vem/space/interpolate.hh>
 
 #include <dune/vem/misc/vector.hh>
 
 namespace Dune
 {
 
@@ -41,38 +43,39 @@
     public:
       typedef typename BaseType::Traits Traits;
       typedef typename BaseType::GridPartType GridPartType;
 
       typedef Agglomeration<GridPartType> AgglomerationType;
 
       typedef typename Traits::IndexSetType IndexSetType;
-      typedef typename Traits::InterpolationType AgglomerationInterpolationType;
-      typedef typename Traits::BasisSetsType BasisSetsType;
+      typedef typename Traits::template InterpolationType<Traits> AgglomerationInterpolationType;
+      typedef typename AgglomerationInterpolationType::TestBasisSetsType TestBasisSetsType;
 
     public:
       typedef typename BaseType::BasisFunctionSetType BasisFunctionSetType;
       typedef typename BaseType::BlockMapperType BlockMapperType;
 
       typedef typename BaseType::EntityType EntityType;
-      typedef typename BasisSetsType::EdgeShapeFunctionSetType EdgeShapeFunctionSetType;
+      typedef typename Traits::EdgeShapeFunctionSetType EdgeShapeFunctionSetType;
       typedef typename BasisFunctionSetType::DomainFieldType DomainFieldType;
       typedef typename BasisFunctionSetType::DomainType DomainType;
 
       typedef typename BasisFunctionSetType::RangeType RangeType;
       typedef typename BasisFunctionSetType::JacobianRangeType JacobianRangeType;
       typedef typename BasisFunctionSetType::HessianRangeType HessianRangeType;
       typedef typename GridPartType::template Codim<0>::EntityType ElementType;
       typedef typename GridPartType::template Codim<0>::EntitySeedType ElementSeedType;
 
-      static constexpr int dimDomain = Traits::dimDomain;
-      static constexpr size_t blockSize = BaseType::localBlockSize;
+      static const int dimDomain = Traits::dimDomain;
 
       typedef Dune::Fem::ElementQuadrature<GridPartType, 0> Quadrature0Type;
       typedef Dune::Fem::ElementQuadrature<GridPartType, 1> Quadrature1Type;
 
+      typedef typename Traits::ScalarBasisFunctionSetType::HessianMatrixType HessianMatrixType;
+
       typedef DynamicMatrix<typename BasisFunctionSetType::DomainFieldType> Stabilization;
 
       using BaseType::gridPart;
 
       enum { hasLocalInterpolate = false };
 
       // for interpolation
@@ -86,40 +89,42 @@
           const EntityType &element_;
       };
 
       // basisChoice:
       // 1: use onb for inner moments but not for computing projections
       // 2: use onb for both the inner moments and computation of projection
       // 3: don't use onb at all
-      DefaultAgglomerationVEMSpace(AgglomerationType &agglom,
+      DefaultAgglomerationVEMSpace(AgglomerationType &agglomeration,
           const unsigned int polOrder,
-          const typename Traits::BasisSetsType &basisSets,
+          const typename IndexSetType::TestSpacesType &testSpaces,
           int basisChoice,
           bool edgeInterpolation)
-      : BaseType(agglom.gridPart()),
-        polOrder_(basisSets.maxOrder()),
-        basisSets_(basisSets),
+      : BaseType(agglomeration.gridPart()),
+        polOrder_(polOrder),
         basisChoice_(basisChoice),
+        useOnb_(basisChoice == 2),
         edgeInterpolation_(edgeInterpolation),
-        agIndexSet_(agglom),
-        blockMapper_(agIndexSet_, basisSets_.dofsPerCodim()),
-        interpolation_(new AgglomerationInterpolationType(blockMapper().indexSet(), basisSets_, polOrder, basisChoice != 3)),
+        agIndexSet_(agglomeration, testSpaces),
+        blockMapper_(agIndexSet_, agIndexSet_.dofsPerCodim()),
+        interpolation_(blockMapper().indexSet(), polOrder, basisChoice != 3),
+        testBasisSets_(polOrder_, agIndexSet_.maxEdgeDegree(), useOnb_),
         counter_(0),
         useThreads_(Fem::MPIManager::numThreads()),
         valueProjections_(new Vector<
             typename Traits::ScalarBasisFunctionSetType::ValueProjection>()),
         jacobianProjections_(new Vector<
             typename Traits::ScalarBasisFunctionSetType::JacobianProjection>()),
         hessianProjections_(new Vector<
             typename Traits::ScalarBasisFunctionSetType::HessianProjection>()),
         stabilizations_(new Vector<Stabilization>())
       {
-        if (basisChoice != 3) // !!!!! get order information from BasisSets
-          agglomeration().onbBasis(basisSets_.maxOrder());
-        // std::cout << "using " << useThreads_ << " threads\n";
+        std::cout << "using " << useThreads_ << " threads\n";
+        if (basisChoice != 3)
+          this->agglomeration().onbBasis(order());
+        update(true);
       }
       DefaultAgglomerationVEMSpace(const DefaultAgglomerationVEMSpace&) = delete;
       DefaultAgglomerationVEMSpace& operator=(const DefaultAgglomerationVEMSpace&) = delete;
       ~DefaultAgglomerationVEMSpace() {}
 
       void update(bool first=false)
       {
@@ -160,21 +165,21 @@
       const typename Traits::ScalarBasisFunctionSetType scalarBasisFunctionSet(const EntityType &entity) const
       {
         const std::size_t agglomerate = agglomeration().index(entity);
         assert(agglomerate<valueProjections().size());
         assert(agglomerate<jacobianProjections().size());
         assert(agglomerate<hessianProjections().size());
         return typename Traits::ScalarBasisFunctionSetType(entity, agglomerate,
-                        valueProjections_, jacobianProjections_, hessianProjections_,
-                        basisSets_.basisFunctionSet(agglomeration(), entity),
-                        interpolation_
+                       valueProjections_, jacobianProjections_, hessianProjections_,
+                       testBasisSets_.bbBasisFunctionSet(agglomeration(), entity)
                );
       }
       const BasisFunctionSetType basisFunctionSet(const EntityType &entity) const
       {
+        // if constexpr (vectorSpace) return scalarBasisFunctionSet(entity); else
         return BasisFunctionSetType( std::move(scalarBasisFunctionSet(entity)) );
       }
 
       BlockMapperType &blockMapper() const { return blockMapper_; }
 
       // extra interface methods
       static constexpr bool continuous() noexcept { return false; }
@@ -199,52 +204,51 @@
       //////////////////////////////////////////////////////////
       /** \brief return local interpolation for given entity
        *
        *  \param[in]  entity  grid part entity
        */
       InterpolationType interpolation(const EntityType &entity) const
       {
-        return InterpolationType(blockMapper().indexSet(), basisSets_, entity);
+        return InterpolationType(blockMapper().indexSet(), entity);
       }
 
-      const AgglomerationInterpolationType& interpolation() const
+      AgglomerationInterpolationType interpolation() const
       {
-        return *interpolation_;
+        return interpolation_;
       }
 
-    protected:
+    private:
       template <int codim>
-      static std::size_t sizeONB(std::size_t order)
+      std::size_t sizeONB(std::size_t order)
       {
         return Dune::Fem::OrthonormalShapeFunctions<DomainType::dimension - codim>:: size(order) *
                Traits::ScalarBasisFunctionSetType::RangeType::dimension;
+               // Traits::baseRangeDimension;
       }
 
       template <class T>
       using Vector = Std::vector<T>;
       auto& valueProjections() const { return *valueProjections_; }
       auto& jacobianProjections() const { return *jacobianProjections_; }
       auto& hessianProjections() const { return *hessianProjections_; }
       auto& stabilizations() const { return *stabilizations_; }
 
-      virtual void finalize(const Std::vector<Std::vector<ElementSeedType> > &entitySeeds, unsigned int agglomerate)
-      {}
-      virtual void setupConstraintRHS(const Std::vector<Std::vector<ElementSeedType> > &entitySeeds, unsigned int agglomerate, DynamicMatrix<DomainFieldType> &RHSconstraintsMatrix, double volume)
-      {}
       void buildProjections(const Std::vector<Std::vector<ElementSeedType> > &entitySeeds,
                             unsigned int start, unsigned int end);
 
       // issue with making these const: use of delete default constructor in some python bindings...
       unsigned int polOrder_;
-      BasisSetsType basisSets_;
       int basisChoice_;
+      const bool useOnb_;
       bool edgeInterpolation_;
       IndexSetType agIndexSet_;
       mutable BlockMapperType blockMapper_;
-      std::shared_ptr<AgglomerationInterpolationType> interpolation_;
+      AgglomerationInterpolationType interpolation_;
+      // ScalarShapeFunctionSetType scalarShapeFunctionSet_;
+      TestBasisSetsType testBasisSets_;
       std::size_t counter_;
       int useThreads_;
       std::shared_ptr<Vector<typename Traits::ScalarBasisFunctionSetType::ValueProjection>> valueProjections_;
       std::shared_ptr<Vector<typename Traits::ScalarBasisFunctionSetType::JacobianProjection>> jacobianProjections_;
       std::shared_ptr<Vector<typename Traits::ScalarBasisFunctionSetType::HessianProjection>> hessianProjections_;
       std::shared_ptr<Vector<Stabilization>> stabilizations_;
     };
@@ -254,543 +258,334 @@
 
     template<class Traits>
     inline void DefaultAgglomerationVEMSpace<Traits> :: buildProjections(
           const Std::vector<Std::vector<ElementSeedType> > &entitySeeds,
           unsigned int start, unsigned int end )
     {
       int polOrder = order();
-      typedef typename BasisSetsType::EdgeShapeFunctionSetType EdgeTestSpace;
-      // this is scalar space in the case that vectorial extension is used
-      typedef typename BasisSetsType::ShapeFunctionSetType::FunctionSpaceType FunctionSpaceType;
-      typedef typename FunctionSpaceType::DomainType DomainType;
-      typedef typename FunctionSpaceType::RangeFieldType RangeFieldType;
-      typedef typename FunctionSpaceType::RangeType RangeType;
-      typedef typename FunctionSpaceType::JacobianRangeType JacobianRangeType;
-      typedef typename FunctionSpaceType::HessianRangeType HessianRangeType;
-      const std::size_t dimDomain = DomainType::dimension;
-      const std::size_t dimRange = RangeType::dimension;
-
-      const std::size_t numShapeFunctions = basisSets_.size(0);
-      const std::size_t numGradShapeFunctions = basisSets_.size(1);
-      const std::size_t numHessShapeFunctions = basisSets_.size(2);
-      const std::size_t numConstraintShapeFunctions = basisSets_.constraintSize();
-
-      double maxStab = 0;
-
-      /*
-      std::cout << "pol order / dimDomain / dimRange: "
-                << polOrder << " / "
-                << dimDomain << " / "
-                << dimRange << std::endl;
-      std::cout << "num val / grad / hess / constr shapefunctions: "
-                << numShapeFunctions << " / "
-                << numGradShapeFunctions << " / "
-                << numHessShapeFunctions << " / "
-                << numConstraintShapeFunctions << std::endl;
-      */
+      typedef typename Traits::BBBasisFunctionSetType InnerTestSpace;
+      typedef typename Traits::EdgeShapeFunctionSetType EdgeTestSpace;
+      AgglomerationInterpolationType interpolation(blockMapper().indexSet(), polOrder, basisChoice_ != 3);
+
+      const std::size_t baseRangeDimension = InnerTestSpace::RangeType::dimension;
+      assert( InnerTestSpace::RangeType::dimension == Traits::baseRangeDimension );
+      assert( EdgeTestSpace::RangeType::dimension == Traits::baseRangeDimension );
+
+      Std::vector<int> orders = agIndexSet_.orders();
+      const std::size_t numShapeFunctions = testBasisSets_.size();
+      const std::size_t numHessShapeFunctions =
+            polOrder==1? baseRangeDimension :
+            std::min( numShapeFunctions, sizeONB<0>(std::max(orders[2], polOrder - 2)) );
+      std::size_t numGradShapeFunctions =
+               std::min( numShapeFunctions, sizeONB<0>(std::max(orders[1], polOrder - 1)) );
+      const std::size_t numInnerShapeFunctions = orders[0] < 0 ? 0 : sizeONB<0>(orders[0]);
 
       // set up matrices used for constructing gradient, value, and edge projections
       // Note: the code is set up with the assumption that the dofs suffice to compute the edge projection
       //       Is this still the case?
 
-      // Mass matrices and their inverse: HpGrad, HpHess, HpGradInv, HpHessInv
-      // !!! HpGrad/HpHess are not needed after inversion so use HpGradInv/HpHessInv from the start
-      DynamicMatrix<DomainFieldType> HpGrad, HpHess, HpGradInv, HpHessInv;
+      // Mass matrices and their inverse: Hp, HpGrad, HpHess, HpInv, HpGradInv, HpHessInv
+      DynamicMatrix<DomainFieldType> Hp, HpGrad, HpHess, HpInv, HpGradInv, HpHessInv;
+      Hp.resize(numShapeFunctions, numShapeFunctions, 0);
       HpGrad.resize(numGradShapeFunctions, numGradShapeFunctions, 0);
       HpHess.resize(numHessShapeFunctions, numHessShapeFunctions, 0);
 
       // interpolation of basis function set used for least squares part of value projection
       DynamicMatrix<DomainFieldType> D;
       // constraint matrix for value projection
       DynamicMatrix<DomainFieldType> constraintValueProj;
+      constraintValueProj.resize(numInnerShapeFunctions, numShapeFunctions, 0);
       // right hand sides and solvers for CLS for value projection (b: ls, d: constraints)
-      Dune::DynamicVector<DomainFieldType> b;
-      DynamicMatrix<DomainFieldType> RHSconstraintsMatrix;
+      Dune::DynamicVector<DomainFieldType> b, d;
+      d.resize(numInnerShapeFunctions, 0);
 
       // matrices for edge projections
       Std::vector<Dune::DynamicMatrix<double> > edgePhiVector(2);
-      edgePhiVector[0].resize(basisSets_.edgeSize(0), basisSets_.edgeSize(0), 0);
-      edgePhiVector[1].resize(basisSets_.edgeSize(1), basisSets_.edgeSize(1), 0);
-
-      // std::cout << "edgePhiVector:" << basisSets_.edgeSize(0) << "," <<  basisSets_.edgeSize(1) << std::endl;
+      edgePhiVector[0].resize(interpolation.edgeSize(0), interpolation.edgeSize(0), 0);
+      edgePhiVector[1].resize(interpolation.edgeSize(1), interpolation.edgeSize(1), 0);
 
       // matrix for rhs of gradient and hessian projections
-      DynamicMatrix<DomainFieldType> R;
-      DynamicMatrix<DomainFieldType> P;
-      std::vector<RangeType> phi0Values;
-      std::vector<JacobianRangeType> psi1Values;
+      DynamicMatrix<DomainType> R;
+      DynamicMatrix<Dune::FieldMatrix<DomainFieldType,dimDomain,dimDomain>> P;
 
       // start iteration over all polygons
       for (std::size_t agglomerate = start; agglomerate < end; ++agglomerate)
       {
-        // case 1: dimRange=1 (e.g. a vector extension is applied later)
-        //         then the blockSize will be the actual vector size but we
-        //         are computing the scalar basisfunctions here
-        // case 2: dimRange>1: in this case blockSize=dimRange or blockSize=1.
-        //         In the second case the blockMapper is already returning the correct size.
-        const std::size_t numDofs = blockMapper().numDofs(agglomerate) *
-               std::min(dimRange, blockSize);
-        /*
-        std::cout << "numDofs: " << numDofs << " = "
-                  << blockMapper().numDofs(agglomerate) << " * "
-                  << blockSize << std::endl;
-        */
+        const std::size_t numDofs = blockMapper().numDofs(agglomerate) * baseRangeDimension;
 
-        phi0Values.resize(numDofs);
-        psi1Values.resize(numDofs);
-
-        const DomainFieldType H0 = blockMapper_.indexSet().volume(agglomerate);
+        const int numEdges = agIndexSet_.subAgglomerates(agglomerate, IndexSetType::dimension - 1);
 
         //////////////////////////////////////////////////////////////////////////////
         /// resize matrices that depend on the local number of degrees of freedom  ///
         //////////////////////////////////////////////////////////////////////////////
 
         auto &valueProjection = valueProjections()[agglomerate];
         auto &jacobianProjection = jacobianProjections()[agglomerate];
         auto &hessianProjection = hessianProjections()[agglomerate];
         valueProjection.resize(numShapeFunctions);
-        jacobianProjection.resize(numGradShapeFunctions);
-        hessianProjection.resize(numHessShapeFunctions);
+        jacobianProjection.resize(numShapeFunctions);
+        hessianProjection.resize(numShapeFunctions);
         for (std::size_t alpha = 0; alpha < numShapeFunctions; ++alpha)
-          valueProjection[alpha].resize(numDofs, DomainFieldType(0));
-        for (std::size_t alpha = 0; alpha < numGradShapeFunctions; ++alpha)
-          jacobianProjection[alpha].resize(numDofs, DomainFieldType(0));
-        for (std::size_t alpha = 0; alpha < numHessShapeFunctions; ++alpha)
-          hessianProjection[alpha].resize(numDofs, DomainFieldType(0));
+        {
+          valueProjection[alpha].resize(numDofs, 0);
+          jacobianProjection[alpha].resize(numDofs, DomainType(0));
+          hessianProjection[alpha].resize(numDofs, HessianMatrixType(0));
+        }
 
         // value projection CLS
-        std::size_t numConstraints = (numDofs >= numShapeFunctions)? // LS is large enough
-                          numConstraintShapeFunctions : numShapeFunctions-numDofs;
-        // std::cout << "numConstraints " << numConstraints << std::endl;
         constraintValueProj = 0;
         D.resize(numDofs, numShapeFunctions, 0);
-        RHSconstraintsMatrix.resize(numDofs, numConstraints, 0);
-        constraintValueProj.resize(numConstraints, numShapeFunctions, 0);
-
         b.resize(numDofs, 0);
+        std::fill(d.begin(),d.end(),0);
 
         // rhs structures for gradient/hessian projection
-        R.resize(numGradShapeFunctions, numDofs, 0);
+        R.resize(numGradShapeFunctions, numDofs, DomainType(0));
         P.resize(numHessShapeFunctions, numDofs, 0);
 
         //////////////////////////////////////////////////////////////////////////
         /// compute L(B) and the mass matrices ///////////////////////////////////
         //////////////////////////////////////////////////////////////////////////
 
+        Hp = 0;
         HpGrad = 0;
         HpHess = 0;
         for (const ElementSeedType &entitySeed : entitySeeds[agglomerate])
         {
           const ElementType &element = gridPart().entity(entitySeed);
           const auto geometry = element.geometry();
-          Quadrature0Type quadrature(element, 3 * polOrder);
+          Quadrature0Type quadrature(element, 2 * polOrder);
 
           // get the bounding box monomials and apply all dofs to them
           // GENERAL: these are the same as used as test function in 'interpolation'
-          const auto &shapeFunctionSet = basisSets_.basisFunctionSet(agglomeration(), element);
+          const typename Traits::BBBasisFunctionSetType &shapeFunctionSet
+                  = testBasisSets_.bbBasisFunctionSet(agglomeration(), element);
 
-          interpolation().interpolateBasis(element, shapeFunctionSet.valueBasisSet(), D);
-          // std::cout << "checkpoint inerpolate basis" << std::endl;
-          // compute mass matrices
-          for (std::size_t qp = 0; qp < quadrature.nop(); ++qp)
-          {
+          interpolation.interpolateBasis(element, shapeFunctionSet, D);
+
+          // compute mass matrices Hp, HpGrad, and the gradient matrices G^l
+          // CHANGE: need to change this to different 'evaluateEach' calls'
+          // CHANGE: constraintValueProjection?
+          for (std::size_t qp = 0; qp < quadrature.nop(); ++qp) {
             const DomainFieldType weight =
                     geometry.integrationElement(quadrature.point(qp)) * quadrature.weight(qp);
-            shapeFunctionSet.evaluateEach(quadrature[qp], [&](std::size_t alpha, RangeType phi)
-            {
-              shapeFunctionSet.evaluateEach(quadrature[qp], [&](std::size_t beta, RangeType psi)
-              {
-                if (alpha < numConstraintShapeFunctions)
-                {
+            shapeFunctionSet.evaluateEach(quadrature[qp], [&](std::size_t alpha, typename InnerTestSpace::RangeType phi) {
+              shapeFunctionSet.evaluateEach(quadrature[qp], [&](std::size_t beta, typename InnerTestSpace::RangeType psi) {
+                Hp[alpha][beta] += phi * psi * weight;
+                if (alpha < numGradShapeFunctions && beta < numGradShapeFunctions) // basis set is hierarchic so we can compute HpGrad using the order p shapeFunctionSet
+                  HpGrad[alpha][beta] += phi * psi * weight;
+                if (alpha < numHessShapeFunctions && beta < numHessShapeFunctions)
+                  HpHess[alpha][beta] += phi * psi * weight;
+                if (alpha < numInnerShapeFunctions)
                   constraintValueProj[alpha][beta] += phi * psi * weight;
-                }
               });
             });
-            // the following is only for the C^1 spaces (especially lowest order on triangles)
-            // adding a constraint on the average of the laplace
-            if (basisSets_.edgeSize(1)>0 && numConstraints == numConstraintShapeFunctions+1)
-            {
-              std::size_t alpha = constraintValueProj.size()-1;
-              const auto &vbs = shapeFunctionSet.valueBasisSet();
-              vbs.hessianEach(quadrature[qp], [&](std::size_t beta, HessianRangeType psi)
-              {
-                double laplace = psi[0][0][0] + psi[0][1][1];
-                constraintValueProj[alpha][beta] += laplace * weight;
-              });
-            }
-            else assert(numConstraints == numConstraintShapeFunctions); // no other case covered yet
-
-            if (numGradShapeFunctions>0)
-              shapeFunctionSet.jacobianEach(quadrature[qp], [&](std::size_t alpha, JacobianRangeType phi) {
-                shapeFunctionSet.jacobianEach(quadrature[qp], [&](std::size_t beta, JacobianRangeType psi) {
-                  for (std::size_t i=0;i<dimRange;++i)
-                    for (std::size_t j=0;j<dimDomain;++j)
-                      HpGrad[alpha][beta] += phi[i][j] * psi[i][j] * weight;
-                });
-              });
-            if (numHessShapeFunctions>0)
-              shapeFunctionSet.hessianEach(quadrature[qp], [&](std::size_t alpha, HessianRangeType phi) {
-                shapeFunctionSet.hessianEach(quadrature[qp], [&](std::size_t beta, HessianRangeType psi) {
-                  for (std::size_t i=0;i<dimRange;++i)
-                    for (std::size_t j=0;j<dimDomain;++j)
-                      for (std::size_t k=0;k<dimDomain;++k)
-                        HpHess[alpha][beta] += phi[i][j][k] * psi[i][j][k] * weight;
-                });
-              });
           } // quadrature loop
-          // std::cout << "checkpoint mass matrices" << std::endl;
         } // loop over triangles in agglomerate
 
         // compute inverse mass matrix
-        if (numGradShapeFunctions>0)
-        {
-          HpGradInv = HpGrad;
-          try
-          {
-            HpGradInv.invert();
-          }
-          catch (const FMatrixError&)
-          {
-            std::cout << "HpGradInv.invert() failed!\n";
-            assert(0);
-            throw FMatrixError();
-          }
-        }
-
-        if (numHessShapeFunctions>0)
-        {
-          HpHessInv = HpHess;
-          HpHessInv.invert();
-        }
+        // GENERAL: should we simply assume that the mass matrix is diagonal and not compute anything here?
+        HpInv = Hp;
+        HpInv.invert();
+        HpGradInv = HpGrad;
+        HpGradInv.invert();
+        HpHessInv = HpHess;
+        HpHessInv.invert();
 
         //////////////////////////////////////////////////////////////////////////
-        /// ValueProjection /////////////////////////////////////////////////////
+        /// ValueProjecjtion /////////////////////////////////////////////////////
         //////////////////////////////////////////////////////////////////////////
-        // std::cout << "checkpoint constructed constraint value proj matrix " << std::endl;
-#if 0
-        {
-          for (std::size_t beta = 0; beta < numConstraints; ++beta )
-          {
-            std::cout << "CMatrix_" << beta << " = ";
-            for (std::size_t alpha = 0; alpha < numShapeFunctions; ++alpha)
-            {
-              std::cout << constraintValueProj[beta][alpha] << " ";
-            }
-            std::cout << std::endl;
-          }
-        }
-#endif
-        // set up matrix RHSconstraintsMatrix
-        setupConstraintRHS(entitySeeds, agglomerate, RHSconstraintsMatrix, H0);
 
-#if 0
-        {
-            std::cout << "Constraint RHS:\n";
-            for (std::size_t alpha=0; alpha < numDofs; ++alpha )
-            {
-              for (std::size_t beta=0; beta < numConstraints; ++beta )
-                std::cout << RHSconstraintsMatrix[alpha][beta] << ", ";
-              std::cout << std::endl;
-            }
-        }
-#endif
-#if 0
-        // std::cout << "checkpoint setupRHS constraints matrix done" << std::endl;
+        DomainFieldType H0 = blockMapper_.indexSet().volume(agglomerate);
+        auto leastSquaresMinimizer = LeastSquares(D, constraintValueProj);
+        for ( std::size_t beta = 0; beta < numDofs; ++beta )
         {
-            std::cout << "Basis interpolation\n";
-            for (std::size_t alpha=0;alpha<D.size();++alpha)
-            {
-              for (std::size_t beta=0;beta<D[alpha].size();++beta)
-                std::cout << D[alpha][beta] << " ";
-              std::cout << std::endl;
-            }
-        }
-#endif
-
-        if (numConstraints < numShapeFunctions)
-        { // need to use a CLS approach
-          // std::cout << "CLS" << std::endl;
-          auto leastSquaresMinimizer = LeastSquares(D, constraintValueProj);
-          for ( std::size_t beta = 0; beta < numDofs; ++beta )
-          {
-            // set up vectors b (rhs for least squares)
-            b[ beta ] = 1;
+          // set up vectors b (rhs for least squares)
+          b[ beta ] = 1;
 
-            // if( beta >= numDofs - numConstraintShapeFunctions )
-              // assert( std::abs( d[ beta - numDofs + numConstraintShapeFunctions ] - H0 ) < 1e-13);
-
-            // compute CLS solution and store in right column of 'valueProjection'
-            auto colValueProjection = vectorizeMatrixCol( valueProjection, beta );
-            colValueProjection = leastSquaresMinimizer.solve(b, RHSconstraintsMatrix[beta]);
-
-            b[beta] = 0;
-          }
-        }
-        else
-        { // constraintValueProj is square and can be inverted
-          try
-          {
-            constraintValueProj.invert();
-          }
-          catch (const FMatrixError&)
-          {
-            std::cout << "constraintValueProj.invert() failed!\n";
-            for (std::size_t alpha=0;alpha<constraintValueProj.size();++alpha)
-            {
-              for (std::size_t beta=0;beta<constraintValueProj[alpha].size();++beta)
-                std::cout << constraintValueProj[alpha][beta] << " ";
-              std::cout << std::endl;
-            }
-            assert(0);
-            throw FMatrixError();
-          }
-          for (std::size_t beta = 0; beta < numDofs; ++beta )
-          {
-            for (std::size_t alpha = 0; alpha < numShapeFunctions; ++alpha)
-            {
-              valueProjection[alpha][beta] = 0;
-              for (std::size_t i = 0; i < constraintValueProj.cols(); ++i)
-              {
-                valueProjection[alpha][beta] += constraintValueProj[alpha][i] * RHSconstraintsMatrix[beta][i];
-              }
-            }
-          }
-        }
-#if 0
-        std::cout << "*******************************\n";
-        std::cout << "** RHS constraints 1        **\n";
-        std::cout << "*******************************\n";
-        for (std::size_t beta = 0; beta < numDofs; ++beta )
-        {
-          std::cout << "phi_" << beta << " = ";
-          for (std::size_t alpha = 0; alpha < numConstraintShapeFunctions; ++alpha)
+          // set up vector d (rhs for constraints)
+          interpolation.valueL2constraints(beta, H0, D, d);
+          if( beta >= numDofs - numInnerShapeFunctions )
           {
-            std::cout << RHSconstraintsMatrix[beta][alpha] << " ";
+            assert( std::abs( d[ beta - numDofs + numInnerShapeFunctions ] - H0 ) < 1e-13 );
           }
-          std::cout << std::endl;
-        }
-        std::cout << "*******************************\n";
-#endif
 
-#if 0
-        std::cout << "*******************************\n";
-        std::cout << "****  Value projection  ****\n";
-        std::cout << "*******************************\n";
-        for (std::size_t beta = 0; beta < numDofs; ++beta )
-        {
-          std::cout << "phi_" << beta << " = ";
-          for (std::size_t alpha = 0; alpha < numShapeFunctions; ++alpha)
-          {
-            std::cout << valueProjection[alpha][beta] << " ";
-          }
-          std::cout << std::endl;
+          // compite CLS solution and store in right column of 'valueProjection'
+          auto colValueProjection = vectorizeMatrixCol( valueProjection, beta );
+          colValueProjection = leastSquaresMinimizer.solve(b, d);
+
+          b[beta] = 0;
         }
-        std::cout << "*******************************\n";
-#endif
-        if (numGradShapeFunctions==0) continue;
 
         //////////////////////////////////////////////////////////////////////////
-        /// GradientProjection //////////////////////////////////////////////////
+        /// GradientProjecjtion //////////////////////////////////////////////////
         //////////////////////////////////////////////////////////////////////////
 
         for (const ElementSeedType &entitySeed : entitySeeds[agglomerate])
         {
           const ElementType &element = gridPart().entity(entitySeed);
           const auto geometry = element.geometry();
           const auto &refElement = ReferenceElements<typename GridPartType::ctype, GridPartType::dimension>::general( element.type());
 
           // get the bounding box monomials and apply all dofs to them
-          const auto &shapeFunctionSet = basisSets_.basisFunctionSet(agglomeration(), element);
+          const typename Traits::BBBasisFunctionSetType &shapeFunctionSet
+                  = testBasisSets_.bbBasisFunctionSet(agglomeration(), element);
+          const typename Traits::EdgeShapeFunctionSetType &edgeShapeFunctionSet
+                  = testBasisSets_.edgeBasisFunctionSet(agglomeration(), element);
 
           auto vemBasisFunction = scalarBasisFunctionSet(element);
 
           // compute the boundary terms for the gradient projection
           for (const auto &intersection : intersections(gridPart(), element))
           {
             // ignore edges inside the given polygon
             if (!intersection.boundary() && (agglomeration().index(intersection.outside()) == agglomerate))
               continue;
             assert(intersection.conforming());
-            const auto &geo = intersection.geometry();
-
-            const typename BasisSetsType::EdgeShapeFunctionSetType edgeShapeFunctionSet
-                  = basisSets_.edgeBasisFunctionSet(agglomeration(),
-                  intersection, blockMapper().indexSet().twist(intersection));
 
             Std::vector<Std::vector<unsigned int>>
               mask(2,Std::vector<unsigned int>(0)); // contains indices with Phi_mask[i] is attached to given edge
-            // calling the interpolation can resize the edge vector to add the 'normal' derivative vertex dof so we need to resize again
-            edgePhiVector[0].resize(basisSets_.edgeSize(0), basisSets_.edgeSize(0), 0);
-            edgePhiVector[1].resize(basisSets_.edgeSize(1), basisSets_.edgeSize(1), 0);
-
-            interpolation()(intersection, edgeShapeFunctionSet, edgePhiVector, mask);
+            edgePhiVector[0] = 0;
+            edgePhiVector[1] = 0;
+            // CHANGE: will this still work?
+            interpolation(intersection, edgeShapeFunctionSet, edgePhiVector, mask);
 
             auto normal = intersection.centerUnitOuterNormal();
             typename Dune::FieldMatrix<DomainFieldType,dimDomain,dimDomain> factorTN, factorNN;
-            DomainType tau = geo.corner(1);
-            tau -= geo.corner(0);
+            DomainType tau = intersection.geometry().corner(1);
+            tau -= intersection.geometry().corner(0);
             double h = tau.two_norm();
             tau /= h;
             for (std::size_t i = 0; i < factorTN.rows; ++i)
               for (std::size_t j = 0; j < factorTN.cols; ++j)
               {
                 factorTN[i][j] = 0.5 * (normal[i] * tau[j] + normal[j] * tau[i]);
                 factorNN[i][j] = 0.5 * (normal[i] * normal[j] + normal[j] * normal[i]);
               }
 
             // now compute int_e Phi_mask[i] m_alpha
-            Quadrature1Type quadrature(gridPart(), intersection, 3 * polOrder, Quadrature1Type::INSIDE);
+            Quadrature1Type quadrature(gridPart(), intersection, 2 * polOrder, Quadrature1Type::INSIDE);
             for (std::size_t qp = 0; qp < quadrature.nop(); ++qp)
             {
               auto x = quadrature.localPoint(qp);
               auto y = intersection.geometryInInside().global(x);
               const DomainFieldType weight = intersection.geometry().integrationElement(x) * quadrature.weight(qp);
-              const auto &jit = geo.jacobianInverseTransposed(x);
-              auto normal = intersection.unitOuterNormal(x);
-              shapeFunctionSet.jacobianEach(y, [&](std::size_t alpha, JacobianRangeType phi)
-              {
-                  // evaluate each here for edge shape fns
-                  // first check if we should be using interpolation (for the
-                  // existing edge moments - or for H4 space)
-                  // !!!!! sfs.degree(alpha) <= basisSets_.edgeOrders()[0]
-                  if (alpha < dimDomain*sizeONB<0>(basisSets_.edgeValueMoments())       // have enough edge momentsa
-                      || edgePhiVector[0].size() >= dimRange*(polOrder+1)                    // interpolation is exact enough
-                      || edgeInterpolation_)                                                 // user want interpolation no matter what
+              // CHANGE: which 'sfs' should this be - what is the // // 'RangeType'?
+              // CHANGE: 'evaluateAll' for hessian must be done seperately
+              shapeFunctionSet.evaluateEach(y, [&](std::size_t alpha, typename Traits::BBBasisFunctionSetType::RangeType phi) {
+                  if (alpha < numGradShapeFunctions)
                   {
-                    edgeShapeFunctionSet.evaluateEach(x, [&](std::size_t beta,
-                          typename BasisSetsType::EdgeShapeFunctionSetType::RangeType psi)
+                    // evaluate each here for edge shape fns
+                    // first check if we should be using interpolation (for the
+                    // existing edge moments - or for H4 space)
+                    if (alpha < sizeONB<0>( agIndexSet_.edgeOrders()[0])       // have enough edge momentsa
+                        || edgePhiVector[0].size() == polOrder+1               // interpolation is exact
+                        || edgeInterpolation_)                                 // user want interpolation no matter what
                     {
-                      if (beta < edgePhiVector[0].size())
-                        for (std::size_t s=0; s<mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-                          for (std::size_t i=0;i<dimRange;++i)
-                            for (std::size_t j=0;j<dimDomain;++j)
-                              R[alpha][mask[0][s]] += weight *
-                                edgePhiVector[0][beta][s] * psi[i] * phi[i][j] * normal[j];
-                      else
-                        assert(0);
-                    });
+                      edgeShapeFunctionSet.evaluateEach(x, [&](std::size_t beta,
+                           typename Traits::EdgeShapeFunctionSetType::RangeType psi) {
+                        if (beta < edgePhiVector[0].size())
+                          for (std::size_t s = 0; s < mask[0].size(); ++s)// note that edgePhi is the transposed of the basis transform matrix
+                            R[alpha][mask[0][s]].axpy(edgePhiVector[0][beta][s] * psi*phi * weight, normal);
+                      });
+                    }
+                    else // use value projection
+                    {
+                      auto factor = normal;
+                      factor *= weight;
+                      vemBasisFunction.axpy(y, phi, factor, R[alpha]);
+                    }
                   }
-                  else // use value projection
+
+                  // compute the phi.tau boundary terms for the hessian projection using d/ds Pi^e
+                  if (alpha < numHessShapeFunctions && interpolation.edgeSize(1) > 0)
                   {
-                    vemBasisFunction.evaluateAll(y, phi0Values);
-                    for (std::size_t s=0;s<numDofs;++s)
-                      for (std::size_t i=0;i<dimRange;++i)
-                        for (std::size_t j=0;j<dimDomain;++j)
-                          R[alpha][s] += weight * phi0Values[s][i] * phi[i][j] * normal[j];
-                  }
-              });
-              shapeFunctionSet.hessianEach(y, [&](std::size_t alpha, HessianRangeType phi)
-              {
-                // compute the phi.tau boundary terms for the hessian projection using d/ds Pi^e
-                if ( 1 ) // basisSets_.edgeSize(1) > 0 ) // can always use the edge projection?
-                {
-                  // jacobian each here for edge shape fns
-                  edgeShapeFunctionSet.jacobianEach(x, [&](std::size_t beta, auto dhatpsi) {
-                      // note: the edgeShapeFunctionSet is defined over
-                      // the reference element of the edge so the jit has to be applied here
-                      JacobianRangeType dpsi;
-                      for (std::size_t r=0;r<dimRange;++r)
-                        jit.mv(dhatpsi[r], dpsi[r]);
-                      if (beta < edgePhiVector[0].size())
-                      {
-                        double gradPsiDottau;
-
-                        // GENERAL: this assumed that the Pi_0 part of Pi^e is not needed?
-                        for (std::size_t r = 0; r < dimRange; ++r)
-                        {
-                          gradPsiDottau = dpsi[r] * tau;
+                    auto jit = intersection.geometry().jacobianInverseTransposed(x);
+                    // jacobian each here for edge shape fns
+                    edgeShapeFunctionSet.jacobianEach(x, [&](std::size_t beta,
+                                                              typename EdgeTestSpace::JacobianRangeType dpsi) {
+                        if (beta < edgePhiVector[0].size()) {
+                          // note: the edgeShapeFunctionSet is defined over
+                          // the reference element of the edge so the jit has
+                          // to be applied here
+                          Dune::FieldVector<double,1> gradHatPsiPhi;
+                          dpsi.mtv(phi, gradHatPsiPhi);
+                          DomainType gradPsiPhi;
+                          jit.mv(gradHatPsiPhi, gradPsiPhi);
+                          double gradPsiPhiDottau = gradPsiPhi * tau;
+                          // assert(std::abs(gradPsiDottau - dpsi[r][0] / h) < 1e-8);
+                          // GENERAL: this assumed that the Pi_0 part of Pi^e is not needed?
                           for (std::size_t s = 0; s < mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-                            for (std::size_t i = 0; i < dimDomain; ++i)
-                              for (std::size_t j = 0; j < dimDomain; ++j)
-                                P[alpha][mask[0][s]] += weight * edgePhiVector[0][beta][s] * gradPsiDottau * phi[r][i][j] * factorTN[i][j];
+                            P[alpha][mask[0][s]].axpy(edgePhiVector[0][beta][s] * gradPsiPhiDottau * weight, factorTN);
                         }
-                      }
-                  });
-                } // alpha < numHessSF
-
-                // compute the phi.n boundary terms for the hessian projection in
-                // the case that there are dofs for the normal gradient on the edge
-                // int_e Pi^1_e u m  n x n
-                if ( basisSets_.edgeSize(1) > 0 )
-                {
-                  edgeShapeFunctionSet.evaluateEach(x, [&](std::size_t beta, typename EdgeTestSpace::RangeType psi) {
-                    if (beta < edgePhiVector[1].size())
-                      // GENERAL: could use Pi_0 here as suggested in varying coeff paper
-                      //         avoid having to use the gradient projection later for the hessian projection
-                      for (std::size_t s = 0; s < mask[1].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-                        for (std::size_t r=0; r < dimRange; ++r)
-                          for (std::size_t i=0; i < dimDomain; ++i)
-                            for (std::size_t j=0; j < dimDomain; ++j)
-                              P[alpha][mask[1][s]] += weight * edgePhiVector[1][beta][s] * psi[r] * phi[r][i][j] * factorNN[i][j];
-                  });
-                } // alpha < numHessSF and can compute normal derivative
+                    });
+                  } // alpha < numHessSF
+
+                  // compute the phi.n boundary terms for the hessian projection in
+                  // the case that there are dofs for the normal gradient on the edge
+                  // CHANGE: same if as above so can be combined?
+                  if (alpha < numHessShapeFunctions && interpolation.edgeSize(1) > 0) {
+                    edgeShapeFunctionSet.evaluateEach(x, [&](std::size_t beta, typename EdgeTestSpace::RangeType psi) {
+                      if (beta < edgePhiVector[1].size())
+                        // GENERL: could use Pi_0 here as suggested in varying coeff paper
+                        //         avoid having to use the gradient projection later for the hessian projection
+                        for (std::size_t s = 0; s < mask[1].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
+                          P[alpha][mask[1][s]].axpy(edgePhiVector[1][beta][s] * psi*phi * weight, factorNN);
+                    });
+                  } // alpha < numHessSF and can compute normal derivative
               });
             } // quadrature loop
             // store the masks for each edge
           } // loop over intersections
 
           // Compute element part for the gradient projection
-          Quadrature0Type quadrature(element, 3 * polOrder);
+          Quadrature0Type quadrature(element, 2 * polOrder);
           for (std::size_t qp = 0; qp < quadrature.nop(); ++qp)
           {
             const DomainFieldType weight =
                     geometry.integrationElement(quadrature.point(qp)) * quadrature.weight(qp);
-            vemBasisFunction.evaluateAll(quadrature[qp], phi0Values);
-            shapeFunctionSet.divJacobianEach(quadrature[qp], [&](std::size_t alpha, RangeType divGradPhi)
-            {
-                assert(alpha>=0 && alpha<R.size());
-                // divGradPhi = RangeType = div( D GradSF )
-                for (std::size_t s=0; s<numDofs; ++s)
-                  R[alpha][s] -= weight * phi0Values[s] * divGradPhi;
+            // CHANGE: use correct shapefunction set - so need 'jacobinEach' as well on the gradient sfs
+            shapeFunctionSet.jacobianEach(quadrature[qp], [&](std::size_t alpha, auto gradPhi) {
+                // Note: the shapeFunctionSet is defined in physical space so
+                // the jit is not needed here
+                // R[alpha][j]  -=  Pi phi_j  grad(m_alpha) * weight
+                if (alpha < numGradShapeFunctions) {
+                  gradPhi *= -weight;
+                  vemBasisFunction.axpy(quadrature[qp], gradPhi, R[alpha]);
+                }
             });
           } // quadrature loop
         } // loop over triangles in agglomerate
 
         // now compute gradient projection by multiplying with inverse mass matrix
         for (std::size_t alpha = 0; alpha < numGradShapeFunctions; ++alpha)
           for (std::size_t i = 0; i < numDofs; ++i)
           {
             jacobianProjection[alpha][i] = 0;
             for (std::size_t beta = 0; beta < numGradShapeFunctions; ++beta)
-              jacobianProjection[alpha][i] += HpGradInv[alpha][beta] * R[beta][i];
+              jacobianProjection[alpha][i].axpy(HpGradInv[alpha][beta], R[beta][i]);
           }
 
-#if 0
-        std::cout << "*******************************\n";
-        std::cout << "****  Gradient projection  ****\n";
-        std::cout << "*******************************\n";
-        for (std::size_t beta = 0; beta < numDofs; ++beta )
-        {
-          std::cout << "phi_" << beta << " = ";
-          for (std::size_t alpha = 0; alpha < numGradShapeFunctions; ++alpha)
-          {
-            std::cout << jacobianProjection[alpha][beta] << " ";
-          }
-          std::cout << std::endl;
-        }
-        std::cout << "*******************************\n";
-#endif
-
         /////////////////////////////////////////////////////////////////////
         // HessianProjection ////////////////////////////////////////////////
         /////////////////////////////////////////////////////////////////////
 
         // iterate over the triangles of this polygon (for Hessian projection)
         for (const ElementSeedType &entitySeed : entitySeeds[agglomerate])
         {
           const ElementType &element = gridPart().entity(entitySeed);
           const auto geometry = element.geometry();
 
           // get the bounding box monomials and apply all dofs to them
-          auto shapeFunctionSet = basisSets_.basisFunctionSet(agglomeration(), element);
+          typename Traits::BBBasisFunctionSetType shapeFunctionSet
+                  = testBasisSets_.bbBasisFunctionSet(agglomeration(), element);
           auto vemBasisFunction = scalarBasisFunctionSet(element);
-#if 0 // TODO needed to provide hessians for H^1 spaces
+
           // compute the phi.n boundary terms for the hessian projection in
           // the case that there are no dofs for the normal gradient on the edge
-          if ( basisSets_.edgeSize(1) == 0 )
+          if (interpolation.edgeSize(1) == 0)
           {
             // GENERAL: more efficient to avoid this by using
             //          parital_n Pi^0 and compute that in the above intersection loop?
             //          Was this a bad idea?
             for (const auto &intersection : intersections(gridPart(), element))
             {
               // ignore edges inside the given polygon
@@ -803,59 +598,58 @@
               // now compute int_e Phi_mask[i] m_alpha
               Quadrature1Type quadrature(gridPart(), intersection, 2 * polOrder, Quadrature1Type::INSIDE);
               for (std::size_t qp = 0; qp < quadrature.nop(); ++qp)
               {
                 auto x = quadrature.localPoint(qp);
                 auto y = intersection.geometryInInside().global(x);
                 const DomainFieldType weight = intersection.geometry().integrationElement(x) * quadrature.weight(qp);
-                shapeFunctionSet.hessianEach(y, [&](std::size_t alpha, auto phi) {
-                    phi *= weight;
-                    vemBasisFunction.axpy(y, phi, normal, P[alpha]);
+                // CHANGE: need hessian sfs here - what is phi?
+                shapeFunctionSet.evaluateEach(y, [&](std::size_t alpha, auto phi) {
+                    if (alpha < numHessShapeFunctions)
+                    {
+                      phi *= weight;
+                      vemBasisFunction.axpy(y, phi, normal, P[alpha]);
+                    }
                 });
               } // quadrature loop
             } // loop over intersections
           }
-#endif
 
           // Compute element part for the hessian projection
           // GENERAL: could use the value projection here by using additional integration by parts
           //          i.e., Pi^0 D^2 m
-          Quadrature0Type quadrature(element, 3 * polOrder);
+          Quadrature0Type quadrature(element, 2 * polOrder);
           for (std::size_t qp = 0; qp < quadrature.nop(); ++qp)
           {
             const DomainFieldType weight = geometry.integrationElement(quadrature.point(qp)) * quadrature.weight(qp);
-            vemBasisFunction.jacobianAll(quadrature[qp], psi1Values);
-            shapeFunctionSet.divHessianEach(quadrature[qp],
-                          [&](std::size_t alpha, JacobianRangeType gradPhi) {
+            // CHANGE: need jacobianEach on hessian sfs
+            shapeFunctionSet.jacobianEach(quadrature[qp],
+                          [&](std::size_t alpha, auto gradPhi) {
                 // Note: the shapeFunctionSet is defined in physical space so
                 // the jit is not needed here
                 // P[alpha][j] -= Pi grad phi_j grad(m_alpha) * weight
-                // P[alpha] vector of hessians i.e. use axpy with type DynamicVector <HessianMatrixType>
-                for (std::size_t s = 0; s < numDofs; ++s)
-                  for (std::size_t d = 0; d < dimDomain; ++d)
-                    for (std::size_t r = 0; r < dimRange; ++r)
-                    {
-                      P[alpha][s] -= weight * psi1Values[s][r][d] * gradPhi[r][d];
-                    }
+                if (alpha < numHessShapeFunctions)
+                {
+                  // P[alpha] vector of hessians i.e. use axpy with type DynamicVector <HessianMatrixType>
+                  gradPhi *= -weight;
+                  vemBasisFunction.axpy(quadrature[qp], gradPhi, P[alpha]);
+                }
             });
+
           } // quadrature loop
         } // loop over triangles in agglomerate
 
         // now compute hessian projection by multiplying with inverse mass matrix
         for (std::size_t alpha = 0; alpha < numHessShapeFunctions; ++alpha)
-        {
           for (std::size_t i = 0; i < numDofs; ++i)
           {
             hessianProjection[alpha][i] = 0;
             for (std::size_t beta = 0; beta < numHessShapeFunctions; ++beta)
-              hessianProjection[alpha][i] += HpHessInv[alpha][beta] * P[beta][i];
+              hessianProjection[alpha][i].axpy(HpHessInv[alpha][beta], P[beta][i]);
           }
-        }
-
-        finalize(entitySeeds, agglomerate);
 
         /////////////////////////////////////////////////////////////////////
         // stabilization matrix /////////////////////////////////////////////
         /////////////////////////////////////////////////////////////////////
 
         Stabilization S(numDofs, numDofs, 0);
         for (std::size_t i = 0; i < numDofs; ++i)
@@ -867,25 +661,17 @@
         Stabilization &stabilization = stabilizations()[agglomerate];
         stabilization.resize(numDofs, numDofs, 0);
         for (std::size_t i = 0; i < numDofs; ++i)
           for (std::size_t j = 0; j < numDofs; ++j)
           {
             for (std::size_t k = 0; k < numDofs; ++k)
               stabilization[i][j] += S[k][i] * S[k][j];
-            maxStab = std::max(maxStab, abs(stabilization[i][j]) );
           }
-      } // end iteration over polygons
-      // std::cout << "max stabilization factor: " << maxStab << std::endl;
-    } // end build projections
 
-    // IsAgglomerationVEMSpace
-    // -----------------------
+      } // end iteration over polygonsa
 
-    template<class DiscreteFunctionSpace>
-    struct IsAgglomerationVEMSpace
-            : std::integral_constant<bool, false> {
-    };
+    } // end build projections
 
   } // namespace Vem
 } // namespace Dune
 
 #endif // #ifndef DUNE_VEM_SPACE_AGGLOMERATION_HH
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/space/divfree.hh` & `dune-vem-2.9.dev20220529/dune/vem/space/hk.hh`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#ifndef DUNE_VEM_SPACE_DIVFREE_HH
-#define DUNE_VEM_SPACE_DIVFREE_HH
+#ifndef DUNE_VEM_SPACE_HK_HH
+#define DUNE_VEM_SPACE_HK_HH
 
 #include <cassert>
 #include <utility>
 
 #include <dune/common/dynmatrix.hh>
 #include <dune/geometry/referenceelements.hh>
 #include <dune/fem/quadrature/elementquadrature.hh>
@@ -14,788 +14,898 @@
 #include <dune/fem/space/shapefunctionset/orthonormal.hh>
 #include <dune/fem/function/localfunction/converter.hh>
 #include <dune/fem/space/combinedspace/interpolation.hh>
 #include <dune/vem/misc/compatibility.hh>
 
 #include <dune/vem/agglomeration/basisfunctionset.hh>
 #include <dune/vem/misc/vector.hh>
-#include <dune/vem/space/interpolation.hh>
 #include <dune/vem/space/default.hh>
 
 namespace Dune
 {
   namespace Vem
   {
     // Internal Forward Declarations
     // -----------------------------
 
-    template<class GridPart>
-    struct DivFreeVEMSpace;
+    template<class FunctionSpace, class GridPart, bool vectorSpace = false>
+    class AgglomerationVEMSpace;
+    template< class Traits >
+    class AgglomerationVEMInterpolation;
+
+    // IsAgglomerationVEMSpace
+    // -----------------------
+
+    template<class DiscreteFunctionSpace>
+    struct IsAgglomerationVEMSpace
+            : std::integral_constant<bool, false> {
+    };
 
-    template<class GridPart>
-    struct IsAgglomerationVEMSpace<DivFreeVEMSpace<GridPart> >
+    template<class FunctionSpace, class GridPart, bool vectorSpace>
+    struct IsAgglomerationVEMSpace<AgglomerationVEMSpace<FunctionSpace, GridPart,vectorSpace> >
             : std::integral_constant<bool, true> {
     };
 
-    // DivFreeVEMSpaceTraits
+    // AgglomerationVEMSpaceTraits
     // ---------------------------
 
-    template<class FunctionSpace, class GridPart, bool reduced=true>
-    struct DivFreeVEMBasisSets
+    template<class FunctionSpace, class GridPart, bool vectorspace>
+    struct AgglomerationVEMSpaceTraits
     {
+      static const bool vectorSpace = vectorspace;
+      friend class AgglomerationVEMSpace<FunctionSpace, GridPart, vectorSpace>;
+
+      typedef AgglomerationVEMSpace<FunctionSpace, GridPart, vectorSpace> DiscreteFunctionSpaceType;
+
       typedef GridPart GridPartType;
-      static constexpr bool vectorSpace = true;
-      static constexpr int dimDomain = GridPartType::dimension;
-      static constexpr bool valReduced = false;  // true: only project values into k-1 polynomials
-      static constexpr bool jacReduced = false;  // true: only use grad phi_ for gradient basisfunctions
-      typedef typename GridPart::template Codim<0>::EntityType EntityType;
-      typedef typename GridPart::IntersectionType IntersectionType;
+
+      static const int dimension = GridPartType::dimension;
+      static const int codimension = 0;
+      static const int dimDomain = FunctionSpace::DomainType::dimension;
+      static const int dimRange = FunctionSpace::RangeType::dimension;
+      static const int baseRangeDimension = vectorSpace ? dimRange : 1;
+
+      typedef typename GridPartType::template Codim<codimension>::EntityType EntityType;
+      typedef FunctionSpace FunctionSpaceType;
 
       // a scalar function space
       typedef Dune::Fem::FunctionSpace<
               typename FunctionSpace::DomainFieldType, typename FunctionSpace::RangeFieldType,
-              dimDomain, 1 > ScalarFunctionSpaceType;
+              GridPartType::dimension, 1 > ScalarFunctionSpaceType;
 
       // scalar BB basis
-      typedef Dune::Fem::OrthonormalShapeFunctionSet< ScalarFunctionSpaceType > ONBShapeFunctionSetType;
-      typedef BoundingBoxBasisFunctionSet< GridPartType, ONBShapeFunctionSetType > ScalarBBBasisFunctionSetType;
+      typedef Dune::Fem::OrthonormalShapeFunctionSet< ScalarFunctionSpaceType > ScalarShapeFunctionSetType;
+      typedef BoundingBoxBasisFunctionSet< GridPartType, ScalarShapeFunctionSetType > ScalarBBBasisFunctionSetType;
 
       // vector version of the BB basis for use with vector spaces
       typedef std::conditional_t< vectorSpace,
-              Fem::VectorialShapeFunctionSet<ScalarBBBasisFunctionSetType, typename FunctionSpace::RangeType>,
+              Fem::VectorialShapeFunctionSet< ScalarBBBasisFunctionSetType,typename FunctionSpace::RangeType>,
+              // Fem::VectorialShapeFunctionSet< ScalarBBBasisFunctionSetType,typename ScalarFunctionSpaceType::RangeType>
               ScalarBBBasisFunctionSetType
               > BBBasisFunctionSetType;
 
+      // vem basis function sets
+      typedef VEMBasisFunctionSet <EntityType, BBBasisFunctionSetType> ScalarBasisFunctionSetType;
+      typedef std::conditional_t< vectorSpace,
+              ScalarBasisFunctionSetType,
+              Fem::VectorialBasisFunctionSet<ScalarBasisFunctionSetType, typename FunctionSpaceType::RangeType>
+              > BasisFunctionSetType;
+
       // Next we define test function space for the edges
       typedef Dune::Fem::FunctionSpace<double,double,GridPartType::dimensionworld-1,1> EdgeFSType;
       typedef Dune::Fem::OrthonormalShapeFunctionSet<EdgeFSType> ScalarEdgeShapeFunctionSetType;
+      typedef Fem::VectorialShapeFunctionSet< ScalarEdgeShapeFunctionSetType,
+              typename BBBasisFunctionSetType::RangeType> EdgeShapeFunctionSetType;
 
-    private:
-      struct ShapeFunctionSet
+      // types for the mapper
+      typedef Hybrid::IndexRange<int, FunctionSpaceType::dimRange> LocalBlockIndices;
+      typedef VemAgglomerationIndexSet <GridPartType> IndexSetType;
+      typedef AgglomerationDofMapper <GridPartType, IndexSetType> BlockMapperType;
+
+      template<class DiscreteFunction, class Operation = Fem::DFCommunicationOperation::Copy>
+      struct CommDataHandle {
+          typedef Operation OperationType;
+          typedef Fem::DefaultCommunicationHandler <DiscreteFunction, Operation> Type;
+      };
+
+      template <class T>
+      using InterpolationType = AgglomerationVEMInterpolation<T>;
+    };
+
+    // AgglomerationVEMSpace
+    // ---------------------
+    template<class FunctionSpace, class GridPart, bool vectorSpace>
+    struct AgglomerationVEMSpace
+    : public DefaultAgglomerationVEMSpace< AgglomerationVEMSpaceTraits<FunctionSpace,GridPart,vectorSpace> >
+    {
+      typedef DefaultAgglomerationVEMSpace< AgglomerationVEMSpaceTraits<FunctionSpace,GridPart,vectorSpace> > BaseType;
+      using BaseType::BaseType;
+    };
+
+    //////////////////////////////////////////////////////////////////////////////
+    // Interpolation classes
+    //////////////////////////////////////////////////////////////////////////////
+
+    template <class Traits>
+    struct AgglomerationVEMTestBasisSets
+    {
+      AgglomerationVEMTestBasisSets( const unsigned int order0, const unsigned int order1, bool useOnb)
+      : scalarSFS_(Dune::GeometryType(Dune::GeometryType::cube, Traits::dimension), order0)
+      , edgeSFS_( Dune::GeometryType(Dune::GeometryType::cube,Traits::dimension-1), order1 )
+      , useOnb_(useOnb)
+      {}
+      template <class Agglomeration>
+      const typename Traits::BBBasisFunctionSetType bbBasisFunctionSet(
+             const Agglomeration &agglomeration, const typename Traits::EntityType &entity) const
+      {
+        const std::size_t agglomerate = agglomeration.index(entity);
+        return typename Traits::BBBasisFunctionSetType( entity, agglomerate, agglomeration.boundingBoxes(), useOnb_, scalarSFS_);
+      }
+      template <class Agglomeration>
+      const typename Traits::EdgeShapeFunctionSetType &edgeBasisFunctionSet(
+             const Agglomeration &agglomeration, const typename Traits::EntityType &entity) const
+      {
+        return edgeSFS_;
+      }
+      std::size_t size() const
+      {
+        // note: scalarSFS has dimension=1 in all cases since the vector space is defined over the element
+        return scalarSFS_.size()*Traits::baseRangeDimension;
+      }
+      std::size_t edgeSize() const
       {
-        typedef typename ScalarFunctionSpaceType::RangeType ScalarRangeType;
-        typedef typename ScalarFunctionSpaceType::JacobianRangeType ScalarJacobianRangeType;
-        typedef typename ScalarFunctionSpaceType::HessianRangeType ScalarHessianRangeType;
-
-        typedef typename BBBasisFunctionSetType::FunctionSpaceType FunctionSpaceType;
-        typedef typename FunctionSpaceType::RangeType RangeType;
-        typedef typename FunctionSpaceType::JacobianRangeType JacobianRangeType;
-        typedef typename FunctionSpaceType::HessianRangeType HessianRangeType;
-        static const int dimDomain = FunctionSpaceType::DomainType::dimension;
-        static const int dimRange = RangeType::dimension;
-
-        ShapeFunctionSet() = default;
-        template <class Agglomeration>
-        ShapeFunctionSet(bool useOnb, const ONBShapeFunctionSetType& onbSFS,
-                         std::size_t numValueSF, std::size_t numGradSF, std::size_t numHessSF,
-                         std::size_t numInnerSF, std::size_t numOrthoSF,
-                         const Agglomeration &agglomeration, const EntityType &entity)
-        : vsfs_(entity, agglomeration.index(entity),
-                agglomeration.boundingBoxes(), useOnb, onbSFS)
-        , sfs_(entity, agglomeration.index(entity),
-               agglomeration.boundingBoxes(), useOnb, onbSFS)
-        , entity_(entity)
-        , scale_( 1 ) // std::sqrt( sfs_.bbox().volume() ) )
-        , numValueShapeFunctions_(numValueSF)
-        , numGradShapeFunctions_(numGradSF)
-        , numHessShapeFunctions_(numHessSF)
-        , numInnerShapeFunctions_(numInnerSF)
-        , numOrthoShapeFunctions_(numOrthoSF)
-        {}
+        // the edge sfs already has baseRangeDimension since it can be defined over the reference edge
+        return edgeSFS_.size();
+      }
+      private:
+      // note: the actual shape function set depends on the entity so
+      // we can only construct the underlying monomial basis in the ctor
+      typename Traits::ScalarShapeFunctionSetType scalarSFS_;
+      typename Traits::EdgeShapeFunctionSetType edgeSFS_;
+      bool useOnb_;
+    };
 
-        int order () const { return sfs_.order()-1;  }
+    // AgglomerationVEMInterpolation
+    // -----------------------------
+    /* Methods:
+      // interpolation of a local function
+      template< class LocalFunction, class LocalDofVector >
+      void operator() ( const ElementType &element, const LocalFunction &localFunction,
+                        LocalDofVector &localDofVector ) const
+      // set mask for active (and type of) dofs - needed for DirichletConstraints
+      // Note: this is based on the block dof mapper approach, i.e., one
+      //       entry in the mask per block
+      void operator() ( const ElementType &element, Std::vector<char> &mask) const
+
+      // apply all dofs to a basis function set (A=L(B))
+      template< class BasisFunctionSet, class LocalDofMatrix >
+      void interpolateBasis ( const ElementType &element,
+                   const BasisFunctionSet &basisFunctionSet, LocalDofMatrix &localDofMatrix ) const
+      // setup constraints rhs for value projection CLS problem
+      template <class DomainFieldType>
+      void valueL2constraints(unsigned int beta, double volume,
+                              Dune::DynamicMatrix<DomainFieldType> &D,
+                              Dune::DynamicVector<DomainFieldType> &d)
+      // interpolate given shape function set on intersection (needed for gradient projection)
+      // Note: this fills in the full mask and localDofs, i.e., not only for each block
+      template< class EdgeShapeFunctionSet >
+      void operator() (const IntersectionType &intersection,
+                       const EdgeShapeFunctionSet &edgeShapeFunctionSet, Std::vector < Dune::DynamicMatrix<double> > &localDofVectorMatrix,
+                       Std::vector<Std::vector<unsigned int>> &mask) const
+      // size of the edgePhiVector
+      std::size_t edgeSize(int deriv) const
+    */
 
-        const auto &valueBasisSet() const
-        {
-          return *this;
+    template< class Traits >
+    class AgglomerationVEMInterpolation
+    {
+      typedef AgglomerationVEMInterpolation< Traits > ThisType;
+
+    public:
+      typedef typename Traits::IndexSetType IndexSetType;
+      typedef typename IndexSetType::ElementType ElementType;
+      typedef typename IndexSetType::GridPartType GridPartType;
+      typedef typename GridPartType::IntersectionType IntersectionType;
+      typedef AgglomerationVEMTestBasisSets<Traits> TestBasisSetsType;
+
+      static const int dimension = IndexSetType::dimension;
+      static const int baseRangeDimension = Traits::baseRangeDimension;
+    private:
+      typedef Dune::Fem::ElementQuadrature<GridPartType,0> InnerQuadratureType;
+      typedef Dune::Fem::ElementQuadrature<GridPartType,1> EdgeQuadratureType;
+
+      typedef typename ElementType::Geometry::ctype ctype;
+      typedef typename Traits::BBBasisFunctionSetType InnerShapeFunctionSet;
+
+    public:
+      explicit AgglomerationVEMInterpolation ( const IndexSetType &indexSet, unsigned int polOrder, bool useOnb ) noexcept
+        : indexSet_( indexSet )
+        , testBasisSets_( std::max(indexSet_.maxDegreePerCodim()[2],0),
+                          std::max(indexSet_.maxDegreePerCodim()[1],0),
+                          useOnb )
+        , polOrder_( polOrder )
+        , useOnb_(useOnb)
+      {}
+
+      const GridPartType &gridPart() const { return indexSet_.agglomeration().gridPart(); }
+
+      template< class LocalFunction, class LocalDofVector >
+      void operator() ( const ElementType &element, const LocalFunction &localFunction,
+                        LocalDofVector &localDofVector ) const
+      {
+        // the interpolate__ method handles the 'vector valued' case
+        // calling the interpolate_ method for each component - the actual
+        // work is done in the interpolate_ method
+        interpolate__(element,localFunction,localDofVector, Dune::PriorityTag<LocalFunction::RangeType::dimension>() );
+      }
+
+      // setup right hand side constraints vector for valueProjection CLS
+      // beta: current basis function phi_beta for which to setup CLS
+      // volune: volume of current polygon
+      // D:    Lambda(B) matrix (numDofs x numShapeFunctions)
+      // d:    right hand side vector (numInnerShapeFunctions)
+      template <class DomainFieldType>
+      void valueL2constraints(unsigned int beta, double volume,
+                              Dune::DynamicMatrix<DomainFieldType> &D,
+                              Dune::DynamicVector<DomainFieldType> &d)
+      {
+        unsigned int numInnerShapeFunctions = d.size();
+        if (numInnerShapeFunctions == 0) return;
+        unsigned int numDofs = D.rows();
+        assert( numInnerShapeFunctions == testBasisSets_.size() );
+        for (int alpha=0; alpha<numInnerShapeFunctions; ++alpha)
+        {
+          // d[alpha] = e_gamma * D_beta
+          // with gamma = beta + numInnerShapeFunctions - numDofs
+          if( beta - numDofs + numInnerShapeFunctions == alpha )
+            d[ alpha ] = D[beta][alpha] * volume;
+          else
+            d[ alpha ] = 0;
         }
+      }
 
-        template< class Point, class Functor >
-        void scalarEach ( const Point &x, Functor functor ) const
+      // fill a mask vector providing the information which dofs are
+      // 'active' on the given element, i.e., are attached to a given
+      // subentity of this element. Needed for dirichlet boundary data for
+      // example
+      // Note: this returns the same mask independent of the baseRangeDimension,
+      //       i.e., vector extension has to be done on the calling side
+      void operator() ( const ElementType &element, Std::vector<char> &mask) const
+      {
+        std::fill(mask.begin(),mask.end(),-1);
+        auto vertex = [&] (int poly,auto i,int k,int numDofs)
         {
-          sfs_.evaluateEach(x, [&](std::size_t alpha, ScalarRangeType phi)
+          k /= baseRangeDimension;
+          mask[k] = 1;
+          ++k;
+          if (order2size<0>(1)>0)
           {
-            // TODO check what condition on alpha needed here
-            // scalarEach used in RHS constraints set up
-            if (alpha>=1)
-            {
-              phi[0] *= scale_;
-              functor(alpha-1, phi[0]);
-            }
-          });
-        }
-        /*
-             ortho   1     x    y        scalar   x     y    xy    x^2   y^2
-        k=2                                      (1)   (0)
-                                                 (0)   (1)
-        k=3         (-y)                         (1)   (0)   (y)   (2x)  (0)
-                    ( x)                         (0)   (1)   (x)   (0)   (2y)
-        */
-        template< class Point, class Functor >
-        void evaluateEach ( const Point &x, Functor functor ) const
-        {
-          // Note: basis functions that are included in the constraint have
-          // to be evaluated first and unconstraint basis functions have to
-          // be together at the end.
-          // To achieve this the 'ortho' part of the basis set is split
-          // with the 'alpha' for the 'inner' once being 0,..,numInner-1
-          // and the additional 'ortho' basisfunctions getting 'alpha'
-          // values so that a gap is left for the 'grad' basisfunctions.
-          int test = 0;
-          RangeType y = sfs_.position( x );
-          sfs_.bbox().gradientTransform(y, true);
-          y *= std::sqrt( sfs_.bbox().volume() );
-          assert( y.two_norm() < 1.5 );
-          sfs_.evaluateEach(x, [&](std::size_t alpha, ScalarRangeType phi)
+              mask[k]   = 2;
+              mask[k+1] = 2;
+          }
+        };
+        auto edge = [&] (int poly,auto i,int k,int numDofs)
+        {
+          k /= baseRangeDimension;
+#ifndef NDEBUG
+          auto kStart = k;
+#endif
+          for (std::size_t alpha=0;alpha<testBasisSets_.edgeSize()/baseRangeDimension;++alpha)
           {
-            if (alpha < numOrthoShapeFunctions_)
+            if (alpha < indexSet_.template order2size<1>(0))
             {
-              //// (-y,x) * phi(x,y)
-              RangeType val{-y[1]*phi[0], y[0]*phi[0]};
-              if (alpha<numInnerShapeFunctions_)
-                functor(alpha,val);
-              else
-                functor(alpha+sfs_.size()-1,val);
-              ++test;
+              mask[k] = 1;
+              ++k;
             }
-          });
-          sfs_.jacobianEach(x, [&](std::size_t alpha, ScalarJacobianRangeType dphi)
-          {
-            if (alpha>=1)
+            if (alpha < indexSet_.template order2size<1>(1))
             {
-              dphi[0] *= scale_;
-              functor(alpha-1+numInnerShapeFunctions_, dphi[0]);
-              ++test;
+              mask[k] = 2;
+              ++k;
             }
-          });
-          if (test != numValueShapeFunctions_)
-            std::cout << "evaluated " << test << " basis functions instead of " << numValueShapeFunctions_ << std::endl;
-          assert(test == numValueShapeFunctions_);
-        }
-
-        template< class Point, class Functor >
-        void jacobianEach ( const Point &x, Functor functor ) const
+          }
+          // assert(k-kStart == numDofs/baseRangeDimension);
+        };
+        auto inner = [&mask] (int poly,auto i,int k,int numDofs)
         {
-          if constexpr (!jacReduced)
-          {
-            JacobianRangeType jac(0);
-            sfs_.evaluateEach(x, [&](std::size_t alpha, ScalarRangeType phi)
-            {
-              if (alpha*dimDomain*dimDomain < numGradShapeFunctions_)
+          // assert( innerShapeFunctionSet.size() == numDofs );
+          k /= baseRangeDimension;
+          std::fill(mask.begin()+k,mask.begin()+k+numDofs/baseRangeDimension,1);
+        };
+        apply(element,vertex,edge,inner);
+        // assert( std::none_of(mask.begin(),mask.end(), [](char m){return // m==-1;}) ); // ???? needs investigation - issue with DirichletBCs
+      }
+
+      // preform interpolation of a full shape function set filling a transformation matrix
+      template< class BasisFunctionSet, class LocalDofMatrix >
+      void interpolateBasis ( const ElementType &element,
+                   const BasisFunctionSet &basisFunctionSet, LocalDofMatrix &localDofMatrix ) const
+      {
+        const auto &refElement = ReferenceElements< ctype, dimension >::general( element.type() );
+
+        // use the bb set for this polygon for the inner testing space
+        const auto &innerShapeFunctionSet = testBasisSets_.bbBasisFunctionSet( indexSet_.agglomeration(), element );
+        const auto &edgeBFS = testBasisSets_.edgeBasisFunctionSet( indexSet_.agglomeration(), element );
+
+        // define the corresponding vertex,edge, and inner parts of the interpolation
+        auto vertex = [&] (int poly,int i,int k,int numDofs)
+        { //!TS add derivatives at vertex for conforming space
+          const auto &x = refElement.position( i, dimension );
+          basisFunctionSet.evaluateEach( x, [ &localDofMatrix, k ] ( std::size_t alpha, typename BasisFunctionSet::RangeType phi ) {
+              assert( phi.dimension == baseRangeDimension );
+              if (alpha < localDofMatrix[k].size())
+                for (int r=0;r<phi.dimension;++r)
+                  localDofMatrix[ k+r ][ alpha ] = phi[ r ];
+            } );
+          k += baseRangeDimension;
+          if (order2size<0>(1)>0)
+            basisFunctionSet.jacobianEach( x, [ & ] ( std::size_t alpha, typename BasisFunctionSet::JacobianRangeType dphi ) {
+              assert( dphi[0].dimension == 2 );
+              if (alpha < localDofMatrix[k+1].size())
               {
-                for (size_t d1=0;d1<dimDomain;++d1)
+                for (int r=0;r<dphi.rows;++r)
                 {
-                  for (size_t d2=0;d2<dimDomain;++d2)
-                  {
-                    jac[d1][d2] = phi[0];
-                    functor(alpha*dimDomain*dimDomain+d1*dimDomain+d2, jac);
-                    jac[d1][d2] = 0;
-                  }
+                  localDofMatrix[ k+2*r ][ alpha ]   = dphi[r][ 0 ] * indexSet_.vertexDiameter(element, i);
+                  localDofMatrix[ k+2*r+1 ][ alpha ] = dphi[r][ 1 ] * indexSet_.vertexDiameter(element, i);
                 }
               }
-            });
-          }
-          else
-          {
-            vsfs_.jacobianEach(x, [&](std::size_t alpha, JacobianRangeType dphi)
-            {
-              if (alpha>=dimRange) functor(alpha-dimRange,dphi);
-            });
+            } );
+        };
+        auto edge = [&,this] (int poly,auto intersection,int k,int numDofs)
+        { //!TS add nomral derivatives
+          int kStart = k;
+          // int edgeNumber = intersection.indexInInside();
+          EdgeQuadratureType edgeQuad( gridPart(), intersection, 2*polOrder_, EdgeQuadratureType::INSIDE );
+          auto normal = intersection.centerUnitOuterNormal();
+          if (intersection.neighbor()) // we need to check the orientation of the normal
+            if (indexSet_.index(intersection.inside()) > indexSet_.index(intersection.outside()))
+              normal *= -1;
+          for (unsigned int qp=0;qp<edgeQuad.nop();++qp)
+          {
+            k = kStart;
+            auto x = edgeQuad.localPoint(qp);
+            auto y = intersection.geometryInInside().global(x);
+            double weight = edgeQuad.weight(qp) * intersection.geometry().integrationElement(x);
+            edgeBFS.evaluateEach(x,
+                [&](std::size_t alpha, typename BasisFunctionSet::RangeType phi ) {
+                if (alpha < order2size<1>(0))
+                {
+                  basisFunctionSet.evaluateEach( y,
+                    [ & ] ( std::size_t beta, typename BasisFunctionSet::RangeType value )
+                    {
+                      assert(k<localDofMatrix.size());
+                      localDofMatrix[ k ][ beta ] += value*phi * weight
+                                                     / intersection.geometry().volume();
+                    }
+                  );
+                  ++k;
+                }
+                if (alpha < order2size<1>(1))
+                {
+                  basisFunctionSet.jacobianEach( y,
+                    [ & ] ( std::size_t beta, typename BasisFunctionSet::JacobianRangeType dvalue )
+                    {
+                      // we assume here that jacobianEach is in global
+                      // space so the jit is not applied
+                      assert(k<localDofMatrix.size());
+                      typename BasisFunctionSet::RangeType dn;
+                      dvalue.mv(normal, dn);
+                      assert( dn[0] == dvalue[0]*normal );
+
+                      localDofMatrix[ k ][ beta ] += dn*phi * weight;
+                    }
+                  );
+                  ++k;
+                }
+              }
+            );
           }
-        }
-
-        template< class Point, class Functor >
-        void hessianEach ( const Point &x, Functor functor ) const
-        {}
-        // functor(alpha, psi) with psi in R^r
-        //
-        // for each g = g_{alpha*D+s*D+t} = m_alpha e_s e_t           (1<=alpha<=numGradSF and 1<=s,t<=dimDomain)
-        // sum_{ij} int_E d_j v_i g_ij = - sum_{ij} int_E v_i d_j g_ij + ...
-        //     = - int_E sum_i ( v_i sum_j d_j g_ij )
-        //     = - int_E v . psi
-        // with psi=(psi_i) and psi_i = sum_j d_j g_ij
-        //
-        // g_{ij} = m_a delta_{js} delta_{it}   (m=m_alpha and fixed s=1,..,dimDomain)
-        // psi_i = sum_j d_j g_ij = sum_j d_j m_a delta_{js} delta_{it}
-        //                        = d_s m_a delta_t
-        template< class Point, class Functor >
-        void divJacobianEach( const Point &x, Functor functor ) const
+        };
+        auto inner = [&] (int poly,int i,int k,int numDofs)
         {
-          RangeType divGrad(0);
-          if constexpr (!jacReduced)
-          {
-            sfs_.jacobianEach(x, [&](std::size_t alpha, ScalarJacobianRangeType dphi)
-            {
-              if (alpha*dimDomain*dimDomain < numGradShapeFunctions_)
+          assert(numDofs == innerShapeFunctionSet.size());
+          InnerQuadratureType innerQuad( element, 2*polOrder_ );
+          for (int qp=0;qp<innerQuad.nop();++qp)
+          {
+            auto y = innerQuad.point(qp);
+            double weight = innerQuad.weight(qp) * element.geometry().integrationElement(y) / indexSet_.volume(poly);
+            basisFunctionSet.evaluateEach( innerQuad[qp],
+              [ & ] ( std::size_t beta, typename BasisFunctionSet::RangeType value )
               {
-                for (size_t d1=0;d1<dimDomain;++d1)
-                {
-                  for (size_t d2=0;d2<dimDomain;++d2)
-                  {
-                    divGrad[d1] = dphi[0][d2];
-                    functor(alpha*dimDomain*dimDomain+d1*dimDomain+d2, divGrad);
-                    divGrad[d1] = 0;
+                innerShapeFunctionSet.evaluateEach( innerQuad[qp],
+                  [&](std::size_t alpha, typename InnerShapeFunctionSet::RangeType phi ) {
+                    int kk = alpha+k;
+                    assert(kk<localDofMatrix.size());
+                    localDofMatrix[ kk ][ beta ] += value*phi * weight;
                   }
-                }
+                );
               }
-            });
+            );
           }
-          else
+        };
+        apply(element,vertex,edge,inner);
+      }
+
+      // interpolate the full shape function set on intersection needed for
+      // the gradient projection matrix
+      // Note: for a vector valued space this fills in the full 'baseRangeDimension' mask and localDofs
+      template< class EdgeShapeFunctionSet >
+      void operator() (const IntersectionType &intersection,
+                       const EdgeShapeFunctionSet &edgeShapeFunctionSet, Std::vector < Dune::DynamicMatrix<double> > &localDofVectorMatrix,
+                       Std::vector<Std::vector<unsigned int>> &mask) const
+      {
+        for (std::size_t i=0;i<mask.size();++i)
+          mask[i].clear();
+        const ElementType &element = intersection.inside();
+        const auto &edgeBFS = testBasisSets_.edgeBasisFunctionSet( indexSet_.agglomeration(), element );
+        const auto &refElement = ReferenceElements< ctype, dimension >::general( element.type() );
+        int edgeNumber = intersection.indexInInside();
+        const auto &edgeGeo = refElement.template geometry<1>(edgeNumber);
+        /**/ // Question: is it correct that the nomral and derivatives are not needed here
+        auto normal = intersection.centerUnitOuterNormal();
+        double flipNormal = 1.;
+        if (intersection.neighbor()) // we need to check the orientation of the normal
+          if (indexSet_.index(intersection.inside()) > indexSet_.index(intersection.outside()))
           {
-            vsfs_.hessianEach(x, [&](std::size_t alpha, HessianRangeType d2phi)
+            normal *= -1;
+            flipNormal = -1;
+          }
+
+        /**/
+        Std::vector<std::size_t> entry(localDofVectorMatrix.size(), 0);
+
+        // define the three relevant part of the interpolation, i.e.,
+        // vertices,edges - no inner needed since only doing interpolation
+        // on intersectionn
+        auto vertex = [&] (int poly,int i,int k,int numDofs)
+        { //!TS add derivatives at vertex (probably only normal component - is the mask then correct?)
+          const auto &x = edgeGeo.local( refElement.position( i, dimension ) );
+          edgeShapeFunctionSet.evaluateEach( x, [ &localDofVectorMatrix, &entry ] ( std::size_t alpha, typename EdgeShapeFunctionSet::RangeType phi ) {
+              assert( phi.dimension == baseRangeDimension );
+              assert( entry[0] < localDofVectorMatrix[0].size() );
+              if (alpha < localDofVectorMatrix[0][ entry[0] ].size())
+                for (int r=0;r<phi.dimension;++r)
+                  localDofVectorMatrix[0][ entry[0]+r ][ alpha ] = phi[ r ];
+            } );
+          entry[0] += baseRangeDimension;
+          if (order2size<0>(1)>0)
+          {
+            edgeShapeFunctionSet.jacobianEach( x, [ & ] ( std::size_t alpha, typename EdgeShapeFunctionSet::JacobianRangeType dphi ) {
+              assert( entry[0] < localDofVectorMatrix[0].size() );
+              assert( dphi[0].dimension == 1 );
+              // note: edge sfs in reference coordinate so apply scaling 1/|S|
+              if (alpha < localDofVectorMatrix[0][entry[0]].size())
+                for (int r=0;r<dphi.rows;++r)
+                  localDofVectorMatrix[ 0 ][ entry[0]+r ][ alpha ] = dphi[r][0] / intersection.geometry().volume()
+                                                                   * indexSet_.vertexDiameter(element, i);
+            } );
+            edgeShapeFunctionSet.evaluateEach( x, [ & ] ( std::size_t alpha, typename EdgeShapeFunctionSet::RangeType phi ) {
+              assert( entry[1] < localDofVectorMatrix[1].size() );
+              if (alpha < localDofVectorMatrix[1][entry[1]].size())
+                for (int r=0;r<phi.dimension;++r)
+                  localDofVectorMatrix[ 1 ][ entry[1]+r ][ alpha ] = phi[r]*flipNormal
+                                                                 * indexSet_.vertexDiameter(element, i);
+            } );
+            entry[0] += baseRangeDimension;
+            entry[1] += baseRangeDimension;
+          }
+        };
+        auto edge = [&] (int poly,auto intersection,int k,int numDofs)
+        { //!TS add normal derivatives
+          EdgeQuadratureType edgeQuad( gridPart(),
+                intersection, 2*polOrder_, EdgeQuadratureType::INSIDE );
+          for (unsigned int qp=0;qp<edgeQuad.nop();++qp)
+          {
+            auto x = edgeQuad.localPoint(qp);
+            auto xx = x;
+            double weight = edgeQuad.weight(qp) * intersection.geometry().integrationElement(x);
+            edgeShapeFunctionSet.evaluateEach( x, [ & ] ( std::size_t beta, typename EdgeShapeFunctionSet::RangeType value ) {
+                edgeBFS.evaluateEach( xx,
+                  [&](std::size_t alpha, typename EdgeShapeFunctionSet::RangeType phi ) {
+                    //!TS add alpha<...
+                    if (alpha < order2size<1>(0) && beta < edgeSize(0))
+                    {
+                      assert( entry[0]+alpha < localDofVectorMatrix[0].size() );
+                      localDofVectorMatrix[0][ entry[0]+alpha ][ beta ] += value*phi * weight
+                                                                           / intersection.geometry().volume();
+                    }
+                    // FIX ME
+                    if (alpha < order2size<1>(1) && beta < edgeSize(1))
+                    {
+                      assert( entry[1]+alpha < localDofVectorMatrix[1].size() );
+                      localDofVectorMatrix[1][ entry[1]+alpha ][ beta ] += value*phi * weight * flipNormal;
+                    }
+                  }
+                );
+              }
+            );
+          }
+          entry[0] += order2size<1>(0);
+          entry[1] += order2size<1>(1);
+        };
+        applyOnIntersection(intersection,vertex,edge,mask);
+        assert( entry[0] == localDofVectorMatrix[0].size() );
+        assert( entry[1] == localDofVectorMatrix[1].size() );
+
+        //////////////////////////////////////////////////////////////////////////////////
+        auto tau = intersection.geometry().corner(1);
+        tau -= intersection.geometry().corner(0);
+        if (localDofVectorMatrix[0].size() > 0)
+        {
+          localDofVectorMatrix[0].invert();
+
+          if (mask[1].size() > edgeSize(1))
+          { // need to take tangential derivatives at vertices into account
+            assert(mask[0].size() == edgeSize(0)+2);
+            auto A = localDofVectorMatrix[0];
+            localDofVectorMatrix[0].resize(edgeSize(0), mask[0].size(), 0);
+            // vertex basis functions (values)
+            for (std::size_t j=0;j<edgeSize(0);++j)
+            {
+              localDofVectorMatrix[0][j][0] = A[j][0];
+              localDofVectorMatrix[0][j][3] = A[j][2];
+            }
+            // vertex basis functions (tangential derivatives)
+            // TODO: add baseRangeDimension
+            for (std::size_t j=0;j<edgeSize(0);++j)
             {
-              if (alpha>=dimRange)
+              localDofVectorMatrix[0][j][1] = A[j][1]*tau[0];
+              localDofVectorMatrix[0][j][2] = A[j][1]*tau[1];
+              localDofVectorMatrix[0][j][4] = A[j][3]*tau[0];
+              localDofVectorMatrix[0][j][5] = A[j][3]*tau[1];
+            }
+            for (std::size_t i=6;i<mask[0].size();++i)
+              for (std::size_t j=0;j<edgeSize(0);++j)
               {
-                for (size_t i=0;i<divGrad.size();++i)
-                {
-                  divGrad[i] = 0;
-                  for (size_t s=0;s<dimDomain;++s)
-                    divGrad[i] += d2phi[i][s][s];
-                }
-                functor(alpha-dimRange, divGrad);
+                assert( i-2 < A[j].size() );
+                localDofVectorMatrix[0][j][i] = A[j][i-2];
               }
-            });
           }
         }
-        // functor(alpha, psi) with psi in R^{r,d}
-        //
-        // h_{alpha*D^2+d1*D+d2}
-        // for each h_r = m_{alpha,r} S_{d1,d2}    (fixed 1<=alpha<=numHessSF and 1<=d1,d2<=dimDomain)
-        // sum_{rij} int_E d_ij v_r h_rij = - sum_{rij} int_E d_i v_r d_j h_rij + ...
-        //     = - int_E sum_ri (d_i v_r sum_j d_j h_rij )
-        //     = - int_E sum_ri d_i v_r psi_ri
-        // with psi_ri = sum_j d_j h_rij
-        //
-        // h_{rij} = m_{alpha,r} (delta_{i,d1}delta_{j,d2}+delta_{j,d1}delta_{i,d2})
-        //           (m=m_alpha and fixed ij=1,..,dimDomain)
-        // psi_ri = sum_j d_j h_rij
-        //        = sum_j d_j m_{alpha,r} (delta_{i,d1}delta_{j,d2}+delta_{j,d1}delta_{i,d2})
-        //        = (d_d2 m_{alpha,r} delta_{i,d1} + d_d1 m_{alpha,r} delta_{i,d2}
-        template< class Point, class Functor >
-        void divHessianEach( const Point &x, Functor functor ) const
+        if (localDofVectorMatrix[1].size() > 0)
         {
-        }
-
-        template< class Point, class Functor >
-        void evaluateTestEach ( const Point &x, Functor functor ) const
-        {
-          RangeType y = sfs_.position( x );
-          sfs_.bbox().gradientTransform(y, true);
-          y *= std::sqrt( sfs_.bbox().volume() );
-          assert( y.two_norm() < 1.5 );
-          sfs_.evaluateEach(x, [&](std::size_t alpha, ScalarRangeType phi)
+          localDofVectorMatrix[1].invert();
+          if (mask[1].size() > edgeSize(1))
           {
-            if (alpha < numInnerShapeFunctions_)
+            assert(mask[1].size() == edgeSize(1)+2);
+            auto A = localDofVectorMatrix[1];
+            localDofVectorMatrix[1].resize(edgeSize(1), mask[1].size(), 0);
+            std::size_t i=0;
+            // vertex basis functions
+            for (;i<4;i+=2)
             {
-              RangeType val{-y[1]*phi[0], y[0]*phi[0]};
-              functor(alpha, val );
+              for (std::size_t j=0;j<edgeSize(1);++j)
+              {
+                localDofVectorMatrix[1][j][i]   = A[j][i/2]*normal[0];
+                localDofVectorMatrix[1][j][i+1] = A[j][i/2]*normal[1];
+              }
             }
-          });
-        }
-
-        private:
-        BBBasisFunctionSetType vsfs_;
-        ScalarBBBasisFunctionSetType sfs_;
-        EntityType entity_;
-        double scale_;
-        std::size_t numValueShapeFunctions_;
-        std::size_t numGradShapeFunctions_;
-        std::size_t numHessShapeFunctions_;
-        std::size_t numInnerShapeFunctions_;
-        std::size_t numOrthoShapeFunctions_;
-      };
-      struct EdgeShapeFunctionSet
-      {
-        typedef typename BBBasisFunctionSetType::FunctionSpaceType FunctionSpaceType;
-        typedef typename FunctionSpaceType::DomainType DomainType;
-        typedef typename FunctionSpaceType::RangeType RangeType;
-        typedef typename FunctionSpaceType::JacobianRangeType JacobianRangeType;
-        typedef typename FunctionSpaceType::HessianRangeType HessianRangeType;
-        static const int dimDomain = DomainType::dimension;
-        static const int dimRange = RangeType::dimension;
-
-        typedef Fem::VectorialShapeFunctionSet<ScalarEdgeShapeFunctionSetType, RangeType> VectorEdgeShapeFunctionSetType;
-        typedef typename VectorEdgeShapeFunctionSetType::JacobianRangeType EdgeJacobianRangeType;
-
-        EdgeShapeFunctionSet(const IntersectionType &intersection, const ScalarEdgeShapeFunctionSetType &sfs,
-                             bool twist,
-                             unsigned int numEdgeTestFunctions)
-        : intersection_(intersection), sfs_(sfs), twist_(twist), numEdgeTestFunctions_(numEdgeTestFunctions)
-        {}
-        template< class Point, class Functor >
-        void evaluateEach ( const Point &xx, Functor functor ) const
-        {
-          auto x = Dune::Fem::coordinate(xx);
-          if (twist_) x[0] = 1.-x[0];
-          sfs_.evaluateEach(x,functor);
-        }
-        template< class Point, class Functor >
-        void jacobianEach ( const Point &xx, Functor functor ) const
-        {
-          auto x = Dune::Fem::coordinate(xx);
-          if (twist_) x[0] = 1.-x[0];
-          JacobianRangeType jac;
-          const auto &geo = intersection_.geometry();
-          const auto &jit = geo.jacobianInverseTransposed(x);
-          sfs_.jacobianEach(x, [&](std::size_t alpha, EdgeJacobianRangeType dphi)
-          {
-            if (twist_) dphi *= -1;
-            for (std::size_t r=0;r<dimRange;++r)
-              jit.mv(dphi[r],jac[r]);
-            functor(alpha,jac);
-          });
+            for (;i<mask[1].size();++i)
+              for (std::size_t j=0;j<edgeSize(1);++j)
+                localDofVectorMatrix[1][j][i] = A[j][i-2];
+          }
         }
-        template< class Point, class Functor >
-        void evaluateTestEach ( const Point &xx, Functor functor ) const
-        {
-          auto x = Dune::Fem::coordinate(xx);
-          if (twist_) x[0] = 1.-x[0];
-          sfs_.evaluateEach(x, [&](std::size_t alpha, RangeType phi)
-          {
-            if (alpha<numEdgeTestFunctions_)
-              functor(alpha,phi);
-          });
+        /* ////////////////////////////////////////////////////////////////////// */
+        // It might be necessary to flip the vertex entries in the masks around
+        // due to a twist in the intersection.
+        // At the moment this is done by checking that the
+        /* ////////////////////////////////////////////////////////////////////// */
+        {
+          auto otherTau = element.geometry().corner(
+                       refElement.subEntity(intersection.indexInInside(),1,1,2)
+                     );
+          otherTau -= element.geometry().corner(
+                        refElement.subEntity(intersection.indexInInside(),1,0,2)
+                      );
+          otherTau /= otherTau.two_norm();
+          if (indexSet_.vertexOrders()[0]>=0) // vertices might have to be flipped
+          {
+            if (otherTau*tau<0)
+            {
+              if (mask[1].size() > edgeSize(1))
+              {
+                // swap vertex values and tangential derivatives
+                for (int r=0;r<3*baseRangeDimension;++r)
+                  std::swap(mask[0][r], mask[0][3*baseRangeDimension+r]);
+                // swap normal derivatives at vertices
+                for (int r=0;r<2*baseRangeDimension;++r)
+                  std::swap(mask[1][r], mask[1][2*baseRangeDimension+r]);
+              }
+              else
+              {
+                // swap vertex values
+                for (int r=0;r<baseRangeDimension;++r)
+                  std::swap(mask[0][r], mask[0][baseRangeDimension+r]);
+              }
+            }
+          }
         }
-        private:
-        const IntersectionType &intersection_;
-        VectorEdgeShapeFunctionSetType sfs_;
-        unsigned int numEdgeTestFunctions_;
-        bool twist_;
-      };
-
-      public:
-      typedef ShapeFunctionSet ShapeFunctionSetType;
-      typedef EdgeShapeFunctionSet EdgeShapeFunctionSetType;
-
-      DivFreeVEMBasisSets( const int order, bool useOnb, bool conforming )
-      : innerOrder_( order )
-      , conforming_( conforming )
-      , onbSFS_(Dune::GeometryType(Dune::GeometryType::cube, dimDomain),
-          valReduced? order-1:order+1
-        )
-      , edgeSFS_( Dune::GeometryType(Dune::GeometryType::cube,dimDomain-1), maxEdgeDegree() )
-      , dofsPerCodim_(calcDofsPerCodim(order))
-      , useOnb_(useOnb)
-      , numValueShapeFunctions_( sizeONB<0>(onbSFS_.order()-1) )
-      , numGradShapeFunctions_ (
-              (!jacReduced)?
-              sizeONB<0>(order-1)*BBBasisFunctionSetType::RangeType::dimension:
-              (onbSFS_.size()-1)*BBBasisFunctionSetType::RangeType::dimension
-          )
-      , numHessShapeFunctions_ ( 0 )
-      , numInnerShapeFunctions_( order==2 ? 0 :
-                                 sizeONB<0>(order-3)/BBBasisFunctionSetType::RangeType::dimension )
-      , numOrthoShapeFunctions_(valReduced?
-          numInnerShapeFunctions_:
-          sizeONB<0>(order-1)/BBBasisFunctionSetType::RangeType::dimension
-        )
-      , numEdgeTestShapeFunctions_( (conforming_)? sizeONB<1>(order-2):sizeONB<1>(order-1) )
-      {
-        auto degrees = edgeDegrees();
-        /*
-        std::cout << "dofsPerCodim:" << dofsPerCodim_[0].second << " "
-                                     << dofsPerCodim_[1].second << " "
-                                     << dofsPerCodim_[2].second << std::endl;
-        std::cout << "[" << numValueShapeFunctions_ << ","
-                  << numGradShapeFunctions_ << ","
-                  << numHessShapeFunctions_ << ","
-                  << numInnerShapeFunctions_ << "]"
-                  << constraintSize() << "]"
-                  << "   edge: ["
-                  << edgeSize(0) << "," << edgeSize(1) << ","
-                  << numEdgeTestShapeFunctions_ << "]"
-                  << " " << degrees[0] << " " << degrees[1]
-                  << " max size of edge set: " << edgeSFS_.size()*2
-                  << " edgeSize(): " << edgeSize()
-                  << std::endl;
-        std::cout << "dofs per codim: "
-                  << dofsPerCodim_[0].second << " " << dofsPerCodim_[1].second << " " << dofsPerCodim_[2].second
-                  << std::endl;
-        */
       }
 
-      const std::size_t maxOrder() const
+      std::size_t edgeSize(int deriv) const
       {
-        return onbSFS_.order();
+        return indexSet_.edgeSize(deriv) * baseRangeDimension;
       }
 
-      const std::array< std::pair< int, unsigned int >, dimDomain+1 > &dofsPerCodim() const
+    private:
+      template <int dim>
+      std::size_t order2size(unsigned int deriv) const
       {
-        return dofsPerCodim_;
+        return indexSet_.template order2size<dim>(deriv) * baseRangeDimension;
       }
 
-      template <class Agglomeration>
-      ShapeFunctionSetType basisFunctionSet(
-             const Agglomeration &agglomeration, const EntityType &entity) const
-      {
-        return ShapeFunctionSet(useOnb_, onbSFS_, numValueShapeFunctions_, numGradShapeFunctions_, numHessShapeFunctions_,
-                                numInnerShapeFunctions_,numOrthoShapeFunctions_,
-                                agglomeration,entity);
-      }
-      template <class Agglomeration>
-      EdgeShapeFunctionSetType edgeBasisFunctionSet(
-             const Agglomeration &agglomeration,
-             const IntersectionType &intersection, bool twist) const
-      {
-        return EdgeShapeFunctionSetType(intersection, edgeSFS_, 0, numEdgeTestShapeFunctions_);
-      }
-      std::size_t size( std::size_t orderSFS ) const
-      {
-        {
-          if (orderSFS == 0)
-            return numValueShapeFunctions_;
-          else if (orderSFS == 1)
-            return numGradShapeFunctions_;
-          else if (orderSFS == 2)
-            return numHessShapeFunctions_;
-        }
-        assert(0);
-        return 0;
-      }
-      std::size_t constraintSize() const
-      {
-        if (conforming_)
-        {
-          return numInnerShapeFunctions_ + onbSFS_.size()-1;
+      void getSizesAndOffsets(int poly,
+                  int &vertexSize,
+                  int &edgeOffset, int &edgeSize,
+                  int &innerOffset, int &innerSize) const
+      {
+        auto dofs   = indexSet_.dofsPerCodim();  // assume always three entries in dim order (i.e. 2d)
+        assert(dofs.size()==3);
+        vertexSize  = dofs[0].second*baseRangeDimension;
+        edgeOffset  = indexSet_.subAgglomerates(poly,dimension)*vertexSize;
+        edgeSize    = dofs[1].second*baseRangeDimension;
+        innerOffset = edgeOffset + indexSet_.subAgglomerates(poly,dimension-1)*edgeSize;
+        innerSize   = dofs[2].second*baseRangeDimension;
+      }
+
+      // carry out actual interpolation giving the three components, i.e.,
+      // for the vertex, edge, and inner parts.
+      // This calls these interpolation operators with the correct indices
+      // to fill the dof vector or the matrix components
+      template< class Vertex, class Edge, class Inner>
+      void apply ( const ElementType &element,
+          const Vertex &vertex, const Edge &edge, const Inner &inner) const
+      {
+        const auto &refElement = ReferenceElements< ctype, dimension >::general( element.type() );
+        const int poly = indexSet_.index( element );
+        int vertexSize, edgeOffset,edgeSize, innerOffset,innerSize;
+        getSizesAndOffsets(poly, vertexSize,edgeOffset,edgeSize,innerOffset,innerSize);
+
+        // vertex dofs
+        //!TS needs changing
+        if (indexSet_.vertexOrders()[0] >= 0)
+        {
+          for( int i = 0; i < refElement.size( dimension ); ++i )
+          {
+            const int k = indexSet_.localIndex( element, i, dimension) * vertexSize;
+            if ( k >= 0 ) // is a 'real' vertex of the polygon
+              vertex(poly,i,k,1);
+          }
         }
-        else
-        {
-          // innerOrder_ fails (P^3 solution not exactly interpolated with innerOrder_==3
-          return numInnerShapeFunctions_ +
-                 sizeONB<0>(innerOrder_-1) / BBBasisFunctionSetType::RangeType::dimension
-                 -1;
+        //!TS needs changing
+        if (order2size<1>(0)>0 ||
+            order2size<1>(1)>0)
+        {
+          // to avoid any issue with twists we use an intersection iterator
+          // here instead of going over the edges
+          auto it = gridPart().ibegin( element );
+          const auto endit = gridPart().iend( element );
+          for( ; it != endit; ++it )
+          {
+            const auto& intersection = *it;
+            const int i = intersection.indexInInside();
+            const int k = indexSet_.localIndex( element, i, dimension-1 )*edgeSize + edgeOffset; //
+            if ( k>=edgeOffset ) // 'real' edge of polygon
+              edge(poly,intersection,k,edgeSize);
+          }
         }
-      }
-      std::size_t vertexSize(int deriv) const
-      {
-        // vertex values in div free space
-        if (conforming_)
+        //! needs changing
+        if (indexSet_.innerOrders()[0] >=0)
         {
-          if (deriv==0)
-            return pow(dimDomain,deriv);
-          else
-            return 0;
+          // inner dofs
+          const int k = indexSet_.localIndex( element, 0, 0 )*innerSize + innerOffset;
+          inner(poly,0,k,innerSize);
         }
-        else
-          return 0;
-      }
-      std::size_t innerSize() const
-      {
-        return numInnerShapeFunctions_;
-      }
-      std::size_t edgeValueMoments() const
-      {
-        // returns order of edge moments up to P_k where k is the entry in dof tuple
-        if (conforming_)
-          return innerOrder_-2;
-        else
-          return innerOrder_-1;
-          // return innerOrder_;
-      }
-      std::size_t edgeSize(int deriv) const
-      {
-        auto degrees = edgeDegrees();
-        return degrees[deriv] < 0 ? 0 : sizeONB<1>( degrees[deriv] );
       }
 
-      ////////////////////////////
-      // used in interpolation  //
-      ////////////////////////////
-      std::size_t edgeSize() const
-      {
-        return edgeSFS_.size() * BBBasisFunctionSetType::RangeType::dimension;
-      }
-      std::size_t numEdgeTestShapeFunctions() const
-      {
-        return numEdgeTestShapeFunctions_;
-      }
-      template <int dim>
-      std::size_t order2size(unsigned int deriv) const
-      {
-        if (dim == 0 && deriv == 0) // vertex size
-        {
-          if (conforming_)
-            return pow(dimDomain,deriv);
-          else
-            return 0;
-        }
-        if (dim == 1 && deriv == 0)
-        {
-          if (conforming_)
+      // perform interpolation for a single localized function, calls the
+      // 'apply' method with the correct 'vertex','edge','inner' functions
+      template< class LocalFunction, class LocalDofVector >
+      void interpolate_ ( const ElementType &element, const LocalFunction &localFunction,
+                          LocalDofVector &localDofVector ) const
+      {
+        typename LocalFunction::RangeType value;
+        typename LocalFunction::JacobianRangeType dvalue;
+        assert( value.dimension == baseRangeDimension );
+        const auto &refElement = ReferenceElements< ctype, dimension >::general( element.type() );
+
+        // use the bb set for this polygon for the inner testing space
+        const auto &innerShapeFunctionSet = testBasisSets_.bbBasisFunctionSet( indexSet_.agglomeration(), element );
+        const auto &edgeBFS = testBasisSets_.edgeBasisFunctionSet( indexSet_.agglomeration(), element );
+
+        // define the vertex,edge, and inner parts of the interpolation
+        auto vertex = [&] (int poly,auto i,int k,int numDofs)
+        { //!TS vertex derivatives
+          const auto &x = refElement.position( i, dimension );
+          localFunction.evaluate( x, value );
+          //! SubDofWrapper does not have size assert( k < localDofVector.size() );
+          for (int r=0;r<value.dimension;++r)
+            localDofVector[ k+r ] = value[ r ];
+          k += value.dimension;
+          if (order2size<0>(1)>0)
           {
-            if (innerOrder_-2<0)
-              return 0;
-            else
-              return Dune::Fem::OrthonormalShapeFunctions<1>::size(innerOrder_-2);
+            localFunction.jacobian( x, dvalue );
+            for (int r=0;r<value.dimension;++r)
+            {
+              localDofVector[ k+2*r ]   = dvalue[ r ][ 0 ] * indexSet_.vertexDiameter(element, i);
+              localDofVector[ k+2*r+1 ] = dvalue[ r ][ 1 ] * indexSet_.vertexDiameter(element, i);
+            }
           }
-          else
-          {
-            if (innerOrder_-1<0)
-              return 0;
-            else
-              return Dune::Fem::OrthonormalShapeFunctions<1>::size(innerOrder_-1);
-          /*
-            if (innerOrder_<0)
-              return 0;
-            else
-              return Dune::Fem::OrthonormalShapeFunctions<1>::size(innerOrder_);
-           */
+        };
+        auto edge = [&] (int poly,auto intersection,int k,int numDofs)
+        { //!TS edge derivatives
+          int kStart = k;
+          auto normal = intersection.centerUnitOuterNormal();
+          if (intersection.neighbor()) // we need to check the orientation of the normal
+            if (indexSet_.index(intersection.inside()) > indexSet_.index(intersection.outside()))
+              normal *= -1;
+          EdgeQuadratureType edgeQuad( gridPart(),
+                intersection, 2*polOrder_, EdgeQuadratureType::INSIDE );
+          for (unsigned int qp=0;qp<edgeQuad.nop();++qp)
+          {
+            k = kStart;
+            auto x = edgeQuad.localPoint(qp);
+            auto y = intersection.geometryInInside().global(x);
+            localFunction.evaluate( y, value );
+            double weight = edgeQuad.weight(qp) * intersection.geometry().integrationElement(x);
+            if (order2size<1>(1)>0)
+              localFunction.jacobian( y, dvalue);
+            typename LocalFunction::RangeType dnvalue;
+            dvalue.mv(normal,dnvalue);
+            assert( dnvalue[0] == dvalue[0]*normal );
+            edgeBFS.evaluateEach(x,
+              [&](std::size_t alpha, typename LocalFunction::RangeType phi ) {
+                //! SubDofWrapper has no size assert( kk < localDofVector.size() );
+                if (alpha < order2size<1>(0))
+                {
+                  //! see above assert(k < localDofVector.size() );
+                  localDofVector[ k ] += value*phi * weight
+                                         / intersection.geometry().volume();
+                  ++k;
+                }
+                if (alpha < order2size<1>(1))
+                {
+                  //! see above assert(k < localDofVector.size() );
+                  localDofVector[ k ] += dnvalue*phi * weight;
+                  ++k;
+                }
+              }
+            );
           }
-        }
-        if (dim == 2 && deriv == 0 && innerOrder_ >=3)
-          return Dune::Fem::OrthonormalShapeFunctions<2>::size(innerOrder_-3);
-        else
-          return 0;
-      }
-      int vectorDofs(int dim) const
-      {
-        // return 1 for scalar dofs (inner moments) or dimRange for vector dofs (vertex and edge)
-        // BBBasisFunctionSetType::FunctionSpaceType::RangeType::dimension = dimRange
-        if (dim == 2)
-          return 1;
-        if (dim == 0 || dim == 1)
-          return BBBasisFunctionSetType::FunctionSpaceType::RangeType::dimension;
-        else // shouldn't get here
+        };
+        auto inner = [&] (int poly,int i,int k,int numDofs)
         {
-          assert(false);
-          return -1;
-        }
+          assert(numDofs == innerShapeFunctionSet.size());
+          //! SubVector has no size: assert(k+numDofs == localDofVector.size());
+          InnerQuadratureType innerQuad( element, 2*polOrder_ );
+          for (unsigned int qp=0;qp<innerQuad.nop();++qp)
+          {
+            auto y = innerQuad.point(qp);
+            localFunction.evaluate( innerQuad[qp], value );
+            double weight = innerQuad.weight(qp) * element.geometry().integrationElement(y) / indexSet_.volume(poly);
+            innerShapeFunctionSet.evaluateEach(innerQuad[qp],
+              [&](std::size_t alpha, typename LocalFunction::RangeType phi ) {
+                int kk = alpha+k;
+                //! SubVector has no size assert( kk < localDofVector.size() );
+                localDofVector[ kk ] += value*phi * weight;
+              }
+            );
+          }
+        };
+        apply(element,vertex,edge,inner);
       }
-
-      private:
-      Std::vector<int> edgeDegrees() const
+      // these methods are simply used to handle the vector valued case,
+      // for which the interpolation needs to be applied for each component
+      // separately
+      template< class LocalFunction, class LocalDofVector >
+      void interpolate__( const ElementType &element, const LocalFunction &localFunction,
+                          LocalDofVector &localDofVector, Dune::PriorityTag<2> ) const
       {
-        Std::vector<int> degrees(2, -1);
-        if (conforming_)
+        if constexpr (Traits::vectorSpace)
         {
-          degrees[0] += 2;
-          degrees[0] += std::max(0,innerOrder_-1);
+          interpolate_(element,localFunction,localDofVector);
         }
         else
-          degrees[0] = innerOrder_-1;
-          // degrees[0] = innerOrder_;
-        return degrees;
-      }
-      std::size_t maxEdgeDegree() const
-      {
-        auto degrees = edgeDegrees();
-        return *std::max_element(degrees.begin(),degrees.end());
+        {
+          typedef Dune::Fem::VerticalDofAlignment<
+                  ElementType, typename LocalFunction::RangeType> DofAlignmentType;
+          DofAlignmentType dofAlignment(element);
+          for( std::size_t i = 0; i < LocalFunction::RangeType::dimension; ++i )
+          {
+            Fem::Impl::SubDofVectorWrapper< LocalDofVector, DofAlignmentType > subLdv( localDofVector, i, dofAlignment );
+            interpolate__(element,
+                Dune::Fem::localFunctionConverter( localFunction, Fem::Impl::RangeConverter<LocalFunction::RangeType::dimension>(i) ),
+                subLdv, PriorityTag<1>()
+                );
+          }
+        }
       }
-
-      template <int codim>
-      static std::size_t sizeONB(std::size_t order)
+      template< class LocalFunction, class LocalDofVector >
+      void interpolate__( const ElementType &element, const LocalFunction &localFunction,
+                          LocalDofVector &localDofVector, Dune::PriorityTag<1> ) const
       {
-        return Dune::Fem::OrthonormalShapeFunctions<dimDomain - codim> :: size(order) *
-               BBBasisFunctionSetType::RangeType::dimension;
+        interpolate_(element,localFunction,localDofVector);
       }
 
-      std::array< std::pair< int, unsigned int >, dimDomain+1 > calcDofsPerCodim (unsigned int order) const
+      ///////////////////////////////////////////////////////////////////////////
+      // interpolation onto a single intersection
+      // (bool argument needed to distinguish from the method following this one)
+      template< class Vertex, class Edge>
+      void applyOnIntersection( const IntersectionType &intersection,
+                                const Vertex &vertex, const Edge &edge,
+                                Std::vector<Std::vector<unsigned int>> &mask) const
       {
-        auto vSize = order2size<0>(0) * BBBasisFunctionSetType::RangeType::dimension;
-        // std::cout << "vSize: " << vSize << std::endl;
-        auto eSize = order2size<1>(0) * BBBasisFunctionSetType::RangeType::dimension;
-        // std::cout << "eSize: " << eSize << std::endl;
-        auto iSize = order2size<2>(0);
-        // std::cout << "iSize: " << iSize << std::endl;
-        return std::array< std::pair< int, unsigned int >, dimDomain+1 >
-               { std::make_pair( dimDomain,   vSize ),
-                 std::make_pair( dimDomain-1, eSize ),
-                 std::make_pair( dimDomain-2, iSize ) };
-      }
-
-      // note: the actual shape function set depends on the entity so
-      // we can only construct the underlying monomial basis in the ctor
-      const int innerOrder_;
-      const bool useOnb_;
-      const bool conforming_;
-      std::array< std::pair< int, unsigned int >, dimDomain+1 > dofsPerCodim_;
-      const ONBShapeFunctionSetType onbSFS_;
-      const ScalarEdgeShapeFunctionSetType edgeSFS_;
-      const std::size_t numValueShapeFunctions_;
-      const std::size_t numGradShapeFunctions_;
-      const std::size_t numHessShapeFunctions_;
-      const std::size_t numInnerShapeFunctions_;
-      const std::size_t numOrthoShapeFunctions_;
-      const std::size_t numEdgeTestShapeFunctions_;
-    };
-
-
-
-    template<class GridPart>
-    struct DivFreeVEMSpaceTraits
-    {
-      typedef GridPart GridPartType;
-      static const int dimension = GridPartType::dimension;
-      typedef Dune::Fem::FunctionSpace<double,double,dimension,dimension> FunctionSpaceType;
-
-      typedef DivFreeVEMBasisSets<FunctionSpaceType,GridPart> BasisSetsType;
-      friend struct DivFreeVEMSpace<GridPart>;
-      typedef DivFreeVEMSpace<GridPart> DiscreteFunctionSpaceType;
-
-      static const int codimension = 0;
-      static const int dimDomain = FunctionSpaceType::DomainType::dimension;
-      static const int dimRange = FunctionSpaceType::RangeType::dimension;
-      static const bool vectorSpace = true;
-      typedef Hybrid::IndexRange<int, 1> LocalBlockIndices;
-      // static const int baseRangeDimension = dimRange;
-
-      typedef typename GridPartType::template Codim<codimension>::EntityType EntityType;
+        const ElementType &element = intersection.inside();
+        const auto &refElement = ReferenceElements< ctype, dimension >::general( element.type() );
 
+        const int poly = indexSet_.index( element );
+        int vertexSize, edgeOffset,edgeSize, innerOffset,innerSize;
+        getSizesAndOffsets(poly, vertexSize,edgeOffset,edgeSize,innerOffset,innerSize);
 
-      // types for the mapper
-      typedef VemAgglomerationIndexSet <GridPartType> IndexSetType;
-    };
-
-    // DivFreeVEMSpace
-    // ---------------------
-    template<class GridPart>
-    struct DivFreeVEMSpace : public DefaultAgglomerationVEMSpace<
-          AgglomerationVEMSpaceTraits<DivFreeVEMSpaceTraits<GridPart>> >
-    {
-      typedef AgglomerationVEMSpaceTraits<DivFreeVEMSpaceTraits<GridPart>> TraitsType;
-      typedef DefaultAgglomerationVEMSpace<TraitsType> BaseType;
-      typedef typename BaseType::AgglomerationType AgglomerationType;
-      typedef typename BaseType::BasisSetsType::ShapeFunctionSetType::FunctionSpaceType FunctionSpaceType;
-      typedef typename FunctionSpaceType::DomainFieldType DomainFieldType;
-      DivFreeVEMSpace(AgglomerationType &agglomeration,
-          const unsigned int polOrder,
-          const bool conforming,
-          int basisChoice,
-          bool edgeInterpolation)
-      : BaseType(agglomeration,polOrder,
-                 typename TraitsType::BasisSetsType(polOrder, basisChoice, conforming),
-                 basisChoice,edgeInterpolation)
-      {
-        // TODO: move this to the default and add a method to the baisisSets to
-        // obtain the required order (here polOrder+1)
-        assert( BaseType::basisSets_.maxOrder() == polOrder+1 );
-        BaseType::update(true);
-      }
-
-    protected:
-      virtual void setupConstraintRHS(const Std::vector<Std::vector<typename BaseType::ElementSeedType> > &entitySeeds, unsigned int agglomerate,
-                                    Dune::DynamicMatrix<DomainFieldType> &RHSconstraintsMatrix, double volume) override
-      {
-        //////////////////////////////////////////////////////////////////////////
-        /// Fix RHS constraints for value projection /////////////////////////////
-        //////////////////////////////////////////////////////////////////////////
-
-        typedef typename BaseType::BasisSetsType::EdgeShapeFunctionSetType EdgeTestSpace;
-        typedef typename FunctionSpaceType::DomainType DomainType;
-        typedef typename FunctionSpaceType::RangeFieldType RangeFieldType;
-        typedef typename FunctionSpaceType::RangeType RangeType;
-        typedef typename FunctionSpaceType::JacobianRangeType JacobianRangeType;
-        typedef typename FunctionSpaceType::HessianRangeType HessianRangeType;
-        const std::size_t dimDomain = DomainType::dimension;
-        const std::size_t dimRange = RangeType::dimension;
-        static constexpr int blockSize = BaseType::localBlockSize;
-        const std::size_t numDofs = BaseType::blockMapper().numDofs(agglomerate) * blockSize;
-        int polOrder = BaseType::order();
-        const std::size_t numConstraintShapeFunctions = BaseType::basisSets_.constraintSize();
-        const std::size_t numInnerShapeFunctions = BaseType::basisSets_.innerSize();
-
-        assert( numInnerShapeFunctions <= numConstraintShapeFunctions );
-        if (numConstraintShapeFunctions == 0) return;
-
-        // first fill in entries relating to inner dofs (alpha < inner shape functions)
-        for ( int beta=0; beta<numDofs; ++beta)
+        int edgeNumber = intersection.indexInInside();
+        const int k = indexSet_.localIndex( element, edgeNumber, dimension-1 );
+        assert(k>=0); // should only be called for 'outside' intersection
+        if (k>=0)  // this doesn't make sense - remove?
         {
-          for (int alpha=0; alpha<numInnerShapeFunctions; ++alpha)
+          std::size_t i = 0;
+          if (indexSet_.vertexOrders()[0]>=0) //!TS
           {
-            if( beta - numDofs + numInnerShapeFunctions == alpha )
-              RHSconstraintsMatrix[ beta ][ alpha ] = volume;
-          }
-        }
-
-        /*
-          q in P_{k-1}\R
-          int_E v grad q = - int_E div(v) q + int_bE q v.n
-                         = - div(v) int_E q + int_bE q v.n
-                         = int_bE q v.n
-          since int_E q = int_E 1 q = 0 since q is from ONB set
-        */
-
-#if 1
-        // matrices for edge projections
-        Std::vector<Dune::DynamicMatrix<double> > edgePhiVector(2);
-        edgePhiVector[0].resize(BaseType::basisSets_.edgeSize(0), BaseType::basisSets_.edgeSize(0), 0);
-        edgePhiVector[1].resize(BaseType::basisSets_.edgeSize(1), BaseType::basisSets_.edgeSize(1), 0);
-
-        for (const typename BaseType::ElementSeedType &entitySeed : entitySeeds[agglomerate])
-        {
-          const typename BaseType::ElementType &element = BaseType::gridPart().entity(entitySeed);
-          const auto geometry = element.geometry();
-
-          const auto &shapeFunctionSet = BaseType::basisSets_.basisFunctionSet(BaseType::agglomeration(), element);
-
-          // compute the boundary terms for the value projection
-          for (const auto &intersection : intersections(BaseType::gridPart(), element))
-          {
-            // ignore edges inside the given polygon
-            if (!intersection.boundary() && (BaseType::agglomeration().index(intersection.outside()) == agglomerate))
-              continue;
-            assert(intersection.conforming());
-
-            const typename BaseType::BasisSetsType::EdgeShapeFunctionSetType edgeShapeFunctionSet
-                  = BaseType::basisSets_.edgeBasisFunctionSet(BaseType::agglomeration(),
-                               intersection, BaseType::blockMapper().indexSet().twist(intersection) );
-
-            Std::vector<Std::vector<unsigned int>> mask(2,Std::vector<unsigned int>(0)); // contains indices with Phi_mask[i] is attached to given edge
-            edgePhiVector[0] = 0;
-            edgePhiVector[1] = 0;
-
-            BaseType::interpolation()(intersection, edgeShapeFunctionSet, edgePhiVector, mask);
-
-            auto normal = intersection.centerUnitOuterNormal();
-
-            // now compute int_e Phi^e m_alpha
-            typename BaseType::Quadrature1Type quadrature(BaseType::gridPart(), intersection, 2 * polOrder + 1, BaseType::Quadrature1Type::INSIDE);
-            for (std::size_t qp = 0; qp < quadrature.nop(); ++qp)
+            for( ; i < refElement.size( edgeNumber, dimension-1, dimension ); ++i )
             {
-              auto x = quadrature.localPoint(qp);
-              auto y = intersection.geometryInInside().global(x);
-              const DomainFieldType weight = intersection.geometry().integrationElement(x) * quadrature.weight(qp);
-              // need to call shape set scalar each for the correct test functions
-              shapeFunctionSet.scalarEach(y, [&](std::size_t alpha, RangeFieldType m)
+              int vertexNumber = refElement.subEntity( edgeNumber, dimension-1, i, dimension);
+              const int vtxk = indexSet_.localIndex( element, vertexNumber, dimension );
+              assert(vtxk>=0); // intersection is 'outside' so vertices should be as well
+              vertex(poly,vertexNumber,i*vertexSize,1);
+              for (int r=0;r<baseRangeDimension;++r)
+                mask[0].push_back(vtxk*vertexSize+r);
+              if (order2size<0>(1)>0)
               {
-                alpha += numInnerShapeFunctions;
-                if (alpha<RHSconstraintsMatrix[0].size())
-                {
-                  edgeShapeFunctionSet.evaluateEach(x, [&](std::size_t beta,
-                        typename BaseType::BasisSetsType::EdgeShapeFunctionSetType::RangeType psi)
-                  {
-                    for (std::size_t s=0; s<mask[0].size(); ++s) // note that edgePhi is the transposed of the basis transform matrix
-                      // put into correct offset place in constraint RHS matrix
-                      RHSconstraintsMatrix[mask[0][s]][alpha] += weight * edgePhiVector[0][beta][s] * psi*normal * m;
-                  });
-                }
-                /*
-                else
+                assert(vertexSize==3*baseRangeDimension);
+                for (int r=0;r<baseRangeDimension;++r)
+                  mask[0].push_back(vtxk*vertexSize+baseRangeDimension+r);
+                for (int r=0;r<baseRangeDimension;++r)
+                  mask[0].push_back(vtxk*vertexSize+2*baseRangeDimension+r);
+                for (int r=0;r<baseRangeDimension;++r)
+                  mask[1].push_back(vtxk*vertexSize+baseRangeDimension+r);
+                for (int r=0;r<baseRangeDimension;++r)
+                  mask[1].push_back(vtxk*vertexSize+2*baseRangeDimension+r);
+              }
+              else
+                assert(vertexSize==baseRangeDimension);
+            }
+          }
+          if (order2size<1>(0)>0 ||
+              order2size<1>(1)>0)
+          {
+            edge(poly,intersection,i,edgeSize);
+            int count = 0;
+            for (std::size_t alpha=0;alpha<testBasisSets_.edgeSize();++alpha)
+              for (int deriv=0;deriv<2;++deriv)
+                if (alpha < order2size<1>(deriv))
                 {
-                  std::cout << "shouldn't get here!\n";
-                  std::cout << "should have " << alpha << "<" << RHSconstraintsMatrix[0].size() << std::endl;
-                  abort();
+                  mask[deriv].push_back(k*edgeSize+edgeOffset+count);
+                  ++count;
                 }
-                */
-              });
-            } // quadrature loop
-          } // loop over intersections
-        } // loop over triangles in agglomerate
-#endif
+          }
+        }
       }
+
+      const IndexSetType &indexSet_;
+      TestBasisSetsType testBasisSets_;
+      const unsigned int polOrder_;
+      const bool useOnb_;
     };
 
   } // namespace Vem
 
   namespace Fem
   {
     namespace Capabilities
     {
-        template<class GridPart>
-        struct hasInterpolation<Vem::DivFreeVEMSpace<GridPart> > {
+        template<class FunctionSpace, class GridPart, bool vectorSpace>
+        struct hasInterpolation<Vem::AgglomerationVEMSpace<FunctionSpace, GridPart, vectorSpace> > {
             static const bool v = false;
         };
     }
   } // namespace Fem
 } // namespace Dune
 
-#endif // #ifndef DUNE_VEM_SPACE_DIVFREE_HH
+#endif // #ifndef DUNE_VEM_SPACE_HK_HH
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/space/indexset.hh` & `dune-vem-2.9.dev20220529/dune/vem/space/indexset.hh`

 * *Files 17% similar despite different names*

```diff
@@ -22,69 +22,87 @@
   namespace Vem
   {
 
     // AgglomerationIndexSet
     // ---------------------
 
     template< class GridPart, class Allocator = std::allocator< std::size_t > >
-    using VemAgglomerationIndexSet = AgglomerationIndexSet< GridPart, Allocator >;
-#if 0
+    class VemAgglomerationIndexSet
+    : public AgglomerationIndexSet< GridPart, Allocator >
     {
       typedef VemAgglomerationIndexSet< GridPart, Allocator > ThisType;
       typedef AgglomerationIndexSet< GridPart, Allocator > BaseType;
 
     public:
       // !TS
+      typedef std::array<std::vector<int>,BaseType::dimension+1> TestSpacesType;
       typedef GridPart GridPartType;
 
       typedef typename BaseType::AgglomerationType AgglomerationType;
       typedef typename BaseType::AllocatorType AllocatorType;
 
       // !TS assume vector of vectors
       explicit VemAgglomerationIndexSet ( AgglomerationType &agglomeration,
+          const TestSpacesType &testSpaces,
           AllocatorType allocator = AllocatorType() )
       : BaseType( agglomeration, allocator )
+      , testSpaces_( testSpaces )
       {}
       using BaseType::update;
 
+      // return the number of dofs per codimension
+      // !TS change to take into account vector of vector storage
+      std::array< std::pair< int, unsigned int >, BaseType::dimension+1 > dofsPerCodim () const
+      {
+        const int dimension = BaseType::dimension;
+        int vSize = 0;
+        int eSize = 0;
+        int iSize = 0;
+        for (size_t i=0;i<testSpaces_[0].size();++i)
+          // vSize += (testSpaces_[0][i]>=0) ? pow(BaseType::dimension,i):0;
+          vSize += order2size<0>(i);
+        for (size_t i=0;i<testSpaces_[1].size();++i)
+          eSize += order2size<1>(i);
+        for (size_t i=0;i<testSpaces_[2].size();++i)
+          iSize += order2size<2>(i);
+        return std::array< std::pair< int, unsigned int >, BaseType::dimension+1 >
+               { std::make_pair( dimension,   vSize ),
+                 std::make_pair( dimension-1, eSize ),
+                 std::make_pair( dimension-2, iSize ) };
+      }
+
       Std::vector<int> orders()
       {
-        /*
-        Std::vector<int> ret(3,0);
-        ret[0] += testSpaces_[2][0];
-        ret[1] += std::min( {testSpaces_[2][0] + 1, edgeDegrees()[0]} );
-        ret[2] += std::min( {testSpaces_[2][0] + 2, edgeDegrees()[0]+1, edgeDegrees()[1]} );
-        return ret;
-        */
+          Std::vector<int> ret(3,0);
+          ret[0] += testSpaces_[2][0];
+          ret[1] += std::min( {testSpaces_[2][0] + 1, edgeDegrees()[0]} );
+          ret[2] += std::min( {testSpaces_[2][0] + 2, edgeDegrees()[0]+1, edgeDegrees()[1]} );
+          return ret;
       }
 
       const Std::vector<int> maxDegreePerCodim() const
       {
-        /*
-        Std::vector<int> ret(3);
-          for ( int k = 0; k < ret.size(); k++){
-            ret[k] = *std::max_element( testSpaces_[k].begin(), testSpaces_[k].end() );
-          }
-         return ret;
-       */
+          Std::vector<int> ret(3);
+            for ( int k = 0; k < ret.size(); k++){
+              ret[k] = *std::max_element( testSpaces_[k].begin(), testSpaces_[k].end() );
+            }
+           return ret;
       }
 
       Std::vector<int> edgeDegrees() const
       {
-        /*
         assert( testSpaces_[2].size()<2 );
         Std::vector<int> degrees(2, -1);
         for (std::size_t i=0;i<testSpaces_[0].size();++i)
           degrees[i] += 2*(testSpaces_[0][i]+1);
         if (testSpaces_[0].size()>1 && testSpaces_[0][1]>-1) // add tangential derivatives
           degrees[0] += 2;
         for (std::size_t i=0;i<testSpaces_[1].size();++i)
           degrees[i] += std::max(0,testSpaces_[1][i]+1);
         return degrees;
-        */
       }
       std::size_t edgeSize(int deriv) const
       {
         auto degrees = edgeDegrees();
         return degrees[deriv] < 0 ? 0 :
               Dune::Fem::OrthonormalShapeFunctions<1>::size( degrees[deriv] );
       }
@@ -92,51 +110,51 @@
       {
         auto degrees = edgeDegrees();
         return *std::max_element(degrees.begin(),degrees.end());
       }
 
       const std::vector<int> vertexOrders() const
       {
-        // return testSpaces_[0];
+          return testSpaces_[0];
       }
 
       const std::vector<int> edgeOrders() const
       {
-        // return testSpaces_[1];
+          return testSpaces_[1];
       }
 
       const std::vector<int> innerOrders() const
       {
-        // return testSpaces_[2];
+          return testSpaces_[2];
       }
 
       template <int dim>
       std::size_t order2size(unsigned int deriv) const
       {
-      /*
         if (testSpaces_[dim].size()<=deriv || testSpaces_[dim][deriv]<0)
           return 0;
         else
         {
           if constexpr (dim>0)
             return Dune::Fem::OrthonormalShapeFunctions<dim>::
               size(testSpaces_[dim][deriv]);
           else
             return pow(BaseType::dimension,deriv);
         }
-      */
       }
 
 
     private:
       std::size_t sumTestSpaces(unsigned int codim) const
       {
-        // return std::accumulate(testSpaces_[codim].begin(),testSpaces_[codim].end(),0);
+        return std::accumulate(testSpaces_[codim].begin(),testSpaces_[codim].end(),0);
       }
+      // !TS
+      const TestSpacesType testSpaces_;
     };
-#endif
+
 
   } // namespace Vem
 
 } // namespace Dune
 
 #endif // #ifndef DUNE_VEM_AGGLOMERATION_INDEXSET_HH
```

### Comparing `dune-vem-2.9.0rc1/dune/vem/space/interpolate.hh` & `dune-vem-2.9.dev20220529/dune/vem/space/interpolate.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/dune/vem/space/test.hh` & `dune-vem-2.9.dev20220529/dune/vem/space/test.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/CMakeLists.txt` & `dune-vem-2.9.dev20220529/notMaintained/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/dune-vem.cc` & `dune-vem-2.9.dev20220529/notMaintained/dune-vem.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_4x4_npart=4.msh` & `dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_4x4_npart=4.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_8x8_npart=16.msh` & `dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_8x8_npart=16.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_8x8_npart=2.msh` & `dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_8x8_npart=2.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/gmsh/unit_sq_8x8_npart=4.msh` & `dune-vem-2.9.dev20220529/notMaintained/gmsh/unit_sq_8x8_npart=4.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/gmsh/unitsq-tria-unstr_npart=16.msh` & `dune-vem-2.9.dev20220529/notMaintained/gmsh/unitsq-tria-unstr_npart=16.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/agglo-heat.cc` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/agglo-heat.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/data/parameter` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/data/parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/data/sphere.dgf` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/data/sphere.dgf`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/dirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/dirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/elliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/heat.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/heat.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/heatmodel.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/heatmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/heatscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/heatscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/l2model.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/l2model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/model.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/modelinterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/modelinterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/temporalprobleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/temporalprobleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/vemelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/vemelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/heat-test/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/heat-test/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/fem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/fem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/partitioned-mesh.msh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/partitioned-mesh.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/data/vem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/data/vem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/dataoutputparameters.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/dataoutputparameters.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/dirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/dirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/elliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/fem-helmholtz.cc` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/fem-helmholtz.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/model.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/modelinterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/modelinterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/poisson.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/poisson.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vem-helmholtz.cc` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vem-helmholtz.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vemdirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vemdirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vemelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vemelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/helmholtz-test/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/helmholtz-test/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/fem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/fem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/unit-square-one-partition.msh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/unit-square-one-partition.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/data/vem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/data/vem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/dirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/dirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/elliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/fem-nonlinear.cc` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/fem-nonlinear.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/nonlinearmodel.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/nonlinearmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vem-nonlinear.cc` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vem-nonlinear.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vemdirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vemdirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vemelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vemelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/nonlinear-test/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/nonlinear-test/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/agglo-dg.cc` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/agglo-dg.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/data/agglomeration-parameter` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/data/agglomeration-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/data/partitioned-mesh.msh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/data/partitioned-mesh.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/dataoutputparameters.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/dataoutputparameters.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/dgelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/dgelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/dgrhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/dgrhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/model.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/anisotropic.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/anisotropic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproduct.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproduct.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproductmixedbc.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/cosinusproductmixedbc.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/curvedridges.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/curvedridges.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/interface.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/interface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/reentrantcorner.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/reentrantcorner.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/sinusproduct.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/sinusproduct.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/problems/sphereproblem.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/problems/sphereproblem.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/agglomeration-DG/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/agglomeration-DG/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/data/parameter` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/data/trivial.param` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/data/trivial.param`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/dgelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/dgelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/dgrhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/dgrhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/dune-poisson-agglo-DG.cc` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/dune-poisson-agglo-DG.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/data/mesh.msh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/data/mesh.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/data/parameter` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/data/parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/dgelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/dgelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/dgrhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/dgrhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/dune-dgpoisson.cc` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/dune-dgpoisson.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/model.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/poisson.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/poisson.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/howto-DG/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/howto-DG/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/model.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/poisson.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/poisson.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/travel.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/travel.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/trivial-agglomeration.cc` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/trivial-agglomeration.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/data/mymesh.msh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/data/mymesh.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/data/vem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/data/vem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/dirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/dirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/model.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/model.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/poisson.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/poisson.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vem-poisson-pmesh.cc` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vem-poisson-pmesh.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vemdirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vemdirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vemelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vemelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/poisson-test/vem-test/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/poisson-test/vem-test/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/CMakeLists.txt` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/fem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/fem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-quads.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-quads.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-trias.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-16x16-trias.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-4x4-quads.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-4x4-quads.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/pmesh-agg-trias-4x4.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/pmesh-agg-trias-4x4.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/unit-square-one-partition.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/unit-square-one-partition.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/data/vem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/data/vem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/dirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/dirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/elliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/fem-quasilinear-fp.cc` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/fem-quasilinear-fp.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/quasilinearmodel.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/quasilinearmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vem-quasilinear-fp.cc` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vem-quasilinear-fp.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemdirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemdirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemdirichletconstraintsfromnewton.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemdirichletconstraintsfromnewton.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemelliptic-fp.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemelliptic-fp.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-fixed-point/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-fixed-point/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/CMakeLists.txt` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/fem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/fem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-16x16-quads.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-16x16-quads.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-16x16-trias.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-16x16-trias.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-4x4-quads.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-4x4-quads.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/pmesh-agg-trias-4x4.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/pmesh-agg-trias-4x4.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/unit-square-one-partition.msh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/unit-square-one-partition.msh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/data/vem-parameter` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/data/vem-parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/dirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/dirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/elliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/elliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/fem-quasilinear.cc` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/fem-quasilinear.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/femscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/femscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/probleminterface.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/probleminterface.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/quasilinearmodel.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/quasilinearmodel.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/rhs.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/rhs.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vem-quasilinear.cc` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vem-quasilinear.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vemdirichletconstraints.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vemdirichletconstraints.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vemelliptic.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vemelliptic.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/quasilinear-test/vemscheme.hh` & `dune-vem-2.9.dev20220529/notMaintained/quasilinear-test/vemscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-Pk.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-Pk.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-dgspace.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-dgspace.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-dmatrix.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-dmatrix.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-gmsh.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-gmsh.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-indexset.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-indexset.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-leastsquares.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-leastsquares.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-reactiondiffusion.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-reactiondiffusion.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/notMaintained/test-reactiondiffusion2.cc` & `dune-vem-2.9.dev20220529/notMaintained/test-reactiondiffusion2.cc`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/biharmonic.py` & `dune-vem-2.9.dev20220529/pydemo/biharmonic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 import matplotlib
 matplotlib.rc( 'image', cmap='jet' )
 from matplotlib import pyplot
 import math
 from dune import create
 from dune.grid import cartesianDomain, gridFunction
 from dune.fem.plotting import plotPointData as plot
-from dune.fem.function import integrate, discreteFunction, uflFunction
+from dune.fem.function import integrate, discreteFunction
 from dune.fem import parameter
 from dune.vem import voronoiCells
 from dune.fem.operator import linear as linearOperator
 from scipy.sparse.linalg import spsolve
-from hexagons import hexaGrid
 
 from ufl import *
 import dune.ufl
 
 maxLevel     = 4
-order        = 3
+order        = 4
 epsilon      = 1
 laplaceCoeff = 1
-mu           = 1
+mu           = 0
 
 dune.fem.parameter.append({"fem.verboserank": 0})
 
 # <markdowncell>
 # we can compare different method, e.g., a lagrange space (on the # subtriangulation),
 # a bounding box dg space and a conforming/non conforming VEM space
 
 # <codecell>
 # Note: suboptimal laplace error for bubble (space is reduced to polorder=3 but could be 4 = ts+2
 methods = [ ### "[space,scheme,spaceKwrags]"
-        ["vem","vem",{"order":order, "testSpaces":[ [0,0],[order-4,order-3], [order-4] ] }, "C1-conforming"],
         # ["vem","vem",{"order":order, "testSpaces":[ [0],  [order-3,order-2], [order-4] ] }, "C1-non-conforming"],
         # ["vem","vem",{"order":order, "testSpaces":[ [0],  [order-2,order-2], [order-2] ] }, "C1C0-conforming"],
-        # ["vem","vem",{"order":order, "testSpaces":[ [0],  [order-3,order-2], [order-3] ] }, "C1mod-conforming"],
+        ["vem","vem",{"order":order, "testSpaces":[ [0],  [order-3,order-2], [order-3] ] }, "C1mod-conforming"],
           ]
 if epsilon == 0:
     methods += [
             ["vem","vem",{"order":order, "testSpaces":[ [0],  [order-2,-1], [order-2] ] },      "C0-conforming"],
-            # ["vem","vem",{"order":order-1, "testSpaces":[ [0],  [order-3,-1], [order-3] ] },      "C0pm1-conforming"],
+            ["vem","vem",{"order":order-1, "testSpaces":[ [0],  [order-3,-1], [order-3] ] },      "C0pm1-conforming"],
                ]
 parameters = {"newton.linear.tolerance": 1e-12,
               "newton.linear.preconditioning.method": "jacobi",
               "penalty": 40,  # for the bbdg scheme
               "newton.linear.verbose": False,
-              "newton.verbose": False
+              "newton.verbose": True
               }
 
 # <markdowncell>
 # Now we define the model starting with the exact solution:
 
 # <codecell>
 uflSpace = dune.ufl.Space(2, dimRange=1)
 x = SpatialCoordinate(uflSpace)
 exact = as_vector( [sin(2*pi*x[0])**2*sin(2*pi*x[1])**2] )
-# exact = as_vector( [x[0]**3] )
 
 # next the bilinear form
 # Note: for function which continuous derivatives we have
 #       laplace(u)*laplace(v)*dx = inner(u,v)*dx
 #       as can be seen by using integration by parts on the mixed terms on the right
 #       and using continuety of u,v
 #       For the non conforming spaces we don't have continuety of the
@@ -67,75 +64,54 @@
 #       the norm on H^2 (the left is not a norm in this case).
 #       For computing the forcing term 'b' both formula are fine since
 #       'exact' is smooth enough.
 laplace = lambda w: div(grad(w))
 H = lambda w: grad(grad(w))
 u = TrialFunction(uflSpace)
 v = TestFunction(uflSpace)
-if False:
-    a = ( epsilon*inner(H(u[0]),H(v[0])) +\
-          laplaceCoeff*inner(grad(u),grad(v)) +\
-          mu*inner(u,v)
-        ) * dx
-    # finally the right hand side and the boundary conditions
-    b = ( epsilon*laplace(laplace(exact[0])) -\
-          laplaceCoeff*laplace(exact[0]) +\
-          mu*exact[0] ) * v[0] * dx
-    biLaplaceCoeff = epsilon
-    diffCoeff      = laplaceCoeff
-    massCoeff      = mu
-else:
-    kappa = 1./(1+dot(x,x))
-    beta  = exp(-x[0]*x[1])
-    gamma = sin(dot(x,x))**2
-    a = ( kappa*inner(H(u[0]),H(v[0])) +\
-          beta*inner(grad(u),grad(v)) +\
-          gamma*inner(u,v)
-        ) * dx
-    q = sum([ H(kappa*H(exact[0])[i,j])[i,j] for i in range(2) for j in range(2) ])
-    b = ( q -\
-          laplaceCoeff*div(beta*grad(exact[0])) +\
-          mu*gamma*exact[0] ) * v[0] * dx
-    biLaplaceCoeff = kappa
-    diffCoeff      = laplaceCoeff*beta
-    massCoeff      = mu*gamma
-
+a = ( epsilon*inner(H(u[0]),H(v[0])) +\
+      laplaceCoeff*inner(grad(u),grad(v)) +\
+      mu*inner(u,v)
+    ) * dx
+
+# finally the right hand side and the boundary conditions
+b = ( epsilon*laplace(laplace(exact[0])) -\
+      laplaceCoeff*laplace(exact[0]) +\
+      mu*exact[0] ) * v[0] * dx
 dbc = [dune.ufl.DirichletBC(uflSpace, [0], i+1) for i in range(4)]
+biLaplaceCoeff = epsilon
+diffCoeff      = laplaceCoeff
+massCoeff      = mu
 
 # <markdowncell>
 # Now we define a grid build up of voronoi cells around $50$ random points
 
 # We now define a function to compute the solution and the $L^2,H^1$ error
 # given a grid and a space
 
 # <codecell>
 def compute(grid, space, schemeName):
     # solve the pde
     df = discreteFunction(space, name="solution") # space.interpolate([0],name="solution")
     # df.plot(level=3)
     info = {"linear_iterations":1}
-    if False:
-        df.interpolate(exact)
-        # df.plot(level=3)
-        # uflFunction(grid,name="grad",order=1,ufl=grad(df[0])[0]).plot(level=3)
-        # uflFunction(grid,name="grad",order=1,ufl=grad(df[0])[1]).plot(level=3)
-    else:
-        scheme = create.scheme(schemeName, [a==b, *dbc], space,
-                            # solver="cg",
-                            solver=("suitesparse","umfpack"),
-                            hessStabilization=biLaplaceCoeff,
-                            gradStabilization=diffCoeff,
-                            massStabilization=massCoeff,
-                            parameters=parameters)
-        # info = scheme.solve(target=df)
-        jacobian = linearOperator(scheme)
-        rhs = discreteFunction(space,name="rhs")
-        scheme(df,rhs)
-        rhs.as_numpy[:] *= -1
-        df.as_numpy[:] = spsolve(jacobian.as_numpy, rhs.as_numpy[:])
+    scheme = create.scheme(schemeName, [a==b, *dbc], space,
+                        # solver="cg",
+                        # solver=("suitesparse","umfpack"),
+                        hessStabilization=biLaplaceCoeff,
+                        gradStabilization=diffCoeff,
+                        massStabilization=massCoeff,
+                        parameters=parameters)
+    # df.interpolate(exact)
+    # info = scheme.solve(target=df)
+    jacobian = linearOperator(scheme)
+    rhs = discreteFunction(space,name="rhs")
+    scheme(df,rhs)
+    rhs.as_numpy[:] *= -1
+    df.as_numpy[:] = spsolve(jacobian.as_numpy, rhs.as_numpy[:])
     edf = exact-df
     err = [inner(edf,edf),
            inner(grad(edf),grad(edf)),
            inner(grad(grad(edf)),grad(grad(edf)))]
     errors = [ math.sqrt(e) for e in integrate(grid, err, order=8) ]
     return df, errors, info
 
@@ -143,25 +119,22 @@
 # Finally we iterate over the requested methods and solve the problems
 
 # <codecell>
 # fig = pyplot.figure(figsize=(10*maxLevel,10*len(methods)))
 # figPos = 100*len(methods)+10*maxLevel+1
 results = []
 for level in range(maxLevel):
-    constructor = cartesianDomain([0,0],[1,1],[2*2**level,2*2**level])
+    # constructor = cartesianDomain([0,0],[1,1],[4*2**level,4*2**level])
     # polyGrid = create.grid("agglomerate", constructor, cubes=False )
-    polyGrid = create.grid("agglomerate", voronoiCells(constructor,4*2**level*2**level,"voronoiseeds",
+    constructor = cartesianDomain([0,0],[1,1],[4,4])
+    polyGrid = create.grid("agglomerate", voronoiCells(constructor,16*2**level*2**level,"voronoiseeds",
                load=True,show=False,lloyd=5), convex=True )
-
-    # N = 10*3*2**level+1 # needs to be of the form 6*i+1
-    # polyGrid = hexaGrid(N, 1, 1)
-
     res = []
     for i,m in enumerate(methods):
-        space = create.space(m[0], polyGrid, dimRange=1, storage="numpy", **m[2])
+        space = create.space(m[0], polyGrid, dimRange=1, storage="fem", **m[2])
         dfs,errors,info = compute(polyGrid, space, m[1])
         print("[",level,"]","method:(",m[0],m[2],")",
               "Sizes (polys,simplex,dofs): ",polyGrid.hierarchicalGrid.agglomerate.size, polyGrid.size(0), space.size, "L^2: ", errors[0], "H^1: ", errors[1],
               "H^2: ", errors[2],
               info["linear_iterations"], flush=True)
         res += [ [polyGrid.hierarchicalGrid.agglomerate.size,space.size,errors[0],errors[1],errors[2]] ]
         # dfs.plot(level=4)
```

### Comparing `dune-vem-2.9.0rc1/pydemo/conditioning.py` & `dune-vem-2.9.dev20220529/pydemo/conditioning.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/conditioning.sh` & `dune-vem-2.9.dev20220529/pydemo/conditioning.sh`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/interpolation.py` & `dune-vem-2.9.dev20220529/pydemo/interpolation.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/oldScript/demoA.py` & `dune-vem-2.9.dev20220529/pydemo/oldScript/demoA.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/oldScript/elasticity.py` & `dune-vem-2.9.dev20220529/pydemo/oldScript/elasticity.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/oldScript/elliptic.py` & `dune-vem-2.9.dev20220529/pydemo/oldScript/elliptic.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/parameter` & `dune-vem-2.9.dev20220529/pydemo/parameter`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/plotInterpolation.py` & `dune-vem-2.9.dev20220529/pydemo/plotInterpolation.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/script.py` & `dune-vem-2.9.dev20220529/pydemo/wilmore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,116 @@
+import dune.vem
 import matplotlib
 matplotlib.rc( 'image', cmap='jet' )
 from matplotlib import pyplot
 import math
 from dune import create
 from dune.grid import cartesianDomain, gridFunction
 from dune.fem.plotting import plotPointData as plot
 from dune.fem.function import integrate, discreteFunction
 from dune.fem import parameter
 from dune.vem import voronoiCells
 from dune.fem.operator import linear as linearOperator
 from scipy.sparse.linalg import spsolve
-import numpy
 
-import ufl.algorithms
 from ufl import *
 import dune.ufl
 
-dune.fem.parameter.append({"fem.verboserank": -1})
+maxLevel     = 5
+order        = 3
 
-maxLevel = 5
-order = 3
+dune.fem.parameter.append({"fem.verboserank": 0})
 
-parameters = {"newton.linear.tolerance": 1e-12,
+methods = [ ### "[space,scheme,spaceKwrags]"
+            ["vem","vem",{"testSpaces":[ [0],  [order-3,order-2], [order-4] ] }, "C1-non-conforming"],
+            # ["vem","vem",{"testSpaces":[ [0],  [order-2,order-2], [order-2] ] }, "C1C0-conforming"],
+            # ["vem","vem",{"testSpaces":[ [-1], [order-1,-1], [order-2] ] },   "C0-non-conforming"],
+   ]
+parameters = {"newton.linear.tolerance": 1e-8,
+              "newton.tolerance": 5e-6,
               "newton.linear.preconditioning.method": "jacobi",
-              "penalty": 40,  # for the dg schemes
+              "newton.lineSearch": "simple",
+              "penalty": 40,  # for the bbdg scheme
               "newton.linear.verbose": False,
-              "newton.verbose": False
+              "newton.verbose": True
               }
 
-def runTest(exact, spaceConstructor, get_df):
-    Nval = 5
-    N_values = [2**i*Nval for i in range(maxLevel)]
-    results = []
-    for N in N_values:
-        print('grid size N:', N)
-
-        # set up grid for testing
-        constructor = cartesianDomain([0,0],[1,1],[N,N])
-        cells = voronoiCells(constructor,N*N,"voronoiseeds",load=True,show=False,lloyd=10)
-        grid = create.grid("agglomerate", cells, convex=True)
-
-        # get dimension of range
-        dimRange = exact.ufl_shape[0]
-        print('dim Range:', dimRange)
-
-        # construct space to use using spaceConstructor passed in
-        space = spaceConstructor(grid,dimRange)
-
-        # get sizes for eoc calculation
-        sizes = [grid.hierarchicalGrid.agglomerate.size, space.size, *space.diameters()]
-
-        # solve for df
-        df = get_df(space,exact)
-
-        # calculate errors
-        edf = exact-df
-        err = [inner(edf,edf),
-           inner(grad(edf),grad(edf)),
-           inner(grad(grad(edf)),grad(grad(edf))),
-           energy]
-        errors = [ math.sqrt(e) for e in integrate(grid, err, order=8) ]
-
-        print("bi-laplace errors:", errors )
-        results += [[sizes] + [errors]]
-
-    # calculate eocs
-    h = lambda sizes: sizes[3]
-    eoc = len(results[0][1])*[-1]
-    for level in range(0,maxLevel):
-        print(*results[level], *eoc)
-        if level < maxLevel -1:
-            eoc = [math.log(results[level+1][1][j]/results[level][1][j])/
-            math.log(h(results[level+1][0])/h(results[level][0]))
-            for j in range(len(eoc))]
-
-    assert(0.8*(order-1) <= eoc[2] <= 1.2*(order-1), "eoc out of expected range")
-
-def testElliptic(space, exact):
-    # set up scheme, df, and solve
-    u = TrialFunction(space)
-    v = TestFunction(space)
-    x = SpatialCoordinate(space)
-
-    massCoeff = 1+sin(dot(x,x))       # factor for mass term
-    diffCoeff = 1-0.9*cos(dot(x,x))
-
-    a = (diffCoeff*inner(grad(u),grad(v)) + massCoeff*dot(u,v) ) * dx
-
-    # finally the right hand side and the boundary conditions
-    b = (-div(diffCoeff*grad(exact[0])) + massCoeff*exact[0] ) * v[0] * dx
-    dbc = [dune.ufl.DirichletBC(space, exact, i+1) for i in range(4)]
-
-    df = space.interpolate([0],name="solution")
-    scheme = dune.vem.vemScheme( [a==b, *dbc], space, solver="cg",
-                            gradStabilization=diffCoeff,
-                            massStabilization=massCoeff,
-                            parameters=parameters )
-
-    scheme.solve(target=df)
-
-    return df
-
-def biharmonic(space, exact):
-    laplace = lambda w: div(grad(w))
-    H = lambda w: grad(grad(w))
-    u = TrialFunction(space)
-    v = TestFunction(space)
-
-    a = ( inner(H(u[0]),H(v[0])) ) * dx
-    b = ( laplace(laplace(exact[0])) )* v[0] * dx
-    dbcs = [dune.ufl.DirichletBC(space, [0], i+1) for i in range(4)]
-
-    scheme = dune.vem.vemScheme( [a==b, *dbcs], space, hessStabilization=1, solver="cg", parameters=parameters )
-    df = discreteFunction(space, name="solution")
-    info = scheme.solve(target=df)
 
+def compute(grid, s, schemeName):
+    dt = 4e-4
+    space = create.space(s[0], polyGrid, order=order, **s[1])
+    t   = dune.ufl.Constant(0,"time")
+
+    x   = SpatialCoordinate(space)
+    initial = sin(2*pi*x[0])**2*sin(2*pi*x[1])**2
+
+    # Wilmore functional W(psi)
+    psi = Coefficient(space)
+    Q = lambda p: 1+inner(p,p)
+    E = lambda p: 1/Q(p)**0.25 * ( Identity(2) - outer(p,p)/Q(p) )
+    Wint = 1/2*inner( E(grad(psi)),grad(grad(psi)) )**2
+    W = Wint * dx
+
+    # variation bilinear form
+    phi = TestFunction(space)
+    a   = derivative(W,psi,phi)
+
+    # third order time stepping (Gauss radau collocation)
+    tau = dune.ufl.Constant(0,"dt")
+    df  = discreteFunction(space, name="solution") # main solution
+    # space for time stepping (df=U^n, U[0]=intermediate, U[1]=U^{n+1}
+    rkSpace = create.space(s[0], polyGrid, order=order, dimRange=2, **s[1])
+    U       = TrialFunction(rkSpace)
+    V       = TestFunction(rkSpace)
+    dfs     = [  df,   U[0],  U[1]  ]
+    factors = [ [-2,  3./2., 1./2.] ,
+                [ 2, -9./2., 5./2.] ]
+    dtForm = lambda w,u,v: inner(w/Q(u),v)*dx
+    rkForm  = sum(f*dtForm(u,U[i],V[i]) for i in range(2) for u,f in zip(dfs,factors[i]))
+    rkForm += tau*sum(replace(a,{psi:U[i],phi:V[i]}) for i in range(2))
+
+    dbc = [dune.ufl.DirichletBC(rkSpace, rkSpace.dimRange*[0], i+1) for i in range(4)]
+    biLaplaceCoeff = [dt,dt]
+    diffCoeff      = [0,0]
+    massCoeff      = [1,1] # 1/Q(U[i]) for i in range(2)]
+
+    print("# solving: ",s, "size",space.size, "parameters:(", biLaplaceCoeff,",",diffCoeff,",",massCoeff,")")
+
+    scheme = create.scheme(schemeName,
+                        [rkForm == 0, *dbc], # space, # this gives is a compiler error
+                        solver=("suitesparse","umfpack"),
+                        hessStabilization=biLaplaceCoeff,
+                        gradStabilization=diffCoeff,
+                        massStabilization=massCoeff,
+                        parameters=parameters)
+    df.interpolate(initial)
+    energy = integrate(grid,replace(Wint,{psi:df}),order=5)
+    vtk = grid.sequencedVTK("voro", pointdata=[df],subsampling=2)
+    t.value = 0
+    tau.value = dt
+    count = 0
+    info = None
+    # tmp = discreteFunction(rkSpace, name="rk")
+    tmp = rkSpace.interpolate([initial,initial], name="rk")
+    while t.value < 0.01:
+        count += 1
+        if count % 1 == 0:
+            energy = integrate(grid,replace(Wint,{psi:df}),order=5)
+            vtk()
+        print("[",count,"]",t.value,energy,tau.value,info,flush=True)
+        info = scheme.solve(target=tmp)
+        t.value += tau
+        df.interpolate(tmp[1])
     return df
 
-def main():
-    # test with conforming second order VEM space
-    conformingSpaceConstructor = lambda grid, r: dune.vem.vemSpace( grid, order=order, dimRange=r, storage="istl", testSpaces = [0,order-2,order-2] )
-    # define exact solution
-    x = ufl.SpatialCoordinate(ufl.triangle)
-    exact = as_vector( [x[0]*x[1] * cos(pi*x[0]*x[1])] )
-
-    # run tests for second order case
-    # runTest(exact, conformingSpaceConstructor, testElliptic)
-
-    # exact solution for biharmonic problem
-    exact_biharmonic = as_vector( [sin(2*pi*x[0])**2*sin(2*pi*x[1])**2] )
-    ncC1testSpaces = [ [0], [order-3,order-2], [order-4] ]
-    nonconformingSpaceConstructor = lambda grid, r: dune.vem.vemSpace( grid, order=order, dimRange=r, storage="istl", testSpaces = ncC1testSpaces )
-
-    # run tests for fourth order problems
-    runTest(exact_biharmonic, nonconformingSpaceConstructor, biharmonic)
-
-main()
+for level in range(1,2): # maxLevel): # 2,3
+    constructor = cartesianDomain([0,0],[1,1],[20*2**level,20*2**level])
+    polyGrid = create.grid("agglomerate", constructor, cubes=False )
+    # polyGrid = create.grid("agglomerate", voronoiCells(constructor,400*2**level*2**level,"voronoiseeds",load=True,show=False,lloyd=5) )
+    @gridFunction(polyGrid, name="cells")
+    def polygons(en,x):
+        return polyGrid.hierarchicalGrid.agglomerate(en)
+    # polygons.plot(colorbar="horizontal")
+    for i,m in enumerate(methods):
+        dfs = compute(polyGrid, [m[0], m[2]], m[1])
+        print("[",level,"]","method:(",m[0],m[2],")",
+              "Grid-Size: ",polyGrid.size(0), flush=True)
```

### Comparing `dune-vem-2.9.0rc1/pydemo/testelliptic.py` & `dune-vem-2.9.dev20220529/pydemo/testelliptic.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/pydemo/uzawa.py` & `dune-vem-2.9.dev20220529/pydemo/uzawa.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-# %% [markdown]
-# .. index:: Solvers; Saddle Point (Uzawa)
-#
-# # Saddle Point Solver (using Scipy)
-# %%
 import matplotlib
 matplotlib.rc( 'image', cmap='jet' )
 from matplotlib import pyplot
-import numpy
-from scipy.sparse import linalg
-from dune.grid import cartesianDomain
-from dune.alugrid import aluCubeGrid
+
 from ufl import SpatialCoordinate, CellVolume, TrialFunction, TestFunction,\
-                inner, dot, div, nabla_grad, grad, dx, as_vector, transpose, Identity, sym, \
-                FacetNormal, ds, dS, avg, jump, CellVolume, FacetArea
+                inner, dot, div, grad, dx, as_vector, transpose, Identity
 from dune.ufl import Constant, DirichletBC
-import dune.fem
+
 from dune.fem.operator import linear as linearOperator
+from dune.fem import parameter
+parameter.append({"fem.verboserank": 0})
 
-import dune.vem
-from dune.fem.operator import galerkin as galerkinOperator
-from dune.vem import vemScheme as vemScheme
-from dune.fem.scheme import galerkin as galerkinScheme
-
-def plot(target):
-    fig = pyplot.figure(figsize=(10,10))
-    target[0].plot(colorbar="vertical", figure=(fig, 211))
-    target[1].plot(colorbar="vertical", figure=(fig, 212))
-    pyplot.show()
-
-def dgLaplace(beta, p,q, spc, p_bnd, dD):
-    n             = FacetNormal(spc)
-    he            = avg( CellVolume(spc) ) / FacetArea(spc)
-    hbnd          = CellVolume(spc) / FacetArea(spc)
-    aInternal     = dot(grad(p), grad(q)) * dx
-    diffSkeleton  = beta/he*jump(p)*jump(q)*dS -\
-                    dot(avg(grad(p)),n('+'))*jump(q)*dS -\
-                    jump(p)*dot(avg(grad(q)),n('+'))*dS
-    diffSkeleton -= ( dot(grad(p),n)*q*dD +\
-                      p_bnd*dot(grad(q),n)*dD ) * ds
-    if p_bnd is not None:
-        diffSkeleton += beta/hbnd*(p-p_bnd)*dD*q*ds
-    return aInternal + diffSkeleton
-class Uzawa:
-    def __init__(self, grid, spcU, spcP, dbc_u, forcing,
-                 mu, tau, u_h_n=None, explicit=False,
-                 tolerance=1e-9, precondition=True, verbose=False,
-                 lagrange=False):
-        self.dimension = grid.dimension
-        self.verbose = verbose
-        self.tolerance2 = tolerance**2
-        self.dbc_u = dbc_u
-        self.mu = Constant(mu, "mu")
-        if tau is not None:
-            assert tau>0
-            self.nu  = Constant(1/tau, "nu")
+useCartesian  = False
+uzawaPreconditioner = True
+storage="petsc"
+
+mu_   = 0.1
+nu_   = 10.0
+
+def compute(useVem,order,version,plot=False):
+    print("########################################################")
+    print(useVem,order,version)
+    print("########################################################")
+    # grid construction
+    from dune.grid import structuredGrid, cartesianDomain
+    from dune.vem import polyGrid        as leafGridView
+    domain = cartesianDomain([0,0],[3,1],[30,10])
+    if useCartesian:
+        constructor = domain
+    else:
+        from dune.vem import voronoiCells
+        constructor = voronoiCells(domain,300,"uzawaseeds",True)
+    grid = leafGridView( constructor )
+    if plot: grid.plot()
+
+    # spaces and schemes
+    from dune.fem.operator import galerkin   as galerkinOperator
+    if not useVem:
+        from dune.fem.space    import lagrange   as velocitySpace
+        from dune.fem.scheme   import galerkin   as velocityScheme
+        if version=="TH":
+            from dune.fem.space  import lagrange as pressureSpace
+            from dune.fem.scheme import galerkin as pressureScheme
+            useDGPressure = False
         else:
-            self.nu  = Constant(0, "nu")
-        u = TrialFunction(spcU)
-        v = TestFunction(spcU)
-        p = TrialFunction(spcP)
-        q = TestFunction(spcP)
-        forcing = dot(forcing,v)
-        if u_h_n is not None:
-            forcing += dot(self.nu*u_h_n,v)
-            b = lambda u1,u2,phi: dot( dot(u1, nabla_grad(u2)), phi)
-            symb = lambda u1,u2,phi: ( b(u1,u2,phi) - b(u1,phi,u2) ) / 2
-            if explicit:
-                forcing -= b( u_h_n, u_h_n, v )
-            else:
-                # forcing -= b(u_h_n, u, v)
-                # forcing -= b(u,u_h_n,v)
-                # ustable forcing -= symb(u_h_n, u, v)
-                # default
-                forcing -= ( b(u_h_n, u, v) + b(u,u_h_n,v) ) / 2
-                # unstable at outflow forcing -= ( symb(u_h_n, u, v) + symb(u,u_h_n,v) ) / 2
-        epsilon = lambda u: sym(nabla_grad(u))
-        mainModel   = ( self.nu*dot(u,v) - forcing + 2*self.mu*inner(epsilon(u), epsilon(v)) ) * dx
-        gradModel   = -p*div(v) * dx
-        divModel    = -div(u)*q * dx
-        massModel   = p*q * dx
-        preconModel = inner(grad(p),grad(q)) * dx
-
-        if not lagrange:
-            self.mainOp = vemScheme( ( mainModel==0, *dbc_u ),
-                                       gradStabilization=as_vector([self.mu*2,self.mu*2]),
-                                       massStabilization=as_vector([self.nu,self.nu])
-                                     )
+            from dune.fem.space  import dgonb    as pressureSpace
+            from dune.fem.scheme import dg       as pressureScheme
+            useDGPressure = True
+        spcU = velocitySpace(grid, dimRange=grid.dimension, order=order, storage=storage)
+        spcP = pressureSpace(grid, dimRange=1, order=order-1, storage=storage),
+    else:
+        if version=="TH":
+            veloTestSpaces = [order,   [0,order-2,order-2]]
+            presTestSpaces = [order-1, [0,order-3,order-3]]
+            useDGPressure = False
+        if version=="mini":
+            veloTestSpaces = [order,   [0,order-2,order-1]]
+            presTestSpaces = [order,   [0,order-2,order-2]]
+            useDGPressure = False
+        if version=="non-conf":
+            veloTestSpaces = [order,   [-1,order-1,order-2]]
+            presTestSpaces = order-1
+            useDGPressure = True
+        if version=="SV":
+            veloTestSpaces = [order,   [0,order-2,order-2]]
+            presTestSpaces = order-1
+            useDGPressure = True
+        from dune.vem import vemSpace   as velocitySpace
+        from dune.vem import vemScheme  as velocityScheme
+        if not useDGPressure:
+            from dune.vem import vemSpace   as pressureSpace
+            from dune.vem import vemScheme  as pressureScheme
+            spcU = velocitySpace(grid, dimRange=grid.dimension, storage=storage,
+                      order=veloTestSpaces[0], testSpaces=veloTestSpaces[1])
+            spcP = pressureSpace(grid, dimRange=1, storage=storage,
+                      order=presTestSpaces[0], testSpaces=presTestSpaces[1])
         else:
-            self.mainOp = galerkinScheme( ( mainModel==0, *dbc_u ) )
-        gradOp    = galerkinOperator( gradModel, spcP,spcU)
-        divOp     = galerkinOperator( divModel, spcU,spcP)
-        massOp    = galerkinOperator( massModel, spcP)
-
-        self.mainLinOp = linearOperator(self.mainOp)
-        self.G    = linearOperator(gradOp).as_numpy
-        self.D    = linearOperator(divOp).as_numpy
-        self.M    = linearOperator(massOp).as_numpy
-        self.Minv = lambda rhs: linalg.spsolve(self.M,rhs)
-
-        if precondition and self.mainOp.model.nu > 0:
-            if not lagrange:
-                preconModel = dgLaplace(10, p,q, spcP, 0, 1)
-                preconOp    = galerkinOperator( preconModel, spcP)
-            else:
-                preconModel = inner(grad(p),grad(q)) * dx
-                preconOp    = galerkinOperator( (preconModel,DirichletBC(spcP,0)), spcP)
-            self.P    = linearOperator(preconOp).as_numpy
-            self.Pinv = lambda rhs: linalg.spsolve(self.P,rhs)
+            from dune.vem import bbdgSpace  as pressureSpace
+            from dune.vem import bbdgScheme as pressureScheme
+            spcU = velocitySpace(grid, dimRange=grid.dimension, storage=storage,
+                      order=veloTestSpaces[0], testSpaces=veloTestSpaces[1])
+            spcP = pressureSpace(grid, dimRange=1, storage=storage,
+                      order=presTestSpaces)
+
+    velocity = spcU.interpolate([0,]*spcU.dimRange, name="velocity")
+    pressure = spcP.interpolate([0], name="pressure")
+    print("size of pressure space:",spcP.size)
+    print("size of velocity space:",spcU.size)
+
+    # setting up the problem
+    cell  = spcU.cell()
+    x     = SpatialCoordinate(cell)
+    mu    = Constant(mu_,  "mu")
+    nu    = Constant(nu_,  "nu")
+    u     = TrialFunction(spcU)
+    v     = TestFunction(spcU)
+    p     = TrialFunction(spcP)
+    q     = TestFunction(spcP)
+
+    # exact solution and resulting forcing
+    exact_u     = as_vector( [x[1] * (1.-x[1]), 0] )
+    exact_p     = as_vector( [ (-2*x[0] + 2)*mu ] )
+    f           = as_vector( [0,]*grid.dimension )
+    f          += nu*exact_u
+
+    # ufl forms
+    mainModel   = (nu*dot(u,v) + mu*inner(grad(u)+grad(u).T, grad(v)) - dot(f,v)) * dx
+    gradModel   = -inner( p[0]*Identity(grid.dimension), grad(v) ) * dx
+    divModel    = -div(u)*q[0] * dx
+    massModel   = inner(p,q) * dx
+    preconModel = inner(grad(p),grad(q)) * dx
+
+    # operators and schemes
+    if not useVem:
+        mainOp       = velocityScheme([mainModel==0,DirichletBC(spcU,exact_u,1)])
+        if useDGPressure:
+            preconOp = pressureScheme(preconModel==0, parameters={"penalty":20})
         else:
-            self.Pinv = None
-
-        self.rhsVelo  = spcU.interpolate(spcU.dimRange*[0], name="vel")
-        self.rhsPress = spcP.interpolate(0, name="pres")
-        self.rhs_u  = self.rhsVelo.as_numpy
-        self.rhs_p  = self.rhsPress.as_numpy
-        self.r      = numpy.copy(self.rhs_p)
-        self.d      = numpy.copy(self.rhs_p)
-        self.precon = numpy.copy(self.rhs_p)
-        self.xi     = numpy.copy(self.rhs_u)
-
-    def solve(self,target):
-        velocity = target[0]
-        pressure = target[1]
-        info = {"uzawa.outer.iterations":0,
-                "uzawa.converged":False}
-        # problem is linear but coefficients depend on previous time step so need to reassemble
-        self.mainOp.jacobian(velocity, self.mainLinOp)
-        A = self.mainLinOp.as_numpy
-        Ainv = lambda rhs: linalg.spsolve(A,rhs)
-        sol_u = velocity.as_numpy
-        sol_p = pressure.as_numpy
-        # right hand side for Shur complement problem
-        velocity.clear()
-        self.mainOp(velocity,self.rhsVelo)
-        self.rhs_u *= -1
-        self.xi[:]  = self.G*sol_p
-        self.rhs_u -= self.xi
-        self.mainOp.setConstraints(self.rhsVelo)
-        sol_u[:]      = Ainv(self.rhs_u[:])
-        self.rhs_p[:] = self.D*sol_u
-        self.r[:]     = self.Minv(self.rhs_p[:])
-        if self.Pinv:
-            self.precon.fill(0)
-            self.precon[:] = self.Pinv(self.rhs_p[:])
-            self.r *= self.mu.value
-            self.r += self.nu.value*self.precon
-        self.d[:] = self.r[:]
-        delta = numpy.dot(self.r,self.rhs_p)
-        if self.verbose:
-            print(0,delta,self.tolerance2)
-        # cg type iteration
-        for m in range(1,1000):
-            self.xi.fill(0)
-            self.rhs_u[:] = self.G*self.d
-            self.mainOp.setConstraints([0,]*self.dimension, self.rhsVelo)
-            self.xi[:] = Ainv(self.rhs_u[:])
-            self.rhs_p[:] = self.D*self.xi
-            rho = delta / numpy.dot(self.d,self.rhs_p)
-            sol_p += rho*self.d
-            sol_u -= rho*self.xi
-            self.rhs_p[:] = self.D*sol_u
-            self.r[:] = self.Minv(self.rhs_p[:])
-            if self.Pinv:
-                self.precon.fill(0)
-                self.precon[:] = self.Pinv(self.rhs_p[:])
-                self.r *= self.mu.value
-                self.r += self.nu.value*self.precon
-            oldDelta = delta
-            delta = numpy.dot(self.r,self.rhs_p)
-            if self.verbose:
-                print(m,delta,self.tolerance2)
-            if delta < self.tolerance2:
-                info["uzawa.converged"] = True
-                break
-            gamma = delta/oldDelta
-            self.d *= gamma
-            self.d += self.r
-        info["uzawa.outer.iterations"] = m
-        return info
-
-def main():
-    useVem   = True
-    muValue  = 0.1
-    tauValue = 1e-2
-    order    = 2
-    grid = dune.vem.polyGrid(cartesianDomain([0,0],[3,1],[30*4,10*4]),cubes=False)
-    if useVem:
-        spcU = dune.vem.divFreeSpace( grid, order=order, conforming=True)
-        spcP = dune.vem.bbdgSpace( grid, order=0 )
+            preconOp = pressureScheme(preconModel==0)
     else:
-        spcU = dune.fem.space.lagrange( grid, order=order, dimRange=2 )
-        spcP = dune.fem.space.lagrange( grid, order=order-1 )
-
-    x       = SpatialCoordinate(spcU)
-    exact_u = as_vector( [x[1] * (1.-x[1]), 0] ) # dy u_x = 1-2y, -dy^2 u_x = 2
-    exact_p = (-2*x[0] + 2)*muValue              # dx p   = -2mu
-    f       = as_vector( [0,]*grid.dimension )
-    f      += exact_u/tauValue
-
-    # discrete functions
-    velocity = spcU.interpolate(spcU.dimRange*[0], name="velocity")
-    pressure = spcP.interpolate(0, name="pressure")
-
-    dbc = [ DirichletBC(velocity.space,exact_u,None) ]
-    uzawa = Uzawa(grid, spcU, spcP, dbc, f,
-                  muValue, tauValue, u_h_n=None,
-                  tolerance=1e-9, precondition=True, verbose=True, # tolerance 2e-5 (TH p=2)
-                  lagrange=not useVem )
-    uzawa.solve([velocity,pressure])
-    print("Retry")
-    uzawa.solve([velocity,pressure])
-
-    fig = pyplot.figure(figsize=(10,10))
-    velocity.plot(colorbar="vertical", figure=(fig, 211))
-    pressure.plot(colorbar="vertical", figure=(fig, 212))
-    pyplot.show()
-    fig = pyplot.figure(figsize=(10,10))
-    dune.fem.plotting.plotPointData(grad(velocity[0])[0], grid=grid,colorbar="vertical", figure=(fig, 211))
-    dune.fem.plotting.plotPointData(grad(velocity[0])[1], grid=grid,colorbar="vertical", figure=(fig, 212))
-    pyplot.show()
-
-if __name__ == "__main__":
-    main()
+        mainOp       = velocityScheme([mainModel==0,DirichletBC(spcU,exact_u,1)],
+                             gradStabilization=as_vector([2*mu_,2*mu_]),
+                             massStabilization=as_vector([nu_,nu_]) )
+        if useDGPressure:
+            preconOp = pressureScheme(preconModel==0, parameters={"penalty":20})
+        else:
+            preconOp = pressureScheme(preconModel==0, gradStabilization=1)
+    mainOp.model.mu = mu_
+    mainOp.model.nu = nu_
+
+    gradOp      = galerkinOperator(gradModel)
+    divOp       = galerkinOperator(divModel)
+    massOp      = pressureScheme(massModel==0)
+
+    A = linearOperator(mainOp)
+    G = linearOperator(gradOp)
+    D = linearOperator(divOp)
+    M = linearOperator(massOp)
+    P = linearOperator(preconOp)
+
+    solver = {"method":"cg","tolerance":1e-10, "verbose":False}
+    Ainv   = mainOp.inverseLinearOperator(A,parameters=solver)
+    Minv   = massOp.inverseLinearOperator(M,parameters=solver)
+    Pinv   = preconOp.inverseLinearOperator(P,solver)
+
+    # auxiliary variables for uzawa algorithm
+    rhsVelo  = velocity.copy()
+    rhsPress = pressure.copy()
+    r      = rhsPress.copy()
+    d      = rhsPress.copy()
+    precon = rhsPress.copy()
+    xi     = rhsVelo.copy()
+
+    # compute initial residual
+    mainOp(velocity,rhsVelo)
+    rhsVelo *= -1
+    G(pressure,xi)
+    rhsVelo -= xi
+    mainOp.setConstraints(rhsVelo)
+    mainOp.setConstraints(velocity)
+
+    Ainv(rhsVelo, velocity)
+    D(velocity,rhsPress)
+    Minv(rhsPress, r)
+
+    if uzawaPreconditioner and mainOp.model.nu > 0:
+        precon.clear()
+        Pinv(rhsPress, precon)
+        r *= mainOp.model.mu
+        r.axpy(mainOp.model.nu,precon)
+
+    d.assign(r)
+    delta = r.scalarProductDofs(rhsPress)
+    print("delta:",delta,flush=True)
+    assert delta >= 0
+
+    # start iteration
+    for m in range(100):
+        xi.clear()
+        G(d,rhsVelo)
+        mainOp.setConstraints(\
+            [0,]*grid.dimension, rhsVelo)
+        Ainv(rhsVelo, xi)
+        D(xi,rhsPress)
+        rho = delta /\
+           d.scalarProductDofs(rhsPress)
+        pressure.axpy(rho,d)
+        velocity.axpy(-rho,xi)
+        D(velocity, rhsPress)
+        Minv(rhsPress,r)
+        if uzawaPreconditioner and mainOp.model.nu > 0:
+            precon.clear()
+            Pinv(rhsPress,precon)
+            r *= mainOp.model.mu
+            r.axpy(mainOp.model.nu,precon)
+        oldDelta = delta
+        delta = r.scalarProductDofs(rhsPress)
+        print("delta:",delta,flush=True)
+        if delta < 1e-9: break
+        gamma = delta/oldDelta
+        d *= gamma
+        d += r
+    if plot:
+        velocity.plot(colorbar="horizontal")
+        pressure.plot(colorbar="horizontal")
+    return velocity,pressure
+
+fig = pyplot.figure(figsize=(40,20))
+order = 2
+solutions = []
+solutions += [compute(True, order, "TH")]
+solutions[0][0].plot(figure=(fig,421),gridLines=None, colorbar=None)
+solutions[0][1].plot(figure=(fig,422),gridLines=None, colorbar=None)
+solutions += [compute(True, order-1, "mini")]
+solutions[1][0].plot(figure=(fig,423),gridLines=None, colorbar=None)
+solutions[1][1].plot(figure=(fig,424),gridLines=None, colorbar=None)
+solutions += [compute(True, order, "non-conf")]
+solutions[2][0].plot(figure=(fig,425),gridLines=None, colorbar=None)
+solutions[2][1].plot(figure=(fig,426),gridLines=None, colorbar=None)
+solutions += [compute(True, order, "SV")]
+solutions[3][0].plot(figure=(fig,427),gridLines=None, colorbar=None)
+solutions[3][1].plot(figure=(fig,428),gridLines=None, colorbar=None)
+pyplot.tight_layout()
+pyplot.show()
```

### Comparing `dune-vem-2.9.0rc1/pyproject.toml` & `dune-vem-2.9.dev20220529/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # This is uses the `Python-Requires` field in the `dune.modules` file to
 # populate the `requires` entry. Additional packages needed for the package
 # build should be added in the `dune.modules`. These packages will then also be
 # included in the package install from source.
 #
 [build-system]
-requires = ['cmake>=3.13', 'dune-alugrid<=v2.9.0rc1', 'dune-fem<=v2.9.0rc1', 'matplotlib', 'ninja', 'pip', 'requests', 'scikit-build', 'scipy', 'setuptools', 'sortedcontainers', 'wheel']
+requires = ['cmake>=3.13', 'dune-alugrid<=2.9.dev20220529', 'dune-fem<=2.9.dev20220529', 'matplotlib', 'ninja', 'pip', 'requests', 'scikit-build', 'scipy', 'setuptools', 'sortedcontainers', 'triangle', 'wheel']
 build-backend = 'setuptools.build_meta'
```

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/bbox.py` & `dune-vem-2.9.dev20220529/python/dune/vem/bbox.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/min_bounding_rect.py` & `dune-vem-2.9.dev20220529/python/dune/vem/min_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/patch.py` & `dune-vem-2.9.dev20220529/python/dune/vem/patch.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/qhull_2d.py` & `dune-vem-2.9.dev20220529/python/dune/vem/qhull_2d.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/tutorial/vemdemo.py` & `dune-vem-2.9.dev20220529/pydemo/vemdemo.py`

 * *Files identical despite different names*

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/vem.py` & `dune-vem-2.9.dev20220529/python/dune/vem/vem.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,17 +88,14 @@
                     '}',
                     'auto obj = new DuneType( *agglo );',
                     'return obj;'],
                    ['"gridView"_a', '"agglomerate"_a', '"rotatedBB"_a',
                     'pybind11::keep_alive< 1, 2 >()'] )
 
 
-    # is defined on the index set which is not used for the dg space
-    # diameterMethod = Method('diameters',
-    #    '''[]( DuneType &self ) { return self.blockMapper().indexSet().diameters(); }''' )
     updateMethod = Method('update',
        '''[]( DuneType &self ) { self.update(); }''' )
 
     spc = module(field, includes, typeName, constructor, updateMethod, scalar=scalar, storage=storage,
              ctorArgs=[view, agglomerate,rotatedBB])
     addStorage(spc, storage)
     return spc.as_ufl()
@@ -115,16 +112,15 @@
     return dg(model,space,penalty,solver,parameters,penaltyClass)
     # return galerkin(model,space,solver,parameters)
 
 def vemSpace(view, order=1, testSpaces=None, scalar=False,
              dimRange=None, conforming=True, field="double",
              storage="numpy",
              basisChoice=2, rotatedBB=True,
-             edgeInterpolation=False,
-             vectorSpace=False, reduced=False):
+             edgeInterpolation=False, vectorSpace=False):
     """create a virtual element space over an agglomerated grid
 
     Args:
         view: the underlying grid view
         order: polynomial order of the finite element functions
         dimRrange: dimension of the range space
         field: field of the range space
@@ -175,18 +171,15 @@
     includes = [ "dune/fem/gridpart/common/gridpart.hh", "dune/vem/space/hk.hh" ] + view.cppIncludes
     dimw = view.dimWorld
     viewType = view.cppTypeName
 
     gridPartName = "Dune::FemPy::GridPart< " + view.cppTypeName + " >"
     typeName = "Dune::Vem::AgglomerationVEMSpace< " +\
       "Dune::Fem::FunctionSpace< double, " + field + ", " + str(dimw) + ", " + str(dimRange) + " >, " +\
-      gridPartName +\
-      (", true " if vectorSpace else ", false ") +\
-      (", true " if reduced else ", false ") +\
-      " >"
+      gridPartName + (", true " if vectorSpace else ", false ") + " >"
     constructor = Constructor(
                    ['pybind11::handle gridView',
                     'const pybind11::object agglomerate',
                     'unsigned int order',
                     'const std::array<std::vector<int>,'+str(view.dimension+1)+'> &testSpaces',
                     'int basisChoice','bool edgeInterpolation','bool rotatedBB'],
                    ['typedef Dune::Vem::Agglomeration<' + gridPartName + '> AggloType;',
@@ -266,190 +259,23 @@
         from dune.fem.space import lagrange
         return lagrange(view,order=order,scalar=scalar,dimRange=dimRange,field=field,storage=storage)
     elif version == "non-conforming":
         return vemSpace(view,order=order,scalar=scalar,dimRange=dimRange,field=field,storage=storage,
                         conforming=False, basisChoice=basisChoice)
     raise AttributeError("wrong version string provided:",version)
 
-###############################
-
-def curlFreeSpace(view, order=1,
-             field="double", storage="numpy",
-             basisChoice=2, rotatedBB=True):
-    """create a virtual element space over an agglomerated grid
-
-    Args:
-        view: the underlying grid view
-        order: polynomial order of the finite element functions
-        field: field of the range space
-        storage: underlying linear algebra backend
-
-    Returns:
-        Space: the constructed Space
-    """
-
-    from dune.fem.space import module, addStorage
-
-    if order < 0:
-        raise KeyError(\
-            "Parameter error in DiscontinuousGalerkinSpace with "+
-            "order=" + str(order) + ": " +\
-            "order has to be greater or equal to 0")
-
-    agglomerate = view.hierarchicalGrid.agglomerate
-
-    includes = [ "dune/fem/gridpart/common/gridpart.hh", "dune/vem/space/curlfree.hh" ] + view.cppIncludes
-    dimw = view.dimWorld
-    viewType = view.cppTypeName
-
-    gridPartName = "Dune::FemPy::GridPart< " + view.cppTypeName + " >"
-    typeName = "Dune::Vem::CurlFreeVEMSpace< " + gridPartName + " >"
-    constructor = Constructor(
-                   ['pybind11::handle gridView',
-                    'const pybind11::object agglomerate',
-                    'unsigned int order',
-                    'int basisChoice','bool rotatedBB'],
-                   ['typedef Dune::Vem::Agglomeration<' + gridPartName + '> AggloType;',
-                    'AggloType *agglo = nullptr;',
-                    '// check storage',
-                    'pybind11::function retrieve = pybind11::module::import("dune.vem.vem").attr("retrieveAgglo_");',
-                    'pybind11::function insert   = pybind11::module::import("dune.vem.vem").attr("insertAgglo_");',
-                    'pybind11::function remove   = pybind11::module::import("dune.vem.vem").attr("removeAgglo_");',
-                    'pybind11::handle aggloExists = retrieve(gridView);',
-                    'if (! pybind11::isinstance<pybind11::none>(aggloExists) ) {',
-                    '  // std::cout << "retrieve agglo\\n";',
-                    '  agglo = static_cast<AggloType*>(aggloExists.cast<void*>());',
-                    '}',
-                    'else {',
-                    '  agglo = new AggloType(',
-                    '           Dune::FemPy::gridPart<' + viewType + '>(gridView),rotatedBB,',
-                    '      [agglomerate](const auto& idx)',
-                    '      { return agglomerate(idx).template cast<unsigned int>(); } );',
-                    '  insert(gridView,(void*)agglo);',
-                    '  pybind11::cpp_function aggloCleanup(',
-                    '        [agglo,remove](pybind11::handle weakref) {',
-                    '        // std::cout << "remove agglo\\n";',
-                    '        remove((void*)agglo);',
-                    '        delete agglo;',
-                    '        weakref.dec_ref();',
-                    '    });',
-                    '  (void) pybind11::weakref(gridView, aggloCleanup).release();',
-                    '  // std::cout << "new agglo\\n";',
-                    '}',
-                    'auto obj = new DuneType(*agglo, order, basisChoice );',
-                    'return obj;'],
-                   ['"gridView"_a', '"agglomerate"_a',
-                    '"order"_a',
-                    '"basisChoice"_a', '"rotatedBB"_a',
-                    'pybind11::keep_alive< 1, 2 >()'] )
-    diameterMethod = Method('diameters',
-       '''[]( DuneType &self ) { return self.blockMapper().indexSet().diameters(); }''' )
-    updateMethod = Method('update',
-       '''[]( DuneType &self ) { self.update(); }''' )
-
-    spc = module(field, includes, typeName, constructor, diameterMethod, updateMethod,
-                storage=storage,
-                ctorArgs=[view, agglomerate, order, basisChoice, rotatedBB])
-    addStorage(spc, storage)
-    return spc.as_ufl()
-
-#########################################################
-
-def divFreeSpace(view, order=1, conforming=True,
-             field="double", storage="numpy",
-             basisChoice=2, edgeInterpolation=False, rotatedBB=True):
-    """create a virtual element space over an agglomerated grid
-
-    Args:
-        view: the underlying grid view
-        order: polynomial order of the finite element functions
-        field: field of the range space
-        storage: underlying linear algebra backend
-
-    Returns:
-        Space: the constructed Space
-    """
-
-    from dune.fem.space import module, addStorage
-
-    if order < 0:
-        raise KeyError(\
-            "Parameter error in DiscontinuousGalerkinSpace with "+
-            "order=" + str(order) + ": " +\
-            "order has to be greater or equal to 0")
-
-    agglomerate = view.hierarchicalGrid.agglomerate
-
-    includes = [ "dune/fem/gridpart/common/gridpart.hh", "dune/vem/space/divfree.hh" ] + view.cppIncludes
-    dimw = view.dimWorld
-    viewType = view.cppTypeName
-
-    gridPartName = "Dune::FemPy::GridPart< " + view.cppTypeName + " >"
-    typeName = "Dune::Vem::DivFreeVEMSpace< " + gridPartName + " >"
-    constructor = Constructor(
-                   ['pybind11::handle gridView',
-                    'const pybind11::object agglomerate',
-                    'unsigned int order', 'bool conforming',
-                    'int basisChoice','bool edgeInterpolation','bool rotatedBB'],
-                   ['typedef Dune::Vem::Agglomeration<' + gridPartName + '> AggloType;',
-                    'AggloType *agglo = nullptr;',
-                    '// check storage',
-                    'pybind11::function retrieve = pybind11::module::import("dune.vem.vem").attr("retrieveAgglo_");',
-                    'pybind11::function insert   = pybind11::module::import("dune.vem.vem").attr("insertAgglo_");',
-                    'pybind11::function remove   = pybind11::module::import("dune.vem.vem").attr("removeAgglo_");',
-                    'pybind11::handle aggloExists = retrieve(gridView);',
-                    'if (! pybind11::isinstance<pybind11::none>(aggloExists) ) {',
-                    '  // std::cout << "retrieve agglo\\n";',
-                    '  agglo = static_cast<AggloType*>(aggloExists.cast<void*>());',
-                    '}',
-                    'else {',
-                    '  agglo = new AggloType(',
-                    '           Dune::FemPy::gridPart<' + viewType + '>(gridView),rotatedBB,',
-                    '      [agglomerate](const auto& idx)',
-                    '      { return agglomerate(idx).template cast<unsigned int>(); } );',
-                    '  insert(gridView,(void*)agglo);',
-                    '  pybind11::cpp_function aggloCleanup(',
-                    '        [agglo,remove](pybind11::handle weakref) {',
-                    '        // std::cout << "remove agglo\\n";',
-                    '        remove((void*)agglo);',
-                    '        delete agglo;',
-                    '        weakref.dec_ref();',
-                    '    });',
-                    '  (void) pybind11::weakref(gridView, aggloCleanup).release();',
-                    '  // std::cout << "new agglo\\n";',
-                    '}',
-                    'auto obj = new DuneType(*agglo, order, conforming, basisChoice, edgeInterpolation );',
-                    'return obj;'],
-                   ['"gridView"_a', '"agglomerate"_a',
-                    '"order"_a', '"conforming"_a',
-                    '"basisChoice"_a', '"edgeInterpolation"_a','"rotatedBB"_a',
-                    'pybind11::keep_alive< 1, 2 >()'] )
-    diameterMethod = Method('diameters',
-       '''[]( DuneType &self ) { return self.blockMapper().indexSet().diameters(); }''' )
-    updateMethod = Method('update',
-       '''[]( DuneType &self ) { self.update(); }''' )
-
-    spc = module(field, includes, typeName, constructor, diameterMethod, updateMethod,
-                storage=storage,
-                ctorArgs=[view, agglomerate, order, conforming, basisChoice, edgeInterpolation, rotatedBB])
-    addStorage(spc, storage)
-    return spc.as_ufl()
-
-#########################################################
 #########################################################
 
 # from dune.fem.model import elliptic
 from dune.fem.model import integrands
 from dune.vem.patch import transform
-from dune.fem.model import warnNewCartesianIds
 
 def vemModel(view, equation, space,
         hessStabilization=None,gradStabilization=None, massStabilization=None,
         *args, **kwargs):
-    warnNewCartesianIds(view,*args)
     return integrands(view, equation,
                       modelPatch=transform(space,hessStabilization,gradStabilization,massStabilization),
                       includes=["dune/vem/py/integrands.hh"],
                       *args, **kwargs)
 
 def vemScheme(model, space=None, solver=None, parameters={},
               hessStabilization=None, gradStabilization=None, massStabilization=None,
@@ -707,19 +533,15 @@
     return grid
 
 # http://zderadicka.eu/voronoi-diagrams/
 from dune.vem.voronoi import triangulated_voronoi
 from scipy.spatial import Voronoi, voronoi_plot_2d, cKDTree, Delaunay
 import numpy
 
-try:
-    import triangle
-except ImportError:
-    triangle = None
-
+import triangle
 from sortedcontainers import SortedDict
 import matplotlib.pyplot as plt
 class PolyAgglomerate:
     def __init__(self,grid,index):
         indexSet = grid.indexSet
         self.polys = numpy.zeros(grid.size(0),int)
         self.size = 0
@@ -729,21 +551,14 @@
             self.size = max(self.size,idx+1)
 
     def __call__(self,idx):
         return self.polys[idx]
     def roundBary(a):
         return tuple(round(aa,8) for aa in a)
     def construct(cubes,convex,vertices,polygons):
-        if not triangle and not convex:
-            raise ValueError("""
-a grid with non convex polygons requires the 'triangle' package.
-Run 'pip install triangle' and try again.
-Note that 'convex=False' is the default - if all your polygons are convex
-change the parameter to 'True' which will also speedup the grid construction.
-""")
         index = SortedDict()
         if cubes:
             for i,poly in enumerate(polygons):
                 assert len(poly)==4
                 bary = [sum([vertices[p][i] for p in poly]) / 4 for i in range(2)]
                 index[PolyAgglomerate.roundBary(bary)] = i
                 polygons[i][2], polygons[i][3] = poly[3], poly[2]
@@ -783,27 +598,18 @@
         grid = aluSimplexGrid(domain)
     agglomerate = PolyAgglomerate(grid,index)
     agglomerate.minEdgeNumber = min([len(p) for p in constructor["polygons"]])
     grid.hierarchicalGrid.agglomerate = agglomerate
     return grid
 
 def polyGrid(constructor,cubes=False, convex=None,**kwargs):
-    from dune.alugrid import ALUGridEnvVar
-    verbosity = ALUGridEnvVar('ALUGRID_VERBOSITY_LEVEL', 0)
     if isinstance(constructor,dict) and constructor.get("polygons",None) is not None:
         grid = polyAgglomerate(constructor,cubes,convex)
     else:
         grid = trivialAgglomerate(constructor, cubes, **kwargs)
-    # in case of a carteisan domain store if old or new boundary ids was used
-    # this can be removed in later version - it is only used in dune-fem
-    # to give a warning that the boundary ids for the cartesian domains have changed
-    try:
-        grid.hierarchicalGrid._cartesianConstructionWithIds = constructor.boundaryWasSet
-    except AttributeError:
-        pass
     return grid
 
 import weakref
 agglomerationStorage_ = weakref.WeakKeyDictionary()
 def removeAgglo_(agglo):
     for key, value in agglomerationStorage_.items():
         if value == agglo:
```

### Comparing `dune-vem-2.9.0rc1/python/dune/vem/voronoi.py` & `dune-vem-2.9.dev20220529/python/dune/vem/voronoi.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,38 +37,16 @@
     except AttributeError:
         pass
     lowerleft  = numpy.array(constructor[0])
     upperright = numpy.array(constructor[1])
     bounding_box = numpy.array(
             [lowerleft[0],upperright[0],lowerleft[1],upperright[1]] )
 
-    if isinstance(towers,(int,numpy.integer)):
-        # new mechanism only uses `load` to store the file name (or set to None/False)
-        if isinstance(load, str):
-            assert fileName is None, "new load mechanism uses `load` parameter as file name. Do not use the `fileName` at the same time"
-            load = load + str(towers) + '.pickle'
-            if os.path.exists(load):
-                with open(load, 'rb') as f:
-                    ret = pickle.load(f)
-                # make sure old pickle files still work:
-                try:
-                    v = ret["vertices"]
-                    return ret
-                except IndexError:
-                    towers = ret
-            else:
-                towers = numpy.array(
-                        [ p*(upperright-lowerleft) + lowerleft
-                            for p in numpy.random.rand(towers, 2) ])
-        elif fileName:
-            print("""
-Deprecation warning: calling `voronoiCells` with the `fileName ` parameter is deprecated.
-The file name should now be provided using the `load` parameter, i.e., instead of
-`load=True,fileName="voronoi"` use `load="voronoi".
-""")
+    if isinstance(towers,int):
+        if fileName:
             fileName = fileName + str(towers) + '.pickle'
             if not load or not os.path.exists(fileName):
                 # print("generating new seeds for voronoi grid")
                 numpy.random.seed(1234)
                 towers = numpy.array(
                         [ p*(upperright-lowerleft) + lowerleft
                             for p in numpy.random.rand(towers, 2) ])
@@ -132,24 +110,26 @@
                 if not(bounding_box[0] - eps <= x and x <= bounding_box[1] + eps and
                        bounding_box[2] - eps <= y and y <= bounding_box[3] + eps):
                     flag = False
                     break
         if region != [] and flag:
             regions.append(region)
 
-    assert isinstance(lloyd,int)
     if lloyd > 0:
+        dist = 0
         seeds = []
         for i,r in enumerate(regions):
+            # old = seeds[i].copy()
+            # new = centroid(vor.vertices[r])
+            # dist = max(dist,numpy.linalg.norm(new-old))
             seeds.append(centroid(vor.vertices[r]))
-        ret = voronoiCells(constructor, seeds, fileName=None, load=False, lloyd=lloyd-1, show=show)
-        if isinstance(load, str):
-            with open(load, 'wb') as f:
-                pickle.dump(ret, f)
-        return ret
+        if type(lloyd) == int:
+            return voronoiCells(constructor, seeds, fileName=None, load=False, lloyd=lloyd-1, show=show)
+        elif dist > lloyd:
+            return voronoiCells(constructor, towers, fileName=None, load=False, lloyd=lloyd, show=show)
 
     lowerleft  = numpy.array(constructor[0])
     upperright = numpy.array(constructor[1])
     bounding_box = numpy.array(
             [lowerleft[0],upperright[0],lowerleft[1],upperright[1]] )
 
     indices = set()
```

### Comparing `dune-vem-2.9.0rc1/python/dune_vem.egg-info/PKG-INFO` & `dune-vem-2.9.dev20220529/python/dune_vem.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-vem
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Implementation of a number of virtual element spaces and bilinear forms
 Home-page: https://gitlab.dune-project.org/dune-fem/dune-vem
 Author: Andreas Dedner
 Author-email: a.s.dedner@warwick.ac.uk
 License: UNKNOWN
 Description: Preparing the Sources
         =========================
@@ -59,15 +59,15 @@
         
         for further options.
         
         
         The full build-system is described in the dune-common/doc/buildsystem (Git version) or under share/doc/dune-common/buildsystem if you installed DUNE!
         
         
-        git-ebed1814cbfb128fa8b3fd6ae1061263d3eb653e
+        git-b8e7da0a28e5a215676202b5b80fda0bd32a9191
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-vem-2.9.0rc1/python/dune_vem.egg-info/SOURCES.txt` & `dune-vem-2.9.dev20220529/python/dune_vem.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .gitignore
-.gitlab-ci.yml
 CMakeLists.txt
 README.md
 config.h.cmake
 dune-vem.pc.in
 dune.module
 pyproject.toml
 setup.py
@@ -87,37 +86,19 @@
 dune/vem/operator/constraints/CMakeLists.txt
 dune/vem/operator/constraints/dirichlet.hh
 dune/vem/operator/constraints/noconstraints.hh
 dune/vem/py/CMakeLists.txt
 dune/vem/py/integrands.hh
 dune/vem/space/CMakeLists.txt
 dune/vem/space/basisfunctionset.hh
-dune/vem/space/curlfree.hh
 dune/vem/space/default.hh
-dune/vem/space/divfree.hh
 dune/vem/space/hk.hh
 dune/vem/space/indexset.hh
 dune/vem/space/interpolate.hh
-dune/vem/space/interpolation.hh
 dune/vem/space/test.hh
-dune/vem/test/CMakeLists.txt
-dune/vem/test/biharmonic.py
-dune/vem/test/curlfree.py
-dune/vem/test/divfree.py
-dune/vem/test/elliptic.py
-dune/vem/test/hk.py
-dune/vem/test/hk_laplace.py
-dune/vem/test/interpolate.py
-dune/vem/test/perturbation.py
-dune/vem/test/script.py
-dune/vem/test/threadedgenerator.py
-dune/vem/test/uzawa.py
-dune/vem/test/varyingcoeff.py
-dune/vem/test/voronoiseeds368.pickle
-dune/vem/test/voronoiseeds92.pickle
 lib/CMakeLists.txt
 notMaintained/CMakeLists.txt
 notMaintained/dune-vem.cc
 notMaintained/test-Pk.cc
 notMaintained/test-dgspace.cc
 notMaintained/test-dmatrix.cc
 notMaintained/test-gmsh.cc
@@ -288,32 +269,24 @@
 notMaintained/quasilinear-test/data/fem-parameter
 notMaintained/quasilinear-test/data/pmesh-16x16-quads.msh
 notMaintained/quasilinear-test/data/pmesh-16x16-trias.msh
 notMaintained/quasilinear-test/data/pmesh-4x4-quads.msh
 notMaintained/quasilinear-test/data/pmesh-agg-trias-4x4.msh
 notMaintained/quasilinear-test/data/unit-square-one-partition.msh
 notMaintained/quasilinear-test/data/vem-parameter
-pydemo/Hdivspace
 pydemo/biharmonic.py
 pydemo/conditioning.py
 pydemo/conditioning.sh
-pydemo/cylinderSplit.py
-pydemo/cylinderUzawa.py
-pydemo/divfree.py
-pydemo/divfree2.py
-pydemo/hktest.py
 pydemo/interpolation.py
-pydemo/mixed.py
 pydemo/parameter
 pydemo/plotInterpolation.py
-pydemo/script.py
 pydemo/testelliptic.py
-pydemo/testingscript.py
 pydemo/uzawa.py
 pydemo/vemdemo.py
+pydemo/vemtest.py
 pydemo/wilmore.py
 pydemo/oldScript/demoA.py
 pydemo/oldScript/elasticity.py
 pydemo/oldScript/elliptic.py
 python/CMakeLists.txt
 python/dune/CMakeLists.txt
 python/dune/vem/CMakeLists.txt
@@ -321,20 +294,14 @@
 python/dune/vem/__main__.py
 python/dune/vem/bbox.py
 python/dune/vem/min_bounding_rect.py
 python/dune/vem/patch.py
 python/dune/vem/qhull_2d.py
 python/dune/vem/vem.py
 python/dune/vem/voronoi.py
-python/dune/vem/tutorial/CMakeLists.txt
 python/dune/vem/tutorial/__init__.py
-python/dune/vem/tutorial/cylinderUzawa.py
-python/dune/vem/tutorial/laplace.py
-python/dune/vem/tutorial/mixedSolver.py
-python/dune/vem/tutorial/uzawa.py
 python/dune/vem/tutorial/vemdemo.py
-python/dune/vem/tutorial/willmore.py
 python/dune_vem.egg-info/PKG-INFO
 python/dune_vem.egg-info/SOURCES.txt
 python/dune_vem.egg-info/dependency_links.txt
 python/dune_vem.egg-info/requires.txt
 python/dune_vem.egg-info/top_level.txt
```

