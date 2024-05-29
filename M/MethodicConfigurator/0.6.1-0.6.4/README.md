# Comparing `tmp/methodicconfigurator-0.6.1.tar.gz` & `tmp/methodicconfigurator-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodicconfigurator-0.6.1.tar", last modified: Thu May 16 12:17:07 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.6.4.tar", last modified: Wed May 29 22:20:38 2024, max compression
```

## Comparing `methodicconfigurator-0.6.1.tar` & `methodicconfigurator-0.6.4.tar`

### file list

```diff
@@ -1,309 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.135321 methodicconfigurator-0.6.1/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27852 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/annotate_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4993 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29041 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_configuration_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_vehicle_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    31001 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/backend_mavftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/battery_cell_voltages.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/common_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_connection_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_directory_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    37652 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/get_release_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/tempcal_imu.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23766 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 12:17:07.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:16:59.000000 methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-16 12:16:41.000000 methodicconfigurator-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:17:07.195321 methodicconfigurator-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.131321 methodicconfigurator-0.6.1/vehicle_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.131321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.147321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/
--rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1998191 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
--rw-r--r--   0 runner    (1001) docker     (127)    78746 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.131321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.159321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    20075 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.171321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.183321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:17:07.191321 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-16 12:16:42.000000 methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.317293 methodicconfigurator-0.6.4/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28737 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/annotate_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4997 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30690 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_configuration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_vehicle_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31001 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_mavftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/battery_cell_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37652 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/get_release_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/tempcal_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24202 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:20:31.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.309292 methodicconfigurator-0.6.4/vehicle_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.309292 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.337293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/47_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/48_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/50_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1998191 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78746 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
+-rw-r--r--   0 runner    (1001) docker     (127)  5007981 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.313293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.349293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.357293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.369293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/50_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.6.1/LICENSE.md` & `methodicconfigurator-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_icon.png` & `methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_icon.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/ArduPilot_logo.png` & `methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_logo.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/annotate_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 
 def arg_parser():
     parser = argparse.ArgumentParser(description='Fetches on-line ArduPilot parameter documentation and adds it to the '
                                      'specified file or to all *.param and *.parm files in the specified directory.')
     parser.add_argument('target',
                         help='The target file or directory.',
                         )
