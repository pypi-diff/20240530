# Comparing `tmp/lqs-client-0.1.8.tar.gz` & `tmp/lqs-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqs-client-0.1.8.tar", last modified: Tue Jan 23 20:07:14 2024, max compression
+gzip compressed data, was "lqs-client-0.1.9.tar", last modified: Tue Jan 23 20:24:30 2024, max compression
```

## Comparing `lqs-client-0.1.8.tar` & `lqs-client-0.1.9.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.979113 lqs-client-0.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2022-12-19 19:59:13.000000 lqs-client-0.1.8/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4850 2024-01-23 20:07:14.979113 lqs-client-0.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3946 2023-03-31 19:13:53.000000 lqs-client-0.1.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.899113 lqs-client-0.1.8/lqs_client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5829 2024-01-23 20:04:20.000000 lqs-client-0.1.8/lqs_client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.1.8/lqs_client/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.899113 lqs-client-0.1.8/lqs_client/definitions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-19 19:48:58.000000 lqs-client-0.1.8/lqs_client/definitions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.891113 lqs-client-0.1.8/lqs_client/definitions/actionlib_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.903113 lqs-client-0.1.8/lqs_client/definitions/actionlib_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2022-12-20 19:36:05.000000 lqs-client-0.1.8/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1626 2022-12-20 19:36:05.000000 lqs-client-0.1.8/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2022-12-20 19:36:05.000000 lqs-client-0.1.8/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.891113 lqs-client-0.1.8/lqs_client/definitions/diagnostic_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.903113 lqs-client-0.1.8/lqs_client/definitions/diagnostic_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2022-12-20 19:36:25.000000 lqs-client-0.1.8/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      426 2022-12-20 19:36:25.000000 lqs-client-0.1.8/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2022-12-20 19:36:25.000000 lqs-client-0.1.8/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.891113 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.915113 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Accel.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Point.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Point32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Pose.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      122 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Transform.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Twist.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      382 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      103 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.891113 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.919113 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2022-12-20 19:36:31.000000 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/msg/GridCells.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2022-12-20 19:36:31.000000 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-12-20 19:36:31.000000 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2022-12-20 19:36:31.000000 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/msg/Odometry.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2022-12-20 19:36:31.000000 lqs-client-0.1.8/lqs_client/definitions/nav_msgs/msg/Path.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.895113 lqs-client-0.1.8/lqs_client/definitions/rosgraph_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.919113 lqs-client-0.1.8/lqs_client/definitions/rosgraph_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      184 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      722 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.895113 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.939113 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6284 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1008 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      640 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      986 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1362 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Image.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1206 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Imu.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/JointState.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Joy.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1519 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1596 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      425 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/PointField.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Range.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      618 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-20 19:36:33.000000 lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.895113 lqs-client-0.1.8/lqs_client/definitions/shape_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.943113 lqs-client-0.1.8/lqs_client/definitions/shape_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      196 2022-12-20 19:36:36.000000 lqs-client-0.1.8/lqs_client/definitions/shape_msgs/msg/Mesh.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-12-20 19:36:36.000000 lqs-client-0.1.8/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2022-12-20 19:36:36.000000 lqs-client-0.1.8/lqs_client/definitions/shape_msgs/msg/Plane.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-12-20 19:36:36.000000 lqs-client-0.1.8/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.895113 lqs-client-0.1.8/lqs_client/definitions/std_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.963113 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Bool.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Byte.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Char.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Duration.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Empty.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Float32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Float64.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      551 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Header.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int16.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int64.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int8.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      141 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      911 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/String.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Time.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt16.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt64.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt8.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.895113 lqs-client-0.1.8/lqs_client/definitions/stereo_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.967113 lqs-client-0.1.8/lqs_client/definitions/stereo_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1137 2022-12-20 19:36:39.000000 lqs-client-0.1.8/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.895113 lqs-client-0.1.8/lqs_client/definitions/trajectory_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.967113 lqs-client-0.1.8/lqs_client/definitions/trajectory_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2022-12-20 19:36:42.000000 lqs-client-0.1.8/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:42.000000 lqs-client-0.1.8/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2022-12-20 19:36:42.000000 lqs-client-0.1.8/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:42.000000 lqs-client-0.1.8/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.899113 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.975113 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      827 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      808 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2586 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      950 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1935 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/Marker.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1586 2022-12-20 19:36:44.000000 lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.975113 lqs-client-0.1.8/lqs_client/gen/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-04-26 13:56:12.000000 lqs-client-0.1.8/lqs_client/gen/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.979113 lqs-client-0.1.8/lqs_client/interface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      239 2023-07-01 00:05:49.000000 lqs-client-0.1.8/lqs_client/interface/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8696 2023-06-05 19:22:37.000000 lqs-client-0.1.8/lqs_client/interface/ark_deserialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5848 2024-01-23 20:06:44.000000 lqs-client-0.1.8/lqs_client/interface/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6158 2023-06-22 18:52:49.000000 lqs-client-0.1.8/lqs_client/interface/creator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.1.8/lqs_client/interface/deleter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9312 2023-05-19 14:25:06.000000 lqs-client-0.1.8/lqs_client/interface/fs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.1.8/lqs_client/interface/getter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11610 2023-05-19 14:25:06.000000 lqs-client-0.1.8/lqs_client/interface/input_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18199 2023-07-01 00:05:49.000000 lqs-client-0.1.8/lqs_client/interface/lister.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16489 2023-06-05 19:22:37.000000 lqs-client-0.1.8/lqs_client/interface/message_converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6849 2023-07-27 14:31:30.000000 lqs-client-0.1.8/lqs_client/interface/node.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18266 2023-07-27 13:19:54.000000 lqs-client-0.1.8/lqs_client/interface/ros_deserialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29571 2024-01-23 20:06:45.000000 lqs-client-0.1.8/lqs_client/interface/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15734 2023-04-24 20:09:51.000000 lqs-client-0.1.8/lqs_client/interface/terminal.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.1.8/lqs_client/interface/updater.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17479 2023-12-07 17:55:20.000000 lqs-client-0.1.8/lqs_client/interface/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:07:14.979113 lqs-client-0.1.8/lqs_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4850 2024-01-23 20:07:14.000000 lqs-client-0.1.8/lqs_client.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7647 2024-01-23 20:07:14.000000 lqs-client-0.1.8/lqs_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-23 20:07:14.000000 lqs-client-0.1.8/lqs_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-01-23 20:07:14.000000 lqs-client-0.1.8/lqs_client.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-01-23 20:07:14.000000 lqs-client-0.1.8/lqs_client.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.1.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-23 20:07:14.979113 lqs-client-0.1.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1286 2024-01-23 20:07:01.000000 lqs-client-0.1.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.587723 lqs-client-0.1.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2022-12-19 19:59:13.000000 lqs-client-0.1.9/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4850 2024-01-23 20:24:30.587723 lqs-client-0.1.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3946 2023-03-31 19:13:53.000000 lqs-client-0.1.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5829 2024-01-23 20:04:20.000000 lqs-client-0.1.9/lqs_client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.1.9/lqs_client/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.563722 lqs-client-0.1.9/lqs_client/definitions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-19 19:48:58.000000 lqs-client-0.1.9/lqs_client/definitions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.555722 lqs-client-0.1.9/lqs_client/definitions/actionlib_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.563722 lqs-client-0.1.9/lqs_client/definitions/actionlib_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2022-12-20 19:36:05.000000 lqs-client-0.1.9/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1626 2022-12-20 19:36:05.000000 lqs-client-0.1.9/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2022-12-20 19:36:05.000000 lqs-client-0.1.9/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/diagnostic_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.563722 lqs-client-0.1.9/lqs_client/definitions/diagnostic_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2022-12-20 19:36:25.000000 lqs-client-0.1.9/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      426 2022-12-20 19:36:25.000000 lqs-client-0.1.9/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2022-12-20 19:36:25.000000 lqs-client-0.1.9/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.567722 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Accel.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Point.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Point32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Pose.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      122 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Transform.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Twist.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      382 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      103 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.567722 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2022-12-20 19:36:31.000000 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/msg/GridCells.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2022-12-20 19:36:31.000000 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-12-20 19:36:31.000000 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2022-12-20 19:36:31.000000 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/msg/Odometry.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2022-12-20 19:36:31.000000 lqs-client-0.1.9/lqs_client/definitions/nav_msgs/msg/Path.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/rosgraph_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.567722 lqs-client-0.1.9/lqs_client/definitions/rosgraph_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      184 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      722 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.571723 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6284 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1008 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      640 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      986 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1362 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Image.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1206 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Imu.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/JointState.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Joy.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1519 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1596 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      425 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/PointField.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Range.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      618 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-20 19:36:33.000000 lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/shape_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.575723 lqs-client-0.1.9/lqs_client/definitions/shape_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      196 2022-12-20 19:36:36.000000 lqs-client-0.1.9/lqs_client/definitions/shape_msgs/msg/Mesh.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-12-20 19:36:36.000000 lqs-client-0.1.9/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2022-12-20 19:36:36.000000 lqs-client-0.1.9/lqs_client/definitions/shape_msgs/msg/Plane.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-12-20 19:36:36.000000 lqs-client-0.1.9/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/std_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.579723 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Bool.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Byte.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Char.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Duration.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Empty.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Float32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Float64.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      551 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Header.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int16.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int64.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int8.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      141 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      911 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/String.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Time.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt16.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt32.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt64.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt8.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/stereo_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.579723 lqs-client-0.1.9/lqs_client/definitions/stereo_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1137 2022-12-20 19:36:39.000000 lqs-client-0.1.9/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/trajectory_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.579723 lqs-client-0.1.9/lqs_client/definitions/trajectory_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2022-12-20 19:36:42.000000 lqs-client-0.1.9/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:42.000000 lqs-client-0.1.9/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2022-12-20 19:36:42.000000 lqs-client-0.1.9/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:42.000000 lqs-client-0.1.9/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.559723 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.583722 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      827 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      808 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2586 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      950 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1935 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/Marker.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1586 2022-12-20 19:36:44.000000 lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.583722 lqs-client-0.1.9/lqs_client/gen/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-04-26 13:56:12.000000 lqs-client-0.1.9/lqs_client/gen/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.583722 lqs-client-0.1.9/lqs_client/interface/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      239 2023-07-01 00:05:49.000000 lqs-client-0.1.9/lqs_client/interface/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8696 2023-06-05 19:22:37.000000 lqs-client-0.1.9/lqs_client/interface/ark_deserialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5848 2024-01-23 20:06:44.000000 lqs-client-0.1.9/lqs_client/interface/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6158 2023-06-22 18:52:49.000000 lqs-client-0.1.9/lqs_client/interface/creator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.1.9/lqs_client/interface/deleter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9312 2023-05-19 14:25:06.000000 lqs-client-0.1.9/lqs_client/interface/fs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.1.9/lqs_client/interface/getter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11610 2023-05-19 14:25:06.000000 lqs-client-0.1.9/lqs_client/interface/input_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18199 2023-07-01 00:05:49.000000 lqs-client-0.1.9/lqs_client/interface/lister.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16489 2023-06-05 19:22:37.000000 lqs-client-0.1.9/lqs_client/interface/message_converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6849 2023-07-27 14:31:30.000000 lqs-client-0.1.9/lqs_client/interface/node.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18266 2023-07-27 13:19:54.000000 lqs-client-0.1.9/lqs_client/interface/ros_deserialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30771 2024-01-23 20:24:16.000000 lqs-client-0.1.9/lqs_client/interface/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15734 2023-04-24 20:09:51.000000 lqs-client-0.1.9/lqs_client/interface/terminal.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.1.9/lqs_client/interface/updater.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17479 2023-12-07 17:55:20.000000 lqs-client-0.1.9/lqs_client/interface/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-23 20:24:30.583722 lqs-client-0.1.9/lqs_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4850 2024-01-23 20:24:30.000000 lqs-client-0.1.9/lqs_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7647 2024-01-23 20:24:30.000000 lqs-client-0.1.9/lqs_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-23 20:24:30.000000 lqs-client-0.1.9/lqs_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-01-23 20:24:30.000000 lqs-client-0.1.9/lqs_client.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-01-23 20:24:30.000000 lqs-client-0.1.9/lqs_client.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.1.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-23 20:24:30.587723 lqs-client-0.1.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1286 2024-01-23 20:21:56.000000 lqs-client-0.1.9/setup.py
```

### Comparing `lqs-client-0.1.8/PKG-INFO` & `lqs-client-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.1.8/README.md` & `lqs-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/__init__.py` & `lqs-client-0.1.9/lqs_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg` & `lqs-client-0.1.9/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg` & `lqs-client-0.1.9/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg` & `lqs-client-0.1.9/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Image.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Image.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Imu.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Imu.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/JointState.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/JointState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/Range.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/Range.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg` & `lqs-client-0.1.9/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg` & `lqs-client-0.1.9/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/Header.msg` & `lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/Header.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg` & `lqs-client-0.1.9/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg` & `lqs-client-0.1.9/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/Marker.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/Marker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg` & `lqs-client-0.1.9/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/gen/__init__.py` & `lqs-client-0.1.9/lqs_client/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/ark_deserialization.py` & `lqs-client-0.1.9/lqs_client/interface/ark_deserialization.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/common.py` & `lqs-client-0.1.9/lqs_client/interface/common.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/creator.py` & `lqs-client-0.1.9/lqs_client/interface/creator.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/deleter.py` & `lqs-client-0.1.9/lqs_client/interface/deleter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/fs.py` & `lqs-client-0.1.9/lqs_client/interface/fs.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/getter.py` & `lqs-client-0.1.9/lqs_client/interface/getter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/input_stream.py` & `lqs-client-0.1.9/lqs_client/interface/input_stream.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/lister.py` & `lqs-client-0.1.9/lqs_client/interface/lister.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/message_converter.py` & `lqs-client-0.1.9/lqs_client/interface/message_converter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/node.py` & `lqs-client-0.1.9/lqs_client/interface/node.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/ros_deserialization.py` & `lqs-client-0.1.9/lqs_client/interface/ros_deserialization.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/s3.py` & `lqs-client-0.1.9/lqs_client/interface/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,14 +214,16 @@
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.post(
                 url, data=complete_multipart_payload, verify=self._verify_ssl
             )
