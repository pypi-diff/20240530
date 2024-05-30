# Comparing `tmp/foxglove-schemas-flatbuffer-0.1.0.tar.gz` & `tmp/foxglove_schemas_flatbuffer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-schemas-flatbuffer-0.1.0.tar", last modified: Tue Apr 18 22:45:24 2023, max compression
+gzip compressed data, was "foxglove_schemas_flatbuffer-0.2.0.tar", last modified: Thu May 30 19:36:31 2024, max compression
```

## Comparing `foxglove-schemas-flatbuffer-0.1.0.tar` & `foxglove_schemas_flatbuffer-0.2.0.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-18 22:44:51.000000 foxglove-schemas-flatbuffer-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ByteVector.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ByteVector.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Color.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Color.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Duration.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransforms.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/GeoJSON.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/GeoJSON.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/KeyValuePair.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/KeyValuePair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LineType.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LogLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/NumericType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point2.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point2.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point3.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotationType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PositionCovarianceType.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Quaternion.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextAnnotation.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Time.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector2.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector2.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector3.bfbs
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector3.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 22:45:20.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 22:45:24.000000 foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 22:44:51.000000 foxglove-schemas-flatbuffer-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:45:24.745345 foxglove-schemas-flatbuffer-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 22:44:51.000000 foxglove-schemas-flatbuffer-0.1.0/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:31.831550 foxglove_schemas_flatbuffer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-30 19:36:31.831550 foxglove_schemas_flatbuffer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-30 19:36:03.000000 foxglove_schemas_flatbuffer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:31.831550 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ArrowPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ByteVector.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ByteVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CameraCalibration.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CameraCalibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CircleAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Color.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CompressedImage.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CompressedImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CompressedVideo.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CompressedVideo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CubePrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CubePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CylinderPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Duration.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransform.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransforms.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/GeoJSON.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/GeoJSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Grid.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ImageAnnotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/KeyValuePair.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/KeyValuePair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LaserScan.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LaserScan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LinePrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LinePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LineType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LocationFix.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LocationFix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Log.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LogLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ModelPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/NumericType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PackedElementField.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PackedElementField.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Point2.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Point2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Point3.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Point3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointCloud.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointCloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointsAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointsAnnotationType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Pose.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Pose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PoseInFrame.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PoseInFrame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PosesInFrame.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PosesInFrame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PositionCovarianceType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Quaternion.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/RawImage.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/RawImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntity.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)    15535 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntityDeletionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneUpdate.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SpherePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextAnnotation.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Time.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Vector2.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Vector2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Vector3.bfbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Vector3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 19:36:28.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:31.831550 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-30 19:36:31.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-30 19:36:31.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:36:31.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 19:36:31.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 19:36:31.000000 foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 19:36:03.000000 foxglove_schemas_flatbuffer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-30 19:36:31.831550 foxglove_schemas_flatbuffer-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:36:31.831550 foxglove_schemas_flatbuffer-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-30 19:36:03.000000 foxglove_schemas_flatbuffer-0.2.0/tests/test_schemas.py
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/PKG-INFO` & `foxglove_schemas_flatbuffer-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-flatbuffer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Flatbuffer classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: flatbuffers
 
 # Foxglove Schemas (Flatbuffer)
 
