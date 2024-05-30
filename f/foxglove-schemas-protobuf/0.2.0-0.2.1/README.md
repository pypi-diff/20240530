# Comparing `tmp/foxglove-schemas-protobuf-0.2.0.tar.gz` & `tmp/foxglove_schemas_protobuf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-schemas-protobuf-0.2.0.tar", last modified: Fri Nov 17 20:27:34 2023, max compression
+gzip compressed data, was "foxglove_schemas_protobuf-0.2.1.tar", last modified: Thu May 30 19:36:35 2024, max compression
```

## Comparing `foxglove-schemas-protobuf-0.2.0.tar` & `foxglove_schemas_protobuf-0.2.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 20:27:34.883100 foxglove-schemas-protobuf-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-17 20:27:34.883100 foxglove-schemas-protobuf-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-11-17 20:26:50.000000 foxglove-schemas-protobuf-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 20:27:34.883100 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CameraCalibration_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Color_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Color_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedImage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedImage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedVideo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedVideo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CubePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransform_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransform_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransforms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/GeoJSON_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/GeoJSON_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Grid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Grid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/KeyValuePair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LaserScan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LaserScan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LinePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LocationFix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LocationFix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PackedElementField_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PackedElementField_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointCloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointCloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PoseInFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Pose_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Pose_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PosesInFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Quaternion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Quaternion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/RawImage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/RawImage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneUpdate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextAnnotation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-11-17 20:27:27.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 20:26:50.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 20:26:50.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 20:27:34.883100 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-17 20:27:34.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2023-11-17 20:27:34.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 20:27:34.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-17 20:27:34.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-17 20:27:34.000000 foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-17 20:26:50.000000 foxglove-schemas-protobuf-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-11-17 20:27:34.883100 foxglove-schemas-protobuf-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 20:27:34.883100 foxglove-schemas-protobuf-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-17 20:26:50.000000 foxglove-schemas-protobuf-0.2.0/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:35.891683 foxglove_schemas_protobuf-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-30 19:36:35.891683 foxglove_schemas_protobuf-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-30 19:36:03.000000 foxglove_schemas_protobuf-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:35.891683 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CameraCalibration_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Color_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Color_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedImage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedImage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedVideo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedVideo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CubePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransform_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransform_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransforms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/GeoJSON_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/GeoJSON_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Grid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Grid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/KeyValuePair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LaserScan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LaserScan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LinePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LocationFix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LocationFix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PackedElementField_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PackedElementField_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointCloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointCloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PoseInFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Pose_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Pose_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PosesInFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Quaternion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Quaternion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/RawImage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/RawImage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneUpdate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextAnnotation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-30 19:36:28.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:03.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:03.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:35.891683 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-30 19:36:35.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-30 19:36:35.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:36:35.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 19:36:35.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 19:36:35.000000 foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 19:36:03.000000 foxglove_schemas_protobuf-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-30 19:36:35.895683 foxglove_schemas_protobuf-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:35.891683 foxglove_schemas_protobuf-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 19:36:03.000000 foxglove_schemas_protobuf-0.2.1/tests/test_schemas.py
```

### Comparing `foxglove-schemas-protobuf-0.2.0/PKG-INFO` & `foxglove_schemas_protobuf-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-protobuf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Protobuf classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: protobuf>=3.20.0
 
 # Foxglove Schemas (Protobuf)
 
