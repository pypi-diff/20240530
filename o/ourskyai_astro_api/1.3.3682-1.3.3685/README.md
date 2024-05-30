# Comparing `tmp/ourskyai_astro_api-1.3.3682.tar.gz` & `tmp/ourskyai_astro_api-1.3.3685.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3682.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3685.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3682.tar` & `ourskyai_astro_api-1.3.3685.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    11541 2024-05-28 23:34:35.555793 ourskyai_astro_api-1.3.3682/README.md
--rw-r--r--   0        0        0     6292 2024-05-28 23:34:39.259419 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-28 23:34:39.295415 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   260295 2024-05-28 23:34:39.395405 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-28 23:34:39.443400 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-28 23:34:39.499395 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-28 23:34:39.547390 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-28 23:34:39.591385 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5651 2024-05-28 23:34:39.639381 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-28 23:34:39.707374 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-28 23:34:39.755369 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-28 23:34:39.807364 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     2092 2024-05-28 23:34:39.859358 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_city.py
--rw-r--r--   0        0        0     4308 2024-05-28 23:34:39.903354 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_item.py
--rw-r--r--   0        0        0     2527 2024-05-28 23:34:39.967347 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
--rw-r--r--   0        0        0     2551 2024-05-28 23:34:40.003344 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
--rw-r--r--   0        0        0     2947 2024-05-28 23:34:40.075337 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
--rw-r--r--   0        0        0     1904 2024-05-28 23:34:40.127331 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-28 23:34:40.199324 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-28 23:34:40.255318 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-28 23:34:40.299314 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-28 23:34:40.331311 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-28 23:34:40.371307 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-28 23:34:40.455298 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-28 23:34:40.503293 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-28 23:34:40.543289 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-28 23:34:40.607283 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-28 23:34:40.671276 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-28 23:34:40.715272 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-28 23:34:40.759268 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-28 23:34:40.827261 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-28 23:34:40.895254 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-28 23:34:40.951248 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-28 23:34:41.019241 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-28 23:34:41.059237 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-28 23:34:41.115232 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-28 23:34:41.175226 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-28 23:34:41.223221 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-28 23:34:41.267216 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-28 23:34:41.315211 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-28 23:34:41.351208 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-28 23:34:41.383205 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-28 23:34:41.427200 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-28 23:34:41.479195 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-28 23:34:41.535189 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-28 23:34:41.579185 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-28 23:34:41.615181 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-28 23:34:41.671175 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-28 23:34:41.719171 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-28 23:34:41.779164 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-28 23:34:41.847158 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-28 23:34:41.895153 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-28 23:34:41.955147 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-28 23:34:42.007141 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-28 23:34:42.051137 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-28 23:34:42.095133 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-28 23:34:42.159126 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-28 23:34:42.219120 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-28 23:34:42.303112 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-28 23:34:42.351107 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-28 23:34:42.407101 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-28 23:34:42.451097 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-28 23:34:42.499092 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-28 23:34:42.555086 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-28 23:34:42.603081 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-28 23:34:42.655076 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-28 23:34:42.751066 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-28 23:34:42.815060 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-28 23:34:42.859055 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-28 23:34:42.915050 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-28 23:34:42.955046 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-28 23:34:42.991042 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-28 23:34:43.023039 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-28 23:34:43.067034 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-28 23:34:43.099031 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-28 23:34:43.175023 ourskyai_astro_api-1.3.3682/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-28 23:34:43.231018 ourskyai_astro_api-1.3.3682/pyproject.toml
--rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3682/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-05-29 22:34:23.861472 ourskyai_astro_api-1.3.3685/README.md
+-rw-r--r--   0        0        0     6292 2024-05-29 22:34:27.745483 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-29 22:34:27.777484 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   260295 2024-05-29 22:34:27.897484 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-29 22:34:27.985484 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-29 22:34:28.037485 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-29 22:34:28.085485 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-29 22:34:28.153485 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5651 2024-05-29 22:34:28.233485 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-29 22:34:28.269485 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-29 22:34:28.321486 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-29 22:34:28.365486 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     2092 2024-05-29 22:34:28.409486 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_city.py
+-rw-r--r--   0        0        0     4308 2024-05-29 22:34:28.477486 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-29 22:34:28.517486 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-29 22:34:28.561486 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2947 2024-05-29 22:34:28.609487 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-29 22:34:28.649487 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-29 22:34:28.693487 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-29 22:34:28.737487 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-29 22:34:28.817487 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-29 22:34:28.869488 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-29 22:34:28.961488 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-29 22:34:29.013488 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-29 22:34:29.045488 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-29 22:34:29.109488 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-29 22:34:29.201489 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-29 22:34:29.281489 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-29 22:34:29.325489 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-29 22:34:29.393489 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-29 22:34:29.429489 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-29 22:34:29.505490 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-29 22:34:29.553490 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-29 22:34:29.605490 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-29 22:34:29.649490 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-29 22:34:29.681491 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-29 22:34:29.729491 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-05-29 22:34:29.789491 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-29 22:34:29.841491 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-29 22:34:29.873491 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-29 22:34:29.945491 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-29 22:34:29.993492 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-29 22:34:30.057492 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-29 22:34:30.097492 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-29 22:34:30.165492 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-29 22:34:30.209492 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-29 22:34:30.249493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-29 22:34:30.317493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-29 22:34:30.349493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-29 22:34:30.389493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-29 22:34:30.437493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-29 22:34:30.489493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-29 22:34:30.545493 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-29 22:34:30.629494 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-29 22:34:30.693494 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-29 22:34:30.757494 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-29 22:34:30.805494 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-29 22:34:30.849495 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-29 22:34:30.897495 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-29 22:34:30.953495 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-29 22:34:31.029495 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-29 22:34:31.077495 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-29 22:34:31.137496 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-29 22:34:31.185496 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-29 22:34:31.225496 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-29 22:34:31.273496 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-29 22:34:31.321496 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-29 22:34:31.357496 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-29 22:34:31.393497 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-29 22:34:31.437497 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-29 22:34:31.481497 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-29 22:34:31.549497 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-29 22:34:31.629497 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-29 22:34:31.701498 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:34:31.729498 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-29 22:34:31.761498 ourskyai_astro_api-1.3.3685/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-29 22:34:31.841498 ourskyai_astro_api-1.3.3685/pyproject.toml
+-rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3685/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3682/README.md` & `ourskyai_astro_api-1.3.3685/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3682
-- Package version: 1.3.3682
+- API version: 1.3.3685
+- Package version: 1.3.3685
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3682"
+__version__ = "1.3.3685"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3682/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3685/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3682\n"\
-               "SDK Package Version: 1.3.3682".\
+               "Version of the API: 1.3.3685\n"\
+               "SDK Package Version: 1.3.3685".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/asset_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_city.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_city.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_item.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/daily_weather_forecast_list_response.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/daily_weather_forecast_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/filter_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/fits_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/shutter_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MountType(str, Enum):
+class ShutterType(str, Enum):
     """
-    MountType
+    ShutterType
     """
 
     """
     allowed enum values
     """
