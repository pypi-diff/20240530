# Comparing `tmp/insta360-0.1.2.tar.gz` & `tmp/insta360-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insta360-0.1.2.tar", max compression
+gzip compressed data, was "insta360-0.1.3.tar", max compression
```

## Comparing `insta360-0.1.2.tar` & `insta360-0.1.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    35149 2024-05-25 05:28:01.698637 insta360-0.1.2/LICENSE
--rw-r--r--   0        0        0     8482 2024-05-25 05:28:01.698637 insta360-0.1.2/README.md
--rw-r--r--   0        0        0     8903 2024-05-25 05:28:01.700637 insta360-0.1.2/insta360/osc.py
--rw-r--r--   0        0        0     1943 2024-05-25 05:28:01.700637 insta360-0.1.2/insta360/pb2/active_sensor_device_pb2.py
--rw-r--r--   0        0        0     1291 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/authorization_operation_type_pb2.py
--rw-r--r--   0        0        0     1882 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/authorization_result_pb2.py
--rw-r--r--   0        0        0     1301 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/battery_low_pb2.py
--rw-r--r--   0        0        0     1849 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/battery_pb2.py
--rw-r--r--   0        0        0     1319 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/battery_update_pb2.py
--rw-r--r--   0        0        0     1396 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/bluetooth_pb2.py
--rw-r--r--   0        0        0     1883 2024-05-25 05:28:01.701637 insta360-0.1.2/insta360/pb2/bt_central_notification_pb2.py
--rw-r--r--   0        0        0     2228 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/bt_central_pb2.py
--rw-r--r--   0        0        0     1831 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/button_press_params_pb2.py
--rw-r--r--   0        0        0     4820 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/button_press_pb2.py
--rw-r--r--   0        0        0     1174 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/calibrate_gyro_pb2.py
--rw-r--r--   0        0        0     1841 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/camera_posture_pb2.py
--rw-r--r--   0        0        0     1555 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/camera_submode_pb2.py
--rw-r--r--   0        0        0     1835 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/camera_wifi_connection_result_pb2.py
--rw-r--r--   0        0        0     1280 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/cancel_capture_pb2.py
--rw-r--r--   0        0        0     1425 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/cancel_request_authorization_pb2.py
--rw-r--r--   0        0        0     1316 2024-05-25 05:28:01.702637 insta360-0.1.2/insta360/pb2/capture_auto_split_pb2.py
--rw-r--r--   0        0        0     2569 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/capture_state_pb2.py
--rw-r--r--   0        0        0     2053 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/capture_stopped_pb2.py
--rw-r--r--   0        0        0     2714 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/chargebox_pb2.py
--rw-r--r--   0        0        0     1780 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/charging_command_type_pb2.py
--rw-r--r--   0        0        0     1760 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/check_authorization_pb2.py
--rw-r--r--   0        0        0     1300 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/close_camera_oled_pb2.py
--rw-r--r--   0        0        0     1642 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/current_capture_status_pb2.py
--rw-r--r--   0        0        0     1713 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/darkeis_status_pb2.py
--rw-r--r--   0        0        0     1266 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/delete_file_operation_pb2.py
--rw-r--r--   0        0        0     1345 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/delete_files_pb2.py
--rw-r--r--   0        0        0     1197 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/detect_face_pb2.py
--rw-r--r--   0        0        0     2861 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/download_info_pb2.py
--rw-r--r--   0        0        0     1563 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/error_pb2.py
--rw-r--r--   0        0        0     1625 2024-05-25 05:28:01.703637 insta360-0.1.2/insta360/pb2/exposure_pb2.py
--rw-r--r--   0        0        0     1546 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/exposure_update_pb2.py
--rw-r--r--   0        0        0    19622 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/extra_info_pb2.py
--rw-r--r--   0        0        0     1246 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/file_type_pb2.py
--rw-r--r--   0        0        0     1387 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/fileinfo_list_pb2.py
--rw-r--r--   0        0        0     1207 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/flicker_pb2.py
--rw-r--r--   0        0        0     2618 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/fw_upgrade_state_pb2.py
--rw-r--r--   0        0        0     1905 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_button_press_params_pb2.py
--rw-r--r--   0        0        0     2158 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_current_button_status_pb2.py
--rw-r--r--   0        0        0     2009 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_current_capture_status_pb2.py
--rw-r--r--   0        0        0     2269 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_file_extra_pb2.py
--rw-r--r--   0        0        0     1399 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_file_finish_pb2.py
--rw-r--r--   0        0        0     1521 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_file_list_pb2.py
--rw-r--r--   0        0        0     1423 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_file_pb2.py
--rw-r--r--   0        0        0     1355 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_flowstate_enable_pb2.py
--rw-r--r--   0        0        0     1293 2024-05-25 05:28:01.704637 insta360-0.1.2/insta360/pb2/get_gyro_pb2.py
--rw-r--r--   0        0        0     1189 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_mini_thumbnail_pb2.py
--rw-r--r--   0        0        0     1982 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_multi_photography_options_pb2.py
--rw-r--r--   0        0        0     1523 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_options_pb2.py
--rw-r--r--   0        0        0     1821 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_photography_options_pb2.py
--rw-r--r--   0        0        0     1173 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_sfr_result_pb2.py
--rw-r--r--   0        0        0     1170 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_sfr_status_pb2.py
--rw-r--r--   0        0        0     1486 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_sync_capture_mode_pb2.py
--rw-r--r--   0        0        0     1541 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_timelapse_options_pb2.py
--rw-r--r--   0        0        0     1540 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_whiteblance_status_pb2.py
--rw-r--r--   0        0        0     1525 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/get_wifi_connection_info_pb2.py
--rw-r--r--   0        0        0     1177 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/heat_shell_pb2.py
--rw-r--r--   0        0        0     1520 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/key_pressed_pb2.py
--rw-r--r--   0        0        0     1761 2024-05-25 05:28:01.705637 insta360-0.1.2/insta360/pb2/live_stream_params_update_pb2.py
--rw-r--r--   0        0        0     2204 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/media_pb2.py
--rw-r--r--   0        0        0    10568 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/message_code_pb2.py
--rw-r--r--   0        0        0     2933 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/multi_photography_options_pb2.py
--rw-r--r--   0        0        0     1634 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/offset_state_pb2.py
--rw-r--r--   0        0        0     1282 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/open_camera_oled_pb2.py
--rw-r--r--   0        0        0     1420 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/open_iperf_service_pb2.py
--rw-r--r--   0        0        0    20380 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/options_pb2.py
--rw-r--r--   0        0        0     2658 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/photo_pb2.py
--rw-r--r--   0        0        0    15011 2024-05-25 05:28:01.706637 insta360-0.1.2/insta360/pb2/photography_options_pb2.py
--rw-r--r--   0        0        0     1382 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/request_authorization_pb2.py
--rw-r--r--   0        0        0     1435 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/sd_card_speed_pb2.py
--rw-r--r--   0        0        0     2538 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/sensor_pb2.py
--rw-r--r--   0        0        0     1835 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_access_camera_file_state_pb2.py
--rw-r--r--   0        0        0     1261 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_appid_pb2.py
--rw-r--r--   0        0        0     1894 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_button_press_params_pb2.py
--rw-r--r--   0        0        0     1364 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_charging_data_pb2.py
--rw-r--r--   0        0        0     1361 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_file_extra_pb2.py
--rw-r--r--   0        0        0     1355 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_flowstate_enable_pb2.py
--rw-r--r--   0        0        0     1773 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_key_time_point_pb2.py
--rw-r--r--   0        0        0     1974 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_multi_photography_options_pb2.py
--rw-r--r--   0        0        0     1523 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_options_pb2.py
--rw-r--r--   0        0        0     1814 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_photography_options_pb2.py
--rw-r--r--   0        0        0     1658 2024-05-25 05:28:01.707637 insta360-0.1.2/insta360/pb2/set_standby_mode_pb2.py
--rw-r--r--   0        0        0     1488 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/set_sync_capture_mode_pb2.py
--rw-r--r--   0        0        0     1551 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/set_timelapse_options_pb2.py
--rw-r--r--   0        0        0     1526 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/set_wifi_connection_info_pb2.py
--rw-r--r--   0        0        0     1666 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/set_wifi_seize_pb2.py
--rw-r--r--   0        0        0     1515 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/shutdown_pb2.py
--rw-r--r--   0        0        0     1288 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/start_bullettime_pb2.py
--rw-r--r--   0        0        0     1387 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/start_capture_pb2.py
--rw-r--r--   0        0        0     1223 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/start_hdr_pb2.py
--rw-r--r--   0        0        0     2069 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/start_live_stream_pb2.py
--rw-r--r--   0        0        0     1558 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/start_timelapse_pb2.py
--rw-r--r--   0        0        0     1279 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/start_timeshift_pb2.py
--rw-r--r--   0        0        0     1544 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/stop_bullettime_pb2.py
--rw-r--r--   0        0        0     1639 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/stop_capture_pb2.py
--rw-r--r--   0        0        0     1481 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/stop_hdr_pb2.py
--rw-r--r--   0        0        0     1282 2024-05-25 05:28:01.708637 insta360-0.1.2/insta360/pb2/stop_live_stream_pb2.py
--rw-r--r--   0        0        0     1660 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/stop_timelapse_pb2.py
--rw-r--r--   0        0        0     1533 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/stop_timeshift_pb2.py
--rw-r--r--   0        0        0     1893 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/storage_pb2.py
--rw-r--r--   0        0        0     1364 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/storage_update_pb2.py
--rw-r--r--   0        0        0     1600 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/support_take_photo_on_rec_pb2.py
--rw-r--r--   0        0        0     1637 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/sync_capture_mode_pb2.py
--rw-r--r--   0        0        0     1219 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/sync_capture_mode_update_pb2.py
--rw-r--r--   0        0        0     2406 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/take_picture_pb2.py
--rw-r--r--   0        0        0     1642 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/take_picture_state_update_pb2.py
--rw-r--r--   0        0        0     1523 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/temperature_pb2.py
--rw-r--r--   0        0        0     2180 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/timelapse_pb2.py
--rw-r--r--   0        0        0     1261 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/timelapse_status_update_pb2.py
--rw-r--r--   0        0        0     2097 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/track_pb2.py
--rw-r--r--   0        0        0     1265 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/upload_gps_pb2.py
--rw-r--r--   0        0        0    11289 2024-05-25 05:28:01.709637 insta360-0.1.2/insta360/pb2/video_pb2.py
--rw-r--r--   0        0        0     1311 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/pb2/wifi_connection_info_pb2.py
--rw-r--r--   0        0        0     1388 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/pb2/window_crop_info_pb2.py
--rw-r--r--   0        0        0    40788 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/rtmp.py
--rwxr-xr-x   0        0        0     1201 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/utils/extract-proto-and-compile
--rwxr-xr-x   0        0        0     2905 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/utils/from_binary.py
--rw-r--r--   0        0        0        0 2024-05-25 05:28:01.744636 insta360-0.1.2/insta360/utils/sample_generator.py
--rw-r--r--   0        0        0     1866 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/utils/utilities.py
--rw-r--r--   0        0        0    10246 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/utils/utils/common.py
--rw-r--r--   0        0        0     9109 2024-05-25 05:28:01.710636 insta360-0.1.2/insta360/utils/utils/descpb_to_proto.py
--rw-r--r--   0        0        0      656 2024-05-25 05:28:01.712637 insta360-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9247 1970-01-01 00:00:00.000000 insta360-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-30 15:27:03.538821 insta360-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8410 2024-05-30 15:27:03.538821 insta360-0.1.3/README.md
+-rw-r--r--   0        0        0     8903 2024-05-30 15:27:03.540821 insta360-0.1.3/insta360/osc.py
+-rw-r--r--   0        0        0     1943 2024-05-30 15:27:03.541821 insta360-0.1.3/insta360/pb2/active_sensor_device_pb2.py
+-rw-r--r--   0        0        0     1291 2024-05-30 15:27:03.541821 insta360-0.1.3/insta360/pb2/authorization_operation_type_pb2.py
+-rw-r--r--   0        0        0     1882 2024-05-30 15:27:03.541821 insta360-0.1.3/insta360/pb2/authorization_result_pb2.py
+-rw-r--r--   0        0        0     1301 2024-05-30 15:27:03.541821 insta360-0.1.3/insta360/pb2/battery_low_pb2.py
+-rw-r--r--   0        0        0     1849 2024-05-30 15:27:03.541821 insta360-0.1.3/insta360/pb2/battery_pb2.py
+-rw-r--r--   0        0        0     1319 2024-05-30 15:27:03.541821 insta360-0.1.3/insta360/pb2/battery_update_pb2.py
+-rw-r--r--   0        0        0     1396 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/bluetooth_pb2.py
+-rw-r--r--   0        0        0     1883 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/bt_central_notification_pb2.py
+-rw-r--r--   0        0        0     2228 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/bt_central_pb2.py
+-rw-r--r--   0        0        0     1831 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/button_press_params_pb2.py
+-rw-r--r--   0        0        0     4820 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/button_press_pb2.py
+-rw-r--r--   0        0        0     1174 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/calibrate_gyro_pb2.py
+-rw-r--r--   0        0        0     1841 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/camera_posture_pb2.py
+-rw-r--r--   0        0        0     1555 2024-05-30 15:27:03.542821 insta360-0.1.3/insta360/pb2/camera_submode_pb2.py
+-rw-r--r--   0        0        0     1835 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/camera_wifi_connection_result_pb2.py
+-rw-r--r--   0        0        0     1280 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/cancel_capture_pb2.py
+-rw-r--r--   0        0        0     1425 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/cancel_request_authorization_pb2.py
+-rw-r--r--   0        0        0     1316 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/capture_auto_split_pb2.py
+-rw-r--r--   0        0        0     2569 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/capture_state_pb2.py
+-rw-r--r--   0        0        0     2053 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/capture_stopped_pb2.py
+-rw-r--r--   0        0        0     2714 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/chargebox_pb2.py
+-rw-r--r--   0        0        0     1780 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/charging_command_type_pb2.py
+-rw-r--r--   0        0        0     1760 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/check_authorization_pb2.py
+-rw-r--r--   0        0        0     1300 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/close_camera_oled_pb2.py
+-rw-r--r--   0        0        0     1642 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/current_capture_status_pb2.py
+-rw-r--r--   0        0        0     1713 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/darkeis_status_pb2.py
+-rw-r--r--   0        0        0     1266 2024-05-30 15:27:03.543821 insta360-0.1.3/insta360/pb2/delete_file_operation_pb2.py
+-rw-r--r--   0        0        0     1345 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/delete_files_pb2.py
+-rw-r--r--   0        0        0     1197 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/detect_face_pb2.py
+-rw-r--r--   0        0        0     2861 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/download_info_pb2.py
+-rw-r--r--   0        0        0     1563 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/error_pb2.py
+-rw-r--r--   0        0        0     1625 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/exposure_pb2.py
+-rw-r--r--   0        0        0     1546 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/exposure_update_pb2.py
+-rw-r--r--   0        0        0    19622 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/extra_info_pb2.py
+-rw-r--r--   0        0        0     1246 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/file_type_pb2.py
+-rw-r--r--   0        0        0     1387 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/fileinfo_list_pb2.py
+-rw-r--r--   0        0        0     1207 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/flicker_pb2.py
+-rw-r--r--   0        0        0     2618 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/fw_upgrade_state_pb2.py
+-rw-r--r--   0        0        0     1905 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/get_button_press_params_pb2.py
+-rw-r--r--   0        0        0     2158 2024-05-30 15:27:03.544821 insta360-0.1.3/insta360/pb2/get_current_button_status_pb2.py
+-rw-r--r--   0        0        0     2009 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_current_capture_status_pb2.py
+-rw-r--r--   0        0        0     2269 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_file_extra_pb2.py
+-rw-r--r--   0        0        0     1399 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_file_finish_pb2.py
+-rw-r--r--   0        0        0     1521 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_file_list_pb2.py
+-rw-r--r--   0        0        0     1423 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_file_pb2.py
+-rw-r--r--   0        0        0     1355 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_flowstate_enable_pb2.py
+-rw-r--r--   0        0        0     1293 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_gyro_pb2.py
+-rw-r--r--   0        0        0     1189 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_mini_thumbnail_pb2.py
+-rw-r--r--   0        0        0     1982 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_multi_photography_options_pb2.py
+-rw-r--r--   0        0        0     1523 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_options_pb2.py
+-rw-r--r--   0        0        0     1821 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_photography_options_pb2.py
+-rw-r--r--   0        0        0     1173 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_sfr_result_pb2.py
+-rw-r--r--   0        0        0     1170 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_sfr_status_pb2.py
+-rw-r--r--   0        0        0     1486 2024-05-30 15:27:03.545821 insta360-0.1.3/insta360/pb2/get_sync_capture_mode_pb2.py
+-rw-r--r--   0        0        0     1541 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/get_timelapse_options_pb2.py
+-rw-r--r--   0        0        0     1540 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/get_whiteblance_status_pb2.py
+-rw-r--r--   0        0        0     1525 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/get_wifi_connection_info_pb2.py
+-rw-r--r--   0        0        0     1177 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/heat_shell_pb2.py
+-rw-r--r--   0        0        0     1520 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/key_pressed_pb2.py
+-rw-r--r--   0        0        0     1761 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/live_stream_params_update_pb2.py
+-rw-r--r--   0        0        0     2204 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/media_pb2.py
+-rw-r--r--   0        0        0    10568 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/message_code_pb2.py
+-rw-r--r--   0        0        0     2933 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/multi_photography_options_pb2.py
+-rw-r--r--   0        0        0     1634 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/offset_state_pb2.py
+-rw-r--r--   0        0        0     1282 2024-05-30 15:27:03.546821 insta360-0.1.3/insta360/pb2/open_camera_oled_pb2.py
+-rw-r--r--   0        0        0     1420 2024-05-30 15:27:03.547821 insta360-0.1.3/insta360/pb2/open_iperf_service_pb2.py
+-rw-r--r--   0        0        0    20380 2024-05-30 15:27:03.547821 insta360-0.1.3/insta360/pb2/options_pb2.py
+-rw-r--r--   0        0        0     2658 2024-05-30 15:27:03.547821 insta360-0.1.3/insta360/pb2/photo_pb2.py
+-rw-r--r--   0        0        0    15011 2024-05-30 15:27:03.547821 insta360-0.1.3/insta360/pb2/photography_options_pb2.py
+-rw-r--r--   0        0        0     1382 2024-05-30 15:27:03.547821 insta360-0.1.3/insta360/pb2/request_authorization_pb2.py
+-rw-r--r--   0        0        0     1435 2024-05-30 15:27:03.547821 insta360-0.1.3/insta360/pb2/sd_card_speed_pb2.py
+-rw-r--r--   0        0        0     2538 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/sensor_pb2.py
+-rw-r--r--   0        0        0     1835 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_access_camera_file_state_pb2.py
+-rw-r--r--   0        0        0     1261 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_appid_pb2.py
+-rw-r--r--   0        0        0     1894 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_button_press_params_pb2.py
+-rw-r--r--   0        0        0     1364 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_charging_data_pb2.py
+-rw-r--r--   0        0        0     1361 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_file_extra_pb2.py
+-rw-r--r--   0        0        0     1355 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_flowstate_enable_pb2.py
+-rw-r--r--   0        0        0     1773 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_key_time_point_pb2.py
+-rw-r--r--   0        0        0     1974 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_multi_photography_options_pb2.py
+-rw-r--r--   0        0        0     1523 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_options_pb2.py
+-rw-r--r--   0        0        0     1814 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_photography_options_pb2.py
+-rw-r--r--   0        0        0     1658 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_standby_mode_pb2.py
+-rw-r--r--   0        0        0     1488 2024-05-30 15:27:03.548821 insta360-0.1.3/insta360/pb2/set_sync_capture_mode_pb2.py
+-rw-r--r--   0        0        0     1551 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/set_timelapse_options_pb2.py
+-rw-r--r--   0        0        0     1526 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/set_wifi_connection_info_pb2.py
+-rw-r--r--   0        0        0     1666 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/set_wifi_seize_pb2.py
+-rw-r--r--   0        0        0     1515 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/shutdown_pb2.py
+-rw-r--r--   0        0        0     1288 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/start_bullettime_pb2.py
+-rw-r--r--   0        0        0     1387 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/start_capture_pb2.py
+-rw-r--r--   0        0        0     1223 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/start_hdr_pb2.py
+-rw-r--r--   0        0        0     2069 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/start_live_stream_pb2.py
+-rw-r--r--   0        0        0     1558 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/start_timelapse_pb2.py
+-rw-r--r--   0        0        0     1279 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/start_timeshift_pb2.py
+-rw-r--r--   0        0        0     1544 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/stop_bullettime_pb2.py
+-rw-r--r--   0        0        0     1639 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/stop_capture_pb2.py
+-rw-r--r--   0        0        0     1481 2024-05-30 15:27:03.549821 insta360-0.1.3/insta360/pb2/stop_hdr_pb2.py
+-rw-r--r--   0        0        0     1282 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/stop_live_stream_pb2.py
+-rw-r--r--   0        0        0     1660 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/stop_timelapse_pb2.py
+-rw-r--r--   0        0        0     1533 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/stop_timeshift_pb2.py
+-rw-r--r--   0        0        0     1893 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/storage_pb2.py
+-rw-r--r--   0        0        0     1364 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/storage_update_pb2.py
+-rw-r--r--   0        0        0     1600 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/support_take_photo_on_rec_pb2.py
+-rw-r--r--   0        0        0     1637 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/sync_capture_mode_pb2.py
+-rw-r--r--   0        0        0     1219 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/sync_capture_mode_update_pb2.py
+-rw-r--r--   0        0        0     2406 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/take_picture_pb2.py
+-rw-r--r--   0        0        0     1642 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/take_picture_state_update_pb2.py
+-rw-r--r--   0        0        0     1523 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/temperature_pb2.py
+-rw-r--r--   0        0        0     2180 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/timelapse_pb2.py
+-rw-r--r--   0        0        0     1261 2024-05-30 15:27:03.550821 insta360-0.1.3/insta360/pb2/timelapse_status_update_pb2.py
+-rw-r--r--   0        0        0     2097 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/pb2/track_pb2.py
+-rw-r--r--   0        0        0     1265 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/pb2/upload_gps_pb2.py
+-rw-r--r--   0        0        0    11289 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/pb2/video_pb2.py
+-rw-r--r--   0        0        0     1311 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/pb2/wifi_connection_info_pb2.py
+-rw-r--r--   0        0        0     1388 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/pb2/window_crop_info_pb2.py
+-rw-r--r--   0        0        0    40788 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/rtmp.py
+-rwxr-xr-x   0        0        0     1201 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/utils/extract-proto-and-compile
+-rwxr-xr-x   0        0        0     2905 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/utils/from_binary.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:27:03.593821 insta360-0.1.3/insta360/utils/sample_generator.py
+-rw-r--r--   0        0        0     1866 2024-05-30 15:27:03.551821 insta360-0.1.3/insta360/utils/utilities.py
+-rw-r--r--   0        0        0    10246 2024-05-30 15:27:03.552821 insta360-0.1.3/insta360/utils/utils/common.py
+-rw-r--r--   0        0        0     9109 2024-05-30 15:27:03.552821 insta360-0.1.3/insta360/utils/utils/descpb_to_proto.py
+-rw-r--r--   0        0        0      658 2024-05-30 15:27:03.553821 insta360-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9069 1970-01-01 00:00:00.000000 insta360-0.1.3/PKG-INFO
```

### Comparing `insta360-0.1.2/LICENSE` & `insta360-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/README.md` & `insta360-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# insta360-api
+# insta360
 
 This python package implements both [RTMP (Real-Time Messaging Protocol)](https://en.wikipedia.org/wiki/Real-Time_Messaging_Protocol) and [OSC (Open Spherical Camera)](https://developers.google.com/streetview/open-spherical-camera) protocols for interacting with Insta360 cameras.
 
 While OSC is an open standard for controlling spherical cameras, RTMP is a proprietary protocol used by Insta360 cameras for many of its core functionalities. This package aims to provide a unified interface for interacting with Insta360 cameras by reverse engineering the proprietary RTMP protocol and implementing the open OSC protocol.
 
 The RTMP protocol is implemented by reverse engineering the communication between Insta360 cameras and the official Android app. OSC is implemented with respect to the official [OSC API v2 specification](https://developers.google.com/streetview/open-spherical-camera).
 
-More info here: [Insta360: WiFi protocol reverse engineering](https://www.rigacci.org/wiki/doku.php/doc/appunti/hardware/insta360_one_rs_wifi_reverse_engineering).
+Documentation is available at [https://insta360.whitebox.aero](https://insta360.whitebox.aero).
 
 # Compatibility
 
 While the package is developed and tested with Insta360 X3 and X4, it should work with other Insta360 cameras as well. If you find any compatibility issues, please open an issue. PRs are also welcome to improve the compatibility with other Insta360 cameras.
 
 Here is a list all the functions that are implemented and tested and their compatibility with different Insta360 cameras:
```

### Comparing `insta360-0.1.2/insta360/osc.py` & `insta360-0.1.3/insta360/osc.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/active_sensor_device_pb2.py` & `insta360-0.1.3/insta360/pb2/active_sensor_device_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/authorization_operation_type_pb2.py` & `insta360-0.1.3/insta360/pb2/authorization_operation_type_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/authorization_result_pb2.py` & `insta360-0.1.3/insta360/pb2/authorization_result_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/battery_low_pb2.py` & `insta360-0.1.3/insta360/pb2/battery_low_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/battery_pb2.py` & `insta360-0.1.3/insta360/pb2/battery_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/battery_update_pb2.py` & `insta360-0.1.3/insta360/pb2/battery_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/bluetooth_pb2.py` & `insta360-0.1.3/insta360/pb2/bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/bt_central_notification_pb2.py` & `insta360-0.1.3/insta360/pb2/bt_central_notification_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/bt_central_pb2.py` & `insta360-0.1.3/insta360/pb2/bt_central_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/button_press_params_pb2.py` & `insta360-0.1.3/insta360/pb2/button_press_params_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/button_press_pb2.py` & `insta360-0.1.3/insta360/pb2/button_press_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/calibrate_gyro_pb2.py` & `insta360-0.1.3/insta360/pb2/calibrate_gyro_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/camera_posture_pb2.py` & `insta360-0.1.3/insta360/pb2/camera_posture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/camera_submode_pb2.py` & `insta360-0.1.3/insta360/pb2/camera_submode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/camera_wifi_connection_result_pb2.py` & `insta360-0.1.3/insta360/pb2/camera_wifi_connection_result_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/cancel_capture_pb2.py` & `insta360-0.1.3/insta360/pb2/cancel_capture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/cancel_request_authorization_pb2.py` & `insta360-0.1.3/insta360/pb2/cancel_request_authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/capture_auto_split_pb2.py` & `insta360-0.1.3/insta360/pb2/capture_auto_split_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/capture_state_pb2.py` & `insta360-0.1.3/insta360/pb2/capture_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/capture_stopped_pb2.py` & `insta360-0.1.3/insta360/pb2/capture_stopped_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/chargebox_pb2.py` & `insta360-0.1.3/insta360/pb2/chargebox_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/charging_command_type_pb2.py` & `insta360-0.1.3/insta360/pb2/charging_command_type_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/check_authorization_pb2.py` & `insta360-0.1.3/insta360/pb2/check_authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/close_camera_oled_pb2.py` & `insta360-0.1.3/insta360/pb2/close_camera_oled_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/current_capture_status_pb2.py` & `insta360-0.1.3/insta360/pb2/current_capture_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/darkeis_status_pb2.py` & `insta360-0.1.3/insta360/pb2/darkeis_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/delete_file_operation_pb2.py` & `insta360-0.1.3/insta360/pb2/delete_file_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/delete_files_pb2.py` & `insta360-0.1.3/insta360/pb2/delete_files_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/detect_face_pb2.py` & `insta360-0.1.3/insta360/pb2/detect_face_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/download_info_pb2.py` & `insta360-0.1.3/insta360/pb2/download_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/error_pb2.py` & `insta360-0.1.3/insta360/pb2/error_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/exposure_pb2.py` & `insta360-0.1.3/insta360/pb2/exposure_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/exposure_update_pb2.py` & `insta360-0.1.3/insta360/pb2/exposure_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/extra_info_pb2.py` & `insta360-0.1.3/insta360/pb2/extra_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/file_type_pb2.py` & `insta360-0.1.3/insta360/pb2/file_type_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/fileinfo_list_pb2.py` & `insta360-0.1.3/insta360/pb2/fileinfo_list_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/flicker_pb2.py` & `insta360-0.1.3/insta360/pb2/flicker_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/fw_upgrade_state_pb2.py` & `insta360-0.1.3/insta360/pb2/fw_upgrade_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_button_press_params_pb2.py` & `insta360-0.1.3/insta360/pb2/get_button_press_params_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_current_button_status_pb2.py` & `insta360-0.1.3/insta360/pb2/get_current_button_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_current_capture_status_pb2.py` & `insta360-0.1.3/insta360/pb2/get_current_capture_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_file_extra_pb2.py` & `insta360-0.1.3/insta360/pb2/get_file_extra_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_file_finish_pb2.py` & `insta360-0.1.3/insta360/pb2/get_file_finish_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_file_list_pb2.py` & `insta360-0.1.3/insta360/pb2/get_file_list_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_file_pb2.py` & `insta360-0.1.3/insta360/pb2/get_file_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_flowstate_enable_pb2.py` & `insta360-0.1.3/insta360/pb2/get_flowstate_enable_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_gyro_pb2.py` & `insta360-0.1.3/insta360/pb2/get_gyro_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_mini_thumbnail_pb2.py` & `insta360-0.1.3/insta360/pb2/get_mini_thumbnail_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_multi_photography_options_pb2.py` & `insta360-0.1.3/insta360/pb2/get_multi_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_options_pb2.py` & `insta360-0.1.3/insta360/pb2/get_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_photography_options_pb2.py` & `insta360-0.1.3/insta360/pb2/get_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_sfr_result_pb2.py` & `insta360-0.1.3/insta360/pb2/get_sfr_result_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_sfr_status_pb2.py` & `insta360-0.1.3/insta360/pb2/get_sfr_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_sync_capture_mode_pb2.py` & `insta360-0.1.3/insta360/pb2/get_sync_capture_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_timelapse_options_pb2.py` & `insta360-0.1.3/insta360/pb2/get_timelapse_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_whiteblance_status_pb2.py` & `insta360-0.1.3/insta360/pb2/get_whiteblance_status_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/get_wifi_connection_info_pb2.py` & `insta360-0.1.3/insta360/pb2/get_wifi_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/heat_shell_pb2.py` & `insta360-0.1.3/insta360/pb2/heat_shell_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/key_pressed_pb2.py` & `insta360-0.1.3/insta360/pb2/key_pressed_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/live_stream_params_update_pb2.py` & `insta360-0.1.3/insta360/pb2/live_stream_params_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/media_pb2.py` & `insta360-0.1.3/insta360/pb2/media_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/message_code_pb2.py` & `insta360-0.1.3/insta360/pb2/message_code_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/multi_photography_options_pb2.py` & `insta360-0.1.3/insta360/pb2/multi_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/offset_state_pb2.py` & `insta360-0.1.3/insta360/pb2/offset_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/open_camera_oled_pb2.py` & `insta360-0.1.3/insta360/pb2/open_camera_oled_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/open_iperf_service_pb2.py` & `insta360-0.1.3/insta360/pb2/open_iperf_service_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/options_pb2.py` & `insta360-0.1.3/insta360/pb2/options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/photo_pb2.py` & `insta360-0.1.3/insta360/pb2/photo_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/photography_options_pb2.py` & `insta360-0.1.3/insta360/pb2/photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/request_authorization_pb2.py` & `insta360-0.1.3/insta360/pb2/request_authorization_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/sd_card_speed_pb2.py` & `insta360-0.1.3/insta360/pb2/sd_card_speed_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/sensor_pb2.py` & `insta360-0.1.3/insta360/pb2/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_access_camera_file_state_pb2.py` & `insta360-0.1.3/insta360/pb2/set_access_camera_file_state_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_appid_pb2.py` & `insta360-0.1.3/insta360/pb2/set_appid_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_button_press_params_pb2.py` & `insta360-0.1.3/insta360/pb2/set_button_press_params_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_charging_data_pb2.py` & `insta360-0.1.3/insta360/pb2/set_charging_data_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_file_extra_pb2.py` & `insta360-0.1.3/insta360/pb2/set_file_extra_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_flowstate_enable_pb2.py` & `insta360-0.1.3/insta360/pb2/set_flowstate_enable_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_key_time_point_pb2.py` & `insta360-0.1.3/insta360/pb2/set_key_time_point_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_multi_photography_options_pb2.py` & `insta360-0.1.3/insta360/pb2/set_multi_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_options_pb2.py` & `insta360-0.1.3/insta360/pb2/set_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_photography_options_pb2.py` & `insta360-0.1.3/insta360/pb2/set_photography_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_standby_mode_pb2.py` & `insta360-0.1.3/insta360/pb2/set_standby_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_sync_capture_mode_pb2.py` & `insta360-0.1.3/insta360/pb2/set_sync_capture_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_timelapse_options_pb2.py` & `insta360-0.1.3/insta360/pb2/set_timelapse_options_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_wifi_connection_info_pb2.py` & `insta360-0.1.3/insta360/pb2/set_wifi_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/set_wifi_seize_pb2.py` & `insta360-0.1.3/insta360/pb2/set_wifi_seize_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/shutdown_pb2.py` & `insta360-0.1.3/insta360/pb2/shutdown_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/start_bullettime_pb2.py` & `insta360-0.1.3/insta360/pb2/start_bullettime_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/start_capture_pb2.py` & `insta360-0.1.3/insta360/pb2/start_capture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/start_hdr_pb2.py` & `insta360-0.1.3/insta360/pb2/start_hdr_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/start_live_stream_pb2.py` & `insta360-0.1.3/insta360/pb2/start_live_stream_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/start_timelapse_pb2.py` & `insta360-0.1.3/insta360/pb2/start_timelapse_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/start_timeshift_pb2.py` & `insta360-0.1.3/insta360/pb2/start_timeshift_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/stop_bullettime_pb2.py` & `insta360-0.1.3/insta360/pb2/stop_bullettime_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/stop_capture_pb2.py` & `insta360-0.1.3/insta360/pb2/stop_capture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/stop_hdr_pb2.py` & `insta360-0.1.3/insta360/pb2/stop_hdr_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/stop_live_stream_pb2.py` & `insta360-0.1.3/insta360/pb2/stop_live_stream_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/stop_timelapse_pb2.py` & `insta360-0.1.3/insta360/pb2/stop_timelapse_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/stop_timeshift_pb2.py` & `insta360-0.1.3/insta360/pb2/stop_timeshift_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/storage_pb2.py` & `insta360-0.1.3/insta360/pb2/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/storage_update_pb2.py` & `insta360-0.1.3/insta360/pb2/storage_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/support_take_photo_on_rec_pb2.py` & `insta360-0.1.3/insta360/pb2/support_take_photo_on_rec_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/sync_capture_mode_pb2.py` & `insta360-0.1.3/insta360/pb2/sync_capture_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/sync_capture_mode_update_pb2.py` & `insta360-0.1.3/insta360/pb2/sync_capture_mode_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/take_picture_pb2.py` & `insta360-0.1.3/insta360/pb2/take_picture_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/take_picture_state_update_pb2.py` & `insta360-0.1.3/insta360/pb2/take_picture_state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/temperature_pb2.py` & `insta360-0.1.3/insta360/pb2/temperature_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/timelapse_pb2.py` & `insta360-0.1.3/insta360/pb2/timelapse_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/timelapse_status_update_pb2.py` & `insta360-0.1.3/insta360/pb2/timelapse_status_update_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/track_pb2.py` & `insta360-0.1.3/insta360/pb2/track_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/upload_gps_pb2.py` & `insta360-0.1.3/insta360/pb2/upload_gps_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/video_pb2.py` & `insta360-0.1.3/insta360/pb2/video_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/wifi_connection_info_pb2.py` & `insta360-0.1.3/insta360/pb2/wifi_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/pb2/window_crop_info_pb2.py` & `insta360-0.1.3/insta360/pb2/window_crop_info_pb2.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/rtmp.py` & `insta360-0.1.3/insta360/rtmp.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/utils/extract-proto-and-compile` & `insta360-0.1.3/insta360/utils/extract-proto-and-compile`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/utils/from_binary.py` & `insta360-0.1.3/insta360/utils/from_binary.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/utils/utilities.py` & `insta360-0.1.3/insta360/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/utils/utils/common.py` & `insta360-0.1.3/insta360/utils/utils/common.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/insta360/utils/utils/descpb_to_proto.py` & `insta360-0.1.3/insta360/utils/utils/descpb_to_proto.py`

 * *Files identical despite different names*

### Comparing `insta360-0.1.2/pyproject.toml` & `insta360-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "insta360"
-version = "0.1.2"
+version = "0.1.3"
 description = "APIs to interact with insta360 cameras."
 authors = ["avilabss <contact@avilabs.net>", "Niccolo Rigacci <niccolo@rigacci.org>", "WhiteBox <contact@whitebox.aero>"]
 license = "GNU General Public License v3.0 or later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
+python = ">=3.10.0"
 requests = "^2.31.0"
 pydantic = "^2.7.1"
 protobuf = "^5.26.1"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.5.0"
 mkdocs = "^1.6.0"
```

### Comparing `insta360-0.1.2/PKG-INFO` & `insta360-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: insta360
-Version: 0.1.2
+Version: 0.1.3
 Summary: APIs to interact with insta360 cameras.
 License: GPL-3.0-or-later
 Author: avilabss
 Author-email: contact@avilabs.net
-Requires-Python: >=3.8.0,<4.0.0
+Requires-Python: >=3.10.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: protobuf (>=5.26.1,<6.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# insta360-api
+# insta360
 
 This python package implements both [RTMP (Real-Time Messaging Protocol)](https://en.wikipedia.org/wiki/Real-Time_Messaging_Protocol) and [OSC (Open Spherical Camera)](https://developers.google.com/streetview/open-spherical-camera) protocols for interacting with Insta360 cameras.
 
 While OSC is an open standard for controlling spherical cameras, RTMP is a proprietary protocol used by Insta360 cameras for many of its core functionalities. This package aims to provide a unified interface for interacting with Insta360 cameras by reverse engineering the proprietary RTMP protocol and implementing the open OSC protocol.
 
 The RTMP protocol is implemented by reverse engineering the communication between Insta360 cameras and the official Android app. OSC is implemented with respect to the official [OSC API v2 specification](https://developers.google.com/streetview/open-spherical-camera).
 
-More info here: [Insta360: WiFi protocol reverse engineering](https://www.rigacci.org/wiki/doku.php/doc/appunti/hardware/insta360_one_rs_wifi_reverse_engineering).
+Documentation is available at [https://insta360.whitebox.aero](https://insta360.whitebox.aero).
 
 # Compatibility
 
 While the package is developed and tested with Insta360 X3 and X4, it should work with other Insta360 cameras as well. If you find any compatibility issues, please open an issue. PRs are also welcome to improve the compatibility with other Insta360 cameras.
 
 Here is a list all the functions that are implemented and tested and their compatibility with different Insta360 cameras:
```