+    parser.add_argument('-d', '--delete-documentation-annotations',
+                        action='store_true',
+                        help='Delete parameter documentation annotations (comments above parameters). Defaults to %(default)s',
+                        )
     parser.add_argument('-s', '--sort',
                         choices=['none', 'missionplanner', 'mavproxy'],
                         default='none',
                         help='Sort the parameters in the file. Defaults to not sorting.',
                         )
     parser.add_argument('-t', '--vehicle-type',
                         choices=['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
@@ -60,15 +64,15 @@
                         help='The type of the vehicle. Defaults to ArduCopter',
                         )
     parser.add_argument('-m', '--max-line-length',
                         type=int, default=100,
                         help='Maximum documentation line length. Defaults to %(default)s',
                         )
     parser.add_argument('--verbose', action='store_true',
-                        help='Increase output verbosity, print ReadOnly parameter list. Defaults to false',
+                        help='Increase output verbosity, print ReadOnly parameter list. Defaults to %(default)s',
                         )
     parser.add_argument('-v', '--version', action='version', version=f'%(prog)s {VERSION}',
                         help='Display version information and exit.',
                         )
 
     args = parser.parse_args()
 
@@ -226,15 +230,16 @@
 
         Returns:
         None
         """
         if not formatted_params:
             return
         try:
-            with open(filename_out, "w", encoding="utf-8") as output_file:
+            # Ensure newline character is LF, even on windows
+            with open(filename_out, "w", encoding="utf-8", newline='\n') as output_file:
                 for line in formatted_params:
                     output_file.write(line + "\n")
         except IOError as e:
             raise SystemExit(f"ERROR: writing to file {filename_out}: {e}") from e
 
     @staticmethod
     def print_out(formatted_params: List[str], name: str) -> None:
@@ -508,15 +513,16 @@
     if param_len > PARAM_NAME_MAX_LEN:
         logging.critical("Too long parameter name on line %d in file %s", line_nr, filename)
         raise SystemExit("Too long parameter name")
     return param_name
 
 
 def update_parameter_documentation(doc: Dict[str, Any], target: str = '.',
-                                   sort_type: str = 'none', param_default_dict: Optional[Dict] = None) -> None:
+                                   sort_type: str = 'none', param_default_dict: Optional[Dict] = None,
+                                   delete_documentation_annotations = False) -> None:
     """
     Updates the parameter documentation in the target file or in all *.param,*.parm files of the target directory.
 
     This function iterates over all the ArduPilot parameter files in the target directory or file.
     For each file, it DELETES all comments that start at the beginning of a line, optionally sorts the
     parameter names and checks if the parameter name is in the dictionary of parameter documentation.
     If it is, it prefixes the line with a comment derived from the dictionary element.
@@ -544,44 +550,46 @@
 
     if param_default_dict is None:
         param_default_dict = {}
 
     # Iterate over all the target ArduPilot parameter files
     for param_file in param_files:
 
-        if os_path.basename(param_file).endswith("22_inflight_magnetometer_fit_setup.param") and "MAGH_ALT_DELTA" not in doc:
+        if os_path.basename(param_file).endswith("24_inflight_magnetometer_fit_setup.param") and "MAGH_ALT_DELTA" not in doc:
             continue
 
         # Read the entire file contents
         with open(param_file, "r", encoding="utf-8") as file:
             lines = file.readlines()
 
-        update_parameter_documentation_file(doc, sort_type, param_default_dict, param_file, lines)
+        update_parameter_documentation_file(doc, sort_type, param_default_dict, param_file, lines,
+                                            delete_documentation_annotations)
 
-def update_parameter_documentation_file(doc, sort_type, param_default_dict, param_file, lines):  # pylint: disable=too-many-locals
+def update_parameter_documentation_file(doc, sort_type, param_default_dict, param_file, lines,  # pylint: disable=too-many-locals, too-many-arguments
+                                        delete_documentation_annotations: bool):
     new_lines = []
-    if os_path.basename(param_file).endswith("15_pid_adjustment.param"):
-        new_lines.extend(lines[0:7])  # copy the first 8 lines verbatim
+    if os_path.basename(param_file).endswith("16_pid_adjustment.param"):
+        new_lines.extend(lines[0:5])  # copy the first 6 lines verbatim
 
     total_params = 0
     documented_params = 0
     undocumented_params = []
     is_first_param_in_file = True
     if sort_type == "missionplanner":
         lines.sort(key=missionplanner_sort)
     if sort_type == "mavproxy":
         lines.sort(key=extract_parameter_name)
     for n, line in enumerate(lines, start=1):
         line = line.strip()
         if not line.startswith("#") and line:
             param_name = extract_parameter_name_and_validate(line, param_file, n)
 
-            if param_name in doc:
-                    # If the parameter name is in the dictionary,
-                    #  prefix the line with a comment derived from the dictionary element
+            if param_name in doc and not delete_documentation_annotations:
+                # If the parameter name is in the dictionary,
+                #  prefix the line with a comment derived from the dictionary element
                 data = doc[param_name]
                 prefix_parts = [
                         f"{data['humanName']}",
                     ]
                 prefix_parts += data["documentation"]
                 for key, value in data["fields"].items():
                     prefix_parts.append(f"{key}: {value}")
@@ -591,30 +599,30 @@
                     default_value = format(param_default_dict[param_name].value, '.6f').rstrip('0').rstrip('.')
                     doc_text += f"\n# Default: {default_value}"
                 if not is_first_param_in_file:
                     new_lines.append("\n")
                 new_lines.append(f"# {doc_text}\n{line}\n")
                 documented_params += 1
             else:
-                    # If the parameter name is in not the dictionary, copy the parameter line 1-to-1
+                # If the parameter name is in not the dictionary, copy the parameter line 1-to-1
                 new_lines.append(f"{line}\n")
                 undocumented_params.append(param_name)
             total_params += 1
             is_first_param_in_file = False
 
     if total_params == documented_params:
         logging.info("Read file %s with %d parameters, all got documented",
                          param_file, total_params)
     else:
         logging.warning("Read file %s with %d parameters, but only %s of which got documented",
                             param_file, total_params, documented_params)
         logging.warning("No documentation found for: %s", ", ".join(undocumented_params))
 
-        # Write the new file contents to the file
-    with open(param_file, "w", encoding="utf-8") as file:
+    # Write the new file contents to the file
+    with open(param_file, "w", encoding="utf-8", newline='\n') as file:  # Ensure newline character is LF, even on windows
         file.writelines(new_lines)
 
 
 def print_read_only_params(doc):
     """
     Print the names of read-only parameters.
 
@@ -629,23 +637,25 @@
 
 def main():
     args = arg_parser()
     try:
         xml_dir = args.target if os_path.isdir(args.target) else os_path.dirname(os_path.realpath(args.target))
         xml_root, param_default_dict = get_xml_data(BASE_URL + args.vehicle_type + "/", xml_dir, PARAM_DEFINITION_XML_FILE)
         doc_dict = create_doc_dict(xml_root, args.vehicle_type, args.max_line_length)
-        update_parameter_documentation(doc_dict, args.target, args.sort, param_default_dict)
+        update_parameter_documentation(doc_dict, args.target, args.sort, param_default_dict,
+                                       args.delete_documentation_annotations)
         if args.verbose:
             print_read_only_params(doc_dict)
         if os_path.isfile(os_path.join(os_path.dirname(args.target), LUA_PARAM_DEFINITION_XML_FILE)):
             xml_root, param_default_dict = get_xml_data(BASE_URL + args.vehicle_type + "/",
                                                         xml_dir, LUA_PARAM_DEFINITION_XML_FILE)
             doc_dict = create_doc_dict(xml_root, args.vehicle_type, args.max_line_length)
             update_parameter_documentation(doc_dict, os_path.join(os_path.dirname(args.target),
-                                                                  "22_inflight_magnetometer_fit_setup.param"))
+                                                                  "24_inflight_magnetometer_fit_setup.param"),
+                                           args.sort, param_default_dict, args.delete_documentation_annotations)
     except Exception as exp:  # pylint: disable=W0718
         logging.fatal(exp)
         exit(1)  # pylint: disable=R1722
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
     # Connect to the flight controller and read the parameters
     flight_controller = FlightController(args.reboot_time)
 
     error_str = flight_controller.connect(args.device)
     if error_str:
-        logging_error(error_str)
+        if "No serial ports found" not in error_str:
+            logging_error(error_str)
         conn_sel_window = ConnectionSelectionWindow(flight_controller, error_str)
         conn_sel_window.root.mainloop()
 
     vehicle_type = args.vehicle_type
     if vehicle_type == "":  # not explicitly set, to try to guess it
         if flight_controller.vehicle_type is not None:
             vehicle_type = flight_controller.vehicle_type
@@ -80,21 +81,20 @@
     else:
         logging_info("Vehicle type explicitly set to %s.", vehicle_type)
 
     if vehicle_type == "": # did not guess it, default to ArduCopter
         vehicle_type = "ArduCopter"
         logging_warning("Could not detect vehicle type. Defaulting to ArduCopter.")
 
-    local_filesystem = LocalFilesystem(args.vehicle_dir, vehicle_type)
+    local_filesystem = LocalFilesystem(args.vehicle_dir, vehicle_type, args.allow_editing_template_files)
 
     # Get the list of intermediate parameter files files that will be processed sequentially
     files = list(local_filesystem.file_parameters.keys())
 
     if not files:
-        logging_error("No intermediate parameter files found in %s.", args.vehicle_dir)
         vehicle_dir_window = VehicleDirectorySelectionWindow(local_filesystem)
         vehicle_dir_window.root.mainloop()
 
     start_file = local_filesystem.get_start_file(args.n)
 
     if not args.skip_component_editor:
         component_editor_window = ComponentEditorWindow(VERSION, local_filesystem)
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 SPDX-License-Identifier:    GPL-3
 '''
 
 from os import path as os_path
 from os import getcwd as os_getcwd
 from os import listdir as os_listdir
 from os import makedirs as os_makedirs
+from os import rename as os_rename
 from os import sep as os_sep
 
 from shutil import copy2 as shutil_copy2
 from shutil import copytree as shutil_copytree
 
 from re import compile as re_compile
 from re import match as re_match
 from re import escape as re_escape
 from re import sub as re_sub
 
 # from sys import exit as sys_exit
-# from logging import debug as logging_debug
+from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
 
 from json import load as json_load
 from json import dump as json_dump
 
@@ -87,40 +88,56 @@
     Attributes:
         vehicle_dir (str): The directory path where the vehicle configuration files are stored.
         vehicle_type (str): The type of the vehicle (e.g., "ArduCopter", "Rover").
         file_parameters (dict): A dictionary of parameters read from intermediate parameter files.
         param_default_dict (dict): A dictionary of default parameter values.
         doc_dict (dict): A dictionary containing documentation for each parameter.
     """
-    def __init__(self, vehicle_dir: str, vehicle_type: str):
+    def __init__(self, vehicle_dir: str, vehicle_type: str, allow_editing_template_files: bool = False):
         self.file_parameters = None
         VehicleComponents.__init__(self)
         ConfigurationSteps.__init__(self, vehicle_dir, vehicle_type)
+        self.allow_editing_template_files = allow_editing_template_files
         if vehicle_dir is not None:
             self.re_init(vehicle_dir, vehicle_type)
 
     def re_init(self, vehicle_dir: str, vehicle_type: str):
+        ConfigurationSteps.re_init(self, vehicle_dir, vehicle_type)
         self.vehicle_dir = vehicle_dir
         self.vehicle_type = vehicle_type
         self.param_default_dict = {}
         self.doc_dict = {}
 
+        # Rename parameter files if some new files got added to the vehicle directory
+        self.rename_parameter_files()
+
         # Read intermediate parameters from files
         self.file_parameters = self.read_params_from_files()
         if not self.file_parameters:
             return # No files intermediate parameters files found, no need to continue, the rest needs them
 
         # Read ArduPilot parameter documentation
         xml_dir = vehicle_dir if os_path.isdir(vehicle_dir) else os_path.dirname(os_path.realpath(vehicle_dir))
         xml_root, self.param_default_dict = get_xml_data(BASE_URL + vehicle_type + "/", xml_dir, PARAM_DEFINITION_XML_FILE)
         self.doc_dict = create_doc_dict(xml_root, vehicle_type, TOOLTIP_MAX_LENGTH)
 
         self.__extend_and_reformat_parameter_documentation_metadata()
         self.load_vehicle_components_json_data(vehicle_dir)
 
+    def rename_parameter_files(self):
+        # Rename parameter files if some new files got added to the vehicle directory
+        if self.vehicle_dir is not None and self.configuration_steps is not None:
+            for new_filename in self.configuration_steps:
+                if 'old_filenames' in self.configuration_steps[new_filename]:
+                    for old_filename in self.configuration_steps[new_filename]['old_filenames']:
+                        if self.intermediate_parameter_file_exists(old_filename) and old_filename != new_filename:
+                            new_filename_path = os_path.join(self.vehicle_dir, new_filename)
+                            old_filename_path = os_path.join(self.vehicle_dir, old_filename)
+                            os_rename(old_filename_path, new_filename_path)
+                            logging_info("Renamed %s to %s", old_filename, new_filename)
 
     def __extend_and_reformat_parameter_documentation_metadata(self):
         for param_name, param_info in self.doc_dict.items():
             if 'fields' in param_info:
                 if 'Units' in param_info['fields']:
                     param_info['unit'] = param_info['fields']['Units'].split('(')[0].strip()
                     param_info['unit_tooltip'] = param_info['fields']['Units'].split('(')[1].strip(')')
@@ -562,14 +579,16 @@
         except Exception as e:  # pylint: disable=broad-except
             logging_error("Error writing last uploaded filename: %s", e)
 
     def __read_last_uploaded_filename(self) -> str:
         try:
             with open(os_path.join(self.vehicle_dir, 'last_uploaded_filename.txt'), 'r', encoding='utf-8') as file:
                 return file.read().strip()
+        except FileNotFoundError as e:
+            logging_debug("last_uploaded_filename.txt not found: %s", e)
         except Exception as e:  # pylint: disable=broad-except
             logging_error("Error reading last uploaded filename: %s", e)
         return ""
 
     def get_start_file(self, explicit_index: int):
         # Get the list of intermediate parameter files files that will be processed sequentially
         files = list(self.file_parameters.keys())
@@ -626,8 +645,12 @@
                             'Defaults to the current working directory')
         parser.add_argument('--n',
                             type=int,
                             default=-1,
                             help='Start directly on the nth intermediate parameter file (skips previous files). '
                             'Default is to start on the file next to the last that you wrote to the flight controller.'
                             'If the file does not exist, it will start on the first file.')