-    ALT_AZ = 'ALT_AZ'
-    EQUITORIAL = 'EQUITORIAL'
+    ROLLING = 'ROLLING'
+    GLOBAL = 'GLOBAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> MountType:
-        """Create an instance of MountType from a JSON string"""
-        return MountType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> ShutterType:
+        """Create an instance of ShutterType from a JSON string"""
+        return ShutterType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/mount_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ShutterType(str, Enum):
+class MountType(str, Enum):
     """
-    ShutterType
+    MountType
     """
 
     """
     allowed enum values
     """
-    ROLLING = 'ROLLING'
-    GLOBAL = 'GLOBAL'
+    ALT_AZ = 'ALT_AZ'
+    EQUITORIAL = 'EQUITORIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> ShutterType:
-        """Create an instance of ShutterType from a JSON string"""
-        return ShutterType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> MountType:
+        """Create an instance of MountType from a JSON string"""
+        return MountType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/tracking_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3682/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3685/ourskyai_astro_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3682
+    The version of the OpenAPI document: 1.3.3685
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3682/pyproject.toml` & `ourskyai_astro_api-1.3.3685/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3682"
+version = "1.3.3685"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3682/PKG-INFO` & `ourskyai_astro_api-1.3.3685/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3682
+Version: 1.3.3685
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3682
-- Package version: 1.3.3682
+- API version: 1.3.3685
+- Package version: 1.3.3685
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