+            if r.status_code != 200:
+                raise ValueError(f"Error completing multipart upload: {r.text}")
             if decode_response:
                 response_text = unquote(r.text)
             else:
                 response_text = r.text
             response_content = (
                 xmltodict.parse(response_text) if convert_to_dict else response_text
             )
@@ -257,14 +259,16 @@
                 method="create_multipart_upload",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.post(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error creating multipart upload: {r.text}")
             if decode_response:
                 response_text = unquote(r.text)
             else:
                 response_text = r.text
             response_content = (
                 xmltodict.parse(response_text) if convert_to_dict else response_text
             )
@@ -301,14 +305,16 @@
                 method="delete_object",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.delete(url, verify=self._verify_ssl)
+            if r.status_code != 204:
+                raise ValueError(f"Error deleting object: {r.text}")
             return r.headers, used_params, None
 
         return self._handle_retries(make_requests)
 
     def get_object(
         self,
         resource: S3Resource,
@@ -338,14 +344,16 @@
                 method="get_object",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.get(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error getting object: {r.text}")
             return r.headers, used_params, r.content
 
         return self._handle_retries(make_requests)
 
     def head_object(
         self,
         resource: S3Resource,
@@ -378,14 +386,16 @@
                 method="head_object",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.head(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error heading object: {r.text}")
             # TODO: may need to return a status code as well
             # for now, we'll just return it as the body
             return r.headers, used_params, {"exists": r.status_code == 200}
 
         return self._handle_retries(make_requests)
 
     def list_multipart_uploads(
@@ -415,14 +425,16 @@
                 method="list_multipart_uploads",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.get(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error listing multipart uploads: {r.text}")
             if decode_response:
                 response_text = unquote(r.text)
             else:
                 response_text = r.text
             response_content = (
                 xmltodict.parse(response_text) if convert_to_dict else response_text
             )
@@ -457,14 +469,16 @@
                 method="list_object_versions",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.get(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error listing object versions: {r.text}")
             if decode_response:
                 response_text = unquote(r.text)
             else:
                 response_text = r.text
             response_content = (
                 xmltodict.parse(response_text) if convert_to_dict else response_text
             )
@@ -502,14 +516,16 @@
                 method="list_objects_v2",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.get(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error listing objects: {r.text}")
             if decode_response:
                 response_text = unquote(r.text)
             else:
                 response_text = r.text
             response_content = (
                 xmltodict.parse(response_text) if convert_to_dict else response_text
             )
@@ -549,14 +565,16 @@
                 method="list_parts",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.get(url, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error listing parts: {r.text}")
             if decode_response:
                 response_text = unquote(r.text)
             else:
                 response_text = r.text
             response_content = (
                 xmltodict.parse(response_text) if convert_to_dict else response_text
             )
@@ -587,14 +605,16 @@
                 method="put_object",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.put(url, data=body, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error putting object: {r.text}")
             return r.headers, used_params, None
 
         return self._handle_retries(make_requests)
 
     def restore_object(self):
         raise NotImplementedError("Restore object is not implemented yet.")
 
@@ -627,14 +647,16 @@
                 method="upload_part",
                 resource=resource,
                 params=params,
                 resource_id=resource_id,
                 timestamp=timestamp,
             )
             r = requests.put(url, data=body, verify=self._verify_ssl)
+            if r.status_code != 200:
+                raise ValueError(f"Error uploading part: {r.text}")
             return r.headers, used_params, None
 
         return self._handle_retries(make_requests)
 
     def get_message_data_from_record(
         self, record, s3_bucket=None, s3_key=None, ingestion_id=None
     ):
```

### Comparing `lqs-client-0.1.8/lqs_client/interface/terminal.py` & `lqs-client-0.1.9/lqs_client/interface/terminal.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/updater.py` & `lqs-client-0.1.9/lqs_client/interface/updater.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client/interface/utils.py` & `lqs-client-0.1.9/lqs_client/interface/utils.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/lqs_client.egg-info/PKG-INFO` & `lqs-client-0.1.9/lqs_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.1.8/lqs_client.egg-info/SOURCES.txt` & `lqs-client-0.1.9/lqs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.8/setup.py` & `lqs-client-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqs-client",
-    version="0.1.8",
+    version="0.1.9",
     author="Nathan Margaglio",
     author_email="nmargaglio@carnegierobotics.com",
     description="LogQS Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carnegierobotics/LogQS-Client",
     project_urls={
```

