# Comparing `tmp/pyluba-0.0.8.tar.gz` & `tmp/pyluba-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluba-0.0.8.tar", max compression
+gzip compressed data, was "pyluba-0.0.9.tar", max compression
```

## Comparing `pyluba-0.0.8.tar` & `pyluba-0.0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.8/LICENSE
--rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.8/README.md
--rw-r--r--   0        0        0      903 2024-05-15 09:07:45.520662 pyluba-0.0.8/pyluba/__init__.py
--rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.8/pyluba/aliyun/cloud_gateway.py
--rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.8/pyluba/aliyun/cloud_service.py
--rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.8/pyluba/aliyun/test_alicloud_api_gateway.py
--rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/aliyun/tmp_constant.py
--rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.8/pyluba/bluetooth/__init__.py
--rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.8/pyluba/bluetooth/ble.py
--rw-r--r--   0        0        0    40473 2024-05-15 09:07:42.251526 pyluba-0.0.8/pyluba/bluetooth/ble_message.py
--rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/const.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/__init__.py
--rw-r--r--   0        0        0     4405 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/bluetooth/data/convert.py
--rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/framectrldata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/model/__init__.py
--rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/notifydata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/__init__.py
--rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/__init__.py
--rw-r--r--   0        0        0     1359 2024-05-14 22:34:13.652444 pyluba-0.0.8/pyluba/data/model/excute_boarder_params.py
--rw-r--r--   0        0        0     1088 2024-05-18 23:22:44.570535 pyluba-0.0.8/pyluba/data/model/execute_boarder.py
--rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/generate_route_information.py
--rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/hash_list.py
--rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/mowing_modes.py
--rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/plan.py
--rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/rapid_state.py
--rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/region_data.py
--rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/mqtt/__init__.py
--rw-r--r--   0        0        0     1802 2024-05-18 23:15:54.054056 pyluba-0.0.8/pyluba/data/mqtt/event.py
--rw-r--r--   0        0        0     2795 2024-05-18 23:17:51.762904 pyluba-0.0.8/pyluba/data/mqtt/properties.py
--rw-r--r--   0        0        0     1064 2024-05-18 23:18:33.829029 pyluba-0.0.8/pyluba/data/mqtt/status.py
--rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/event/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.8/pyluba/event/event.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/http/_init_.py
--rw-r--r--   0        0        0     1937 2024-05-18 23:19:47.517975 pyluba-0.0.8/pyluba/http/http.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/luba/_init_.py
--rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/luba/base.py
--rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.8/pyluba/mammotion/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.8/pyluba/mammotion/commands/proto.py
--rw-r--r--   0        0        0       48 2024-05-14 22:27:59.597338 pyluba-0.0.8/pyluba/mammotion/devices/__init__.py
--rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.8/pyluba/mammotion/devices/luba.py
--rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.8/pyluba/mqtt/mqtt.py
--rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/proto/common.proto
--rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.8/pyluba/proto/common_pb2.py
--rw-r--r--   0        0        0      460 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/common_pb2.pyi
--rw-r--r--   0        0        0     5502 2024-05-15 09:07:42.251526 pyluba-0.0.8/pyluba/proto/dev_net.proto
--rw-r--r--   0        0        0    12853 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/dev_net_pb2.py
--rw-r--r--   0        0        0    21825 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/dev_net_pb2.pyi
--rw-r--r--   0        0        0     1553 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_msg.proto
--rw-r--r--   0        0        0     4215 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_msg_pb2.py
--rw-r--r--   0        0        0     4031 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/luba_msg_pb2.pyi
--rw-r--r--   0        0        0     1114 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_mul.proto
--rw-r--r--   0        0        0     3387 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_mul_pb2.py
--rw-r--r--   0        0        0     3913 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/luba_mul_pb2.pyi
--rw-r--r--   0        0        0     1383 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/mctrl_driver.proto
--rw-r--r--   0        0        0     3770 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.py
--rw-r--r--   0        0        0     5852 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.pyi
--rw-r--r--   0        0        0    10530 2024-05-15 09:07:42.253526 pyluba-0.0.8/pyluba/proto/mctrl_nav.proto
--rw-r--r--   0        0        0    21725 2024-05-15 09:07:42.253526 pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.py
--rw-r--r--   0        0        0    45951 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.pyi
--rw-r--r--   0        0        0      629 2024-05-15 09:07:42.253526 pyluba-0.0.8/pyluba/proto/mctrl_ota.proto
--rw-r--r--   0        0        0     2259 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.py
--rw-r--r--   0        0        0     2821 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.pyi
--rw-r--r--   0        0        0      664 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_pept.proto
--rw-r--r--   0        0        0     2121 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.py
--rw-r--r--   0        0        0     2840 2024-05-18 08:45:36.776446 pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.pyi
--rw-r--r--   0        0        0    10186 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_sys.proto
--rw-r--r--   0        0        0    21469 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.py
--rw-r--r--   0        0        0    38893 2024-05-18 08:45:36.776446 pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.8/pyluba/py.typed
--rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.8/pyluba/utility/constant/device_constant.py
--rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.8/pyluba/utility/periodic.py
--rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.8/pyluba/utility/rocker_util.py
--rw-r--r--   0        0        0     1443 2024-05-18 23:25:34.314790 pyluba-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 pyluba-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.9/LICENSE
+-rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.9/README.md
+-rw-r--r--   0        0        0      903 2024-05-15 09:07:45.520662 pyluba-0.0.9/pyluba/__init__.py
+-rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.9/pyluba/aliyun/cloud_gateway.py
+-rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.9/pyluba/aliyun/cloud_service.py
+-rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.9/pyluba/aliyun/test_alicloud_api_gateway.py
+-rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/aliyun/tmp_constant.py
+-rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.9/pyluba/bluetooth/__init__.py
+-rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.9/pyluba/bluetooth/ble.py
+-rw-r--r--   0        0        0    40473 2024-05-15 09:07:42.251526 pyluba-0.0.9/pyluba/bluetooth/ble_message.py
+-rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/bluetooth/const.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/bluetooth/data/__init__.py
+-rw-r--r--   0        0        0     4405 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/bluetooth/data/convert.py
+-rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/bluetooth/data/framectrldata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/bluetooth/data/model/__init__.py
+-rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/bluetooth/data/notifydata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/__init__.py
+-rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/__init__.py
+-rw-r--r--   0        0        0     1359 2024-05-14 22:34:13.652444 pyluba-0.0.9/pyluba/data/model/excute_boarder_params.py
+-rw-r--r--   0        0        0     1088 2024-05-18 23:22:44.570535 pyluba-0.0.9/pyluba/data/model/execute_boarder.py
+-rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/generate_route_information.py
+-rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/hash_list.py
+-rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/mowing_modes.py
+-rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/plan.py
+-rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/rapid_state.py
+-rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/model/region_data.py
+-rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.9/pyluba/data/mqtt/__init__.py
+-rw-r--r--   0        0        0     2161 2024-05-19 00:09:02.201971 pyluba-0.0.9/pyluba/data/mqtt/event.py
+-rw-r--r--   0        0        0     2795 2024-05-18 23:17:51.762904 pyluba-0.0.9/pyluba/data/mqtt/properties.py
+-rw-r--r--   0        0        0     1064 2024-05-18 23:18:33.829029 pyluba-0.0.9/pyluba/data/mqtt/status.py
+-rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.9/pyluba/event/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.9/pyluba/event/event.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.9/pyluba/http/_init_.py
+-rw-r--r--   0        0        0     1937 2024-05-18 23:19:47.517975 pyluba-0.0.9/pyluba/http/http.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.9/pyluba/luba/_init_.py
+-rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.9/pyluba/luba/base.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.9/pyluba/mammotion/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.9/pyluba/mammotion/commands/proto.py
+-rw-r--r--   0        0        0       48 2024-05-14 22:27:59.597338 pyluba-0.0.9/pyluba/mammotion/devices/__init__.py
+-rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.9/pyluba/mammotion/devices/luba.py
+-rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.9/pyluba/mqtt/mqtt.py
+-rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.9/pyluba/proto/common.proto
+-rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.9/pyluba/proto/common_pb2.py
+-rw-r--r--   0        0        0      460 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/common_pb2.pyi
+-rw-r--r--   0        0        0     5502 2024-05-15 09:07:42.251526 pyluba-0.0.9/pyluba/proto/dev_net.proto
+-rw-r--r--   0        0        0    12853 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/dev_net_pb2.py
+-rw-r--r--   0        0        0    21825 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/dev_net_pb2.pyi
+-rw-r--r--   0        0        0     1553 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/luba_msg.proto
+-rw-r--r--   0        0        0     4215 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/luba_msg_pb2.py
+-rw-r--r--   0        0        0     4031 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/luba_msg_pb2.pyi
+-rw-r--r--   0        0        0     1114 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/luba_mul.proto
+-rw-r--r--   0        0        0     3387 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/luba_mul_pb2.py
+-rw-r--r--   0        0        0     3913 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/luba_mul_pb2.pyi
+-rw-r--r--   0        0        0     1383 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/mctrl_driver.proto
+-rw-r--r--   0        0        0     3770 2024-05-15 09:07:42.252526 pyluba-0.0.9/pyluba/proto/mctrl_driver_pb2.py
+-rw-r--r--   0        0        0     5852 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/mctrl_driver_pb2.pyi
+-rw-r--r--   0        0        0    10530 2024-05-15 09:07:42.253526 pyluba-0.0.9/pyluba/proto/mctrl_nav.proto
+-rw-r--r--   0        0        0    21725 2024-05-15 09:07:42.253526 pyluba-0.0.9/pyluba/proto/mctrl_nav_pb2.py
+-rw-r--r--   0        0        0    45951 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/mctrl_nav_pb2.pyi
+-rw-r--r--   0        0        0      629 2024-05-15 09:07:42.253526 pyluba-0.0.9/pyluba/proto/mctrl_ota.proto
+-rw-r--r--   0        0        0     2259 2024-05-15 09:07:42.254526 pyluba-0.0.9/pyluba/proto/mctrl_ota_pb2.py
+-rw-r--r--   0        0        0     2821 2024-05-18 08:45:36.775444 pyluba-0.0.9/pyluba/proto/mctrl_ota_pb2.pyi
+-rw-r--r--   0        0        0      664 2024-05-15 09:07:42.254526 pyluba-0.0.9/pyluba/proto/mctrl_pept.proto
+-rw-r--r--   0        0        0     2121 2024-05-15 09:07:42.254526 pyluba-0.0.9/pyluba/proto/mctrl_pept_pb2.py
+-rw-r--r--   0        0        0     2840 2024-05-18 08:45:36.776446 pyluba-0.0.9/pyluba/proto/mctrl_pept_pb2.pyi
+-rw-r--r--   0        0        0    10186 2024-05-15 09:07:42.254526 pyluba-0.0.9/pyluba/proto/mctrl_sys.proto
+-rw-r--r--   0        0        0    21469 2024-05-15 09:07:42.254526 pyluba-0.0.9/pyluba/proto/mctrl_sys_pb2.py
+-rw-r--r--   0        0        0    38893 2024-05-18 08:45:36.776446 pyluba-0.0.9/pyluba/proto/mctrl_sys_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.9/pyluba/py.typed
+-rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.9/pyluba/utility/constant/device_constant.py
+-rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.9/pyluba/utility/periodic.py
+-rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.9/pyluba/utility/rocker_util.py
+-rw-r--r--   0        0        0     1443 2024-05-19 02:02:09.854858 pyluba-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 pyluba-0.0.9/PKG-INFO
```

### Comparing `pyluba-0.0.8/LICENSE` & `pyluba-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/README.md` & `pyluba-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/__init__.py` & `pyluba-0.0.9/pyluba/__init__.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/aliyun/cloud_gateway.py` & `pyluba-0.0.9/pyluba/aliyun/cloud_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/aliyun/cloud_service.py` & `pyluba-0.0.9/pyluba/aliyun/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/aliyun/test_alicloud_api_gateway.py` & `pyluba-0.0.9/pyluba/aliyun/test_alicloud_api_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/aliyun/tmp_constant.py` & `pyluba-0.0.9/pyluba/aliyun/tmp_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/bluetooth/ble.py` & `pyluba-0.0.9/pyluba/bluetooth/ble.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/bluetooth/ble_message.py` & `pyluba-0.0.9/pyluba/bluetooth/ble_message.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/bluetooth/const.py` & `pyluba-0.0.9/pyluba/bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/bluetooth/data/convert.py` & `pyluba-0.0.9/pyluba/bluetooth/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/bluetooth/data/framectrldata.py` & `pyluba-0.0.9/pyluba/bluetooth/data/framectrldata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/bluetooth/data/notifydata.py` & `pyluba-0.0.9/pyluba/bluetooth/data/notifydata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/model/excute_boarder_params.py` & `pyluba-0.0.9/pyluba/data/model/excute_boarder_params.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/model/execute_boarder.py` & `pyluba-0.0.9/pyluba/data/model/execute_boarder.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/model/generate_route_information.py` & `pyluba-0.0.9/pyluba/data/model/generate_route_information.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/model/plan.py` & `pyluba-0.0.9/pyluba/data/model/plan.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/model/rapid_state.py` & `pyluba-0.0.9/pyluba/data/model/rapid_state.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/model/region_data.py` & `pyluba-0.0.9/pyluba/data/model/region_data.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/mqtt/event.py` & `pyluba-0.0.9/pyluba/data/mqtt/event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 from base64 import b64decode
 from dataclasses import dataclass
 from typing import Literal, Any, Union
 
