# Comparing `tmp/sdss_kaiju-1.4.0b4.tar.gz` & `tmp/sdss_kaiju-1.4.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_kaiju-1.4.0b4.tar", last modified: Mon May  6 05:52:57 2024, max compression
+gzip compressed data, was "sdss_kaiju-1.4.0b5.tar", last modified: Mon May  6 06:03:28 2024, max compression
```

## Comparing `sdss_kaiju-1.4.0b4.tar` & `sdss_kaiju-1.4.0b5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.271085 sdss_kaiju-1.4.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 05:52:57.271085 sdss_kaiju-1.4.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.263085 sdss_kaiju-1.4.0b4/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.267085 sdss_kaiju-1.4.0b4/python/kaiju/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.267085 sdss_kaiju-1.4.0b4/python/kaiju/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/etc/fiducialCoords.csv
--rw-r--r--   0 runner    (1001) docker     (127)    19309 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/etc/fps_DesignReference.txt
--rw-r--r--   0 runner    (1001) docker     (127)    49750 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/etc/positionerTable.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/etc/robotGrid.html
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/etc/robotGrid.js
--rw-r--r--   0 runner    (1001) docker     (127)    42610 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/etc/wokCoords.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.267085 sdss_kaiju-1.4.0b4/python/kaiju/include/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/include/fiducial.h
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/include/gfa.h
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/include/robot.h
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/include/robotGrid.h
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/include/target.h
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/include/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/robotGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/python/kaiju/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.271085 sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 05:52:57.000000 sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-06 05:52:57.000000 sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 05:52:57.000000 sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 05:52:57.000000 sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 05:52:57.000000 sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 05:52:57.271085 sdss_kaiju-1.4.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.271085 sdss_kaiju-1.4.0b4/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/cKaiju.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/fiducial.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/gfa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/robot.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    50832 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/robotGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/target.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/src/utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 05:52:57.271085 sdss_kaiju-1.4.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_collide.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_explode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_fiducial.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_gfaCollision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_initGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_offlineRobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_pathGen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_robotGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_rotGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_rotPath.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_unevenCBs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-06 05:52:26.000000 sdss_kaiju-1.4.0b4/tests/test_updatedGrids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.120143 sdss_kaiju-1.4.0b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 06:03:28.120143 sdss_kaiju-1.4.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.108143 sdss_kaiju-1.4.0b5/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.112143 sdss_kaiju-1.4.0b5/python/kaiju/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.112143 sdss_kaiju-1.4.0b5/python/kaiju/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/etc/fiducialCoords.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19309 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/etc/fps_DesignReference.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    49750 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/etc/positionerTable.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/etc/robotGrid.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/etc/robotGrid.js
+-rw-r--r--   0 runner    (1001) docker     (127)    42610 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/etc/wokCoords.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.112143 sdss_kaiju-1.4.0b5/python/kaiju/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/include/fiducial.h
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/include/gfa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/include/robot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/include/robotGrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/include/target.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/include/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44501 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/robotGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/python/kaiju/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.116143 sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-06 06:03:28.000000 sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-06 06:03:28.000000 sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:03:28.000000 sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 06:03:28.000000 sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 06:03:28.000000 sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:03:28.120143 sdss_kaiju-1.4.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.116143 sdss_kaiju-1.4.0b5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/cKaiju.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/fiducial.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/gfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/robot.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    50832 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/robotGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/target.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/src/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:28.116143 sdss_kaiju-1.4.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_collide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_explode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_fiducial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_gfaCollision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_initGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_offlineRobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_pathGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_robotGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_rotGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_rotPath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_unevenCBs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-06 06:02:59.000000 sdss_kaiju-1.4.0b5/tests/test_updatedGrids.py
```

### Comparing `sdss_kaiju-1.4.0b4/LICENSE.md` & `sdss_kaiju-1.4.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/PKG-INFO` & `sdss_kaiju-1.4.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-kaiju
-Version: 1.4.0b4
+Version: 1.4.0b5
 Summary: Collision Avoidance for SDSS-V Positioners
 Home-page: https://github.com/sdss/kaiju
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD3
 Keywords: astronomy software
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/etc/fiducialCoords.csv` & `sdss_kaiju-1.4.0b5/python/kaiju/etc/fiducialCoords.csv`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/etc/fps_DesignReference.txt` & `sdss_kaiju-1.4.0b5/python/kaiju/etc/fps_DesignReference.txt`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/etc/positionerTable.csv` & `sdss_kaiju-1.4.0b5/python/kaiju/etc/positionerTable.csv`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/etc/robotGrid.html` & `sdss_kaiju-1.4.0b5/python/kaiju/etc/robotGrid.html`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/etc/robotGrid.js` & `sdss_kaiju-1.4.0b5/python/kaiju/etc/robotGrid.js`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/etc/wokCoords.csv` & `sdss_kaiju-1.4.0b5/python/kaiju/etc/wokCoords.csv`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/include/robot.h` & `sdss_kaiju-1.4.0b5/python/kaiju/include/robot.h`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/include/robotGrid.h` & `sdss_kaiju-1.4.0b5/python/kaiju/include/robotGrid.h`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/include/target.h` & `sdss_kaiju-1.4.0b5/python/kaiju/include/target.h`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/include/utils.h` & `sdss_kaiju-1.4.0b5/python/kaiju/include/utils.h`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/robotGrid.py` & `sdss_kaiju-1.4.0b5/python/kaiju/robotGrid.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/kaiju/utils.py` & `sdss_kaiju-1.4.0b5/python/kaiju/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/PKG-INFO` & `sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-kaiju
-Version: 1.4.0b4
+Version: 1.4.0b5
 Summary: Collision Avoidance for SDSS-V Positioners
 Home-page: https://github.com/sdss/kaiju
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD3
 Keywords: astronomy software
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sdss_kaiju-1.4.0b4/python/sdss_kaiju.egg-info/SOURCES.txt` & `sdss_kaiju-1.4.0b5/python/sdss_kaiju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/setup.py` & `sdss_kaiju-1.4.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/Makefile` & `sdss_kaiju-1.4.0b5/src/Makefile`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/cKaiju.cpp` & `sdss_kaiju-1.4.0b5/src/cKaiju.cpp`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/main.cpp` & `sdss_kaiju-1.4.0b5/src/main.cpp`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/robot.cpp` & `sdss_kaiju-1.4.0b5/src/robot.cpp`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/robotGrid.cpp` & `sdss_kaiju-1.4.0b5/src/robotGrid.cpp`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/target.cpp` & `sdss_kaiju-1.4.0b5/src/target.cpp`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/src/utils.cpp` & `sdss_kaiju-1.4.0b5/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_collide.py` & `sdss_kaiju-1.4.0b5/tests/test_collide.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_explode.py` & `sdss_kaiju-1.4.0b5/tests/test_explode.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_fiducial.py` & `sdss_kaiju-1.4.0b5/tests/test_fiducial.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_gfaCollision.py` & `sdss_kaiju-1.4.0b5/tests/test_gfaCollision.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_initGrid.py` & `sdss_kaiju-1.4.0b5/tests/test_initGrid.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_memory.py` & `sdss_kaiju-1.4.0b5/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_offlineRobots.py` & `sdss_kaiju-1.4.0b5/tests/test_offlineRobots.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_pathGen.py` & `sdss_kaiju-1.4.0b5/tests/test_pathGen.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_robotGrid.py` & `sdss_kaiju-1.4.0b5/tests/test_robotGrid.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_rotGrid.py` & `sdss_kaiju-1.4.0b5/tests/test_rotGrid.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_rotPath.py` & `sdss_kaiju-1.4.0b5/tests/test_rotPath.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_target.py` & `sdss_kaiju-1.4.0b5/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_unevenCBs.py` & `sdss_kaiju-1.4.0b5/tests/test_unevenCBs.py`

 * *Files identical despite different names*

### Comparing `sdss_kaiju-1.4.0b4/tests/test_updatedGrids.py` & `sdss_kaiju-1.4.0b5/tests/test_updatedGrids.py`

 * *Files identical despite different names*