+        parser.add_argument('--allow-editing-template-files',
+                            action='store_true',
+                            help='Allow opening and editing template files directly. '
+                            'Only for software developers that know what they are doing.')
         return parser
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_configuration_steps.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_configuration_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     This class provides methods for reading and validating configuration steps, including forced and derived parameters.
     It is designed to simplify the interaction with configuration steps for managing ArduPilot configuration files.
 
     Attributes:
         configuration_steps_filename (str): The name of the file containing documentation for the configuration files.
         configuration_steps (dict): A dictionary containing the configuration steps.
     """
-    def __init__(self, vehicle_dir: str, vehicle_type: str):
+    def __init__(self, _vehicle_dir: str, vehicle_type: str):
         self.configuration_steps_filename = vehicle_type + "_configuration_steps.json"
         self.configuration_steps = {}
         self.forced_parameters = {}
         self.derived_parameters = {}
 
+    def re_init(self, vehicle_dir: str, vehicle_type: str):
+        self.configuration_steps_filename = vehicle_type + "_configuration_steps.json"
         # Define a list of directories to search for the configuration_steps_filename file
         search_directories = [vehicle_dir, os_path.dirname(os_path.abspath(__file__))]
         file_found = False
         for i, directory in enumerate(search_directories):
             try:
                 with open(os_path.join(directory, self.configuration_steps_filename), 'r', encoding='utf-8') as file:
                     self.configuration_steps = json_load(file)
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/backend_filesystem_vehicle_components.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_vehicle_components.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/backend_flightcontroller.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/backend_flightcontroller.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/backend_mavftp.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/backend_mavftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/battery_cell_voltages.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/battery_cell_voltages.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/common_arguments.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/common_arguments.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_base.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_base.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,25 @@
         ComponentEditorWindowBase.__init__(self, version, local_filesystem)
         style = ttk.Style()
         style.configure("comb_input_invalid.TCombobox", fieldbackground="red")
         style.configure("comb_input_valid.TCombobox", fieldbackground="white")
         style.configure("entry_input_invalid.TEntry", fieldbackground="red")
         style.configure("entry_input_valid.TEntry", fieldbackground="white")
 
+    def update_json_data(self):
+        super().update_json_data()
+        if 'Components' not in self.data:
+            self.data['Components'] = {}
+        if 'Battery' not in self.data['Components']:
+            self.data['Components']['Battery'] = {}
+        if 'Specifications' not in self.data['Components']['Battery']:
+            self.data['Components']['Battery']['Specifications'] = {}
+        if 'Chemistry' not in self.data['Components']['Battery']['Specifications']:
+            self.data['Components']['Battery']['Specifications']['Chemistry'] = "Lipo"
+
     def set_vehicle_type_and_version(self, vehicle_type: str, version: str):
         self.data['Components']['Flight Controller']['Firmware']['Type'] = vehicle_type
         entry = self.entry_widgets[('Flight Controller', 'Firmware', 'Type')]
         entry.delete(0, tk.END)
         entry.insert(0, vehicle_type)
         entry.config(state="disabled")
         if version:
@@ -350,10 +361,10 @@
 
 
 if __name__ == "__main__":
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
-    filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type)
+    filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type, args.allow_editing_template_files)
     app = ComponentEditorWindow(VERSION, filesystem)
     app.root.mainloop()
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_component_editor_base.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,20 +86,26 @@
         else:
             image_label = tk.Label(main_frame, text="No vehicle.jpg image file found on the vehicle directory.")
             image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
 
         self.scroll_frame = ScrollFrame(self.root)
         self.scroll_frame.pack(side="top", fill="both", expand=True)
 
+        self.update_json_data()
+
         self.__populate_frames()
 
         self.save_button = ttk.Button(self.root, text="Save data and start configuration", command=self.save_data)
         show_tooltip(self.save_button, "Save component data and start parameter value configuration and tuning.")
         self.save_button.pack(pady=7)
 
+    def update_json_data(self):  # should be overwritten in child classes
+        if 'Format version' not in self.data:
+            self.data['Format version'] = 1
+
     def __populate_frames(self):
         """
         Populates the ScrollFrame with widgets based on the JSON data.
         """
         if "Components" in self.data:
             for key, value in self.data["Components"].items():
                 self.__add_widget(self.scroll_frame.view_port, key, value, [])
@@ -183,10 +189,10 @@
 
 
 if __name__ == "__main__":
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
-    filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type)
+    filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type, args.allow_editing_template_files)
     app = ComponentEditorWindowBase(VERSION, filesystem)
     app.root.mainloop()
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_connection_selection.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_connection_selection.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_directory_selection.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_directory_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                             if destroy_parent_on_open else '')
         self.local_filesystem = local_filesystem
         self.destroy_parent_on_open = destroy_parent_on_open
 
     def on_select_directory(self):
         # Call the base class method to open the directory selection dialog
         if super().on_select_directory():
-            if "vehicle_templates" in self.directory:
+            if "vehicle_templates" in self.directory and not self.local_filesystem.allow_editing_template_files:
                 show_error_message("Invalid Vehicle Directory Selected",
                                    "Please do not edit the files provided 'vehicle_templates' directory\n"
                                    "as those are used as a template for new vehicles")
                 return
             self.local_filesystem.vehicle_dir = self.directory
             self.local_filesystem.re_init(self.directory, self.local_filesystem.vehicle_type)
             files = list(self.local_filesystem.file_parameters.keys())
@@ -346,15 +346,15 @@
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
     logging_warning("This main is for testing and development only, usually the VehicleDirectorySelectionWindow is"
                     " called from another script")
 
-    local_filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type)
+    local_filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type, args.allow_editing_template_files)
 
     # Get the list of intermediate parameter files files that will be processed sequentially
     files = list(local_filesystem.file_parameters.keys())
 
     if not files:
         logging_error("No intermediate parameter files found in %s.", args.vehicle_dir)
         window = VehicleDirectorySelectionWindow(local_filesystem)
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/get_release_stats.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/get_release_stats.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/param_ftp.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/param_ftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description="""
 Updates PID adjustment parameters values based on the given ADJUSTMENT_FACTOR argument.
 
 It loads three sets of parameters from files in the DIRECTORY directory:
     00_default.param - the (complete) default parameters,
     optimized_param_file - the (complete) optimized parameters, and
