# Comparing `tmp/ourskyai_platform_api-1.3.3678.tar.gz` & `tmp/ourskyai_platform_api-1.3.3682.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3678.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3682.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3678.tar` & `ourskyai_platform_api-1.3.3682.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     9968 2024-05-27 23:24:31.150924 ourskyai_platform_api-1.3.3678/README.md
--rw-r--r--   0        0        0     6552 2024-05-27 23:24:34.446963 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-27 23:24:34.478964 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   206365 2024-05-27 23:24:34.558965 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-27 23:24:34.598965 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-27 23:24:34.650966 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-27 23:24:34.694966 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-27 23:24:34.738967 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5881 2024-05-27 23:24:34.778967 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-27 23:24:34.814968 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-27 23:24:34.858968 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-27 23:24:34.906969 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     1933 2024-05-27 23:24:34.986970 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/fits_header.py
--rw-r--r--   0        0        0     2158 2024-05-27 23:24:35.030970 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-27 23:24:35.070971 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-27 23:24:35.110971 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-27 23:24:35.198972 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-27 23:24:35.238973 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-27 23:24:35.298974 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-27 23:24:35.346974 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-27 23:24:35.402975 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-27 23:24:35.454975 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-27 23:24:35.502976 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-27 23:24:35.550977 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-27 23:24:35.602977 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-27 23:24:35.650978 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-27 23:24:35.706978 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-27 23:24:35.766979 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-27 23:24:35.846980 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-27 23:24:35.902981 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-27 23:24:35.946981 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2071 2024-05-27 23:24:36.002982 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
--rw-r--r--   0        0        0     2710 2024-05-27 23:24:36.046983 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-27 23:24:36.090983 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-27 23:24:36.146984 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-27 23:24:36.198984 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-27 23:24:36.254985 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-27 23:24:36.378986 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-27 23:24:36.430987 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-27 23:24:36.474988 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-27 23:24:36.550989 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-27 23:24:36.602989 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-27 23:24:36.646990 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-27 23:24:36.694990 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-27 23:24:36.746991 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-27 23:24:36.806992 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-27 23:24:36.846992 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-27 23:24:36.894993 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-27 23:24:36.942993 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5803 2024-05-27 23:24:36.986994 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-27 23:24:37.034994 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-27 23:24:37.078995 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-27 23:24:37.122995 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-27 23:24:37.170996 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-27 23:24:37.210996 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1963 2024-05-27 23:24:37.254997 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_controller_artifact.py
--rw-r--r--   0        0        0     1669 2024-05-27 23:24:37.290998 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-27 23:24:37.354998 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-27 23:24:37.398999 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-27 23:24:37.475000 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-27 23:24:37.539000 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-27 23:24:37.583001 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-27 23:24:37.647002 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-27 23:24:37.695002 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-27 23:24:37.759003 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-27 23:24:37.803004 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-27 23:24:37.855004 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-27 23:24:37.899005 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-27 23:24:37.967006 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-27 23:24:38.011006 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-27 23:24:38.055007 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-27 23:24:38.099007 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-27 23:24:38.151008 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-27 23:24:38.179008 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-27 23:24:38.207008 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-27 23:24:38.271009 ourskyai_platform_api-1.3.3678/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-27 23:24:38.315010 ourskyai_platform_api-1.3.3678/pyproject.toml
--rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3678/PKG-INFO
+-rw-r--r--   0        0        0     9968 2024-05-28 23:34:35.499799 ourskyai_platform_api-1.3.3682/README.md
+-rw-r--r--   0        0        0     6552 2024-05-28 23:34:39.151430 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-28 23:34:39.183427 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   206365 2024-05-28 23:34:39.279417 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-28 23:34:39.327412 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-28 23:34:39.367408 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-28 23:34:39.447400 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-28 23:34:39.487396 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5881 2024-05-28 23:34:39.547390 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-28 23:34:39.595385 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-28 23:34:39.655379 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-28 23:34:39.719373 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-28 23:34:39.775367 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-28 23:34:39.839361 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-28 23:34:39.883356 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-28 23:34:39.951349 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-28 23:34:40.003344 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-28 23:34:40.063338 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-28 23:34:40.111333 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-28 23:34:40.159328 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-28 23:34:40.247319 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-28 23:34:40.303314 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2622 2024-05-28 23:34:40.359308 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-28 23:34:40.415302 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-28 23:34:40.459298 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-28 23:34:40.571287 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-28 23:34:40.619282 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-28 23:34:40.663277 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-28 23:34:40.703273 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-28 23:34:40.755268 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-28 23:34:40.791264 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2071 2024-05-28 23:34:40.843259 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
+-rw-r--r--   0        0        0     2710 2024-05-28 23:34:40.899253 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-28 23:34:40.947249 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-28 23:34:40.991244 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-28 23:34:41.051238 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-28 23:34:41.095234 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-28 23:34:41.163227 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-28 23:34:41.199223 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-28 23:34:41.239219 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-28 23:34:41.299213 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-28 23:34:41.347208 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-28 23:34:41.403202 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-28 23:34:41.459197 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-28 23:34:41.495193 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-28 23:34:41.575185 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-28 23:34:41.615181 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-28 23:34:41.663176 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-28 23:34:41.703172 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-28 23:34:41.735169 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-28 23:34:41.783164 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-28 23:34:41.815161 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-28 23:34:41.871155 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-28 23:34:41.915151 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-28 23:34:41.987144 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1963 2024-05-28 23:34:42.035139 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_controller_artifact.py
+-rw-r--r--   0        0        0     1669 2024-05-28 23:34:42.075135 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-28 23:34:42.115131 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-28 23:34:42.187123 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-28 23:34:42.219120 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-28 23:34:42.279114 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-28 23:34:42.331109 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-28 23:34:42.379104 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-28 23:34:42.451097 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-28 23:34:42.507091 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-28 23:34:42.587083 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-28 23:34:42.631078 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-28 23:34:42.687073 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-28 23:34:42.727069 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-28 23:34:42.771064 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-28 23:34:42.819059 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-28 23:34:42.915050 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-28 23:34:42.963045 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-28 23:34:43.023039 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-28 23:34:43.055036 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-28 23:34:43.107030 ourskyai_platform_api-1.3.3682/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-28 23:34:43.155026 ourskyai_platform_api-1.3.3682/pyproject.toml
+-rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3682/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3678/README.md` & `ourskyai_platform_api-1.3.3682/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3678
-- Package version: 1.3.3678
+- API version: 1.3.3682
+- Package version: 1.3.3682
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3678"
+__version__ = "1.3.3682"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
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
-        self.user_agent = 'OpenAPI-Generator/1.3.3678/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3682/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
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
-               "Version of the API: 1.3.3678\n"\
-               "SDK Package Version: 1.3.3678".\
+               "Version of the API: 1.3.3682\n"\
+               "SDK Package Version: 1.3.3682".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictStr, conlist
 