+from google.protobuf import json_format
+from mashumaro.types import SerializableType
+
 from pyluba.proto import luba_msg_pb2
 
 from mashumaro.mixins.orjson import DataClassORJSONMixin
 
-class Base64EncodedProtobuf:
+class Base64EncodedProtobuf(SerializableType):
+    def __init__(self, proto: str):
+        self.proto = proto
+
+    def _serialize(self):
+        return self.proto
+
+    @classmethod
+    def _deserialize(cls, value):
+        return cls(*value)
+
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     def validate(cls, v: str):
         if not isinstance(v, str):
             raise TypeError("string required")
         binary = b64decode(v, validate=True)
         data = luba_msg_pb2.LubaMsg()
         data.ParseFromString(binary)
-        return data
+        return json_format.MessageToDict(data)
+
+
 
 @dataclass
 class DeviceProtobufMsgEventValue(DataClassORJSONMixin):
     content: Base64EncodedProtobuf
 
 @dataclass
 class DeviceWarningEventValue(DataClassORJSONMixin):
     # TODO: enum for error codes
     # (see resources/res/values-en-rUS/strings.xml in APK)
     code: int
 
-
+@dataclass
 class GeneralParams(DataClassORJSONMixin):
     identifier: str
     groupIdList: list[str]
     groupId: str
     categoryKey: Literal["LawnMower"]
     batchId: str
     gmtCreate: int