-    14_pid_adjustment.param - the (intermediate) PID adjustment parameters.
+    16_pid_adjustment.param - the (intermediate) PID adjustment parameters.
 It calculates the PID adjustment parameter values based on the ADJUSTMENT_FACTOR argument.
-It updates the intermediate parameter file 14_pid_adjustment.param with parameter comments
+It updates the intermediate parameter file 16_pid_adjustment.param with parameter comments
 explaining how their new value relates to the default parameter value.
 """)
     parser.add_argument("-d", "--directory",
                         required=True,
                         help="The directory where the parameter files are located.",
                         )
     parser.add_argument("-a", "--adjustment_factor",
@@ -151,15 +151,15 @@
     Args:
         directory (str): The directory where the parameter files are located.
         optimized_param_file (str): The name of the optimized parameter file.
         adjustment_factor (float): The adjustment factor to apply to the optimized parameters.
     """
     default_param_file_path = os.path.join(directory, "00_default.param")
     optimized_param_file_path = os.path.join(directory, optimized_param_file)
-    pid_adjustment_file_path = os.path.join(directory, "14_pid_adjustment.param")
+    pid_adjustment_file_path = os.path.join(directory, "16_pid_adjustment.param")
 
     # Load the default parameter file into a dictionary (comment source)
     default_params_dict, _ = Par.load_param_file_into_dict(default_param_file_path)
 
     # Load the optimized parameter file into a dictionary (source)
     optimized_params_dict, _ = Par.load_param_file_into_dict(optimized_param_file_path)
 