-This package provides [Flatbuffer](https://google.github.io/flatbuffers/) classes for [Foxglove Schemas](https://foxglove.dev/docs/studio/messages/introduction).
+This package provides [Flatbuffer](https://google.github.io/flatbuffers/) classes for [Foxglove Schemas](https://docs.foxglove.dev/docs/visualization/message-schemas/introduction).
 
 ## Installation
 
 Install via [Pipenv](https://pipenv.pypa.io/en/latest/) by adding `foxglove-schemas-flatbuffer` to your `Pipfile` or via the command line:
 
 ```bash
 pipenv install foxglove-schemas-flatbuffer
@@ -42,8 +43,8 @@
 
 # Serialized CompressedImage message
 msg_data = builder.Output()
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/README.md` & `foxglove_schemas_flatbuffer-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Foxglove Schemas (Flatbuffer)
 
-This package provides [Flatbuffer](https://google.github.io/flatbuffers/) classes for [Foxglove Schemas](https://foxglove.dev/docs/studio/messages/introduction).
+This package provides [Flatbuffer](https://google.github.io/flatbuffers/) classes for [Foxglove Schemas](https://docs.foxglove.dev/docs/visualization/message-schemas/introduction).
 
 ## Installation
 
 Install via [Pipenv](https://pipenv.pypa.io/en/latest/) by adding `foxglove-schemas-flatbuffer` to your `Pipfile` or via the command line:
 
 ```bash
 pipenv install foxglove-schemas-flatbuffer
@@ -31,8 +31,8 @@
 
 # Serialized CompressedImage message
 msg_data = builder.Output()
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ArrowPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ArrowPrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ArrowPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ByteVector.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ByteVector.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CameraCalibration.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CameraCalibration.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CameraCalibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Uint32Flags, o + self._tab.Pos)
         return 0
 
     # Name of distortion model
     # 
-    # Supported values: `plumb_bob` and `rational_polynomial`
+    # Supported parameters: `plumb_bob` (k1, k2, p1, p2, k3) and `rational_polynomial` (k1, k2, p1, p2, k3, k4, k5, k6). Distortion models are based on [OpenCV's](https://docs.opencv.org/2.4/modules/calib3d/doc/camera_calibration_and_3d_reconstruction.html) [pinhole camera model](https://en.wikipedia.org/wiki/Distortion_%28optics%29#Software_correction). This is the same [implementation used by ROS](http://docs.ros.org/en/diamondback/api/image_geometry/html/c++/pinhole__camera__model_8cpp_source.html)
     # CameraCalibration
     def DistortionModel(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             return self._tab.String(o + self._tab.Pos)
         return None
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CircleAnnotation.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CircleAnnotation.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CircleAnnotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,16 @@
             x = o + self._tab.Pos
             from .Time import Time
             obj = Time()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
-    # Center of the circle in 2D image coordinates (pixels)
+    # Center of the circle in 2D image coordinates (pixels).
+    # The coordinate uses the top-left corner of the top-left pixel of the image as the origin.
     # CircleAnnotation
     def Position(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             from .Point2 import Point2
             obj = Point2()
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Color.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Color.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CompressedImage.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CompressedImage.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CompressedImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     # CompressedImage
     def DataIsNone(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         return o == 0
 
     # Image format
     # 
-    # Supported values: `webp`, `jpeg`, `png`
+    # Supported values: image media types supported by Chrome, such as `webp`, `jpeg`, `png`
     # CompressedImage
     def Format(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             return self._tab.String(o + self._tab.Pos)
         return None
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CubePrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CubePrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CubePrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/CylinderPrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/CylinderPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Duration.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Duration.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # Duration
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
     # Signed seconds of the span of time. Must be from -315,576,000,000 to +315,576,000,000 inclusive.
     # Duration
     def Sec(self): return self._tab.Get(flatbuffers.number_types.Int32Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(0))
-    # if sec === 0 : -999,999,999 <= nsec <= +999,999,999 
+    # if sec === 0 : -999,999,999 <= nsec <= +999,999,999
     # otherwise sign of sec must match sign of nsec or be 0 and abs(nsec) <= 999,999,999
     # Duration
     def Nsec(self): return self._tab.Get(flatbuffers.number_types.Int32Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(4))
 
 def CreateDuration(builder, sec, nsec):
     builder.Prep(4, 8)
     builder.PrependInt32(nsec)
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransform.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransform.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransform.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransforms.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransforms.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/FrameTransforms.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/FrameTransforms.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/GeoJSON.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/GeoJSON.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Grid.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Grid.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Grid.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ImageAnnotations.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ImageAnnotations.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ImageAnnotations.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/KeyValuePair.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/KeyValuePair.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LaserScan.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LaserScan.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LaserScan.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LinePrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LinePrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LinePrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/LocationFix.bfbs`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,83 @@
-00000000: 1c00 0000 4246 4253 1400 2000 0400 0800  ....BFBS.. .....
-00000010: 0c00 1000 1400 1800 0000 1c00 1400 0000  ................
-00000020: 3800 0000 2c00 0000 2000 0000 1400 0000  8...,... .......
-00000030: c801 0000 0800 0000 2800 0000 0000 0000  ........(.......
+00000000: 2000 0000 4246 4253 0000 0000 1400 2000   ...BFBS...... .
+00000010: 0400 0800 0c00 1000 1400 1800 0000 1c00  ................
+00000020: 1400 0000 3800 0000 2c00 0000 2000 0000  ....8...,... ...
+00000030: 1400 0000 dc01 0000 0800 0000 2c00 0000  ............,...
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0100 0000 4000 0000 0100 0000 9c01 0000  ....@...........
-00000060: 0100 0000 0c00 0000 0800 0c00 0400 0800  ................
-00000070: 0800 0000 9801 0000 0400 0000 0000 0000  ................
-00000080: 0000 1200 1400 0400 0800 0000 0c00 0000  ................
-00000090: 0000 1000 1200 0000 3800 0000 2000 0000  ........8... ...
-000000a0: 0800 0000 6801 0000 40fe ffff 0000 0004  ....h...@.......
-000000b0: 0000 0000 0100 0000 0100 0000 0400 0000  ................
-000000c0: f000 0000 a800 0000 6400 0000 2800 0000  ........d...(...
-000000d0: 1f00 0000 666f 7867 6c6f 7665 2e50 6f73  ....foxglove.Pos
-000000e0: 6974 696f 6e43 6f76 6172 6961 6e63 6554  itionCovarianceT
-000000f0: 7970 6500 d4ff ffff 1c00 0000 0c00 0000  ype.............
-00000100: 0300 0000 0000 0000 4cff ffff 0100 0000  ........L.......
-00000110: 0100 0000 0500 0000 4b4e 4f57 4e00 0000  ........KNOWN...
-00000120: 0c00 1400 0400 0c00 0000 0800 0c00 0000  ................
-00000130: 1c00 0000 0c00 0000 0200 0000 0000 0000  ................
-00000140: 84ff ffff 0100 0000 0100 0000 0e00 0000  ................
-00000150: 4449 4147 4f4e 414c 5f4b 4e4f 574e 0000  DIAGONAL_KNOWN..
-00000160: 0c00 1800 0400 0c00 0000 0800 0c00 0000  ................
-00000170: 2000 0000 1000 0000 0100 0000 0000 0000   ...............
-00000180: 0000 0000 c8ff ffff 0100 0000 0100 0000  ................
-00000190: 0c00 0000 4150 5052 4f58 494d 4154 4544  ....APPROXIMATED
-000001a0: 0000 0000 0c00 0c00 0400 0000 0000 0800  ................
-000001b0: 0c00 0000 2400 0000 1400 0000 1000 0c00  ....$...........
-000001c0: 0000 0000 0000 0000 0400 0800 1000 0000  ................
-000001d0: 0100 0000 0100 0000 0700 0000 554e 4b4e  ............UNKN
-000001e0: 4f57 4e00 1400 1400 0400 0800 0000 0c00  OWN.............
-000001f0: 0000 0000 0000 1000 1400 0000 4000 0000  ............@...
-00000200: 2400 0000 0100 0000 0400 0000 1100 0000  $...............
-00000210: 2f2f 4c6f 6361 7469 6f6e 4669 782e 6662  //LocationFix.fb
-00000220: 7300 0000 0500 0000 e800 0000 5c01 0000  s...........\...
-00000230: 1c01 0000 9400 0000 2000 0000 1400 0000  ........ .......
-00000240: 666f 7867 6c6f 7665 2e4c 6f63 6174 696f  foxglove.Locatio
-00000250: 6e46 6978 0000 0000 18ff ffff 0400 0c00  nFix............
-00000260: 2c00 0000 1400 0000 1000 1400 0700 0000  ,...............
-00000270: 0800 0000 0c00 1000 1000 0000 0000 0004  ................
-00000280: 0000 0000 0100 0000 0100 0000 1800 0000  ................
-00000290: 706f 7369 7469 6f6e 5f63 6f76 6172 6961  position_covaria
-000002a0: 6e63 655f 7479 7065 0000 0000 1c00 1400  nce_type........
-000002b0: 0c00 1000 0800 0a00 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0700 1c00 0000 0000 0001  ................
-000002d0: 0300 0a00 2400 0000 1400 0000 1000 0c00  ....$...........
-000002e0: 0600 0700 0000 0000 0000 0800 1000 0000  ................
-000002f0: 0000 0e0c 0800 0000 1300 0000 706f 7369  ............posi
-00000300: 7469 6f6e 5f63 6f76 6172 6961 6e63 6500  tion_covariance.
-00000310: d0ff ffff 0200 0800 1800 0000 0400 0000  ................
-00000320: 88ff ffff 0000 000c 0800 0000 0100 0000  ................
-00000330: 0800 0000 616c 7469 7475 6465 0000 0000  ....altitude....
-00000340: 0c00 1000 0800 0c00 0400 0600 0c00 0000  ................
-00000350: 0100 0600 1800 0000 0400 0000 c4ff ffff  ................
-00000360: 0000 000c 0800 0000 0100 0000 0900 0000  ................
-00000370: 6c6f 6e67 6974 7564 6500 0000 0c00 1000  longitude.......
-00000380: 0800 0c00 0000 0600 0c00 0000 0000 0400  ................
-00000390: 2800 0000 1400 0000 1000 1000 0700 0000  (...............
-000003a0: 0000 0000 0800 0c00 1000 0000 0000 000c  ................
-000003b0: 0800 0000 0100 0000 0800 0000 6c61 7469  ............lati
-000003c0: 7475 6465 0000 0000                      tude....
+00000050: 0000 0000 0100 0000 5400 0000 0200 0000  ........T.......
+00000060: b001 0000 0c04 0000 0200 0000 1800 0000  ................
+00000070: 0400 0000 84fb ffff 1404 0000 0400 0000  ................
+00000080: 0000 0000 94fb ffff 9c01 0000 0400 0000  ................
+00000090: 0100 0000 f803 0000 0000 1200 1400 0400  ................
+000000a0: 0800 0000 0c00 0000 0000 1000 1200 0000  ................
+000000b0: 3800 0000 2000 0000 0800 0000 6801 0000  8... .......h...
+000000c0: 38fe ffff 0000 0004 0000 0000 0100 0000  8...............
+000000d0: 0100 0000 0400 0000 f000 0000 a800 0000  ................
+000000e0: 6400 0000 2800 0000 1f00 0000 666f 7867  d...(.......foxg
+000000f0: 6c6f 7665 2e50 6f73 6974 696f 6e43 6f76  love.PositionCov
+00000100: 6172 6961 6e63 6554 7970 6500 d4ff ffff  arianceType.....
+00000110: 1c00 0000 0c00 0000 0300 0000 0000 0000  ................
+00000120: 4cff ffff 0100 0000 0100 0000 0500 0000  L...............
+00000130: 4b4e 4f57 4e00 0000 0c00 1400 0400 0c00  KNOWN...........
+00000140: 0000 0800 0c00 0000 1c00 0000 0c00 0000  ................
+00000150: 0200 0000 0000 0000 84ff ffff 0100 0000  ................
+00000160: 0100 0000 0e00 0000 4449 4147 4f4e 414c  ........DIAGONAL
+00000170: 5f4b 4e4f 574e 0000 0c00 1800 0400 0c00  _KNOWN..........
+00000180: 0000 0800 0c00 0000 2000 0000 1000 0000  ........ .......
+00000190: 0100 0000 0000 0000 0000 0000 c8ff ffff  ................
+000001a0: 0100 0000 0100 0000 0c00 0000 4150 5052  ............APPR
+000001b0: 4f58 494d 4154 4544 0000 0000 0c00 0c00  OXIMATED........
+000001c0: 0400 0000 0000 0800 0c00 0000 2400 0000  ............$...
+000001d0: 1400 0000 1000 0c00 0000 0000 0000 0000  ................
+000001e0: 0400 0800 1000 0000 0100 0000 0100 0000  ................
+000001f0: 0700 0000 554e 4b4e 4f57 4e00 1400 1400  ....UNKNOWN.....
+00000200: 0400 0800 0000 0c00 0000 0000 0000 1000  ................
+00000210: 1400 0000 4800 0000 2400 0000 0100 0000  ....H...$.......
+00000220: 0400 0000 1100 0000 2f2f 4c6f 6361 7469  ........//Locati
+00000230: 6f6e 4669 782e 6662 7300 0000 0700 0000  onFix.fbs.......
+00000240: d400 0000 8c01 0000 2c01 0000 f800 0000  ........,.......
+00000250: 7c00 0000 2400 0000 c401 0000 1400 0000  |...$...........
+00000260: 666f 7867 6c6f 7665 2e4c 6f63 6174 696f  foxglove.Locatio
+00000270: 6e46 6978 0000 0000 bcfd ffff 0600 1000  nFix............
+00000280: 2c00 0000 1400 0000 1000 1400 0700 0000  ,...............
+00000290: 0800 0000 0c00 1000 1000 0000 0000 0004  ................
+000002a0: 0000 0000 0100 0000 0100 0000 1800 0000  ................
+000002b0: 706f 7369 7469 6f6e 5f63 6f76 6172 6961  position_covaria
+000002c0: 6e63 655f 7479 7065 0000 0000 18ff ffff  nce_type........
+000002d0: 0000 0001 0500 0e00 2400 0000 1400 0000  ........$.......
+000002e0: 1000 0c00 0600 0700 0000 0000 0000 0800  ................
+000002f0: 1000 0000 0000 0e0c 0800 0000 1300 0000  ................
+00000300: 706f 7369 7469 6f6e 5f63 6f76 6172 6961  position_covaria
+00000310: 6e63 6500 58fe ffff 0400 0c00 1800 0000  nce.X...........
+00000320: 0400 0000 a0ff ffff 0000 000c 0800 0000  ................
+00000330: 0100 0000 0800 0000 616c 7469 7475 6465  ........altitude
+00000340: 0000 0000 88fe ffff 0300 0a00 1800 0000  ................
+00000350: 0400 0000 d0ff ffff 0000 000c 0800 0000  ................
+00000360: 0100 0000 0900 0000 6c6f 6e67 6974 7564  ........longitud
+00000370: 6500 0000 b8fe ffff 0200 0800 2800 0000  e...........(...
+00000380: 1400 0000 1000 1000 0700 0000 0000 0000  ................
+00000390: 0800 0c00 1000 0000 0000 000c 0800 0000  ................
+000003a0: 0100 0000 0800 0000 6c61 7469 7475 6465  ........latitude
+000003b0: 0000 0000 1c00 1400 0c00 1000 0800 0a00  ................
+000003c0: 0000 0000 0000 0000 0000 0000 0000 0700  ................
+000003d0: 1c00 0000 0000 0001 0100 0600 1400 0000  ................
+000003e0: 0400 0000 e0fe ffff 0000 000d 0100 0000  ................
+000003f0: 0800 0000 6672 616d 655f 6964 0000 0000  ....frame_id....
+00000400: 1c00 1000 0800 0c00 0000 0600 0000 0000  ................
+00000410: 0000 0000 0000 0000 0000 0500 1c00 0000  ................
+00000420: 0001 0400 2800 0000 1400 0000 1000 1000  ....(...........
+00000430: 0700 0000 0800 0000 0000 0c00 1000 0000  ................
+00000440: 0000 000f 0100 0000 0100 0000 0900 0000  ................
+00000450: 7469 6d65 7374 616d 7000 0000 1400 1c00  timestamp.......
+00000460: 0800 0c00 0700 1000 1400 0000 0000 1800  ................
+00000470: 1400 0000 0000 0001 3000 0000 2000 0000  ........0... ...
+00000480: 0400 0000 0800 0000 0400 0000 0a00 0000  ................
+00000490: 2f2f 5469 6d65 2e66 6273 0000 0200 0000  //Time.fbs......
+000004a0: 2800 0000 5400 0000 0d00 0000 666f 7867  (...T.......foxg
+000004b0: 6c6f 7665 2e54 696d 6500 0000 0c00 1000  love.Time.......
+000004c0: 0800 0c00 0400 0600 0c00 0000 0100 0400  ................
+000004d0: 1400 0000 0400 0000 d4ff ffff 0000 0008  ................
+000004e0: 0100 0000 0400 0000 6e73 6563 0000 0000  ........nsec....
+000004f0: 0800 0c00 0400 0800 0800 0000 2400 0000  ............$...
+00000500: 1400 0000 1000 0c00 0700 0000 0000 0000  ................
+00000510: 0000 0800 1000 0000 0000 0008 0100 0000  ................
+00000520: 0300 0000 7365 6300                      ....sec.
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/LocationFix.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/RawImage.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,111 +2,138 @@
 
 # namespace: foxglove
 
 import flatbuffers
 from flatbuffers.compat import import_numpy
 np = import_numpy()
 
-# A navigation satellite fix for any Global Navigation Satellite System
-class LocationFix(object):
+# A raw image
+class RawImage(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAs(cls, buf, offset=0):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
-        x = LocationFix()
+        x = RawImage()
         x.Init(buf, n + offset)
         return x
 
     @classmethod
-    def GetRootAsLocationFix(cls, buf, offset=0):
+    def GetRootAsRawImage(cls, buf, offset=0):
         """This method is deprecated. Please switch to GetRootAs."""
         return cls.GetRootAs(buf, offset)
-    # LocationFix
+    # RawImage
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
-    # Latitude in degrees
-    # LocationFix
-    def Latitude(self):
+    # Timestamp of image
+    # RawImage
+    def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
-        return 0.0
-
-    # Longitude in degrees
-    # LocationFix
-    def Longitude(self):
+            x = o + self._tab.Pos
+            from .Time import Time
+            obj = Time()
+            obj.Init(self._tab.Bytes, x)
+            return obj
+        return None
+
+    # Frame of reference for the image. The origin of the frame is the optical center of the camera. +x points to the right in the image, +y points down, and +z points into the plane of the image.
+    # RawImage
+    def FrameId(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
-        return 0.0
+            return self._tab.String(o + self._tab.Pos)
+        return None
 
-    # Altitude in meters
-    # LocationFix
-    def Altitude(self):
+    # Image width
+    # RawImage
+    def Width(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
-        return 0.0
+            return self._tab.Get(flatbuffers.number_types.Uint32Flags, o + self._tab.Pos)
+        return 0
 
-    # Position covariance (m^2) defined relative to a tangential plane through the reported position. The components are East, North, and Up (ENU), in row-major order.
-    # length 9
-    # LocationFix
-    def PositionCovariance(self, j):
+    # Image height
+    # RawImage
+    def Height(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
-            a = self._tab.Vector(o)
-            return self._tab.Get(flatbuffers.number_types.Float64Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 8))
+            return self._tab.Get(flatbuffers.number_types.Uint32Flags, o + self._tab.Pos)
         return 0
 
-    # LocationFix
-    def PositionCovarianceAsNumpy(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+    # Encoding of the raw image data
+    # 
+    # Supported values: `8UC1`, `8UC3`, `16UC1`, `32FC1`, `bayer_bggr8`, `bayer_gbrg8`, `bayer_grbg8`, `bayer_rggb8`, `bgr8`, `bgra8`, `mono8`, `mono16`, `rgb8`, `rgba8`, `uyvy` or `yuv422`, `yuyv` or `yuv422_yuy2`
+    # RawImage
+    def Encoding(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
-            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Float64Flags, o)
+            return self._tab.String(o + self._tab.Pos)
+        return None
+
+    # Byte length of a single row
+    # RawImage
+    def Step(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(14))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Uint32Flags, o + self._tab.Pos)
         return 0
 
-    # LocationFix
-    def PositionCovarianceLength(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+    # Raw image data
+    # RawImage
+    def Data(self, j):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
         if o != 0:
-            return self._tab.VectorLen(o)
+            a = self._tab.Vector(o)
+            return self._tab.Get(flatbuffers.number_types.Uint8Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 1))
         return 0
 
-    # LocationFix
-    def PositionCovarianceIsNone(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
-        return o == 0
+    # RawImage
+    def DataAsNumpy(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
+        if o != 0:
+            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Uint8Flags, o)
+        return 0
 
-    # If `position_covariance` is available, `position_covariance_type` must be set to indicate the type of covariance.
-    # LocationFix
-    def PositionCovarianceType(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
+    # RawImage
+    def DataLength(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Uint8Flags, o + self._tab.Pos)
+            return self._tab.VectorLen(o)
         return 0
 
-def LocationFixStart(builder): builder.StartObject(5)
+    # RawImage
+    def DataIsNone(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
+        return o == 0
+
+def RawImageStart(builder): builder.StartObject(7)
 def Start(builder):
-    return LocationFixStart(builder)
-def LocationFixAddLatitude(builder, latitude): builder.PrependFloat64Slot(0, latitude, 0.0)
-def AddLatitude(builder, latitude):
-    return LocationFixAddLatitude(builder, latitude)
-def LocationFixAddLongitude(builder, longitude): builder.PrependFloat64Slot(1, longitude, 0.0)
-def AddLongitude(builder, longitude):
-    return LocationFixAddLongitude(builder, longitude)
-def LocationFixAddAltitude(builder, altitude): builder.PrependFloat64Slot(2, altitude, 0.0)
-def AddAltitude(builder, altitude):
-    return LocationFixAddAltitude(builder, altitude)
-def LocationFixAddPositionCovariance(builder, positionCovariance): builder.PrependUOffsetTRelativeSlot(3, flatbuffers.number_types.UOffsetTFlags.py_type(positionCovariance), 0)
-def AddPositionCovariance(builder, positionCovariance):
-    return LocationFixAddPositionCovariance(builder, positionCovariance)
-def LocationFixStartPositionCovarianceVector(builder, numElems): return builder.StartVector(8, numElems, 8)
-def StartPositionCovarianceVector(builder, numElems):
-    return LocationFixStartPositionCovarianceVector(builder, numElems)
-def LocationFixAddPositionCovarianceType(builder, positionCovarianceType): builder.PrependUint8Slot(4, positionCovarianceType, 0)
-def AddPositionCovarianceType(builder, positionCovarianceType):
-    return LocationFixAddPositionCovarianceType(builder, positionCovarianceType)
-def LocationFixEnd(builder): return builder.EndObject()
+    return RawImageStart(builder)
+def RawImageAddTimestamp(builder, timestamp): builder.PrependStructSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(timestamp), 0)
+def AddTimestamp(builder, timestamp):
+    return RawImageAddTimestamp(builder, timestamp)
+def RawImageAddFrameId(builder, frameId): builder.PrependUOffsetTRelativeSlot(1, flatbuffers.number_types.UOffsetTFlags.py_type(frameId), 0)
+def AddFrameId(builder, frameId):
+    return RawImageAddFrameId(builder, frameId)
+def RawImageAddWidth(builder, width): builder.PrependUint32Slot(2, width, 0)
+def AddWidth(builder, width):
+    return RawImageAddWidth(builder, width)
+def RawImageAddHeight(builder, height): builder.PrependUint32Slot(3, height, 0)
+def AddHeight(builder, height):
+    return RawImageAddHeight(builder, height)
+def RawImageAddEncoding(builder, encoding): builder.PrependUOffsetTRelativeSlot(4, flatbuffers.number_types.UOffsetTFlags.py_type(encoding), 0)
+def AddEncoding(builder, encoding):
+    return RawImageAddEncoding(builder, encoding)
+def RawImageAddStep(builder, step): builder.PrependUint32Slot(5, step, 0)
+def AddStep(builder, step):
+    return RawImageAddStep(builder, step)
+def RawImageAddData(builder, data): builder.PrependUOffsetTRelativeSlot(6, flatbuffers.number_types.UOffsetTFlags.py_type(data), 0)
+def AddData(builder, data):
+    return RawImageAddData(builder, data)
+def RawImageStartDataVector(builder, numElems): return builder.StartVector(1, numElems, 1)
+def StartDataVector(builder, numElems):
+    return RawImageStartDataVector(builder, numElems)
+def RawImageEnd(builder): return builder.EndObject()
 def End(builder):
-    return LocationFixEnd(builder)
+    return RawImageEnd(builder)
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Log.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Log.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Log.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ModelPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/ModelPrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/ModelPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PackedElementField.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PackedElementField.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PackedElementField.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point2.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Point2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Point3.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Point3.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointCloud.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointCloud.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointCloud.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointsAnnotation.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PointsAnnotation.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PointsAnnotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     # PointsAnnotation
     def Type(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Uint8Flags, o + self._tab.Pos)
         return 0
 
-    # Points in 2D image coordinates (pixels)
+    # Points in 2D image coordinates (pixels).
+    # These coordinates use the top-left corner of the top-left pixel of the image as the origin.
     # PointsAnnotation
     def Points(self, j):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             x = self._tab.Vector(o)
             x += flatbuffers.number_types.UOffsetTFlags.py_type(j) * 4
             x = self._tab.Indirect(x)
@@ -79,15 +80,15 @@
             x = self._tab.Indirect(o + self._tab.Pos)
             from .Color import Color
             obj = Color()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
-    # Per-point colors, if `type` is `POINTS`, or per-segment stroke colors, if `type` is `LINE_LIST`.
+    # Per-point colors, if `type` is `POINTS`, or per-segment stroke colors, if `type` is `LINE_LIST`, `LINE_STRIP` or `LINE_LOOP`.
     # PointsAnnotation
     def OutlineColors(self, j):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             x = self._tab.Vector(o)
             x += flatbuffers.number_types.UOffsetTFlags.py_type(j) * 4
             x = self._tab.Indirect(x)
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Pose.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Pose.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Pose.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PoseInFrame.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PoseInFrame.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PoseInFrame.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PosesInFrame.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/PosesInFrame.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/PosesInFrame.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Quaternion.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Quaternion.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/RawImage.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/RawImage.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntity.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntity.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntity.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneEntityDeletion.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneUpdate.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SceneUpdate.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SceneUpdate.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SpherePrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/SpherePrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/SpherePrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextAnnotation.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextAnnotation.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextAnnotation.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextAnnotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
             x = o + self._tab.Pos
             from .Time import Time
             obj = Time()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
-    # Bottom-left origin of the text label in 2D image coordinates (pixels)
+    # Bottom-left origin of the text label in 2D image coordinates (pixels).
+    # The coordinate uses the top-left corner of the top-left pixel of the image as the origin.
     # TextAnnotation
     def Position(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             from .Point2 import Point2
             obj = Point2()
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TextPrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TextPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Time.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Time.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.bfbs`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/TriangleListPrimitive.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector2.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Vector2.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer/Vector3.py` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer/Vector3.py`

 * *Files identical despite different names*

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/PKG-INFO` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: foxglove-schemas-flatbuffer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Flatbuffer classes for Foxglove Schemas
 Home-page: https://github.com/foxglove/schemas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: flatbuffers
 
 # Foxglove Schemas (Flatbuffer)
 
-This package provides [Flatbuffer](https://google.github.io/flatbuffers/) classes for [Foxglove Schemas](https://foxglove.dev/docs/studio/messages/introduction).
+This package provides [Flatbuffer](https://google.github.io/flatbuffers/) classes for [Foxglove Schemas](https://docs.foxglove.dev/docs/visualization/message-schemas/introduction).
 
 ## Installation
 
 Install via [Pipenv](https://pipenv.pypa.io/en/latest/) by adding `foxglove-schemas-flatbuffer` to your `Pipfile` or via the command line:
 
 ```bash
 pipenv install foxglove-schemas-flatbuffer
@@ -42,8 +43,8 @@
 
 # Serialized CompressedImage message
 msg_data = builder.Output()
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt` & `foxglove_schemas_flatbuffer-0.2.0/foxglove_schemas_flatbuffer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 foxglove_schemas_flatbuffer/CameraCalibration.py
 foxglove_schemas_flatbuffer/CircleAnnotation.bfbs
 foxglove_schemas_flatbuffer/CircleAnnotation.py
 foxglove_schemas_flatbuffer/Color.bfbs
 foxglove_schemas_flatbuffer/Color.py
 foxglove_schemas_flatbuffer/CompressedImage.bfbs
 foxglove_schemas_flatbuffer/CompressedImage.py
+foxglove_schemas_flatbuffer/CompressedVideo.bfbs
+foxglove_schemas_flatbuffer/CompressedVideo.py
 foxglove_schemas_flatbuffer/CubePrimitive.bfbs
 foxglove_schemas_flatbuffer/CubePrimitive.py
 foxglove_schemas_flatbuffer/CylinderPrimitive.bfbs
 foxglove_schemas_flatbuffer/CylinderPrimitive.py
 foxglove_schemas_flatbuffer/Duration.bfbs
 foxglove_schemas_flatbuffer/Duration.py
 foxglove_schemas_flatbuffer/FrameTransform.bfbs
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/setup.cfg` & `foxglove_schemas_flatbuffer-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-schemas-flatbuffer
-version = 0.1.0
+version = 0.2.0
 description = Flatbuffer classes for Foxglove Schemas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/schemas
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-schemas-flatbuffer-0.1.0/tests/test_schemas.py` & `foxglove_schemas_flatbuffer-0.2.0/tests/test_schemas.py`

 * *Files identical despite different names*