@@ -47,21 +62,21 @@
     tenantId: str
     name: str
     thingType: Literal["DEVICE"]
     time: int
     tenantInstanceId: str
     value: Any
 
-
+@dataclass
 class DeviceProtobufMsgEventParams(GeneralParams):
     identifier: Literal["device_protobuf_msg_event"]
     type: Literal["info"]
     value: DeviceProtobufMsgEventValue
 
-
+@dataclass
 class DeviceWarningEventParams(GeneralParams):
     identifier: Literal["device_warning_event"]
     type: Literal["alert"]
     value: DeviceWarningEventValue
 
 @dataclass
 class ThingEventMessage(DataClassORJSONMixin):
```

### Comparing `pyluba-0.0.8/pyluba/data/mqtt/properties.py` & `pyluba-0.0.9/pyluba/data/mqtt/properties.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/data/mqtt/status.py` & `pyluba-0.0.9/pyluba/data/mqtt/status.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/event/event.py` & `pyluba-0.0.9/pyluba/event/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/http/http.py` & `pyluba-0.0.9/pyluba/http/http.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/luba/base.py` & `pyluba-0.0.9/pyluba/luba/base.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/mammotion/devices/luba.py` & `pyluba-0.0.9/pyluba/mammotion/devices/luba.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/mqtt/mqtt.py` & `pyluba-0.0.9/pyluba/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/common_pb2.py` & `pyluba-0.0.9/pyluba/proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/dev_net.proto` & `pyluba-0.0.9/pyluba/proto/dev_net.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/dev_net_pb2.py` & `pyluba-0.0.9/pyluba/proto/dev_net_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/dev_net_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/dev_net_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/luba_msg.proto` & `pyluba-0.0.9/pyluba/proto/luba_msg.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/luba_msg_pb2.py` & `pyluba-0.0.9/pyluba/proto/luba_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/luba_msg_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/luba_msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/luba_mul.proto` & `pyluba-0.0.9/pyluba/proto/luba_mul.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/luba_mul_pb2.py` & `pyluba-0.0.9/pyluba/proto/luba_mul_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/luba_mul_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/luba_mul_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_driver.proto` & `pyluba-0.0.9/pyluba/proto/mctrl_driver.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.py` & `pyluba-0.0.9/pyluba/proto/mctrl_driver_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/mctrl_driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_nav.proto` & `pyluba-0.0.9/pyluba/proto/mctrl_nav.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.py` & `pyluba-0.0.9/pyluba/proto/mctrl_nav_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/mctrl_nav_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_ota.proto` & `pyluba-0.0.9/pyluba/proto/mctrl_ota.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.py` & `pyluba-0.0.9/pyluba/proto/mctrl_ota_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/mctrl_ota_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_pept.proto` & `pyluba-0.0.9/pyluba/proto/mctrl_pept.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.py` & `pyluba-0.0.9/pyluba/proto/mctrl_pept_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/mctrl_pept_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_sys.proto` & `pyluba-0.0.9/pyluba/proto/mctrl_sys.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.py` & `pyluba-0.0.9/pyluba/proto/mctrl_sys_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.pyi` & `pyluba-0.0.9/pyluba/proto/mctrl_sys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/utility/constant/device_constant.py` & `pyluba-0.0.9/pyluba/utility/constant/device_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/utility/periodic.py` & `pyluba-0.0.9/pyluba/utility/periodic.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyluba/utility/rocker_util.py` & `pyluba-0.0.9/pyluba/utility/rocker_util.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.8/pyproject.toml` & `pyluba-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name        = "pyluba"
-version     = "0.0.8"
+version     = "0.0.9"
 license     = "GNU-3.0"
 description = ""
 readme      = "README.md"
 authors     = [
     "Michael Arthur <michael@jumblesoft.co.nz>",
     "Jan Dalheimer <jan@dalheimer.de>"
 ]
```

### Comparing `pyluba-0.0.8/PKG-INFO` & `pyluba-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyluba
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 License: GNU-3.0
 Author: Michael Arthur
 Author-email: michael@jumblesoft.co.nz
 Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