@@ -199,12 +199,12 @@
     args = parse_arguments()
     # calculate the parameter values and their comments
     pid_adjustment_params_dict, pid_adjustment_file_path, content_header = update_pid_adjustment_params(
         args.directory, args.optimized_param_file, args.adjustment_factor)
     # export the updated PID adjust parameters to a file, preserving the first eight header lines
     Par.export_to_param(pid_adjustment_params_dict, pid_adjustment_file_path, content_header)
     # annotate each parameter with up-to date documentation
-    subprocess.run(['./annotate_params.py', os.path.join(args.directory, "14_pid_adjustment.param")], check=True)
+    subprocess.run(['./annotate_params.py', os.path.join(args.directory, "16_pid_adjustment.param")], check=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator/tempcal_imu.py` & `methodicconfigurator-0.6.4/MethodicConfigurator/tempcal_imu.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.6.1
+Version: 0.6.4
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
@@ -25,14 +25,15 @@
 License-File: LICENSE.md
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: pymavlink
 Requires-Dist: pyserial
 Requires-Dist: pillow
+Requires-Dist: setuptools
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mock; extra == "dev"
```

### Comparing `methodicconfigurator-0.6.1/MethodicConfigurator.egg-info/SOURCES.txt` & `methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,258 +39,264 @@
 vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
 vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
 vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
 vehicle_templates/ArduCopter/X11_plus/07_esc.param
 vehicle_templates/ArduCopter/X11_plus/08_batt1.param
 vehicle_templates/ArduCopter/X11_plus/10_gnss.param
-vehicle_templates/ArduCopter/X11_plus/11_mp_setup_mandatory_hardware.param
-vehicle_templates/ArduCopter/X11_plus/12_general_configuration.param
-vehicle_templates/ArduCopter/X11_plus/13_logging.param
-vehicle_templates/ArduCopter/X11_plus/14_motor.param
-vehicle_templates/ArduCopter/X11_plus/15_pid_adjustment.param
-vehicle_templates/ArduCopter/X11_plus/16_remote_id.param
-vehicle_templates/ArduCopter/X11_plus/17_notch_filter_setup.param
-vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param
-vehicle_templates/ArduCopter/X11_plus/19_throttle_controller.param
-vehicle_templates/ArduCopter/X11_plus/20_quick_tune_setup.param
-vehicle_templates/ArduCopter/X11_plus/21_quick_tune_results.param
-vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param
+vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param
+vehicle_templates/ArduCopter/X11_plus/14_logging.param
+vehicle_templates/ArduCopter/X11_plus/15_motor.param
+vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param
+vehicle_templates/ArduCopter/X11_plus/17_remote_id.param
+vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param
+vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param
+vehicle_templates/ArduCopter/X11_plus/20_throttle_controller.param
+vehicle_templates/ArduCopter/X11_plus/21_ekf_config.param
 vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
-vehicle_templates/ArduCopter/X11_plus/23_inflight_magnetometer_fit_results.param
-vehicle_templates/ArduCopter/X11_plus/24_quick_tune_setup.param
-vehicle_templates/ArduCopter/X11_plus/25_quick_tune_results.param
-vehicle_templates/ArduCopter/X11_plus/26_evaluate_the_aircraft_tune_ff_disable.param
-vehicle_templates/ArduCopter/X11_plus/27_evaluate_the_aircraft_tune_ff_enable.param
-vehicle_templates/ArduCopter/X11_plus/28_autotune_roll_setup.param
-vehicle_templates/ArduCopter/X11_plus/29_autotune_roll_results.param
-vehicle_templates/ArduCopter/X11_plus/30_autotune_pitch_setup.param
-vehicle_templates/ArduCopter/X11_plus/31_autotune_pitch_results.param
-vehicle_templates/ArduCopter/X11_plus/32_autotune_yaw_setup.param
-vehicle_templates/ArduCopter/X11_plus/33_autotune_yaw_results.param
-vehicle_templates/ArduCopter/X11_plus/34_autotune_yawd_setup.param
-vehicle_templates/ArduCopter/X11_plus/35_autotune_yawd_results.param
-vehicle_templates/ArduCopter/X11_plus/36_autotune_roll_pitch_retune_setup.param
-vehicle_templates/ArduCopter/X11_plus/37_autotune_roll_pitch_retune_results.param
-vehicle_templates/ArduCopter/X11_plus/38_windspeed_estimation.param
-vehicle_templates/ArduCopter/X11_plus/39_barometer_compensation.param
-vehicle_templates/ArduCopter/X11_plus/40_system_id_roll.param
-vehicle_templates/ArduCopter/X11_plus/41_system_id_pitch.param
-vehicle_templates/ArduCopter/X11_plus/42_system_id_yaw.param
-vehicle_templates/ArduCopter/X11_plus/43_system_id_thrust.param
-vehicle_templates/ArduCopter/X11_plus/44_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/X11_plus/45_everyday_use.param
-vehicle_templates/ArduCopter/X11_plus/46_position_controller.param
-vehicle_templates/ArduCopter/X11_plus/47_precision_land.param
-vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param
+vehicle_templates/ArduCopter/X11_plus/22_quick_tune_setup.param
+vehicle_templates/ArduCopter/X11_plus/23_quick_tune_results.param
+vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param
+vehicle_templates/ArduCopter/X11_plus/26_quick_tune_setup.param
+vehicle_templates/ArduCopter/X11_plus/27_quick_tune_results.param
+vehicle_templates/ArduCopter/X11_plus/28_evaluate_the_aircraft_tune_ff_disable.param
+vehicle_templates/ArduCopter/X11_plus/29_evaluate_the_aircraft_tune_ff_enable.param
+vehicle_templates/ArduCopter/X11_plus/30_autotune_roll_setup.param
+vehicle_templates/ArduCopter/X11_plus/31_autotune_roll_results.param
+vehicle_templates/ArduCopter/X11_plus/32_autotune_pitch_setup.param
+vehicle_templates/ArduCopter/X11_plus/33_autotune_pitch_results.param
+vehicle_templates/ArduCopter/X11_plus/34_autotune_yaw_setup.param
+vehicle_templates/ArduCopter/X11_plus/35_autotune_yaw_results.param
+vehicle_templates/ArduCopter/X11_plus/36_autotune_yawd_setup.param
+vehicle_templates/ArduCopter/X11_plus/37_autotune_yawd_results.param
+vehicle_templates/ArduCopter/X11_plus/38_autotune_roll_pitch_retune_setup.param
+vehicle_templates/ArduCopter/X11_plus/39_autotune_roll_pitch_retune_results.param
+vehicle_templates/ArduCopter/X11_plus/40_windspeed_estimation.param
+vehicle_templates/ArduCopter/X11_plus/41_barometer_compensation.param
+vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param
+vehicle_templates/ArduCopter/X11_plus/43_system_id_pitch.param
+vehicle_templates/ArduCopter/X11_plus/44_system_id_yaw.param
+vehicle_templates/ArduCopter/X11_plus/45_system_id_thrust.param
+vehicle_templates/ArduCopter/X11_plus/46_analytical_pid_optimization.param
+vehicle_templates/ArduCopter/X11_plus/47_everyday_use.param
+vehicle_templates/ArduCopter/X11_plus/48_position_controller.param
+vehicle_templates/ArduCopter/X11_plus/49_precision_land.param
+vehicle_templates/ArduCopter/X11_plus/50_guided_operation.param
 vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
 vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
 vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
+vehicle_templates/ArduCopter/X11_plus/vehicle.jpg
 vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_logging.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_motor.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_remote_id.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_notch_filter_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_throttle_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_ekf_config.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_inflight_magnetometer_fit_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_evaluate_the_aircraft_tune_ff_disable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_evaluate_the_aircraft_tune_ff_enable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_roll_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_roll_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_pitch_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_pitch_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yaw_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yaw_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_yawd_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_yawd_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_autotune_roll_pitch_retune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_autotune_roll_pitch_retune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_windspeed_estimation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_barometer_compensation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_pitch.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_system_id_yaw.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_system_id_thrust.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_analytical_pid_optimization.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_everyday_use.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_logging.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_motor.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_remote_id.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_notch_filter_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_throttle_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_ekf_config.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_inflight_magnetometer_fit_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_evaluate_the_aircraft_tune_ff_disable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_evaluate_the_aircraft_tune_ff_enable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_roll_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_roll_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_pitch_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_pitch_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yaw_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yaw_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_yawd_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_yawd_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_autotune_roll_pitch_retune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_autotune_roll_pitch_retune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_windspeed_estimation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_barometer_compensation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_pitch.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_system_id_yaw.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_system_id_thrust.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_analytical_pid_optimization.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_everyday_use.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_mp_setup_mandatory_hardware.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_general_configuration.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_logging.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_motor.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_pid_adjustment.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_remote_id.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_notch_filter_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_throttle_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_ekf_config.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_inflight_magnetometer_fit_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_evaluate_the_aircraft_tune_ff_disable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_evaluate_the_aircraft_tune_ff_enable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_roll_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_roll_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_pitch_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_pitch_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yaw_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yaw_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_yawd_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_yawd_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_autotune_roll_pitch_retune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_autotune_roll_pitch_retune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_windspeed_estimation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_barometer_compensation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_roll.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_pitch.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_system_id_yaw.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_system_id_thrust.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_analytical_pid_optimization.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_everyday_use.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/49_precision_land.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/50_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_mp_setup_mandatory_hardware.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_general_configuration.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_logging.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_motor.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_remote_id.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_notch_filter_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_throttle_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_ekf_config.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_inflight_magnetometer_fit_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_evaluate_the_aircraft_tune_ff_disable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_evaluate_the_aircraft_tune_ff_enable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_roll_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_roll_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_pitch_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_pitch_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yaw_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yaw_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_yawd_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_yawd_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_autotune_roll_pitch_retune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_autotune_roll_pitch_retune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_windspeed_estimation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_barometer_compensation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_pitch.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_system_id_yaw.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_system_id_thrust.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_analytical_pid_optimization.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_everyday_use.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/49_precision_land.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.6.1/PKG-INFO` & `methodicconfigurator-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.6.1
+Version: 0.6.4
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
@@ -25,14 +25,15 @@
 License-File: LICENSE.md
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: pymavlink
 Requires-Dist: pyserial
 Requires-Dist: pillow
+Requires-Dist: setuptools
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mock; extra == "dev"
```

### Comparing `methodicconfigurator-0.6.1/README.md` & `methodicconfigurator-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/setup.py` & `methodicconfigurator-0.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     install_requires=[
         'matplotlib',
         'numpy',
         'platformdirs',
         'pymavlink',
         'pyserial',
         'pillow',
+        'setuptools',
         'requests',
     ],
     extras_require={
         'dev': dev_requirements,
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/00_default.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-INS_LOG_BAT_MASK,7  # Do IMU temperature compensation on all three CubeOrange IMUs
-INS_TCAL1_ENABLE,2  # Activates the temperature calibration for IMU 1 at the next start
-INS_TCAL1_TMAX,70  # CubeOrange has an heater that heats up the board to almost 70 deg
-INS_TCAL2_ENABLE,2  # Activates the temperature calibration for IMU 2 at the next start
-INS_TCAL2_TMAX,70  # CubeOrange has an heater that heats up the board to almost 70 deg
-
-LOG_BITMASK,524416  # Only for IMU and Raw-IMU
-LOG_DISARMED,1  # Gather data for the offline IMU temperature compensation while the FC is disarmed
+INS_LOG_BAT_MASK,7  # Do IMU temperature compensation on all three CubeOrange IMUs
+INS_TCAL1_ENABLE,2  # Activates the temperature calibration for IMU 1 at the next start
+INS_TCAL1_TMAX,70  # CubeOrange has an heater that heats up the board to almost 70 deg
+INS_TCAL2_ENABLE,2  # Activates the temperature calibration for IMU 2 at the next start
+INS_TCAL2_TMAX,70  # CubeOrange has an heater that heats up the board to almost 70 deg
+LOG_BITMASK,524416  # Only for IMU and Raw-IMU
+LOG_DISARMED,1  # Gather data for the offline IMU temperature compensation while the FC is disarmed
```

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-INS_TCAL1_ENABLE 1
-INS_TCAL1_TMIN -27.7
-INS_TCAL1_TMAX 65.2
-INS_TCAL1_ACC1_X 1247.871253135
-INS_TCAL1_ACC1_Y -892.049074204
-INS_TCAL1_ACC1_Z 1207.190783926
-INS_TCAL1_ACC2_X 9.275325353
-INS_TCAL1_ACC2_Y 7.953769516
-INS_TCAL1_ACC2_Z -5.040771430
-INS_TCAL1_ACC3_X 0.179680847
-INS_TCAL1_ACC3_Y 0.077448526
-INS_TCAL1_ACC3_Z 0.352090854
-INS_TCAL1_GYR1_X -427.997725367
-INS_TCAL1_GYR1_Y -236.667872281
-INS_TCAL1_GYR1_Z 62.792551728
-INS_TCAL1_GYR2_X -4.177657407
-INS_TCAL1_GYR2_Y 2.301448994
-INS_TCAL1_GYR2_Z 2.299436373
-INS_TCAL1_GYR3_X -0.048496838
-INS_TCAL1_GYR3_Y -0.097145480
-INS_TCAL1_GYR3_Z 0.009887841
-INS_TCAL2_ENABLE 1
-INS_TCAL2_TMIN -30.1
-INS_TCAL2_TMAX 63.7
-INS_TCAL2_ACC1_X 4815.212183474
-INS_TCAL2_ACC1_Y -6441.654763889
-INS_TCAL2_ACC1_Z -2473.756443939
-INS_TCAL2_ACC2_X -1.253623783
-INS_TCAL2_ACC2_Y 29.489814772
-INS_TCAL2_ACC2_Z 26.796802173
-INS_TCAL2_ACC3_X -1.031974608
-INS_TCAL2_ACC3_Y 2.179268625
-INS_TCAL2_ACC3_Z 0.696695388
-INS_TCAL2_GYR1_X -184.261848642
-INS_TCAL2_GYR1_Y -127.112597066
-INS_TCAL2_GYR1_Z -61.481194933
-INS_TCAL2_GYR2_X -1.610634809
-INS_TCAL2_GYR2_Y 3.901946757
-INS_TCAL2_GYR2_Z -0.582771477
-INS_TCAL2_GYR3_X -0.020563080
-INS_TCAL2_GYR3_Y 0.040040303
-INS_TCAL2_GYR3_Z -0.015435894
-INS_TCAL3_ENABLE 1
-INS_TCAL3_TMIN -27.7
-INS_TCAL3_TMAX 57.3
-INS_TCAL3_ACC1_X -1465.066631174
-INS_TCAL3_ACC1_Y 458.876383573
-INS_TCAL3_ACC1_Z 2544.281946448
-INS_TCAL3_ACC2_X 3.881862162
-INS_TCAL3_ACC2_Y 6.304407443
-INS_TCAL3_ACC2_Z 16.704324561
-INS_TCAL3_ACC3_X 1.217048892
-INS_TCAL3_ACC3_Y -0.670616159
-INS_TCAL3_ACC3_Z -1.336884747
-INS_TCAL3_GYR1_X -311.394614775
-INS_TCAL3_GYR1_Y 44.271917183
-INS_TCAL3_GYR1_Z 46.225659749
-INS_TCAL3_GYR2_X -0.843643268
-INS_TCAL3_GYR2_Y 1.902222809
-INS_TCAL3_GYR2_Z -0.561674562
-INS_TCAL3_GYR3_X 0.004106825
-INS_TCAL3_GYR3_Y -0.061593897
-INS_TCAL3_GYR3_Z 0.019881423
+INS_TCAL1_ENABLE 1
+INS_TCAL1_TMIN -27.7
+INS_TCAL1_TMAX 65.2
+INS_TCAL1_ACC1_X 1247.871253135
+INS_TCAL1_ACC1_Y -892.049074204
+INS_TCAL1_ACC1_Z 1207.190783926
+INS_TCAL1_ACC2_X 9.275325353
+INS_TCAL1_ACC2_Y 7.953769516
+INS_TCAL1_ACC2_Z -5.040771430
+INS_TCAL1_ACC3_X 0.179680847
+INS_TCAL1_ACC3_Y 0.077448526
+INS_TCAL1_ACC3_Z 0.352090854
+INS_TCAL1_GYR1_X -427.997725367
+INS_TCAL1_GYR1_Y -236.667872281
+INS_TCAL1_GYR1_Z 62.792551728
+INS_TCAL1_GYR2_X -4.177657407
+INS_TCAL1_GYR2_Y 2.301448994
+INS_TCAL1_GYR2_Z 2.299436373
+INS_TCAL1_GYR3_X -0.048496838
+INS_TCAL1_GYR3_Y -0.097145480
+INS_TCAL1_GYR3_Z 0.009887841
+INS_TCAL2_ENABLE 1
+INS_TCAL2_TMIN -30.1
+INS_TCAL2_TMAX 63.7
+INS_TCAL2_ACC1_X 4815.212183474
+INS_TCAL2_ACC1_Y -6441.654763889
+INS_TCAL2_ACC1_Z -2473.756443939
+INS_TCAL2_ACC2_X -1.253623783
+INS_TCAL2_ACC2_Y 29.489814772
+INS_TCAL2_ACC2_Z 26.796802173
+INS_TCAL2_ACC3_X -1.031974608
+INS_TCAL2_ACC3_Y 2.179268625
+INS_TCAL2_ACC3_Z 0.696695388
+INS_TCAL2_GYR1_X -184.261848642
+INS_TCAL2_GYR1_Y -127.112597066
+INS_TCAL2_GYR1_Z -61.481194933
+INS_TCAL2_GYR2_X -1.610634809
+INS_TCAL2_GYR2_Y 3.901946757
+INS_TCAL2_GYR2_Z -0.582771477
+INS_TCAL2_GYR3_X -0.020563080
+INS_TCAL2_GYR3_Y 0.040040303
+INS_TCAL2_GYR3_Z -0.015435894
+INS_TCAL3_ENABLE 1
+INS_TCAL3_TMIN -27.7
+INS_TCAL3_TMAX 57.3
+INS_TCAL3_ACC1_X -1465.066631174
+INS_TCAL3_ACC1_Y 458.876383573
+INS_TCAL3_ACC1_Z 2544.281946448
+INS_TCAL3_ACC2_X 3.881862162
+INS_TCAL3_ACC2_Y 6.304407443
+INS_TCAL3_ACC2_Z 16.704324561
+INS_TCAL3_ACC3_X 1.217048892
+INS_TCAL3_ACC3_Y -0.670616159
+INS_TCAL3_ACC3_Z -1.336884747
+INS_TCAL3_GYR1_X -311.394614775
+INS_TCAL3_GYR1_Y 44.271917183
+INS_TCAL3_GYR1_Z 46.225659749
+INS_TCAL3_GYR2_X -0.843643268
+INS_TCAL3_GYR2_Y 1.902222809
+INS_TCAL3_GYR2_Z -0.561674562
+INS_TCAL3_GYR3_X 0.004106825
+INS_TCAL3_GYR3_Y -0.061593897
+INS_TCAL3_GYR3_Z 0.019881423
```

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_results.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-INS_HNTCH_ATT,40  # just enough to filter the noise created by the motors/propellers
-INS_HNTCH_BW,12  # just enough to filter the noise created by the motors/propellers
-INS_HNTCH_FM_RAT,0.5  # Allowed undercutting of the base frequency of the first notch filter
-INS_HNTCH_FREQ,27  # the minimum frequency that the motors are expected to operate at
-INS_HNTCH_HMNCS,3  # the motors produce secondary harmonics on this vehicle
-INS_HNTCH_OPTS,1
-INS_HNTCH_REF,0.13  # Calculate and change this according to the wiki
+INS_HNTCH_ATT,40  # just enough to filter the noise created by the motors/propellers
+INS_HNTCH_BW,12  # just enough to filter the noise created by the motors/propellers
+INS_HNTCH_FM_RAT,0.5  # Allowed undercutting of the base frequency of the first notch filter
+INS_HNTCH_FREQ,27  # the minimum frequency that the motors are expected to operate at
+INS_HNTCH_HMNCS,3  # the motors produce secondary harmonics on this vehicle
+INS_HNTCH_OPTS,1
+INS_HNTCH_REF,0.125018  # MOT_THST_HOVER * SQUARE(min_freq / hover_freq)
```

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949544270833334%*

 * *Differences: {"'Components'": "{'Frame': {'Product': {'Manufacturer': 'Papa Seleckis', 'Model': 'Custom "*

 * *                 "Aluminiumm', 'Version': '30 Kg payload'}}, 'RC Transmitter': {'Notes': "*

 * *                 "'integrated in RC controller'}, 'Telemetry': {'FC Connection': {'Type': "*

 * *                 "'SERIAL1', 'Protocol': 'MAVLink2'}}, 'Battery Monitor': {'Product': {'Model': "*

 * *                 "'HX4-06008', 'URL': "*

 * *                 "'https://docs.cubepilot.org/user-guides/autopilot/the-cube-user-manual#power-mod […]*

```diff
@@ -1,13 +1,13 @@
 {
     "Components": {
         "Battery": {
             "Notes": "Normal battery 3.5 kg.",
             "Product": {
-                "Manufacturer": "TATTO",
+                "Manufacturer": "gensTattu",
                 "Model": "6C 30000mah",
                 "URL": "https://genstattu.com/tattu-g-tech-30000mah-6s-22-2v-25c-lipo-battery-pack-with-as150u-f-plug/",
                 "Version": "AS150U-F"
             },
             "Specifications": {
                 "Chemistry": "LipoHV",
                 "Number of cells": 6,
@@ -15,26 +15,26 @@
                 "Volt per cell low": 3.6,
                 "Volt per cell max": 4.2
             }
         },
         "Battery Monitor": {
             "FC Connection": {
                 "Protocol": "Analog Voltage and Current",
-                "Type": "I2C1"
+                "Type": "Analog"
             },
             "Firmware": {
-                "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Type": "",
+                "Version": ""
             },
             "Notes": "Voltage is done via the flight controller. Current is done via the ESC.",
             "Product": {
                 "Manufacturer": "CubePilot",
-                "Model": "CubeOrange",
-                "URL": "https://www.robotshop.com/products/cubepilot-the-cube-orange-standard-set-ads-b-carrier-board",
-                "Version": "3"
+                "Model": "HX4-06008",
+                "URL": "https://docs.cubepilot.org/user-guides/autopilot/the-cube-user-manual#power-module-connection",
+                "Version": "PB01A21"
             }
         },
         "ESC": {
             "FC Connection": {
                 "Protocol": "Normal",
                 "Type": "Main Out"
             },
@@ -62,18 +62,18 @@
                 "URL": "https://www.robotshop.com/products/cubepilot-the-cube-orange-standard-set-ads-b-carrier-board",
                 "Version": "1.0"
             }
         },
         "Frame": {
             "Notes": "Frame is custom, X type frame, the middle is welded. Arm lenght is 1950mm.",
             "Product": {
-                "Manufacturer": "Aluminiumm",
-                "Model": "Custom",
+                "Manufacturer": "Papa Seleckis",
+                "Model": "Custom Aluminiumm",
                 "URL": "",
-                "Version": ""
+                "Version": "30 Kg payload"
             }
         },
         "GNSS receiver": {
             "FC Connection": {
                 "Protocol": "DroneCAN",
                 "Type": "CAN1"
             },
@@ -144,26 +144,26 @@
             }
         },
         "RC Transmitter": {
             "Firmware": {
                 "Type": "",
                 "Version": ""
             },
-            "Notes": "",
+            "Notes": "integrated in RC controller",
             "Product": {
                 "Manufacturer": "",
                 "Model": "",
                 "URL": "",
                 "Version": ""
             }
         },
         "Telemetry": {
             "FC Connection": {
-                "Protocol": "MAVLink High Latency",
-                "Type": "SERIAL2"
+                "Protocol": "MAVLink2",
+                "Type": "SERIAL1"
             },
             "Firmware": {
                 "Type": "",
                 "Version": ""
             },
             "Notes": "High range and strenght telemetry.",
             "Product": {
```

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 SERVO3_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO3_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO3_TRIM,1000  # Use the full available 1000-2000 DShot range
 SERVO4_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO4_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO4_TRIM,1000  # Use the full available 1000-2000 DShot range
 TKOFF_RPM_MIN,1400  # Our motors should idle at around 1400 RPM, see https://ardupilot.org/copter/docs/tkoff-rpm-min.html
-
 MOT_HOVER_LEARN,2
```

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json` & `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json`

 * *Files identical despite different names*

