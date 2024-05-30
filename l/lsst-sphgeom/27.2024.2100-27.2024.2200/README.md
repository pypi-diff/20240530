# Comparing `tmp/lsst_sphgeom-27.2024.2100.tar.gz` & `tmp/lsst_sphgeom-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_sphgeom-27.2024.2100.tar", last modified: Thu May 23 10:09:01 2024, max compression
+gzip compressed data, was "lsst_sphgeom-27.2024.2200.tar", last modified: Thu May 30 09:56:39 2024, max compression
```

## Comparing `lsst_sphgeom-27.2024.2100.tar` & `lsst_sphgeom-27.2024.2200.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.986069 lsst_sphgeom-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-23 10:09:01.986069 lsst_sphgeom-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/bsd_license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/gpl-v3.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.958069 lsst_sphgeom-27.2024.2100/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.962069 lsst_sphgeom-27.2024.2100/include/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.970069 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Angle.h
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/AngleInterval.h
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/BigInteger.h
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Box.h
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Box3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Chunker.h
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Circle.h
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/CompoundRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/ConvexPolygon.h
--rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Ellipse.h
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/HtmPixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Interval.h
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Interval1d.h
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/LonLat.h
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Matrix3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Mq3cPixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/NormalizedAngle.h
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/NormalizedAngleInterval.h
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Pixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Q3cPixelization.h
--rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/RangeSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Region.h
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Relationship.h
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/UnitVector3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Vector3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/codec.h
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/curve.h
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/orientation.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.970069 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/interval.h
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/relationship.h
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python.h
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.962069 lsst_sphgeom-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.970069 lsst_sphgeom-27.2024.2100/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.974069 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_angle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_angleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_box.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_box3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_chunker.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_circle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_compoundRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_continue_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_convexPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_curve.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_ellipse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_healpixPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_htmPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_interval1d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_lonLat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_matrix3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_mq3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_normalizedAngle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_normalizedAngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_orientation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_pixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_q3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_rangeSet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_region.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_relationship.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_sphgeom.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_unitVector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_vector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/pixelization_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.986069 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:09:01.000000 lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 10:09:01.986069 lsst_sphgeom-27.2024.2100/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.982069 lsst_sphgeom-27.2024.2100/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Angle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/AngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/BigInteger.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Box.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Box3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Chunker.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Circle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/CompoundRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/ConvexPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/ConvexPolygonImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Ellipse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/HtmPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Interval1d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/LonLat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Matrix3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Mq3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/NormalizedAngle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/NormalizedAngleInterval.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/PixelFinder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Q3cPixelization.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Q3cPixelizationImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/RangeSet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Region.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/UnitVector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/Vector3d.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/orientation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/src/utils.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:01.986069 lsst_sphgeom-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_AngleIntervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Box3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Chunker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_CompoundRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_ConvexPolygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_HealpixPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_HtmPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Interval1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_LonLat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Matrix3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Mq3cPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_NormalizedAngle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Q3cPixelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_RangeSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_UnitVector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_Vector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-23 10:08:53.000000 lsst_sphgeom-27.2024.2100/tests/test_ivoa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.894026 lsst_sphgeom-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-30 09:56:39.890026 lsst_sphgeom-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/bsd_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/gpl-v3.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.866026 lsst_sphgeom-27.2024.2200/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.866026 lsst_sphgeom-27.2024.2200/include/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.874026 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Angle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/AngleInterval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/BigInteger.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Box.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Box3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Chunker.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Circle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/CompoundRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/ConvexPolygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Ellipse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/HtmPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Interval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Interval1d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/LonLat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Matrix3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Mq3cPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/NormalizedAngle.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/NormalizedAngleInterval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Pixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Q3cPixelization.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/RangeSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Region.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Relationship.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/UnitVector3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Vector3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/codec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/orientation.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.874026 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/interval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/relationship.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.866026 lsst_sphgeom-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.874026 lsst_sphgeom-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.882026 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_angle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_angleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_box.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_box3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_chunker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_circle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_compoundRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_continue_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_convexPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_curve.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_ellipse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_healpixPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_htmPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_interval1d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_lonLat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_matrix3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_mq3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_normalizedAngle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_normalizedAngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_orientation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_pixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_q3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_rangeSet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_region.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_relationship.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_sphgeom.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_unitVector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_vector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/pixelization_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.890026 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:56:39.000000 lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 09:56:39.894026 lsst_sphgeom-27.2024.2200/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.886026 lsst_sphgeom-27.2024.2200/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Angle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/AngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/BigInteger.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Box.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Box3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Chunker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Circle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/CompoundRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/ConvexPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/ConvexPolygonImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Ellipse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/HtmPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Interval1d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/LonLat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Matrix3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Mq3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/NormalizedAngle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/NormalizedAngleInterval.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/PixelFinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Q3cPixelization.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Q3cPixelizationImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/RangeSet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Region.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/UnitVector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/Vector3d.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/orientation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/src/utils.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:39.890026 lsst_sphgeom-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_AngleIntervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Box3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Chunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_CompoundRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_ConvexPolygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_HealpixPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_HtmPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Interval1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_LonLat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Matrix3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Mq3cPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_NormalizedAngle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Q3cPixelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_RangeSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_UnitVector3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_Vector3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-30 09:56:28.000000 lsst_sphgeom-27.2024.2200/tests/test_ivoa.py
```

### Comparing `lsst_sphgeom-27.2024.2100/PKG-INFO` & `lsst_sphgeom-27.2024.2200/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-sphgeom
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: A spherical geometry library.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/sphgeom
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_sphgeom-27.2024.2100/README.md` & `lsst_sphgeom-27.2024.2200/README.md`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/bsd_license.txt` & `lsst_sphgeom-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/gpl-v3.0.txt` & `lsst_sphgeom-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Angle.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Angle.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/AngleInterval.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/AngleInterval.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/BigInteger.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/BigInteger.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Box.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Box.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Box3d.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Box3d.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Chunker.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Chunker.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Circle.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Circle.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/CompoundRegion.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/CompoundRegion.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/ConvexPolygon.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/ConvexPolygon.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Ellipse.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Ellipse.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/HtmPixelization.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/HtmPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Interval.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Interval.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Interval1d.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Interval1d.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/LonLat.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/LonLat.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Matrix3d.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Matrix3d.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Mq3cPixelization.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Mq3cPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/NormalizedAngle.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/NormalizedAngle.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/NormalizedAngleInterval.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/NormalizedAngleInterval.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Pixelization.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Pixelization.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Q3cPixelization.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Q3cPixelization.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/RangeSet.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/RangeSet.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Region.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Region.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Relationship.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Relationship.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/UnitVector3d.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/UnitVector3d.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/Vector3d.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/Vector3d.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/codec.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/codec.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/constants.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/constants.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/curve.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/curve.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/orientation.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/orientation.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/interval.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/interval.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/relationship.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/relationship.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python/utils.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python/utils.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/python.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/python.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/include/lsst/sphgeom/utils.h` & `lsst_sphgeom-27.2024.2200/include/lsst/sphgeom/utils.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/pyproject.toml` & `lsst_sphgeom-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/__init__.py` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_angle.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_angle.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_angleInterval.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_angleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_box.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_box.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_box3d.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_box3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_chunker.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_chunker.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_circle.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_circle.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_compoundRegion.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_compoundRegion.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_continue_class.py` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_continue_class.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_convexPolygon.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_convexPolygon.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_curve.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_curve.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_ellipse.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_ellipse.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_healpixPixelization.py` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_healpixPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_htmPixelization.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_htmPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_interval1d.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_interval1d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_lonLat.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_lonLat.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_matrix3d.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_matrix3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_mq3cPixelization.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_mq3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_normalizedAngle.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_normalizedAngle.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_normalizedAngleInterval.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_normalizedAngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_orientation.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_orientation.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_pixelization.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_pixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_q3cPixelization.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_q3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_rangeSet.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_rangeSet.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_region.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_region.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_relationship.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_relationship.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_sphgeom.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_sphgeom.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_unitVector3d.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_unitVector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_utils.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_utils.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_vector3d.cc` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_vector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/_yaml.py` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst/sphgeom/pixelization_abc.py` & `lsst_sphgeom-27.2024.2200/python/lsst/sphgeom/pixelization_abc.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/PKG-INFO` & `lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-sphgeom
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: A spherical geometry library.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/sphgeom
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_sphgeom-27.2024.2100/python/lsst_sphgeom.egg-info/SOURCES.txt` & `lsst_sphgeom-27.2024.2200/python/lsst_sphgeom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/setup.py` & `lsst_sphgeom-27.2024.2200/setup.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Angle.cc` & `lsst_sphgeom-27.2024.2200/src/Angle.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/AngleInterval.cc` & `lsst_sphgeom-27.2024.2200/src/AngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/BigInteger.cc` & `lsst_sphgeom-27.2024.2200/src/BigInteger.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Box.cc` & `lsst_sphgeom-27.2024.2200/src/Box.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Box3d.cc` & `lsst_sphgeom-27.2024.2200/src/Box3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Chunker.cc` & `lsst_sphgeom-27.2024.2200/src/Chunker.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Circle.cc` & `lsst_sphgeom-27.2024.2200/src/Circle.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/CompoundRegion.cc` & `lsst_sphgeom-27.2024.2200/src/CompoundRegion.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/ConvexPolygon.cc` & `lsst_sphgeom-27.2024.2200/src/ConvexPolygon.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/ConvexPolygonImpl.h` & `lsst_sphgeom-27.2024.2200/src/ConvexPolygonImpl.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Ellipse.cc` & `lsst_sphgeom-27.2024.2200/src/Ellipse.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/HtmPixelization.cc` & `lsst_sphgeom-27.2024.2200/src/HtmPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Interval1d.cc` & `lsst_sphgeom-27.2024.2200/src/Interval1d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/LonLat.cc` & `lsst_sphgeom-27.2024.2200/src/LonLat.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Matrix3d.cc` & `lsst_sphgeom-27.2024.2200/src/Matrix3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Mq3cPixelization.cc` & `lsst_sphgeom-27.2024.2200/src/Mq3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/NormalizedAngle.cc` & `lsst_sphgeom-27.2024.2200/src/NormalizedAngle.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/NormalizedAngleInterval.cc` & `lsst_sphgeom-27.2024.2200/src/NormalizedAngleInterval.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/PixelFinder.h` & `lsst_sphgeom-27.2024.2200/src/PixelFinder.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Q3cPixelization.cc` & `lsst_sphgeom-27.2024.2200/src/Q3cPixelization.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Q3cPixelizationImpl.h` & `lsst_sphgeom-27.2024.2200/src/Q3cPixelizationImpl.h`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/RangeSet.cc` & `lsst_sphgeom-27.2024.2200/src/RangeSet.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Region.cc` & `lsst_sphgeom-27.2024.2200/src/Region.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/UnitVector3d.cc` & `lsst_sphgeom-27.2024.2200/src/UnitVector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/Vector3d.cc` & `lsst_sphgeom-27.2024.2200/src/Vector3d.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/orientation.cc` & `lsst_sphgeom-27.2024.2200/src/orientation.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/src/utils.cc` & `lsst_sphgeom-27.2024.2200/src/utils.cc`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Angle.py` & `lsst_sphgeom-27.2024.2200/tests/test_Angle.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_AngleIntervals.py` & `lsst_sphgeom-27.2024.2200/tests/test_AngleIntervals.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Box.py` & `lsst_sphgeom-27.2024.2200/tests/test_Box.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Box3d.py` & `lsst_sphgeom-27.2024.2200/tests/test_Box3d.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Chunker.py` & `lsst_sphgeom-27.2024.2200/tests/test_Chunker.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Circle.py` & `lsst_sphgeom-27.2024.2200/tests/test_Circle.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_CompoundRegion.py` & `lsst_sphgeom-27.2024.2200/tests/test_CompoundRegion.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_ConvexPolygon.py` & `lsst_sphgeom-27.2024.2200/tests/test_ConvexPolygon.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Ellipse.py` & `lsst_sphgeom-27.2024.2200/tests/test_Ellipse.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_HealpixPixelization.py` & `lsst_sphgeom-27.2024.2200/tests/test_HealpixPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_HtmPixelization.py` & `lsst_sphgeom-27.2024.2200/tests/test_HtmPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Interval1d.py` & `lsst_sphgeom-27.2024.2200/tests/test_Interval1d.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_LonLat.py` & `lsst_sphgeom-27.2024.2200/tests/test_LonLat.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Matrix3d.py` & `lsst_sphgeom-27.2024.2200/tests/test_Matrix3d.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Mq3cPixelization.py` & `lsst_sphgeom-27.2024.2200/tests/test_Mq3cPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_NormalizedAngle.py` & `lsst_sphgeom-27.2024.2200/tests/test_NormalizedAngle.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Q3cPixelization.py` & `lsst_sphgeom-27.2024.2200/tests/test_Q3cPixelization.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_RangeSet.py` & `lsst_sphgeom-27.2024.2200/tests/test_RangeSet.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_UnitVector3d.py` & `lsst_sphgeom-27.2024.2200/tests/test_UnitVector3d.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_Vector3d.py` & `lsst_sphgeom-27.2024.2200/tests/test_Vector3d.py`

 * *Files identical despite different names*

### Comparing `lsst_sphgeom-27.2024.2100/tests/test_ivoa.py` & `lsst_sphgeom-27.2024.2200/tests/test_ivoa.py`

 * *Files identical despite different names*