-This package provides [Protobuf](https://developers.google.com/protocol-buffers/) classes for [Foxglove Schemas](https://foxglove.dev/docs/studio/messages/introduction).
+This package provides [Protobuf](https://developers.google.com/protocol-buffers/) classes for [Foxglove Schemas](https://docs.foxglove.dev/docs/visualization/message-schemas/introduction).
 
 ## Installation
 
 Install via [Pipenv](https://pipenv.pypa.io/en/latest/) by adding `foxglove-schemas-protobuf` to your `Pipfile` or via the command line:
 
 ```bash
 pipenv install foxglove-schemas-protobuf
@@ -28,8 +28,8 @@
 
 ```py
 from foxglove_schemas_protobuf.CompressedImage_pb2 import CompressedImage
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `foxglove-schemas-protobuf-0.2.0/README.md` & `foxglove_schemas_protobuf-0.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Foxglove Schemas (Protobuf)
 
-This package provides [Protobuf](https://developers.google.com/protocol-buffers/) classes for [Foxglove Schemas](https://foxglove.dev/docs/studio/messages/introduction).
+This package provides [Protobuf](https://developers.google.com/protocol-buffers/) classes for [Foxglove Schemas](https://docs.foxglove.dev/docs/visualization/message-schemas/introduction).
 
 ## Installation
 
 Install via [Pipenv](https://pipenv.pypa.io/en/latest/) by adding `foxglove-schemas-protobuf` to your `Pipfile` or via the command line:
 
 ```bash
 pipenv install foxglove-schemas-protobuf
@@ -16,8 +16,8 @@
 
 ```py
 from foxglove_schemas_protobuf.CompressedImage_pb2 import CompressedImage
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ArrowPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CameraCalibration_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CameraCalibration_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CameraCalibration_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     width: builtins.int
     """Image width"""
     height: builtins.int
     """Image height"""
     distortion_model: builtins.str
     """Name of distortion model
 
-    Supported values: `plumb_bob` and `rational_polynomial`
+    Supported parameters: `plumb_bob` (k1, k2, p1, p2, k3) and `rational_polynomial` (k1, k2, p1, p2, k3, k4, k5, k6). Distortion models are based on [OpenCV's](https://docs.opencv.org/2.4/modules/calib3d/doc/camera_calibration_and_3d_reconstruction.html) [pinhole camera model](https://en.wikipedia.org/wiki/Distortion_%28optics%29#Software_correction). This is the same [implementation used by ROS](http://docs.ros.org/en/diamondback/api/image_geometry/html/c++/pinhole__camera__model_8cpp_source.html)
     """
     @property
     def D(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Distortion parameters"""
     @property
     def K(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Intrinsic camera matrix (3x3 row-major matrix)
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CircleAnnotation_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     FILL_COLOR_FIELD_NUMBER: builtins.int
     OUTLINE_COLOR_FIELD_NUMBER: builtins.int
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Timestamp of circle"""
     @property
     def position(self) -> foxglove_Point2_pb2.Point2:
-        """Center of the circle in 2D image coordinates (pixels)"""
+        """Center of the circle in 2D image coordinates (pixels).
+        The coordinate uses the top-left corner of the top-left pixel of the image as the origin.
+        """
     diameter: builtins.float
     """Circle diameter in pixels"""
     thickness: builtins.float
     """Line thickness in pixels"""
     @property
     def fill_color(self) -> foxglove_Color_pb2.Color:
         """Fill color"""
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Color_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Color_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Color_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Color_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedImage_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedImage_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedImage_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedImage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedVideo_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedVideo_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CompressedVideo_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CompressedVideo_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """Frame of reference for the video.
 
     The origin of the frame is the optical center of the camera. +x points to the right in the video, +y points down, and +z points into the plane of the video.
     """
     data: builtins.bytes
     """Compressed video frame data.
 
-    For packet-based video codecs this data must begin and end on packet boundaries (no partial packets), and must contain enough video packets to decode exactly one image (either a keyframe or delta frame). Note: Foxglove Studio does not support video streams that include B frames because they require lookahead.
+    For packet-based video codecs this data must begin and end on packet boundaries (no partial packets), and must contain enough video packets to decode exactly one image (either a keyframe or delta frame). Note: Foxglove does not support video streams that include B frames because they require lookahead.
     """
     format: builtins.str
     """Video format.
 
     Supported values: `h264` (Annex B formatted data only)
     """
     def __init__(
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CubePrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CubePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CubePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/CylinderPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransform_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransform_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransform_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransforms_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransforms_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/FrameTransforms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/GeoJSON_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/GeoJSON_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/GeoJSON_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/GeoJSON_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Grid_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Grid_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Grid_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Grid_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ImageAnnotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/KeyValuePair_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/KeyValuePair_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/KeyValuePair_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LaserScan_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LaserScan_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LaserScan_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LaserScan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LinePrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LinePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LinePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LocationFix_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LocationFix_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/LocationFix_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/LocationFix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Log_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Log_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/ModelPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PackedElementField_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PackedElementField_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PackedElementField_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PackedElementField_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point2_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point2_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point2_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point3_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point3_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Point3_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Point3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointCloud_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointCloud_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointCloud_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointCloud_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PointsAnnotation_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,17 @@
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Timestamp of annotation"""
     type: global___PointsAnnotation.Type.ValueType
     """Type of points annotation to draw"""
     @property
     def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_Point2_pb2.Point2]:
-        """Points in 2D image coordinates (pixels)"""
+        """Points in 2D image coordinates (pixels).
+        These coordinates use the top-left corner of the top-left pixel of the image as the origin.
+        """
     @property
     def outline_color(self) -> foxglove_Color_pb2.Color:
         """Outline color"""
     @property
     def outline_colors(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[foxglove_Color_pb2.Color]:
         """Per-point colors, if `type` is `POINTS`, or per-segment stroke colors, if `type` is `LINE_LIST`, `LINE_STRIP` or `LINE_LOOP`."""
     @property
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PoseInFrame_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PoseInFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PoseInFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Pose_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Pose_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Pose_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Pose_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PosesInFrame_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PosesInFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/PosesInFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Quaternion_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Quaternion_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Quaternion_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Quaternion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/RawImage_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/RawImage_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/RawImage_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/RawImage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntityDeletion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntity_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntity_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneEntity_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneEntity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneUpdate_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneUpdate_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SceneUpdate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/SpherePrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextAnnotation_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextAnnotation_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextAnnotation_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     TEXT_COLOR_FIELD_NUMBER: builtins.int
     BACKGROUND_COLOR_FIELD_NUMBER: builtins.int
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Timestamp of annotation"""
     @property
     def position(self) -> foxglove_Point2_pb2.Point2:
-        """Bottom-left origin of the text label in 2D image coordinates (pixels)"""
+        """Bottom-left origin of the text label in 2D image coordinates (pixels).
+        The coordinate uses the top-left corner of the top-left pixel of the image as the origin.
+        """
     text: builtins.str
     """Text to display"""
     font_size: builtins.float
     """Font size in pixels"""
     @property
     def text_color(self) -> foxglove_Color_pb2.Color:
         """Text color"""
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextPrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TextPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/TriangleListPrimitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector2_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector2_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector2_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector3_pb2.py` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector3_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf/Vector3_pb2.pyi` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf/Vector3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/PKG-INFO` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-protobuf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Protobuf classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: protobuf>=3.20.0
 
 # Foxglove Schemas (Protobuf)
 
-This package provides [Protobuf](https://developers.google.com/protocol-buffers/) classes for [Foxglove Schemas](https://foxglove.dev/docs/studio/messages/introduction).
+This package provides [Protobuf](https://developers.google.com/protocol-buffers/) classes for [Foxglove Schemas](https://docs.foxglove.dev/docs/visualization/message-schemas/introduction).
 
 ## Installation
 
 Install via [Pipenv](https://pipenv.pypa.io/en/latest/) by adding `foxglove-schemas-protobuf` to your `Pipfile` or via the command line:
 
 ```bash
 pipenv install foxglove-schemas-protobuf
@@ -28,8 +28,8 @@
 
 ```py
 from foxglove_schemas_protobuf.CompressedImage_pb2 import CompressedImage
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `foxglove-schemas-protobuf-0.2.0/foxglove_schemas_protobuf.egg-info/SOURCES.txt` & `foxglove_schemas_protobuf-0.2.1/foxglove_schemas_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-protobuf-0.2.0/setup.cfg` & `foxglove_schemas_protobuf-0.2.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-schemas-protobuf
-version = 0.2.0
+version = 0.2.1
 description = Protobuf classes for Foxglove Schemas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/schemas
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