-class EmptySuccess(BaseModel):
+class V1SetupAction(BaseModel):
     """
-    EmptySuccess
+    Setup Action  # noqa: E501
     """
-    message: Optional[StrictStr] = None
-    __properties = ["message"]
+    action: StrictStr = Field(...)
+    arguments: Optional[conlist(StrictStr)] = None
+    __properties = ["action", "arguments"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -38,34 +39,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> EmptySuccess:
-        """Create an instance of EmptySuccess from a JSON string"""
+    def from_json(cls, json_str: str) -> V1SetupAction:
+        """Create an instance of V1SetupAction from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> EmptySuccess:
-        """Create an instance of EmptySuccess from a dict"""
+    def from_dict(cls, obj: dict) -> V1SetupAction:
+        """Create an instance of V1SetupAction from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return EmptySuccess.parse_obj(obj)
+            return V1SetupAction.parse_obj(obj)
 
-        _obj = EmptySuccess.parse_obj({
-            "message": obj.get("message")
+        _obj = V1SetupAction.parse_obj({
+            "action": obj.get("action"),
+            "arguments": obj.get("arguments")
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/fits_header.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/fits_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/metric_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/shutter_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
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

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/node_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/mount_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
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

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/tracking_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_file_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_controller_artifact.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_controller_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
 
-class V1SetupAction(BaseModel):
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+class V2CompleteObservationRequest(BaseModel):
     """
-    Setup Action  # noqa: E501
+    V2CompleteObservationRequest
     """
-    action: StrictStr = Field(...)
-    arguments: Optional[conlist(StrictStr)] = None
-    __properties = ["action", "arguments"]
+    image_set_id: StrictStr = Field(..., alias="imageSetId")
+    expected_image_count: StrictInt = Field(..., alias="expectedImageCount")
+    __properties = ["imageSetId", "expectedImageCount"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,35 +39,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1SetupAction:
-        """Create an instance of V1SetupAction from a JSON string"""
+    def from_json(cls, json_str: str) -> V2CompleteObservationRequest:
+        """Create an instance of V2CompleteObservationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1SetupAction:
-        """Create an instance of V1SetupAction from a dict"""
+    def from_dict(cls, obj: dict) -> V2CompleteObservationRequest:
+        """Create an instance of V2CompleteObservationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return V1SetupAction.parse_obj(obj)
+            return V2CompleteObservationRequest.parse_obj(obj)
 
-        _obj = V1SetupAction.parse_obj({
-            "action": obj.get("action"),
-            "arguments": obj.get("arguments")
+        _obj = V2CompleteObservationRequest.parse_obj({
+            "image_set_id": obj.get("imageSetId"),
+            "expected_image_count": obj.get("expectedImageCount")
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/models/empty_success.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
-
-class V2CompleteObservationRequest(BaseModel):
+class EmptySuccess(BaseModel):
     """
-    V2CompleteObservationRequest
+    EmptySuccess
     """
-    image_set_id: StrictStr = Field(..., alias="imageSetId")
-    expected_image_count: StrictInt = Field(..., alias="expectedImageCount")
-    __properties = ["imageSetId", "expectedImageCount"]
+    message: Optional[StrictStr] = None
+    __properties = ["message"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,35 +38,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V2CompleteObservationRequest:
-        """Create an instance of V2CompleteObservationRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> EmptySuccess:
+        """Create an instance of EmptySuccess from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V2CompleteObservationRequest:
-        """Create an instance of V2CompleteObservationRequest from a dict"""
+    def from_dict(cls, obj: dict) -> EmptySuccess:
+        """Create an instance of EmptySuccess from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return V2CompleteObservationRequest.parse_obj(obj)
+            return EmptySuccess.parse_obj(obj)
 
-        _obj = V2CompleteObservationRequest.parse_obj({
-            "image_set_id": obj.get("imageSetId"),
-            "expected_image_count": obj.get("expectedImageCount")
+        _obj = EmptySuccess.parse_obj({
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3678/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3682/ourskyai_platform_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3678
+    The version of the OpenAPI document: 1.3.3682
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3678/pyproject.toml` & `ourskyai_platform_api-1.3.3682/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3678"
+version = "1.3.3682"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3678/PKG-INFO` & `ourskyai_platform_api-1.3.3682/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3678
+Version: 1.3.3682
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3678
-- Package version: 1.3.3678
+- API version: 1.3.3682
+- Package version: 1.3.3682
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

